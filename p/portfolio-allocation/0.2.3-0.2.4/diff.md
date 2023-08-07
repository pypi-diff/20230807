# Comparing `tmp/portfolio_allocation-0.2.3.tar.gz` & `tmp/portfolio_allocation-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_allocation-0.2.3.tar", last modified: Tue May 30 18:50:31 2023, max compression
+gzip compressed data, was "portfolio_allocation-0.2.4.tar", last modified: Mon Aug  7 18:58:44 2023, max compression
```

## Comparing `portfolio_allocation-0.2.3.tar` & `portfolio_allocation-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.657543 portfolio_allocation-0.2.3/portfolio_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/gnucash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/funds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/report/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.657543 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:50:31.665543 portfolio_allocation-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/portfolio_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/gnucash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/portfolio_allocation/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/funds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/portfolio_allocation/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/portfolio_allocation/report/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/report/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/report/resources/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/report/resources/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/portfolio_allocation/report/resources/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-07 18:58:44.000000 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-07 18:58:44.000000 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:58:44.000000 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 18:58:44.000000 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-07 18:58:44.000000 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 18:58:44.000000 portfolio_allocation-0.2.4/portfolio_allocation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 18:58:44.706703 portfolio_allocation-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-08-07 18:58:35.000000 portfolio_allocation-0.2.4/setup.py
```

### Comparing `portfolio_allocation-0.2.3/LICENSE` & `portfolio_allocation-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/PKG-INFO` & `portfolio_allocation-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_allocation
-Version: 0.2.3
+Version: 0.2.4
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.3/README.md` & `portfolio_allocation-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/cli.py` & `portfolio_allocation-0.2.4/portfolio_allocation/cli.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/gnucash.py` & `portfolio_allocation-0.2.4/portfolio_allocation/gnucash.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/instruments/instruments.py` & `portfolio_allocation-0.2.4/portfolio_allocation/instruments/instruments.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/currencies.py` & `portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/currencies.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/custom.py` & `portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/custom.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/funds.py` & `portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/funds.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 def _tinkoff(instrument: str) -> dict:
     url = "https://www.tinkoff.ru/invest/etfs/" + instrument
     print("Sending request GET " + url)
     start = time.time()
     r = requests.get(url)
     print("Got response in " + str(time.time() - start) + " seconds")
     r.encoding = 'UTF-8'
-    group = re.search("<script id=\"__REACT_QUERY_STATE__invest\" type=\"application/json\">(.*)</script><script>", r.text).group(1) \
+    group = re.search("<script id=\"__REACT_QUERY_STATE__invest\" type=\"application/json\">(.*?)</script>", r.text).group(1) \
         .replace('\\\\"', '')
     data = json.loads(group)
     try:
         response_data = data['queries'][0]['state']['data']['detail']
     except IndexError:
         raise _InstrumentMissingException
     return asdict(InstrumentData(
```

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/securities.py` & `portfolio_allocation-0.2.4/portfolio_allocation/instruments/sources/securities.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/report/report.py` & `portfolio_allocation-0.2.4/portfolio_allocation/report/report.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.css` & `portfolio_allocation-0.2.4/portfolio_allocation/report/resources/main.css`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.js` & `portfolio_allocation-0.2.4/portfolio_allocation/report/resources/main.js`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation.egg-info/PKG-INFO` & `portfolio_allocation-0.2.4/portfolio_allocation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-allocation
-Version: 0.2.3
+Version: 0.2.4
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.3/portfolio_allocation.egg-info/SOURCES.txt` & `portfolio_allocation-0.2.4/portfolio_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.3/setup.py` & `portfolio_allocation-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name="portfolio_allocation",
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.3",
+    version="0.2.4",
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds",
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -122,15 +122,15 @@
     python_requires=">=3.9",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['appdirs==1.4.4', 'banal==1.0.6', "beautifulsoup4==4.12.2; python_full_version >= '3.6.0'", 'cache-to-disk==2.0.0', "certifi==2023.5.7; python_version >= '3.6'", 'cffi==1.15.1', "chardet==5.1.0; python_version >= '3.7'", "charset-normalizer==3.1.0; python_full_version >= '3.7.0'", 'countrynames==1.15.0', "cryptography==40.0.2; python_version >= '3.6'", "frozendict==2.3.8; python_version >= '3.6'", "html5lib==1.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", "idna==3.4; python_version >= '3.5'", "jellyfish==0.11.2; python_version >= '3.7'", "lxml==4.9.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", 'multitasking==0.0.11', 'normality==2.4.0', "numpy==1.24.3; python_version >= '3.8'", "pandas==2.0.2; python_version >= '3.8'", 'pycountry==22.3.5', 'pycparser==2.21', "python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", 'pytz==2023.3', "pyyaml==6.0; python_version >= '3.6'", 'requests==2.31.0', "setuptools==67.8.0; python_version >= '3.7'", "six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", "soupsieve==2.4.1; python_version >= '3.7'", 'text-unidecode==1.3', "tzdata==2023.3; python_version >= '2'", "urllib3==2.0.2; python_version >= '3.7'", 'webencodings==0.5.1', 'yfinance==0.2.18'],
+    install_requires=['appdirs==1.4.4', 'banal==1.0.6', "beautifulsoup4==4.12.2; python_full_version >= '3.6.0'", 'cache-to-disk==2.0.0', "certifi==2023.7.22; python_version >= '3.6'", "chardet==5.2.0; python_version >= '3.7'", "charset-normalizer==3.2.0; python_full_version >= '3.7.0'", 'countrynames==1.15.2', "frozendict==2.3.8; python_version >= '3.6'", "html5lib==1.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", "idna==3.4; python_version >= '3.5'", "jellyfish==1.0.0; python_version >= '3.7'", "lxml==4.9.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", 'multitasking==0.0.11', 'normality==2.4.0', "numpy==1.25.2; python_version >= '3.9'", "pandas==2.0.3; python_version >= '3.8'", 'pycountry==22.3.5', "python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", 'pytz==2023.3', "pyyaml==6.0.1; python_version >= '3.6'", 'requests==2.31.0', "setuptools==68.0.0; python_version >= '3.7'", "six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", "soupsieve==2.4.1; python_version >= '3.7'", 'text-unidecode==1.3', "tzdata==2023.3; python_version >= '2'", "urllib3==2.0.4; python_version >= '3.7'", 'webencodings==0.5.1', 'yfinance==0.2.27'],
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```

