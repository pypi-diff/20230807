# Comparing `tmp/apie-0.0.6.tar.gz` & `tmp/apie-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apie-0.0.6.tar", last modified: Mon Apr 24 23:05:55 2023, max compression
+gzip compressed data, was "apie-0.0.7.tar", last modified: Mon Aug  7 00:29:11 2023, max compression
```

## Comparing `apie-0.0.6.tar` & `apie-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-24 23:05:55.427378 apie-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-24 23:05:38.000000 apie-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.423378 apie-0.0.6/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/api/api_hack.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/api/api_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/api/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16245 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/apie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/auth/auth_from_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/auth/auth_noauth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 23:05:46.000000 apie-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 23:05:55.427378 apie-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:29:11.239506 apie-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-08-07 00:29:11.239506 apie-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-08-07 00:28:50.000000 apie-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:29:11.231506 apie-0.0.7/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:29:11.235506 apie-0.0.7/pkg/apie/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 00:28:59.000000 apie-0.0.7/pkg/apie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 00:28:59.000000 apie-0.0.7/pkg/apie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:29:11.239506 apie-0.0.7/pkg/apie/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:28:59.000000 apie-0.0.7/pkg/apie/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-07 00:28:29.000000 apie-0.0.7/pkg/apie/api/api_hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-07 00:28:29.000000 apie-0.0.7/pkg/apie/api/api_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-07 00:28:29.000000 apie-0.0.7/pkg/apie/api/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-08-07 00:28:59.000000 apie-0.0.7/pkg/apie/apie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:29:11.239506 apie-0.0.7/pkg/apie/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:28:59.000000 apie-0.0.7/pkg/apie/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 00:28:29.000000 apie-0.0.7/pkg/apie/auth/auth_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 00:28:29.000000 apie-0.0.7/pkg/apie/auth/auth_noauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:29:11.239506 apie-0.0.7/pkg/apie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-08-07 00:29:11.000000 apie-0.0.7/pkg/apie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 00:29:11.000000 apie-0.0.7/pkg/apie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:29:11.000000 apie-0.0.7/pkg/apie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 00:29:11.000000 apie-0.0.7/pkg/apie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 00:29:11.000000 apie-0.0.7/pkg/apie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 00:29:11.000000 apie-0.0.7/pkg/apie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 00:28:59.000000 apie-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-07 00:29:11.243506 apie-0.0.7/setup.cfg
```

### Comparing `apie-0.0.6/PKG-INFO` & `apie-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apie
-Version: 0.0.6
+Version: 0.0.7
 Summary: Application Program Interface with eons
 Home-page: https://github.com/eons-dev/bin_apie
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_apie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `apie-0.0.6/README.md` & `apie-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `apie-0.0.6/pkg/apie/api/api_hack.py` & `apie-0.0.7/pkg/apie/api/api_hack.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.6/pkg/apie/api/api_help.py` & `apie-0.0.7/pkg/apie/api/api_help.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.6/pkg/apie/api/api_multi.py` & `apie-0.0.7/pkg/apie/api/api_multi.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.6/pkg/apie/apie.py` & `apie-0.0.7/pkg/apie/apie.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,206 +83,14 @@
 
 	def fetch_location_request_files(this, varName, default, fetchFrom, attempted):
 		if (not this.request.files):
 			return  default, False
 		return this.FetchFromRequest('files', varName, default)
 
 
-class APIE(eons.Executor):
-
-	def __init__(this):
-		super().__init__(name="Application Program Interface with Eons", descriptionStr="A readily extensible take on APIs.")
-
-		# this.RegisterDirectory("ebbs")
-
-		this.optionalKWArgs['host'] = "0.0.0.0"
-		this.optionalKWArgs['port'] = 80
-		this.optionalKWArgs['dev'] = False
-		this.optionalKWArgs['clean_start'] = False
-		this.optionalKWArgs['authenticator'] = "noauth"
-		this.optionalKWArgs['preprocessor'] = ""
-
-		this.supportedMethods = [
-			'POST',
-			'GET',
-			'PUT',
-			'DELETE',
-			'PATCH'
-		]
-
-		# Used in Function()
-		this.auth = None
-		this.flask = None
-
-		# *this is single-threaded. If we want parallel processing, we can create replicas.
-		this.lastEndpoint = None
-
-		this.defaultConfigFile = "apie.json"
-		this.defaultPackageType = "api"
-
-	# Override of eons.Executor method. See that class for details
-	def RegisterIncludedClasses(this):
-		super().RegisterIncludedClasses()
-		this.RegisterAllClassesInDirectory(str(Path(__file__).resolve().parent.joinpath("api")))
-		this.RegisterAllClassesInDirectory(str(Path(__file__).resolve().parent.joinpath("auth")))
-		
-
-	# Override of eons.Executor method. See that class for details
-	def RegisterAllClasses(this):
-		super().RegisterAllClasses()
-
-
-	# Acquire and run the given endpoint with the given request.
-	def ProcessEndpoint(this, endpointName, request, **kwargs):
-
-		# Parse Endpoint syntax.
-		# "[..., ...]something" => multi(domain=[..., ...], next="something")
-		if (endpointName.startswith('[')):
-			if ('domain' in kwargs):
-				raise APIError(f"Domain already exists in multicall; domain={kwargs['domain']}; multicall={endpointName}")
-
-			domainStrEndPos = endpointName.find(']')+1
-			domainStr = endpointName[:domainStrEndPos]
-			if ('next' in kwargs):
-				kwargs['next'] = [endpointName[domainStrEndPos:]].extend(kwargs['next'])
-			else:
-				kwargs['next'] = endpointName[domainStrEndPos:]
-
-			# Trim '(' and ')', then make list.
-			kwargs['domain'] = domainStr[1:-1].split(',')
-
-			endpointName = "multi"
-
-		if (endpointName in this.cachedFunctors):
-			return this.cachedFunctors[endpointName](executor=this, request=request, **kwargs)
-
-		endpoint = this.GetRegistered(endpointName, "api")
-		this.cachedFunctors.update({endpointName: endpoint})
-		return endpoint(executor=this, request=request, **kwargs)
-
-
-	# What to do when a request causes an exception to be thrown.
-	def HandleBadRequest(this, request, error):
-		message = f"Bad request: {str(error)}"
-		return message, 400
-
-
-	# Override of eons.Executor method. See that class for details
-	def Function(this):
-		super().Function()
-
-		if (this.clean_start):
-			this.Clean()
-
-		this.auth = this.GetRegistered(this.authenticator, "auth")
-
-		this.flask = Flask(this.name)
-
-		@this.flask.route("/", defaults={"path": ""}, methods = this.supportedMethods)
-		def root(path):
-			return "It works!", 200
-
-		@this.flask.route("/<string:path>", methods = this.supportedMethods)
-		@this.flask.route("/<path:path>", methods = this.supportedMethods)
-		def handler(path):
-			try:
-				if (this.auth(executor=this, path=path, request=request)):
-					endpoints = []
-					if (this.preprocessor):
-						endpoints.append(this.preprocessor)
-					if (path.endswith('/')):
-						path = path[:-1]
-					endpoints.extend(path.split('/'))
-					this.lastEndpoint = None
-					logging.debug(f"Responding to request for {path}; request: {request}")
-					response = this.ProcessEndpoint(endpoints.pop(0), request, next=endpoints)
-					logging.debug(f"Got headers: {response.headers}")
-					logging.debug(f"Got response: {response}")
-					return response
-				else:
-					return this.auth.Unauthorized(path)
-			except Exception as error:
-				traceback.print_exc()
-				logging.error(str(error))
-				if (this.lastEndpoint):
-					try:
-						return this.lastEndpoint.HandleBadRequest(request, error)
-					except Exception:
-						pass
-				return this.HandleBadRequest(request, error) #fine. We'll do it ourselves.
-
-		options = {}
-		options['app'] = this.flask
-		options['host'] = this.host
-		options['port'] = this.port
-
-		# Only applicable if using this.flask.run(**options)
-		# if (this.args.verbose > 0):
-		#	 options['debug'] = True
-		#	 options['use_reloader'] = False
-
-		serve(**options)
-
-
-	# Remove possibly stale modules.
-	def Clean(this):
-		repoPath = Path(this.repo['store'])
-		if (repoPath.exists()):
-			shutil.rmtree(this.repo['store'])
-		repoPath.mkdir(parents=True, exist_ok=True)
-
-
-# Authenticator is a Functor which validates whether or not a request is valid.
-# The inputs will be the path of the request and the request itself.
-# If you need to check whether the request parameters, data, files, etc. are valid, please do so in your Endpoint.
-# Because this class will be invoked often, we have made some performant modifications to the default Functor methods.
-# Authenticators may be called sequentially but in such a case, only the last Authenticator will Authenticate(), all precursors are skipped over.
-# NOTE: All logic for *this should be in Authenticate. There are no extra functions called (e.g. PreCall, PostCall, etc.)
-# Authenticate should either return False or raise an exception if the provided request is invalid and should return True if it is.
-class Authenticator(Functor):
-	def __init__(this, name="Authenticator"):
-		super().__init__(name)
-
-	# Override of eons.Functor method. See that class for details
-	# NOTE: All logic for *this should be in Authenticate. There are no extra functions called (e.g. PreCall, PostCall, etc.)
-	# Authenticate should either return False or raise an exception if the provided request is invalid and should return True if it is.
-	def Authenticate(this):
-		return True
-
-	# This will be called whenever an unauthorized request is made.
-	def Unauthorized(this, path):
-		logging.debug(f"Unauthorized: {this.name} on {path}")
-		return "Unauthorized", 401
-
-	# Override of eons.Functor method. See that class for details
-	def ParseInitialArgs(this):
-		super().ParseInitialArgs()
-
-		this.path = this.kwargs.pop('path')
-
-	# Override of eons.Functor method. See that class for details
-	# Slimmed down for performance
-	def __call__(this, *args, **kwargs):
-		this.args = args
-		this.kwargs = kwargs
-		
-		this.PopulatePrecursor()
-		this.Initialize() # nop on call 2+
-		this.PopulateMethods() # Doesn't require Fetch; depends on precursor
-		this.ParseInitialArgs() # Usually where config is read in.
-		this.ValidateStaticArgs() # nop on call 2+
-		this.ValidateArgs()
-		this.PopulateNext()
-		this.ValidateMethods()
-
-		if (this.next):
-			return this.CallNext()
-		return this.Authenticate()
-
-
 # Endpoints are what is run when a given request is successfully authenticated.
 # Put all your actual API logic in these!
 # Keep in mind that Endpoints will be made available in a just-in-time, as-needed basis. There is no need to preload logic, etc.
 # That also means that each Endpoint should operate in isolation and not require any other Endpoint to function.
 # The exception to this isolation is when Endpoints are intended to be called in sequence.
 # Any number of Endpoints can be chained together in any order. The behavior of the first affects the behavior of the last.
 # This allows you to create generic "upload" Endpoints, where what is uploaded is determined by the preceding Endpoint.
@@ -485,7 +293,199 @@
 			if (this.next and this.next[-1] == 'help'):
 				return
 			raise e
 		
 
 
 
+
+# Authenticator is a Functor which validates whether or not a request is valid.
+# The inputs will be the path of the request and the request itself.
+# If you need to check whether the request parameters, data, files, etc. are valid, please do so in your Endpoint.
+# Because this class will be invoked often, we have made some performant modifications to the default Functor methods.
+# Authenticators may be called sequentially but in such a case, only the last Authenticator will Authenticate(), all precursors are skipped over.
+# NOTE: All logic for *this should be in Authenticate. There are no extra functions called (e.g. PreCall, PostCall, etc.)
+# Authenticate should either return False or raise an exception if the provided request is invalid and should return True if it is.
+class Authenticator(Functor):
+	def __init__(this, name="Authenticator"):
+		super().__init__(name)
+
+	# Override of eons.Functor method. See that class for details
+	# NOTE: All logic for *this should be in Authenticate. There are no extra functions called (e.g. PreCall, PostCall, etc.)
+	# Authenticate should either return False or raise an exception if the provided request is invalid and should return True if it is.
+	def Authenticate(this):
+		return True
+
+	# This will be called whenever an unauthorized request is made.
+	def Unauthorized(this, path):
+		logging.debug(f"Unauthorized: {this.name} on {path}")
+		return "Unauthorized", 401
+
+	# Override of eons.Functor method. See that class for details
+	def ParseInitialArgs(this):
+		super().ParseInitialArgs()
+
+		this.path = this.kwargs.pop('path')
+
+	# Override of eons.Functor method. See that class for details
+	# Slimmed down for performance
+	def __call__(this, *args, **kwargs):
+		this.args = args
+		this.kwargs = kwargs
+		
+		this.PopulatePrecursor()
+		this.Initialize() # nop on call 2+
+		this.PopulateMethods() # Doesn't require Fetch; depends on precursor
+		this.ParseInitialArgs() # Usually where config is read in.
+		this.ValidateStaticArgs() # nop on call 2+
+		this.ValidateArgs()
+		this.PopulateNext()
+		this.ValidateMethods()
+
+		if (this.next):
+			return this.CallNext()
+		return this.Authenticate()
+
+
+class APIE(eons.Executor):
+
+	def __init__(this, name="Application Program Interface with Eons", description="A readily extensible take on APIs."):
+		super().__init__(name, description)
+
+		# this.RegisterDirectory("ebbs")
+
+		this.optionalKWArgs['host'] = "0.0.0.0"
+		this.optionalKWArgs['port'] = 80
+		this.optionalKWArgs['dev'] = False
+		this.optionalKWArgs['clean_start'] = False
+		this.optionalKWArgs['authenticator'] = "noauth"
+		this.optionalKWArgs['preprocessor'] = ""
+
+		this.supportedMethods = [
+			'POST',
+			'GET',
+			'PUT',
+			'DELETE',
+			'PATCH'
+		]
+
+		# Used in Function()
+		this.auth = None
+		this.flask = None
+
+		# *this is single-threaded. If we want parallel processing, we can create replicas.
+		this.lastEndpoint = None
+
+		this.defaultConfigFile = "apie.json"
+		this.defaultPackageType = "api"
+
+	# Override of eons.Executor method. See that class for details
+	def RegisterIncludedClasses(this):
+		super().RegisterIncludedClasses()
+		this.RegisterAllClassesInDirectory(str(Path(__file__).resolve().parent.joinpath("api")))
+		this.RegisterAllClassesInDirectory(str(Path(__file__).resolve().parent.joinpath("auth")))
+		
+
+	# Override of eons.Executor method. See that class for details
+	def RegisterAllClasses(this):
+		super().RegisterAllClasses()
+
+
+	# Acquire and run the given endpoint with the given request.
+	def ProcessEndpoint(this, endpointName, request, **kwargs):
+
+		# Parse Endpoint syntax.
+		# "[..., ...]something" => multi(domain=[..., ...], next="something")
+		if (endpointName.startswith('[')):
+			if ('domain' in kwargs):
+				raise APIError(f"Domain already exists in multicall; domain={kwargs['domain']}; multicall={endpointName}")
+
+			domainStrEndPos = endpointName.find(']')+1
+			domainStr = endpointName[:domainStrEndPos]
+			if ('next' in kwargs):
+				kwargs['next'] = [endpointName[domainStrEndPos:]].extend(kwargs['next'])
+			else:
+				kwargs['next'] = endpointName[domainStrEndPos:]
+
+			# Trim '(' and ')', then make list.
+			kwargs['domain'] = domainStr[1:-1].split(',')
+
+			endpointName = "multi"
+
+		if (endpointName in this.cachedFunctors):
+			return this.cachedFunctors[endpointName](executor=this, request=request, **kwargs)
+
+		endpoint = this.GetRegistered(endpointName, "api")
+		this.cachedFunctors.update({endpointName: endpoint})
+		return endpoint(executor=this, request=request, **kwargs)
+
+
+	# What to do when a request causes an exception to be thrown.
+	def HandleBadRequest(this, request, error):
+		message = f"Bad request: {str(error)}"
+		return message, 400
+
+
+	# Override of eons.Executor method. See that class for details
+	def Function(this):
+		super().Function()
+
+		if (this.clean_start):
+			this.Clean()
+
+		this.auth = this.GetRegistered(this.authenticator, "auth")
+
+		this.flask = Flask(this.name)
+
+		@this.flask.route("/", defaults={"path": ""}, methods = this.supportedMethods)
+		def root(path):
+			return "It works!", 200
+
+		@this.flask.route("/<string:path>", methods = this.supportedMethods)
+		@this.flask.route("/<path:path>", methods = this.supportedMethods)
+		def handler(path):
+			try:
+				if (this.auth(executor=this, path=path, request=request)):
+					endpoints = []
+					if (this.preprocessor):
+						endpoints.append(this.preprocessor)
+					if (path.endswith('/')):
+						path = path[:-1]
+					endpoints.extend(path.split('/'))
+					this.lastEndpoint = None
+					logging.debug(f"Responding to request for {path}; request: {request}")
+					response = this.ProcessEndpoint(endpoints.pop(0), request, next=endpoints)
+					logging.debug(f"Got headers: {response.headers}")
+					logging.debug(f"Got response: {response}")
+					return response
+				else:
+					return this.auth.Unauthorized(path)
+			except Exception as error:
+				traceback.print_exc()
+				logging.error(str(error))
+				if (this.lastEndpoint):
+					try:
+						return this.lastEndpoint.HandleBadRequest(request, error)
+					except Exception:
+						pass
+				return this.HandleBadRequest(request, error) #fine. We'll do it ourselves.
+
+		options = {}
+		options['app'] = this.flask
+		options['host'] = this.host
+		options['port'] = this.port
+
+		# Only applicable if using this.flask.run(**options)
+		# if (this.args.verbose > 0):
+		#	 options['debug'] = True
+		#	 options['use_reloader'] = False
+
+		serve(**options)
+
+
+	# Remove possibly stale modules.
+	def Clean(this):
+		repoPath = Path(this.repo['store'])
+		if (repoPath.exists()):
+			shutil.rmtree(this.repo['store'])
+		repoPath.mkdir(parents=True, exist_ok=True)
+
```

### Comparing `apie-0.0.6/pkg/apie/auth/auth_from_config.py` & `apie-0.0.7/pkg/apie/auth/auth_from_config.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.6/pkg/apie/auth/auth_noauth.py` & `apie-0.0.7/pkg/apie/auth/auth_noauth.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.6/pkg/apie.egg-info/PKG-INFO` & `apie-0.0.7/pkg/apie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apie
-Version: 0.0.6
+Version: 0.0.7
 Summary: Application Program Interface with eons
 Home-page: https://github.com/eons-dev/bin_apie
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_apie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `apie-0.0.6/setup.cfg` & `apie-0.0.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apie
-version = 0.0.6
+version = 0.0.7
 author = eons
 author_email = support@eons.llc
 description = Application Program Interface with eons
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_apie
@@ -18,17 +18,17 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
+	eons
 	flask
 	waitress
-	eons
 	jsonpickle
 
 [options.packages.find]
 where = pkg
 
 [options.entry_points]
 console_scripts =
```

