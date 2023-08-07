# Comparing `tmp/riprova-0.2.7.tar.gz` & `tmp/riprova-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riprova-0.2.7.tar", last modified: Fri Aug 24 18:18:50 2018, max compression
+gzip compressed data, was "riprova-0.3.1.tar", last modified: Mon Aug  7 09:23:08 2023, max compression
```

## Comparing `riprova-0.2.7.tar` & `riprova-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 h2non      (501) staff       (20)        0 2018-08-24 18:18:50.000000 riprova-0.2.7/
--rw-r--r--   0 h2non      (501) staff       (20)    14859 2018-08-24 18:18:50.000000 riprova-0.2.7/PKG-INFO
--rwxr-xr-x   0 h2non      (501) staff       (20)     1066 2016-12-24 13:06:38.000000 riprova-0.2.7/LICENSE
--rw-r--r--   0 h2non      (501) staff       (20)       12 2018-03-21 13:23:45.000000 riprova-0.2.7/requirements.txt
--rw-r--r--   0 h2non      (501) staff       (20)       77 2016-12-24 11:46:43.000000 riprova-0.2.7/MANIFEST.in
--rwxr-xr-x   0 h2non      (501) staff       (20)     3341 2018-08-24 18:17:28.000000 riprova-0.2.7/setup.py
--rwxr-xr-x   0 h2non      (501) staff       (20)      287 2017-01-06 10:54:44.000000 riprova-0.2.7/requirements-dev.txt
--rwxr-xr-x   0 h2non      (501) staff       (20)     2424 2018-08-24 18:06:55.000000 riprova-0.2.7/History.rst
--rw-r--r--   0 h2non      (501) staff       (20)       38 2018-08-24 18:18:50.000000 riprova-0.2.7/setup.cfg
--rwxr-xr-x   0 h2non      (501) staff       (20)     8602 2018-03-20 02:39:25.000000 riprova-0.2.7/README.rst
-drwxr-xr-x   0 h2non      (501) staff       (20)        0 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova.egg-info/
--rw-r--r--   0 h2non      (501) staff       (20)    14859 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova.egg-info/PKG-INFO
--rw-r--r--   0 h2non      (501) staff       (20)        1 2018-08-24 18:18:48.000000 riprova-0.2.7/riprova.egg-info/not-zip-safe
--rw-r--r--   0 h2non      (501) staff       (20)      562 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova.egg-info/SOURCES.txt
--rw-r--r--   0 h2non      (501) staff       (20)       12 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova.egg-info/requires.txt
--rw-r--r--   0 h2non      (501) staff       (20)        8 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova.egg-info/top_level.txt
--rw-r--r--   0 h2non      (501) staff       (20)        1 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova.egg-info/dependency_links.txt
-drwxr-xr-x   0 h2non      (501) staff       (20)        0 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova/
--rw-r--r--   0 h2non      (501) staff       (20)    11416 2018-08-24 18:06:13.000000 riprova-0.2.7/riprova/retrier.py
-drwxr-xr-x   0 h2non      (501) staff       (20)        0 2018-08-24 18:18:50.000000 riprova-0.2.7/riprova/strategies/
--rw-r--r--   0 h2non      (501) staff       (20)      260 2016-12-24 15:47:25.000000 riprova-0.2.7/riprova/strategies/__init__.py
--rw-r--r--   0 h2non      (501) staff       (20)     6545 2018-03-20 02:39:25.000000 riprova-0.2.7/riprova/strategies/exponential.py
--rw-r--r--   0 h2non      (501) staff       (20)     2189 2017-01-02 17:45:20.000000 riprova-0.2.7/riprova/strategies/constant.py
--rw-r--r--   0 h2non      (501) staff       (20)     3018 2018-08-24 18:06:13.000000 riprova-0.2.7/riprova/strategies/fibonacci.py
--rw-r--r--   0 h2non      (501) staff       (20)      239 2016-12-25 11:30:00.000000 riprova-0.2.7/riprova/constants.py
--rwxr-xr-x   0 h2non      (501) staff       (20)      932 2018-08-24 18:07:52.000000 riprova-0.2.7/riprova/__init__.py
--rw-r--r--   0 h2non      (501) staff       (20)     1112 2017-01-02 17:00:36.000000 riprova-0.2.7/riprova/backoff.py
--rw-r--r--   0 h2non      (501) staff       (20)     4676 2017-01-11 10:14:30.000000 riprova-0.2.7/riprova/retry.py
--rw-r--r--   0 h2non      (501) staff       (20)     1560 2018-08-24 18:06:13.000000 riprova-0.2.7/riprova/exceptions.py
--rw-r--r--   0 h2non      (501) staff       (20)     3545 2016-12-30 19:20:57.000000 riprova-0.2.7/riprova/errors.py
--rw-r--r--   0 h2non      (501) staff       (20)    11086 2018-08-24 18:06:13.000000 riprova-0.2.7/riprova/async_retrier.py
+drwxr-xr-x   0 h2non      (501) staff       (20)        0 2023-08-07 09:23:08.751425 riprova-0.3.1/
+-rwxr-xr-x   0 h2non      (501) staff       (20)     2533 2023-05-20 22:54:38.000000 riprova-0.3.1/History.rst
+-rwxr-xr-x   0 h2non      (501) staff       (20)     1066 2023-05-20 22:53:31.000000 riprova-0.3.1/LICENSE
+-rw-r--r--   0 h2non      (501) staff       (20)       77 2023-05-20 22:53:31.000000 riprova-0.3.1/MANIFEST.in
+-rw-r--r--   0 h2non      (501) staff       (20)    12243 2023-08-07 09:23:08.751211 riprova-0.3.1/PKG-INFO
+-rwxr-xr-x   0 h2non      (501) staff       (20)     8444 2023-06-05 18:49:47.000000 riprova-0.3.1/README.rst
+-rwxr-xr-x   0 h2non      (501) staff       (20)      287 2023-05-20 22:53:31.000000 riprova-0.3.1/requirements-dev.txt
+-rw-r--r--   0 h2non      (501) staff       (20)       12 2023-05-20 22:53:31.000000 riprova-0.3.1/requirements.txt
+drwxr-xr-x   0 h2non      (501) staff       (20)        0 2023-08-07 09:23:08.750025 riprova-0.3.1/riprova/
+-rwxr-xr-x   0 h2non      (501) staff       (20)      826 2023-06-05 18:54:10.000000 riprova-0.3.1/riprova/__init__.py
+-rw-r--r--   0 h2non      (501) staff       (20)    10726 2023-06-05 18:53:45.000000 riprova-0.3.1/riprova/async_retrier.py
+-rw-r--r--   0 h2non      (501) staff       (20)     1112 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/backoff.py
+-rw-r--r--   0 h2non      (501) staff       (20)      274 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/constants.py
+-rw-r--r--   0 h2non      (501) staff       (20)     3545 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/errors.py
+-rw-r--r--   0 h2non      (501) staff       (20)     1560 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/exceptions.py
+-rw-r--r--   0 h2non      (501) staff       (20)    11416 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/retrier.py
+-rw-r--r--   0 h2non      (501) staff       (20)     4676 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/retry.py
+drwxr-xr-x   0 h2non      (501) staff       (20)        0 2023-08-07 09:23:08.751068 riprova-0.3.1/riprova/strategies/
+-rw-r--r--   0 h2non      (501) staff       (20)      260 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/strategies/__init__.py
+-rw-r--r--   0 h2non      (501) staff       (20)     2189 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/strategies/constant.py
+-rw-r--r--   0 h2non      (501) staff       (20)     6545 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/strategies/exponential.py
+-rw-r--r--   0 h2non      (501) staff       (20)     3018 2023-05-20 22:53:31.000000 riprova-0.3.1/riprova/strategies/fibonacci.py
+drwxr-xr-x   0 h2non      (501) staff       (20)        0 2023-08-07 09:23:08.750645 riprova-0.3.1/riprova.egg-info/
+-rw-r--r--   0 h2non      (501) staff       (20)    12243 2023-08-07 09:23:08.000000 riprova-0.3.1/riprova.egg-info/PKG-INFO
+-rw-r--r--   0 h2non      (501) staff       (20)      562 2023-08-07 09:23:08.000000 riprova-0.3.1/riprova.egg-info/SOURCES.txt
+-rw-r--r--   0 h2non      (501) staff       (20)        1 2023-08-07 09:23:08.000000 riprova-0.3.1/riprova.egg-info/dependency_links.txt
+-rw-r--r--   0 h2non      (501) staff       (20)        1 2023-08-07 09:20:59.000000 riprova-0.3.1/riprova.egg-info/not-zip-safe
+-rw-r--r--   0 h2non      (501) staff       (20)       12 2023-08-07 09:23:08.000000 riprova-0.3.1/riprova.egg-info/requires.txt
+-rw-r--r--   0 h2non      (501) staff       (20)        8 2023-08-07 09:23:08.000000 riprova-0.3.1/riprova.egg-info/top_level.txt
+-rw-r--r--   0 h2non      (501) staff       (20)       38 2023-08-07 09:23:08.751457 riprova-0.3.1/setup.cfg
+-rwxr-xr-x   0 h2non      (501) staff       (20)     3296 2023-05-20 22:53:31.000000 riprova-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `riprova-0.2.7/LICENSE` & `riprova-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/setup.py` & `riprova-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,22 +86,21 @@
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Operating System :: OS Independent',
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Programming Language :: Python :: Implementation :: Jython'
     ],
 )
```

### Comparing `riprova-0.2.7/History.rst` & `riprova-0.3.1/History.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 
+v0.3.0 / 2023-05-20
+-------------------
+
+  * Deprecate asyncio.corouting
+  * Drop Python 2 and 3.4 support
+
 v0.2.7 / 2018-08-24
 -------------------
 
   * Merge pull request #20 from ffix/forward-exception-instance
   * Correct linter warnings
   * Re-raise exception instance instead of new exception with no args
   * Merge pull request #19 from EdwardBetts/spelling
@@ -19,15 +25,15 @@
 -------------------
 
 * Merge pull request #15 from jstasiak/allow-newer-six
 * Allow newer six
 * feat(History): update changes
 
 v0.2.5 / 2018-03-21
-------------------
+-------------------
 
 * Merge pull request #15 from jstasiak/allow-newer-six
 * Allow newer six
 * feat(History): update changes
 
 v0.2.4 / 2018-03-20
 -------------------
```

### Comparing `riprova-0.2.7/README.rst` & `riprova-0.3.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-riprova |Build Status| |PyPI| |Coverage Status| |Documentation Status| |Quality| |Versions|
-===========================================================================================
+riprova |PyPI| |Coverage Status| |Documentation Status| |Quality| |Versions|
+============================================================================
 
 ``riprova`` (meaning ``retry`` in Italian) is a small, general-purpose and versatile `Python`_ library
 that provides retry mechanisms with multiple backoff strategies for any sort of failed operations.
 
 It's domain agnostic, highly customizable, extensible and provides a minimal API that's easy to instrument in any code base via decorators, context managers or raw API consumption.
 
 For a brief introduction about backoff mechanisms for potential failed operations, `read this article`_.
@@ -199,16 +199,14 @@
 .. _Exponential backoff: http://riprova.readthedocs.io/en/latest/api.html#riprova.ExponentialBackOff
 .. _ConstantBackoff: https://github.com/h2non/riprova/blob/master/riprova/strategies/constant.py
 .. _whitelisting: https://github.com/h2non/riprova/blob/master/examples/whitelisting_errors.py
 .. _blacklisting: https://github.com/h2non/riprova/blob/master/examples/blacklisting_errors.py
 .. _error evaluation: https://github.com/h2non/riprova/blob/master/examples/http_request.py
 .. _asynchronous coroutines: https://github.com/h2non/riprova/blob/master/examples/http_asyncio.py
 
-.. |Build Status| image:: https://travis-ci.org/h2non/riprova.svg?branch=master
-   :target: https://travis-ci.org/h2non/riprova
 .. |PyPI| image:: https://img.shields.io/pypi/v/riprova.svg?maxAge=2592000?style=flat-square
    :target: https://pypi.python.org/pypi/riprova
 .. |Coverage Status| image:: https://coveralls.io/repos/github/h2non/riprova/badge.svg?branch=master
    :target: https://coveralls.io/github/h2non/riprova?branch=master
 .. |Documentation Status| image:: https://img.shields.io/badge/docs-latest-green.svg?style=flat
    :target: http://riprova.readthedocs.io/en/latest/?badge=latest
 .. |Quality| image:: https://codeclimate.com/github/h2non/riprova/badges/gpa.svg
```

### Comparing `riprova-0.2.7/riprova.egg-info/SOURCES.txt` & `riprova-0.3.1/riprova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/retrier.py` & `riprova-0.3.1/riprova/retrier.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/strategies/exponential.py` & `riprova-0.3.1/riprova/strategies/exponential.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/strategies/constant.py` & `riprova-0.3.1/riprova/strategies/constant.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/strategies/fibonacci.py` & `riprova-0.3.1/riprova/strategies/fibonacci.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/__init__.py` & `riprova-0.3.1/riprova/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # -*- coding: utf-8 -*-
 from .retry import retry
 from .retrier import Retrier
 from .backoff import Backoff
-from .constants import PY_34
 from .errors import ErrorWhitelist, ErrorBlacklist, add_whitelist_error
 from .strategies import *  # noqa
+from .async_retrier import AsyncRetrier  # noqa
 from .exceptions import (RetryError, MaxRetriesExceeded,
                          RetryTimeoutError, NotRetriableError)
 
 
 __author__ = 'Tomas Aparicio'
 __license__ = 'MIT'
 
 # Current package version
-__version__ = '0.2.7'
+__version__ = '0.3.1'
 
 # Explicit symbols to export
 __all__ = (
     'retry',
     'Retrier',
     'Backoff',
+    'AsyncRetrier',
     'ConstantBackoff',
     'FibonacciBackoff',
     'ExponentialBackOff',
     'ErrorWhitelist',
     'ErrorBlacklist',
     'add_whitelist_error',
     'RetryError',
     'MaxRetriesExceeded',
     'RetryTimeoutError',
     'NotRetriableError'
 )
-
-
-# Expose asynchronous retrier if running in Python +3.4
-if PY_34:
-    from .async_retrier import AsyncRetrier
-    __all__ += ('AsyncRetrier',)
```

### Comparing `riprova-0.2.7/riprova/backoff.py` & `riprova-0.3.1/riprova/backoff.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/retry.py` & `riprova-0.3.1/riprova/retry.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/exceptions.py` & `riprova-0.3.1/riprova/exceptions.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/errors.py` & `riprova-0.3.1/riprova/errors.py`

 * *Files identical despite different names*

### Comparing `riprova-0.2.7/riprova/async_retrier.py` & `riprova-0.3.1/riprova/async_retrier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 # -*- coding: utf-8 -*-
+import asyncio  # noqa
 from six import raise_from
 from .backoff import Backoff
 from .retrier import Retrier
-from .constants import PY_34
 from .errors import ErrorWhitelist
 from .strategies import ConstantBackoff
 from .exceptions import MaxRetriesExceeded, RetryError
 
-# Ensure user do not import this module in unsupported Python runtimes
-if not PY_34:  # pragma: no cover
-    raise RuntimeError('cannot import async_retrier module in Python <= 3.4')
-
-import asyncio  # noqa
-
 
 class AsyncRetrier(Retrier):
     """
     AsyncRetrier implements an asynchronous corutine based operation retrier.
 
     Only compatible with `asyncio` in Python 3.4+.
 
@@ -144,31 +138,30 @@
         # Function used to sleep. Defaults `asyncio.sleep()`.
         self.sleep = sleep_coro or asyncio.sleep
         # Stores the default error whitelist used for error retry evaluation
         self.whitelist = (AsyncRetrier.blacklist or
                           AsyncRetrier.whitelist or
                           ErrorWhitelist())
 
-    @asyncio.coroutine
-    def _call(self, coro, *args, **kw):
+    async def _call(self, coro, *args, **kw):
         """
         Calls the given coroutine function with the given variadic arguments.
         """
-        res = yield from coro(*args, **kw)  # noqa (required for Python 2.x)
+        res = await coro(*args, **kw)  # noqa (required for Python 2.x)
 
         # If not evaluator function response is error
         if not self.evaluator or res is None:
             # Clean error on success
             self.error = None
             # Return response object
             return res
 
         # Use custom result evaluator in order to determine if the
         # operation failed or not
-        err = yield from self.evaluator(res)
+        err = await self.evaluator(res)
         if not err:
             self.error = None
             return res
 
         # Raise custom error exception
         if isinstance(err, Exception):
             self.error = err
@@ -177,28 +170,27 @@
         # If True, raise a custom exception
         if err is True:
             raise RuntimeError('evaluator assertion returned True')
 
         # Otherwise simply return the error object
         return err
 
-    @asyncio.coroutine
-    def _handle_error(self, err):
+    async def _handle_error(self, err):
         """
         Handle execution error state and sleep the required amount of time.
         """
         # Update latest cached error
         self.error = err
 
         # Defaults to false
         retry = True
 
         # Evaluate if error is legit or should be retried
         if self.error_evaluator:
-            retry = yield from (asyncio.coroutine(self.error_evaluator)(err))
+            retry = await (asyncio.coroutine(self.error_evaluator)(err))
 
         # If evalutor returns an error exception, just raise it
         if retry and isinstance(retry, Exception):
             raise_from(retry, self.error)
 
         # If retry evaluator returns False, raise original error and
         # stop the retry cycle
@@ -210,48 +202,46 @@
 
         # If backoff is ready
         if delay == Backoff.STOP:
             raise MaxRetriesExceeded('max retries exceeded') from err
 
         # Notify retry subscriber, if needed
         if self.on_retry:
-            yield from self.on_retry(err, delay)
+            await self.on_retry(err, delay)
 
         # Sleep before the next try attempt
-        yield from self.sleep(delay)
+        await self.sleep(delay)
 
-    @asyncio.coroutine
-    def _run(self, coro, *args, **kw):
+    async def _run(self, coro, *args, **kw):
         """
         Runs coroutine in a error-safe infinitive loop until the
         operation succeed or the max retry attempts is reached.
         """
         err = None
 
         while True:
             try:
-                return (yield from self._call(coro, *args, **kw))
+                return await self._call(coro, *args, **kw)
 
             # Collect raised errors by cancelled futures
             except asyncio.CancelledError as _err:
                 err = _err
 
             # Handle any other exception error
             except Exception as _err:
-                yield from self._handle_error(_err)
+                await self._handle_error(_err)
 
             # Increment number of retry attempts
             self.attempts += 1
 
             # Forward raised exception, if needed
             if err is not None:
                 raise err
 
-    @asyncio.coroutine
-    def run(self, coro, *args, **kw):
+    async def run(self, coro, *args, **kw):
         """
         Runs the given coroutine function in a retry loop until the operation
         is completed successfully or maximum retries attempts are reached.
 
         Arguments:
             coro (coroutinefunction): coroutine function to retry.
             *args (args): partial arguments to pass to the function.
@@ -272,20 +262,18 @@
         self.backoff.reset()
 
         # Reset state
         self.error = None
         self.attempts = 0
 
         # If not timeout defined, run the coroutine function
-        return (yield from asyncio.wait_for(
+        return await asyncio.wait_for(
             self._run(coro, *args, **kw),
             self.timeout,
             loop=self.loop
-        ))
+        )
 
-    @asyncio.coroutine
-    def __aenter__(self):
+    async def __aenter__(self):
         return self
 
-    @asyncio.coroutine
-    def __aexit__(self, exc_type, exc_value, traceback):
+    async def __aexit__(self, exc_type, exc_value, traceback):
         return self.__exit__(exc_type, exc_value, traceback)
```

