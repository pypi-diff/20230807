# Comparing `tmp/pyairvisual-5.0.8.tar.gz` & `tmp/pyairvisual-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyairvisual-5.0.8.tar", max compression
+gzip compressed data, was "pyairvisual-5.0.9.tar", max compression
```

## Comparing `pyairvisual-5.0.8.tar` & `pyairvisual-5.0.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1077 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/LICENSE
--rw-r--r--   0        0        0     6758 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/README.md
--rw-r--r--   0        0        0      117 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/__init__.py
--rw-r--r--   0        0        0     2363 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/air_quality.py
--rw-r--r--   0        0        0     2825 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/cloud_api.py
--rw-r--r--   0        0        0       71 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/const.py
--rw-r--r--   0        0        0     1769 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/errors.py
--rw-r--r--   0        0        0     8950 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/node.py
--rw-r--r--   0        0        0     1412 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyairvisual/supported.py
--rw-r--r--   0        0        0     1505 2021-04-28 18:45:23.399017 pyairvisual-5.0.8/pyproject.toml
--rw-r--r--   0        0        0     7693 2021-04-28 18:45:35.361855 pyairvisual-5.0.8/setup.py
--rw-r--r--   0        0        0     7719 2021-04-28 18:45:35.362427 pyairvisual-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-07-27 18:33:53.332767 pyairvisual-5.0.9/LICENSE
+-rw-r--r--   0        0        0     6758 2021-07-27 18:33:53.332767 pyairvisual-5.0.9/README.md
+-rw-r--r--   0        0        0      117 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/__init__.py
+-rw-r--r--   0        0        0     2363 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/air_quality.py
+-rw-r--r--   0        0        0     2825 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/cloud_api.py
+-rw-r--r--   0        0        0       71 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/const.py
+-rw-r--r--   0        0        0     1769 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/errors.py
+-rw-r--r--   0        0        0     8950 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/node.py
+-rw-r--r--   0        0        0        0 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/py.typed
+-rw-r--r--   0        0        0     1412 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyairvisual/supported.py
+-rw-r--r--   0        0        0     1505 2021-07-27 18:33:53.336767 pyairvisual-5.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7693 2021-07-27 18:34:02.919636 pyairvisual-5.0.9/setup.py
+-rw-r--r--   0        0        0     7719 2021-07-27 18:34:02.920286 pyairvisual-5.0.9/PKG-INFO
```

### Comparing `pyairvisual-5.0.8/LICENSE` & `pyairvisual-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/README.md` & `pyairvisual-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/pyairvisual/air_quality.py` & `pyairvisual-5.0.9/pyairvisual/air_quality.py`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/pyairvisual/cloud_api.py` & `pyairvisual-5.0.9/pyairvisual/cloud_api.py`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/pyairvisual/errors.py` & `pyairvisual-5.0.9/pyairvisual/errors.py`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/pyairvisual/node.py` & `pyairvisual-5.0.9/pyairvisual/node.py`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/pyairvisual/supported.py` & `pyairvisual-5.0.9/pyairvisual/supported.py`

 * *Files identical despite different names*

### Comparing `pyairvisual-5.0.8/pyproject.toml` & `pyairvisual-5.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 multi_line_output = 3
 not_skip = "__init__.py"
 sections = "FUTURE,STDLIB,INBETWEENS,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 use_parentheses = true
 
 [tool.poetry]
 name = "pyairvisual"
-version = "5.0.8"
+version = "5.0.9"
 description = "A simple API for AirVisual air quality data"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/pyairvisual"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `pyairvisual-5.0.8/setup.py` & `pyairvisual-5.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.7.4,<4.0.0', 'numpy>=1.18.2,<2.0.0', 'pysmb>=1.2.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyairvisual',
-    'version': '5.0.8',
+    'version': '5.0.9',
     'description': 'A simple API for AirVisual air quality data',
     'long_description': '# ☀️ pyairvisual: a thin Python wrapper for the AirVisual© API\n\n[![CI](https://github.com/bachya/pyairvisual/workflows/CI/badge.svg)](https://github.com/bachya/pyairvisual/actions)\n[![PyPi](https://img.shields.io/pypi/v/pyairvisual.svg)](https://pypi.python.org/pypi/pyairvisual)\n[![Version](https://img.shields.io/pypi/pyversions/pyairvisual.svg)](https://pypi.python.org/pypi/pyairvisual)\n[![License](https://img.shields.io/pypi/l/pyairvisual.svg)](https://github.com/bachya/pyairvisual/blob/master/LICENSE)\n[![Code Coverage](https://codecov.io/gh/bachya/pyairvisual/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/pyairvisual)\n[![Maintainability](https://api.codeclimate.com/v1/badges/948e4e3c84e5c49826f1/maintainability)](https://codeclimate.com/github/bachya/pyairvisual/maintainability)\n[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)\n\n`pyairvisual` is a simple, clean, well-tested library for interacting with\n[AirVisual](https://www.airvisual.com/) to retrieve air quality information.\n\n- [Python Versions](#python-versions)\n- [Installation](#installation)\n- [API Key](#api-key)\n  * [Community](#community)\n  * [Startup](#startup)\n  * [Enterprise](#enterprise)\n- [Usage](#usage)\n  * [Using the Cloud API](#using-the-cloud-api)\n  * [Working with Node/Pro Units](#working-with-node-pro-units)\n- [Contributing](#contributing)\n\n# Python Versions\n\n`pyairvisual` is currently supported on:\n\n* Python 3.6\n* Python 3.7\n* Python 3.8\n* Python 3.9\n\n# Installation\n\n```python\npip install pyairvisual\n```\n\n# API Key\n\nYou can get an AirVisual API key from\n[the AirVisual API site](https://www.airvisual.com/user/api). Depending on\nthe plan you choose, more functionality will be available from the API:\n\n## Community\n\nThe Community Plan gives access to:\n\n* List supported countries\n* List supported states\n* List supported cities\n* Get data from the nearest city based on IP address\n* Get data from the nearest city based on latitude/longitude\n* Get data from a specific city\n\n## Startup\n\nThe Startup Plan gives access to:\n\n* List supported stations in a city\n* Get data from the nearest station based on IP address\n* Get data from the nearest station based on latitude/longitude\n* Get data from a specific station\n\n## Enterprise\n\nThe Enterprise Plan gives access to:\n\n* Get a global city ranking of air quality\n\n# Usage\n\n## Using the Cloud API\n\n```python\nimport asyncio\n\nfrom pyairvisual import CloudAPI\n\n\nasync def main() -> None:\n    """Run!"""\n    cloud_api = CloudAPI("<YOUR_AIRVISUAL_API_KEY>")\n\n    # Get data based on the city nearest to your IP address:\n    data = await cloud_api.air_quality.nearest_city()\n\n    # ...or get data based on the city nearest to a latitude/longitude:\n    data = await cloud_api.air_quality.nearest_city(\n        latitude=39.742599, longitude=-104.9942557\n    )\n\n    # ...or get it explicitly:\n    data = await cloud_api.air_quality.city(\n        city="Los Angeles", state="California", country="USA"\n    )\n\n    # If you have the appropriate API key, you can also get data based on\n    # station (nearest or explicit):\n    data = await cloud_api.air_quality.nearest_station()\n    data = await cloud_api.air_quality.nearest_station(\n        latitude=39.742599, longitude=-104.9942557\n    )\n    data = await cloud_api.air_quality.station(\n        station="US Embassy in Beijing",\n        city="Beijing",\n        state="Beijing",\n        country="China",\n    )\n\n    # With the appropriate API key, you can get an air quality ranking:\n    data = await cloud_api.air_quality.ranking()\n\n    # pyairvisual gives you several methods to look locations up:\n    countries = await cloud_api.supported.countries()\n    states = await cloud_api.supported.states("USA")\n    cities = await cloud_api.supported.cities("USA", "Colorado")\n    stations = await cloud_api.supported.stations("USA", "Colorado", "Denver")\n\n\nasyncio.run(main())\n```\n\nBy default, the library creates a new connection to AirVisual with each coroutine. If\nyou are calling a large number of coroutines (or merely want to squeeze out every second\nof runtime savings possible), an\n[`aiohttp`](https://github.com/aio-libs/aiohttp) `ClientSession` can be used for connection\npooling:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pyairvisual import CloudAPI\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        cloud_api = CloudAPI("<YOUR_AIRVISUAL_API_KEY>", session=session)\n\n        # ...\n\n\nasyncio.run(main())\n```\n\n## Working with Node/Pro Units\n\n`pyairvisual` also allows users to interact with\n[Node/Pro units](https://www.airvisual.com/air-quality-monitor), both via the cloud API:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pyairvisual import CloudAPI\n\n\nasync def main() -> None:\n    """Run!"""\n    cloud_api = CloudAPI("<YOUR_AIRVISUAL_API_KEY>")\n\n    # The Node/Pro unit ID can be retrieved from the "API" section of the cloud\n    # dashboard:\n    data = await cloud_api.node.get_by_node_id("<NODE_ID>")\n\n\nasyncio.run(main())\n```\n\n...or over the local network via Samba (the unit password can be found\n[on the device itself](https://support.airvisual.com/en/articles/3029331-download-the-airvisual-node-pro-s-data-using-samba)):\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom pyairvisual.node import NodeSamba\n\n\nasync def main() -> None:\n    """Run!"""\n    async with NodeSamba("<IP_ADDRESS_OR_HOST>", "<PASSWORD>") as node:\n        measurements = node.async_get_latest_measurements()\n\n        # Can take some optional parameters:\n        #   1. include_trends: include trends (defaults to True)\n        #   2. measurements_to_use: the number of measurements to use when calculating\n        #      trends (defaults to -1, which means "use all measurements")\n        history = node.async_get_history()\n\n\nasyncio.run(main())\n```\n\nCheck out the examples, the tests, and the source files themselves for method\nsignatures and more examples.\n\n# Contributing\n\n1. [Check for open features/bugs](https://github.com/bachya/pyairvisual/issues)\n  or [initiate a discussion on one](https://github.com/bachya/pyairvisual/issues/new).\n2. [Fork the repository](https://github.com/bachya/pyairvisual/fork).\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `script/test`\n9. Update `README.md` with any new documentation.\n10. Add yourself to `AUTHORS.md`.\n11. Submit a pull request!\n',
     'author': 'Aaron Bach',
     'author_email': 'bachya1208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/bachya/pyairvisual',
```

### Comparing `pyairvisual-5.0.8/PKG-INFO` & `pyairvisual-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairvisual
-Version: 5.0.8
+Version: 5.0.9
 Summary: A simple API for AirVisual air quality data
 Home-page: https://github.com/bachya/pyairvisual
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.6.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

