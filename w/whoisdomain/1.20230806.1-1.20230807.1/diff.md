# Comparing `tmp/whoisdomain-1.20230806.1.tar.gz` & `tmp/whoisdomain-1.20230807.1.tar.gz`

## Comparing `whoisdomain-1.20230806.1.tar` & `whoisdomain-1.20230807.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     4823 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/_0_init_tld.py
--rwxr-xr-x   0        0        0     2486 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/__init__.py
--rwxr-xr-x   0        0        0     2331 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/doParse.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/doQuery.py
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/doWhoisCommand.py
--rwxr-xr-x   0        0        0     4753 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/domain.py
--rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/exceptions.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/handleDateStrings.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/lastWhois.py
--rwxr-xr-x   0        0        0    19904 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/main.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/noneStrings.py
--rwxr-xr-x   0        0        0     6022 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/parameterContext.py
--rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/processWhoisDomainRequest.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/quotaStrings.py
--rwxr-xr-x   0        0        0     1498 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/simpleCacheBase.py
--rwxr-xr-x   0        0        0     1681 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/simpleCacheWithFile.py
--rwxr-xr-x   0        0        0   131874 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/tld_regexpr.py
--rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/version.py
--rwxr-xr-x   0        0        0     6141 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/whoisCliInterface.py
--rwxr-xr-x   0        0        0     8786 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/whoisdomain/whoisParser.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/LICENSE
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/README.md
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/pyproject.toml
--rw-r--r--   0        0        0    12252 2020-02-02 00:00:00.000000 whoisdomain-1.20230806.1/PKG-INFO
+-rwxr-xr-x   0        0        0     4823 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/_0_init_tld.py
+-rwxr-xr-x   0        0        0     2486 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/__init__.py
+-rwxr-xr-x   0        0        0     2331 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/doParse.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/doQuery.py
+-rwxr-xr-x   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/doWhoisCommand.py
+-rwxr-xr-x   0        0        0     4753 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/domain.py
+-rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/exceptions.py
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/handleDateStrings.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/lastWhois.py
+-rwxr-xr-x   0        0        0    19904 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/main.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/noneStrings.py
+-rwxr-xr-x   0        0        0     6057 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/parameterContext.py
+-rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/processWhoisDomainRequest.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/quotaStrings.py
+-rwxr-xr-x   0        0        0     1777 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/simpleCacheBase.py
+-rwxr-xr-x   0        0        0     1769 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/simpleCacheWithFile.py
+-rwxr-xr-x   0        0        0   131874 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/tld_regexpr.py
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/version.py
+-rwxr-xr-x   0        0        0     6234 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/whoisCliInterface.py
+-rwxr-xr-x   0        0        0     8786 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/whoisdomain/whoisParser.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/LICENSE
+-rw-r--r--   0        0        0    11473 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/README.md
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/pyproject.toml
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 whoisdomain-1.20230807.1/PKG-INFO
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230807.1/whoisdomain/_0_init_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/__init__.py` & `whoisdomain-1.20230807.1/whoisdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/doParse.py` & `whoisdomain-1.20230807.1/whoisdomain/doParse.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/doQuery.py` & `whoisdomain-1.20230807.1/whoisdomain/doQuery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 
 from typing import (
     Optional,
 )
 
 from .domain import Domain
 from .parameterContext import ParameterContext
@@ -72,15 +73,18 @@
             ignore_returncode=ignore_returncode,
             server=server,
             verbose=verbose,
             with_cleanup_results=with_cleanup_results,
             internationalized=internationalized,
             include_raw_whois_text=include_raw_whois_text,
             return_raw_text_for_unsupported_tld=return_raw_text_for_unsupported_tld,
-            timeout=float(timeout) if timeout else float(0),
+            timeout=timeout,
             parse_partial_response=parse_partial_response,
             cmd=cmd,
             simplistic=simplistic,
             withRedacted=withRedacted,
         )
 
+    if verbose:
+        print(pc, file=sys.stderr)
+
     return q2(domain=domain, pc=pc)
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/doWhoisCommand.py` & `whoisdomain-1.20230807.1/whoisdomain/doWhoisCommand.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!  /usr/bin/env python3
 
-# import sys
+import sys
 
 # from .simpleCacheBase import SimpleCacheBase
 from .simpleCacheWithFile import SimpleCacheWithFile
 
 from typing import (
     # Dict,
     List,
@@ -31,18 +31,17 @@
     if CACHE_STUB is None:
         # if no cache defined init the default cache (optional with file storage based on pc)
         CACHE_STUB = SimpleCacheWithFile(
             verbose=pc.verbose,
             cacheFilePath=pc.cache_file,
             cacheMaxAge=pc.cache_age,
         )
-
-    # allways test CACHE_STUB is a subclass of SimpleCacheBase
-    # if pc.withVerifyCacheStubType:
-    #   assert isinstance(CACHE_STUB, SimpleCacheBase), Exception("CACHE_STUB - must inherit from SimpleCacheBase")
+    else:
+        if pc.verbose:
+            print("cache already initialized", file=sys.stderr)
 
     return CACHE_STUB
 
 
 def _getNewDataForKey(
     dList: List[str],
     pc: ParameterContext,
@@ -58,14 +57,17 @@
 def doWhoisAndReturnString(
     dList: List[str],
     pc: ParameterContext,
 ) -> str:
     cache = _initDefaultCache(pc)
     keyString = ".".join(dList)
 
+    if pc.verbose:
+        print(f"force: {pc.force}", file=sys.stderr)
+
     if pc.force is False:
         oldData: Optional[str] = cache.get(keyString)
         if oldData is not None:
             return str(oldData)
 
     newData = _getNewDataForKey(dList=dList, pc=pc)
     cache.put(keyString, newData)
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/domain.py` & `whoisdomain-1.20230807.1/whoisdomain/domain.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/exceptions.py` & `whoisdomain-1.20230807.1/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/handleDateStrings.py` & `whoisdomain-1.20230807.1/whoisdomain/handleDateStrings.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/lastWhois.py` & `whoisdomain-1.20230807.1/whoisdomain/lastWhois.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/main.py` & `whoisdomain-1.20230807.1/whoisdomain/main.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/noneStrings.py` & `whoisdomain-1.20230807.1/whoisdomain/noneStrings.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/parameterContext.py` & `whoisdomain-1.20230807.1/whoisdomain/parameterContext.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     "optional": true,
     "default": 0,
     "help": "Time [s] it will wait after you query WHOIS database."
   },
   "timeout": {
     "type": "float",
     "optional": true,
-    "default": null,
+    "default": 30.0,
     "help": "timeout in seconds for the whois command to return a result."
   }
 }
 """
 
 
 class ParameterContext:
@@ -202,15 +202,15 @@
                 msg = f"unknown type: {t} for {name}"
                 raise TypeError(msg)
 
             if value is not None:
                 if not isinstance(value, self.KT[t]):
                     msg = f"unknown type: {t} for {name}, {value}"
                     raise TypeError(msg)
-
-            self.value[name] = value
+                self.value[name] = value
+            # leave the default
 
 
 if __name__ == "__main__":
     domain: str = "haha.ha"
     pc = ParameterContext(domain=domain)
     print(pc.value)
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/processWhoisDomainRequest.py` & `whoisdomain-1.20230807.1/whoisdomain/processWhoisDomainRequest.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/quotaStrings.py` & `whoisdomain-1.20230807.1/whoisdomain/quotaStrings.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/simpleCacheBase.py` & `whoisdomain-1.20230807.1/whoisdomain/simpleCacheBase.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,60 +8,67 @@
     Dict,
     Optional,
     Tuple,
 )
 
 
 class SimpleCacheBase:
-    verbose: bool = False
-    memCache: Dict[str, Tuple[float, str]] = {}
-    cacheMaxAge: int = 60 * 60 * 48
+    # verbose: bool = False
+    # memCache: Dict[str, Tuple[float, str]] = {}
+    # cacheMaxAge: int = 60 * 60 * 48
 
     def __init__(
         self,
         verbose: bool = False,
         cacheMaxAge: int = (60 * 60 * 48),
     ) -> None:
         self.verbose = verbose
-        self.memCache = {}
-        self.cacheMaxAge = cacheMaxAge
+        self.memCache: Dict[str, Tuple[float, str]] = {}
+        self.cacheMaxAge: int = cacheMaxAge
+
+        if self.verbose:
+            print("init SimpleCacheBase", file=sys.stderr)
 
     def put(
         self,
         keyString: str,
         data: str,
     ) -> str:
         if self.verbose:
             print(f"put: {keyString}", file=sys.stderr)
 
+        # print(f"put: {keyString}", file=sys.stderr)
+
         # store the currentTime and data tuple (time, data)
         self.memCache[keyString] = (
             int(time.time()),
             data,
         )
         return data
 
     def get(
         self,
         keyString: str,
     ) -> Optional[str]:
+        if self.verbose:
+            print(f"get: {keyString}", file=sys.stderr)
+        # print(f"get: {keyString}", file=sys.stderr)
+        # print(f"verbose: {self.verbose}", file=sys.stderr)
 
         cData = self.memCache.get(keyString)
         if cData is None:
             if self.verbose:
-                print(f"get: no data for {keyString}", file=sys.stderr)
+                print("get: no data", file=sys.stderr)
             return None
 
         t = time.time()
         hasExpired = cData[0] < (t - self.cacheMaxAge)
         if hasExpired is True:
             if self.verbose:
                 print(f"get: data has expired {keyString} {cData[0]}, {t}, {self.cacheMaxAge}", file=sys.stderr)
             return None
 
-        if self.verbose:
-            print(f"get: {keyString}", file=sys.stderr)
         return cData[1]
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/simpleCacheWithFile.py` & `whoisdomain-1.20230807.1/whoisdomain/simpleCacheWithFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         self,
         verbose: bool = False,
         cacheFilePath: Optional[str] = None,
         cacheMaxAge: int = (60 * 60 * 48),
     ) -> None:
         super().__init__(verbose=verbose, cacheMaxAge=cacheMaxAge)
         self.cacheFilePath = cacheFilePath
+        if self.verbose:
+            print("init SimpleCacheWithFile", file=sys.stderr)
 
     def _fileLoad(
         self,
     ) -> None:
         if self.cacheFilePath is None:
             return
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230807.1/whoisdomain/tld_regexpr.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/whoisdomain/whoisCliInterface.py` & `whoisdomain-1.20230807.1/whoisdomain/whoisCliInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
         self.processHandle = subprocess.Popen(
             # STDBUF_OFF_CMD needed to not lose data on kill
             self.STDBUF_OFF_CMD + self.makeWhoisCommandToRun(),
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             env={"LANG": "en"} if self.dList[-1] in ".jp" else None,
         )
+        if self.pc.verbose:
+            print(f"timout: {self.pc.timeout}", file=sys.stderr)
 
         try:
             self.rawWhoisResultString = self.processHandle.communicate(timeout=self.pc.timeout,)[
                 0
             ].decode(errors="ignore")
         except subprocess.TimeoutExpired:
             # Kill the child process & flush any output buffers
```

### Comparing `whoisdomain-1.20230806.1/whoisdomain/whoisParser.py` & `whoisdomain-1.20230807.1/whoisdomain/whoisParser.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/.gitignore` & `whoisdomain-1.20230807.1/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/LICENSE` & `whoisdomain-1.20230807.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/README.md` & `whoisdomain-1.20230807.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -225,7 +225,9 @@
   * 1.20230804.1 testing
   * 1.20230804.2 testing after remove of leading dot in rw second level domains
   * 1.20230804.3 simplefy cache implementation after feedback from `baderdean`
   * "more lembas bread", refactor parse and query
   * remove option to typecheck CACHE_STUB, use try/catch/exit instead, does not work when timout happens, removed ;-(
   * refactor doQuery create processWhoisDomainRequest, split of lastWhois
   * 1.20230806.1 testing done, prep new release: "more lembas bread"
+  * bug found with the default timeout: if no timeout is specified the program fails: all pypi released befote 2023-07-17 yanked
+  * 1.20230807.1 fix default timeout
```

### Comparing `whoisdomain-1.20230806.1/pyproject.toml` & `whoisdomain-1.20230807.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230806.1/PKG-INFO` & `whoisdomain-1.20230807.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230806.1
+Version: 1.20230807.1
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -247,7 +247,9 @@
   * 1.20230804.1 testing
   * 1.20230804.2 testing after remove of leading dot in rw second level domains
   * 1.20230804.3 simplefy cache implementation after feedback from `baderdean`
   * "more lembas bread", refactor parse and query
   * remove option to typecheck CACHE_STUB, use try/catch/exit instead, does not work when timout happens, removed ;-(
   * refactor doQuery create processWhoisDomainRequest, split of lastWhois
   * 1.20230806.1 testing done, prep new release: "more lembas bread"
+  * bug found with the default timeout: if no timeout is specified the program fails: all pypi released befote 2023-07-17 yanked
+  * 1.20230807.1 fix default timeout
```

