# Comparing `tmp/climatePy-0.4.37.tar.gz` & `tmp/climatePy-0.4.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.37.tar", last modified: Thu Jul 27 23:48:46 2023, max compression
+gzip compressed data, was "climatePy-0.4.38.tar", last modified: Mon Aug  7 16:26:28 2023, max compression
```

## Comparing `climatePy-0.4.37.tar` & `climatePy-0.4.38.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.580408 climatePy-0.4.37/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-27 23:48:43.000000 climatePy-0.4.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-27 23:48:46.580408 climatePy-0.4.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-27 23:48:43.000000 climatePy-0.4.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.536408 climatePy-0.4.37/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    63328 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39286 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.536408 climatePy-0.4.37/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.536408 climatePy-0.4.37/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:48:46.580408 climatePy-0.4.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-27 23:48:45.000000 climatePy-0.4.37/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.580408 climatePy-0.4.37/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/test_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:26:28.037632 climatePy-0.4.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-07 16:26:23.000000 climatePy-0.4.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-07 16:26:28.033632 climatePy-0.4.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-07 16:26:23.000000 climatePy-0.4.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:26:27.969631 climatePy-0.4.38/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63790 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39448 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46260 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:26:27.973631 climatePy-0.4.38/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-08-07 16:26:23.000000 climatePy-0.4.38/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:26:27.973631 climatePy-0.4.38/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-07 16:26:27.000000 climatePy-0.4.38/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-07 16:26:27.000000 climatePy-0.4.38/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:26:27.000000 climatePy-0.4.38/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 16:26:27.000000 climatePy-0.4.38/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 16:26:27.000000 climatePy-0.4.38/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:26:28.037632 climatePy-0.4.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-07 16:26:26.000000 climatePy-0.4.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:26:28.033632 climatePy-0.4.38/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:26:23.000000 climatePy-0.4.38/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-07 16:26:23.000000 climatePy-0.4.38/tests/test_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49522 2023-08-07 16:26:23.000000 climatePy-0.4.38/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-07 16:26:23.000000 climatePy-0.4.38/tests/test_utils.py
```

### Comparing `climatePy-0.4.37/LICENSE` & `climatePy-0.4.38/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/PKG-INFO` & `climatePy-0.4.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.37
+Version: 0.4.38
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Author-email: anguswatters@gmail.com, mikecp11@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `climatePy-0.4.37/README.md` & `climatePy-0.4.38/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/climatePy/__init__.py` & `climatePy-0.4.38/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/climatePy/_climatepy_filter.py` & `climatePy-0.4.38/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/climatePy/_dap.py` & `climatePy-0.4.38/climatePy/_dap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1483,24 +1483,35 @@
     interval_map = {
         "hour": "H",
         "hours": "H",
         "minute": "min",
         "minutes": "min",
         "second": "S",
         "seconds": "S",
-        "month": "MS",  # Month Start
-        "months": "MS"  # Month Start
+        "month": "MS",  # month start
+        "months": "MS"  
         }
     
     # split interval string
     interval_type = interval.split(" ")[-1]
 
     # get frequency from interval_map
     freq = interval_map.get(interval_type, interval_type[0])
     
+    # if date interval is just a single date or if start and end dates are the same, return a single date date_range 
+    if interval == "0" or d[0] == d[1]:
+
+        # pd.date_range(start=d[0], end=d[1], freq=freq)
+        # pd.date_range(start=d[0], end=d[1])
+
+        # TODO: could also set interval to None within _resource_time() function instead of 0 ...
+        # pd.date_range(start=d[0], end=d[1], freq=None)
+
+        return pd.date_range(start=d[0], end=d[1])
+    
     # # convert start_date and end_date to pandas Timestamp objects
     # start_date = pd.Timestamp(d[0])
     # end_date = pd.Timestamp(d[1])
     # # calculate the number of days between start and end dates
     # delta = (end_date - start_date) / (nT - 1)
     # # generate the date range
     # date_range = pd.date_range(start=start_date, end=end_date, freq=str(int(delta.days))+'D')
```

### Comparing `climatePy-0.4.37/climatePy/_extract_sites.py` & `climatePy-0.4.38/climatePy/_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/climatePy/_netrc_utils.py` & `climatePy-0.4.38/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/climatePy/_shortcuts.py` & `climatePy-0.4.38/climatePy/_shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -804,33 +804,35 @@
 # TODO: too much data is extracted when function is called, need to look into what is going on here with the dap function
 # TODO: currently crashes my computer, even when I try to run on a small AOI and for a short time period
 def getCHIRPS(
         AOI       = None,
         varname   = None,
         startDate = None, 
         endDate   = None, 
+        timeRes   = "monthly",
         dopar     = True,
         verbose   = False
         ):
     
     """Get CHIRPS data for an Area of Interest
 
     CHIRPS is a global dataset of daily precipitation estimates, with a spatial resolution of 0.05 degrees (~5 km).
     Currently only monthly data is available.
 
     Args:
         AOI (geopandas dataframe, shapely geometry): Area of Interest polygon to extract data for.
         varname (str): variable name to extract (e.g. tmin).
         startDate (str): start date of data to be downloaded (YYYY-MM-DD). Default is None.
         endDate (str): end date of data to be downloaded (YYYY-MM-DD). Default is None.
+        timeRes (str): time resolution of data to be downloaded ("monthly", "daily", "annual", "pentad" ). Default is "monthly".
         dopar (bool): use parallel processing. If True multiple workers will fetch data from remote sources in parallel.
         verbose (bool): print verbose output. Default is False.
     """
 
-    timeRes = "monthly"
+    # timeRes = "monthly"
 
     # make sure timeRes is capitalized correctly
     timeRes = " ".join(word.capitalize() for word in timeRes.split())
 
     # Regex to capitalize first letter of each word
     # timeRes = re.sub(r"(^|[[:space:]])([[:alpha:]])",
     # 	lambda match: match.group(1) + match.group(2).upper(), timeRes)
```

### Comparing `climatePy-0.4.37/climatePy/_utils.py` & `climatePy-0.4.38/climatePy/_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import xarray as xr
 import netCDF4 as nc
 from pyproj import CRS, Proj
 
 # data wrangling and manipulation
 import numpy as np
 import pandas as pd
+from collections import Counter
 
 # warnings lib
 import warnings
 
 # suppress warnings
 warnings.filterwarnings('ignore', category=Warning)
 
@@ -547,127 +548,538 @@
     raw_df["dim_order"] = "".join([str(i) for sub in o for i in sub])
     
     # replace the time variable name with the name found in NetCDF
     raw_df.at[0, 'T_name'] = time_var
 
     return raw_df
 
+def match_date_abbr(key):
+    
+    """Match the abbreviated time units to the full time units
+    
+    Args:
+        key (str): The abbreviated time unit.
+    
+    Returns:    
+        str: The full time unit.
+    """
+
+    # map of abbreviated time units to full time units
+    abbr_map = {
+        "H": "hours",
+        "D": "days",
+        "min": "minutes",
+        "S": "seconds",
+        "MS": "months"
+        }
+    
+    if key in abbr_map.keys():
+        return abbr_map[key]
+    else:
+        return key
+
+def match_long_time_units(key):
+        
+        long_map = {
+            "hour": "H",
+            "hours": "H",
+            "day": "D",
+            "days": "D",
+            "minutes": "min",
+            "seconds": "S",
+            "month": "M",
+            "months": "MS",
+            "years": "Y"
+            }
+        
+        if key in long_map.keys():
+            return long_map[key]
+        else:
+            return key
+
+def days_to_intervals(key):
+
+    """ Convert days to other common intervals """
+
+    # if interval is "2-4 day"
+    if key > 1 and key < 3:
+        return f"{key} day"
+    
+    day_conversions = {
+        1: "1 day",
+        4: "5 days",
+        5: "5 days",
+        6: "5 days",
+        7: "1 week",
+        28: "1 month",
+        29: "1 month",
+        30: "1 month",
+        31: "1 month",
+        60: "2 months",
+        90: "3 months",
+        120: "4 months",
+        150: "5 months",
+        180: "6 months",
+        365: "1 year",
+        730: "2 year",
+        1095: "3 years",
+        1825: "5 years",
+        3650: "10 years",
+    }
+    if key in day_conversions:
+        return day_conversions[key]
+    else:
+        return False
+    
+def seconds_to_intervals(key):
+
+    """ Convert seconds to other common intervals """
+
+    sec_conversions = {
+        1: "1 second",
+        60: "1 minute",
+        3600: "1 hour",
+        86400: "1 day",
+        432000: "5 days",
+        2592000: "1 month",
+        31536000: "1 year"
+    }
+
+    if key in sec_conversions:
+        return sec_conversions[key]
+    else:
+        return False
+    
+def has_hms(timesteps):
+    """Check if datetime object has valid hours, minutes, or seconds, or if it is a duplicate value that can be dropped"""
+    
+    # convert timedelta object to string
+    ts = [str(i) for i in timesteps]
+
+    # get the time differences between each timestep
+    res = set(dstring.split("T")[1] for dstring in ts if "T" in dstring)
+
+    # convert timedelta object to string
+    if len(res) == 0:
+        return False
+    elif len(res) == 1:
+        return "duplicates"
+    else:
+        return True
+
+def convert_to_days(time_interval):
+    # time_interval = "720 minutes"
+    # Define conversion factors
+    conversion_factors = {
+        "second": 1 / 86400,
+        "seconds": 1 / 86400,
+        "minute": 1 / 1440,
+        "minutes": 1 / 1440,
+        "hour": 1 / 24,
+        "hours": 1 / 24,
+        "day": 1,
+        "days": 1,
+        "month": 30,
+        "months": 30,
+        "year": 365,
+        "years": 365
+    }
+    
+    # get time and unit parts
+    parts = time_interval.split()
+
+    if len(parts) != 2:
+        return "Invalid input"
+    
+    # convert the value to a float and the unit to lowercase
+    value, unit = float(parts[0]), parts[1].lower()
+    
+    # Check if the unit is in conversion_factors map
+    if unit not in conversion_factors:
+        return "Invalid unit"
+    
+    # calc the equivalent value in days
+    value_in_days = value * conversion_factors[unit]
+
+    # check if the value is a whole number and return it without decimal places
+    # if value_in_days.is_integer():
+    if value_in_days.is_integer() or abs(value_in_days - round(value_in_days)) < 0.10:
+        return str(int(value_in_days)) + " days"
+    
+    # return str(int(value_in_days)) + " days"
+    return f"{value_in_days:.1f} days"
+
+def get_time_intervals(timesteps):
+    """Get timedelta intervals from a list of datetime objects
+    
+    Args:
+        timesteps (list): np.array of np.datetime64 objects
+
+    Returns:
+        np.array: numpy.timedelta64 intervals
+    """
+
+    # timesteps  = np.array([np.datetime64('2020-01-01'),np.datetime64('2020-01-02'),
+    #                         np.datetime64('2020-01-03'),
+    #                         np.datetime64('2020-01-04')])
+    # timesteps  = np.array([np.datetime64('2020-01-01'),np.datetime64('2020-02-01'),
+    #                         np.datetime64('2020-03-01'), np.datetime64('2020-04-01'),
+    #                         np.datetime64('2020-05-01')])
+    # timesteps = np.array([np.datetime64('2023-01-01 00:00:00'),np.datetime64('2023-01-01 01:00:00'),
+    #                     np.datetime64('2023-01-01 02:00:00'),
+    #                     np.datetime64('2023-01-01 03:00:00') ])
+    # timesteps = np.array([np.datetime64('2023-01-01'), np.datetime64('2023-01-05'),
+    #                 np.datetime64('2023-01-10'),np.datetime64('2023-01-15')])
+
+    # timesteps = time_steps
+
+    # check if valid hour minutes seconds in date
+    valid_hms = has_hms(timesteps)
+
+    # if valid_hms == "duplicates" then the timesteps are duplicates 
+    # and can be dropped because it is just an irrelevent HMS for each timestamp
+    if valid_hms == "duplicates":
+        # convert HMS to days
+        timesteps = timesteps.astype('datetime64[D]')
+
+    # get the time differences between each timestep
+    time_diffs = [timesteps[i+1] - timesteps[i] for i in range(len(timesteps)-1)]
+
+    # IF no values in time_diffs
+    if len(time_diffs) == 0:
+        # return 0 and give warning if no values in time_diffs
+        # print("Warning: time_steps has only one value. Setting dT to 0")
+        return 0
+
+    return time_diffs
+
+def count_time_intervals(timesteps):
+    """Count the number of unique time intervals in a numpy array of timedelta objects
+
+    Args:
+        timesteps (np.array): np.array of np.timedelta64 objects
+    Returns:
+        dict: dictionary of unique time intervals and their counts
+        """
+
+    # timesteps  = np.array([np.datetime64('2020-01-01'),np.datetime64('2020-01-02'),
+    #                         np.datetime64('2020-01-03'),
+    #                         np.datetime64('2020-01-04')])
+
+    # convert timedelta object to string
+    time_diffs = [str(i) for i in timesteps]
+
+    # determine the most common interval
+    interval_count = Counter(time_diffs)
+
+    return interval_count
+
+def validate_time_interval(time_interval):
+    """Correct time interval string to a common interval
+
+    Typically function will take a time interval string with seconds and 
+    convert it to a common interval. For example, "86400 seconds" will become "1 day".
+
+    Args:
+        time_interval (str): time interval string in the format <time_value> <time_unit>
+
+    Returns:
+        str: corrected time interval string in the format <time_value> <time_unit>
+    """
+
+    # time_interval = most_freq
+    # verbose = True
+
+    # extract the time interval integer value and unit string
+    time_val = int(time_interval.split(" ")[0])
+    unit = time_interval.split(" ")[-1]
+
+    # if the unit value is "seconds" or "second", check if a common interval equists and convert it
+    if unit in ["seconds", "second"]:
+
+        # convert seconds to other common intervals
+        sec_convert = seconds_to_intervals(time_val)
+
+        # if a conversion exists, convert the time interval
+        if sec_convert:
+            # if verbose: 
+            #     print(f"Converting {time_val} seconds to {sec_convert}")
+            time_interval = sec_convert
+
+    # # if the unit value is "days" or "day", check if a common interval equists and convert it
+    # if unit in ["days", "day"]:
+    #     # convert days to other common intervals
+    #     day_convert = days_to_intervals(time_val)
+
+    #     # if a conversion exists, convert the time interval
+    #     if day_convert:
+    #         if verbose: 
+    #             print(f"Converting {time_val} days to {day_convert}")
+    #         time_interval = day_convert
+
+    # if verbose:
+    #     print(f"Most common time interval: {time_interval}")
+
+    # return the full string if only_units is False
+    return time_interval
+
+### VERSION 2 of _resource_time() function, dealing with Livneh issues 
+#### because of time interval being 0 (only a single timestamp in resource)
+
 def _resource_time(
         nc     = None,
         T_name = None
         ):
-    """Get information about the time variable in a NetCDF dataset
+    
+    """Get time information from a xarray netcdf file
+    
     Args:
-        nc (xarray.DataArray): xarray DataArray from a NetCDF file.
-        T_name (str): The name of the time variable.
-
+        nc (xarray.core.dataset.Dataset): netcdf file to extract time informations from
+        T_name (str, optional): name of the time variable. Defaults to None.
+    
     Returns:
-        dict: A dictionary containing the duration, interval, and number of time steps (nT).
-            - duration: The start and end dates of the time variable, formatted as "start_date/end_date".
-            - interval: The interval between time steps, formatted as "value units".
-            - nT: The number of time steps.
+        dict: dictionary of time information with duration, interval, and nT keys
     """
+
     # Time variable info
     T_var_info = nc[T_name]
-
+    
     # time variable units
     T_units    = T_var_info.attrs["units"].split(" ")[0]
-    
-    # time steps
+
+    # time variable values
     time_steps = xr.decode_cf(nc)[T_name].values
 
     # check if time steps are isoformatted
     # if isinstance(time_steps[0], cftime._cftime.DatetimeNoLeap):
     if not isinstance(time_steps[0], (datetime, np.datetime64)):
         vec_isoformat = np.vectorize(lambda x: datetime.fromisoformat(x.isoformat()))
 
         # apply the vectorized function to the dates array to get an array of isoformatted date strings
         time_steps = vec_isoformat(time_steps)
 
-    # time_steps = xr.decode_cf(nc).time.values
+    # get the time intervals between each datetime in the time_steps array
+    dT = get_time_intervals(time_steps)
 
-    # change in time dT
-    dT = time_steps[1:] - time_steps[:-1]
+    # Check that there is more than one time step (dT NOT equal to 0):
+    # Conditions breakdown:
+        # IF dT IS 0 (first 'if' condition), then the time interval is 0 (i.e. a dataset that has a single timestamp), 
+        # thus we will set the 'interval' variable to 0 and proceed on
+        # OTHERWISE (the else condition), if dT is NOT 0, then we will get the time interval info 
+        # for the timestamps/dataset (most common interval, verify correct units, check if monthly data, etc.)
+
+    # Case when there is only a single timestamp in the dataset
+    if not dT:
+        # if interval length is 0, set interval to 0
+        interval = "0"
 
-    if len(dT) == 0:
-        print("Warning: time_steps has only one value. Setting dT to 0")
-        dT = time_steps - time_steps
-        
-    # grid of time steps and units
-    g = pd.Series(dT).sort_values().value_counts().to_frame().reset_index()
+        # print("No time intervals found")
 
-    # rename columns
-    g.columns = ["value", "n"]
-    
-    # insert interval (units) column between value and n count
-    g.insert(g.columns.get_loc('value')+1, 'interval', T_units)  # insert new column
-    
-    # sort by days value
-    g = g.sort_values(by='value')
-    
-    # value in days
-    day_vals = (g["value"].values.astype('timedelta64[s]').astype(int)/86400).astype(int).tolist()
-    
-    # if the time interval is a month, set the interval to month
-    if len(g) > 1 and all(i in [28, 29, 30, 31] for i in day_vals):
-    # if len(g) > 1 and np.isin([28, 29, 30, 31], day_vals).all():
+    # Case when there are multiple timestamps in the dataset (typical case)
+    else: 
 
-        g = pd.DataFrame({"value": [1], "interval": ["months"]})
+        # print(f"Found {len(dT)} time intervals")
 
-    else:
-        # get the most common interval
-        g = g.iloc[[np.argmax(g["n"])], :]
+        # get the number of time intervals
+        interval_count = count_time_intervals(dT)
+
+        # get the interval values
+        interval_vals = [int(i.split(' ')[0]) for i in list(interval_count.keys())]
+
+        # get the interval units
+        interval_units = [i.split(' ')[-1] for i in list(interval_count.keys())]
+
+        # get the most common interval value
+        most_freq = interval_count.most_common(1)[0][0]
 
-    # time_steps.max() >= np.datetime64(datetime.now() - timedelta(days=5))
-    # time_steps.max() <=  np.datetime64(datetime.now() + timedelta(days=1))
+        # correct seconds to days if necessary
+        most_freq = validate_time_interval(most_freq)
+
+        # get the most common interval unit
+        good_units = most_freq.split(' ')[-1]
+
+        # switch T_units with good_units IF T_units does NOT equal the most common interval unit (good_units), set T_units to the most common interval unit
+        if T_units != good_units:
+            T_units = good_units
+
+        # (np.datetime64(int(most_freq.split(' ')[0]), "D")).astype('datetime64[s]').astype(int)/86400
+        # (np.datetime64(most_freq.split(' ')[0]).astype('datetime64[s]').astype(int)/86400).astype(int).tolist()
+        # (time_steps[0].astype('datetime64[s]').astype(int)/86400).astype(int).tolist()
+
+        # # value in days
+        # day_vals = (g["value"].values.astype('timedelta64[s]').astype(int)/86400).astype(int).tolist()
+        
+        # if the time interval is a month, make a dictionary with 1 month time intervals, 
+        #   otherwise, use most common interval and corrected units
+        if len(interval_vals) > 1 and all(i in [28, 29, 30, 31] for i in interval_vals):
+            time_dict = {
+                "value": 1,
+                "interval": "months"
+                }
+        else:
+            # get the most common interval
+            time_dict = {
+                "value": int(most_freq.split(' ')[0]),
+                "interval": good_units
+                }
+            
+        # create a string of the interval
+        interval = str(time_dict["value"]) + " " + time_dict["interval"]
 
-    # If time is within 5 days of today then we call the range Open
+        # format the interval string
+        interval = format_units(interval, T_units)
+    
+    # determine the max date of the time steps
+    # If time is within 5 days of today then we call the range open
     maxDate = np.where((time_steps.max() >=  np.datetime64(datetime.now() - timedelta(days=5)) and 
                         time_steps.max() <=  np.datetime64(datetime.now() + timedelta(days=1))),
                         "..",
                         str(time_steps.max())
                         ).item()
     
     # get length of the timesteps or if open, a None value
     if maxDate == "..":
         nT = None
     else:
         nT = len(time_steps)
 
-    # get length of the timesteps or if open, a None value
-    # nT = np.where(maxDate == "..", None, len(time_steps)).item()
-    
-    # create a string of the interval
-    interval = (g['value'].astype(str) + " " + g['interval'].astype(str)).iloc[0]
-
-    # format the interval string
-    interval = format_units(interval, T_units)
-
-    # if interval length is 0, set interval to 0
-    if len([interval]) == 0:
-        interval = "0"
-
+    # format_date(str(time_steps.min())) + "/" + (".." if maxDate == ".." else format_date(str(maxDate)))
+        
     # create a dictionary of the time attributes
     time_dict = {
         "duration" : format_date(str(time_steps.min())) + "/" + (".." if maxDate == ".." else format_date(str(maxDate))),
         "interval" : interval,
         "nT"       : nT
         }
 
     return time_dict
 
+# def _resource_time(
+#         nc     = None,
+#         T_name = None
+#         ):
+#     """Get information about the time variable in a NetCDF dataset
+#     Args:
+#         nc (xarray.DataArray): xarray DataArray from a NetCDF file.
+#         T_name (str): The name of the time variable.
+
+#     Returns:
+#         dict: A dictionary containing the duration, interval, and number of time steps (nT).
+#             - duration: The start and end dates of the time variable, formatted as "start_date/end_date".
+#             - interval: The interval between time steps, formatted as "value units".
+#             - nT: The number of time steps.
+#     """
+#     # Time variable info
+#     T_var_info = nc[T_name]
+
+#     # time variable units
+#     T_units    = T_var_info.attrs["units"].split(" ")[0]
+    
+#     # time steps
+#     time_steps = xr.decode_cf(nc)[T_name].values
+
+#     # if time unit is seconds, infer the frequency and 
+#     # check if inferred frequency is days ("D") if so, force the 'T_unit' value to days
+#     if T_units in ["second", "seconds"]:
+
+#         # infer the frequency of the time steps
+#         inferred_freq = pd.infer_freq(time_steps)
+
+#         # if the inferred frequency is NOT seconds, force the time unit to appropriate date interval 
+#         if inferred_freq != "S":
+#             T_units = match_date_abbr(inferred_freq)
+
+#     # check if time steps are isoformatted
+#     # if isinstance(time_steps[0], cftime._cftime.DatetimeNoLeap):
+#     if not isinstance(time_steps[0], (datetime, np.datetime64)):
+#         vec_isoformat = np.vectorize(lambda x: datetime.fromisoformat(x.isoformat()))
+
+#         # apply the vectorized function to the dates array to get an array of isoformatted date strings
+#         time_steps = vec_isoformat(time_steps)
+
+#     # time_steps = xr.decode_cf(nc).time.values
+
+#     # change in time dT
+#     dT = time_steps[1:] - time_steps[:-1]
+
+#     if len(dT) == 0:
+#         print("Warning: time_steps has only one value. Setting dT to 0")
+#         dT = time_steps - time_steps
+        
+#     # grid of time steps and units
+#     g = pd.Series(dT).sort_values().value_counts().to_frame().reset_index()
+
+#     # rename columns
+#     g.columns = ["value", "n"]
+    
+#     # insert interval (units) column between value and n count
+#     g.insert(g.columns.get_loc('value')+1, 'interval', T_units)  # insert new column
+    
+#     # sort by days value
+#     g = g.sort_values(by='value')
+    
+#     # value in days
+#     day_vals = (g["value"].values.astype('timedelta64[s]').astype(int)/86400).astype(int).tolist()
+    
+#     # if the time interval is a month, set the interval to month
+#     if len(g) > 1 and all(i in [28, 29, 30, 31] for i in day_vals):
+#     # if len(g) > 1 and np.isin([28, 29, 30, 31], day_vals).all():
+
+#         g = pd.DataFrame({"value": [1], "interval": ["months"]})
+
+#     else:
+#         # get the most common interval
+#         g = g.iloc[[np.argmax(g["n"])], :]
+
+#     # time_steps.max() >= np.datetime64(datetime.now() - timedelta(days=5))
+#     # time_steps.max() <=  np.datetime64(datetime.now() + timedelta(days=1))
+
+#     # If time is within 5 days of today then we call the range Open
+#     maxDate = np.where((time_steps.max() >=  np.datetime64(datetime.now() - timedelta(days=5)) and 
+#                         time_steps.max() <=  np.datetime64(datetime.now() + timedelta(days=1))),
+#                         "..",
+#                         str(time_steps.max())
+#                         ).item()
+    
+#     # get length of the timesteps or if open, a None value
+#     if maxDate == "..":
+#         nT = None
+#     else:
+#         nT = len(time_steps)
+
+#     # get length of the timesteps or if open, a None value
+#     # nT = np.where(maxDate == "..", None, len(time_steps)).item()
+    
+#     # create a string of the interval
+#     interval = (g['value'].astype(str) + " " + g['interval'].astype(str)).iloc[0]
+
+#     # format the interval string
+#     interval = format_units(interval, T_units)
+
+#     # if interval length is 0, set interval to 0
+#     if len([interval]) == 0:
+#         interval = "0"
+
+#     # create a dictionary of the time attributes
+#     time_dict = {
+#         "duration" : format_date(str(time_steps.min())) + "/" + (".." if maxDate == ".." else format_date(str(maxDate))),
+#         "interval" : interval,
+#         "nT"       : nT
+#         }
+
+#     return time_dict
+
 def _resource_grid(
         nc, 
         X_name               = None,
         Y_name               = None, 
         stopIfNotEqualSpaced = True
         ):
     
-    """
-    Extract grid information from a xarray/NetCDF
+    """Extract grid information from a xarray/NetCDF
 
     Parameters:
         nc (xarray.DataArray): xarray DataArray from a NetCDF file.
         X_name (str): The name of the X coordinate variable. If None, it will be extracted from the NetCDF attributes.
         Y_name (str): The name of the Y coordinate variable. If None, it will be extracted from the NetCDF attributes.
         stopIfNotEqualSpaced (bool): If True, raise a warning or an exception if the grid cells are not equally spaced (default is True).
```

### Comparing `climatePy-0.4.37/climatePy/data/catalog.csv` & `climatePy-0.4.38/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.38/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.37
+Version: 0.4.38
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Author-email: anguswatters@gmail.com, mikecp11@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `climatePy-0.4.37/setup.py` & `climatePy-0.4.38/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.37',
+    version='0.4.38',
     author="Angus Watters, Mike Johnson",     # authors
     author_email = "anguswatters@gmail.com, mikecp11@gmail.com",
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
```

### Comparing `climatePy-0.4.37/tests/test_extract_sites.py` & `climatePy-0.4.38/tests/test_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.37/tests/test_shortcuts.py` & `climatePy-0.4.38/tests/test_shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
 
 # @pytest.fixture(params=['miami_dade_county', 'san_luis_obispo_county', 
 #                         'litchfield_county', 'tuscaloosa_county', 
 #                         'boulder_county', 'king_county'])
 
 @pytest.fixture(params=['san_luis_obispo_county', 'boulder_county'])
+# @pytest.fixture(params=['san_luis_obispo_county'])
 
 def AOI(request): 
     # filepath = f'src/data/{request.param}.gpkg'
     filepath = f'climatePy/data/{request.param}.gpkg'
     AOI = gpd.read_file(filepath)
     yield AOI
 
@@ -1100,7 +1101,159 @@
     assert output["Gypsisols"].attrs['crs'] == "EPSG:4326"
 
     # assert len(output["Vertisols"]) == 432
     # assert len(output["Gypsisols"]) == 432
 
     # assert output['Vertisols'].shape == (432, 945)
     # assert output['Gypsisols'].shape == (432, 945)
+
+def test_getCHIRPS_case1(AOI):
+	#  ---- Case 1: Single month CHIRPS ----
+	verbose   = True
+	startDate = "2019-01-01"
+	endDate   = "2019-01-01"
+	varname       = 'precip'
+	timeRes = "daily"
+	
+	# Call function to get output
+	output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+
+	# Assert that the output is a dictionary
+	assert type(output) == dict
+
+	# Assert that the output dictionary has the correct keys
+	assert set(output.keys()) == {"precip"}
+	
+	# Assert that the values of the output dictionary are xarray DataArrays
+	assert isinstance(output["precip"], xr.DataArray)
+
+	# Assert that the dimensions of the output DataArrays are correct
+	assert output["precip"].dims == ("y", "x", "time")
+
+	# Assert that the temporal resolution of the output DataArrays is correct
+	start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+	end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+	# check temporal range
+	assert end_date1 - start_date1 == pd.Timedelta("0D")
+
+	assert "precip" in output["precip"].time[0].values.item()
+
+	# assert len(output["precip"].time.values) == 1
+	# assert output['precip'].shape == (19, 40, 1)
+
+def test_getCHIRPS_case2(AOI):
+	#  ---- Case 2: Multi Month CHIRPS ----
+	verbose   = True
+	startDate = "2019-01-01"
+	endDate   = "2019-03-01"
+	varname       = 'precip'
+	timeRes = "daily"
+
+	# Call function to get output
+	output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+
+	# Assert that the output is a dictionary
+	assert type(output) == dict
+
+	# Assert that the output dictionary has the correct keys
+	assert set(output.keys()) == {"precip"}
+	
+	# Assert that the values of the output dictionary are xarray DataArrays
+	assert isinstance(output["precip"], xr.DataArray)
+
+	# Assert that the dimensions of the output DataArrays are correct
+	assert output["precip"].dims == ("y", "x", "time")
+
+	# Assert that the temporal resolution of the output DataArrays is correct
+	start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+	end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+	# check temporal range
+	assert end_date1 - start_date1 == pd.Timedelta("59D")
+
+	assert "precip" in output["precip"].time[0].values.item()
+
+	# assert len(output["precip"].time.values) == 3
+	# assert output['precip'].shape == (19, 40, 3)
+
+
+def test_getCHIRPS_case3(AOI):
+	#  ---- Case 3: Multi Year Month CHIRPS ----
+	verbose   = True
+	startDate = "2019-01-01"
+	endDate   = "2020-02-01"
+	varname       = 'precip'
+	timeRes = "daily"
+
+	# Call function to get output
+	output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+
+	# Assert that the output is a dictionary
+	assert type(output) == dict
+
+	# Assert that the output dictionary has the correct keys
+	assert set(output.keys()) == {"precip"}
+	
+	# Assert that the values of the output dictionary are xarray DataArrays
+	assert isinstance(output["precip"], xr.DataArray)
+
+	# Assert that the dimensions of the output DataArrays are correct
+	assert output["precip"].dims == ("y", "x", "time")
+
+	# Assert that the temporal resolution of the output DataArrays is correct
+	start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}',
+					output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+	
+	end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', 
+					output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+	# check temporal range
+	assert end_date1 - start_date1 == pd.Timedelta("396D")
+
+	assert "precip" in output["precip"].time[0].values.item()
+
+	# assert len(output["precip"].time.values) == 14
+	# assert output['precip'].shape == (19, 40, 14)
+
+def test_getCHIRPS_case4(AOI):
+	#  ---- Case 4: Monthly Multi Year CHIRPS ----
+	verbose   = True
+	startDate = "2019-01-01"
+	endDate   = "2020-02-01"
+	varname       = 'precip'
+	timeRes = "monthly"
+
+	# Call function to get output
+	output = climatePy.getCHIRPS(AOI, varname, startDate, endDate, timeRes, verbose)
+
+	# Assert that the output is a dictionary
+	assert type(output) == dict
+
+	# Assert that the output dictionary has the correct keys
+	assert set(output.keys()) == {"precip"}
+	
+	# Assert that the values of the output dictionary are xarray DataArrays
+	assert isinstance(output["precip"], xr.DataArray)
+
+	# Assert that the dimensions of the output DataArrays are correct
+	assert output["precip"].dims == ("y", "x", "time")
+
+	# Assert that the temporal resolution of the output DataArrays is correct
+	start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}',
+					output["precip"].time[0].values.item()).group(0), "%Y-%m-%d")
+	
+	end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', 
+					output["precip"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+	# check temporal range
+	assert end_date1 - start_date1 == pd.Timedelta("396D")
+	assert "precip" in output["precip"].time[0].values.item()
+
+	# calculate number of months
+	months = (end_date1.year - start_date1.year) * 12 + end_date1.month - start_date1.month
+	months = months + 1 if end_date1.day >= end_date1.day else months
+
+	# check that number of months in output is correct (within 1 month)
+	assert (len(output["precip"]['time']) == months or
+			len(output["precip"]['time']) + 1 == months or
+			len(output["precip"]['time']) - 1 == months)
```

### Comparing `climatePy-0.4.37/tests/test_utils.py` & `climatePy-0.4.38/tests/test_utils.py`

 * *Files identical despite different names*

