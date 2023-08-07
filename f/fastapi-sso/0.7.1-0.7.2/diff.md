# Comparing `tmp/fastapi_sso-0.7.1.tar.gz` & `tmp/fastapi_sso-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sso-0.7.1.tar", max compression
+gzip compressed data, was "fastapi_sso-0.7.2.tar", max compression
```

## Comparing `fastapi_sso-0.7.1.tar` & `fastapi_sso-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1093 2023-02-07 15:13:40.445140 fastapi_sso-0.7.1/LICENSE.md
--rw-r--r--   0        0        0     6118 2023-07-25 18:36:55.037625 fastapi_sso-0.7.1/README.md
--rw-r--r--   0        0        0     1110 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/__init__.py
--rw-r--r--   0        0        0        0 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/__init__.py
--rw-r--r--   0        0        0    11117 2023-07-25 18:00:47.042827 fastapi_sso-0.7.1/fastapi_sso/sso/base.py
--rw-r--r--   0        0        0     1215 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/facebook.py
--rw-r--r--   0        0        0     1146 2023-03-25 12:01:05.759478 fastapi_sso-0.7.1/fastapi_sso/sso/fitbit.py
--rw-r--r--   0        0        0     2506 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/generic.py
--rw-r--r--   0        0        0      918 2023-07-26 10:46:06.524412 fastapi_sso-0.7.1/fastapi_sso/sso/github.py
--rw-r--r--   0        0        0      920 2023-07-25 18:02:43.979431 fastapi_sso-0.7.1/fastapi_sso/sso/gitlab.py
--rw-r--r--   0        0        0     1319 2023-03-25 12:01:05.771478 fastapi_sso-0.7.1/fastapi_sso/sso/google.py
--rw-r--r--   0        0        0      753 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/kakao.py
--rw-r--r--   0        0        0     1574 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/microsoft.py
--rw-r--r--   0        0        0      807 2023-07-25 09:20:48.153414 fastapi_sso-0.7.1/fastapi_sso/sso/naver.py
--rw-r--r--   0        0        0     1172 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/spotify.py
--rw-r--r--   0        0        0      944 2023-07-26 10:47:48.701371 fastapi_sso-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 fastapi_sso-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-08-03 19:12:06.791996 fastapi_sso-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0     7447 2023-08-06 07:33:27.249562 fastapi_sso-0.7.2/README.md
+-rw-r--r--   0        0        0     1110 2023-08-03 19:12:06.798839 fastapi_sso-0.7.2/fastapi_sso/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:12:06.799270 fastapi_sso-0.7.2/fastapi_sso/sso/__init__.py
+-rw-r--r--   0        0        0    11197 2023-08-07 17:12:40.796740 fastapi_sso-0.7.2/fastapi_sso/sso/base.py
+-rw-r--r--   0        0        0     1215 2023-08-03 19:12:06.800047 fastapi_sso-0.7.2/fastapi_sso/sso/facebook.py
+-rw-r--r--   0        0        0     1146 2023-08-03 19:12:06.800357 fastapi_sso-0.7.2/fastapi_sso/sso/fitbit.py
+-rw-r--r--   0        0        0     2506 2023-08-03 19:12:06.800668 fastapi_sso-0.7.2/fastapi_sso/sso/generic.py
+-rw-r--r--   0        0        0      918 2023-08-03 19:12:06.800982 fastapi_sso-0.7.2/fastapi_sso/sso/github.py
+-rw-r--r--   0        0        0      920 2023-08-03 19:12:06.801253 fastapi_sso-0.7.2/fastapi_sso/sso/gitlab.py
+-rw-r--r--   0        0        0     1319 2023-08-03 19:12:06.801549 fastapi_sso-0.7.2/fastapi_sso/sso/google.py
+-rw-r--r--   0        0        0      753 2023-08-03 19:12:06.801888 fastapi_sso-0.7.2/fastapi_sso/sso/kakao.py
+-rw-r--r--   0        0        0     1766 2023-08-07 17:21:24.326847 fastapi_sso-0.7.2/fastapi_sso/sso/microsoft.py
+-rw-r--r--   0        0        0      808 2023-08-06 07:33:27.259267 fastapi_sso-0.7.2/fastapi_sso/sso/naver.py
+-rw-r--r--   0        0        0     1138 2023-08-05 22:39:41.259680 fastapi_sso-0.7.2/fastapi_sso/sso/spotify.py
+-rw-r--r--   0        0        0     1899 2023-08-07 17:22:52.990212 fastapi_sso-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 fastapi_sso-0.7.2/PKG-INFO
```

### Comparing `fastapi_sso-0.7.1/LICENSE.md` & `fastapi_sso-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/README.md` & `fastapi_sso-0.7.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # FastAPI SSO
 
+![Supported Python Versions](https://img.shields.io/pypi/pyversions/fastapi-sso)
+![Test Coverage](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgist.githubusercontent.com%2Ftomasvotava%2F328acf6207500c2e836b1c68b5c910f7%2Fraw%2F&query=totals.percent_covered_display&suffix=%25&logo=pytest&label=coverage&color=blue&cacheSeconds=300
+)
+![Tests Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/test.yml?label=tests)
+![Pylint Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=pylint)
+![Mypy Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=mypy)
+![Black Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=black)
+![CodeQL Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/codeql-analysis.yml?label=CodeQL)
+![PyPi weekly downloads](https://img.shields.io/pypi/dw/fastapi-sso)
+![Project License](https://img.shields.io/github/license/tomasvotava/fastapi-sso)
+![PyPi Version](https://img.shields.io/pypi/v/fastapi-sso)
+
 FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 account).
 
 This allows you to implement the famous `Login with Google/Facebook/Microsoft` buttons functionality on your backend very easily.
 
 ## Security warning
 
 Please note that versions preceding `0.7.0` had a security vulnerability.
@@ -103,15 +115,16 @@
 ...
 
 google_sso = GoogleSSO("my-client-id", "my-client-secret")
 
 @app.get("/google/login")
 async def google_login(request: Request):
     """Generate login url and redirect"""
-    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
+    with google_sso:
+        return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
 
 @app.get("/google/callback")
 async def google_callback(request: Request):
     ...
 ```
 
 ### Specify scope
@@ -130,18 +143,19 @@
 sent to the login screen.
 
 E.g. sometimes you want to specify `access_type=offline` or `prompt=consent` in order for
 Google to return `refresh_token`.
 
 ```python
 async def google_login(request: Request):
-    return await google_sso.get_login_redirect(
-        redirect_uri=request.url_for("google_callback"),
-        params={"prompt": "consent", "access_type": "offline"}
-        )
+    with google_sso:
+        return await google_sso.get_login_redirect(
+            redirect_uri=request.url_for("google_callback"),
+            params={"prompt": "consent", "access_type": "offline"}
+            )
 
 ```
 
 ## HTTP and development
 
 **You should always use `https` in production**. But in case you need to test on `localhost` and do not want to
 use self-signed certificate, make sure you set up redirect uri within your SSO provider to `http://localhost:{port}`
@@ -169,23 +183,25 @@
 
 ```python
 from fastapi import Request
 from fastapi.responses import RedirectResponse
 
 # E.g. https://example.com/auth/login?return_url=https://example.com/welcome
 async def google_login(return_url: str):
-    google_sso = GoogleSOO("client-id", "client-secret")
-    # Send return_url to Google as a state so that Google knows to return it back to us
-    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"), state=return_url)
+    with google_sso:
+        google_sso = GoogleSOO("client-id", "client-secret")
+        # Send return_url to Google as a state so that Google knows to return it back to us
+        return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"), state=return_url)
 
 async def google_callback(request: Request):
-    google_sso = GoogleSOO("client-id", "client-secret")
-    user = await google_sso.verify_and_process(request)
-    # google_sso.state now holds your return_url (https://example.com/welcome)
-    return RedirectResponse(google_sso.state)
+    with google_sso:
+        google_sso = GoogleSOO("client-id", "client-secret")
+        user = await google_sso.verify_and_process(request)
+        # google_sso.state now holds your return_url (https://example.com/welcome)
+        return RedirectResponse(google_sso.state)
 
 ```
 
 **Deprecation Warning**: legacy `use_state` argument in `SSOBase` constructor is deprecated and will be removed.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,17 +1,31 @@
-# FastAPI SSO FastAPI plugin to enable SSO to most common providers (such as
-Facebook login, Google login and login via Microsoft Office 365 account). This
-allows you to implement the famous `Login with Google/Facebook/Microsoft`
-buttons functionality on your backend very easily. ## Security warning Please
-note that versions preceding `0.7.0` had a security vulnerability. The SSO
-instance could share state between requests, which could lead to security
-issues. **Please update to `0.7.0` or newer**. Also, the preferred way of using
-the SSO instances is to use `with` statement, which will ensure the state is
-cleared. See example below. ## Support this project If you'd like to support
-this project, consider [buying me a coffee â](https://www.buymeacoffee.com/
+# FastAPI SSO ![Supported Python Versions](https://img.shields.io/pypi/
+pyversions/fastapi-sso) ![Test Coverage](https://img.shields.io/badge/dynamic/
+json?url=https%3A%2F%2Fgist.githubusercontent.com%2Ftomasvotava%2F328acf6207500c2e836b1c68b5c910f7%2Fraw%2F&query=totals.percent_covered_display&suffix=%25&logo=pytest&label=coverage&color=blue&cacheSeconds=300
+) ![Tests Workflow Status](https://img.shields.io/github/actions/workflow/
+status/tomasvotava/fastapi-sso/test.yml?label=tests) ![Pylint Workflow Status]
+(https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/
+lint.yml?label=pylint) ![Mypy Workflow Status](https://img.shields.io/github/
+actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=mypy) ![Black
+Workflow Status](https://img.shields.io/github/actions/workflow/status/
+tomasvotava/fastapi-sso/lint.yml?label=black) ![CodeQL Workflow Status](https:/
+/img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/codeql-
+analysis.yml?label=CodeQL) ![PyPi weekly downloads](https://img.shields.io/
+pypi/dw/fastapi-sso) ![Project License](https://img.shields.io/github/license/
+tomasvotava/fastapi-sso) ![PyPi Version](https://img.shields.io/pypi/v/fastapi-
+sso) FastAPI plugin to enable SSO to most common providers (such as Facebook
+login, Google login and login via Microsoft Office 365 account). This allows
+you to implement the famous `Login with Google/Facebook/Microsoft` buttons
+functionality on your backend very easily. ## Security warning Please note that
+versions preceding `0.7.0` had a security vulnerability. The SSO instance could
+share state between requests, which could lead to security issues. **Please
+update to `0.7.0` or newer**. Also, the preferred way of using the SSO
+instances is to use `with` statement, which will ensure the state is cleared.
+See example below. ## Support this project If you'd like to support this
+project, consider [buying me a coffee â](https://www.buymeacoffee.com/
 tomas.votava). I tend to process Pull Requests faster when properly caffeinated
 ð. [Buy_Me_A_Coffee] ## Supported login providers ### Official - Google -
 Microsoft - Facebook - Spotify - Fitbit - Github (credits to [Brandl](https://
 github.com/Brandl) for hint using `accept` header) - generic (see [docs](https:
 //tomasvotava.github.io/fastapi-sso/sso/generic.html)) ### Contributed - Kakao
 (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor)) - Naver (by
 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92) - Gitlab (by
@@ -32,25 +46,26 @@
 (request) return { "id": user.id, "picture": user.picture, "display_name":
 user.display_name, "email": user.email, "provider": user.provider, } ``` Run
 using `uvicorn example:app`. ### Specify `redirect_uri` on request time In
 scenarios you cannot provide the `redirect_uri` upon the SSO class
 initialization, you may simply omit the parameter and provide it when calling
 `get_login_redirect` method. ```python ... google_sso = GoogleSSO("my-client-
 id", "my-client-secret") @app.get("/google/login") async def google_login
-(request: Request): """Generate login url and redirect""" return await
-google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
-@app.get("/google/callback") async def google_callback(request: Request): ...
-``` ### Specify scope Since `0.4.0` you may specify `scope` when initializing
-the SSO class. ```python from fastapi_sso.sso.microsoft import MicrosoftSSO sso
-= MicrosoftSSO(client_id="client-id", client_secret="client-secret", scope=
-["openid", "email"]) ``` ### Additional query parameters Since `0.4.0` you may
-provide additional query parameters to be sent to the login screen. E.g.
-sometimes you want to specify `access_type=offline` or `prompt=consent` in
-order for Google to return `refresh_token`. ```python async def google_login
-(request: Request): return await google_sso.get_login_redirect
+(request: Request): """Generate login url and redirect""" with google_sso:
+return await google_sso.get_login_redirect(redirect_uri=request.url_for
+("google_callback")) @app.get("/google/callback") async def google_callback
+(request: Request): ... ``` ### Specify scope Since `0.4.0` you may specify
+`scope` when initializing the SSO class. ```python from
+fastapi_sso.sso.microsoft import MicrosoftSSO sso = MicrosoftSSO
+(client_id="client-id", client_secret="client-secret", scope=["openid",
+"email"]) ``` ### Additional query parameters Since `0.4.0` you may provide
+additional query parameters to be sent to the login screen. E.g. sometimes you
+want to specify `access_type=offline` or `prompt=consent` in order for Google
+to return `refresh_token`. ```python async def google_login(request: Request):
+with google_sso: return await google_sso.get_login_redirect
 ( redirect_uri=request.url_for("google_callback"), params={"prompt": "consent",
 "access_type": "offline"} ) ``` ## HTTP and development **You should always use
 `https` in production**. But in case you need to test on `localhost` and do not
 want to use self-signed certificate, make sure you set up redirect uri within
 your SSO provider to `http://localhost:{port}` and then add this to your
 environment: ```bash OAUTHLIB_INSECURE_TRANSPORT=1 ``` And make sure you pass
 `allow_insecure_http = True` to SSO class' constructor, such as: ```python
@@ -59,18 +74,18 @@
 more information. ## State State is useful if you want the server to return
 something back to you to help you understand in what context the authentication
 was initiated. It is mostly used to store the url you want your user to be
 redirected to after successful login. You may use `.state` property to get the
 state returned from the server. Example: ```python from fastapi import Request
 from fastapi.responses import RedirectResponse # E.g. https://example.com/auth/
 login?return_url=https://example.com/welcome async def google_login(return_url:
-str): google_sso = GoogleSOO("client-id", "client-secret") # Send return_url to
-Google as a state so that Google knows to return it back to us return await
-google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"),
-state=return_url) async def google_callback(request: Request): google_sso =
-GoogleSOO("client-id", "client-secret") user = await
-google_sso.verify_and_process(request) # google_sso.state now holds your
-return_url (https://example.com/welcome) return RedirectResponse
+str): with google_sso: google_sso = GoogleSOO("client-id", "client-secret") #
+Send return_url to Google as a state so that Google knows to return it back to
+us return await google_sso.get_login_redirect(redirect_uri=request.url_for
+("google_callback"), state=return_url) async def google_callback(request:
+Request): with google_sso: google_sso = GoogleSOO("client-id", "client-secret")
+user = await google_sso.verify_and_process(request) # google_sso.state now
+holds your return_url (https://example.com/welcome) return RedirectResponse
 (google_sso.state) ``` **Deprecation Warning**: legacy `use_state` argument in
 `SSOBase` constructor is deprecated and will be removed. ## Contributing If
 you'd like to contribute and add your specific login provider, please see
 [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `fastapi_sso-0.7.1/fastapi_sso/__init__.py` & `fastapi_sso-0.7.2/fastapi_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/base.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import RedirectResponse
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
-    from typing_extensions import TypedDict
+    from typing_extensions import TypedDict  # pragma: no cover
 
 DiscoveryDocument = TypedDict(
     "DiscoveryDocument", {"authorization_endpoint": str, "token_endpoint": str, "userinfo_endpoint": str}
 )
 
 
 class UnsetStateWarning(UserWarning):
@@ -101,15 +101,15 @@
             )
         return self._state
 
     @property
     def oauth_client(self) -> WebApplicationClient:
         """OAuth Client to help us generate requests and parse responses"""
         if self.client_id == NotImplemented:
-            raise NotImplementedError(f"Provider {self.provider} not supported")
+            raise NotImplementedError(f"Provider {self.provider} not supported")  # pragma: no cover
         if self._oauth_client is None:
             self._oauth_client = WebApplicationClient(self.client_id)
         return self._oauth_client
 
     @property
     def access_token(self) -> Optional[str]:
         """Access token from token endpoint"""
@@ -239,15 +239,15 @@
         This is low level, you should use {verify_and_process} instead.
 
         Arguments:
             params {Optional[Dict[str, Any]]} -- Optional additional query parameters to pass to the provider
             additional_headers {Optional[Dict[str, Any]]} -- Optional additional headers to be added to all requests
         """
         # pylint: disable=too-many-locals
-        if self._oauth_client is not None:
+        if self._oauth_client is not None:  # pragma: no cover
             self._oauth_client = None
             self._refresh_token = None
             warnings.warn(
                 (
                     "Reusing the SSO object is not safe and caused a security issue in previous versions."
                     "To make sure you don't see this warning, please use the SSO object as a context manager."
                 ),
@@ -269,15 +269,15 @@
             await self.token_endpoint,
             authorization_response=current_url,
             redirect_url=redirect_uri or self.redirect_uri or current_path,
             code=code,
             **params,
         )  # type: ignore
 
-        if token_url is None:
+        if token_url is None:  # pragma: no cover
             return None
 
         headers.update(additional_headers)
 
         auth = httpx.BasicAuth(self.client_id, self.client_secret)
         async with httpx.AsyncClient() as session:
             response = await session.post(token_url, headers=headers, content=body, auth=auth)
```

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/facebook.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/facebook.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/fitbit.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/fitbit.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/generic.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/generic.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/github.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/github.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/gitlab.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/gitlab.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/google.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/google.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/kakao.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/kakao.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/microsoft.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/microsoft.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fastapi_sso.sso.base import DiscoveryDocument, OpenID, SSOBase
 
 
 class MicrosoftSSO(SSOBase):
     """Class providing login using Microsoft OAuth"""
 
     provider = "microsoft"
-    scope = ["openid"]
+    scope = ["openid", "User.Read"]
     version = "v1.0"
     tenant: str = "common"
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
@@ -38,8 +38,15 @@
             "authorization_endpoint": f"https://login.microsoftonline.com/{self.tenant}/oauth2/v2.0/authorize",
             "token_endpoint": f"https://login.microsoftonline.com/{self.tenant}/oauth2/v2.0/token",
             "userinfo_endpoint": f"https://graph.microsoft.com/{self.version}/me",
         }
 
     @classmethod
     async def openid_from_response(cls, response: dict) -> OpenID:
-        return OpenID(email=response["mail"], display_name=response["displayName"], provider=cls.provider)
+        return OpenID(
+            email=response["mail"],
+            display_name=response["displayName"],
+            provider=cls.provider,
+            id=response.get("id"),
+            first_name=response.get("givenName"),
+            last_name=response.get("surname"),
+        )
```

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/naver.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/naver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Naver SSO Oauth Helper class"""
 
 from typing import List
+
 from fastapi_sso.sso.base import DiscoveryDocument, OpenID, SSOBase
 
 
 class NaverSSO(SSOBase):
     """Class providing login using Naver OAuth"""
 
     provider = "naver"
```

### Comparing `fastapi_sso-0.7.1/fastapi_sso/sso/spotify.py` & `fastapi_sso-0.7.2/fastapi_sso/sso/spotify.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class SpotifySSO(SSOBase):
     """Class providing login via Spotify OAuth"""
 
     provider = "spotify"
     scope = ["user-read-private", "user-read-email"]
 
-    # pylint: disable=no-self-use
     async def get_discovery_document(self) -> DiscoveryDocument:
         """Get document containing handy urls"""
         return {
             "authorization_endpoint": "https://accounts.spotify.com/authorize",
             "token_endpoint": "https://accounts.spotify.com/api/token",
             "userinfo_endpoint": "https://api.spotify.com/v1/me",
         }
```

### Comparing `fastapi_sso-0.7.1/PKG-INFO` & `fastapi_sso-0.7.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: fastapi-sso
-Version: 0.7.1
+Version: 0.7.2
 Summary: FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)
 Home-page: https://tomasvotava.github.io/fastapi-sso/
 License: MIT
 Keywords: fastapi,sso,oauth,google,facebook,spotify
 Author: Tomas Votava
 Author-email: info@tomasvotava.eu
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (<1)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: fastapi (>=0.80)
+Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: oauthlib (>=3.1.0)
-Requires-Dist: pydantic (>=1.8.1)
+Requires-Dist: pydantic (>=1.8.0)
 Requires-Dist: starlette (>=0.13.6)
 Project-URL: Documentation, https://tomasvotava.github.io/fastapi-sso/
 Project-URL: Repository, https://github.com/tomasvotava/fastapi-sso
 Description-Content-Type: text/markdown
 
 # FastAPI SSO
 
+![Supported Python Versions](https://img.shields.io/pypi/pyversions/fastapi-sso)
+![Test Coverage](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgist.githubusercontent.com%2Ftomasvotava%2F328acf6207500c2e836b1c68b5c910f7%2Fraw%2F&query=totals.percent_covered_display&suffix=%25&logo=pytest&label=coverage&color=blue&cacheSeconds=300
+)
+![Tests Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/test.yml?label=tests)
+![Pylint Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=pylint)
+![Mypy Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=mypy)
+![Black Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=black)
+![CodeQL Workflow Status](https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/codeql-analysis.yml?label=CodeQL)
+![PyPi weekly downloads](https://img.shields.io/pypi/dw/fastapi-sso)
+![Project License](https://img.shields.io/github/license/tomasvotava/fastapi-sso)
+![PyPi Version](https://img.shields.io/pypi/v/fastapi-sso)
+
 FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 account).
 
 This allows you to implement the famous `Login with Google/Facebook/Microsoft` buttons functionality on your backend very easily.
 
 ## Security warning
 
 Please note that versions preceding `0.7.0` had a security vulnerability.
@@ -129,15 +140,16 @@
 ...
 
 google_sso = GoogleSSO("my-client-id", "my-client-secret")
 
 @app.get("/google/login")
 async def google_login(request: Request):
     """Generate login url and redirect"""
-    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
+    with google_sso:
+        return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
 
 @app.get("/google/callback")
 async def google_callback(request: Request):
     ...
 ```
 
 ### Specify scope
@@ -156,18 +168,19 @@
 sent to the login screen.
 
 E.g. sometimes you want to specify `access_type=offline` or `prompt=consent` in order for
 Google to return `refresh_token`.
 
 ```python
 async def google_login(request: Request):
-    return await google_sso.get_login_redirect(
-        redirect_uri=request.url_for("google_callback"),
-        params={"prompt": "consent", "access_type": "offline"}
-        )
+    with google_sso:
+        return await google_sso.get_login_redirect(
+            redirect_uri=request.url_for("google_callback"),
+            params={"prompt": "consent", "access_type": "offline"}
+            )
 
 ```
 
 ## HTTP and development
 
 **You should always use `https` in production**. But in case you need to test on `localhost` and do not want to
 use self-signed certificate, make sure you set up redirect uri within your SSO provider to `http://localhost:{port}`
@@ -195,23 +208,25 @@
 
 ```python
 from fastapi import Request
 from fastapi.responses import RedirectResponse
 
 # E.g. https://example.com/auth/login?return_url=https://example.com/welcome
 async def google_login(return_url: str):
-    google_sso = GoogleSOO("client-id", "client-secret")
-    # Send return_url to Google as a state so that Google knows to return it back to us
-    return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"), state=return_url)
+    with google_sso:
+        google_sso = GoogleSOO("client-id", "client-secret")
+        # Send return_url to Google as a state so that Google knows to return it back to us
+        return await google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"), state=return_url)
 
 async def google_callback(request: Request):
-    google_sso = GoogleSOO("client-id", "client-secret")
-    user = await google_sso.verify_and_process(request)
-    # google_sso.state now holds your return_url (https://example.com/welcome)
-    return RedirectResponse(google_sso.state)
+    with google_sso:
+        google_sso = GoogleSOO("client-id", "client-secret")
+        user = await google_sso.verify_and_process(request)
+        # google_sso.state now holds your return_url (https://example.com/welcome)
+        return RedirectResponse(google_sso.state)
 
 ```
 
 **Deprecation Warning**: legacy `use_state` argument in `SSOBase` constructor is deprecated and will be removed.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,32 +1,46 @@
-Metadata-Version: 2.1 Name: fastapi-sso Version: 0.7.1 Summary: FastAPI plugin
+Metadata-Version: 2.1 Name: fastapi-sso Version: 0.7.2 Summary: FastAPI plugin
 to enable SSO to most common providers (such as Facebook login, Google login
 and login via Microsoft Office 365 Account) Home-page: https://
 tomasvotava.github.io/fastapi-sso/ License: MIT Keywords:
 fastapi,sso,oauth,google,facebook,spotify Author: Tomas Votava Author-email:
-info@tomasvotava.eu Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
+info@tomasvotava.eu Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: fastapi (<1) Requires-Dist: httpx
-(>=0.23.0,<0.24.0) Requires-Dist: oauthlib (>=3.1.0) Requires-Dist: pydantic
-(>=1.8.1) Requires-Dist: starlette (>=0.13.6) Project-URL: Documentation,
-https://tomasvotava.github.io/fastapi-sso/ Project-URL: Repository, https://
-github.com/tomasvotava/fastapi-sso Description-Content-Type: text/markdown #
-FastAPI SSO FastAPI plugin to enable SSO to most common providers (such as
-Facebook login, Google login and login via Microsoft Office 365 account). This
-allows you to implement the famous `Login with Google/Facebook/Microsoft`
-buttons functionality on your backend very easily. ## Security warning Please
-note that versions preceding `0.7.0` had a security vulnerability. The SSO
-instance could share state between requests, which could lead to security
-issues. **Please update to `0.7.0` or newer**. Also, the preferred way of using
-the SSO instances is to use `with` statement, which will ensure the state is
-cleared. See example below. ## Support this project If you'd like to support
-this project, consider [buying me a coffee â](https://www.buymeacoffee.com/
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fastapi
+(>=0.80) Requires-Dist: httpx (>=0.23.0) Requires-Dist: oauthlib (>=3.1.0)
+Requires-Dist: pydantic (>=1.8.0) Requires-Dist: starlette (>=0.13.6) Project-
+URL: Documentation, https://tomasvotava.github.io/fastapi-sso/ Project-URL:
+Repository, https://github.com/tomasvotava/fastapi-sso Description-Content-
+Type: text/markdown # FastAPI SSO ![Supported Python Versions](https://
+img.shields.io/pypi/pyversions/fastapi-sso) ![Test Coverage](https://
+img.shields.io/badge/dynamic/
+json?url=https%3A%2F%2Fgist.githubusercontent.com%2Ftomasvotava%2F328acf6207500c2e836b1c68b5c910f7%2Fraw%2F&query=totals.percent_covered_display&suffix=%25&logo=pytest&label=coverage&color=blue&cacheSeconds=300
+) ![Tests Workflow Status](https://img.shields.io/github/actions/workflow/
+status/tomasvotava/fastapi-sso/test.yml?label=tests) ![Pylint Workflow Status]
+(https://img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/
+lint.yml?label=pylint) ![Mypy Workflow Status](https://img.shields.io/github/
+actions/workflow/status/tomasvotava/fastapi-sso/lint.yml?label=mypy) ![Black
+Workflow Status](https://img.shields.io/github/actions/workflow/status/
+tomasvotava/fastapi-sso/lint.yml?label=black) ![CodeQL Workflow Status](https:/
+/img.shields.io/github/actions/workflow/status/tomasvotava/fastapi-sso/codeql-
+analysis.yml?label=CodeQL) ![PyPi weekly downloads](https://img.shields.io/
+pypi/dw/fastapi-sso) ![Project License](https://img.shields.io/github/license/
+tomasvotava/fastapi-sso) ![PyPi Version](https://img.shields.io/pypi/v/fastapi-
+sso) FastAPI plugin to enable SSO to most common providers (such as Facebook
+login, Google login and login via Microsoft Office 365 account). This allows
+you to implement the famous `Login with Google/Facebook/Microsoft` buttons
+functionality on your backend very easily. ## Security warning Please note that
+versions preceding `0.7.0` had a security vulnerability. The SSO instance could
+share state between requests, which could lead to security issues. **Please
+update to `0.7.0` or newer**. Also, the preferred way of using the SSO
+instances is to use `with` statement, which will ensure the state is cleared.
+See example below. ## Support this project If you'd like to support this
+project, consider [buying me a coffee â](https://www.buymeacoffee.com/
 tomas.votava). I tend to process Pull Requests faster when properly caffeinated
 ð. [Buy_Me_A_Coffee] ## Supported login providers ### Official - Google -
 Microsoft - Facebook - Spotify - Fitbit - Github (credits to [Brandl](https://
 github.com/Brandl) for hint using `accept` header) - generic (see [docs](https:
 //tomasvotava.github.io/fastapi-sso/sso/generic.html)) ### Contributed - Kakao
 (by Jae-Baek Song - [thdwoqor](https://github.com/thdwoqor)) - Naver (by
 1tang2bang92) - [1tang2bang92](https://github.com/1tang2bang92) - Gitlab (by
@@ -47,25 +61,26 @@
 (request) return { "id": user.id, "picture": user.picture, "display_name":
 user.display_name, "email": user.email, "provider": user.provider, } ``` Run
 using `uvicorn example:app`. ### Specify `redirect_uri` on request time In
 scenarios you cannot provide the `redirect_uri` upon the SSO class
 initialization, you may simply omit the parameter and provide it when calling
 `get_login_redirect` method. ```python ... google_sso = GoogleSSO("my-client-
 id", "my-client-secret") @app.get("/google/login") async def google_login
-(request: Request): """Generate login url and redirect""" return await
-google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"))
-@app.get("/google/callback") async def google_callback(request: Request): ...
-``` ### Specify scope Since `0.4.0` you may specify `scope` when initializing
-the SSO class. ```python from fastapi_sso.sso.microsoft import MicrosoftSSO sso
-= MicrosoftSSO(client_id="client-id", client_secret="client-secret", scope=
-["openid", "email"]) ``` ### Additional query parameters Since `0.4.0` you may
-provide additional query parameters to be sent to the login screen. E.g.
-sometimes you want to specify `access_type=offline` or `prompt=consent` in
-order for Google to return `refresh_token`. ```python async def google_login
-(request: Request): return await google_sso.get_login_redirect
+(request: Request): """Generate login url and redirect""" with google_sso:
+return await google_sso.get_login_redirect(redirect_uri=request.url_for
+("google_callback")) @app.get("/google/callback") async def google_callback
+(request: Request): ... ``` ### Specify scope Since `0.4.0` you may specify
+`scope` when initializing the SSO class. ```python from
+fastapi_sso.sso.microsoft import MicrosoftSSO sso = MicrosoftSSO
+(client_id="client-id", client_secret="client-secret", scope=["openid",
+"email"]) ``` ### Additional query parameters Since `0.4.0` you may provide
+additional query parameters to be sent to the login screen. E.g. sometimes you
+want to specify `access_type=offline` or `prompt=consent` in order for Google
+to return `refresh_token`. ```python async def google_login(request: Request):
+with google_sso: return await google_sso.get_login_redirect
 ( redirect_uri=request.url_for("google_callback"), params={"prompt": "consent",
 "access_type": "offline"} ) ``` ## HTTP and development **You should always use
 `https` in production**. But in case you need to test on `localhost` and do not
 want to use self-signed certificate, make sure you set up redirect uri within
 your SSO provider to `http://localhost:{port}` and then add this to your
 environment: ```bash OAUTHLIB_INSECURE_TRANSPORT=1 ``` And make sure you pass
 `allow_insecure_http = True` to SSO class' constructor, such as: ```python
@@ -74,18 +89,18 @@
 more information. ## State State is useful if you want the server to return
 something back to you to help you understand in what context the authentication
 was initiated. It is mostly used to store the url you want your user to be
 redirected to after successful login. You may use `.state` property to get the
 state returned from the server. Example: ```python from fastapi import Request
 from fastapi.responses import RedirectResponse # E.g. https://example.com/auth/
 login?return_url=https://example.com/welcome async def google_login(return_url:
-str): google_sso = GoogleSOO("client-id", "client-secret") # Send return_url to
-Google as a state so that Google knows to return it back to us return await
-google_sso.get_login_redirect(redirect_uri=request.url_for("google_callback"),
-state=return_url) async def google_callback(request: Request): google_sso =
-GoogleSOO("client-id", "client-secret") user = await
-google_sso.verify_and_process(request) # google_sso.state now holds your
-return_url (https://example.com/welcome) return RedirectResponse
+str): with google_sso: google_sso = GoogleSOO("client-id", "client-secret") #
+Send return_url to Google as a state so that Google knows to return it back to
+us return await google_sso.get_login_redirect(redirect_uri=request.url_for
+("google_callback"), state=return_url) async def google_callback(request:
+Request): with google_sso: google_sso = GoogleSOO("client-id", "client-secret")
+user = await google_sso.verify_and_process(request) # google_sso.state now
+holds your return_url (https://example.com/welcome) return RedirectResponse
 (google_sso.state) ``` **Deprecation Warning**: legacy `use_state` argument in
 `SSOBase` constructor is deprecated and will be removed. ## Contributing If
 you'd like to contribute and add your specific login provider, please see
 [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

