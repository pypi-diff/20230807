# Comparing `tmp/prefect-monte-carlo-0.1.0.tar.gz` & `tmp/prefect-monte-carlo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-monte-carlo/prefect-monte-carlo/dist/tmpuids5hf0/prefect-monte-carlo-0.1.0.tar", last modified: Fri Oct 14 22:05:04 2022, max compression
+gzip compressed data, was "/home/runner/work/prefect-monte-carlo/prefect-monte-carlo/dist/.tmp-q8xjcwmw/prefect-monte-carlo-0.2.0.tar", last modified: Mon Jul 24 16:17:33 2023, max compression
```

## Comparing `prefect-monte-carlo-0.1.0.tar` & `prefect-monte-carlo-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/circuit_breakers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2543 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)    12088 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-10-14 22:05:04.000000 prefect-monte-carlo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80049 2022-10-14 22:04:24.000000 prefect-monte-carlo-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/circuit_breakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:17:33.000000 prefect-monte-carlo-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/tests/test_circuit_breakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/tests/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-24 16:16:33.000000 prefect-monte-carlo-0.2.0/versioneer.py
```

### Comparing `prefect-monte-carlo-0.1.0/LICENSE` & `prefect-monte-carlo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-monte-carlo-0.1.0/PKG-INFO` & `prefect-monte-carlo-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-monte-carlo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prefect integrations for interacting with Monte Carlo.
 Home-page: https://github.com/PrefectHQ/prefect-monte-carlo
 Author: Prefect Technologies
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -20,14 +20,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-monte-carlo
 
+Visit the full docs [here](https://PrefectHQ.github.io/prefect-monte-carlo) to see additional examples and the API reference.
+
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-monte-carlo/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-monte-carlo?color=0052FF&labelColor=090422"></a>
     <a href="https://github.com/PrefectHQ/prefect-monte-carlo/" alt="Stars">
         <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-monte-carlo?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-monte-carlo/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-monte-carlo?color=0052FF&labelColor=090422" /></a>
@@ -70,27 +72,26 @@
 
 Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
 
 ### Write and run a flow
 #### Execute a query against the Monte Carlo GraphQL API
 ```python
 from prefect import flow
-from prefect_monte_carlo import execute_graphql_operation
+from prefect_monte_carlo.graphql import execute_graphql_operation
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 
 @flow
 def example_execute_query():
     monte_carlo_credentials = MonteCarloCredentials.load("my-mc-creds")
     result = execute_graphql_operation(
         monte_carlo_credentials=monte_carlo_credentials,
         operation="query getUser { getUser { email firstName lastName }}",
     )
-
-example_execute_query()
 ```
+
 #### Create or update Monte Carlo lineage
 ```python
 from prefect import flow
 from prefect.context import get_run_context
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 from prefect_monte_carlo.lineage import create_or_update_lineage, MonteCarloLineageNode
 
@@ -128,41 +129,49 @@
 
 #### Conditionally execute a flow based on a Monte Carlo circuit breaker rule
 ```python
 from prefect import flow
 from prefect_monte_carlo.circuit_breakers import skip_if_circuit_breaker_flipped
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 
+my_mc_creds = MonteCarloCredentials.load("my-mc-creds")
+rule_name = "myRule"
+
 @flow
 @skip_if_circuit_breaker_flipped(
-    monte_carlo_credentials=MonteCarloCredentials.load("my-mc-creds")
-    rule_uuid="7810b1ce-4dee-4f40-b14f-ced65c80aea9",
+    monte_carlo_credentials=my_mc_creds
+    rule_name=rule_name,
 )
 def conditional_flow():
     logger = get_run_logger()
     logger.info("If you see this, your circuit breaker rule was not breached!")
-
-conditional_flow()
 ```
 
 ## Resources
 
 If you encounter any bugs while using `prefect-monte-carlo`, feel free to open an issue in the [prefect-monte-carlo](https://github.com/PrefectHQ/prefect-monte-carlo) repository.
 
 If you have any questions or issues while using `prefect-monte-carlo`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to ⭐️ or watch [`prefect-monte-carlo`](https://github.com/PrefectHQ/prefect-monte-carlo) for updates too!
+Feel free to star or watch [`prefect-monte-carlo`](https://github.com/PrefectHQ/prefect-monte-carlo) for updates too!
 
-## Development
+## Contributing
 
-If you'd like to install a version of `prefect-monte-carlo` for development, clone the repository and perform an editable install with `pip`:
+If you'd like to help contribute to fix an issue or add a feature to `prefect-monte-carlo`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
-```bash
-git clone https://github.com/PrefectHQ/prefect-monte-carlo.git
-
-cd prefect-monte-carlo/
+Here are the steps:
 
+1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
+2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
+3. Install the repository and its dependencies:
+```
 pip install -e ".[dev]"
+```
+4. Make desired changes
+5. Add tests
+6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-monte-carlo/blob/main/CHANGELOG.md)
+7. Install `pre-commit` to perform quality checks prior to commit:
 
-# Install linting pre-commit hooks
+```
 pre-commit install
 ```
+8. `git commit`, `git push`, and create a pull request
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-monte-carlo-0.1.0/README.md` & `prefect-monte-carlo-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # prefect-monte-carlo
 
+Visit the full docs [here](https://PrefectHQ.github.io/prefect-monte-carlo) to see additional examples and the API reference.
+
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-monte-carlo/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-monte-carlo?color=0052FF&labelColor=090422"></a>
     <a href="https://github.com/PrefectHQ/prefect-monte-carlo/" alt="Stars">
         <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-monte-carlo?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-monte-carlo/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-monte-carlo?color=0052FF&labelColor=090422" /></a>
@@ -46,27 +48,26 @@
 
 Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
 
 ### Write and run a flow
 #### Execute a query against the Monte Carlo GraphQL API
 ```python
 from prefect import flow
-from prefect_monte_carlo import execute_graphql_operation
+from prefect_monte_carlo.graphql import execute_graphql_operation
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 
 @flow
 def example_execute_query():
     monte_carlo_credentials = MonteCarloCredentials.load("my-mc-creds")
     result = execute_graphql_operation(
         monte_carlo_credentials=monte_carlo_credentials,
         operation="query getUser { getUser { email firstName lastName }}",
     )
-
-example_execute_query()
 ```
+
 #### Create or update Monte Carlo lineage
 ```python
 from prefect import flow
 from prefect.context import get_run_context
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 from prefect_monte_carlo.lineage import create_or_update_lineage, MonteCarloLineageNode
 
@@ -104,41 +105,49 @@
 
 #### Conditionally execute a flow based on a Monte Carlo circuit breaker rule
 ```python
 from prefect import flow
 from prefect_monte_carlo.circuit_breakers import skip_if_circuit_breaker_flipped
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 
+my_mc_creds = MonteCarloCredentials.load("my-mc-creds")
+rule_name = "myRule"
+
 @flow
 @skip_if_circuit_breaker_flipped(
-    monte_carlo_credentials=MonteCarloCredentials.load("my-mc-creds")
-    rule_uuid="7810b1ce-4dee-4f40-b14f-ced65c80aea9",
+    monte_carlo_credentials=my_mc_creds
+    rule_name=rule_name,
 )
 def conditional_flow():
     logger = get_run_logger()
     logger.info("If you see this, your circuit breaker rule was not breached!")
-
-conditional_flow()
 ```
 
 ## Resources
 
 If you encounter any bugs while using `prefect-monte-carlo`, feel free to open an issue in the [prefect-monte-carlo](https://github.com/PrefectHQ/prefect-monte-carlo) repository.
 
 If you have any questions or issues while using `prefect-monte-carlo`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to ⭐️ or watch [`prefect-monte-carlo`](https://github.com/PrefectHQ/prefect-monte-carlo) for updates too!
+Feel free to star or watch [`prefect-monte-carlo`](https://github.com/PrefectHQ/prefect-monte-carlo) for updates too!
 
-## Development
+## Contributing
 
-If you'd like to install a version of `prefect-monte-carlo` for development, clone the repository and perform an editable install with `pip`:
+If you'd like to help contribute to fix an issue or add a feature to `prefect-monte-carlo`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
-```bash
-git clone https://github.com/PrefectHQ/prefect-monte-carlo.git
-
-cd prefect-monte-carlo/
+Here are the steps:
 
+1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
+2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
+3. Install the repository and its dependencies:
+```
 pip install -e ".[dev]"
+```
+4. Make desired changes
+5. Add tests
+6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-monte-carlo/blob/main/CHANGELOG.md)
+7. Install `pre-commit` to perform quality checks prior to commit:
 
-# Install linting pre-commit hooks
+```
 pre-commit install
 ```
+8. `git commit`, `git push`, and create a pull request
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo/circuit_breakers.py` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo/circuit_breakers.py`

 * *Files identical despite different names*

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo/credentials.py` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         from prefect_monte_carlo.credentials import MonteCarloCredentials
         montecarlo_credentials_block = MonteCarloCredentials.load("BLOCK_NAME")
         ```
     """
 
     _block_type_name = "Monte Carlo Credentials"
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/5OqrPNRdLMvqZzxo9f6Z25/f920dff0f1201fc014b0b083a6d2fdb1/image.png?h=250"  # noqa
+    _documentation_url = "https://prefecthq.github.io/prefect-monte-carlo/credentials/#prefect_monte_carlo.credentials.MonteCarloCredentials"  # noqa
 
     api_key: SecretStr = Field(
         default=...,
         title="API Key",
         description="The token to authenticate with Monte Carlo's GraphQL API.",
     )
```

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo/graphql.py` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo/graphql.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Returns:
         The results of the GraphQL operation as a `box.Box` object.
 
     Example:
         Executes a simple GraphQL query against the Monte Carlo GraphQL API.
         ```python
         from prefect import flow
-        from prefect_monte_carlo import execute_graphql_operation
+        from prefect_monte_carlo.graphql import execute_graphql_operation
         from prefect_monte_carlo.credentials import MonteCarloCredentials
 
         @flow
         def example_execute_query():
             monte_carlo_credentials = MonteCarloCredentials.load(
                 "my-montecarlo-credentials"
             )
```

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo/lineage.py` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo/lineage.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 resource_name="some_resource_name",
                 tags=[{"propertyName": "dataset_owner", "propertyValue": "owner_name"}],
             )
 
             # `create_or_update_lineage` is a flow, so this will be a subflow run
             # `extra_tags` are added to both the `source` and `destination` nodes
             create_or_update_lineage(
-                monte_carlo_credentials=MonteCarloCredentials.load("my-mc-creds)
+                monte_carlo_credentials=MonteCarloCredentials.load("my-mc-creds")
                 source=source,
                 destination=destination,
                 expire_at=datetime.now() + timedelta(days=10),
                 extra_tags=[
                     {"propertyName": "flow_run_name", "propertyValue": flow_run_name}
                 ]
             )
@@ -137,24 +137,27 @@
         f"{monte_carlo_credentials.catalog_url}/{destination_node_mcon}/table"
     )
     logger.info(
         "Created or updated a destination lineage node %s", destination_node_url
     )
 
     # edge between source and destination nodes
-    edge_id = await create_or_update_lineage_edge(
+    job_timestamp = await create_or_update_lineage_edge(
         monte_carlo_credentials=monte_carlo_credentials,
         source=source,
         destination=destination,
         expire_at=expire_at,
     )
 
-    logger.info(f"Created or updated a destination lineage edge: {edge_id}")
+    logger.info(
+        f"Created or updated a destination a lineage edge between "
+        f"{source_node_url} and {destination_node_url}"
+    )
 
-    return edge_id
+    return job_timestamp
 
 
 @task(
     retries=2,
     retry_delay_seconds=3,
     description="Create or update a Monte Carlo lineage node via the GraphQL API.",
 )
@@ -243,27 +246,27 @@
     description="Create or update a Monte Carlo lineage edge via the GraphQL API.",
 )
 async def create_or_update_lineage_edge(
     monte_carlo_credentials: MonteCarloCredentials,
     source: MonteCarloLineageNode,
     destination: MonteCarloLineageNode,
     expire_at: Optional[datetime] = None,
-) -> str:
+) -> int:
     """Create or update a Monte Carlo lineage edge via the GraphQL API.
 
     Args:
         source: The source node of the lineage edge.
         destination: The destination node of the lineage edge.
         monte_carlo_credentials: The Monte Carlo credentials block used to generate
             an authenticated GraphQL API client via pycarlo.
         expire_at: The time at which the lineage edge should expire. If not provided,
             the lineage edge will expire after 1 day.
 
     Returns:
-        The `edgeId` of the created or updated lineage edge.
+        The timestamp of the job that created or updated the lineage edge.
 
     Example:
         Create a lineage edge between a source table and a destination table:
         ```python
         from prefect import flow
         from prefect_monte_carlo.credentials import MonteCarloCredentials
         from prefect_monte_carlo.lineage import (
@@ -316,15 +319,15 @@
                 objectId: $source_object_id
                 objectType: $source_object_type
                 resourceName: $source_resource_name
             }
             expireAt: $expire_at
             ){
             edge{
-                edgeId
+                jobTs
             }
             }
         }
         """
 
     variables = dict(
         destination_object_id=destination.object_id,
@@ -334,10 +337,10 @@
         source_object_type=source.object_type,
         source_resource_name=source.resource_name,
         expire_at=expire_at.isoformat() if expire_at else None,
     )
 
     response = client(query=query, variables=variables)
 
-    edge_id = response["create_or_update_lineage_edge"]["edge"]["edge_id"]
+    job_timestamp = response["create_or_update_lineage_edge"]["edge"]["jobTs"]
 
-    return edge_id
+    return job_timestamp
```

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo/resources.py` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo/resources.py`

 * *Files identical despite different names*

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo/utilities.py` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-monte-carlo-0.1.0/prefect_monte_carlo.egg-info/PKG-INFO` & `prefect-monte-carlo-0.2.0/prefect_monte_carlo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-monte-carlo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prefect integrations for interacting with Monte Carlo.
 Home-page: https://github.com/PrefectHQ/prefect-monte-carlo
 Author: Prefect Technologies
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -20,14 +20,16 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-monte-carlo
 
+Visit the full docs [here](https://PrefectHQ.github.io/prefect-monte-carlo) to see additional examples and the API reference.
+
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-monte-carlo/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-monte-carlo?color=0052FF&labelColor=090422"></a>
     <a href="https://github.com/PrefectHQ/prefect-monte-carlo/" alt="Stars">
         <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-monte-carlo?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-monte-carlo/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-monte-carlo?color=0052FF&labelColor=090422" /></a>
@@ -70,27 +72,26 @@
 
 Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
 
 ### Write and run a flow
 #### Execute a query against the Monte Carlo GraphQL API
 ```python
 from prefect import flow
-from prefect_monte_carlo import execute_graphql_operation
+from prefect_monte_carlo.graphql import execute_graphql_operation
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 
 @flow
 def example_execute_query():
     monte_carlo_credentials = MonteCarloCredentials.load("my-mc-creds")
     result = execute_graphql_operation(
         monte_carlo_credentials=monte_carlo_credentials,
         operation="query getUser { getUser { email firstName lastName }}",
     )
-
-example_execute_query()
 ```
+
 #### Create or update Monte Carlo lineage
 ```python
 from prefect import flow
 from prefect.context import get_run_context
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 from prefect_monte_carlo.lineage import create_or_update_lineage, MonteCarloLineageNode
 
@@ -128,41 +129,49 @@
 
 #### Conditionally execute a flow based on a Monte Carlo circuit breaker rule
 ```python
 from prefect import flow
 from prefect_monte_carlo.circuit_breakers import skip_if_circuit_breaker_flipped
 from prefect_monte_carlo.credentials import MonteCarloCredentials
 
+my_mc_creds = MonteCarloCredentials.load("my-mc-creds")
+rule_name = "myRule"
+
 @flow
 @skip_if_circuit_breaker_flipped(
-    monte_carlo_credentials=MonteCarloCredentials.load("my-mc-creds")
-    rule_uuid="7810b1ce-4dee-4f40-b14f-ced65c80aea9",
+    monte_carlo_credentials=my_mc_creds
+    rule_name=rule_name,
 )
 def conditional_flow():
     logger = get_run_logger()
     logger.info("If you see this, your circuit breaker rule was not breached!")
-
-conditional_flow()
 ```
 
 ## Resources
 
 If you encounter any bugs while using `prefect-monte-carlo`, feel free to open an issue in the [prefect-monte-carlo](https://github.com/PrefectHQ/prefect-monte-carlo) repository.
 
 If you have any questions or issues while using `prefect-monte-carlo`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to ⭐️ or watch [`prefect-monte-carlo`](https://github.com/PrefectHQ/prefect-monte-carlo) for updates too!
+Feel free to star or watch [`prefect-monte-carlo`](https://github.com/PrefectHQ/prefect-monte-carlo) for updates too!
 
-## Development
+## Contributing
 
-If you'd like to install a version of `prefect-monte-carlo` for development, clone the repository and perform an editable install with `pip`:
+If you'd like to help contribute to fix an issue or add a feature to `prefect-monte-carlo`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
-```bash
-git clone https://github.com/PrefectHQ/prefect-monte-carlo.git
-
-cd prefect-monte-carlo/
+Here are the steps:
 
+1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
+2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
+3. Install the repository and its dependencies:
+```
 pip install -e ".[dev]"
+```
+4. Make desired changes
+5. Add tests
+6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-monte-carlo/blob/main/CHANGELOG.md)
+7. Install `pre-commit` to perform quality checks prior to commit:
 
-# Install linting pre-commit hooks
+```
 pre-commit install
 ```
+8. `git commit`, `git push`, and create a pull request
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-monte-carlo-0.1.0/setup.cfg` & `prefect-monte-carlo-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-monte-carlo-0.1.0/setup.py` & `prefect-monte-carlo-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-monte-carlo-0.1.0/versioneer.py` & `prefect-monte-carlo-0.2.0/versioneer.py`

 * *Files identical despite different names*

