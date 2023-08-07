# Comparing `tmp/clean_workspace-0.4.0.tar.gz` & `tmp/clean_workspace-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_workspace-0.4.0.tar", max compression
+gzip compressed data, was "clean_workspace-0.4.1.tar", max compression
```

## Comparing `clean_workspace-0.4.0.tar` & `clean_workspace-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-08-03 13:12:49.214667 clean_workspace-0.4.0/LICENSE
--rw-r--r--   0        0        0     2696 2023-08-03 13:12:49.215162 clean_workspace-0.4.0/README.md
--rw-r--r--   0        0        0     9216 2023-08-03 13:12:49.216200 clean_workspace-0.4.0/clean_workspace/__init__.py
--rw-r--r--   0        0        0      903 2023-08-03 13:14:37.853568 clean_workspace-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 clean_workspace-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-07 14:48:27.189588 clean_workspace-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2832 2023-08-07 14:48:27.189902 clean_workspace-0.4.1/README.md
+-rw-r--r--   0        0        0     9658 2023-08-07 14:48:27.190748 clean_workspace-0.4.1/clean_workspace/__init__.py
+-rw-r--r--   0        0        0      776 2023-08-07 14:49:57.241735 clean_workspace-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 clean_workspace-0.4.1/PKG-INFO
```

### Comparing `clean_workspace-0.4.0/LICENSE` & `clean_workspace-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_workspace-0.4.0/README.md` & `clean_workspace-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 ❯ clean-workspace --help
 Usage: clean-workspace [OPTIONS]
 
 Options:
   --blacklist-domains PATH
   --blacklist-urls PATH
   --tab-description TEXT    Description for tab
+  --todoist-label TEXT      label in todoist for all created tasks
+  --todoist-project TEXT    project in todoist for all created tasks
   --help                    Show this message and exit.
 ```
 
 ### Regex Entries
 
 You can use regex matches in both the url and domain blacklist files. For example, if you want to blacklist all Zoom domains, you can use the following:
```

### Comparing `clean_workspace-0.4.0/clean_workspace/__init__.py` & `clean_workspace-0.4.1/clean_workspace/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,50 @@
+import datetime
 import os
 import plistlib
 import re
 import sys
 import typing as t
 
 import chrome_bookmarks
 import click
 from ScriptingBridge import SBApplication
+from todoist_api_python.api import TodoistAPI
 
 
 def todoist_client():
     # extract todoist api key from environment without throwing an exception
     todoist_api_key = os.environ.get("TODOIST_API_KEY", None)
 
     if not todoist_api_key:
         print("todoist api key not found in environment")
         return
 
     print("todoist api key found, adding to todoist")
 
-    from todoist_api_python.api import TodoistAPI
-
     api = TodoistAPI(todoist_api_key)
     return api
 
 
-def export_to_todoist(task_content, description):
-    # TODO should also support .env here as well
-    import dotenv
-
-    dotenv.load_dotenv(".envrc")
-
+def export_to_todoist(task_content, description, todoist_project, todoist_label):
     api = todoist_client()
     if not api:
         return
 
-    import datetime
+    project_name = todoist_project
 
-    project_name = os.environ.get("TODOIST_PROJECT", "Learning")
     project = None
     projects = api.get_projects()
     project_matches = [project for project in projects if project.name == project_name]
 
     if len(project_matches) == 1:
         project = project_matches[0]
 
-    # find a label called "web-archive" or create it
-    label_name = os.environ.get("TODOIST_LABEL", "web-archive")
+    # find or create the label
+    label_name = todoist_label
     labels = api.get_labels()
     label_matches = [label for label in labels if label.name == label_name]
 
     # assigning label for debugging
     if len(label_matches) == 0:
         # https://developer.todoist.com/rest/v1/#create-a-new-label
         print(f"could not find {label_name} label, creating it")
@@ -114,35 +108,46 @@
         ]
 
         raw_bookmark_urls.extend(raw_safari_bookmark_urls)
 
     return [bookmark.split("#")[0] for bookmark in raw_bookmark_urls]
 
 
+# TODO trunk ignore should be cleaner
 def quit_browsers():
+    # trunk-ignore-begin(bandit)
     os.system("osascript -e 'quit app \"Safari\"'")
     os.system("osascript -e 'quit app \"Chrome\"'")
-
+    # trunk-ignore-end(bandit)
 
 # the syntax we use is starting and ending with `/`, like sed
 def _is_regex_entry(entry: str):
     return entry.startswith("/") and entry.endswith("/")
 
+
 # assume `regex_blacklist` contains the raw regex strings (starting & ending with /)
 def _in_regex_blacklist(regex_blacklist, url):
     for regex in regex_blacklist:
         if re.search(regex[1:-1], url):
             return True
 
     return False
 
+
 def _extract_host(url):
     return url.split("/")[2]
 
-def clean_workspace(tab_description, blacklist_domains_file_path, blacklist_urls_file_path):
+
+def clean_workspace(
+    tab_description,
+    blacklist_domains_file_path,
+    blacklist_urls_file_path,
+    todoist_project,
+    todoist_label,
+):
     browser_urls = get_browser_urls()
 
     # if page is blank, there is no url or string does not contain http
     browser_urls = [x for x in browser_urls if x[0] is not None and "http" in x[0]]
 
     # remove duplicates
     browser_urls = list(set(browser_urls))
@@ -176,42 +181,42 @@
         # filter out all regex entries
         domain_blacklist = [
             domain for domain in domain_blacklist if not _is_regex_entry(domain)
         ]
 
         # add a `www.` prefix to each domain in the blacklist and merge it with the existing list
         domain_blacklist = domain_blacklist + [
-            "www." + domain for domain in domain_blacklist if not _is_regex_entry(domain)
+            "www." + domain
+            for domain in domain_blacklist
+            if not _is_regex_entry(domain)
         ]
 
     bookmark_urls = get_bookmarks_urls()
 
     # TODO output skipped domains if verbose flag is set
 
     browser_urls = [
         x for x in browser_urls if _extract_host(x[0]) not in domain_blacklist
     ]
 
     browser_urls = [
-        x for x in browser_urls if not _in_regex_blacklist(domain_regex_blacklist, _extract_host(x[0]))
+        x
+        for x in browser_urls
+        if not _in_regex_blacklist(domain_regex_blacklist, _extract_host(x[0]))
     ]
 
-    browser_urls = [
-        x for x in browser_urls if x[0] not in url_blacklist
-    ]
+    browser_urls = [x for x in browser_urls if x[0] not in url_blacklist]
 
     # regex url blacklist is separate from the url blacklist
     browser_urls = [
         x for x in browser_urls if not _in_regex_blacklist(url_regex_blacklist, x[0])
     ]
 
     # if the url is in the bookmark list of chrome or safari, skip it
-    browser_urls = [
-        x for x in browser_urls if x[0] not in bookmark_urls
-    ]
+    browser_urls = [x for x in browser_urls if x[0] not in bookmark_urls]
 
     # join url and name with "-" and print to stdout
     todoist_content = ""
     for url_with_name in browser_urls:
         if (
             url_with_name[0] not in bookmark_urls
             # TODO should allow for regex in the URL matching, or at least globbing
@@ -228,23 +233,35 @@
         sys.exit()
 
     print(f"\n{todoist_content}\n")
 
     # since we've archived all content we can now close out Safari & Chrome
     quit_browsers()
 
-    export_to_todoist(todoist_content, tab_description)
-
+    export_to_todoist(todoist_content, tab_description, todoist_project, todoist_label)
 
 
+# TODO why isn't the default displayed with help?
 @click.command()
 @click.option("--blacklist-domains", type=click.Path(), default=None)
 @click.option("--blacklist-urls", type=click.Path(), default=None)
 @click.option("--tab-description", default="", help="Description for tab")
-def main(tab_description, blacklist_domains, blacklist_urls):
+@click.option(
+    "--todoist-label",
+    default="web-archive",
+    help="label in todoist for all created tasks",
+)
+@click.option(
+    "--todoist-project",
+    default="Learning",
+    help="project in todoist for all created tasks",
+)
+def main(
+    tab_description, blacklist_domains, blacklist_urls, todoist_label, todoist_project
+):
     if not is_internet_connected():
         print("internet is not connected")
         return
 
     home_dir = os.path.expanduser("~")
 
     if blacklist_domains is None:
@@ -264,15 +281,21 @@
 
         blacklist_urls = (
             default_urls_path
             if os.path.exists(default_urls_path)
             else "blacklist_urls.txt"
         )
 
-    clean_workspace(tab_description, blacklist_domains, blacklist_urls)
+    clean_workspace(
+        tab_description,
+        blacklist_domains,
+        blacklist_urls,
+        todoist_project,
+        todoist_label,
+    )
 
 
 def archive_old_tasks():
     # find all old tasks (>1mo) and archive them
     # optionally only do this when there is not a custom name in the title
     pass
```

### Comparing `clean_workspace-0.4.0/pyproject.toml` & `clean_workspace-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 [tool.poetry]
 name = "clean-workspace"
-version = "0.4.0"
+version = "0.4.1"
 description = "Collect all browser URLs, output to terminal, and archive to todoist. Useful for cleaning up your workspace at the end of the day, without loosing important urls."
 authors = ["Mike Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iloveitaly/clean-workspace"
 keywords = ["todoist", "browser", "productivity"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyobjc-framework-ScriptingBridge = "^9.0.1"
 todoist-api-python = "^2.0.1"
-python-dotenv = "^1.0.0"
 chrome-bookmarks = "^2020.10.25"
 click = "^8.1.4"
 
-[tool.poetry.group.dev.dependencies]
-ipython = "^8.14.0"
-ipython-autoimport = "^0.4"
-pdbr = "^0.8.2"
-
 [tool.poetry.scripts]
 clean-workspace = "clean_workspace:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `clean_workspace-0.4.0/PKG-INFO` & `clean_workspace-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: clean-workspace
-Version: 0.4.0
+Version: 0.4.1
 Summary: Collect all browser URLs, output to terminal, and archive to todoist. Useful for cleaning up your workspace at the end of the day, without loosing important urls.
 Home-page: https://github.com/iloveitaly/clean-workspace
 License: MIT
 Keywords: todoist,browser,productivity
 Author: Mike Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chrome-bookmarks (>=2020.10.25,<2021.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: pyobjc-framework-ScriptingBridge (>=9.0.1,<10.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: todoist-api-python (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Clean Workspace: Archive Web Browser Tabs
 
 I've been experimenting with how to make my mornings more productive. One glitch I've found in my mind is I can easily
 get distracted by open tabs on my browser, especially if I'm trying to write or read something which I want to give
@@ -53,14 +52,16 @@
 ❯ clean-workspace --help
 Usage: clean-workspace [OPTIONS]
 
 Options:
   --blacklist-domains PATH
   --blacklist-urls PATH
   --tab-description TEXT    Description for tab
+  --todoist-label TEXT      label in todoist for all created tasks
+  --todoist-project TEXT    project in todoist for all created tasks
   --help                    Show this message and exit.
 ```
 
 ### Regex Entries
 
 You can use regex matches in both the url and domain blacklist files. For example, if you want to blacklist all Zoom domains, you can use the following:
```

