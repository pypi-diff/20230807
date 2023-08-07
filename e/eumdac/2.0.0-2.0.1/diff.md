# Comparing `tmp/eumdac-2.0.0.tar.gz` & `tmp/eumdac-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eumdac-2.0.0.tar", last modified: Mon Oct 17 11:51:08 2022, max compression
+gzip compressed data, was "eumdac-2.0.1.tar", last modified: Mon Jan 23 16:03:25 2023, max compression
```

## Comparing `eumdac-2.0.0.tar` & `eumdac-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 rdelahoz (11061) met        (207)        0 2022-10-17 11:51:08.041924 eumdac-2.0.0/
--rw-r--r--   0 rdelahoz (11061) met        (207)      237 2022-07-08 07:51:51.000000 eumdac-2.0.0/AUTHORS.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)     1169 2022-07-08 07:51:51.000000 eumdac-2.0.0/LICENSE.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)    10142 2022-07-08 07:51:51.000000 eumdac-2.0.0/LICENSE_APACHE_v2.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)     1049 2022-07-08 07:51:51.000000 eumdac-2.0.0/LICENSE_MIT.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)     4868 2022-10-17 11:51:08.040328 eumdac-2.0.0/PKG-INFO
--rw-r--r--   0 rdelahoz (11061) met        (207)     3919 2022-10-17 09:54:57.000000 eumdac-2.0.0/README.md
-drwxr-xr-x   0 rdelahoz (11061) met        (207)        0 2022-10-17 11:51:07.990205 eumdac-2.0.0/eumdac/
--rw-r--r--   0 rdelahoz (11061) met        (207)     1226 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/__init__.py
--rw-r--r--   0 rdelahoz (11061) met        (207)      393 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/__version__.py
--rw-r--r--   0 rdelahoz (11061) met        (207)    47962 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/cli.py
--rw-r--r--   0 rdelahoz (11061) met        (207)    11223 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/collection.py
--rw-r--r--   0 rdelahoz (11061) met        (207)      419 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/config.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     7525 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/customisation.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     3681 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/datastore.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     5155 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/datatailor.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     3291 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/download_app.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     1277 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/endpoints.ini
--rw-r--r--   0 rdelahoz (11061) met        (207)     1023 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/errors.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     1397 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/fake.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     1231 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/job_id.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     3871 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/logging.py
--rw-r--r--   0 rdelahoz (11061) met        (207)    11211 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/order.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     8941 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/product.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     2985 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/subscription.py
--rw-r--r--   0 rdelahoz (11061) met        (207)    25684 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/tailor_app.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     5103 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/tailor_models.py
--rw-r--r--   0 rdelahoz (11061) met        (207)     3773 2022-10-17 09:54:57.000000 eumdac-2.0.0/eumdac/token.py
-drwxr-xr-x   0 rdelahoz (11061) met        (207)        0 2022-10-17 11:51:08.032425 eumdac-2.0.0/eumdac.egg-info/
--rw-r--r--   0 rdelahoz (11061) met        (207)     4868 2022-10-17 11:51:07.000000 eumdac-2.0.0/eumdac.egg-info/PKG-INFO
--rw-r--r--   0 rdelahoz (11061) met        (207)      649 2022-10-17 11:51:07.000000 eumdac-2.0.0/eumdac.egg-info/SOURCES.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)        1 2022-10-17 11:51:07.000000 eumdac-2.0.0/eumdac.egg-info/dependency_links.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)       42 2022-10-17 11:51:07.000000 eumdac-2.0.0/eumdac.egg-info/entry_points.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)       96 2022-10-17 11:51:07.000000 eumdac-2.0.0/eumdac.egg-info/requires.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)        7 2022-10-17 11:51:07.000000 eumdac-2.0.0/eumdac.egg-info/top_level.txt
--rw-r--r--   0 rdelahoz (11061) met        (207)       38 2022-10-17 11:51:08.043812 eumdac-2.0.0/setup.cfg
--rw-r--r--   0 rdelahoz (11061) met        (207)     1508 2022-10-17 09:54:57.000000 eumdac-2.0.0/setup.py
+drwxr-xr-x   0 rdelahoz (11061) met        (207)        0 2023-01-23 16:03:25.389499 eumdac-2.0.1/
+-rw-r--r--   0 rdelahoz (11061) met        (207)      237 2022-07-08 07:51:51.000000 eumdac-2.0.1/AUTHORS.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1169 2022-07-08 07:51:51.000000 eumdac-2.0.1/LICENSE.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)    10142 2022-07-08 07:51:51.000000 eumdac-2.0.1/LICENSE_APACHE_v2.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1049 2022-07-08 07:51:51.000000 eumdac-2.0.1/LICENSE_MIT.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)     4964 2023-01-23 16:03:25.387451 eumdac-2.0.1/PKG-INFO
+-rw-r--r--   0 rdelahoz (11061) met        (207)     4015 2023-01-23 15:55:27.000000 eumdac-2.0.1/README.md
+drwxr-xr-x   0 rdelahoz (11061) met        (207)        0 2023-01-23 16:03:25.336475 eumdac-2.0.1/eumdac/
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1226 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/__init__.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)      393 2023-01-23 15:55:27.000000 eumdac-2.0.1/eumdac/__version__.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)    50581 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/cli.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)    10714 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/collection.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)      241 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/common.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)      419 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/config.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     7200 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/customisation.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     4093 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/datastore.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     4695 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/datatailor.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     3302 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/download_app.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1277 2023-01-02 14:33:46.000000 eumdac-2.0.1/eumdac/endpoints.ini
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1118 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/errors.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1397 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/fake.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1231 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/job_id.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     3871 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/logging.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)    11211 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/order.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     8568 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/product.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     2865 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/subscription.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)    25684 2022-10-17 09:54:57.000000 eumdac-2.0.1/eumdac/tailor_app.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     5222 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/tailor_models.py
+-rw-r--r--   0 rdelahoz (11061) met        (207)     3862 2023-01-23 15:26:42.000000 eumdac-2.0.1/eumdac/token.py
+drwxr-xr-x   0 rdelahoz (11061) met        (207)        0 2023-01-23 16:03:25.379127 eumdac-2.0.1/eumdac.egg-info/
+-rw-r--r--   0 rdelahoz (11061) met        (207)     4964 2023-01-23 16:03:25.000000 eumdac-2.0.1/eumdac.egg-info/PKG-INFO
+-rw-r--r--   0 rdelahoz (11061) met        (207)      666 2023-01-23 16:03:25.000000 eumdac-2.0.1/eumdac.egg-info/SOURCES.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)        1 2023-01-23 16:03:25.000000 eumdac-2.0.1/eumdac.egg-info/dependency_links.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)       42 2023-01-23 16:03:25.000000 eumdac-2.0.1/eumdac.egg-info/entry_points.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)       96 2023-01-23 16:03:25.000000 eumdac-2.0.1/eumdac.egg-info/requires.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)        7 2023-01-23 16:03:25.000000 eumdac-2.0.1/eumdac.egg-info/top_level.txt
+-rw-r--r--   0 rdelahoz (11061) met        (207)       38 2023-01-23 16:03:25.391584 eumdac-2.0.1/setup.cfg
+-rw-r--r--   0 rdelahoz (11061) met        (207)     1508 2023-01-02 14:33:46.000000 eumdac-2.0.1/setup.py
```

### Comparing `eumdac-2.0.0/LICENSE.txt` & `eumdac-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/LICENSE_APACHE_v2.txt` & `eumdac-2.0.1/LICENSE_APACHE_v2.txt`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/LICENSE_MIT.txt` & `eumdac-2.0.1/LICENSE_MIT.txt`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/PKG-INFO` & `eumdac-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eumdac
-Version: 2.0.0
+Version: 2.0.1
 Summary: EUMETSAT Data Access Client
 Home-page: https://gitlab.eumetsat.int/eumetlab/data-services/eumdac
 Author: EUMETSAT
 Author-email: ops@eumetsat.int
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -73,14 +73,15 @@
 ## Authors
 * [**Carlos Horn**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Ben Loveday**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Niklas Jordan**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Paulo Carmo**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Christopher Saloman**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Matthias Schwarz**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
+* [**Joaquin Rodríguez-Guerra**](mailto://ops@eumetsat.int) - [EUMETSAT](https://eumetsat.int)
 * [**Rafa de la Hoz**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 
 ## Dependencies
 requests,   ver. 2.26.0, License: Apache-2.0 (LICENSE_APACHE_v2.txt), Copyright 2014 Kenneth Reitz,   info: https://anaconda.org/conda-forge/requests  \
 responses,  ver. 0.16.0, License: Apache-2.0 (LICENSE_APACHE_v2.txt), Copyright 2015 David Cramer,    info: https://anaconda.org/conda-forge/responses  \
 setuptools, ver. 58.0.4, License: MIT (LICENSE_MIT.txt),              Copyright 2020 Jason R. Coombs, info: https://anaconda.org/conda-forge/setuptools
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eumdac-2.0.0/README.md` & `eumdac-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 ## Authors
 * [**Carlos Horn**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Ben Loveday**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Niklas Jordan**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Paulo Carmo**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Christopher Saloman**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Matthias Schwarz**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
+* [**Joaquin Rodríguez-Guerra**](mailto://ops@eumetsat.int) - [EUMETSAT](https://eumetsat.int)
 * [**Rafa de la Hoz**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 
 ## Dependencies
 requests,   ver. 2.26.0, License: Apache-2.0 (LICENSE_APACHE_v2.txt), Copyright 2014 Kenneth Reitz,   info: https://anaconda.org/conda-forge/requests  \
 responses,  ver. 0.16.0, License: Apache-2.0 (LICENSE_APACHE_v2.txt), Copyright 2015 David Cramer,    info: https://anaconda.org/conda-forge/responses  \
 setuptools, ver. 58.0.4, License: MIT (LICENSE_MIT.txt),              Copyright 2020 Jason R. Coombs, info: https://anaconda.org/conda-forge/setuptools
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eumdac-2.0.0/eumdac/__init__.py` & `eumdac-2.0.1/eumdac/__init__.py`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/cli.py` & `eumdac-2.0.1/eumdac/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 import os
 import pathlib
 import re
 import shlex
 import signal
 import stat
 import sys
+import urllib
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import requests
 import yaml
 from requests.exceptions import HTTPError
 
 import eumdac
 from eumdac import DataStore, DataTailor
 from eumdac.collection import SearchResults
 from eumdac.config import get_config_dir, get_credentials_path
 from eumdac.download_app import DownloadApp
-from eumdac.errors import EumdacError
+from eumdac.errors import EumdacError, eumdac_raise_for_status
 from eumdac.fake import FakeDataStore, FakeDataTailor  # type: ignore
 from eumdac.logging import gen_table_printer, init_logger, logger
 from eumdac.order import Order, all_order_filenames, resolve_order
-from eumdac.product import Product
+from eumdac.product import Product, ProductError
 from eumdac.tailor_app import TailorApp
 from eumdac.tailor_models import Chain
 from eumdac.token import AccessToken, AnonymousAccessToken
-
-from .__version__ import __documentation__, __title__, __version__  # noqa
+import eumdac.common
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Any, Callable, Collection, Dict, Iterator, Optional, Tuple, Union
 
     if sys.version_info < (3, 9):
         from typing import Iterable, Sequence
     else:
@@ -146,27 +146,37 @@
             return itertools.islice(chained_it, self.limit)
         return chained_it
 
     def __contains__(self, item: object) -> bool:
         raise NotImplementedError()
 
 
-def _search(args: argparse.Namespace) -> Collection[Product]:
+def _search(args: argparse.Namespace) -> Tuple[Collection[Product], int]:
     """given search query arguments will return the list of matching products"""
     datastore = get_datastore(args, anonymous_allowed=True)
     query_results = []
     start = args.dtstart
     end = args.dtend
     if args.dtend:
         if not (end.hour or end.minute or end.second):
             end = end + timedelta(hours=23, minutes=59, seconds=59)
             logger.warning("As no time was given in -e/--end, it was set to 23:59:59.")
     if args.time_range:
         start, end = args.time_range
 
+    # See https://docs.opengeospatial.org/is/13-026r9/13-026r9.html#20 for the mathematical notation expected by the publication filter
+    if args.publication_after and args.publication_before:
+        publication = f"[{args.publication_after.isoformat(timespec='milliseconds')}Z,{args.publication_before.isoformat(timespec='milliseconds')}Z]"
+    elif args.publication_after:
+        publication = f"[{args.publication_after.isoformat(timespec='milliseconds')}Z"
+    elif args.publication_before:
+        publication = f"{args.publication_before.isoformat(timespec='milliseconds')}Z]"
+    else:
+        publication = None
+
     sort_query = None
     if args.sort:
         if args.sort == "ingestion":
             sort_prefix = "publicationDate,,"
         elif args.sort == "sensing":
             sort_prefix = "start,time,"
         else:
@@ -177,14 +187,15 @@
         if args.asc:
             direction = 1
         sort_query = f"{sort_prefix}{direction}"
 
     _query = {
         "dtstart": start,
         "dtend": end,
+        "publication": publication,
         "bbox": args.bbox,
         "geo": args.geo,
         "sat": args.sat,
         "sort": sort_query,
         "cycle": args.cycle,
         "orbit": args.orbit,
         "relorbit": args.relorbit,
@@ -193,46 +204,51 @@
     }
 
     query = {key: value for key, value in _query.items() if value is not None}
     bbox = query.pop("bbox", None)
     if bbox is not None:
         query["bbox"] = ",".join(map(str, bbox))
 
+    products: Collection[Product] = []
+    num_products: int = 0
     for collection_id in args.collection:
-        collection = datastore.get_collection(collection_id)
-        query_results.append(collection.search(**query))
-
-    return ProductIterables(query_results, args.limit, query)
+        try:
+            collection = datastore.get_collection(collection_id)
+            query_results.append(collection.search(**query))
+            products = ProductIterables(query_results, args.limit, query)
+            # Check the number of products to execute the search
+            num_products = len(products)
+        except Exception as err:
+            datastore.check_collection_id(collection_id)
+            raise
+    return products, num_products
 
 
 def search(args: argparse.Namespace) -> None:
     """eumdac search entrypoint"""
+
     if args.time_range and (args.dtstart or args.dtend):
         raise ValueError("You can't combine --time-range and --start/--end.")
 
-    products_query = _search(args)
-    products_count = len(products_query)
+    products_query, products_count = _search(args)
 
-    limit = args.limit or 10
+    limit = args.limit or 10000
     products = itertools.islice(products_query, limit)
     if products_count < 1:
         logger.error(f"No products were found for the given search parameters")
         return
-
     if products_count > limit:
-        # show a warning through stderr only when more than 10
+        # show a warning through stderr only when more than 10000
         # products would be shown and limit keyword is not used.
-        logger.warning(f"By default, only 10 of {products_count} products are displayed.")
+        logger.warning(f"By default, only 10000 of {products_count} products are displayed.")
         logger.warning("Please use --limit to increase the number of products if necessary.")
-
     if products_count > 10000:
         logger.error(
             "Notice: EUMETSATs DataStore APIs allow a maximum of 10.000 items in a single request. If more than 10.000 items are needed, please split your requests."
         )
-
     for product in products:
         CRLF = "\r\n"
         logger.info(str(product).replace(CRLF, "-"))
 
 
 class AngrySigIntHandler:
     """class that will block a SigInt `max_block` times before exiting the program"""
@@ -249,108 +265,131 @@
         logger.warning(
             "Currently shutting down. "
             f"Interrupt {self.max_block - self.ints_received + 1} "
             "more times to forcefully shutdown."
         )
 
 
-def safe_run(app: Any, force: bool = False) -> None:
+def safe_run(
+    app: Any, collection: Optional[str] = None, num_products: int = -1, force: bool = False
+) -> None:
     """wrapper around app.run() for exception handling and logging"""
 
-    num_products = len(list(app.order.iter_product_info()))
-    plural = "" if num_products == 1 else "s"
-    logger.info(f"Processing {num_products} product{plural}.")
+    if num_products < 0:
+        num_products = len(list(app.order.iter_product_info()))
+        plural = "" if num_products == 1 else "s"
+        logger.info(f"Processing {num_products} product{plural}.")
     (chain,) = app.order.get_dict_entries("chain")
-
     if chain:
-        plural = "It" if num_products == 1 else "They"
-        logger.info(f"{plural} will be customized with the following parameters:")
+        plural = "" if num_products == 1 else "s"
+        logger.info(f"Product{plural} will be customized with the following parameters:")
         for line in yaml.dump(chain).splitlines():
             logger.info(f"   {line}")
-    if num_products >= 10 and not force:
-        user_in = input("Do you want to continue (Y/n)?")
-        if user_in.lower() == "n":
-            return
+
     logger.info(f"Using order: {app.order}")
     try:
         return app.run()
     except KeyboardInterrupt:
         signal.signal(signal.SIGINT, AngrySigIntHandler())
         logger.info("Received request to shut down.")
         logger.info("Finishing Threads..")
         app.shutdown()
         logger.info("Resume this order with the following command:")
         logger.info(f"$ eumdac order resume {app.order}")
         raise
+    except ProductError:
+        if collection:
+            app.datastore.check_collection_id(collection)
+            raise
+        else:
+            raise
     except Exception as e:
         logger.critical(f"Unexpected exception: {str(e)}")
         raise
 
 
 def download(args: argparse.Namespace) -> None:
     """eumdac download entrypoint"""
     order = Order()
     datastore = get_datastore(args)
 
     if not args.collection or len(args.collection) > 1:
-        raise ValueError("Please provide a (single) collection")
+        raise ValueError("Please provide a (single) collection.")
 
     if args.time_range and (args.dtstart or args.dtend):
         raise ValueError("You can't combine --time-range and --start/--end.")
 
     if args.time_range:
         args.dtstart = args.time_range[0]
         args.dtend = args.time_range[1]
 
     _collection = args.collection[0]
     if args.product and (args.dtstart or args.dtend):
         raise ValueError("Please provide either products or a time-range!")
 
+    products: Collection[Product]
     if args.product:
-        products: Collection[Product] = [
-            datastore.get_product(_collection, pid) for pid in args.product
-        ]
+        products = [datastore.get_product(_collection, pid) for pid in args.product]
     else:
-        products = _search(args)
+        products = _search(args)[0]
+
+    products_count = len(products)
+
+    if products_count > 10000:
+        logger.info(f"Processing 10000 out of the total {products_count} products.")
+        products = itertools.islice(products, 10000)  # type: ignore
+        products_count = 10000
+        logger.error(
+            "Notice: EUMETSATs DataStore APIs allow a maximum of 10.000 items in a single request. If more than 10.000 items are needed, please split your requests."
+        )
+    else:
+        plural = "" if products_count == 1 else "s"
+        logger.info(f"Processing {products_count} product{plural}.")
+
+    if products_count >= 10 and not args.yes:
+        user_in = input("Do you want to continue (Y/n)? ")
+        if user_in.lower() == "n":
+            return
 
     try:
         query = products.search_query  # type: ignore
     except AttributeError:
         query = None
 
     if args.tailor and args.chain:
         raise ValueError("Please provide either a tailor file or chain yaml string!")
     elif args.tailor or args.chain:
+        chain_config = ""
         if args.tailor:
             chain_config = args.tailor
         elif args.chain:
             chain_config = args.chain
         if chain_config.endswith(".yml") or chain_config.endswith(".yaml"):
             with open(chain_config, "r") as file:
                 try:
                     chain = yaml.safe_load(file)
                 except:
                     logger.error("YAML file is corrupted. Please, check the YAML syntax.")
-                    exit()
+                    sys.exit()
         else:
             chain_config = chain_config.strip()
             if not chain_config.startswith("{"):
                 chain_config = "{" + chain_config + "}"
             try:
                 chain = yaml.safe_load(chain_config)
             except:
                 logger.error("YAML string is corrupted. Please, check the YAML syntax.")
-                exit()
+                sys.exit()
         chain = Chain(**chain)
         order.initialize(chain, products, Path(args.output_dir), args.entry, query)
         app: Any = TailorApp(order, datastore, get_datatailor(args))
     else:
         order.initialize(None, products, Path(args.output_dir), args.entry, query)
         app = DownloadApp(order, datastore)
-    safe_run(app, args.yes)
+    safe_run(app, collection=args.collection[0], num_products=products_count, force=args.yes)
 
 
 def order(args: argparse.Namespace) -> None:
     """eumdac order entrypoint"""
     if args.order_command == "list":
         filenames = list(all_order_filenames())
         logger.info(f"Found {len(filenames)} order(s):")
@@ -403,39 +442,39 @@
             user_in = input(f"Are you sure to delete order {order_name} (Y/n)?")
             if user_in.lower() == "y":
                 try:
                     order.delete()
                     logger.info(f"Order {order_name} successfully deleted.")
                 except:
                     logger.warning(f"Order {order_name} can't be deleted.")
-                exit()
+                sys.exit()
             else:
                 logger.info(f"Order {order_name} wasn't deleted.")
-                exit()
+                sys.exit()
         else:
             logger.info(f"Order {order_name} doesn't exist.")
-            exit()
+            sys.exit()
 
     if not order._order_file.is_file():
         logger.info(f"Order {order_name} doesn't exist.")
-        exit()
+        sys.exit()
 
     (typ,) = order.get_dict_entries("type")
     if typ == "download":
         app: Any = DownloadApp(order, get_datastore(args))
 
     elif typ == "tailor":
         if order.all_done():
             logger.info("Order already completed")
             return
         app = TailorApp(order, get_datastore(args), get_datatailor(args))
 
     else:
         raise Exception(f"Unknown Order Type: {typ}")
-    safe_run(app, True)
+    safe_run(app, force=True)
 
 
 def get_datastore(args: argparse.Namespace, anonymous_allowed: bool = False) -> Any:
     """get an instance of DataStore"""
     if args.test:
         return FakeDataStore()
     try:
@@ -576,24 +615,24 @@
         raise ValueError("Please provide collection ID, product ID and a chain file!")
     if chain_config.endswith(".yml") or chain_config.endswith(".yaml"):
         with open(chain_config, "r") as file:
             try:
                 chain = yaml.safe_load(file)
             except:
                 logger.error("YAML file is corrupted. Please, check the YAML syntax.")
-                exit()
+                sys.exit()
     else:
         chain_config = chain_config.strip()
         if not chain_config.startswith("{"):
             chain_config = "{" + chain_config + "}"
         try:
             chain = yaml.safe_load(chain_config)
         except:
             logger.error("YAML string is corrupted. Please, check the YAML syntax.")
-            exit()
+            sys.exit()
     chain = Chain(**chain)
     products = [datastore.get_product(collection_id, product_id) for product_id in product_ids]
     try:
         customisation = datatailor.new_customisations(products, chain=chain)
         jobidsToStr = "\n".join([str(jobid) for jobid in customisation])
         logger.info("Customisation(s) has been started.")
         logger.info(jobidsToStr)
@@ -772,19 +811,15 @@
     creds = load_credentials()
     token = AccessToken(creds)
     # for customisation_id in customisation_ids:  # type: ignore[union-attr]
     customisation_id = args.job_id
     url = token.urls.get("tailor", "customisations") + f"/{customisation_id}"
     response = requests.get(
         url,
-        headers={
-            "Authorization": "Bearer {}".format(token),
-            "referer": __documentation__,
-            "User-Agent": str(__title__ + "/" + __version__),
-        },
+        headers=dict(eumdac.common.headers, **{"Authorization": "Bearer {}".format(token)}),
     )
     if response.status_code == 200:
         results = response.json()[customisation_id]["output_products"]
 
         # Create output path if it does not exist
         logger.info(f"Output directory: {os.path.abspath(args.output_dir)}")
         if not os.path.exists(args.output_dir):
@@ -794,19 +829,20 @@
         # Download all the output files into the output path
         logger.info(f"Downloading {len(results)} output products")
         for result in results:
             logger.info("Downloading " + os.path.basename(result))
             url = token.urls.get("tailor", "download") + f"?path={result}"
             response = requests.get(
                 url,
-                headers={
-                    "Authorization": "Bearer {}".format(token),
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                headers=dict(
+                    eumdac.common.headers,
+                    **{
+                        "Authorization": "Bearer {}".format(token),
+                    },
+                ),
             )
             output = args.output_dir
             if response.status_code == 200:
                 product_path = os.path.join(output, os.path.basename(result))
                 open(product_path, "wb").write(response.content)
                 logger.info(f"{os.path.basename(result)} has been downloaded.")
             else:
@@ -857,16 +893,16 @@
 
     message = _message_func(response.status_code)
 
     logger.error(message)
     logger.error(f"{response.status_code} - {response.text}")
 
 
-class TailorHelpAction(argparse.Action):
-    """eumdac tailor -h entrypoint"""
+class HelpAction(argparse.Action):
+    """eumdac tailor/search/download/subscribe/order -h entrypoint"""
 
     def __call__(self, parser: argparse.ArgumentParser, *args: Any, **kwargs: Any) -> None:
         # Print the help if the command has 2 args,
         # meaning it's just $ eumdac tailor
         if len(sys.argv) == 2:
             parser.print_help()
             parser.exit()
@@ -941,41 +977,53 @@
     search_argument_parser.add_argument(
         "-c", "--collection", nargs="+", help="collection ID(s)", required=True
     )
     search_argument_parser.add_argument(
         "-s",
         "--start",
         type=parse_isoformat,
-        help="UTC start date e.g. 2002-12-21T12:30:15",
+        help="UTC sensing start date e.g. 2002-12-21T12:30:15",
         metavar="YYYY-MM-DD[THH[:MM[:SS]]]",
         dest="dtstart",
     )
     search_argument_parser.add_argument(
         "-e",
         "--end",
         type=parse_isoformat,
-        help="UTC end date e.g. 2002-12-21T12:30:15",
+        help="UTC sensing end date e.g. 2002-12-21T12:30:15",
         metavar="YYYY-MM-DD[THH[:MM[:SS]]]",
         dest="dtend",
     )
     search_argument_parser.add_argument(
-        "--bbox",
-        nargs=4,
-        type=float,
-        metavar=("W", "S", "E", "N"),
-        help="filter by bounding box, the box is defined in EPSG:4326 decimal degrees",
-    )
-    search_argument_parser.add_argument(
         "--time-range",
         nargs=2,
         type=parse_isoformat,
         help="convenience search on UTC time range",
         metavar="YYYY-MM-DD[THH[:MM[:SS]]]",
     )
     search_argument_parser.add_argument(
+        "--publication-after",
+        type=parse_isoformat,
+        help="filter by publication date, products ingested after this UTC date e.g. 2002-12-21T12:30:15",
+        metavar="YYYY-MM-DD[THH[:MM[:SS]]]",
+    )
+    search_argument_parser.add_argument(
+        "--publication-before",
+        type=parse_isoformat,
+        help="filter by publication date, products ingested before this UTC date e.g. 2002-12-21T12:30:15",
+        metavar="YYYY-MM-DD[THH[:MM[:SS]]]",
+    )
+    search_argument_parser.add_argument(
+        "--bbox",
+        nargs=4,
+        type=float,
+        metavar=("W", "S", "E", "N"),
+        help="filter by bounding box, the box is defined in EPSG:4326 decimal degrees",
+    )
+    search_argument_parser.add_argument(
         "--geometry",
         help="filter by geometry, a custom geomtery in a EPSG:4326 decimal degrees.",
         dest="geo",
     )
     search_argument_parser.add_argument(
         "--cycle",
         help="filter by cycle number, must be a positive integer.",
@@ -1025,14 +1073,17 @@
     )
     parser_search = subparsers.add_parser(
         "search",
         help="search for products at the collection level",
         epilog="example: %(prog)s -s 2020-03-01 -e 2020-03-15T12:15 -c EO:EUM:DAT:MSG:CLM",
         parents=[common_parser, search_argument_parser],
     )
+    parser_search.add_argument(
+        dest="print_help", nargs=0, action=HelpAction, help=argparse.SUPPRESS
+    )
     parser_search.set_defaults(func=search)
 
     parser_download = subparsers.add_parser(
         "download",
         help="download product(s) from a collection",
         parents=[common_parser, search_argument_parser],  # this inherits collection lists
     )
@@ -1059,24 +1110,27 @@
         "-y", "--yes", help="Skip interactive user input", action="store_true"
     )
     parser_download.add_argument(
         "--chain",
         help="Chain YAML string for tailoring prior to downloading",
         metavar="CHAINYMLSTR",
     )
+    parser_download.add_argument(
+        dest="print_help", nargs=0, action=HelpAction, help=argparse.SUPPRESS
+    )
     parser_download.set_defaults(func=download)
 
     # subscribe parser
     parser_subscribe = subparsers.add_parser(
         "subscribe",
         help="subscribe a server for a collection",
         parents=[common_parser],
     )
     parser_subscribe.add_argument(
-        dest="print_help", nargs=0, action=TailorHelpAction, help=argparse.SUPPRESS
+        dest="print_help", nargs=0, action=HelpAction, help=argparse.SUPPRESS
     )
 
     subscribe_subparsers = parser_subscribe.add_subparsers(dest="subscribe-command")
 
     subscribe_list_parser = subscribe_subparsers.add_parser(
         "list",
         description="List subscriptions from Data Store",
@@ -1122,15 +1176,15 @@
     parser_tailor = subparsers.add_parser(
         "tailor",
         description="Manage Data Tailor customisations",
         help="tailoring product(s) from collection",
         parents=[common_parser],
     )
     parser_tailor.add_argument(
-        dest="print_help", nargs=0, action=TailorHelpAction, help=argparse.SUPPRESS
+        dest="print_help", nargs=0, action=HelpAction, help=argparse.SUPPRESS
     )
     tailor_subparsers = parser_tailor.add_subparsers(dest="tailor-command")
 
     tailor_post_parser = tailor_subparsers.add_parser(
         "post",
         description="Posts a new customisation job into Data Tailor",
         help="Posts a new customisation job into Data Tailor",
@@ -1233,17 +1287,15 @@
     #  Order parser
     parser_order = subparsers.add_parser(
         "order",
         description="Manage Data Store and Data Tailor orders",
         help="manage orders",
         parents=[common_parser],
     )
-    parser_order.add_argument(
-        dest="print_help", nargs=0, action=TailorHelpAction, help=argparse.SUPPRESS
-    )
+    parser_order.add_argument(dest="print_help", nargs=0, action=HelpAction, help=argparse.SUPPRESS)
     order_subparsers = parser_order.add_subparsers(dest="order_command")
     order_parsers = {}
     for action in ["restart", "status", "resume", "delete"]:
         subparser = order_subparsers.add_parser(
             action,
             description=f"Order {action}",
             parents=[common_parser],
```

### Comparing `eumdac-2.0.0/eumdac/collection.py` & `eumdac-2.0.1/eumdac/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 import re
 from functools import total_ordering
 from typing import TYPE_CHECKING
 from xml.etree import ElementTree
 
 import requests
 
-from .__version__ import __documentation__, __title__, __version__  # noqa
-
 if TYPE_CHECKING:  # pragma: no cover
     import sys
     from typing import Any, Optional
 
     if sys.version_info < (3, 9):
         from typing import Generator, Mapping, MutableMapping, Pattern
     else:
         from collections.abc import Mapping, MutableMapping, Generator
         from re import Pattern
     from eumdac.datastore import DataStore
     from eumdac.product import Product
 
 from eumdac.errors import EumdacError, eumdac_raise_for_status
+import eumdac.common
 
 
 class SearchResults:
     collection: Collection
     _query: MutableMapping[str, Optional[str]]
     _total_results: Optional[int] = None
     _items_per_page: int = 100
@@ -110,18 +109,15 @@
         auth = self.collection.datastore.token.auth
         url = self.collection.datastore.urls.get("datastore", "search")
         if session is None:
             response = requests.get(
                 url,
                 params=params,
                 auth=auth,
-                headers={
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                headers=eumdac.common.headers,
             )
         else:
             response = session.get(url, params=params, auth=auth)
         eumdac_raise_for_status(
             f"Search query load page failed for {self.collection} with {self._query}",
             response,
             CollectionError,
@@ -189,18 +185,15 @@
             "datastore", "browse collection", vars={"collection_id": self._id}
         )
         auth = self.datastore.token.auth
         response = requests.get(
             url,
             params={"format": "json"},
             auth=auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status(
             f"Could not get properties of {self._id}", response, CollectionError
         )
         geometry = response.json()["collection"]["geometry"]
         properties = response.json()["collection"]["properties"]
         properties.pop("links")
@@ -236,19 +229,15 @@
     def product_type(self) -> Optional[str]:
         """Product type"""
         self._ensure_properties()
         auth = self.datastore.token._access_token
         url = self.datastore.urls.get("tailor", "products")
         response = requests.get(
             url,
-            headers={
-                "Authorization": "Bearer {}".format(auth),
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=dict(eumdac.common.headers, **{"Authorization": "Bearer {}".format(auth)}),
         )
         api_response = json.loads(response.text)
 
         collection_ids = [i["pn_id"] for i in api_response["data"]]
         product_types = [i["id"] for i in api_response["data"]]
         product_types_dict = dict(zip(product_types, collection_ids))
 
@@ -281,18 +270,15 @@
             # a way to load collection specific options
             url_static = self.datastore.urls.get("datastore", "search options")
             url = url_static + "?pi=" + self._id
             auth = self.datastore.token.auth
             response = requests.get(
                 url,
                 auth=auth,
-                headers={
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                headers=eumdac.common.headers,
             )
             eumdac_raise_for_status("Could not get search options", response, CollectionError)
             root = ElementTree.fromstring(response.text)
             (element,) = [
                 ele
                 for ele in root
                 if ele.tag.endswith("Url") and ele.get("type") == "application/json"
```

### Comparing `eumdac-2.0.0/eumdac/customisation.py` & `eumdac-2.0.1/eumdac/customisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 import requests
 
 from eumdac.errors import EumdacError, eumdac_raise_for_status
 
-from .__version__ import __documentation__, __title__, __version__  # noqa
-
 if TYPE_CHECKING:  # pragma: no cover
     if sys.version_info < (3, 9):
         from typing import Generator, Iterable, Mapping, MutableMapping
     else:
         from collections.abc import MutableMapping, Mapping, Iterable, Generator
     from types import TracebackType
     from typing import IO, Any, Optional, Type
 
     from eumdac.datatailor import DataTailor
 
+import eumdac.common
+
 
 class Customisation:
     _id: str
     datatailor: DataTailor
     update_margin: float = 0.5  # seconds
     _properties: Optional[MutableMapping[str, Any]] = None
     _deleted: bool = False
@@ -71,20 +71,15 @@
         now = time.time()
         expired = now - self._last_update > self.update_margin
         if expired or self._properties is None:
             url = self.datatailor.urls.get(
                 "tailor", "customisation", vars={"customisation_id": self._id}
             )
             response = requests.get(
-                url,
-                auth=self.datatailor.token.auth,
-                headers={
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                url, auth=self.datatailor.token.auth, headers=eumdac.common.headers
             )
             eumdac_raise_for_status(
                 "Failed to get customisation", response, UnableToGetCustomisationError
             )
             self._properties = response.json()[self._id]
             self._last_update = now
 
@@ -136,18 +131,15 @@
             raise AlreadyDeletedCustomisationError("Customisation already deleted.")
         url = self.datatailor.urls.get(
             "tailor", "customisation log", vars={"customisation_id": self._id}
         )
         response = requests.get(
             url,
             auth=self.datatailor.token.auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status("Failed to get customisation log", response, CustomisationError)
         return response.json()["log_content"]
 
     @contextmanager
     def _download_response(self, output: str) -> Generator[requests.Response, None, None]:
         if self._deleted:
@@ -158,18 +150,15 @@
         auth = self.datatailor.token.auth
         params = {"path": output}
         with requests.get(
             url,
             auth=auth,
             params=params,
             stream=True,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         ) as response:
             eumdac_raise_for_status("Failed to get tailor download", response, CustomisationError)
             response.raw.name = output.split("/")[-1]
             response.raw.decode_content = True
             yield response
 
     @contextmanager
@@ -185,25 +174,27 @@
             yield resp.raw
 
     def delete(self) -> None:
         if not self._deleted:
             url = self.datatailor.urls.get("tailor", "delete")
             payload = {"uuids": [self._id]}
             auth = self.datatailor.token.auth
-            response = requests.patch(url, auth=auth, json=payload)
+            response = requests.patch(url, auth=auth, json=payload, headers=eumdac.common.headers)
             eumdac_raise_for_status("Failed to patch tailor delete", response, CustomisationError)
             self._deleted = True
 
     def kill(self) -> None:
         if not self._killed:
             url = self.datatailor.urls.get(
                 "tailor", "customisation", vars={"customisation_id": self._id}
             )
             auth = self.datatailor.token.auth
-            response = requests.put(url, json={"status": "killed"}, auth=auth)
+            response = requests.put(
+                url, json={"status": "killed"}, auth=auth, headers=eumdac.common.headers
+            )
             eumdac_raise_for_status(
                 "Failed to put tailor customisation", response, CustomisationError
             )
             self._killed = True
 
 
 class CustomisationError(EumdacError):
```

### Comparing `eumdac-2.0.0/eumdac/datastore.py` & `eumdac-2.0.1/eumdac/datastore.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import requests
 
 from eumdac.collection import Collection
 from eumdac.errors import EumdacError, eumdac_raise_for_status
 from eumdac.product import Product
 from eumdac.subscription import Subscription
 from eumdac.token import AccessToken, URLs
-
-from .__version__ import __documentation__, __title__, __version__  # noqa
+import eumdac.common
 
 if TYPE_CHECKING:  # pragma: no cover
     import sys
     from typing import Optional
 
     if sys.version_info < (3, 9):
         from typing import Iterable, Mapping
@@ -33,21 +32,15 @@
         self._collections = {}
 
     def _load_collections(self) -> None:
         if self._collections:
             return
         url = self.urls.get("datastore", "browse collections")
         response = requests.get(
-            url,
-            params={"format": "json"},
-            auth=self.token.auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            url, params={"format": "json"}, auth=self.token.auth, headers=eumdac.common.headers
         )
         eumdac_raise_for_status("Load collections failed", response, DataStoreError)
         collection_ids = [item["title"] for item in response.json()["links"]]
         self._collections = {
             collection_id: Collection(collection_id, self) for collection_id in collection_ids
         }
 
@@ -58,29 +51,38 @@
 
     @property
     def subscriptions(self) -> Iterable[Subscription]:
         url = self.urls.get("datastore", "subscriptions")
         response = requests.get(
             url,
             auth=self.token.auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status("Get subscriptions failed", response, DataStoreError)
         return [Subscription(properties["uuid"], self) for properties in response.json()]
 
     def get_collection(self, collection_id: str) -> Collection:
         """collection factory"""
-        self._load_collections()
-        try:
-            return self._collections[collection_id]
-        except KeyError as error:
-            raise DataStoreError(f"unknown collection {collection_id}") from error
+        return Collection(collection_id, self)
+
+    def check_collection_id(self, collection_id: str) -> None:
+        """Used to validate the existence of a collection"""
+        url = self.urls.get("datastore", "browse collection", vars={"collection_id": collection_id})
+        response = requests.get(url, auth=self.token.auth, headers=eumdac.common.headers)
+        if (
+            response.status_code == 401
+            or response.status_code == 403
+            or response.status_code == 404
+        ):
+            eumdac_raise_for_status(
+                "The collection you are searching for does not exist or you do not have authorisation to access it",
+                response,
+                CollectionNotFoundError,
+            )
+        return
 
     def get_product(self, collection_id: str, product_id: str) -> Product:
         """product factory"""
         return Product(collection_id, product_id, self)
 
     def get_subscription(self, subscription_id: str) -> Subscription:
         """subscription factory"""
@@ -90,15 +92,21 @@
         self, collection: Collection, url: str, area_of_interest: Optional[str] = None
     ) -> Subscription:
         """create new subscription"""
         parameters = {"collectionId": collection._id, "url": url}
         if area_of_interest is not None:
             parameters["aoi"] = area_of_interest
         subscriptions_url = self.urls.get("datastore", "subscriptions")
-        response = requests.post(subscriptions_url, json=parameters, auth=self.token.auth)
+        response = requests.post(
+            subscriptions_url, json=parameters, auth=self.token.auth, headers=eumdac.common.headers
+        )
         eumdac_raise_for_status("Creation of new subscription failed", response, DataStoreError)
         subscription_id = response.json()
         return Subscription(subscription_id, self)
 
 
 class DataStoreError(EumdacError):
     "Errors related to the DataStore"
+
+
+class CollectionNotFoundError(EumdacError):
+    """Error that will be raised when a collection does not exist"""
```

### Comparing `eumdac-2.0.0/eumdac/datatailor.py` & `eumdac-2.0.1/eumdac/datatailor.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from typing import TYPE_CHECKING
 
 import requests
 
 from eumdac.customisation import Customisation
 from eumdac.errors import EumdacError, eumdac_raise_for_status
 from eumdac.tailor_models import Chain, DataTailorCRUD, Filter, Quicklook, RegionOfInterest
-
-from .__version__ import __documentation__, __title__, __version__  # noqa
+import eumdac.common
 
 if TYPE_CHECKING:  # pragma: no cover
     import sys
     from typing import Any, Optional
 
     from eumdac.product import Product
     from eumdac.token import AccessToken, URLs
@@ -45,68 +44,56 @@
 
     @property
     def customisations(self) -> Sequence[Customisation]:
         url = self.urls.get("tailor", "customisations")
         response = requests.get(
             url,
             auth=self.token.auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status("Could not get customisations", response, DataTailorError)
         customisations = response.json()["data"]
         return [Customisation.from_properties(properties, self) for properties in customisations]
 
     @property
     def info(self) -> Mapping[str, Any]:
         if self._info is None:
             url = self.urls.get("tailor", "info")
             auth = self.token.auth
             response = requests.get(
                 url,
                 auth=auth,
-                headers={
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                headers=eumdac.common.headers,
             )
             eumdac_raise_for_status("Could not get info", response, DataTailorError)
             self._info = response.json()
         return self._info
 
     @property
     def user_info(self) -> Mapping[str, Any]:
         if self._user_info is None:
             url = self.urls.get("tailor", "user info")
             auth = self.token.auth
             response = requests.get(
                 url,
                 auth=auth,
-                headers={
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                headers=eumdac.common.headers,
             )
             eumdac_raise_for_status("Could not get user_info", response, DataTailorError)
             self._user_info = response.json()
         return self._user_info
 
     @property
     def quota(self) -> Mapping[str, Any]:
         url = self.urls.get("tailor", "report quota")
         auth = self.token.auth
         response = requests.get(
             url,
             auth=auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status("Could not get quota", response, DataTailorError)
         return response.json()
 
     def get_customisation(self, cutomisation_id: str) -> Customisation:
         return Customisation(cutomisation_id, self)
 
@@ -133,14 +120,15 @@
             params["chain_name"] = chain
         else:
             params["chain_config"] = json.dumps(chain.asdict())
         response = requests.post(
             self.urls.get("tailor", "customisations"),
             auth=self.token.auth,
             params=params,
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status("Could not add customizations", response, DataTailorError)
 
         customisation_ids = response.json()["data"]
         return [self.get_customisation(customisation_id) for customisation_id in customisation_ids]
```

### Comparing `eumdac-2.0.0/eumdac/download_app.py` & `eumdac-2.0.1/eumdac/download_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 output_subdir.mkdir(exist_ok=True)
                 output = output_subdir / fsrc.name
 
             if output.is_file():
                 logger.info(f"{job_id} Skip {output} it already exists")
             else:
                 logger.info(f"{job_id} Downloading {output}")
-                tmp = Path(output.stem + ".tmp")
+                tmp = Path(str(output) + ".tmp")
                 with tmp.open(mode="wb") as fdst:
                     # note: currently, there is no content-length header
                     # in the data store http response, so it is not simple to
                     # build a progress bar. In case it is added in future,
                     # just check fsrc.getheader("Content-Length")
                     shutil.copyfileobj(fsrc, fdst)
-                tmp.rename(output)
+                shutil.move(str(tmp), output)
```

### Comparing `eumdac-2.0.0/eumdac/endpoints.ini` & `eumdac-2.0.1/eumdac/endpoints.ini`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/errors.py` & `eumdac-2.0.1/eumdac/errors.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     except requests.HTTPError as exc:
         url = urlparse(response.url)
         try:
             extra_info = json.loads(response.text)
         except json.decoder.JSONDecodeError:
             extra_info = {"text": response.text}
         extra_info.update({"url": url, "status": response.status_code})
+        if response.status_code > 500:
+            msg = msg + " (due to a server-side error)"
         exception = exc_cls(msg, extra_info)
         raise exception from exc
 
 
 class EumdacError(Exception):
     """All eumdac errors will inherit from a EumdacError"""
```

### Comparing `eumdac-2.0.0/eumdac/fake.py` & `eumdac-2.0.1/eumdac/fake.py`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/job_id.py` & `eumdac-2.0.1/eumdac/job_id.py`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/logging.py` & `eumdac-2.0.1/eumdac/logging.py`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/order.py` & `eumdac-2.0.1/eumdac/order.py`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/product.py` & `eumdac-2.0.1/eumdac/product.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 from contextlib import contextmanager
 from datetime import datetime
 from functools import total_ordering
 from typing import TYPE_CHECKING
 
 import requests
 
-from .__version__ import __documentation__, __title__, __version__  # noqa
-
 if TYPE_CHECKING:  # pragma: no cover
     import sys
     from typing import IO, Any, Optional
 
     if sys.version_info < (3, 9):
         from typing import Generator, Mapping, MutableMapping, Pattern, Sequence
     else:
         from collections.abc import Mapping, MutableMapping, Generator, Sequence
         from re import Pattern
     from eumdac.datastore import DataStore
     from eumdac.collection import Collection
 
 from eumdac.errors import EumdacError, eumdac_raise_for_status
+import eumdac.common
 
 
 @total_ordering
 class Product:
     """Product of a Collection in the Data Store
 
     Attributes:
@@ -85,18 +84,15 @@
             vars={"collection_id": self.collection._id, "product_id": self._id},
         )
         auth = self.datastore.token.auth
         response = requests.get(
             url,
             params={"format": "json"},
             auth=auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status(
             f"Product {self._id} not found in {self.collection._id}", response, ProductError
         )
         geometry = response.json()["geometry"]
         properties = response.json()["properties"]
         properties.pop("parentIdentifier")
@@ -112,18 +108,15 @@
             vars={"collection_id": self.collection._id, "product_id": self._id},
         )
         auth = self.datastore.token.auth
         response = requests.get(
             url,
             params={"format": "json"},
             auth=auth,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         )
         eumdac_raise_for_status(
             f"Product {self._id} not found in {self.collection._id}", response, ProductError
         )
         properties = response.json()["properties"]
         links = properties.pop("links")
         self._entries = [link["title"] for link in links["sip-entries"]]
@@ -235,18 +228,15 @@
             url += "/entry"
             params = {"name": entry}
         with requests.get(
             url,
             auth=auth,
             params=params,
             stream=True,
-            headers={
-                "referer": __documentation__,
-                "User-Agent": str(__title__ + "/" + __version__),
-            },
+            headers=eumdac.common.headers,
         ) as response:
             eumdac_raise_for_status(
                 f"Could not download Product {self._id} of Collection {self.collection._id}",
                 response,
                 ProductError,
             )
             match = self._extract_filename.search(response.headers["Content-Disposition"])
```

### Comparing `eumdac-2.0.0/eumdac/subscription.py` & `eumdac-2.0.1/eumdac/subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
 import time
 from typing import TYPE_CHECKING
 
 import requests
 
-from .__version__ import __documentation__, __title__, __version__  # noqa
-
 if TYPE_CHECKING:  # pragma: no cover
     import sys
     from typing import Any
 
     from eumdac.collection import Collection
     from eumdac.datastore import DataStore
 
     if sys.version_info < (3, 9):
         from typing import Mapping
     else:
         from collections.abc import Mapping
 
 from eumdac.errors import EumdacError, eumdac_raise_for_status
+import eumdac.common
 
 
 class Subscription:
     _id: str
     datastore: DataStore
     _last_update: float
     _properties: Mapping[str, Any]
@@ -51,18 +50,15 @@
         if expired:
             url = self.datastore.urls.get(
                 "datastore", "subscription", vars={"subscription_id": self._id}
             )
             response = requests.get(
                 url,
                 auth=self.datastore.token.auth,
-                headers={
-                    "referer": __documentation__,
-                    "User-Agent": str(__title__ + "/" + __version__),
-                },
+                headers=eumdac.common.headers,
             )
             eumdac_raise_for_status(
                 "Update properties of subscription {self._id} failed", response, SubscriptionError
             )
             self._properties = response.json()
             self._last_update = now
 
@@ -87,15 +83,17 @@
         self._update_properties()
         return self._properties["status"]
 
     def delete(self) -> None:
         url = self.datastore.urls.get(
             "datastore", "subscription", vars={"subscription_id": self._id}
         )
-        response = requests.delete(url, auth=self.datastore.token.auth)
+        response = requests.delete(
+            url, auth=self.datastore.token.auth, headers=eumdac.common.headers
+        )
         eumdac_raise_for_status(
             "Delete subscription {self._id} failed", response, SubscriptionError
         )
 
 
 class SubscriptionError(EumdacError):
     """Errors related to subscriptions"""
```

### Comparing `eumdac-2.0.0/eumdac/tailor_app.py` & `eumdac-2.0.1/eumdac/tailor_app.py`

 * *Files identical despite different names*

### Comparing `eumdac-2.0.0/eumdac/tailor_models.py` & `eumdac-2.0.1/eumdac/tailor_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 from dataclasses import asdict, dataclass
 from typing import TYPE_CHECKING
 
 import requests
+import eumdac.common
 
 if TYPE_CHECKING:  # pragma: no cover
     import sys
     from typing import Any, Optional, Type, Union
 
     if sys.version_info < (3, 9):
         from typing import MutableMapping, Sequence
@@ -78,14 +79,15 @@
     projection: Optional[str] = None
     roi: Union[None, dict, RegionOfInterest] = None  # type: ignore[type-arg]
     filter: Union[None, dict, Filter] = None  # type: ignore[type-arg]
     quicklook: Union[None, dict, Quicklook] = None  # type: ignore[type-arg]
     resample_method: Optional[str] = None
     resample_resolution: Optional[list] = None  # type: ignore[type-arg]
     compression: Optional[dict] = None  # type: ignore[type-arg]
+    xrit_segments: Optional[list] = None  # type: ignore[type-arg]
 
     def __post_init__(self) -> None:
         for name, Model in self.__submodels.items():
             attr = getattr(self, name)
             if attr is not None and isinstance(attr, Mapping):
                 setattr(self, name, Model(**attr))
 
@@ -138,10 +140,10 @@
         else:
             model_id = model.id  # type: ignore[assignment]
         url = f"{self.url}/{model_id}"
         auth = self.datatailor.token.auth
         self._request("DELETE", url, auth=auth)
 
     def _request(self, method: str, url: str, **options: Any) -> requests.Response:
-        response = requests.request(method, url, **options)
+        response = requests.request(method, url, headers=eumdac.common.headers, **options)
         eumdac_raise_for_status(f"Request for {self.Model} failed.", response, EumdacError)
         return response
```

### Comparing `eumdac-2.0.0/eumdac/token.py` & `eumdac-2.0.1/eumdac/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, NamedTuple
 from urllib.parse import quote as url_quote
 
 import requests
 from pkg_resources import resource_filename
 from requests.auth import AuthBase, HTTPBasicAuth
+import eumdac.common
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Optional
 
     if sys.version_info < (3, 9):
         from typing import Iterable, Mapping
     else:
@@ -111,15 +112,18 @@
     def auth(self) -> AuthBase:
         return HTTPBearerAuth(self.access_token)
 
     def _update_token_data(self) -> None:
         auth = HTTPBasicAuth(*self.credentials)
         now = time.time()
         response = requests.post(
-            self.urls.get("token", "token"), auth=auth, data={"grant_type": "client_credentials"}
+            self.urls.get("token", "token"),
+            auth=auth,
+            data={"grant_type": "client_credentials"},
+            headers=eumdac.common.headers,
         )
         response.raise_for_status()
         token_data = response.json()
         self._expiration = now + token_data["expires_in"]
         self._access_token = token_data["access_token"]
```

### Comparing `eumdac-2.0.0/eumdac.egg-info/PKG-INFO` & `eumdac-2.0.1/eumdac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eumdac
-Version: 2.0.0
+Version: 2.0.1
 Summary: EUMETSAT Data Access Client
 Home-page: https://gitlab.eumetsat.int/eumetlab/data-services/eumdac
 Author: EUMETSAT
 Author-email: ops@eumetsat.int
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -73,14 +73,15 @@
 ## Authors
 * [**Carlos Horn**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Ben Loveday**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Niklas Jordan**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Paulo Carmo**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Christopher Saloman**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 * [**Matthias Schwarz**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
+* [**Joaquin Rodríguez-Guerra**](mailto://ops@eumetsat.int) - [EUMETSAT](https://eumetsat.int)
 * [**Rafa de la Hoz**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 
 ## Dependencies
 requests,   ver. 2.26.0, License: Apache-2.0 (LICENSE_APACHE_v2.txt), Copyright 2014 Kenneth Reitz,   info: https://anaconda.org/conda-forge/requests  \
 responses,  ver. 0.16.0, License: Apache-2.0 (LICENSE_APACHE_v2.txt), Copyright 2015 David Cramer,    info: https://anaconda.org/conda-forge/responses  \
 setuptools, ver. 58.0.4, License: MIT (LICENSE_MIT.txt),              Copyright 2020 Jason R. Coombs, info: https://anaconda.org/conda-forge/setuptools
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eumdac-2.0.0/eumdac.egg-info/SOURCES.txt` & `eumdac-2.0.1/eumdac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE_MIT.txt
 README.md
 setup.py
 eumdac/__init__.py
 eumdac/__version__.py
 eumdac/cli.py
 eumdac/collection.py
+eumdac/common.py
 eumdac/config.py
 eumdac/customisation.py
 eumdac/datastore.py
 eumdac/datatailor.py
 eumdac/download_app.py
 eumdac/endpoints.ini
 eumdac/errors.py
```

### Comparing `eumdac-2.0.0/setup.py` & `eumdac-2.0.1/setup.py`

 * *Files identical despite different names*

