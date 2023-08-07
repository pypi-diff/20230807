# Comparing `tmp/ailess-0.1.2.tar.gz` & `tmp/ailess-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailess-0.1.2.tar", last modified: Wed Jul 26 16:15:11 2023, max compression
+gzip compressed data, was "ailess-0.1.3.tar", last modified: Mon Aug  7 17:05:14 2023, max compression
```

## Comparing `ailess-0.1.2.tar` & `ailess-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 16:15:11.820880 ailess-0.1.2/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1069 2023-07-26 07:24:16.000000 ailess-0.1.2/LICENSE
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      110 2023-07-23 00:16:09.000000 ailess-0.1.2/MANIFEST.in
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5686 2023-07-26 16:15:11.820770 ailess-0.1.2/PKG-INFO
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5573 2023-07-26 16:14:56.000000 ailess-0.1.2/README.md
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 16:15:11.819445 ailess-0.1.2/ailess/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6148 2023-07-26 16:14:56.000000 ailess-0.1.2/ailess/.DS_Store
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       82 2023-07-02 00:10:23.000000 ailess-0.1.2/ailess/__init__.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      127 2023-07-02 00:10:23.000000 ailess-0.1.2/ailess/__main__.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)        0 2023-06-22 22:45:27.000000 ailess-0.1.2/ailess/ailess.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     2915 2023-07-23 00:16:05.000000 ailess-0.1.2/ailess/cli.py
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 16:15:11.819280 ailess-0.1.2/ailess/modules/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6649 2023-07-02 09:06:38.000000 ailess-0.1.2/ailess/modules/aws_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     3648 2023-07-23 00:16:09.000000 ailess-0.1.2/ailess/modules/cli_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      508 2023-07-02 00:10:23.000000 ailess-0.1.2/ailess/modules/config_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5506 2023-07-25 14:22:52.000000 ailess-0.1.2/ailess/modules/docker_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      627 2023-07-02 00:10:23.000000 ailess-0.1.2/ailess/modules/env_utils.py
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1400 2023-07-26 16:14:56.000000 ailess-0.1.2/ailess/modules/python_utils.py
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 16:15:11.820495 ailess-0.1.2/ailess/modules/terraform/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     8995 2023-07-26 16:14:56.000000 ailess-0.1.2/ailess/modules/terraform/cluster.tf
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       52 2023-07-23 00:16:09.000000 ailess-0.1.2/ailess/modules/terraform/iam_policy.json
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     4342 2023-07-23 00:16:09.000000 ailess-0.1.2/ailess/modules/terraform_utils.py
-drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-07-26 16:15:11.820164 ailess-0.1.2/ailess.egg-info/
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5686 2023-07-26 16:15:11.000000 ailess-0.1.2/ailess.egg-info/PKG-INFO
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      911 2023-07-26 16:15:11.000000 ailess-0.1.2/ailess.egg-info/SOURCES.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)        1 2023-07-26 16:15:11.000000 ailess-0.1.2/ailess.egg-info/dependency_links.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       42 2023-07-26 16:15:11.000000 ailess-0.1.2/ailess.egg-info/entry_points.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       75 2023-07-26 16:15:11.000000 ailess-0.1.2/ailess.egg-info/requires.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)        7 2023-07-26 16:15:11.000000 ailess-0.1.2/ailess.egg-info/top_level.txt
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)      297 2023-07-26 16:15:04.000000 ailess-0.1.2/pyproject.toml
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       38 2023-07-26 16:15:11.820912 ailess-0.1.2/setup.cfg
--rw-r--r--   0 arsenyyankovski   (501) staff       (20)       69 2023-07-02 09:06:38.000000 ailess-0.1.2/setup.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-08-07 17:05:14.869688 ailess-0.1.3/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1069 2023-07-26 07:24:16.000000 ailess-0.1.3/LICENSE
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      110 2023-07-23 00:16:09.000000 ailess-0.1.3/MANIFEST.in
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5699 2023-08-07 17:05:14.869578 ailess-0.1.3/PKG-INFO
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5573 2023-07-26 16:14:56.000000 ailess-0.1.3/README.md
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-08-07 17:05:14.867616 ailess-0.1.3/ailess/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6148 2023-07-28 15:28:16.000000 ailess-0.1.3/ailess/.DS_Store
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       82 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/__init__.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      127 2023-07-02 00:10:23.000000 ailess-0.1.3/ailess/__main__.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)        0 2023-06-22 22:45:27.000000 ailess-0.1.3/ailess/ailess.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     2717 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/cli.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-08-07 17:05:14.867397 ailess-0.1.3/ailess/modules/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     6933 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/aws_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     3177 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/cli_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      508 2023-07-02 00:10:23.000000 ailess-0.1.3/ailess/modules/config_utils.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-08-07 17:05:14.869093 ailess-0.1.3/ailess/modules/docker_searchers/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      430 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/docker_searchers/__init__.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      211 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/docker_searchers/python_basic.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1244 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/docker_searchers/pytorch_amd64_nvidia.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1302 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/docker_searchers/tensorflow_amd64_nvidia.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5038 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/docker_utils.py
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5113 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/python_utils.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-08-07 17:05:14.869289 ailess-0.1.3/ailess/modules/terraform/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     9146 2023-08-07 17:04:26.000000 ailess-0.1.3/ailess/modules/terraform/cluster.tf
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       52 2023-07-23 00:16:09.000000 ailess-0.1.3/ailess/modules/terraform/iam_policy.json
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     4342 2023-07-23 00:16:09.000000 ailess-0.1.3/ailess/modules/terraform_utils.py
+drwxr-xr-x   0 arsenyyankovski   (501) staff       (20)        0 2023-08-07 17:05:14.868487 ailess-0.1.3/ailess.egg-info/
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     5699 2023-08-07 17:05:14.000000 ailess-0.1.3/ailess.egg-info/PKG-INFO
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)     1060 2023-08-07 17:05:14.000000 ailess-0.1.3/ailess.egg-info/SOURCES.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)        1 2023-08-07 17:05:14.000000 ailess-0.1.3/ailess.egg-info/dependency_links.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       42 2023-08-07 17:05:14.000000 ailess-0.1.3/ailess.egg-info/entry_points.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       75 2023-08-07 17:05:14.000000 ailess-0.1.3/ailess.egg-info/requires.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)        7 2023-08-07 17:05:14.000000 ailess-0.1.3/ailess.egg-info/top_level.txt
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)      324 2023-08-07 17:04:26.000000 ailess-0.1.3/pyproject.toml
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       38 2023-08-07 17:05:14.869734 ailess-0.1.3/setup.cfg
+-rw-r--r--   0 arsenyyankovski   (501) staff       (20)       69 2023-07-02 09:06:38.000000 ailess-0.1.3/setup.py
```

### Comparing `ailess-0.1.2/LICENSE` & `ailess-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ailess-0.1.2/PKG-INFO` & `ailess-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: ailess
-Version: 0.1.2
+Version: 0.1.3
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ailess - Easily deploy your machine learning models as endpoints on AWS
 
 Ailess is a Python package that allows you to easily deploy your machine learning models and turn them into an endpoint on AWS.
```

### Comparing `ailess-0.1.2/README.md` & `ailess-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ailess-0.1.2/ailess/.DS_Store` & `ailess-0.1.3/ailess/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 000002b0: 636f 6d70 0000 0000 0000 3000 0000 0007  comp......0.....
 000002c0: 006d 006f 0064 0075 006c 0065 0073 6c67  .m.o.d.u.l.e.slg
 000002d0: 3153 636f 6d70 0000 0000 0001 2de9 0000  1Scomp......-...
 000002e0: 0007 006d 006f 0064 0075 006c 0065 0073  ...m.o.d.u.l.e.s
 000002f0: 6d6f 4444 626c 6f62 0000 0008 0688 0100  moDDblob........
 00000300: bf38 c541 0000 0007 006d 006f 0064 0075  .8.A.....m.o.d.u
 00000310: 006c 0065 0073 6d6f 6444 626c 6f62 0000  .l.e.smodDblob..
-00000320: 0008 7feb fc98 8338 c541 0000 0007 006d  .......8.A.....m
+00000320: 0008 0688 0100 bf38 c541 0000 0007 006d  .......8.A.....m
 00000330: 006f 0064 0075 006c 0065 0073 7068 3153  .o.d.u.l.e.sph1S
 00000340: 636f 6d70 0000 0000 0001 d000 0000 0000  comp............
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `ailess-0.1.2/ailess/cli.py` & `ailess-0.1.3/ailess/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from typing import Optional
 
 import typer
 
 from ailess import __app_name__, __version__
 from ailess.modules.aws_utils import push_docker_image, print_endpoint_info, ecs_deploy, wait_for_deployment
-from ailess.modules.cli_utils import config_prompt, define_cuda_version
+from ailess.modules.cli_utils import config_prompt
 from ailess.modules.config_utils import save_config, load_config
 from ailess.modules.docker_utils import (
     generate_or_update_docker_ignore,
     generate_dockerfile,
     build_docker_image,
     generate_docker_compose_file,
 )
@@ -30,20 +30,15 @@
 @app.command()
 def init() -> None:
     """Initialize the project"""
     config = config_prompt()
     print("✔    Config saved to .ailess/config.json")
     ensure_requirements_exists()
     print("✔    requirements.txt")
-    if config["has_gpu"]:
-        config.update({"cuda_version": define_cuda_version()})
-        save_config(config)
-    else:
-        config.update({"cuda_version": None})
-        save_config(config)
+    save_config(config)
     generate_or_update_docker_ignore()
     print("✔    .dockerignore")
     generate_dockerfile(config)
     print("✔    Dockerfile")
     generate_docker_compose_file(config)
     print("✔    docker-compose.yml")
     generate_tfvars_file(config)
```

### Comparing `ailess-0.1.2/ailess/modules/aws_utils.py` & `ailess-0.1.3/ailess/modules/aws_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,27 +54,31 @@
 
 
 def get_instance_type_info(instance_type: str, region: str):
     response = boto3.client("ec2", region_name=region).describe_instance_types(
         DryRun=False,
         InstanceTypes=[instance_type],
     )
-
     if len(response["InstanceTypes"]) == 0:
         print(f"ERROR: {instance_type} is not a valid instance type in {region}")
         exit(1)
 
     arch = DOCKER_ARCHITECTURE_AMD64
 
     if "arm64" in response["InstanceTypes"][0]["ProcessorInfo"]["SupportedArchitectures"]:
         arch = DOCKER_ARCHITECTURE_ARM64
+    if len(response["InstanceTypes"][0].get("GpuInfo", {}).get("Gpus", []))>0:
+        gpu_manufacturer = response["InstanceTypes"][0].get("GpuInfo", {}).get("Gpus", [])[0].get("Manufacturer", {})
+    else:
+        gpu_manufacturer = None
 
     return {
         "memory_size": response["InstanceTypes"][0]["MemoryInfo"]["SizeInMiB"],
         "cpu_size": response["InstanceTypes"][0]["VCpuInfo"]["DefaultVCpus"] * 1024,
+        "gpu_manufacturer": gpu_manufacturer,
         "num_gpus": len(response["InstanceTypes"][0].get("GpuInfo", {}).get("Gpus", [])),
         "cpu_architecture": arch,
     }
 
 
 def get_aws_account_id():
     return boto3.client("sts").get_caller_identity().get("Account")
```

### Comparing `ailess-0.1.2/ailess/modules/cli_utils.py` & `ailess-0.1.3/ailess/modules/cli_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         inquirer.List(
             "aws_region",
             message="Choose an AWS region to deploy to",
             choices=get_regions(),
         ),
         inquirer.Text("host_port", message="What port is your app running on?", default=5000),
         inquirer.Text(
-            "instances_count", message="How many servers in the cluster do you want to run?", default=2
+            "instances_count", message="How many servers in the cluster do you want to run?", default=1
         ),
         inquirer.List(
             "ec2_instance_type",
             message="Choose an EC2 instance (server) type",
             choices=get_predefined_instances(),
         ),
     ]
@@ -49,40 +49,19 @@
     )
 
     answers["entrypoint_path"] = entrypoint_answers["entrypoint_path"]
 
     instance_data = get_instance_type_info(answers["ec2_instance_type"], answers["aws_region"])
     answers["cpu_architecture"] = instance_data["cpu_architecture"]
     answers["has_gpu"] = instance_data["num_gpus"] > 0
+    answers["gpu_manufacturer"] = instance_data["gpu_manufacturer"]
 
     return answers
 
 
-def cuda_version_prompt():
-    questions = [
-        inquirer.Text(
-            "cuda_version",
-            message="You selected a GPU instance. Please enter an NVIDIA CUDA version to use",
-            default="12.1",
-        ),
-    ]
-    answers = inquirer.prompt(questions)
-    return answers["cuda_version"]
-
-
-def define_cuda_version():
-    from ailess.modules.env_utils import get_cuda_version
-
-    cuda_version = get_cuda_version()
-    if cuda_version is None:
-        cuda_version = cuda_version_prompt()
-
-    return cuda_version
-
-
 def run_command_in_working_directory(command, spinner, cwd=os.getcwd(), join_stdout_stderr=False):
     try:
         if join_stdout_stderr:
             completed_process = subprocess.run(
                 command, shell=True, stdout=sys.stdout, stderr=subprocess.STDOUT, cwd=cwd
             )
         else:
```

### Comparing `ailess-0.1.2/ailess/modules/docker_utils.py` & `ailess-0.1.3/ailess/modules/docker_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,60 +4,50 @@
 import subprocess
 import sys
 import urllib.request
 
 from yaspin import yaspin
 
 from ailess.modules.cli_utils import run_command_in_working_directory
+from ailess.modules.python_utils import RequirementsParser
+from ailess.modules.docker_searchers import get_sercher_from_config
 
 DOCKER_ARCHITECTURE_AMD64 = "linux/amd64"
 DOCKER_ARCHITECTURE_ARM64 = "linux/arm64"
 
 
-def get_image_name_from_config(config):
-    cuda_version = config["cuda_version"]
-    if cuda_version is None:
-        return "python:3.9"
-    else:
-        response = urllib.request.urlopen(
-            f"https://hub.docker.com/v2/repositories/nvidia/cuda/tags/?name={cuda_version}&page_size=100"
-        )
-        image_names = list(map(lambda result: result["name"], json.load(response)["results"]))
-        pattern = r"^(\d+\.\d+)(\.\d+)?-runtime-ubuntu(\d+\.\d+)$"
-        filtered_images = [image for image in image_names if re.match(pattern, image)]
-        sorted_images = sorted(
-            filtered_images, key=lambda x: x.split("-")[0] + x.split("-")[-1], reverse=True
-        )
-        if len(sorted_images) == 0:
-            print(f"Could not find a suitable docker image for cuda version {cuda_version}")
-            exit(1)
-        latest_image = sorted_images[0]
-        return f"nvidia/cuda:{latest_image}"
-
-
 def generate_dockerfile(config):
     if os.path.exists(os.path.join(os.getcwd(), "Dockerfile")):
         return
+
+    # Get image name from config
+    requirements = RequirementsParser("requirements.txt")
+    searcher = get_sercher_from_config(config, requirements)
+    image_name = searcher.get_image_name(config, requirements)
+    image_extras = searcher.get_image_extras()
+    
     dockerfile_content = []
-    dockerfile_content.append("FROM {}".format(get_image_name_from_config(config)))
-    if config["cuda_version"] is not None:
+    dockerfile_content.append("FROM {}".format(image_name))
+    if config["has_gpu"]:
         dockerfile_content.append(
-            """
+"""
 ENV DEBIAN_FRONTEND=noninteractive
 
 RUN apt update && \
     apt install -y bash \
                    build-essential \
                    curl \
                    ca-certificates \
                    python3 \
                    python3-pip \
 """
         )
 
+    dockerfile_content.append(image_extras)
+    dockerfile_content.append("RUN apt-get update && apt-get install libgl1 -y")
     dockerfile_content.append("ADD requirements.txt /app/requirements.txt")
     dockerfile_content.append("WORKDIR /app")
     dockerfile_content.append("RUN pip3 install -r requirements.txt")
     dockerfile_content.append("ADD . /app")
     dockerfile_content.append('CMD ["python3", "-u", "{}"]'.format(config["entrypoint_path"]))
     with open("Dockerfile", "w") as dockerfile:
         dockerfile.write("\n".join(dockerfile_content))
@@ -73,31 +63,31 @@
   {}:
     environment:
       - PYTHONUNBUFFERED=1
     image: {}:latest
     build: .
     platform: {}
     ports:
-      - "{}:{}"  
+      - "{}:{}"
     """.format(
         convert_to_alphanumeric(config["project_name"]),
         convert_to_alphanumeric(config["project_name"]),
         config["cpu_architecture"],
         config["host_port"],
         config["host_port"],
     )
 
     if config["has_gpu"]:
-        docker_compose_content += """    
+        docker_compose_content += """
     deploy:
       resources:
         reservations:
           devices:
             - driver: nvidia
-              capabilities: [gpu]  
+              capabilities: [gpu]
 """
     with open("docker-compose.yml", "w") as dockerfile:
         dockerfile.write(docker_compose_content)
 
 
 def generate_or_update_docker_ignore():
     if os.path.exists(".dockerignore"):
```

### Comparing `ailess-0.1.2/ailess/modules/terraform/cluster.tf` & `ailess-0.1.3/ailess/modules/terraform/cluster.tf`

 * *Files 2% similar despite different names*

```diff
@@ -305,14 +305,21 @@
   user_data = local.base64_user_data
   lifecycle {
     create_before_destroy = true
   }
   iam_instance_profile {
     name = aws_iam_instance_profile.ecs_agent.name
   }
+  block_device_mappings {
+    device_name = tolist(data.aws_ami.ecs.block_device_mappings)[0].device_name
+
+    ebs {
+      volume_size = 100
+    }
+  }
 }
 
 resource "aws_ecs_capacity_provider" "capacity_provider" {
   name = "${var.project_name}-cluster-capacity-provider"
 
   auto_scaling_group_provider {
     auto_scaling_group_arn         = aws_autoscaling_group.cluster_asg.arn
```

### Comparing `ailess-0.1.2/ailess/modules/terraform_utils.py` & `ailess-0.1.3/ailess/modules/terraform_utils.py`

 * *Files identical despite different names*

### Comparing `ailess-0.1.2/ailess.egg-info/PKG-INFO` & `ailess-0.1.3/ailess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: ailess
-Version: 0.1.2
+Version: 0.1.3
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ailess - Easily deploy your machine learning models as endpoints on AWS
 
 Ailess is a Python package that allows you to easily deploy your machine learning models and turn them into an endpoint on AWS.
```

### Comparing `ailess-0.1.2/ailess.egg-info/SOURCES.txt` & `ailess-0.1.3/ailess.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 ./ailess/__main__.py
 ./ailess/ailess.py
 ./ailess/cli.py
 ./ailess/modules/aws_utils.py
 ./ailess/modules/cli_utils.py
 ./ailess/modules/config_utils.py
 ./ailess/modules/docker_utils.py
-./ailess/modules/env_utils.py
 ./ailess/modules/python_utils.py
 ./ailess/modules/terraform_utils.py
 ailess/.DS_Store
 ailess/__init__.py
 ailess/__main__.py
 ailess/ailess.py
 ailess/cli.py
@@ -25,12 +24,15 @@
 ailess.egg-info/entry_points.txt
 ailess.egg-info/requires.txt
 ailess.egg-info/top_level.txt
 ailess/modules/aws_utils.py
 ailess/modules/cli_utils.py
 ailess/modules/config_utils.py
 ailess/modules/docker_utils.py
-ailess/modules/env_utils.py
 ailess/modules/python_utils.py
 ailess/modules/terraform_utils.py
+ailess/modules/docker_searchers/__init__.py
+ailess/modules/docker_searchers/python_basic.py
+ailess/modules/docker_searchers/pytorch_amd64_nvidia.py
+ailess/modules/docker_searchers/tensorflow_amd64_nvidia.py
 ailess/modules/terraform/cluster.tf
 ailess/modules/terraform/iam_policy.json
```

