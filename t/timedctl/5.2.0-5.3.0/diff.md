# Comparing `tmp/timedctl-5.2.0.tar.gz` & `tmp/timedctl-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.2.0.tar", max compression
+gzip compressed data, was "timedctl-5.3.0.tar", max compression
```

## Comparing `timedctl-5.2.0.tar` & `timedctl-5.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-08-04 20:22:42.635864 timedctl-5.2.0/LICENSE
--rw-r--r--   0        0        0     1764 2023-08-04 20:22:42.635864 timedctl-5.2.0/README.md
--rw-r--r--   0        0        0      858 2023-08-04 20:23:09.424191 timedctl-5.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-04 20:22:42.635864 timedctl-5.2.0/timedctl/__init__.py
--rw-r--r--   0        0        0     2449 2023-08-04 20:22:42.635864 timedctl-5.2.0/timedctl/helpers.py
--rwxr-xr-x   0        0        0    23463 2023-08-04 20:22:42.635864 timedctl-5.2.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 timedctl-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-08-07 06:42:55.365531 timedctl-5.3.0/LICENSE
+-rw-r--r--   0        0        0     2168 2023-08-07 06:42:55.365531 timedctl-5.3.0/README.md
+-rw-r--r--   0        0        0     1237 2023-08-07 06:43:24.046969 timedctl-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 06:42:55.365531 timedctl-5.3.0/timedctl/__init__.py
+-rw-r--r--   0        0        0     2488 2023-08-07 06:42:55.365531 timedctl-5.3.0/timedctl/helpers.py
+-rwxr-xr-x   0        0        0    23400 2023-08-07 06:42:55.365531 timedctl-5.3.0/timedctl/timedctl.py
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 timedctl-5.3.0/PKG-INFO
```

### Comparing `timedctl-5.2.0/LICENSE` & `timedctl-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.2.0/README.md` & `timedctl-5.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,20 +10,39 @@
 $ yay -S timedctl
 ```
 People on other distributions can use pip to install the package from pypi:
 ```bash
 $ pip install timedctl
 ```
 
+### Shell completion
+`timedctl` support shell completion for the unaliased commands:
+
+**bash**
+```bash
+_TIMEDCTL_COMPLETE=bash_source timedctl >> ~/.bashrc`
+```
+
+**zsh**
+```bash
+_TIMEDCTL_COMPLETE=zsh_source timedctl >> ~/.zshrc`
+```
+
+**fish**
+```bash
+_TIMEDCTL_COMPLETE=fish_source timedctl >  ~/.config/fish/completions/timedctl.fish`
+```
+
 ## Local development
 Clone the repository and install the dependencies with `poetry install`. You can now run the project with `poetry run timedctl`. For building wheels, you can use `poetry build`.
+Run tests with `poetry run pytest --cov --cov-fail-under 100`.
 
 ## Known issues
 * Make sure to have a polkit-agent running, otherwise the poetry installation during the installation on arch might fail.
-* You need a keyring installed in order for timedctl to store the SSO token, for example `gnome-keyring`. 
+* You need a keyring installed in order for timedctl to store the SSO token, for example `gnome-keyring`.
 
 ## Feature roadmap
 - [x] SSO auth
 - [x] Overtime
 - [x] Reports
     - [x] Get
     - [x] Add
```

### Comparing `timedctl-5.2.0/timedctl/helpers.py` & `timedctl-5.3.0/timedctl/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+"""
+API unrelated helper functions.
+"""
+import datetime
 import json
-import rich
 import re
-import pyfzf
-import click
-import datetime
 import sys
 
-"""
-API unrelated helper functions.
-"""
+import click
+import pyfzf
+import rich
 
 
 def msg(message, nonl=False):
     """Print a message in bold green."""
     rich.print(f"[bold green]{message}[/bold green]", end="" if nonl else "\n")
 
 
@@ -66,25 +66,25 @@
     for line in arr[1:]:
         val = line[-1]
         total += val
     # format as HH:MM:SS
     return str(total)
 
 
-def output_formatted(data, format):
+def output_formatted(data, output_format):
     """Output data in a specified format."""
-    match format:
+    match output_format:
         case "json":
-            print(json.dumps(data, indent=4))
+            rich.print(json.dumps(data, indent=4))
         case "csv":
             keys = data[0].keys()
             output = ",".join(keys) + "\n"
             for obj in data:
                 output += ",".join(obj.values()) + "\n"
-            print(output)
+            rich.print(output)
         case "text":
             for obj in data:
                 for key, val in obj.items():
-                    print(f"[{key}]: {val}, ", end="")
-                print("")
+                    rich.print(f"[{key}]: {val}, ", end="")
+                rich.print("")
         case _:
-            print("Invalid format")
+            rich.print("Invalid format")
```

### Comparing `timedctl-5.2.0/timedctl/timedctl.py` & `timedctl-5.3.0/timedctl/timedctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 import datetime
 import os
 import re
 
 import click
 import pyfzf
+import requests
 import terminaltables
 import tomllib
 from click_aliases import ClickAliasedGroup
 from libtimed import TimedAPIClient
 from libtimed.oidc import OIDCClient
 from tomlkit import dump
 
 from timedctl.helpers import (
-    msg,
     error_handler,
     fzf_wrapper,
+    msg,
+    output_formatted,
     time_picker,
     time_sum,
-    output_formatted,
 )
 
 
 def load_config():
     """Load the timedctl config."""
     cfg = {
         "username": "test",
@@ -32,25 +33,26 @@
         "sso_url": "https://sso.example.com",
         "sso_realm": "example",
         "sso_client_id": "timedctl",
     }
 
     # Get the path to the config file based on the $XDG_config_HOME environment variable
     if not os.getenv("HOME"):
-        raise EnvironmentError("$HOME is not set")
+        raise OSError("$HOME is not set")
 
     xdg_config_home = os.getenv(
-        "XDG_CONFIG_HOME", os.path.join(os.getenv("HOME"), ".config")
+        "XDG_CONFIG_HOME",
+        os.path.join(os.getenv("HOME"), ".config"),
     )
     config_dir = os.path.join(xdg_config_home, "timedctl")
     config_file = os.path.join(config_dir, "config.toml")
 
     if not os.path.isfile(config_file):
         os.makedirs(config_dir, exist_ok=True)
-        print("No config file found. Please enter the following infos.")
+        click.echo("No config file found. Please enter the following infos.")
         for key in cfg:
             cfg[key] = input(f"{key} ({cfg[key]}): ")
         with open(config_file, "w", encoding="utf-8") as file:
             dump(cfg, file)
     else:
         with open(config_file, "rb") as file:
             user_config = tomllib.load(file)
@@ -77,242 +79,324 @@
     token = oidc_client.authorize()
     return TimedAPIClient(token, url, api_namespace)
 
 
 def select_report(date):
     """FZF prompt to select a report."""
     reports = timed.reports.get(
-        filters={"date": date}, include="task,task.project,task.project.customer"
+        filters={"date": date},
+        include="task,task.project,task.project.customer",
     )
     report_view = []
     for report in reports:
         task = report["relationships"]["task"]
         report_view.append(
             [
                 task["attributes"]["name"],
                 report["attributes"]["comment"],
                 str(report["attributes"]["duration"]),
                 task["id"],
                 report["id"],
-            ]
+            ],
         )
     # get longest key per value
-    max_key_lengths = [max(map(len, col)) for col in zip(*report_view)]
+    max_key_lengths = [max(map(len, col)) for col in zip(*report_view, strict=False)]
     # pad all the values
     report_view = [
         [
             report_view[i][j].ljust(max_key_lengths[j])
             for j in range(len(report_view[i]))
         ]
         for i in range(len(report_view))
     ]
     # create a list for fzf
     fzf_obj = []
     for row in report_view:
         fzf_obj.append(
-            [" | ".join([row[0], row[1], row[2]]), row[1], row[2], row[3], row[4]]
+            [" | ".join([row[0], row[1], row[2]]), row[1], row[2], row[3], row[4]],
         )
 
     report = fzf_wrapper(fzf_obj, [0], "Select a report: ")
     return report
 
 
 def select_activity(date):
     """FZF prompt to select an activity."""
     activities = timed.activities.get(filters={"date": date})
     activity_view = []
     # loop through all activities
-    for activity in activities:
+    for activity_obj in activities:
         # check if there is an actual task, else use an unknown task
-        task_data = activity["relationships"]["task"]["data"]
+        task_data = activity_obj["relationships"]["task"]["data"]
         if task_data:
             task = timed.tasks.get(id=task_data["id"], cached=True)
         else:
             task = {"attributes": {"name": "Unknown task"}, "id": None}
         activity_view.append(
             [
                 task["attributes"]["name"],
-                activity["attributes"]["comment"],
-                activity["attributes"]["from-time"].strftime("%H:%M:%S")
+                activity_obj["attributes"]["comment"],
+                activity_obj["attributes"]["from-time"].strftime("%H:%M:%S")
                 + " - "
-                + activity["attributes"]["to-time"].strftime("%H:%M:%S"),
+                + activity_obj["attributes"]["to-time"].strftime("%H:%M:%S"),
                 task["id"],
-                activity["id"],
-            ]
+                activity_obj["id"],
+            ],
         )
     # get longest key per value
-    max_key_lengths = [max(map(len, col)) for col in zip(*activity_view)]
+    max_key_lengths = [max(map(len, col)) for col in zip(*activity_view, strict=False)]
     # pad all the values
     activity_view = [
         [
             activity_view[i][j].ljust(max_key_lengths[j])
             for j in range(len(activity_view[i]))
         ]
         for i in range(len(activity_view))
     ]
     # create a list for fzf
     fzf_obj = []
     for row in activity_view:
         fzf_obj.append(
-            [" | ".join([row[0], row[1], row[2]]), row[1], row[2], row[3], row[4]]
+            [" | ".join([row[0], row[1], row[2]]), row[1], row[2], row[3], row[4]],
         )
 
-    activity = fzf_wrapper(fzf_obj, [0], "Select an activity: ")
-    return activity
+    activity_obj = fzf_wrapper(fzf_obj, [0], "Select an activity: ")
+    return activity_obj
 
 
-def format_activity(activity):
+def format_activity(activity_obj):
     """Format an activity for display."""
-    task_obj = activity["relationships"]["task"]
+    task_obj = activity_obj["relationships"]["task"]
 
     task = task_obj["attributes"]["name"]
 
     project_obj = timed.projects.get(
-        id=task_obj["relationships"]["project"]["id"], cached=True
+        id=task_obj["relationships"]["project"]["id"],
+        cached=True,
     )
     project = project_obj["attributes"]["name"]
 
     customer_obj = timed.customers.get(
-        id=project_obj["relationships"]["customer"]["data"]["id"], cached=True
+        id=project_obj["relationships"]["customer"]["data"]["id"],
+        cached=True,
     )
     customer = customer_obj["attributes"]["name"]
     return f"{customer} > {project} > {task}"
 
 
+def get_customer_by_name(customers, name, archived):
+    """Get customer by name."""
+    customers = timed.customers.get(cached=True, filters={"archived": archived})
+    customer = [c for c in customers if c["attributes"]["name"] == name]
+    if len(customer) == 0:
+        error_handler("ERR_CUSTOMER_NOT_FOUND")
+    customer_id = customer[0]["id"]
+    return customer_id
+
+
+def get_project_by_name(projects, name, customer_id, archived):
+    """Get project by name."""
+    projects = timed.projects.get(
+        cached=True,
+        filters={"customer": customer_id, "archived": archived},
+    )
+    project = [c for c in projects if c["attributes"]["name"] == name]
+    if len(project) == 0:
+        error_handler("ERR_PROJECT_NOT_FOUND")
+    project_id = project[0]["id"]
+    return project_id
+
+
+def get_task_by_name(tasks, name, project_id, archived):
+    """Get task by name."""
+    tasks = timed.tasks.get(
+        cached=True,
+        filters={"project": project_id, "archived": archived},
+    )
+    task = [c for c in tasks if c["attributes"]["name"] == name]
+    if len(task) == 0:
+        error_handler("ERR_TASK_NOT_FOUND")
+    task_id = task[0]["id"]
+    return task_id
+
+
+def select_task(customer, project, task, show_archived):
+    """Select a task ID with fzf."""
+    # select a customer
+    customers = timed.customers.get(filters={"archived": show_archived}, cached=True)
+    if customer:
+        customer_id = get_customer_by_name(customers, customer, show_archived)
+    else:
+        customer_id = fzf_wrapper(
+            customers,
+            ["attributes", "name"],
+            "Select a customer: ",
+        )["id"]
+    # get projects
+    projects = timed.projects.get(
+        filters={"customer": customer_id, "archived": show_archived},
+        cached=True,
+    )
+    # select a project
+    if project:
+        project_id = get_project_by_name(projects, project, customer_id, show_archived)
+    else:
+        project_id = fzf_wrapper(
+            projects,
+            ["attributes", "name"],
+            "Select a project: ",
+        )["id"]
+    # get tasks
+    tasks = timed.tasks.get(
+        filters={"project": project_id, "archived": show_archived},
+        cached=True,
+    )
+    # select a task
+    if task:
+        task_id = get_task_by_name(tasks, task, project_id, show_archived)
+    else:
+        task_id = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")["id"]
+    return task_id
+
+
 timed = client_setup()
 
 
 @click.group(cls=ClickAliasedGroup)
 def timedctl():
     """Use timedctl."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["g", "show", "describe"])
 def get():
     """Get different things."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @get.group(cls=ClickAliasedGroup)
 def data():
     """Get raw data for building custom scripts."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @data.command("customers")
-@click.option("--format", default="json", type=click.Choice(["json", "csv", "text"]))
-def get_customers(format):
+@click.option(
+    "--format",
+    "output_format",
+    default="json",
+    type=click.Choice(["json", "csv", "text"]),
+)
+def get_customers(output_format):
     """Get customers."""
     customers = timed.customers.get(cached=True)
-    data = []
+    output = []
     for customer in customers:
-        data.append({"id": customer["id"], "name": customer["attributes"]["name"]})
-    output_formatted(data, format)
+        output.append({"id": customer["id"], "name": customer["attributes"]["name"]})
+    output_formatted(output, output_format)
 
 
 @data.command("projects")
-@click.option("--format", default="json", type=click.Choice(["json", "csv", "text"]))
+@click.option(
+    "--format",
+    "output_format",
+    default="json",
+    type=click.Choice(["json", "csv", "text"]),
+)
 @click.option("--customer-id", default=None, type=int)
 @click.option("--customer-name", default=None, type=str)
-def get_projects(format, customer_id, customer_name):
+@click.option("--archived", default=False, is_flag=True)
+def get_projects(output_format, customer_id, customer_name, archived):
     """Get projects."""
     if not (customer_id or customer_name):
         error_handler("ERR_MISSING_ARGUMENTS")
     # Get customer ID if name is specified
     if not customer_id:
         customers = timed.customers.get(cached=True)
-        customer = [c for c in customers if c["attributes"]["name"] == customer_name]
-        if len(customer) == 0:
-            error_handler("ERR_CUSTOMER_NOT_FOUND")
-        customer_id = customer[0]["id"]
+        customer_id = get_customer_by_name(customers, customer_name, archived)
     projects = timed.projects.get(cached=True, filters={"customer": customer_id})
-    data = []
+    output = []
     for project in projects:
-        data.append({"id": project["id"], "name": project["attributes"]["name"]})
-    output_formatted(data, format)
+        output.append({"id": project["id"], "name": project["attributes"]["name"]})
+    output_formatted(output, output_format)
 
 
 @data.command("tasks")
-@click.option("--format", default="json", type=click.Choice(["json", "csv", "text"]))
+@click.option(
+    "--format",
+    "output_format",
+    default="json",
+    type=click.Choice(["json", "csv", "text"]),
+)
 @click.option("--customer-id", default=None, type=int)
 @click.option("--customer-name", default=None, type=str)
 @click.option("--project-id", default=None, type=int)
 @click.option("--project-name", default=None, type=str)
-def get_tasks(format, customer_id, customer_name, project_id, project_name):
+@click.option("--archived", default=False, is_flag=True)
+def get_tasks(
+    output_format,
+    customer_id,
+    customer_name,
+    project_id,
+    project_name,
+    archived,
+):
     """Get tasks."""
     if project_name and not (customer_id or customer_name):
         error_handler("ERR_CUSTOMER_INFO_MISSING")
     if not (project_id or project_name):
         error_handler("ERR_MISSING_ARGUMENTS")
     # Get project ID if name is specified
     if not project_id:
         # we need an id for the customer
         if not customer_id:
             customers = timed.customers.get(cached=True)
-            customer = [
-                c for c in customers if c["attributes"]["name"] == customer_name
-            ]
-            if len(customer) == 0:
-                error_handler("ERR_CUSTOMER_NOT_FOUND")
-            customer_id = customer[0]["id"]
+            customer_id = get_customer_by_name(customers, customer_name, archived)
         # get the project id
         projects = timed.projects.get(cached=True, filters={"customer": customer_id})
-        project = [c for c in projects if c["attributes"]["name"] == project_name]
-        if len(project) == 0:
-            error_handler("ERR_PROJECT_NOT_FOUND")
-        project_id = project[0]["id"]
+        project_id = get_project_by_name(projects, project_name, customer_id, archived)
     # get the tasks for the specified project
     tasks = timed.tasks.get(cached=True, filters={"project": project_id})
-    data = []
+    output = []
     for task in tasks:
-        data.append({"id": task["id"], "name": task["attributes"]["name"]})
-    output_formatted(data, format)
+        output.append({"id": task["id"], "name": task["attributes"]["name"]})
+    output_formatted(output, output_format)
 
 
 @get.command("overtime", aliases=["t", "ot", "undertime"])
 @click.option("--date", default=None)
 def get_overtime(date):
     """Get overtime of user."""
     user = timed.users.me["id"]
     overtime = timed.overtime.get({"user": user, "date": date})
-    msg(f"Currrent overtime is: {overtime}")
+    msg(f"Current overtime is: {overtime}")
 
 
 @get.command("reports", aliases=["report", "r"])
 @click.option("--date", default=None)
 def get_reports(date):
     """Get reports."""
     reports = timed.reports.get(
-        filters={"date": date}, include="task,task.project,task.project.customer"
+        filters={"date": date},
+        include="task,task.project,task.project.customer",
     )
     table = [["Customer", "Project", "Task", "Comment", "Duration"]]
     for report in reports:
         task_obj = report["relationships"]["task"]
-        task = task_obj["attributes"]["name"]
-
-        project_obj = timed.projects.get(
-            id=task_obj["relationships"]["project"]["id"], cached=True
+        project_obj = task_obj["relationships"]["project"]
+        customer_obj = project_obj["relationships"]["customer"]
+        # get name attributes
+        task, project, customer = (
+            x["attributes"]["name"] for x in [task_obj, project_obj, customer_obj]
         )
-        project = project_obj["attributes"]["name"]
+        comment = report["attributes"]["comment"]
+        duration = report["attributes"]["duration"]
 
-        customer_obj = timed.customers.get(
-            id=project_obj["relationships"]["customer"]["data"]["id"], cached=True
-        )
-        customer = customer_obj["attributes"]["name"]
-
-        table.append(
-            [
-                customer,
-                project,
-                task,
-                report["attributes"]["comment"],
-                report["attributes"]["duration"],
-            ]
-        )
+        table.append([customer, project, task, comment, duration])
+    # create the output
     output = terminaltables.SingleTable(table)
     msg(f"Reports for {date if date is not None else 'today'}:")
     click.echo(output.table)
     msg(f"Total: {time_sum(table)}")
 
 
 @get.command("activities", aliases=["a", "ac", "activity"])
@@ -329,43 +413,45 @@
             [
                 format_activity(activity_obj),
                 activity_obj["attributes"]["comment"],
                 activity_obj["attributes"]["from-time"].strftime("%H:%M:%S"),
                 activity_obj["attributes"]["to-time"].strftime("%H:%M:%S")
                 if activity_obj["attributes"]["to-time"] is not None
                 else "active",
-            ]
+            ],
         )
     output = terminaltables.SingleTable(table)
     msg(f"Activities for {date if date is not None else 'today'}:")
     click.echo(output.table)
 
 
 @get.command("absences", aliases=["abs"])
 def get_absences():
     """Get absences."""
+    error_handler("ERR_NOT_IMPLEMENTED")
 
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["rm", "d", "remove", "del"])
 def delete():
     """Delete different things."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @delete.command("report", aliases=["r"])
 @click.option("--date", default=None)
 def delete_report(date):
     """Delete report(s)."""
     report = select_report(date)
     res = pyfzf.FzfPrompt().prompt(
-        ["Yes", "No"], f"--prompt 'Are you sure? Delete \"{report[1]}\"?'"
+        ["Yes", "No"],
+        f"--prompt 'Are you sure? Delete \"{report[1]}\"?'",
     )
     if res[0] == "Yes":
         req = timed.reports.delete(report[-1])
-        if req.status_code == 204:
+        if req.status_code == requests.codes["no_content"]:
             msg(f'Deleted report "{report[1]}"')
         else:
             error_handler("ERR_DELETION_FAILED")
     else:
         error_handler("ERR_DELETION_ABORTED")
 
 
@@ -380,63 +466,35 @@
     """Delete absence(s)."""
     error_handler("ERR_NOT_IMPLEMENTED")
 
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["a", "create"])
 def add():
     """Add different things."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @add.command("report", aliases=["r"])
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 @click.option("--description", default=None)
 @click.option("--duration", default=None)
 @click.option("--show-archived", default=False, is_flag=True)
 def add_report(
-    customer, project, task, description, duration, show_archived
-):  # pylint: disable=R0912
+    customer,
+    project,
+    task,
+    description,
+    duration,
+    show_archived,
+):  # ruff: noqa: PLR0913
     """Add report(s)."""
-    # ask the user to select a customer
-    msg("Select a customer")
-    # select a customer
-    customers = timed.customers.get(filters={"archived": show_archived}, cached=True)
-    if customer:
-        customer = [c for c in customers if c["attributes"]["name"] == customer]
-        if len(customer) == 0:
-            error_handler("ERR_CUSTOMER_NOT_FOUND")
-        customer = customer[0]
-    else:
-        customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
-    # get projects
-    projects = timed.projects.get(
-        filters={"customer": customer["id"], "archived": show_archived}, cached=True
-    )
-    # select a project
-    if project:
-        project = [p for p in projects if p["attributes"]["name"] == project]
-        if len(project) == 0:
-            error_handler("ERR_PROJECT_NOT_FOUND")
-        project = project[0]
-    else:
-        project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
-    # get tasks
-    tasks = timed.tasks.get(
-        filters={"project": project["id"], "archived": show_archived}, cached=True
-    )
     # select a task
-    if task:
-        task = [t for t in tasks if t["attributes"]["name"] == task]
-        if len(task) == 0:
-            error_handler("ERR_TASK_NOT_FOUND")
-        task = task[0]
-    else:
-        task = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")
+    task_id = select_task(customer, project, task, show_archived)
     # ask the user to enter a description
     if not description:
         msg("Enter a description")
         # get description
         description = click.prompt("")
     # ask the user to enter a duration
     if duration:
@@ -444,18 +502,18 @@
             error_handler("ERR_INVALID_DURATION")
     else:
         duration = time_picker()
     # create the report
     res = timed.reports.post(
         {"duration": duration, "comment": description},
         {
-            "task": task["id"],
+            "task": task_id,
         },
     )
-    if res.status_code == 201:
+    if res.status_code == requests.codes["created"]:
         msg("Report created successfully")
         return
     # handle exception
     error_handler("ERR_REPORT_CREATION_FAILED")
 
 
 @add.command("holiday", aliases=["h"])
@@ -469,32 +527,34 @@
     """Add absence(s)."""
     error_handler("ERR_NOT_IMPLEMENTED")
 
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["e", "edit", "update"])
 def edit():
     """Edit different things."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @edit.command("report", aliases=["r"])
 @click.option("--date", default=None)
 def edit_report(date):
     """Edit report(s)."""
     report = select_report(date)
 
     msg("Comment", True)
     comment = click.prompt("", default=report[1].strip())
     duration = time_picker(default=report[2])
     res = pyfzf.FzfPrompt().prompt(["No", "Yes"], "--prompt 'Are you sure?'")
     if res == ["Yes"]:
         res = timed.reports.patch(
-            report[-1], {"comment": comment, "duration": duration}, {"task": report[-2]}
+            report[-1],
+            {"comment": comment, "duration": duration},
+            {"task": report[-2]},
         )
-        if res.status_code == 200:
+        if res.status_code == requests.codes["ok"]:
             msg("Report updated successfully")
             return
         # handle exception
         error_handler("ERR_REPORT_UPDATE_FAILED")
     else:
         error_handler("ERR_REPORT_UPDATE_ABORTED")
 
@@ -510,66 +570,33 @@
     """Edit absence(s)."""
     error_handler("ERR_NOT_IMPLEMENTED")
 
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["ac"])
 def activity():
     """Do stuff with activities."""
-    pass  # pylint: disable=W0107
+    # pylint: disable=W0107
 
 
 @activity.command("start", aliases=["add", "a"])
 @click.argument("comment")
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 @click.option("--show-archived", default=False, is_flag=True)
 def start_activity(comment, customer, project, task, show_archived):
     """Start recording activity."""
-    customers = timed.customers.get(filters={"archived": show_archived}, cached=True)
-    # ask the user to select a customer
-    msg("Select a customer")
-    # select a customer
-    if customer:
-        customer = [c for c in customers if c["attributes"]["name"] == customer]
-        if len(customer) == 0:
-            error_handler("ERR_CUSTOMER_NOT_FOUND")
-        customer = customer[0]
-    else:
-        customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
-    # get projects
-    projects = timed.projects.get(
-        filters={"customer": customer["id"], "archived": show_archived}, cached=True
-    )
-    # select a project
-    if project:
-        project = [p for p in projects if p["attributes"]["name"] == project]
-        if len(project) == 0:
-            error_handler("ERR_PROJECT_NOT_FOUND")
-        project = project[0]
-    else:
-        project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
-    # get tasks
-    tasks = timed.tasks.get(
-        filters={"project": project["id"], "archived": show_archived}, cached=True
-    )
-    # select a task
-    if task:
-        task = [t for t in tasks if t["attributes"]["name"] == task]
-        if len(task) == 0:
-            error_handler("ERR_TASK_NOT_FOUND")
-        task = task[0]
-    else:
-        task = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")
+    task_id = select_task(customer, project, task, show_archived)
     # create the activity
     res = timed.activities.start(
-        attributes={"comment": comment}, relationships={"task": task["id"]}
+        attributes={"comment": comment},
+        relationships={"task": task_id},
     )
 
-    if res.status_code == 201:
+    if res.status_code == requests.codes["created"]:
         msg(f"Activity {comment} started successfully.")
         return
     # handle exception
     error_handler("ERR_ACTIVITY_START_FAILED")
 
 
 @activity.command("stop", aliases=["end", "finish"])
@@ -582,61 +609,62 @@
     msg("Activity stopped successfully.")
 
 
 @activity.command("show", aliases=["s", "get", "info"])
 @click.option("--short", default=False, is_flag=True)
 def show_activity(short):
     """Show current activity."""
-    # TODO: Fix in libtimed so the full object gets returned
-    current_activity = timed.activities.get(
-        filters={"id": timed.activities.current["id"]},
-        include="task,task.project,task.project.customer",
-    )[0]
-    comment = " > " + current_activity["attributes"]["comment"] if not short else ""
-    start = current_activity["attributes"]["from-time"].strftime("%H:%M:%S")
+    current_activity = timed.activities.current
     if current_activity:
+        activity_obj = timed.activities.get(
+            filters={"id": current_activity["id"]},
+            include="task,task.project,task.project.customer",
+        )[0]
+        comment = " > " + activity_obj["attributes"]["comment"] if not short else ""
+        start = activity_obj["attributes"]["from-time"].strftime("%H:%M:%S")
         msg(
-            f"Current activity: {format_activity(current_activity)}{comment} (Since "
-            + f"{start})"
+            f"Current activity: {format_activity(activity_obj)}{comment} (Since "
+            + f"{start})",
         )
     else:
         error_handler("ERR_NO_CURRENT_ACTIVITY")
 
 
 @activity.command("restart", aliases=["r", "continue", "resume"])
 @click.option("--date", default=None)
 def restart_activity(date):
     """Restart an activity."""
     # stop current activity first
     if timed.activities.current:
         timed.activities.stop()
         msg("Stopped current activity.")
     # select an activity
-    activity = select_activity(date)
+    activity_obj = select_activity(date)
     # grab attributes
-    comment = activity[1]
-    task_id = activity[3]
+    comment = activity_obj[1]
+    task_id = activity_obj[3]
     res = timed.activities.start(
-        attributes={"comment": comment}, relationships={"task": task_id}
+        attributes={"comment": comment},
+        relationships={"task": task_id},
     )
-    if res.status_code == 201:
+    if res.status_code == requests.codes["created"]:
         msg(f'Activity "{comment}" restarted successfully.')
         return
     # handle exception
     error_handler("ERR_ACTIVITY_START_FAILED")
 
 
 @activity.command("delete", aliases=["d", "rm", "remove"])
 @click.option("--date", default=None)
 def delete_activity(date):
     """Delete an activity."""
     # select an activity
-    activity = select_activity(date)
-    if timed.activities.delete(activity[-1]):
-        msg(f"Activity {activity[1]} deleted successfully.")
+    activity_obj = select_activity(date)
+    if timed.activities.delete(activity_obj[-1]):
+        msg(f"Activity {activity_obj[1]} deleted successfully.")
         return
     error_handler("ERR_ACTIVITY_DELETE_FAILED")
 
 
 @activity.command("generate-timesheet", aliases=["gts", "ts"])
 def activity_generate_timesheet():
     """Generate the timesheet of the current activities."""
@@ -661,38 +689,40 @@
                     and x["relationships"]["task"]["data"]["id"] == task
                 ]
                 # if report has been found
                 if len(report) > 0:
                     report = report[0]
                     # deserialize the timedelta
                     hours, minutes, seconds = report["attributes"]["duration"].split(
-                        ":"
+                        ":",
                     )
                     old_duration = datetime.timedelta(
-                        hours=int(hours), minutes=int(minutes), seconds=int(seconds)
+                        hours=int(hours),
+                        minutes=int(minutes),
+                        seconds=int(seconds),
                     )
                     # calculate the new duration
                     report["attributes"]["duration"] = old_duration + duration
                     # update report
                     timed.reports.patch(
                         report["id"],
                         report["attributes"],
                         {"task": task},
                     )
                 else:
                     # create report
-                    r = timed.reports.post(
+                    res = timed.reports.post(
                         {
                             "duration": duration,
                             "comment": attr["comment"],
                         },
                         {"task": task},
                     )
                     # append the report to the known reports
-                    reports.append(r.json()["data"])
+                    reports.append(res.json()["data"])
                 # update activity to be transferred
                 attr["transferred"] = True
                 timed.activities.patch(activity_obj["id"], attr, {"task": task})
         msg("Timesheet generated successfully.")
     else:
         error_handler("ERR_NO_ACTIVITIES")
```

### Comparing `timedctl-5.2.0/PKG-INFO` & `timedctl-5.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.2.0
+Version: 5.3.0
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -31,20 +31,39 @@
 $ yay -S timedctl
 ```
 People on other distributions can use pip to install the package from pypi:
 ```bash
 $ pip install timedctl
 ```
 
+### Shell completion
+`timedctl` support shell completion for the unaliased commands:
+
+**bash**
+```bash
+_TIMEDCTL_COMPLETE=bash_source timedctl >> ~/.bashrc`
+```
+
+**zsh**
+```bash
+_TIMEDCTL_COMPLETE=zsh_source timedctl >> ~/.zshrc`
+```
+
+**fish**
+```bash
+_TIMEDCTL_COMPLETE=fish_source timedctl >  ~/.config/fish/completions/timedctl.fish`
+```
+
 ## Local development
 Clone the repository and install the dependencies with `poetry install`. You can now run the project with `poetry run timedctl`. For building wheels, you can use `poetry build`.
+Run tests with `poetry run pytest --cov --cov-fail-under 100`.
 
 ## Known issues
 * Make sure to have a polkit-agent running, otherwise the poetry installation during the installation on arch might fail.
-* You need a keyring installed in order for timedctl to store the SSO token, for example `gnome-keyring`. 
+* You need a keyring installed in order for timedctl to store the SSO token, for example `gnome-keyring`.
 
 ## Feature roadmap
 - [x] SSO auth
 - [x] Overtime
 - [x] Reports
     - [x] Get
     - [x] Add
```

