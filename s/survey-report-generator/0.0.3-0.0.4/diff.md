# Comparing `tmp/survey_report_generator-0.0.3.tar.gz` & `tmp/survey_report_generator-0.0.4.tar.gz`

## Comparing `survey_report_generator-0.0.3.tar` & `survey_report_generator-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/requirements.txt
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/setup.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/__init__.py
--rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/databases.py
--rw-r--r--   0        0        0    12224 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/databases_summary.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/date_time.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/download_files.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/fesm.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/figures_utils.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/filter_utils.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/filter_utils_summary.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/g_drive_utils.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/generate_report.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/koala_habitat.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/pct.py
--rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/report-template.docx
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/report.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/storage.json
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/summary.py
--rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/tables.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/LICENSE
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/.DS_Store
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/.DS_Store
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/__init__.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/databases.py
+-rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/databases_summary.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/date_time.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/download_files.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/fesm.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/figures_utils.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/filter_utils.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/filter_utils_summary.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/g_drive_utils.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/generate_report.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/koala_habitat.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/pct.py
+-rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/report-template.docx
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/report.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/storage.json
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/summary.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/tables.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/README.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/PKG-INFO
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/.DS_Store` & `survey_report_generator-0.0.4/survey_report_generator/.DS_Store`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/databases.py` & `survey_report_generator-0.0.4/survey_report_generator/databases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 from shapely.geometry import Polygon
+import warnings
+warnings.filterwarnings("ignore", category=UserWarning, module="numpy", message=".*Intel MKL WARNING.*")
 import numpy as np
 import os
 
-import download_files
-from filter_utils import filter_location, filter_datetime, filter_species_names
+from .filter_utils import filter_location, filter_datetime
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
 
 def generate_survey_database(report):
     """
     This method filters the survey database to select rows only relevant to the selected survey location.
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/databases_summary.py` & `survey_report_generator-0.0.4/survey_report_generator/databases_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 from shapely.geometry import Polygon
 import numpy as np
 import os
 
 import download_files
-from filter_utils_summary import filter_location, filter_datetime
+from .filter_utils_summary import filter_location, filter_datetime
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
 
 def generate_databases(location_filter, database_location, download_databases, summary=False):
     if download_databases:
         download_files.download_databases(database_location)
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/date_time.py` & `survey_report_generator-0.0.4/survey_report_generator/date_time.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/download_files.py` & `survey_report_generator-0.0.4/survey_report_generator/download_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from collections import defaultdict
-from g_drive_utils import get_gdrive_connection, get_drive_file_list, download_file
+
+from .g_drive_utils import get_gdrive_connection, get_drive_file_list, download_file
 
 
 def download_file_from_filepath(filepath):
     """
     This method takes a filepath and downloads the file using its id
 
     Args:
@@ -85,19 +86,14 @@
 def do_download(drive_service, destination_path, file_id, file_sha1=None, hash_store=defaultdict(str),
                 hash_store_file='', test=False):
     '''
     Download the file
     '''
     folder_path = os.path.dirname(destination_path)
     os.makedirs(folder_path, exist_ok=True)
-    if os.path.exists(destination_path):
-        print(
-            f'update {destination_path},{file_sha1} {hash_store[destination_path]}')
-    else:
-        print(f'dl {destination_path}')
     file_contents = download_file(drive_service, file_id)
     if file_contents is not None:
         with open(destination_path, 'wb') as write:
             write.write(file_contents.getvalue())
         if hash_store_file != '':
             add_hash(destination_path, hash_store_file, file_sha1)
     else:
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/fesm.py` & `survey_report_generator-0.0.4/survey_report_generator/fesm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PIL import Image
 from io import BytesIO
 import requests
-from figures_utils import get_bounding_box, generate_figure
+from .figures_utils import get_bounding_box, generate_figure
 import pandas as pd
 
 
 def generate_fesm_map(kmls, detections, filename):
 	bbox = get_bounding_box(kmls, detections)
 	image = get_fesm_map(bbox)
 	generate_figure(kmls, detections, filename, bbox, image, path_colour='lightgray', alpha=1.0)
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/figures_utils.py` & `survey_report_generator-0.0.4/survey_report_generator/figures_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/filter_utils.py` & `survey_report_generator-0.0.4/survey_report_generator/filter_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/filter_utils_summary.py` & `survey_report_generator-0.0.4/survey_report_generator/filter_utils_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/g_drive_utils.py` & `survey_report_generator-0.0.4/survey_report_generator/g_drive_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from oauth2client import file, client, tools
 from http.client import IncompleteRead
 
 
 def generate_credentials():
     '''Handles login, and then passes on credentials for the connection to be started'''
     SCOPES = 'https://www.googleapis.com/auth/drive.readonly'
-    if not os.path.exists('storage.json') and os.path.exists('~/storage.json'):
+    if not os.path.exists('survey_report_generator/storage.json') and os.path.exists('~/storage.json'):
         store = file.Storage('~/storage.json')
     else:
-        store = file.Storage('storage.json')
+        store = file.Storage('survey_report_generator/storage.json')
     creds = store.get()
     # Get credentials according to either https://cloud.google.com/docs/authentication/provide-credentials-adc#local-dev
     # or https://codelabs.developers.google.com/codelabs/gsuite-apis-intro/#6
     if not creds or creds.invalid:
         flow = client.flow_from_clientsecrets('client_id.json', SCOPES)
         creds = tools.run_flow(flow, store)
     return creds
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/generate_report.py` & `survey_report_generator-0.0.4/survey_report_generator/generate_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 import os
 
 import pandas as pd
 from docx.shared import Cm
 from docxtpl import DocxTemplate, InlineImage
+import warnings
 
-from report import Report
-import tables
-import figures_utils
-from date_time import add_dates, add_summary_dates
-from summary import get_summary
-from koala_habitat import generate_koala_habitat_map
-from pct import generate_pct_map
-from fesm import generate_fesm_map
+
+from .report import Report
+from . import tables
+from . import figures_utils
+from .date_time import add_dates, add_summary_dates
+from .summary import get_summary
+from .koala_habitat import generate_koala_habitat_map
+from .pct import generate_pct_map
+from .fesm import generate_fesm_map
 
 pd.options.mode.chained_assignment = None  # default='warn'
+warnings.filterwarnings("ignore", category=UserWarning, module="numpy", message=".*Intel MKL WARNING.*")
 
 
-def generate_report(report, download_databases=False, report_location='generated-reports'):
+def generate_report(report, download_databases=True, report_location='generated-reports'):
     """
     Args:
         report (Report): Holds all variables specific to each report
         download_databases (bool): If set to true, the relevant databases will be downloaded from Google Drive.
         report_location (str): The folder, in which, the report should be saved. By default, this is the current
             working directory.
     """
     # Import template
-    template = DocxTemplate('report-template.docx')
+    template = DocxTemplate('survey_report_generator/report-template.docx')
 
     report.generate_databases(download_databases)
 
     # The context variable holds all variables to be inserted into the template
     report.context['num_flights'] = len(report.airdata)
     report.context['client'] = 'NSW National Parks'
     add_dates(report)
-    add_summary_dates(report)
+    if os.path.exists(os.path.join(report.database_location, 'summary')):
+        add_summary_dates(report)
 
     get_summary(report)
 
     # Add tables
     tables.add_survey_results_table(report)
-    tables.add_survey_results_summary_table(report)
     tables.add_detections_list(report)
     tables.add_species_list(report)
-    tables.add_detections_list_summary(report)
     tables.add_species_list(report)
-    tables.add_species_list_summary(report)
     tables.add_site_details_table(report)
-    tables.add_site_details_summary_table(report)
     tables.add_plots_table(report)
 
+    if os.path.exists(os.path.join(report.database_location, 'summary')):
+        tables.add_survey_results_summary_table(report)
+        tables.add_detections_list_summary(report)
+        tables.add_species_list_summary(report)
+        tables.add_site_details_summary_table(report)
+
     # Add figures
     print("Generating survey site map...")
     figures_utils.generate_figure(report.kmls, report.detections, 'map.png')
     report.context['figure_1'] = InlineImage(template, 'figures/map.png', Cm(15))
     print("Generating koala habitat map...")
     generate_koala_habitat_map(report.kmls, report.detections, 'koala-habitat-map.png')
     report.context['figure_2'] = InlineImage(template, 'figures/koala-habitat-map.png', Cm(15))
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/koala_habitat.py` & `survey_report_generator-0.0.4/survey_report_generator/koala_habitat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PIL import Image
 from io import BytesIO
 import requests
 from matplotlib import pyplot as plt
 
-from figures_utils import get_bounding_box, generate_figure
+from .figures_utils import get_bounding_box, generate_figure
 import pandas as pd
 
 
 def generate_koala_habitat_map(kmls, detections, file_name):
 	bbox = get_bounding_box(kmls, detections)
 	image = get_koala_habitat_map(bbox)
 	generate_figure(kmls, detections, file_name, bbox, image)
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/pct.py` & `survey_report_generator-0.0.4/survey_report_generator/pct.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PIL import Image
 from io import BytesIO
 import requests
-from figures_utils import get_bounding_box, generate_figure
+from .figures_utils import get_bounding_box, generate_figure
 import pandas as pd
 
 
 def generate_pct_map(kmls, detections, filename):
 	bbox = get_bounding_box(kmls, detections)
 	image = get_pct_map(bbox)
 	generate_figure(kmls, detections, filename, bbox, image, path_colour='grey', alpha=1.0)
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/report-template.docx` & `survey_report_generator-0.0.4/survey_report_generator/report-template.docx`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/report.py` & `survey_report_generator-0.0.4/survey_report_generator/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 
 import pandas as pd
+import warnings
+warnings.filterwarnings("ignore", category=UserWarning, module="numpy", message=".*Intel MKL WARNING.*")
 
-from survey_report_generator import download_files
-from survey_report_generator.databases import generate_survey_database, generate_detections_database, \
+from . import download_files
+from .databases import generate_survey_database, generate_detections_database, \
     generate_airdata_database, generate_kml_database
 
 
 class Report:
     """
     This class represents a report object and includes all variables necessary to extract relevant data to build a
     report.
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/storage.json` & `survey_report_generator-0.0.4/survey_report_generator/storage.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.93359375%*

 * *Differences: {"'access_token'": "'ya29.a0AfB_byAWKhG8hlj-e7aKFUkmVg7715w1SOMXaocQLirqB8HSZ24Wcn_d1akeAvVpXkxR9_tjRP4PFHG0FWfn6vhL70RDVRa2t7TO8Fh8TI7HIyH0Wm51dShaMZ_SU06Yzg980zKd2oM91-I2EHrqss_SIGc6yPZ76AaCgYKAeYSARESFQHsvYlstWHo6CHH-UomwZ1jJwntBg0169'",*

 * * "'token_expiry'": "'2023-08-07T10:49:17Z'",*

 * * "'token_response'": "{'access_token': "*

 * *                     "'ya29.a0AfB_byAWKhG8hlj-e7aKFUkmVg7715w1SOMXaocQLirqB8HSZ24Wcn_d1akeAvVpXkxR9_tjRP4PFHG0FWfn6vhL70RDVRa2t7TO8Fh8TI7HIyH0Wm51dShaMZ_SU06Yzg980zKd2oM91-I2EHrqss_SIGc […]*

```diff
@@ -1,25 +1,25 @@
 {
     "_class": "OAuth2Credentials",
     "_module": "oauth2client.client",
-    "access_token": "ya29.a0AbVbY6M04QIOC6KBAG-EWQQubvFVTscFYty-ZONVXP-inNzwgcwG2wWNRZTyliV_t-Np3YMJIRcRL8jC4-Up6K_N1uMFCsjcaA7zGDdDenVVtVL8CUeqx9DSR2o-fYYTCk2e_MTJw0msPPDoNIETj4Df0R7DB4xEmgaCgYKAeYSARESFQFWKvPlTs285i2kZ3xM0tuK2BBKgw0169",
+    "access_token": "ya29.a0AfB_byAWKhG8hlj-e7aKFUkmVg7715w1SOMXaocQLirqB8HSZ24Wcn_d1akeAvVpXkxR9_tjRP4PFHG0FWfn6vhL70RDVRa2t7TO8Fh8TI7HIyH0Wm51dShaMZ_SU06Yzg980zKd2oM91-I2EHrqss_SIGc6yPZ76AaCgYKAeYSARESFQHsvYlstWHo6CHH-UomwZ1jJwntBg0169",
     "client_id": "45499065701-th8dtkb699i8fft8a3jd7kgg47k6h68c.apps.googleusercontent.com",
     "client_secret": "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",
     "id_token": null,
     "id_token_jwt": null,
     "invalid": false,
     "refresh_token": "1//0gt8ALwWSPqaWCgYIARAAGBASNwF-L9IrvV4k59NARzaI7l11noAIQx-EjxrgkU8laIYTnus5eOX8tjjIpoJUTaVc6quVkiY-8p4",
     "revoke_uri": "https://oauth2.googleapis.com/revoke",
     "scopes": [
         "https://www.googleapis.com/auth/drive.readonly"
     ],
-    "token_expiry": "2023-08-02T00:55:41Z",
+    "token_expiry": "2023-08-07T10:49:17Z",
     "token_info_uri": "https://oauth2.googleapis.com/tokeninfo",
     "token_response": {
-        "access_token": "ya29.a0AbVbY6M04QIOC6KBAG-EWQQubvFVTscFYty-ZONVXP-inNzwgcwG2wWNRZTyliV_t-Np3YMJIRcRL8jC4-Up6K_N1uMFCsjcaA7zGDdDenVVtVL8CUeqx9DSR2o-fYYTCk2e_MTJw0msPPDoNIETj4Df0R7DB4xEmgaCgYKAeYSARESFQFWKvPlTs285i2kZ3xM0tuK2BBKgw0169",
+        "access_token": "ya29.a0AfB_byAWKhG8hlj-e7aKFUkmVg7715w1SOMXaocQLirqB8HSZ24Wcn_d1akeAvVpXkxR9_tjRP4PFHG0FWfn6vhL70RDVRa2t7TO8Fh8TI7HIyH0Wm51dShaMZ_SU06Yzg980zKd2oM91-I2EHrqss_SIGc6yPZ76AaCgYKAeYSARESFQHsvYlstWHo6CHH-UomwZ1jJwntBg0169",
         "expires_in": 3599,
         "scope": "https://www.googleapis.com/auth/drive.readonly",
         "token_type": "Bearer"
     },
     "token_uri": "https://oauth2.googleapis.com/token",
     "user_agent": null
 }
```

### Comparing `survey_report_generator-0.0.3/survey_report_generator/summary.py` & `survey_report_generator-0.0.4/survey_report_generator/summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/survey_report_generator/tables.py` & `survey_report_generator-0.0.4/survey_report_generator/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 import os
 
 import pandas as pd
 import numpy as np
 
-from filter_utils import filter_species_names, filter_target_species
+from .filter_utils import filter_species_names, filter_target_species
 
 
 def add_survey_results_table(report):
     target_species_df = filter_target_species(report.detections, report.target_species, report.database_location)
     target_species_df.loc[:, 'gt_outcome'] = target_species_df.gt_outcome.fillna('unvalidated')
     target_species_df.loc[:, 'gt_outcome'] = target_species_df.gt_outcome.replace('unconfirmed', 'unvalidated')
     target_species_df.loc[:, 'probability'] = target_species_df.probability.fillna('Null')
```

### Comparing `survey_report_generator-0.0.3/.gitignore` & `survey_report_generator-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/LICENSE` & `survey_report_generator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.3/README.md` & `survey_report_generator-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Report Generator
+# Survey Report Generator
 
 [![PyPI version](https://badge.fury.io/py/survey-report-generator.svg)](https://badge.fury.io/py/survey-report-generator)
 
 Report Generator is a Python package used to generate reports for drone surveys. 
 You input the location name and a few other variables and the package will return a Word document pre-filled with tables and figures summarising the data collected for that survey.
 
 ## Installation
@@ -29,26 +29,27 @@
   - `database_location (str)`: In order to generate the contents in the report, databases need to be downloaded to local storage. This parameter specifies the path to the location where you want these databases to be stored. It can be a directory which doesn't exist yet.
   - `start_date (str)`: a string in the format dd-mm-yyyy representing the earliest date you want to include.
   - `end_date (str)`: a string in the format dd-mm-yyyy representing the latest date you want to include.
 
 Here are a few examples of how to initialise a Report object.
 
 ```python
-from report import Report
+from survey_report_generator import Report
 
 meryla = Report(location_name='Meryla State Forest', location_filter='meryla')
 bar = Report(location_name='Bar Flora Reserve', location_filter='Bar', avoid_kmls=True, case=True)
-koreelah = Report(location_name='Koreelah State Forest', location_filter=r"[K|k]oo?ree?lah", avoid_kmls=True,
-                  regex=True)
+koreelah = Report(location_name='Koreelah State Forest', location_filter=r"[K|k]oo?ree?lah", avoid_kmls=True, regex=True)
 ```
 
 Once you have a Report object, you can input this into the `generate_report()` method. 
 
 ```python
-from report-generator import generate_report
-
+from survey_report_generator import generate_report
 
+generate_report(report=meryla)
 ```
 
+This will generate folders with databases and figures along with the report itself as a Word document.
+
 ## License
 
 Report Generator is released under the [MIT License](LICENSE).
```

### Comparing `survey_report_generator-0.0.3/pyproject.toml` & `survey_report_generator-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "survey-report-generator"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Oliver Hahn", email="oliver.a.hahn@gmail.com" },
 ]
 description = "A tool to generate survey reports from collected data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `survey_report_generator-0.0.3/PKG-INFO` & `survey_report_generator-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: survey-report-generator
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to generate survey reports from collected data
 Project-URL: Homepage, https://github.com/nsw-wildlife-drone-hub/report-generator
 Author-email: Oliver Hahn <oliver.a.hahn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Report Generator
+# Survey Report Generator
 
 [![PyPI version](https://badge.fury.io/py/survey-report-generator.svg)](https://badge.fury.io/py/survey-report-generator)
 
 Report Generator is a Python package used to generate reports for drone surveys. 
 You input the location name and a few other variables and the package will return a Word document pre-filled with tables and figures summarising the data collected for that survey.
 
 ## Installation
@@ -42,26 +42,27 @@
   - `database_location (str)`: In order to generate the contents in the report, databases need to be downloaded to local storage. This parameter specifies the path to the location where you want these databases to be stored. It can be a directory which doesn't exist yet.
   - `start_date (str)`: a string in the format dd-mm-yyyy representing the earliest date you want to include.
   - `end_date (str)`: a string in the format dd-mm-yyyy representing the latest date you want to include.
 
 Here are a few examples of how to initialise a Report object.
 
 ```python
-from report import Report
+from survey_report_generator import Report
 
 meryla = Report(location_name='Meryla State Forest', location_filter='meryla')
 bar = Report(location_name='Bar Flora Reserve', location_filter='Bar', avoid_kmls=True, case=True)
-koreelah = Report(location_name='Koreelah State Forest', location_filter=r"[K|k]oo?ree?lah", avoid_kmls=True,
-                  regex=True)
+koreelah = Report(location_name='Koreelah State Forest', location_filter=r"[K|k]oo?ree?lah", avoid_kmls=True, regex=True)
 ```
 
 Once you have a Report object, you can input this into the `generate_report()` method. 
 
 ```python
-from report-generator import generate_report
-
+from survey_report_generator import generate_report
 
+generate_report(report=meryla)
 ```
 
+This will generate folders with databases and figures along with the report itself as a Word document.
+
 ## License
 
 Report Generator is released under the [MIT License](LICENSE).
```

