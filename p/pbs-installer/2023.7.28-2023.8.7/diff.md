# Comparing `tmp/pbs_installer-2023.7.28.tar.gz` & `tmp/pbs_installer-2023.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_installer-2023.7.28.tar", last modified: Fri Jul 28 14:04:45 2023, max compression
+gzip compressed data, was "pbs_installer-2023.8.7.tar", last modified: Mon Aug  7 09:38:14 2023, max compression
```

## Comparing `pbs_installer-2023.7.28.tar` & `pbs_installer-2023.8.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2023-07-28 14:04:21.863690 pbs_installer-2023.7.28/LICENSE
--rw-r--r--   0        0        0      331 2023-07-28 14:04:21.863690 pbs_installer-2023.7.28/README.md
--rw-r--r--   0        0        0     1034 2023-07-28 14:04:45.436038 pbs_installer-2023.7.28/pyproject.toml
--rw-r--r--   0        0        0      275 2023-07-28 14:04:21.863690 pbs_installer-2023.7.28/src/pbs_installer/__init__.py
--rw-r--r--   0        0        0     2163 2023-07-28 14:04:21.863690 pbs_installer-2023.7.28/src/pbs_installer/__main__.py
--rw-r--r--   0        0        0     4930 2023-07-28 14:04:21.863690 pbs_installer-2023.7.28/src/pbs_installer/_install.py
--rw-r--r--   0        0        0     1613 2023-07-28 14:04:21.867690 pbs_installer-2023.7.28/src/pbs_installer/_utils.py
--rw-r--r--   0        0        0    70281 2023-07-28 14:04:21.867690 pbs_installer-2023.7.28/src/pbs_installer/_versions.py
--rw-r--r--   0        0        0        0 2023-07-28 14:04:21.867690 pbs_installer-2023.7.28/tests/__init__.py
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 pbs_installer-2023.7.28/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-08-07 09:37:45.708566 pbs_installer-2023.8.7/LICENSE
+-rw-r--r--   0        0        0      331 2023-08-07 09:37:45.708566 pbs_installer-2023.8.7/README.md
+-rw-r--r--   0        0        0     1033 2023-08-07 09:38:14.845510 pbs_installer-2023.8.7/pyproject.toml
+-rw-r--r--   0        0        0      275 2023-08-07 09:37:45.708566 pbs_installer-2023.8.7/src/pbs_installer/__init__.py
+-rw-r--r--   0        0        0     2573 2023-08-07 09:37:45.712566 pbs_installer-2023.8.7/src/pbs_installer/__main__.py
+-rw-r--r--   0        0        0     5433 2023-08-07 09:37:45.712566 pbs_installer-2023.8.7/src/pbs_installer/_install.py
+-rw-r--r--   0        0        0     1966 2023-08-07 09:37:45.712566 pbs_installer-2023.8.7/src/pbs_installer/_utils.py
+-rw-r--r--   0        0        0    70281 2023-08-07 09:37:45.712566 pbs_installer-2023.8.7/src/pbs_installer/_versions.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:37:45.712566 pbs_installer-2023.8.7/tests/__init__.py
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 pbs_installer-2023.8.7/PKG-INFO
```

### Comparing `pbs_installer-2023.7.28/LICENSE` & `pbs_installer-2023.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.28/pyproject.toml` & `pbs_installer-2023.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors = [
     { name = "Frost Ming", email = "me@frostming.com" },
 ]
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.md"
 dynamic = []
-version = "2023.7.28"
+version = "2023.8.7"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 download = [
     "requests>=2.24.0",
```

### Comparing `pbs_installer-2023.7.28/src/pbs_installer/__main__.py` & `pbs_installer-2023.8.7/src/pbs_installer/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from argparse import SUPPRESS, Action, ArgumentParser, Namespace
 from collections.abc import Sequence
 from typing import Any
 
 from ._install import install
+from ._utils import get_available_arch_platforms
 
 
 def _setup_logger(verbose: bool):
     logger = logging.getLogger("pbs_installer")
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter("%(levelname)s: %(message)s"))
     logger.addHandler(handler)
@@ -42,27 +43,38 @@
         from ._versions import PYTHON_VERSIONS
 
         for version in PYTHON_VERSIONS:
             print(f"- {version}")
 
 
 def main():
+    archs, platforms = get_available_arch_platforms()
     parser = ArgumentParser("pbs-install", description="Installer for Python Build Standalone")
     install_group = parser.add_argument_group("Install Arguments")
     install_group.add_argument("version", help="The version of Python to install, e.g. 3.8,3.10.4")
     install_group.add_argument(
         "--version-dir", help="Install to a subdirectory named by the version", action="store_true"
     )
     install_group.add_argument(
         "-d", "--destination", help="The directory to install to", required=True
     )
+    install_group.add_argument("--arch", choices=archs, help="Override the architecture to install")
+    install_group.add_argument(
+        "--platform", choices=platforms, help="Override the platform to install"
+    )
     parser.add_argument("-v", "--verbose", help="Enable verbose logging", action="store_true")
     parser.add_argument("-l", "--list", action=ListAction, help="List installable versions")
 
     args = parser.parse_args()
     _setup_logger(args.verbose)
-    install(args.version, args.destination, version_dir=args.version_dir)
+    install(
+        args.version,
+        args.destination,
+        version_dir=args.version_dir,
+        arch=args.arch,
+        platform=args.platform,
+    )
     print("Done!")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pbs_installer-2023.7.28/src/pbs_installer/_install.py` & `pbs_installer-2023.8.7/src/pbs_installer/_install.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,31 +24,40 @@
         return None
     return {
         "X-GitHub-Api-Version": "2022-11-28",
         "Authorization": f"Bearer {TOKEN}",
     }
 
 
-def get_download_link(request: str) -> tuple[PythonVersion, str]:
+def get_download_link(
+    request: str, arch: str | None = None, platform: str | None = None
+) -> tuple[PythonVersion, str]:
     """Get the download URL matching the given requested version.
 
     :param request: The version of Python to install, e.g. 3.8,3.10.4
+    :param arch: The architecture to install, e.g. x86_64, arm64
+    :param platform: The platform to install, e.g. linux, macos
     :return: A tuple of the PythonVersion and the download URL
     """
     from ._versions import PYTHON_VERSIONS
 
+    if arch is None:
+        arch = THIS_ARCH
+    if platform is None:
+        platform = THIS_PLATFORM
+
     for py_ver, urls in PYTHON_VERSIONS.items():
         if not py_ver.matches(request):
             continue
 
-        for arch, platform, url in urls:
+        for iarch, iplatform, url in urls:
             logger.debug(
-                "Checking %s %s with current system %s %s", arch, platform, THIS_ARCH, THIS_PLATFORM
+                "Checking %s %s with requested system %s %s", iarch, iplatform, arch, platform
             )
-            if (arch, platform) == (THIS_ARCH, THIS_PLATFORM):
+            if (iarch, iplatform) == (arch, platform):
                 return py_ver, url
         break
     raise ValueError(f"Could not find a CPython {request!r} matching this system")
 
 
 def _read_sha256(url: str, sess: requests.Session) -> str | None:
     resp = sess.get(url + ".sha256", headers=_get_headers())
@@ -129,23 +138,27 @@
 
 
 def install(
     request: str,
     destination: StrPath,
     version_dir: bool = False,
     session: requests.Session | None = None,
+    arch: str | None = None,
+    platform: str | None = None,
 ) -> None:
     """Download and install the requested python version.
 
     :param request: The version of Python to install, e.g. 3.8,3.10.4
     :param destination: The directory to install to
     :param version_dir: Whether to install to a subdirectory named with the python version
     :param session: A requests session to use for downloading
+    :param arch: The architecture to install, e.g. x86_64, arm64
+    :param platform: The platform to install, e.g. linux, macos
     """
-    ver, url = get_download_link(request)
+    ver, url = get_download_link(request, arch=arch, platform=platform)
     if version_dir:
         destination = os.path.join(destination, str(ver))
     logger.debug("Installing %s to %s", ver, destination)
     os.makedirs(destination, exist_ok=True)
     with tempfile.NamedTemporaryFile() as tf:
         tf.close()
         original_filename = download(url, tf.name, session)
```

### Comparing `pbs_installer-2023.7.28/src/pbs_installer/_utils.py` & `pbs_installer-2023.8.7/src/pbs_installer/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,19 @@
     """Unpack the tarfile to the destination, with the first skip_parts parts of the path removed"""
     for member in tf.getmembers():
         fn = member.name.lstrip("/")
         parts = fn.split("/")
         fn = "/".join(parts[skip_parts:])
         member.name = fn
         tf.extract(member, destination)
+
+
+def get_available_arch_platforms() -> tuple[list[str], list[str]]:
+    from ._versions import PYTHON_VERSIONS
+
+    archs: set[str] = set()
+    platforms: set[str] = set()
+    for items in PYTHON_VERSIONS.values():
+        for item in items:
+            archs.add(item[0])
+            platforms.add(item[1])
+    return sorted(archs), sorted(platforms)
```

### Comparing `pbs_installer-2023.7.28/src/pbs_installer/_versions.py` & `pbs_installer-2023.8.7/src/pbs_installer/_versions.py`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.28/PKG-INFO` & `pbs_installer-2023.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbs-installer
-Version: 2023.7.28
+Version: 2023.8.7
 Summary: Installer for Python Build Standalone
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: download
 Provides-Extra: install
 Provides-Extra: all
```

