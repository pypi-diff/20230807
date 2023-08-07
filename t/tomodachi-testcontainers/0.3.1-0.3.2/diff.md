# Comparing `tmp/tomodachi_testcontainers-0.3.1.tar.gz` & `tmp/tomodachi_testcontainers-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.3.1.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.3.2.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.3.1.tar` & `tomodachi_testcontainers-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.3.1/LICENSE
--rw-r--r--   0        0        0    26880 2023-07-31 18:13:07.890597 tomodachi_testcontainers-0.3.1/README.md
--rw-r--r--   0        0        0     3997 2023-08-05 09:23:46.580495 tomodachi_testcontainers-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     3953 2023-08-05 09:15:34.195694 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     3944 2023-07-31 18:13:07.895679 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1942 2023-08-03 07:36:44.798845 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2345 2023-08-05 09:22:32.578276 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1394 2023-07-31 18:13:07.896643 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     1121 2023-08-03 07:36:44.799354 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/async_probes.py
--rw-r--r--   0        0        0     2312 2023-07-31 18:13:07.897004 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2126 2023-08-02 12:29:30.549037 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-31 12:23:17.273453 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    28110 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.3.2/LICENSE
+-rw-r--r--   0        0        0    26783 2023-08-07 07:57:15.319401 tomodachi_testcontainers-0.3.2/README.md
+-rw-r--r--   0        0        0     4118 2023-08-07 08:17:49.625428 tomodachi_testcontainers-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     3953 2023-08-06 08:18:00.308951 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     3775 2023-08-07 07:57:15.321855 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1927 2023-08-07 07:57:15.321984 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2330 2023-08-07 07:57:15.322122 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1606 2023-08-07 08:17:46.564541 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     1121 2023-08-03 07:36:44.799354 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/async_probes.py
+-rw-r--r--   0        0        0     2928 2023-08-07 08:17:46.564802 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2694 2023-08-07 08:17:46.565074 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1589 2023-08-07 07:57:15.322633 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      939 2023-08-07 07:57:15.322750 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    28024 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.3.2/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.3.1/LICENSE` & `tomodachi_testcontainers-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.1/README.md` & `tomodachi_testcontainers-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -145,21 +145,22 @@
 For inter-container communication, use `tomodachi_container.get_internal_url` instead.
 
 That's it! 🎉 We have tested that the Docker image can be built and run, and that the service
 is working as expected, all with a Docker container, on the highest test level - end-to-end.
 
 ### Changing Dockerfile location
 
-If the Dockerfile is not located in the current working directory, specify a new path
-with the `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` environment variable.
+If the Dockerfile is not located in the current working directory or you need a different Docker build context,
+specify a new path with the `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` and `TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT`
+environment variables.
 
 Examples:
 
-- `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/` - specify just a directory, Dockerfile is inferred automatically
-- `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile.testing` - explicitly specify the Dockerfile name
+- `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile.testing`
+- `TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT=examples/`
 
 ### Running Tomodachi container from pre-built image
 
 If the Tomodachi service Docker image is already built, you can run the container
 by specifying the image ID in the `TOMODACHI_TESTCONTAINER_IMAGE_ID` environment variable.
 
 It is useful when running tests in the CI pipeline when the image has been already built
@@ -190,17 +191,17 @@
 from aiohttp import web
 from types_aiobotocore_s3 import S3Client
 
 
 def get_s3_client() -> S3Client:
     return get_session().create_client(
         "s3",
-        aws_access_key_id=os.environ.get("AWS_ACCESS_KEY_ID"),
-        aws_secret_access_key=os.environ.get("AWS_SECRET_ACCESS_KEY"),
-        endpoint_url=os.environ.get("AWS_S3_ENDPOINT_URL"),
+        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
+        aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
+        endpoint_url=os.getenv("AWS_S3_ENDPOINT_URL"),
     )
 
 
 class TomodachiServiceS3(tomodachi.Service):
     name = "service-s3"
 
     async def _start_service(self) -> None:
@@ -438,20 +439,20 @@
 you're well-equipped to get the most value out of Testcontainers.
 
 Bellow is the list of available Testcontainers in this library, but feel free to explore how they're
 implemented and create your own Testcontainers as you go.
 [testcontainers-python](https://github.com/testcontainers/testcontainers-python) provide and easy way
 to create your own Testcontainers.
 
-| Container Name | Default Image               | Fixture                |                                                        Image Env Var Override |
-| :------------- | :-------------------------- | :--------------------- | ----------------------------------------------------------------------------: |
-| Tomodachi      | n/a (build from Dockerfile) | `tomodachi_image`      | `TOMODACHI_TESTCONTAINER_IMAGE_ID`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` |
-| Moto           | `motoserver/moto:latest`    | `moto_container`       |                                                 `MOTO_TESTCONTAINER_IMAGE_ID` |
-| LocalStack     | `localstack/localstack:2.1` | `localstack_container` |                                           `LOCALSTACK_TESTCONTAINER_IMAGE_ID` |
-| SFTP           | `atmoz/sftp:latest`         | `sftp_container`       |                                                 `SFTP_TESTCONTAINER_IMAGE_ID` |
+| Container Name | Default Image               | Fixture                |              Image Env Var Override |
+| :------------- | :-------------------------- | :--------------------- | ----------------------------------: |
+| Tomodachi      | n/a (build from Dockerfile) | `tomodachi_image`      |  `TOMODACHI_TESTCONTAINER_IMAGE_ID` |
+| Moto           | `motoserver/moto:latest`    | `moto_container`       |       `MOTO_TESTCONTAINER_IMAGE_ID` |
+| LocalStack     | `localstack/localstack:2.1` | `localstack_container` | `LOCALSTACK_TESTCONTAINER_IMAGE_ID` |
+| SFTP           | `atmoz/sftp:latest`         | `sftp_container`       |       `SFTP_TESTCONTAINER_IMAGE_ID` |
 
 ### Tomodachi
 
 Tomodachi - a lightweight microservices library on Python asyncio.
 
 Repository: <https://github.com/kalaspuff/tomodachi>
 
@@ -481,20 +482,21 @@
 
 ## Configuration with environment variables
 
 ⚠️ Make sure that environment variables are set before running `pytest` -
 e.g. with [pytest-env](https://pypi.org/project/pytest-env/) plugin or
 by setting it in the shell before running `pytest`.
 
-| Environment Variable                      | Description                                                                                                                   |
-| :---------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
-| `TESTCONTAINER_DOCKER_NETWORK`            | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand                   |
-| `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` | Override path to Dockerfile for building Tomodachi service image. Defaults to '.'                                             |
-| `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID` | Override any supported Testcontainer Image ID. Defaults to `None`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` takes precedence |
-| `DOCKER_BUILDKIT`                         | Set `DOCKER_BUILDKIT=1` to use Docker BuildKit in `EphemeralDockerImage`                                                      |
+| Environment Variable                           | Description                                                                                                              |
+| :--------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
+| `TESTCONTAINER_DOCKER_NETWORK`                 | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand              |
+| `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH`      | Override path to Dockerfile for building Tomodachi service image. Corresponds to `--file` flag in `docker build` command |
+| `TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT` | Override Docker build context                                                                                            |
+| `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID`      | Override any supported Testcontainer Image ID. Defaults to `None`                                                        |
+| `DOCKER_BUILDKIT`                              | Set `DOCKER_BUILDKIT=1` to use Docker BuildKit for building Docker images                                                |
 
 ## Changing default Docker network
 
 By default, testcontainers are started in the default `bridge` Docker network.
 Sometimes it's useful to start containers in a different network, e.g. a network
 specifically dedicated for running automated tests.
```

### Comparing `tomodachi_testcontainers-0.3.1/pyproject.toml` & `tomodachi_testcontainers-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.3.1"
+version = "0.3.2"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
@@ -15,14 +15,16 @@
 asyncssh = { version = "^2.13.2", optional = true }
 pytest = "^7.1.2"
 pytest-asyncio = "^0.21.1"
 tenacity = "^8.2.2"
 testcontainers = "^3.7.1"
 types-aiobotocore = { extras = [
     "dynamodb",
+    "iam",
+    "lambda",
     "s3",
     "sns",
     "sqs",
     "ssm",
 ], version = "^2.5.2" }
 
 [tool.poetry.group.dev.dependencies]
@@ -163,16 +165,18 @@
 minversion = "7.0"
 junit_family = "xunit2"
 testpaths = ["tests"]
 norecursedirs = [".venv", "__pycache__", ".git"]
 log_cli_level = "INFO"
 env = [
     # Set dummy AWS credentials so that we don't accidentally mutate real infrastructure
-    "AWS_ACCESS_KEY_ID=testing",
     "AWS_DEFAULT_REGION=us-east-1",
+    "AWS_ACCESS_KEY_ID=testing",
     "AWS_SECRET_ACCESS_KEY=testing",
     "AWS_SECURITY_TOKEN=testing",
     "AWS_SESSION_TOKEN=testing",
+    # Testcontainers configuration
     "DOCKER_BUILDKIT=1",
     "TESTCONTAINER_DOCKER_NETWORK=tomodachi-testcontainers",
     "TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile",
+    "TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT=examples",
 ]
```

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from docker.models.images import Image as DockerImage
 from testcontainers.core.docker_client import DockerClient
 from testcontainers.core.utils import inside_container
 
 
 class DockerContainer(testcontainers.core.container.DockerContainer):
     def __init__(self, *args: Any, network: Optional[str] = None, **kwargs: Any) -> None:
-        self.network = network or os.getenv("TESTCONTAINER_DOCKER_NETWORK", "bridge")
+        self.network = network or os.getenv("TESTCONTAINER_DOCKER_NETWORK") or "bridge"
         super().__init__(*args, **kwargs, network=self.network)
 
     def get_container_host_ip(self) -> str:
         host = self.get_docker_client().host()
         if not host:
             return "localhost"
 
@@ -36,64 +36,58 @@
         return container["NetworkSettings"]["Networks"][self.network]["Gateway"]
 
     def restart_container(self) -> None:
         self.get_wrapped_container().restart()
 
 
 class EphemeralDockerImage:
-    def __init__(self, dockerfile: Path, docker_client_kw: Optional[Dict] = None) -> None:
+    """Builds a Docker image from a given Dockerfile and removes it when the context manager exits."""
+
+    image: DockerImage
+
+    def __init__(
+        self, dockerfile: Optional[Path] = None, context: Optional[Path] = None, docker_client_kw: Optional[Dict] = None
+    ) -> None:
+        self.dockerfile = str(dockerfile) if dockerfile else None
+        self.context = str(context) if context else "."
         self.client = DockerClient(**(docker_client_kw or {}))
-        self.image = self.build_image(dockerfile)
 
     def __enter__(self) -> DockerImage:
+        self.image = self.build_image()
         return self.image
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.remove_image()
 
-    def build_image(self, path: Path) -> DockerImage:
-        if path.is_dir():
-            dockerfile_dir = path
-            dockerfile_name = ""
-        else:
-            dockerfile_dir = path.parent
-            dockerfile_name = path.name
-
+    def build_image(self) -> DockerImage:
         if os.getenv("DOCKER_BUILDKIT"):
-            return self._build_with_docker_buildkit(dockerfile_dir, dockerfile_name)
-
-        return self._build_with_docker_client(dockerfile_dir, dockerfile_name)
+            return self._build_with_docker_buildkit()
+        return self._build_with_docker_client()
 
     def remove_image(self) -> None:
         self.client.client.images.remove(image=str(self.image.id))
 
-    def _build_with_docker_buildkit(self, dockerfile_dir: Path, dockerfile_name: str) -> DockerImage:
-        filepath = dockerfile_dir / dockerfile_name
-
+    def _build_with_docker_buildkit(self) -> DockerImage:
         cmd = ["docker", "build", "-q", "--rm=true"]
-        if filepath.is_file():
-            cmd.extend(["-f", str(filepath)])
-        cmd.append(str(dockerfile_dir))
-
-        result = subprocess.run(  # nosec: B603
-            cmd,
-            shell=False,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            check=True,
-        )
+        if self.dockerfile:
+            cmd.extend(["-f", self.dockerfile])
+        cmd.append(self.context)
+
+        result = subprocess.run(
+            cmd, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
+        )  # nosec: B603
         image_id = result.stdout.decode("utf-8").strip()
         return cast(DockerImage, self.client.client.images.get(image_id))
 
-    def _build_with_docker_client(self, dockerfile_dir: Path, dockerfile_name: str) -> DockerImage:
+    def _build_with_docker_client(self) -> DockerImage:
         image, _ = cast(
             Tuple[DockerImage, Iterator],
             self.client.client.images.build(
-                path=str(dockerfile_dir),
-                dockerfile=str(dockerfile_name),
+                dockerfile=self.dockerfile,
+                path=self.context,
                 forcerm=True,
             ),
         )
         return image
 
 
 def get_docker_image(image_id: str, docker_client_kw: Optional[Dict] = None) -> DockerImage:
```

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         region_name: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(image, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port
 
-        self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "us-east-1"
-        self.aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
-        self.aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
+        self.region_name = region_name or os.getenv("AWS_DEFAULT_REGION") or "us-east-1"
+        self.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
+        self.aws_secret_access_key = os.getenv("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
 
         self.with_bind_ports(self.internal_port, self.edge_port)
 
         # Docker is needed for running AWS Lambda container
         self.with_env("LAMBDA_DOCKER_NETWORK", self.network)
         self.with_volume_mapping("/var/run/docker.sock", "/var/run/docker.sock")
```

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/moto.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         region_name: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(image, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port
 
-        self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "us-east-1"
-        self.aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
-        self.aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
+        self.region_name = region_name or os.getenv("AWS_DEFAULT_REGION") or "us-east-1"
+        self.aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
+        self.aws_secret_access_key = os.getenv("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
 
         self.with_bind_ports(self.internal_port, self.edge_port)
         self.with_env("AWS_DEFAULT_REGION", self.region_name)
         self.with_env("AWS_ACCESS_KEY_ID", self.aws_access_key_id)
         self.with_env("AWS_SECRET_ACCESS_KEY", self.aws_secret_access_key)
 
         self.with_env("MOTO_PORT", str(self.internal_port))
```

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 import pytest
 
 from tomodachi_testcontainers.pytest.localstack_fixtures import (
     _restart_localstack_container_on_teardown,
     localstack_container,
     localstack_dynamodb_client,
+    localstack_iam_client,
+    localstack_lambda_client,
     localstack_s3_client,
     localstack_sns_client,
     localstack_sqs_client,
     localstack_ssm_client,
 )
 from tomodachi_testcontainers.pytest.moto_fixtures import (
     _reset_moto_container_on_teardown,
     moto_container,
     moto_dynamodb_client,
+    moto_iam_client,
+    moto_lambda_client,
     moto_s3_client,
     moto_sns_client,
     moto_sqs_client,
     moto_ssm_client,
 )
 from tomodachi_testcontainers.pytest.tomodachi_fixtures import tomodachi_image
 
@@ -30,20 +34,24 @@
 
 
 __all__ = [
     "_reset_moto_container_on_teardown",
     "_restart_localstack_container_on_teardown",
     "localstack_container",
     "localstack_dynamodb_client",
+    "localstack_iam_client",
+    "localstack_lambda_client",
     "localstack_s3_client",
     "localstack_sns_client",
     "localstack_sqs_client",
     "localstack_ssm_client",
     "moto_container",
     "moto_dynamodb_client",
+    "moto_iam_client",
+    "moto_lambda_client",
     "moto_s3_client",
     "moto_sns_client",
     "moto_sqs_client",
     "moto_ssm_client",
     "sftp_container",
     "tomodachi_image",
     "userpass_sftp_client",
```

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/async_probes.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/async_probes.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 import os
 from typing import AsyncGenerator, Generator
 
 import pytest
 import pytest_asyncio
 from aiobotocore.session import get_session
 from types_aiobotocore_dynamodb import DynamoDBClient
+from types_aiobotocore_iam import IAMClient
+from types_aiobotocore_lambda import LambdaClient
 from types_aiobotocore_s3 import S3Client
 from types_aiobotocore_sns import SNSClient
 from types_aiobotocore_sqs import SQSClient
 from types_aiobotocore_ssm import SSMClient
 
-from tomodachi_testcontainers.containers import LocalStackContainer
+from tomodachi_testcontainers.containers import MotoContainer
 from tomodachi_testcontainers.utils import get_available_port
 
 
 @pytest.fixture(scope="session")
-def localstack_container() -> Generator[LocalStackContainer, None, None]:
-    image = os.environ.get("LOCALSTACK_TESTCONTAINER_IMAGE_ID", "localstack/localstack:2.1")
-    with LocalStackContainer(image=image, edge_port=get_available_port()) as container:
+def moto_container() -> Generator[MotoContainer, None, None]:
+    image = os.getenv("MOTO_TESTCONTAINER_IMAGE_ID", "motoserver/moto:latest")
+    with MotoContainer(image=image, edge_port=get_available_port()) as container:
         yield container
 
 
 @pytest.fixture()
-def _restart_localstack_container_on_teardown(localstack_container: LocalStackContainer) -> Generator[None, None, None]:
+def _reset_moto_container_on_teardown(moto_container: MotoContainer) -> Generator[None, None, None]:
     yield
-    localstack_container.restart_container()
+    moto_container.reset_moto()
 
 
 @pytest_asyncio.fixture()
-async def localstack_sns_client(localstack_container: LocalStackContainer) -> AsyncGenerator[SNSClient, None]:
-    async with get_session().create_client("sns", **localstack_container.get_aws_client_config()) as c:
+async def moto_dynamodb_client(moto_container: MotoContainer) -> AsyncGenerator[DynamoDBClient, None]:
+    async with get_session().create_client("dynamodb", **moto_container.get_aws_client_config()) as c:
         yield c
 
 
 @pytest_asyncio.fixture()
-async def localstack_sqs_client(localstack_container: LocalStackContainer) -> AsyncGenerator[SQSClient, None]:
-    async with get_session().create_client("sqs", **localstack_container.get_aws_client_config()) as c:
+async def moto_iam_client(moto_container: MotoContainer) -> AsyncGenerator[IAMClient, None]:
+    async with get_session().create_client("iam", **moto_container.get_aws_client_config()) as c:
         yield c
 
 
 @pytest_asyncio.fixture()
-async def localstack_s3_client(localstack_container: LocalStackContainer) -> AsyncGenerator[S3Client, None]:
-    async with get_session().create_client("s3", **localstack_container.get_aws_client_config()) as c:
+async def moto_lambda_client(moto_container: MotoContainer) -> AsyncGenerator[LambdaClient, None]:
+    async with get_session().create_client("lambda", **moto_container.get_aws_client_config()) as c:
         yield c
 
 
 @pytest_asyncio.fixture()
-async def localstack_dynamodb_client(localstack_container: LocalStackContainer) -> AsyncGenerator[DynamoDBClient, None]:
-    async with get_session().create_client("dynamodb", **localstack_container.get_aws_client_config()) as c:
+async def moto_s3_client(moto_container: MotoContainer) -> AsyncGenerator[S3Client, None]:
+    async with get_session().create_client("s3", **moto_container.get_aws_client_config()) as c:
         yield c
 
 
 @pytest_asyncio.fixture()
-async def localstack_ssm_client(localstack_container: LocalStackContainer) -> AsyncGenerator[SSMClient, None]:
-    async with get_session().create_client("ssm", **localstack_container.get_aws_client_config()) as c:
+async def moto_sns_client(moto_container: MotoContainer) -> AsyncGenerator[SNSClient, None]:
+    async with get_session().create_client("sns", **moto_container.get_aws_client_config()) as c:
+        yield c
+
+
+@pytest_asyncio.fixture()
+async def moto_sqs_client(moto_container: MotoContainer) -> AsyncGenerator[SQSClient, None]:
+    async with get_session().create_client("sqs", **moto_container.get_aws_client_config()) as c:
+        yield c
+
+
+@pytest_asyncio.fixture()
+async def moto_ssm_client(moto_container: MotoContainer) -> AsyncGenerator[SSMClient, None]:
+    async with get_session().create_client("ssm", **moto_container.get_aws_client_config()) as c:
         yield c
```

### Comparing `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.3.2/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from tomodachi_testcontainers.containers import SFTPContainer
 from tomodachi_testcontainers.utils import get_available_port
 
 
 @pytest.fixture(scope="session")
 def sftp_container() -> Generator[SFTPContainer, None, None]:
-    image = os.environ.get("SFTP_TESTCONTAINER_IMAGE_ID", "atmoz/sftp:latest")
+    image = os.getenv("SFTP_TESTCONTAINER_IMAGE_ID", "atmoz/sftp:latest")
     with SFTPContainer(image=image, edge_port=get_available_port()) as container:
         yield container
 
 
 @pytest_asyncio.fixture()
 async def userpass_sftp_client(sftp_container: SFTPContainer) -> AsyncGenerator[asyncssh.SFTPClient, None]:
     conn_details = sftp_container.get_external_conn_details()
```

### Comparing `tomodachi_testcontainers-0.3.1/PKG-INFO` & `tomodachi_testcontainers-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.3.1
+Version: 0.3.2
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Provides-Extra: sftp
 Requires-Dist: aiobotocore (>=2.5.2,<3.0.0)
 Requires-Dist: asyncssh (>=2.13.2,<3.0.0) ; extra == "sftp"
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: testcontainers (>=3.7.1,<4.0.0)
-Requires-Dist: types-aiobotocore[dynamodb,s3,sns,sqs,ssm] (>=2.5.2,<3.0.0)
+Requires-Dist: types-aiobotocore[dynamodb,iam,lambda,s3,sns,sqs,ssm] (>=2.5.2,<3.0.0)
 Project-URL: Repository, https://github.com/filipsnastins/tomodachi-testcontainers
 Description-Content-Type: text/markdown
 
 # tomodachi-testcontainers
 
 The library provides [Testcontainers](src/tomodachi_testcontainers/containers/),
 [Pytest fixtures](src/tomodachi_testcontainers/pytest/),
@@ -170,21 +170,22 @@
 For inter-container communication, use `tomodachi_container.get_internal_url` instead.
 
 That's it! 🎉 We have tested that the Docker image can be built and run, and that the service
 is working as expected, all with a Docker container, on the highest test level - end-to-end.
 
 ### Changing Dockerfile location
 
-If the Dockerfile is not located in the current working directory, specify a new path
-with the `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` environment variable.
+If the Dockerfile is not located in the current working directory or you need a different Docker build context,
+specify a new path with the `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` and `TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT`
+environment variables.
 
 Examples:
 
-- `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/` - specify just a directory, Dockerfile is inferred automatically
-- `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile.testing` - explicitly specify the Dockerfile name
+- `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile.testing`
+- `TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT=examples/`
 
 ### Running Tomodachi container from pre-built image
 
 If the Tomodachi service Docker image is already built, you can run the container
 by specifying the image ID in the `TOMODACHI_TESTCONTAINER_IMAGE_ID` environment variable.
 
 It is useful when running tests in the CI pipeline when the image has been already built
@@ -215,17 +216,17 @@
 from aiohttp import web
 from types_aiobotocore_s3 import S3Client
 
 
 def get_s3_client() -> S3Client:
     return get_session().create_client(
         "s3",
-        aws_access_key_id=os.environ.get("AWS_ACCESS_KEY_ID"),
-        aws_secret_access_key=os.environ.get("AWS_SECRET_ACCESS_KEY"),
-        endpoint_url=os.environ.get("AWS_S3_ENDPOINT_URL"),
+        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
+        aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
+        endpoint_url=os.getenv("AWS_S3_ENDPOINT_URL"),
     )
 
 
 class TomodachiServiceS3(tomodachi.Service):
     name = "service-s3"
 
     async def _start_service(self) -> None:
@@ -463,20 +464,20 @@
 you're well-equipped to get the most value out of Testcontainers.
 
 Bellow is the list of available Testcontainers in this library, but feel free to explore how they're
 implemented and create your own Testcontainers as you go.
 [testcontainers-python](https://github.com/testcontainers/testcontainers-python) provide and easy way
 to create your own Testcontainers.
 
-| Container Name | Default Image               | Fixture                |                                                        Image Env Var Override |
-| :------------- | :-------------------------- | :--------------------- | ----------------------------------------------------------------------------: |
-| Tomodachi      | n/a (build from Dockerfile) | `tomodachi_image`      | `TOMODACHI_TESTCONTAINER_IMAGE_ID`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` |
-| Moto           | `motoserver/moto:latest`    | `moto_container`       |                                                 `MOTO_TESTCONTAINER_IMAGE_ID` |
-| LocalStack     | `localstack/localstack:2.1` | `localstack_container` |                                           `LOCALSTACK_TESTCONTAINER_IMAGE_ID` |
-| SFTP           | `atmoz/sftp:latest`         | `sftp_container`       |                                                 `SFTP_TESTCONTAINER_IMAGE_ID` |
+| Container Name | Default Image               | Fixture                |              Image Env Var Override |
+| :------------- | :-------------------------- | :--------------------- | ----------------------------------: |
+| Tomodachi      | n/a (build from Dockerfile) | `tomodachi_image`      |  `TOMODACHI_TESTCONTAINER_IMAGE_ID` |
+| Moto           | `motoserver/moto:latest`    | `moto_container`       |       `MOTO_TESTCONTAINER_IMAGE_ID` |
+| LocalStack     | `localstack/localstack:2.1` | `localstack_container` | `LOCALSTACK_TESTCONTAINER_IMAGE_ID` |
+| SFTP           | `atmoz/sftp:latest`         | `sftp_container`       |       `SFTP_TESTCONTAINER_IMAGE_ID` |
 
 ### Tomodachi
 
 Tomodachi - a lightweight microservices library on Python asyncio.
 
 Repository: <https://github.com/kalaspuff/tomodachi>
 
@@ -506,20 +507,21 @@
 
 ## Configuration with environment variables
 
 ⚠️ Make sure that environment variables are set before running `pytest` -
 e.g. with [pytest-env](https://pypi.org/project/pytest-env/) plugin or
 by setting it in the shell before running `pytest`.
 
-| Environment Variable                      | Description                                                                                                                   |
-| :---------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
-| `TESTCONTAINER_DOCKER_NETWORK`            | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand                   |
-| `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` | Override path to Dockerfile for building Tomodachi service image. Defaults to '.'                                             |
-| `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID` | Override any supported Testcontainer Image ID. Defaults to `None`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` takes precedence |
-| `DOCKER_BUILDKIT`                         | Set `DOCKER_BUILDKIT=1` to use Docker BuildKit in `EphemeralDockerImage`                                                      |
+| Environment Variable                           | Description                                                                                                              |
+| :--------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
+| `TESTCONTAINER_DOCKER_NETWORK`                 | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand              |
+| `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH`      | Override path to Dockerfile for building Tomodachi service image. Corresponds to `--file` flag in `docker build` command |
+| `TOMODACHI_TESTCONTAINER_DOCKER_BUILD_CONTEXT` | Override Docker build context                                                                                            |
+| `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID`      | Override any supported Testcontainer Image ID. Defaults to `None`                                                        |
+| `DOCKER_BUILDKIT`                              | Set `DOCKER_BUILDKIT=1` to use Docker BuildKit for building Docker images                                                |
 
 ## Changing default Docker network
 
 By default, testcontainers are started in the default `bridge` Docker network.
 Sometimes it's useful to start containers in a different network, e.g. a network
 specifically dedicated for running automated tests.
```

