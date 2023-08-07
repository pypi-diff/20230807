# Comparing `tmp/eons-2.7.3.tar.gz` & `tmp/eons-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.7.3.tar", last modified: Tue Jul 18 04:45:08 2023, max compression
+gzip compressed data, was "eons-3.0.0.tar", last modified: Mon Aug  7 00:25:31 2023, max compression
```

## Comparing `eons-2.7.3.tar` & `eons-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-18 04:45:08.520157 eons-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-18 04:44:50.000000 eons-2.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.516157 eons-2.7.3/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99533 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-18 04:44:59.000000 eons-2.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 04:45:08.520157 eons-2.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:25:31.736729 eons-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-08-07 00:25:31.736729 eons-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-08-07 00:25:15.000000 eons-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:25:31.728729 eons-3.0.0/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:25:31.732729 eons-3.0.0/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 00:25:23.000000 eons-3.0.0/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110262 2023-08-07 00:25:23.000000 eons-3.0.0/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:25:31.732729 eons-3.0.0/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:25:23.000000 eons-3.0.0/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:25:31.736729 eons-3.0.0/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:25:23.000000 eons-3.0.0/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/resolve/resolve_install_with_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-07 00:25:00.000000 eons-3.0.0/pkg/eons/resolve/resolve_namespace_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:25:31.732729 eons-3.0.0/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-08-07 00:25:31.000000 eons-3.0.0/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-07 00:25:31.000000 eons-3.0.0/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:25:31.000000 eons-3.0.0/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 00:25:31.000000 eons-3.0.0/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 00:25:31.000000 eons-3.0.0/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 00:25:23.000000 eons-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 00:25:31.736729 eons-3.0.0/setup.cfg
```

### Comparing `eons-2.7.3/PKG-INFO` & `eons-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.3
+Version: 3.0.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.7.3/README.md` & `eons-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.7.3/pkg/eons/eons.py` & `eons-3.0.0/pkg/eons/eons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+import traceback
 import logging
+import jsonpickle
+import inspect
+from copy import deepcopy
 import os
 import shutil
-from copy import deepcopy
+import dis
+import types
 import builtins
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
-import types
-import traceback
-import jsonpickle
-import inspect
-import operator
 from pathlib import Path
 from subprocess import Popen
 from subprocess import PIPE
 from subprocess import STDOUT
 import re
+import operator
 import argparse
 import requests
+import importlib
 import yaml
 from requests_futures.sessions import FuturesSession
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
 from eot import EOT
 
@@ -60,131 +62,15 @@
 class Fatal(Exception, metaclass=ActualType): pass
 class FatalCannotExecute(Fatal, metaclass=ActualType): pass
 
 class PackageError(Exception, metaclass=ActualType): pass
 
 class MethodPendingPopulation(Exception, metaclass=ActualType): pass
 
-
-#Self registration for use with json loading.
-#Any class that derives from SelfRegistering can be instantiated with:
-#   SelfRegistering("ClassName")
-#Based on: https://stackoverflow.com/questions/55973284/how-to-create-this-registering-factory-in-python/55973426
-class SelfRegistering(object):
-
-	def __init__(this, *args, **kwargs):
-		#ignore args.
-		super().__init__()
-
-	@classmethod
-	def GetSubclasses(cls):
-		for subclass in cls.__subclasses__():
-			# logging.info(f"Subclass dict: {subclass.__dict__}")
-			yield subclass
-			for subclass in subclass.GetSubclasses():
-				yield subclass
-
-	@classmethod
-	def GetClass(cls, classname):
-		for subclass in cls.GetSubclasses():
-			if subclass.__name__ == classname:
-				return subclass
-
-		# no subclass with matching classname found (and no default defined)
-		raise ClassNotFound(f"No known SelfRegistering class: {classname}")			
-
-	#TODO: How do we pass args to the subsequently called __init__()?
-	def __new__(cls, classname, *args, **kwargs):
-		toNew = cls.GetClass(classname)
-		logging.debug(f"Creating new {toNew.__name__}")
-
-		# Using "object" base class method avoids recursion here.
-		child = object.__new__(toNew)
-
-		#__dict__ is always blank during __new__ and only populated by __init__.
-		#This is only useful as a negative control.
-		# logging.debug(f"Created object of {child.__dict__}")
-
-		return child
-
-	# Registering classes is typically depth-first.
-	@staticmethod
-	def RegisterAllClassesInDirectory(directory, recurse=True):
-		logging.debug(f"Loading SelfRegistering classes in {directory}")
-		directoryContents = [i for i in sorted(os.listdir(directory)) if not i.startswith('_')]
-
-		directories = [i for i in directoryContents if os.path.isdir(os.path.join(directory, i))]
-		files = [i for i in directoryContents if os.path.isfile(os.path.join(directory, i))]
-		files = [f for f in files if f.endswith('.py')]
-
-		if (recurse):
-			for dir in directories:				
-				SelfRegistering.RegisterAllClassesInDirectory(os.path.join(directory, dir), recurse)
-
-		logging.debug(f"Available modules: {files}")
-		for file in files:
-			moduleName = file.split('.')[0]
-
-			# logging.debug(f"Attempting to registering classes in {moduleName}.")
-			loader = importlib.machinery.SourceFileLoader(moduleName, os.path.join(directory, file))
-			module = types.ModuleType(loader.name)
-			loader.exec_module(module)
-
-			# NOTE: the module is not actually imported in that it is available through sys.modules.
-			# However, this appears to be enough to get both inheritance and SelfRegistering functionality to work.
-			sys.modules[moduleName] = module #But just in case...
-			logging.debug(f"{moduleName} imported.")
-
-			#### Other Options ####
-			# __import__(module)
-			# OR
-			# for importer, module, _ in pkgutil.iter_modules([directory]):
-			#	 importer.find_module(module).exec_module(module) #fails with "AttributeError: 'str' object has no attribute '__name__'"
-			#	 importer.find_module(module).load_module(module) #Deprecated
-
-		# enable importing and inheritance for SelfRegistering classes
-		if (directory not in sys.path):
-			sys.path.append(directory)
-
-
-# A Datum is a base class for any object-oriented class structure.
-# This class is intended to be derived from and added to.
-# The members of this class are helpful labels along with the ability to invalidate a datum.
-class Datum(SelfRegistering):
-
-	# Don't worry about this.
-	# If you really want to know, look at SelfRegistering.
-	def __new__(cls, *args, **kwargs):
-		return object.__new__(cls)
-
-
-	def __init__(this, name=INVALID_NAME(), number=0):
-		# logging.debug("init Datum")
-
-		# Names are generally useful.
-		this.name = name
-
-		# Storing validity as a member makes it easy to generate bad return values (i.e. instead of checking for None) as well as manipulate class (e.g. each analysis step invalidates some class and all invalid class are discarded at the end of analysis).
-		this.valid = True
-
-	# Override this if you have your own validity checks.
-	def IsValid(this):
-		return this.valid == True
-
-
-	# Sets valid to true
-	# Override this if you have members you need to handle with care.
-	def MakeValid(this):
-		this.valid = True
-
-
-	# Sets valid to false.
-	def Invalidate(this):
-		this.valid = False
-
+class ConstellatusError(Exception, metaclass=ActualType): pass
 
 # util is a namespace for any miscellaneous utilities.
 # You cannot create a util.
 class util:
 	def __init__(this):
 		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
 
@@ -317,31 +203,294 @@
 			logging.log(value, message, *args, **kwargs)
 
 		logging.addLevelName(value, levelName)
 		setattr(logging, levelName, value)
 		setattr(logging.getLogger(), methodName, logForLevel)
 		setattr(logging, methodName, logToRoot)
 
+	@staticmethod
+	def forerunner(forerunner, *forerunnerArgs, **forerunnerKwargs):
+		def WrapperFactory(function):
+			def Wrapper(*functionArgs, **functionKwargs):
+				forerunner(*forerunnerArgs, **forerunnerKwargs)
+				return function(*functionArgs, **functionKwargs)
+			return Wrapper
+		return WrapperFactory
+	
+
+	class BlackMagick:
+
+		@staticmethod
+		def InjectIntoModule(source, name, value):
+			moduleToHack = inspect.getmodule(source)
+			setattr(moduleToHack, name, value)
+
 
 jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
 
+# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
+# This can be abused quite a bit, so please try to restrict usage of this to only:
+# * Ease of use global functions
+#
+# Thanks! 
+class ExecutorTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in ExecutorTracker.__dict__:
+			logging.debug(f"Creating new ExecutorTracker: {this}")
+			ExecutorTracker.instance = this
+		else:
+			return None
+
+		this.executors = [None]
+
+	@staticmethod
+	def Instance():
+		if "instance" not in ExecutorTracker.__dict__:
+			ExecutorTracker()
+		return ExecutorTracker.instance
+
+	@staticmethod
+	def Push(executor):
+		ExecutorTracker.Instance().executors.append(executor)
+
+		# Adding the executor to our list here increases its reference count.
+		# Executors are supposed to remove themselves from this list when they are deleted.
+		# A python object cannot be deleted if it has references.
+		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
+		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
+		# If you want your executor to stop being tracked, do it yourself. :(
+		#
+		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+
+		logging.debug(f"Now tracking Executor: {executor}")
+
+	@staticmethod
+	def Pop(executor):
+		try:
+			ExecutorTracker.Instance().executors.remove(executor)
+			logging.debug(f"No longer tracking Executor: {executor}")
+		except:
+			pass
+
+	@staticmethod
+	def GetLatest():
+		return ExecutorTracker.Instance().executors[-1]
+
+
+# The Eons way of tracking logical & extensible groupings.
+class Namespace:
+
+	def __init__(this, namespaces = None):
+		this.namespaces = []
+
+		if (isinstance(namespaces, str)):
+			this.namespaces = namespaces.split(':')
+			this.namespaces = [namespace for namespace in this.namespaces if len(namespace)]
+		elif (isinstance(namespaces, list)):
+			this.namespaces = namespaces
+		elif (isinstance(namespaces, Namespace)):
+			this.namespaces = namespaces.namespaces
+
+	# Get a subset from *this.
+	def Slice(this, start=0, end=None):
+		return Namespace(this.namespaces[start:end])
+	
+	def __str__(this):
+		ret = "::" + ":".join(this.namespaces)
+		if (ret == "::"):
+			return "::"
+		return ret + ":"
+
+	# Get a namespace string as something more reasonable in python.
+	def ToName(this):
+		if (not len(this.namespaces)):
+			return ""
+		return "_".join(this.namespaces) + "_"
+	
+	def __iadd__(this, other):
+		this.namespaces.append(Namespace(other).namespaces)
+		return this
+	
+	def __isub__(this, other):
+		this.namespaces = this.namespaces[:-len(Namespace(other).namespaces)]
+		return this
+
+
+class NamespaceTracker:
+	def __init__(this):
+		# Singletons man...
+		if "instance" not in NamespaceTracker.__dict__:
+			logging.debug(f"Creating new NamespaceTracker: {this}")
+			NamespaceTracker.instance = this
+		else:
+			return None
+
+		this.last = Namespace()
+
+	@staticmethod
+	def Instance():
+		if "instance" not in NamespaceTracker.__dict__:
+			NamespaceTracker()
+		return NamespaceTracker.instance
+
+# Decorator to add a namespace to a class.
+# Should look like @namespace('foo::bar')
+def namespace(ns):
+	def DecorateWithNamespace(cls):
+		locale = Namespace(ns)
+		prepend = locale.ToName()
+		NamespaceTracker.Instance().last = locale
+		return type(f"{prepend}{cls.__name__}", cls.__bases__, dict(cls.__dict__))
+	return DecorateWithNamespace
+
+#Self registration for use with json loading.
+#Any class that derives from SelfRegistering can be instantiated with:
+#   SelfRegistering("ClassName")
+#Based on: https://stackoverflow.com/questions/55973284/how-to-create-this-registering-factory-in-python/55973426
+class SelfRegistering(object):
+
+	def __init__(this, *args, **kwargs):
+		#ignore args.
+		super().__init__()
+
+	@classmethod
+	def GetSubclasses(cls):
+		for subclass in cls.__subclasses__():
+			# logging.info(f"Subclass dict: {subclass.__dict__}")
+			yield subclass
+			for subclass in subclass.GetSubclasses():
+				yield subclass
+
+	@classmethod
+	def GetClass(cls, classname):
+		for subclass in cls.GetSubclasses():
+			if subclass.__name__ == classname:
+				return subclass
+
+		# no subclass with matching classname found (and no default defined)
+		raise ClassNotFound(f"No known SelfRegistering class: {classname}")			
+
+	#TODO: How do we pass args to the subsequently called __init__()?
+	def __new__(cls, classname, *args, **kwargs):
+		toNew = cls.GetClass(classname)
+		logging.debug(f"Creating new {toNew.__name__}")
+
+		# Using "object" base class method avoids recursion here.
+		child = object.__new__(toNew)
+
+		#__dict__ is always blank during __new__ and only populated by __init__.
+		#This is only useful as a negative control.
+		# logging.debug(f"Created object of {child.__dict__}")
+
+		return child
+
+	# Registering classes is typically depth-first.
+	@staticmethod
+	def RegisterAllClassesInDirectory(directory, recurse=True):
+		logging.debug(f"Loading SelfRegistering classes in {directory}")
+		directoryContents = [i for i in sorted(os.listdir(directory)) if not i.startswith('_')]
+
+		directories = [i for i in directoryContents if os.path.isdir(os.path.join(directory, i))]
+		files = [i for i in directoryContents if os.path.isfile(os.path.join(directory, i))]
+		files = [f for f in files if f.endswith('.py')]
+
+		if (recurse):
+			for dir in directories:				
+				SelfRegistering.RegisterAllClassesInDirectory(os.path.join(directory, dir), recurse)
+
+		logging.debug(f"Available modules: {files}")
+		for file in files:
+			moduleName = file.split('.')[0]
+
+			# logging.debug(f"Attempting to registering classes in {moduleName}.")
+			loader = importlib.machinery.SourceFileLoader(moduleName, os.path.join(directory, file))
+			module = types.ModuleType(loader.name)
+			loader.exec_module(module)
+
+			# Mangle the module name to include the namespace.
+			# The namespace is set when exec'ing the module, so we'll reset it after.
+			importName = NamespaceTracker.Instance().last.ToName() + moduleName
+			NamespaceTracker.Instance().last = Namespace()
+
+			setattr(module, '_source', os.path.join(directory, file))
+
+			# NOTE: the module is not actually imported in that it is available through sys.modules.
+			# However, this appears to be enough to get both inheritance and SelfRegistering functionality to work.
+			sys.modules[importName] = module #But just in case...
+			logging.debug(f"{moduleName} imported as {importName}.")
+
+			#### Other Options ####
+			# __import__(module)
+			# OR
+			# for importer, module, _ in pkgutil.iter_modules([directory]):
+			#	 importer.find_module(module).exec_module(module) #fails with "AttributeError: 'str' object has no attribute '__name__'"
+			#	 importer.find_module(module).load_module(module) #Deprecated
+
+		# enable importing and inheritance for SelfRegistering classes
+		if (directory not in sys.path):
+			sys.path.append(directory)
+
+
+# A Datum is a base class for any object-oriented class structure.
+# This class is intended to be derived from and added to.
+# The members of this class are helpful labels along with the ability to invalidate a datum.
+class Datum(SelfRegistering):
+
+	# Don't worry about this.
+	# If you really want to know, look at SelfRegistering.
+	def __new__(cls, *args, **kwargs):
+		return object.__new__(cls)
+
+
+	def __init__(this, name=INVALID_NAME(), number=0):
+		# logging.debug("init Datum")
+
+		# Names are generally useful.
+		this.name = name
+
+		# Storing validity as a member makes it easy to generate bad return values (i.e. instead of checking for None) as well as manipulate class (e.g. each analysis step invalidates some class and all invalid class are discarded at the end of analysis).
+		this.valid = True
+
+	# Override this if you have your own validity checks.
+	def IsValid(this):
+		return this.valid == True
+
+
+	# Sets valid to true
+	# Override this if you have members you need to handle with care.
+	def MakeValid(this):
+		this.valid = True
+
+
+	# Sets valid to false.
+	def Invalidate(this):
+		this.valid = False
+
+
 # FunctorTracker is a global singleton which keeps a record of all functors that are currently in the call stack.
 # Functors should add and remove themselves from this list when they are called.
 class FunctorTracker:
 	def __init__(this):
 		# Singletons man...
 		if "instance" not in FunctorTracker.__dict__:
 			logging.debug(f"Creating new FunctorTracker: {this}")
 			FunctorTracker.instance = this
 		else:
 			return None
 
 		this.functors = [None]
 
+		this.sequence = util.DotDict()
+		this.sequence.current = util.DotDict()
+		this.sequence.current.running = False
+		this.sequence.current.stage = 0
+		this.sequence.stage = []
+
 	@staticmethod
 	def Instance():
 		if "instance" not in FunctorTracker.__dict__:
 			FunctorTracker()
 		return FunctorTracker.instance
 
 	@staticmethod
@@ -359,14 +508,123 @@
 			pass
 		tracker.functors.reverse()
 
 	@staticmethod
 	def GetCount():
 		return len(FunctorTracker.Instance().functors)
 
+
+	# Add a sequence to *this.
+	@staticmethod
+	def InitiateSequence():
+		FunctorTracker.Instance().sequence.current.running = True
+		FunctorTracker.Instance().sequence.current.stage += 1
+		FunctorTracker.Instance().sequence.stage.append(util.DotDict({'state': 'initiated'}))
+
+	# Remove a sequence from *this.
+	@staticmethod
+	def CompleteSequence():
+		if (not FunctorTracker.Instance().sequence.current.running):
+			return
+		FunctorTracker.Instance().sequence.current.stage -= 1
+		FunctorTracker.Instance().sequence.stage.pop()
+		FunctorTracker.Instance().sequence.current.running = FunctorTracker.Instance().sequence.current.stage > 0
+
+	
+	# Calculate the current namespace, trimming off the last backtrack number of namespaces.
+	# The first Functor we Track is likely the Executor, so make sure to skip that.
+	@staticmethod
+	def GetCurrentNamespace(backtrack=0, start=1):
+		return Namespace([functor.name for functor in FunctorTracker.Instance().functors[start:len(FunctorTracker.Instance().functors) - (backtrack+1)]])
+
+	# Get the current namespace as a python usable Functor name.
+	@staticmethod
+	def GetCurrentNamespaceAsName(backtrack=0, start=1):
+		return Namespace.ToName(FunctorTracker.GetCurrentNamespace(start, backtrack))
+
+#from .Executor import Executor # don't import this, it'll be circular!
+
+# @recoverable
+# Decorating another function with this method will engage the error recovery system provided by *this.
+# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
+# For more info, see Executor.ResolveError and the README.md
+def recoverable(function):
+	def RecoverableDecorator(obj, *args, **kwargs):
+		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
+	return RecoverableDecorator
+
+
+# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
+def RecoverableImplementation(obj, executor, function, *args, **kwargs):
+	try:
+		return function(obj, *args, **kwargs)
+	except FailedErrorResolution as fatal:
+		raise fatal
+	except Exception as e:
+		if (not executor.resolveErrors):
+			raise e
+		return Recover(e, obj, executor, function, *args, **kwargs)
+
+
+def Recover(error, obj, executor, function, *args, **kwargs):
+	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
+	util.LogStack()
+
+	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
+	if (str(error) not in executor.errorResolutionStack.keys()):
+		executor.errorResolutionStack.update({str(error):[]})
+
+	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
+	# ResolveError is itself @recoverable.
+	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
+	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
+	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
+
+	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
+		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
+
+	successfullyRecovered = False
+	ret = None
+	resolvedBy = None
+	for i, res in enumerate(executor.resolveErrorsWith):
+
+		logging.debug(f"Checking if {res} can fix '{error}'.")
+		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
+			# if no resolution was attempted, there's no need to re-run the function.
+			continue
+		try:
+			logging.debug(f"Trying function ({function}) again after applying {res}.")
+			resolvedBy = res
+			ret = function(obj, *args, **kwargs)
+			successfullyRecovered = True
+			break
+
+		except Exception as e2:
+			if (str(error) == str(e2)):
+				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
+				# Resolution failed. That's okay. Let's try the next.
+				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
+				continue
+			else:
+				# The error changed, maybe we're making progress.
+				ret = Recover(e2, obj, executor, function, *args, **kwargs)
+				successfullyRecovered = True
+				break
+
+	if (successfullyRecovered):
+		executor.ClearErrorResolutionStack(str(error)) # success!
+		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
+		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
+		return ret
+
+	#  We failed to resolve the error. Die
+	sys.tracebacklimit = 0 # traceback is NOT helpful here.
+	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
+
+
 # Don't import Method or Executor, even though they are required: it will cause a circular dependency.
 # Instead, pretend there's a forward declaration here and don't think too hard about it ;)
 ################################################################################
 
 # Functor is a base class for any function-oriented class structure or operation.
 # This class derives from Datum, primarily, to give it a name but also to allow it to be stored and manipulated, should you so desire.
 # Functors will automatically Fetch any ...Args specified.
@@ -455,17 +713,22 @@
 		# For converting config value names.
 		# e.g. "type": "projectType" makes it so that when calling Set("projectType", ...),  this.type is changed.
 		this.configNameOverrides = {}
 
 		# Rolling back can be disabled by setting this to False.
 		this.enableRollback = True
 
-		# Automatically return the result.data object if the function returns None
+		# Automatically return this.
+		# Also enables partial function calls.
 		this.enableAutoReturn = True
 
+		# Allow partial function calls by marking *this as incomplete.
+		# Incomplete means that more arguments need to be provided.
+		this.incomplete= False
+
 		# this.result encompasses the return value of *this.
 		# The code is a numerical result indication the success or failure of *this and is set automatically.
 		# 0 is success; 1 is no change; higher numbers are some kind of error.
 		# this.result.data should be set manually.
 		# It is highly recommended that you check result.data in DidFunctionSucceed().
 		this.result = util.DotDict()
 		this.result.code = 0
@@ -493,14 +756,17 @@
 		# Those which come next (in order).
 		this.next = []
 
 		# Callback method
 		this.callbacks = util.DotDict()
 		this.callbacks.fetch = None
 
+		this.abort = util.DotDict()
+		this.abort.WarmUp = False
+
 
 	# Override this and do whatever!
 	# This is purposefully vague.
 	def Function(this):
 		pass
 
 
@@ -758,57 +1024,67 @@
 
 		# We have to use util.___Attr() because some sources might have '.'s in them.
 
 		for source, honorPropagate in this.methodSources.items():
 			if (not util.HasAttr(this, source)):
 				logging.debug(f"Could not find {source}; will not pull in its methods.")
 				continue
+
+			methodSource = util.GetAttr(this, source)
+			if (not isinstance(methodSource, dict)):
+				logging.debug(f"{source} is not a dict; will not pull in its methods.")
+				continue
+
 			logging.debug(f"Populating methods from {source}.")
-			for method in util.GetAttr(this, source).values():
+			for method in methodSource.values():
 				if (honorPropagate and not method.propagate):
 					continue
 				if (method.name in this.methods.keys() and honorPropagate):
 					existingMethod = this.methods[method.name]
 					if (not existingMethod.inheritMethods):
 						continue
 
 					methodToInsert = deepcopy(method)
+					methodToInsert.caller = this
 					methodToInsert.UpdateSource()
 
 					if (existingMethod.inheritedMethodsFirst):
 						logging.debug(f"Will call {method.name} from {source} to prior to this.")
 						methodToInsert.next.append(this.methods[method.name])
 						this.methods[method.name] = methodToInsert
 					else:
 						logging.debug(f"Appending {method.name} from {source} to this.")
 						this.methods[method.name].next.append(methodToInsert)
 				else:
 					this.methods[method.name] = deepcopy(method)
+					this.methods[method.name].caller = this
 					this.methods[method.name].UpdateSource()
 
 		for method in this.methods.values():
 			logging.debug(f"Populating method {this.name}.{method.name}({', '.join([a for a in method.requiredKWArgs] + [a+'='+str(v) for a,v in method.optionalKWArgs.items()])})")
-			method.caller = this
 
 			# Python < 3.11
 			# setattr(this, method.name, method.__call__.__get__(this, this.__class__))
 
 			# appears to work for all python versions >= 3.8
-			setattr(this, method.name, method.__call__.__get__(method, method.__class__))
-
+			# setattr(this, method.name, method.__call__.__get__(method, method.__class__))
+			
+			setattr(this, method.name, types.MethodType(method, this))
 
 
 	# Set this.precursor
 	# Also set this.executor because it's easy.
 	def PopulatePrecursor(this):
 		if (this.executor is None):
 			if ('executor' in this.kwargs):
 				this.executor = this.kwargs.pop('executor')
 			else:
-				logging.warning(f"{this.name} was not given an 'executor'. Some features will not be available.")
+				this.executor = ExecutorTracker.GetLatest()
+		if (not this.executor):
+			logging.warning(f"{this.name} was not given an 'executor'. Some features will not be available.")
 
 		if ('precursor' in this.kwargs):
 			this.precursor = this.kwargs.pop('precursor')
 			logging.debug(f"{this.name} was preceded by {this.precursor.name}")
 		else:
 			this.precursor = None
 			logging.debug(f"{this.name} was preceded by None")
@@ -895,34 +1171,58 @@
 		
 		# Something odd happens here; we've been getting:
 		# AttributeError("'builtin_function_or_method' object has no attribute 'pop'")
 		# But that implies we're getting a valid next object that is not a list.
 		# FIXME: Debug this.
 		proceedToNext = False
 		next = None
+		nextName = ""
 		try:
 			next = this.next.pop(0)
+			if (isinstance(next, str)):
+				nextName = next
+			else:
+				nextName = next.name
 			proceedToNext = True
 		except Exception as e:
-			logging.error(f"{this.name} not proceeding to next: {e}; next: {this.next}")
+			logging.error(f"{this.name} not proceeding to next: {e}; next: {nextName} (from {this.next})")
 			return None
 
-		if (this.GetExecutor() is None):
-			raise InvalidNext(f"{this.name} has no executor and cannot execute next ({this.next}).")
-
 		if (proceedToNext):
 			if (not this.ValidateNext(next)):
 				raise InvalidNext(f"Failed to validate {next}")
-			return this.GetExecutor().Execute(next, precursor=this, next=this.next)
+
+			if (this.GetExecutor()):
+				return this.GetExecutor().Execute(next, precursor=this, next=this.next)
+			
+			return next(precursor=this, next=this.next)
 
 
+	# Prepare *this for any kind of operation.
+	# All initialization should be done here.
+	# RETURN boolean indicating whether or not *this is ready to do work.
 	def WarmUp(this, *args, **kwargs):
+		if (FunctorTracker.Instance().sequence.current.running):
+			# We just started a new sequence. We're not ready to do work yet.
+			if (FunctorTracker.Instance().sequence.stage[FunctorTracker.Instance().sequence.current.stage].state == 'initiated'):
+				this.incomplete = True
+				this.abort.WarmUp = True
+				FunctorTracker.Instance().sequence.stage[FunctorTracker.Instance().sequence.current.stage].state = 'ready'
+		# NOTE: this.abortWarmUp will (should) be set by the precursor before calling *this.
+		
+		if (not this.incomplete):
+			this.args = []
+			this.kwargs = {}
+
+		this.args += args
+		this.kwargs.update(kwargs)
 
-		this.args = args
-		this.kwargs = kwargs
+		if (this.abort.WarmUp):
+			return False
+			
 		this.result.code = 0
 		this.result.data = util.DotDict()
 		
 		try:
 			this.PopulatePrecursor()
 			if (this.executor):
 				this.executor.BeginPlacing(this.name)
@@ -931,33 +1231,56 @@
 			this.ParseInitialArgs() # Usually where config is read in.
 			this.ValidateStaticArgs() # nop on call 2+
 			this.PopulateNext()
 			this.ValidateArgs()
 			this.ValidateMethods()
 			if (this.executor):
 				this.executor.ResolvePlacementOf(this.name)
+
 		except Exception as e:
+
+			# Allow partial function calls
+			if (isinstance(e, MissingArgumentError) and this.enableAutoReturn):
+				this.incomplete = True
+				return False
+			
 			if (this.raiseExceptions):
 				raise e
 			else:
 				logging.error(f"ERROR: {e}")
 				util.LogStack()
+		
+		this.incomplete = False
+		return True
 
 
 	# Make functor.
 	# Don't worry about this; logic is abstracted to Function
 	def __call__(this, *args, **kwargs) :
 		logging.info(f"{this.name} ({args}, {kwargs}) {{")
 		FunctorTracker.Push(this)
 
 		ret = None
 		nextRet = None
 		
 		try:
 			this.WarmUp(*args, **kwargs)
+
+			# TODO: Can we make this more performant? We should avoid doing this every time if we can.
+			isSequence = this.WillPerformSequence()
+			if (isSequence):
+				FunctorTracker.InitiateSequence() # Has to be after WarmUp.
+
+			if (this.incomplete):
+				logging.debug(f"{this.name} incomplete.")
+				logging.info(f"return {ret}")
+				FunctorTracker.Pop(this)
+				logging.info(f"}} ({this.name})")
+				return this
+			
 			logging.debug(f"{this.name}({this.args}, {this.kwargs})")
 
 			getattr(this, f"Before{this.callMethod}")()
 			ret = getattr(this, this.callMethod)()
 
 			if (getattr(this, f"Did{this.callMethod}Succeed")()):
 					this.result.code = 0
@@ -987,25 +1310,62 @@
 				util.LogStack()
 
 		if (this.raiseExceptions and this.result.code > 1):
 			raise FunctorError(f"{this.name} failed with result {this.result.code}: {this.result}")
 
 		if (nextRet is not None):
 			ret = nextRet
+		elif (this.enableAutoReturn):
+			if (this.result.data is None):
+				this.result.data = ret
+			elif (not 'returned' in this.result.data):
+					this.result.data.returned = ret
+			else:
+				pass
 
-		if (this.enableAutoReturn and len(this.result.data) and ret is None):
-			ret = this.result.data
+			ret = this
 
 		logging.info(f"return {ret}")
 		FunctorTracker.Pop(this)
 		logging.info(f"}} ({this.name})")
 
 		return ret
 
 
+	# Reduce the work required to access return values.
+	# Make it possible to access related classes on the fly.
+	def __getattribute__(this, attribute):
+		try:
+			return super().__getattribute__(attribute)
+		except AttributeError as e:
+			try:
+				return this.result.data[attribute]
+			except:
+				raise e
+
+				# TODO: This should work, in theory. However, what seems to happen is that the program just gets slower and slower until it hangs. There's no infinite loop (in the python code at least), and there's no obvious point of error. Just some function somewhere will stop working.
+				# Last time I tested this, I was able to get repeatable failures on the line: `logging.getLogger('urllib3').setLevel(logging.WARNING)` while running TestNamespace in isolation (i.e. no other tests, no ebbs, etc)
+				# PyCharm says "unable to display frame variables"
+				# That line doesn't even use this codebase. My best guess is that it has something to do with our custom log formatter. However, pinning that down has proven difficult.
+				#
+				# try:
+				# 	if (not hasattr(this, 'executor')):
+				# 		raise e
+				# 	# Beseech the error resolution machinery.
+				# 	return Recover(
+				# 		e,
+				# 		this,
+				# 		this.executor,
+				# 		this.__getattribute__,
+				# 		attribute
+				# 	)
+				# except:
+				# 	raise e
+
+
 	# Adapter for @recoverable.
 	# See Recoverable.py for details
 	def GetExecutor(this):
 		return this.executor
 
 
 	# Add support for deepcopy.
@@ -1020,14 +1380,35 @@
 		for key, val in [tup for tup in this.__dict__.items() if tup[0] not in ['methods']]:
 			if (callable(val)):
 				# PopulateMethods will take care of recreating skipped Methods
 				# All other methods are dropped since they apparently have problems on some implementations.
 				continue
 			setattr(ret, key, deepcopy(val, memodict))
 		return ret
+	
+
+	# Enable sequences to be built/like/this
+	def __truediv__(this, next):
+		if (not isinstance(next, Functor)):
+			return this
+		this.next.append(next)
+		next.abort.WarmUp = False
+		return this.CallNext()
+	
+
+	# Avert your eyes!
+	# This is deep black magick fuckery.
+	# And no. There does not appear to be any other way to do this on CPython <=3.11
+	def WillPerformSequence(this, backtrack=2):
+		try:
+			# NOTE: 11 is apparently the code for the __truediv__ division operator (/). On this system. For now...
+			return [i for i in [i for i in dis.get_instructions(eval(f"inspect.currentframe(){'.f_back' * backtrack}.f_code")) if i.opname == 'BINARY_OP'] if i.arg == 11] > 0
+		except:
+			# Yeah...
+			return False
 
 
 	######## START: Fetch Locations ########
 
 	def fetch_location_this(this, varName, default, fetchFrom, attempted):
 		if (util.HasAttr(this, varName)):
 			return util.GetAttr(this, varName), True
@@ -1055,14 +1436,16 @@
 		
 		return this.caller.FetchWithout(['environment'], varName, default, fetchFrom, False, attempted)
 
 
 	# Call the Executor's Fetch method.
 	# Exclude 'environment' because we can check that ourselves.
 	def fetch_location_executor(this, varName, default, fetchFrom, attempted):
+		if (not this.GetExecutor()):
+			return default, False
 		return this.GetExecutor().FetchWithout(['environment'], varName, default, fetchFrom, False, attempted)
 
 
 	#NOTE: There is no config in the default Functor. This is done for the convenience of children.
 	def fetch_location_config(this, varName, default, fetchFrom, attempted):
 		if (not util.HasAttr(this, 'config') or this.config is None):
 			return default, False
@@ -1088,204 +1471,14 @@
 		if (envVar is not None):
 			return envVar, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
 
-# Invoke the External Method machinery to fetch a Functor & return it.
-# This should be used with other eons.kinds
-class Inject(Functor):
-	def __init__(this, name = "Inject"):
-		super().__init__(name)
-		this.requiredKWArgs.append('target')
-		this.optionalKWArgs['impl'] = 'External'
-
-		this.argMapping.append('target')
-		this.argMapping.append('impl')
-	
-	def Function(this):
-		# Prepare a dummy function to replace with a Method.
-		code = compile(f"def {this.target}(this):\n\tpass", '', 'exec')
-		exec(code)
-
-		methodToAdd = SelfRegistering(this.impl)
-		methodToAdd.Constructor(eval(this.target), None)
-		for key, value in this.kwargs.items():
-			setattr(methodToAdd, key, value)
-
-		return methodToAdd
-
-def inject(
-	target,
-	impl="External",
-	**kwargs
-):
-	return Inject()(target=target, impl=impl, **kwargs)
-
-
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
-
-
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
-
-
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
-
-
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
-
-
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
-
-
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
-
-
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
-
-
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
-
-
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
-
-
-
 def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
 	raise MethodPendingPopulation("METHOD PENDING POPULATION")
 
 # Store the new method in the class
 def PrepareClassMethod(cls, name, methodToAdd):
 	# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
 	if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
@@ -1358,23 +1551,28 @@
 
 		# We don't care about these checks right now.
 		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
 		this.functionSucceeded = True
 		this.rollbackSucceeded = True
 		this.enableRollback = False
 
+		# Methods,by default, do not return themselves.
+		this.enableAutoReturn = False
+
 		# The source code of the function we're implementing.
 		this.source = ""
 
 		this.original = util.DotDict()
 		this.original.cls = util.DotDict()
 		this.original.cls.object = None
 		this.original.cls.name = 'None'
 		this.original.function = None
 
+		this.argMapping = ['caller']
+
 
 	# Make *this execute the code in this.source
 	def UpdateSource(this):
 		wrappedFunctionName = f'_eons_method_{this.name}'
 		completeSource = f'''\
 def {wrappedFunctionName}(this):
 {this.source}
@@ -1586,62 +1784,45 @@
 		if (saveout):
 			return process.returncode, output
 		
 		return process.returncode
 	######## END: UTILITIES ########
 
 
-# ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
-# This can be abused quite a bit, so please try to restrict usage of this to only:
-# * Ease of use global functions
-#
-# Thanks! 
-class ExecutorTracker:
-	def __init__(this):
-		# Singletons man...
-		if "instance" not in ExecutorTracker.__dict__:
-			logging.debug(f"Creating new ExecutorTracker: {this}")
-			ExecutorTracker.instance = this
-		else:
-			return None
-
-		this.executors = [None]
-
-	@staticmethod
-	def Instance():
-		if "instance" not in ExecutorTracker.__dict__:
-			ExecutorTracker()
-		return ExecutorTracker.instance
+# Invoke the External Method machinery to fetch a Functor & return it.
+# This should be used with other eons.kinds
+class Inject(Functor):
+	def __init__(this, name = "Inject"):
+		super().__init__(name)
+		this.requiredKWArgs.append('target')
+		this.optionalKWArgs['impl'] = 'External'
 
-	@staticmethod
-	def Push(executor):
-		ExecutorTracker.Instance().executors.append(executor)
+		this.argMapping.append('target')
+		this.argMapping.append('impl')
 
-		# Adding the executor to our list here increases its reference count.
-		# Executors are supposed to remove themselves from this list when they are deleted.
-		# A python object cannot be deleted if it has references.
-		# Thus, we forcibly decrease the reference count and rely on Exectuor's self-reporting to avoid accessing deallocated memory.
-		# This appears to cause segfaults on some systems, so we'll just live with the fact that Executors will never be destroyed.
-		# If you want your executor to stop being tracked, do it yourself. :(
-		#
-		# ctypes.pythonapi.Py_DecRef(ctypes.py_object(executor))
+		this.enableAutoReturn = False
+	
+	def Function(this):
+		# Prepare a dummy function to replace with a Method.
+		code = compile(f"def {this.target}(this):\n\tpass", '', 'exec')
+		exec(code)
 
-		logging.debug(f"Now tracking Executor: {executor}")
+		methodToAdd = SelfRegistering(this.impl)
+		methodToAdd.Constructor(eval(this.target), None)
+		for key, value in this.kwargs.items():
+			setattr(methodToAdd, key, value)
 
-	@staticmethod
-	def Pop(executor):
-		try:
-			ExecutorTracker.Instance().executors.remove(executor)
-			logging.debug(f"No longer tracking Executor: {executor}")
-		except:
-			pass
+		return methodToAdd
 
-	@staticmethod
-	def GetLatest():
-		return ExecutorTracker.Instance().executors[-1]
+def inject(
+	target,
+	impl="External",
+	**kwargs
+):
+	return Inject()(target=target, impl=impl, **kwargs)
 
 
 # AccessControl is used in Kind to control how Surfaces are created on a Functor & what is injected inside them.
 # parameters should roughly map to the parameters result of inspect.signature().parameters
 class AccessControl(Functor):
 	def __init__(this, name = "AccessControl"):
 		super().__init__(name)
@@ -1666,16 +1847,14 @@
 		for target, source in toInject.items():
 			this.parameters[target] = util.DotDict({
 				'kind': None,
 				'name': target,
 				'default': inject(source)
 			})
 
-		return this
-
 def public_methods(*args, **kwargs):
 	[kwargs.update({arg: arg}) for arg in args]
 	return PublicMethods()(**kwargs)
 
 def kind(
 	base = StandardFunctor,
 	**kwargs
@@ -1725,15 +1904,15 @@
 					ctor.source.append(f"this.requiredKWArgs.append('{arg.name}')")
 
 				if (shouldMapArg):
 					ctor.source.append(f"this.argMapping.append('{arg.name}')")
 
 			# Source mangling
 			# TODO: Expand as we have more solid test cases.
-			source = re.sub(fr"{arg.name}([\s\[\]\.\(\)\}}\*\+/-=%])", fr"{replaceWith}\1", source)
+			source = re.sub(fr"{arg.name}([\s\[\]\.\(\)\}}\*\+/-=%,]|$)", fr"{replaceWith}\1", source)
 			
 		return functor, source, ctor
 
 	def FunctionToFunctor(function):
 		executor = ExecutorTracker.GetLatest()
 		shouldLog = executor and executor.verbosity > 3
 
@@ -1751,15 +1930,15 @@
 
 		if ('name' not in kwargs):
 			kwargs['name'] = function.__name__
 	
 		args = inspect.signature(function).parameters
 		source = inspect.getsource(function)
 		source = source[source.find(':\n')+1:].strip() # Will fail if an arg has ':\n' in it
-		source = re.sub(r'caller([\s\[\]\.\(\)\}\*\+/-=%])', r'this.caller\1', source)
+		source = re.sub(r'caller([\s\[\]\.\(\)\}\*\+/-=%,]|$)', r'this.caller\1', source)
 
 		ctor = util.DotDict()
 		ctor.source = []
 		ctor.additions = ""
 
 		functor, source, ctor = ParseParameters(functor, args, source, ctor)
 
@@ -1789,114 +1968,194 @@
 		exec(f'functor.{primaryFunctionName} = {wrappedPrimaryFunction}')
 
 		return functor
 
 	return FunctionToFunctor
 
 
-class FetchCallbackFunctor(Functor):
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
 
-	def __init__(this, name = "FetchCallbackFunctor"):
+	def __init__(this, name=INVALID_NAME()):
 		super().__init__(name)
 
-		this.requiredKWArgs.append('varName')
-		this.requiredKWArgs.append('location')
-		this.requiredKWArgs.append('value')
+		# The data *this contains.
+		this.data = []
 
-		this.functionSucceeded = True
-		this.enableRollback = False
 
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
 
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
-#from .Executor import Executor # don't import this, it'll be circular!
 
-# @recoverable
-# Decorating another function with this method will engage the error recovery system provided by *this.
-# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
-# For more info, see Executor.ResolveError and the README.md
-def recoverable(function):
-	def RecoverableDecorator(obj, *args, **kwargs):
-		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
-	return RecoverableDecorator
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
 
 
-# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
-def RecoverableImplementation(obj, executor, function, *args, **kwargs):
-	try:
-		return function(obj, *args, **kwargs)
-	except FailedErrorResolution as fatal:
-		raise fatal
-	except Exception as e:
-		if (not executor.resolveErrors):
-			raise e
-		return Recover(e, obj, executor, function, *args, **kwargs)
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
 
 
-def Recover(error, obj, executor, function, *args, **kwargs):
-	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
-	util.LogStack()
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
 
-	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
-	if (str(error) not in executor.errorResolutionStack.keys()):
-		executor.errorResolutionStack.update({str(error):[]})
 
-	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
-	# ResolveError is itself @recoverable.
-	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
-	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
-	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
 
-	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
-		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
 
-	successfullyRecovered = False
-	ret = None
-	resolvedBy = None
-	for i, res in enumerate(executor.resolveErrorsWith):
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
 
-		logging.debug(f"Checking if {res} can fix '{error}'.")
-		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
-			# if no resolution was attempted, there's no need to re-run the function.
-			continue
+
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
 		try:
-			logging.debug(f"Trying function ({function}) again after applying {res}.")
-			resolvedBy = res
-			ret = function(obj, *args, **kwargs)
-			successfullyRecovered = True
-			break
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
 
-		except Exception as e2:
-			if (str(error) == str(e2)):
-				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
-				# Resolution failed. That's okay. Let's try the next.
-				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
+
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
 				continue
-			else:
-				# The error changed, maybe we're making progress.
-				ret = Recover(e2, obj, executor, function, *args, **kwargs)
-				successfullyRecovered = True
-				break
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
 
-	if (successfullyRecovered):
-		executor.ClearErrorResolutionStack(str(error)) # success!
-		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
-		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
-		return ret
 
-	#  We failed to resolve the error. Die
-	sys.tracebacklimit = 0 # traceback is NOT helpful here.
-	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
 
 
+
+class FetchCallbackFunctor(Functor):
+
+	def __init__(this, name = "FetchCallbackFunctor"):
+		super().__init__(name)
+
+		this.requiredKWArgs.append('varName')
+		this.requiredKWArgs.append('location')
+		this.requiredKWArgs.append('value')
+
+		this.functionSucceeded = True
+		this.enableRollback = False
+
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
+
 # Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
 # ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
 # Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
 # NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
 #
 # startPosition is always positive
 # endPosition is always negative
@@ -1939,14 +2198,15 @@
 		# No rollback, by default and definitely don't throw Exceptions.
 		this.enableRollback = False
 		this.functionSucceeded = True
 		this.raiseExceptions = False
 
 		this.errorShouldBeResolved = False
 
+		this.enableAutoReturn = False
 
 
 	# Put your logic here!
 	def Resolve(this):
 		# You get the following members:
 		# this.error (an Exception)
 		# this.errorString (a string cast of the Exception)
@@ -2074,14 +2334,15 @@
 
 		this.resolveErrors = True
 		this.errorRecursionDepth = 0
 		this.errorResolutionStack = {}
 		this.resolveErrorsWith = [ # order matters: FIFO (first is first).
 			'find_by_fetch',
 			'import_module',
+			'namespace_lookup',
 			'install_from_repo_with_default_package_type',
 			'install_from_repo',
 			'install_with_pip'
 		]
 
 		# Caching is required for Functor's staticKWArgs and other static features to be effective.
 		# This is used in Execute().
@@ -2118,14 +2379,18 @@
 		# Where should we log to?
 		# Set by Fetch('log_file')
 		this.log_file = None
 
 		# All repository configuration.
 		this.repo = util.DotDict()
 
+		# The observatory is a means of communicating with Constellatus.
+		# While the repo may provide any arbitrary data in zip format, Stars observed from Constellatus are specially handled.
+		this.observatory = util.DotDict()
+
 		# Placement helps to construct the correct load order of Functors as they are installed.
 		this.placement = util.DotDict()
 		this.placement.max = 255
 		this.placement.session = util.DotDict()
 		
 		# Defaults.
 		# You probably want to configure these in your own Executors.
@@ -2453,14 +2718,26 @@
 			"registry": str(Path(this.defaultRepoDirectory).joinpath('registry').resolve()),
 			"url": "https://api.infrastructure.tech/v1/package",
 			"username": None,
 			"password": None
 		}
 		for key, default in details.items():
 			this.repo[key] = this.Fetch(f"repo_{key}", default=default)
+	
+
+	# Get information for interacting with Constellatus
+	def PopulateObservatoryDetails(this):
+		details = {
+			"online": not this.Fetch('no_observatory', False, ['this', 'args', 'config']),
+			"url": "http://localhost:1137",
+			"username": None,
+			"password": None
+		}
+		for key, default in details.items():
+			this.observatory[key] = this.Fetch(f"observatory_{key}", default=default)
 
 
 	# How do we get the verbosity level and what do we do with it?
 	# This method should set log levels, etc.
 	def SetVerbosity(this, fetch=True):
 		if (fetch):
 			# Take the highest of -v vs --verbosity
@@ -2570,27 +2847,30 @@
 			current = current.methods[flowList.pop(0)]
 		return current()
 	
 
 	# Execute a Functor based on name alone (not object).
 	# If the given Functor has been Executed before, the cached Functor will be called again. Otherwise, a new Functor will be constructed.
 	@recoverable
-	def Execute(this, functorName, *args, **kwargs):
-		packageType = this.defaultPackageType
-		if ('packageType' in kwargs):
-			packageType = kwargs.pop('packageType')
+	def Execute(this, functor, *args, **kwargs):
+		if (isinstance(functor, str)):
+			functorName = functor
+			packageType = this.defaultPackageType
+			if ('packageType' in kwargs):
+				packageType = kwargs.pop('packageType')
 
-		logging.debug(f"Executing {functorName}({', '.join([str(a) for a in args] + [k+'='+str(v) for k,v in kwargs.items()])})")
-
-		if (functorName in this.cachedFunctors):
-			return this.cachedFunctors[functorName](*args, **kwargs, executor=this)
+			if (functorName in this.cachedFunctors):
+				functor = this.cachedFunctors[functorName]
+			else:
+				functor = this.GetRegistered(functorName, packageType)
+		else:
+			functorName = functor.name
 
-		functor = this.GetRegistered(functorName, packageType)
+		logging.debug(f"Executing {functorName}({', '.join([str(a) for a in args] + [k+'='+str(v) for k,v in kwargs.items()])})")
 		this.cachedFunctors.update({functorName: functor})
-
 		return functor(*args, **kwargs, executor=this)
 
 
 	# Attempts to download the given package from the repo url specified in calling args.
 	# Will refresh registered classes upon success
 	# RETURNS whether or not the package was downloaded. Will raise Exceptions on errors.
 	# Does not guarantee new classes are made available; errors need to be handled by the caller.
@@ -2670,31 +2950,80 @@
 		os.remove(packageZipPath)
 
 		if (registerClasses):
 			this.RegisterAllClassesInDirectory(this.repo.registry)
 
 		return True
 
+
+	@recoverable
+	def ObserveStarCluster(this, starCluster):
+		
+		if (not this.observatory.online):
+			logging.debug(f"Refusing to observe {starCluster}; we were told not to use an observatory.")
+			raise ConstellatusError(f"Unable to observe {starCluster}: Observatory is offline.")
+		
+		logging.debug(f"Observing {starCluster}")
+
+		url = f"{this.observatory.url}/{starCluster}"
+
+		auth = None
+		if this.observatory.username and this.observatory.password:
+			auth = requests.auth.HTTPBasicAuth(this.observatory.username, this.observatory.password)
+
+		headers = {
+			"Connection": "keep-alive",
+		}
+
+		observation = requests.get(url, auth=auth, headers=headers, stream=True)
+
+		if (observation.status_code != 200):
+			raise ConstellatusError(f"Unable to observe {starCluster}")
+		
+		try:
+			# Load the code from Constellatus into a module on the fly
+			moduleName = starCluster.replace(':', '_').replace('.', '_')
+			spec = importlib.util.spec_from_loader(moduleName, loader=None)
+			module = importlib.util.module_from_spec(spec)
+			exec(observation.content, module.__dict__)
+			sys.modules[moduleName] = module
+			globals()[moduleName] = module
+			logging.debug(f"Completed observation of {starCluster}")
+		except Exception as e:
+			raise ConstellatusError(f"Unable to observe {starCluster}: {e}")
+
+
 	# RETURNS and instance of a Datum, Functor, etc. (aka modules) which has been discovered by a prior call of RegisterAllClassesInDirectory()
 	# Will attempt to register existing modules if one of the given name is not found. Failing that, the given package will be downloaded if it can be found online.
 	# Both python modules and other eons modules of the same packageType will be installed automatically in order to meet all required dependencies of the given module.
 	@recoverable
 	def GetRegistered(this,
 		registeredName,
-		packageType=""):
+		packageType="",
+		namespace=None):
+
+		if (packageType):
+			packageType = "." + packageType
+		
+		if (namespace):
+			registeredName = Namespace(namespace).ToName() + registeredName
 
 		try:
 			registered = SelfRegistering(registeredName)
 		except Exception as e:
-			# We couldn't get what was asked for. Let's try asking for help from the error resolution machinery.
-			packageName = registeredName
-			if (packageType):
-				packageName = f"{registeredName}.{packageType}"
-			logging.error(f"While trying to instantiate {packageName}, got: {e}")
-			raise HelpWantedWithRegistering(f"Trying to get SelfRegistering {packageName}")
+			try:
+				# If the Observatory is online, let's try to use Constellatus.
+				this.ObserveStarCluster(f"{str(Namespace(namespace))}{registeredName}{packageType}")
+				registered = SelfRegistering(registeredName)
+			except: # We don't care about Constellatus errors right now.
+
+				# We couldn't get what was asked for. Let's try asking for help from the error resolution machinery.
+				packageName = registeredName + packageType
+				logging.error(f"While trying to instantiate {packageName}, got: {e}")
+				raise HelpWantedWithRegistering(f"Trying to get SelfRegistering {packageName}")
 
 		# NOTE: Functors are Data, so they have an IsValid() method
 		if (not registered or not registered.IsValid()):
 			logging.error(f"No valid object: {registeredName}")
 			raise FatalCannotExecute(f"No valid object: {registeredName}")
 
 		return registered
@@ -2711,23 +3040,14 @@
 
 		if (directory not in this.syspath):
 			this.syspath.append(directory)
 
 		SelfRegistering.RegisterAllClassesInDirectory(directory, recurse=recurse)
 
 
-	# Utility method. may not be useful.
-	@staticmethod
-	def SplitNameOnpackageType(name):
-		splitName = name.split('_')
-		if (len(splitName)>1):
-			return splitName[0], splitName[1]
-		return "", name
-
-
 	# Set a global value for use throughout all python modules.
 	def SetGlobal(this, name, value, setFromFetch=False):
 		# In cause the value was accessed with ".", we need to cast it to a DotDict.
 		if (isinstance(value, dict)):
 			value = util.DotDict(value)
 
 		logging.debug(f"Setting global value {name} = {value}")
```

### Comparing `eons-2.7.3/pkg/eons/method/External.py` & `eons-3.0.0/pkg/eons/method/External.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,44 +15,50 @@
 		this.type = None
 		this.functorName = ""
 		this.functor = None
 
 	def UpdateSource(this):
 		if (not this.type):
 			this.type = eons.ExecutorTracker.GetLatest().defaultPackageType
-
-		this.functor = eons.ExecutorTracker.GetLatest().GetRegistered(this.functorName, this.type)
+		try:
+			this.functor = eons.ExecutorTracker.GetLatest().GetRegistered(this.functorName, this.type, namespace = this.caller.name)
+		except:
+			this.functor = eons.ExecutorTracker.GetLatest().GetRegistered(this.functorName, this.type)
 
 		if (not this.functor):
 			raise eons.MissingMethodError(f"Could not populate external method {this.functorName} (type {this.type})")
 		
 		this.functor.name = f"{this.functor.name} (external)"
+		this.enableAutoReturn = this.functor.enableAutoReturn
 
-		# To allow this.functor to be called with *args, we must also allow this to be called with *args.
-		this.argMapping = this.functor.argMapping
+		# To allow this.functor to be called with *args, we must also allow this to be called with *args (+ this).
+		this.argMapping += this.functor.argMapping
 
 	def PopulateFrom(this, function):
 		this.functorName = function.__name__
 
 	def GetKWArgsForMethod(this):
 		kwargs = this.kwargs
 		kwargs.update({
 			'executor': this.executor,
 			'precursor': this,
 		})
 		this.functor.caller = this.caller
 		return kwargs
+	
+	def WarmUp(this, *args, **kwargs):
+		super().WarmUp(*args, **kwargs)
+		this.functor.WarmUp(*this.args[1:], **this.GetKWArgsForMethod())
 
 	def Function(this):
-		ret = this.functor(*this.args, **this.GetKWArgsForMethod())
+		ret = this.functor.Function()
 		this.result = this.functor.result
 		return ret
 
 	def Rollback(this):
-		this.functor.WarmUp(*this.args, **this.GetKWArgsForMethod())
 		ret = this.functor.Rollback()
 		this.result = this.functor.result
 		return ret
 	
 	def DidFunctionSucceed(this):
 		return this.functor.DidFunctionSucceed()
```

### Comparing `eons-2.7.3/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-3.0.0/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.3/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-3.0.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.3/pkg/eons.egg-info/PKG-INFO` & `eons-3.0.0/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.3
+Version: 3.0.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.7.3/pkg/eons.egg-info/SOURCES.txt` & `eons-3.0.0/pkg/eons.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 pkg/eons/method/External.py
 pkg/eons/method/__init__.py
 pkg/eons/resolve/__init__.py
 pkg/eons/resolve/resolve_find_by_fetch.py
 pkg/eons/resolve/resolve_import_module.py
 pkg/eons/resolve/resolve_install_from_repo.py
 pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
-pkg/eons/resolve/resolve_install_with_pip.py
+pkg/eons/resolve/resolve_install_with_pip.py
+pkg/eons/resolve/resolve_namespace_lookup.py
```

### Comparing `eons-2.7.3/setup.cfg` & `eons-3.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.7.3
+version = 3.0.0
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,20 +18,20 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	requests_futures
 	tqdm
-	eot
-	jsonpickle
 	pyyaml
+	requests_futures
+	jsonpickle
 	requests
+	eot
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

