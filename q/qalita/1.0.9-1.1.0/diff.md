# Comparing `tmp/qalita-1.0.9.tar.gz` & `tmp/qalita-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.9.tar", max compression
+gzip compressed data, was "qalita-1.1.0.tar", max compression
```

## Comparing `qalita-1.0.9.tar` & `qalita-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    19753 2023-07-16 19:52:17.634353 qalita-1.0.9/LICENSE
--rw-r--r--   0        0        0     1942 2023-07-16 19:52:17.635353 qalita-1.0.9/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-16 19:52:28.934563 qalita-1.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 19:52:17.657353 qalita-1.0.9/qalita/__init__.py
--rw-r--r--   0        0        0     4189 2023-07-16 19:52:28.936563 qalita-1.0.9/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-16 19:52:17.657353 qalita-1.0.9/qalita/commands/__init__.py
--rw-r--r--   0        0        0    19666 2023-07-16 19:52:17.635353 qalita-1.0.9/qalita/commands/agent.py
--rw-r--r--   0        0        0    14531 2023-07-16 19:52:17.635353 qalita-1.0.9/qalita/commands/pack.py
--rw-r--r--   0        0        0     9756 2023-07-16 19:52:17.635353 qalita-1.0.9/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-16 19:52:17.657353 qalita-1.0.9/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-16 19:52:17.636353 qalita-1.0.9/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-16 19:52:17.636353 qalita-1.0.9/qalita/internal/utils.py
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-08-07 16:45:46.837922 qalita-1.1.0/LICENSE
+-rw-r--r--   0        0        0    11857 2023-08-07 16:45:46.837922 qalita-1.1.0/docs/README.md
+-rw-r--r--   0        0        0     1197 2023-08-07 16:46:01.125987 qalita-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 16:45:46.897922 qalita-1.1.0/qalita/__init__.py
+-rw-r--r--   0        0        0     3932 2023-08-07 16:45:46.837922 qalita-1.1.0/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-08-07 16:45:46.897922 qalita-1.1.0/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    27109 2023-08-07 16:45:46.841922 qalita-1.1.0/qalita/commands/agent.py
+-rw-r--r--   0        0        0    15468 2023-08-07 16:45:46.841922 qalita-1.1.0/qalita/commands/pack.py
+-rw-r--r--   0        0        0    14776 2023-08-07 16:45:46.841922 qalita-1.1.0/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-08-07 16:45:46.897922 qalita-1.1.0/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-08-07 16:45:46.841922 qalita-1.1.0/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2460 2023-08-07 16:45:46.841922 qalita-1.1.0/qalita/internal/request.py
+-rw-r--r--   0        0        0      173 2023-08-07 16:46:01.129987 qalita-1.1.0/qalita/internal/utils.py
+-rw-r--r--   0        0        0      143 2023-08-07 16:45:46.841922 qalita-1.1.0/qalita/main.py
+-rw-r--r--   0        0        0    12943 1970-01-01 00:00:00.000000 qalita-1.1.0/PKG-INFO
```

### Comparing `qalita-1.0.9/LICENSE` & `qalita-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.9/pyproject.toml` & `qalita-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.9"
+version = "1.1.0"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -17,28 +17,29 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Quality Assurance"
 ]
 include = ["version.json"]
 
 
 [tool.poetry.scripts]
-qalita = "qalita.cli:cli"
+qalita = "qalita.main:cli"
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
+flake8 = ">=3.8.1,<4.0"
 pylint = "^2.17.4"
 black = "^23.3.0"
 pre-commit = "^3.3.3"
 pytest = "^7.4.0"
 
 [tool.poetry.dependencies]
 loguru = "^0.7.0"
 python = "^3.8"
 click = "^8.1.3"
 requests = "^2.31.0"
-pyyaml = "^6.0"
+pyyaml = "^6.0.1"
 toml = "^0.10.2"
 tabulate = "^0.9.0"
+semver = "^3.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qalita-1.0.9/qalita/cli.py` & `qalita-1.1.0/qalita/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 """
 # QALITA (c) COPYRIGHT 2023 - ALL RIGHTS RESERVED -
 """
 import sys
-import os
 import json
 import base64
 import yaml
 import click
 
-from qalita.internal.logger import init_logging
-
-logger = init_logging()
-
-
-class CustomContext(click.Context):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.help_option_names = ["-h", "--help"]
+from qalita.internal.utils import logger, get_version
 
 
 # Config to pass to the commands
 class Config(object):
     agent_data_file_name = ".agent"
 
     def save_source_config(self):
@@ -29,15 +20,17 @@
 
     def load_source_config(self):
         try:
             with open("qalita-conf.yaml", "r") as file:
                 self.config = yaml.safe_load(file)
                 return self.config
         except FileNotFoundError:
-            logger.warning("Configuration file [qalita-conf.yaml] not found, creating a new one.")
+            logger.warning(
+                "Configuration file [qalita-conf.yaml] not found, creating a new one."
+            )
             self.config = {"version": 1, "sources": []}
             self.save_source_config()
             return self.config
         except Exception as e:
             logger.warning(
                 f"An unexpected error occurred while loading the configuration: {e}"
             )
@@ -102,24 +95,22 @@
     Please, Help us improve our service by reporting any bug by filing a bug report, Thanks ! \n\r
     mail : contact-project+qalita-platform-toolset-cli-bug@incoming.gitlab.com \n\r
     ----------------------------------------------------------------------------"""
     pass
 
 
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
-@pass_config
-def version(config):
+def version():
     """
     Display the version of the cli
     """
-    logger.info("------------- QALITA CLI Version -------------")
-    logger.info(f"Version : 1.0.9")
+    print("--- QALITA CLI Version ---")
+    print(f"Version : {get_version()}")
 
-from qalita.commands import agent, source, pack
 
-# Add pack command group to cli
-cli.add_command(pack.pack)
-cli.add_command(agent.agent)
-cli.add_command(source.source)
+def add_commands_to_cli():
+    from qalita.commands import agent, source, pack
 
-if __name__ == "__main__":
-    cli(context_class=CustomContext, auto_envvar_prefix="QALITA")
+    # Add pack command group to cli
+    cli.add_command(pack.pack)
+    cli.add_command(agent.agent)
+    cli.add_command(source.source)
```

### Comparing `qalita-1.0.9/qalita/commands/pack.py` & `qalita-1.1.0/qalita/commands/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,91 @@
 import json
 import tarfile
 import os
 import sys
 import subprocess
 import yaml
 import select
-from qalita.cli import pass_config, logger
-from qalita.internal.utils import send_request
+import logging
 from tabulate import tabulate
 
+from qalita.cli import pass_config
+from qalita.internal.utils import logger
+from qalita.internal.request import send_request
+
 
 def make_tarfile(output_filename, source_dir):
     with tarfile.open(output_filename, "w:gz") as tar:
         tar.add(source_dir, arcname=os.path.basename(source_dir))
 
 
+def run_pack(pack_file_path):
+    logger = logging.getLogger(__name__)
+    logger.setLevel(logging.INFO)
+
+    # create a file handler
+    handler = logging.FileHandler(os.path.join(pack_file_path, "logs.txt"))
+    handler.setLevel(logging.INFO)
+
+    # create a logging format
+    formatter = logging.Formatter(
+        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
+    handler.setFormatter(formatter)
+
+    # add the handlers to the logger
+    logger.addHandler(handler)
+
+    # create a stdout handler
+    stdout_handler = logging.StreamHandler()
+    stdout_handler.setLevel(logging.INFO)
+    stdout_handler.setFormatter(formatter)
+
+    # add the stdout handler to the logger
+    logger.addHandler(stdout_handler)
+
+    logger.info("------------- Pack Run -------------")
+    # Check if the run.sh file exists
+    run_script = "run.sh"  # Only the script name is needed now
+    if not os.path.isfile(os.path.join(pack_file_path, run_script)):
+        logger.error(
+            f"run.sh script does not exist in the package folder {pack_file_path}"
+        )
+        return 1
+
+    # Run the run.sh script and get the output
+    process = subprocess.Popen(
+        ["sh", run_script],
+        cwd=pack_file_path,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        bufsize=1,
+        universal_newlines=True,
+    )
+
+    while process.poll() is None:
+        reads = [process.stdout.fileno(), process.stderr.fileno()]
+        ret = select.select(reads, [], [])
+
+        for fd in ret[0]:
+            if fd == process.stdout.fileno():
+                read = process.stdout.readline().strip()
+                if read:  # Only print if there's output
+                    logger.info(read)
+            if fd == process.stderr.fileno():
+                read = process.stderr.readline().strip()
+                if read:  # Only print if there's output
+                    logger.error(read)
+
+    process.stdout.close()
+    process.stderr.close()
+    logger.info("Pack run completed")
+    return 0
+
+
 def check_name(name):
     all_check_pass = True
     if not name:
         logger.error("Error: Pack name is required!")
         logger.info("\tTo do so, you can set an Environment Variable : ")
         logger.info("\t\texport QALITA_PACK_NAME='mypack'")
         logger.info("\tor add the name as a commandline argument : ")
@@ -33,63 +100,53 @@
         logger.info("\t\tQALITA_PACK_NAME=mypack")
         logger.info("\tand source it : ")
         logger.info("\t\texport $(xargs < .env-local)")
         all_check_pass = False
     if all_check_pass:
         return name
     else:
-        return False
+        sys.exit(1)
 
 
 @click.group()
 @click.option("-p", "--pack", type=int, help="Pack ID")
 @click.pass_context
 def pack(ctx, pack):
     """Manage Qalita Platform Packs"""
     ctx.ensure_object(dict)
     ctx.obj["PACK"] = pack
 
 
 @pack.command()
-@click.pass_context
-def versions(ctx):
-    """Print the versions of the pack"""
-    pack = ctx.obj.get("PACK")
-    logger.info("------------- Pack Versions -------------")
-    logger.info(f"Fetching versions for pack [{pack}]")
-    logger.warning("Not Yet Implemented")
-
-
-@pack.command()
 @pass_config
 def list(config):
     """List all available packs"""
     tab_packs = []
     agent_conf = config.load_agent_config()
-    headers = ["ID", "Name", "Type", "Description"]
-    # TODO : Fetch pack list from local repository
+    headers = ["ID", "Name", "Description"]
 
     r = send_request(
         request=f"{agent_conf['context']['local']['url']}/registries/{agent_conf['registries']['id']}/packs",
         mode="get",
     )
     if r.status_code == 200:
         packs = r.json()
         for pack in packs:
             tab_packs.append(
                 [
                     pack.get("id", ""),
                     pack.get("name", ""),
-                    pack.get("type", ""),
                     pack.get("description", ""),
                 ]
             )
 
     else:
-        logger.error(f"Error cannot fetch pack list, make sure you are logged in with > qalita agent login : {r.status_code} - {r.reason}")
+        logger.error(
+            f"Error cannot fetch pack list, make sure you are logged in with > qalita agent login : {r.status_code} - {r.reason}"
+        )
         return
 
     print(tabulate(tab_packs, headers, tablefmt="simple"))
 
 
 @pass_config
 def validate_pack(config, name):
@@ -137,16 +194,15 @@
     "-n",
     "--name",
     help="The name of the package, it will be used to identify the package in the Qalita platform",
     envvar="QALITA_PACK_NAME",
 )
 @pass_config
 def validate(config, name):
-    # Validation of required options
-
+    """validates pack arborescence, configurations etc...."""
     validate_pack(name)
 
 
 @pack.command()
 @click.option(
     "-n",
     "--name",
@@ -157,20 +213,22 @@
 def push(config, name):
     """Pushes a package to the Qalita Platform"""
 
     agent_conf = config.load_agent_config()
 
     # Validation of required options
     name = check_name(name)
-    if name:
+    if name is not False:
         config.name = name
 
     error_count = validate_pack(name)
     if error_count > 0:
-        logger.error(">> There are errors with your pack, please resolve them before pushing it.")
+        logger.error(
+            ">> There are errors with your pack, please resolve them before pushing it."
+        )
         return
 
     logger.info("------------- Pack Push -------------")
 
     # Create tar.gz archive of directory
     output_filename = f"{name}.tar.gz"
     source_dir = (
@@ -226,16 +284,15 @@
 @click.option(
     "-n",
     "--name",
     help="The name of the package, it will be used to identify the package in the Qalita platform",
     envvar="QALITA_PACK_NAME",
 )
 def run(name):
-    """validates pack arborescence, configurations etc...."""
-    logger.info("------------- Pack Run -------------")
+    """Dry run a pack"""
     # Validation of required options
     all_check_pass = True
     if not name:
         logger.error("Error: Pack name is required!")
         logger.info("\tTo do so, you can set an Environment Variable : ")
         logger.info("\t\texport QALITA_PACK_NAME='mypack'")
         logger.info("\tor add the name as a commandline argument : ")
@@ -260,52 +317,32 @@
     run_script = "run.sh"  # Only the script name is needed now
     if not os.path.isfile(os.path.join(pack_folder, run_script)):
         logger.error(
             f"run.sh script does not exist in the package folder {pack_folder}"
         )
         return
 
-    # Run the run.sh script and get the output
-    process = subprocess.Popen(
-        ["sh", run_script],
-        cwd=pack_folder,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        bufsize=1,
-        universal_newlines=True,
-    )
-
-    while process.poll() is None:
-        reads = [process.stdout.fileno(), process.stderr.fileno()]
-        ret = select.select(reads, [], [])
+    status = run_pack(pack_folder)
 
-        for fd in ret[0]:
-            if fd == process.stdout.fileno():
-                read = process.stdout.readline().strip()
-                if read:  # Only print if there's output
-                    logger.info(read)
-            if fd == process.stderr.fileno():
-                read = process.stderr.readline().strip()
-                if read:  # Only print if there's output
-                    logger.error(read)
-
-    process.stdout.close()
-    process.stderr.close()
-    logger.success("Pack tested")
+    if status == 0:
+        logger.success("Pack Run Success")
+    else:
+        logger.error("Pack Run Failed")
 
 
 @pack.command()
 @click.option(
     "-n",
     "--name",
     help="The name of the package, it will be used to identify the package in the Qalita platform",
     envvar="QALITA_PACK_NAME",
 )
 @pass_config
 def init(config, name):
+    """Initialize a pack"""
     # Validation of required options
     all_check_pass = True
     if not name:
         logger.error("Error: Pack name is required!")
         logger.info("\tTo do so, you can set an Environment Variable : ")
         logger.info("\t\texport QALITA_PACK_NAME='mypack'")
         logger.info("\tor add the name as a commandline argument : ")
```

### Comparing `qalita-1.0.9/qalita/commands/source.py` & `qalita-1.1.0/qalita/commands/source.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 """
 # QALITA (c) COPYRIGHT 2023 - ALL RIGHTS RESERVED -
 """
 import os
 import click
 from tabulate import tabulate
-from qalita.cli import pass_config, logger
-from qalita.internal.utils import send_api_request
+
+from qalita.cli import pass_config
+from qalita.internal.utils import logger
+from qalita.internal.request import send_api_request
 
 
 @click.group()
 @click.option("-s", "--source", type=int, help="Source ID")
 @click.pass_context
 def source(ctx, source):
     """Manage Qalita Platform Sources"""
     ctx.ensure_object(dict)
     ctx.obj["SOURCE"] = source
 
 
 @source.command()
-@click.pass_context
-def versions(ctx):
-    """Print the versions of the source"""
-    source = ctx.obj.get("SOURCE")
-    logger.info("------------- Source Versions -------------")
-    logger.info(f"Fetching versions for source [{source}]")
-    logger.warning("Not Yet Implemented")
-
-
-@source.command()
 @pass_config
 def list(config):
     """List sources that are accessible to the agent"""
     config.load_source_config()
 
     sources = []
-    headers = ["ID", "Name", "Type", "Version" ,"Reference", "Sensitive", "Visibility" ,"Description", "Validity"]
+    headers = [
+        "ID",
+        "Name",
+        "Type",
+        "Reference",
+        "Sensitive",
+        "Visibility",
+        "Description",
+        "Validity",
+    ]
 
     for source in config.config["sources"]:
         sources.append(
             [
                 source.get("id", ""),
                 source.get("name", ""),
                 source.get("type", ""),
-                source.get("version", ""),
                 source.get("reference", ""),
                 source.get("sensitive", ""),
                 source.get("visibility", ""),
                 source.get("description", ""),
                 source.get("validate", ""),
             ]
         )
 
     print(tabulate(sources, headers, tablefmt="simple"))
 
 
+def source_version(source):
+    """Determine the source version"""
+    # La version de la source est déterminée en fonction de sa typologie,
+    # Si la source est d'une version non gérée, elle aura la version 1.0.0
+
+    version = "1.0.0"
+    return version
+
+
 @pass_config
 def validate_source(config):
     """Validate a source configuration"""
     logger.info("------------- Source Validation -------------")
     config.load_source_config()
     agent_conf = config.load_agent_config()
 
@@ -70,36 +79,66 @@
         total_sources += 1
         is_source_valid = True  # Assuming the source is valid initially
 
         # check for name
         if "name" not in source:
             logger.error(f"Source number [{total_sources}] has no name")
             is_source_valid = False
+            return 1
+
+        # check for type
+        if "type" not in source:
+            logger.error(f"Source number [{total_sources}] has no type")
+            is_source_valid = False
+            return 1
+
+        # Check for duplicate names
+        if source["name"] in source_names:
+            logger.error(f"Duplicate source name: [{source['name']}]")
+            is_source_valid = False
         else:
-            # Check for duplicate names
-            if source["name"] in source_names:
-                logger.error(f"Duplicate source name: [{source['name']}]")
-                is_source_valid = False
-            else:
-                source_names.append(source["name"])
+            source_names.append(source["name"])
 
-            # check for description
-            if "description" not in source:
-                logger.warning(f"Source [{source['name']}] has no description")
-                is_source_valid = False
+        # check for description
+        if "description" not in source:
+            logger.warning(
+                f"Source [{source['name']}] has no description, defaulting to empty string"
+            )
+            config.config["sources"][i]["description"] = ""
 
-            # check for owner
-            if "owner" not in source:
-                logger.warning(
-                    f"Source [{source['name']}] must have a owner, if you publish without owner, it will be published under your name"
-                )
-                logger.warning(
-                    f"Source defaulting to owner: {agent_conf['user']['login']}"
-                )
-                source["owner"] = agent_conf["user"]["login"]
+        # check for reference
+        if "reference" not in source:
+            logger.warning(
+                f"Source [{source['name']}] has no reference status, defaulting to False"
+            )
+            config.config["sources"][i]["reference"] = False
+
+        # check for Sensitive
+        if "sensitive" not in source:
+            logger.warning(
+                f"Source [{source['name']}] has no sensitive status, defaulting to False"
+            )
+            config.config["sources"][i]["sensitive"] = False
+
+        # check for visibility
+        if "visibility" not in source:
+            logger.warning(
+                f"Source [{source['name']}] has no visibility status, defaulting to private"
+            )
+            config.config["sources"][i]["visibility"] = "private"
+
+        # check for owner
+        if "owner" not in source:
+            logger.warning(
+                f"Source [{source['name']}] must have a owner, if you publish without owner, it will be published under your name"
+            )
+            logger.warning(
+                f"Source [{source['name']}] defaulting to owner: {agent_conf['user']['login']}"
+            )
+            source["owner"] = agent_conf["user"]["login"]
 
         # check type
         if source["type"] == "database":
             if "config" in source:
                 for key, value in source["config"].items():
                     # If the value starts with '$', assume it's an environment variable
                     if str(value).startswith("$"):
@@ -108,28 +147,35 @@
                         env_value = os.getenv(env_var)
                         if env_value is None:
                             logger.warning(
                                 f"The environment variable [{env_var}] for the source [{source['name']}] is not set"
                             )
                             is_source_valid = False
         elif source["type"] == "file":
-            # check for path in config
-            if "path" not in source["config"]:
-                logger.error(
-                    f"Source [{source['name']}] is of type file but has no path in config"
-                )
-                is_source_valid = False
-
-            # check for read access to path
-            path = source["config"]["path"]
-            if not os.access(path, os.R_OK):
+            # check if config parameter is present
+            if "config" not in source:
                 logger.error(
-                    f"Source [{source['name']}] has a path in config, but it cannot be accessed"
+                    f"Source [{source['name']}] is of type file but has no config"
                 )
                 is_source_valid = False
+            else:
+                # check for path in config
+                if "path" not in source["config"]:
+                    logger.error(
+                        f"Source [{source['name']}] is of type file but has no path in config"
+                    )
+                    is_source_valid = False
+                else:
+                    # check for read access to path
+                    path = source["config"]["path"]
+                    if not os.access(path, os.R_OK):
+                        logger.error(
+                            f"Source [{source['name']}] has a path in config, but it cannot be accessed"
+                        )
+                        is_source_valid = False
 
         # If all checks pass, mark the source as valid
         if is_source_valid:
             source["validate"] = "valid"
             logger.success(f"Source [{source['name']}] validated")
         else:
             source["validate"] = "invalid"
@@ -158,59 +204,82 @@
     validate_source()
     logger.info("------------- Source Publishing -------------")
     logger.info("Publishing sources to the Qalita Platform...")
     invalid_count = 0  # to count failed publishing sources
     agent_conf = config.load_agent_config()
     config.load_source_config()
 
+    if len(config.config["sources"]) == 0:
+        logger.warning("No sources to publish, add new sources > qalita source add")
+        return
+
+    valid_source = 0
+    # count number of valid sources
+    for source in config.config["sources"]:
+        if source["validate"] == "valid":
+            valid_source += 1
+
+    if valid_source == 0:
+        logger.warning("No valid sources to publish")
+        return
+
     for i, source in enumerate(config.config["sources"]):
         if source["validate"] == "valid":
             owner_id = agent_conf["user"]["id"]
             if "id" in source:
                 # Try to get source info from name, type and owner_id
                 r = send_api_request(
                     request="/sources/",
                     mode="get",
                     query_params={
                         "name": source["name"],
                         "type": source["type"],
                         "user_id": agent_conf["user"]["id"],
                     },
                 )
-                if r.status_code != 200:
-                    logger.warning(
-                        f"Agent failed to get source info {r.status_code} - {r.text}"
-                    )
-                    invalid_count += 1
-                else:
+                if r.status_code == 200:
                     # On essaye de matcher les valeurs
                     response_data = r.json()
 
                     # Check if name, type and user_id match with the response data
                     if (
                         source["name"] == response_data["name"]
                         and source["type"] == response_data["type"]
                         and owner_id == response_data["user_id"]
                     ):
                         # If they match, this source is already published, skip to the next source
-
+                        update_source = False
                         if source["description"] == response_data["description"]:
-                            logger.info(
-                                f"Source [{source['name']}] already published with id [{source['id']}] and no updates detected. Skipping..."
-                            )
+                            if response_data["versions"] != []:
+                                if (
+                                    source_version(source)
+                                    == response_data["versions"][0]["sem_ver_id"]
+                                ):
+                                    logger.info(
+                                        f"Source [{source['name']}] already published with id [{source['id']}] and no updates detected. Skipping..."
+                                    )
+                                else:
+                                    logger.info("Version mismatch")
+                                    update_source = True
+                            else:
+                                logger.info("No version")
+                                update_source = True
                         else:
+                            logger.info("Description mismatch")
+                            update_source = True
+
+                        if update_source:
                             r = send_api_request(
                                 request=f"/sources/{response_data['id']}",
                                 mode="put",
                                 query_params={"description": source["description"]},
                             )
-                        continue
-                    else:
-                        # If they don't match, continue with the publishing process
-                        pass
+                            continue
+                        else:
+                            continue
 
             logger.info(f"Publishing source [{source['name']}] ...")
             # test if the owner is the same as the agent user
             if source["owner"] != agent_conf["user"]["login"]:
                 # if the owner is different, we need to fetch the owner-id
                 # from the Qalita Platform
                 r = send_api_request(
@@ -229,16 +298,20 @@
             r = send_api_request(
                 request=f"/sources/publish",
                 mode="post",
                 query_params={
                     "name": source["name"],
                     "type": source["type"],
                     "description": source["description"],
+                    "reference": source["reference"],
+                    "sensitive": source["sensitive"],
+                    "visibility": source["visibility"],
                     "agent_id": agent_conf["context"]["remote"]["id"],
                     "user_id": owner_id,
+                    "version": source_version(source),
                 },
             )
             if r.status_code != 200:
                 logger.warning(
                     f"Agent failed to publish source [{source['name']}] {r.status_code} - {r.text}"
                 )
                 invalid_count += 1
@@ -249,7 +322,78 @@
                 config.config["sources"][i]["id"] = source_id
                 # Save the updated configuration
                 config.save_source_config()
 
     # after all sources have been processed, print a warning if there were any invalid sources
     if invalid_count > 0:
         logger.warning(f"{invalid_count} source(s) skipped due to validation errors.")
+
+
+@source.command()
+@pass_config
+def add(config):
+    """Add a source to the local Qalita Config"""
+
+    # initialize the source dict
+    source = {}
+
+    # hardcode empty source config
+    source["config"] = {}
+
+    # ask for the source name
+    source["name"] = click.prompt("Source name")
+
+    # ask for the source type
+    source["type"] = click.prompt(
+        "Source type",
+        type=click.Choice(["file", "database", "image", "..."], case_sensitive=False),
+    )
+
+    # if the source type is file, ask for the file path
+    if source["type"] == "file":
+        source["config"]["path"] = click.prompt("Source path")
+    elif source["type"] == "database":
+        source['config']['host'] = click.prompt('Source host')
+        source['config']['port'] = click.prompt('Source port')
+        source['config']['username'] = click.prompt('Source username')
+        source['config']['password'] = click.prompt('Source password')
+        source['config']['database'] = click.prompt('Source database')
+
+    # ask for the source description
+    source["description"] = click.prompt("Source description")
+    # ask for the source reference
+    source["reference"] = click.prompt("Source reference", type=bool, default=False)
+    # ask for the source sensitive
+    source["sensitive"] = click.prompt("Source sensitive", type=bool, default=False)
+    # ask for the source visibility
+    source["visibility"] = click.prompt(
+        "Source visibility",
+        default="private",
+        type=click.Choice(["private", "internal", "public"], case_sensitive=False),
+    )
+
+    config.load_source_config()
+    if len(config.config["sources"]) > 0:
+        # check if the source already exists
+        for conf_source in config.config["sources"]:
+            if conf_source["name"] == source["name"]:
+                logger.error("Source already exists in config")
+                return
+
+    # add the source to the config
+    config.config["sources"].append(
+        {
+            "name": source["name"],
+            "config": source["config"],
+            "type": source["type"],
+            "description": source["description"],
+            "reference": source["reference"],
+            "sensitive": source["sensitive"],
+            "visibility": source["visibility"],
+        }
+    )
+
+    # save the config
+    config.save_source_config()
+    logger.success(f"Source [{source['name']}] added to the local config")
+
+    validate_source()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qalita-1.0.9/qalita/internal/logger.py` & `qalita-1.1.0/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.9/qalita/internal/utils.py` & `qalita-1.1.0/qalita/internal/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-"""
-# QALITA (c) COPYRIGHT 2023 - ALL RIGHTS RESERVED -
-"""
-from qalita.cli import pass_config, logger
-import requests
 import time
 import sys
+import requests
+
+from qalita.cli import pass_config
+from qalita.internal.utils import logger
 
 
 @pass_config
 def send_api_request(
     config,
     request,
     mode,
```

