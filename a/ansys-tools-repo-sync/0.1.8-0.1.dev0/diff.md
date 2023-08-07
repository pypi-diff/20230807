# Comparing `tmp/ansys-tools-repo-sync-0.1.8.tar.gz` & `tmp/ansys.tools.repo_sync-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-tools-repo-sync-0.1.8.tar", max compression
+gzip compressed data, was "ansys.tools.repo_sync-0.1.dev0.tar", max compression
```

## Comparing `ansys-tools-repo-sync-0.1.8.tar` & `ansys.tools.repo_sync-0.1.dev0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2022-04-20 09:09:37.444354 ansys-tools-repo-sync-0.1.8/LICENSE
--rw-r--r--   0        0        0     1772 2022-04-20 09:09:37.444354 ansys-tools-repo-sync-0.1.8/README.rst
--rw-r--r--   0        0        0      282 2022-04-20 09:09:37.444354 ansys-tools-repo-sync-0.1.8/ansys/tools/repo_sync/__init__.py
--rw-r--r--   0        0        0     1440 2022-04-20 09:09:37.444354 ansys-tools-repo-sync-0.1.8/ansys/tools/repo_sync/__main__.py
--rw-r--r--   0        0        0     5148 2022-04-20 09:09:37.444354 ansys-tools-repo-sync-0.1.8/ansys/tools/repo_sync/repo_sync.py
--rw-r--r--   0        0        0     1741 2022-04-20 09:09:37.444354 ansys-tools-repo-sync-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3114 2022-04-20 09:09:53.520191 ansys-tools-repo-sync-0.1.8/setup.py
--rw-r--r--   0        0        0     3131 2022-04-20 09:09:53.520514 ansys-tools-repo-sync-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      290 2022-02-18 14:31:24.973808 ansys.tools.repo_sync-0.1.dev0/ansys/tools/repo_sync/__init__.py
+-rw-r--r--   0        0        0     1170 2022-02-18 13:29:58.619862 ansys.tools.repo_sync-0.1.dev0/ansys/tools/repo_sync/__main__.py
+-rw-r--r--   0        0        0     5015 2022-02-28 16:32:49.005649 ansys.tools.repo_sync-0.1.dev0/ansys/tools/repo_sync/repo_sync.py
+-rw-r--r--   0        0        0     1083 2022-01-17 09:18:00.345128 ansys.tools.repo_sync-0.1.dev0/LICENSE
+-rw-r--r--   0        0        0     1711 2022-02-28 17:20:03.164151 ansys.tools.repo_sync-0.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1991 2022-02-28 16:38:18.562018 ansys.tools.repo_sync-0.1.dev0/README.rst
+-rw-r--r--   0        0        0     3127 2022-02-28 17:20:27.560364 ansys.tools.repo_sync-0.1.dev0/setup.py
+-rw-r--r--   0        0        0     3250 2022-02-28 17:20:27.560364 ansys.tools.repo_sync-0.1.dev0/PKG-INFO
```

### Comparing `ansys-tools-repo-sync-0.1.8/README.rst` & `ansys.tools.repo_sync-0.1.dev0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-*********************
-ansys-tools-repo-sync
-*********************
-
-The ``ansys-tools-repo-sync`` library is intended to synchronize the content
-of two different repositories.
-
-What does this library do?
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-For instance, due to intellectual properties concerns, it might not be possible
-to expose publicly the entire content of a private repository.
-Its owner could decide to have a second repository, a public one.
-Part of the content for this public repo would come from the private repository.
-
-``ansys-tools-repo-sync`` allows you to do so by copying a folder and its content
-from one repo to the other.
-In addition, it is possible to filter the type extension file authorized to be copied.
-
-.. image:: doc/images/repo_sync.png
-    :align: center
-
-
-How to use it?
-~~~~~~~~~~~~~~
-
-A common usage for this tool consist to integrate it in one of your CI/CD pipeline or workflow.
-Firstly, the tool must be installed.
-
-.. code:: bash
-
-    pip install ansys-tools-repo-sync
-
-
-Then, it can be used in the considered workflow with the appropriate arguments.
-
-Run it as follows:
-
-.. code:: bash
-
-    repo-sync --manifest path_to_manifest_file --repository target-repository-name --token github_token --organization ansys --protos-path path_to_protos_directory --dry-run
-
-.. note::
-    The ``--dry-run`` flag can be set while establishing the entire
-    workflow for the first time. It helps preventing unnecessary commits
-    of sensitive data. It will print the content expected to be committed in the
-    public repository.
-
-Issues
-------
-To post issues, questions, and code, go to `ansys-tools-repo-sync Issues
-<https://github.com/ansys/ansys-tools-repo-sync/issues>`_.
-
-
-
-License
--------
-``ansys-tools-repo-sync`` is licensed under the MIT license.
+*********************
+ansys-tools-repo-sync
+*********************
+
+The ``ansys-tools-repo-sync`` library is intended to synchronize the content
+of two different repositories.
+
+What does this library do?
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+For instance, due to intellectual properties concerns, it might not be possible
+to expose publicly the entire content of a private repository.
+Its owner could decide to have a second repository, a public one.
+Part of the content for this public repo would come from the private repository.
+
+``ansys-tools-repo-sync`` allows you to do so by copying a folder and its content
+from one repo to the other.
+In addition, it is possible to filter the type extension file authorized to be copied.
+
+.. image:: doc/images/repo_sync.png
+    :align: center
+
+
+How to use it?
+~~~~~~~~~~~~~~
+
+A common usage for this tool consist to integrate it in one of your CI/CD pipeline or workflow.
+Firstly, the tool must be installed.
+
+.. code:: bash
+
+    pip install ansys-tools-repo-sync
+
+
+Then, it can be used in the considered workflow with the appropriate arguments.
+
+Run it as follows:
+
+.. code:: yaml
+
+    python -c "from ansys.tools.repo_sync import synchronize"; synchronize(
+    manifest=os.path.join(ASSETS_DIRECTORY, "manifest.txt"),
+    token=TOKEN,
+    repository="ansys-tools-repo-sync",
+    organization="ansys",
+    protos_path=os.path.join("assets", "ansys", "api", "test", "v0"),
+    dry_run=True,
+    )"
+
+.. note::
+    The parameter ``dry_run`` can be set to ``True`` while establishing
+    the entire workflow for the first time. It helps preventing uncessary commits
+    of sensitive data. It will print the content expected to be committed in the
+    public repository.
+
+Issues
+------
+To post issues, questions, and code, go to `ansys-tools-repo-sync Issues
+<https://github.com/ansys/ansys-tools-repo-sync/issues>`_.
+
+
+
+License
+-------
+``ansys-tools-repo-sync`` is licensed under the MIT license.
```

### Comparing `ansys-tools-repo-sync-0.1.8/ansys/tools/repo_sync/repo_sync.py` & `ansys.tools.repo_sync-0.1.dev0/ansys/tools/repo_sync/repo_sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,152 @@
-import os
-import shutil
-import stat
-import subprocess
-import tempfile
-
-import github
-
-
-def synchronize(
-    manifest: str = None,
-    token: str = None,
-    repository: str = "synchronization-demo-public",
-    organization: str = "pyansys",
-    protos_path: str = r"ansys\api\test\v0",
-    dry_run: bool = True,
-):
-    """Synchronize the content of two different repositories.
-    - clone the content of the reference repository
-    - create a new branch
-    - add/ remove some folders/files.
-    - push the modification into the destination repository
-    - create a pull request to merge the modification into the main branch of the destination repository
-
-    """
-    # use secret
-    if not token:
-        token = os.environ.get("TOKEN")
-
-    user_name = os.environ.get("BOT_NAME")
-    user_email = os.environ.get("BOT_EMAIL")
-
-    branch_name = "sync/sync_branch"
-    origin_directory = os.path.join(os.getcwd())
-
-    # Create a temporary folder
-    with tempfile.TemporaryDirectory() as temp_dir:
-        os.chdir(temp_dir)
-
-        # Clone the repo.
-        process = subprocess.Popen(
-            ["git", "clone", f"https://{token}@github.com/{organization}/{repository}"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        stdout, stderr = process.communicate()
-
-        os.chdir(repository)
-
-        # Set credential
-        process = subprocess.Popen(
-            ["git", "config", "user.name", f"{user_name}"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        stdout, stderr = process.communicate()
-
-        process = subprocess.Popen(
-            ["git", "config", "user.email", f"{user_email}"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        stdout, stderr = process.communicate()
-
-        # Create a new branch.
-        try:
-            process = subprocess.Popen(
-                ["git", "checkout", "-b", branch_name],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            )
-            stdout, stderr = process.communicate()
-        except:
-            process = subprocess.Popen(
-                ["git", "checkout", branch_name],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            )
-            stdout, stderr = process.communicate()
-
-        # Read manifest
-        if manifest:
-            with open(manifest, "r") as f:
-                prohibited_extensions = f.read().splitlines()
-
-                # Add protos.
-                shutil.copytree(
-                    os.path.join(origin_directory, protos_path),
-                    os.path.join(os.getcwd(), protos_path),
-                    ignore=shutil.ignore_patterns(*prohibited_extensions),
-                )
-
-        else:
-            # Add protos.
-            shutil.copytree(
-                os.path.join(origin_directory, protos_path),
-                os.path.join(os.getcwd(), protos_path),
-            )
-
-        # unsafe, should add specific file or directory
-        process = subprocess.Popen(
-            ["git", "add", "--a"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-        stdout, stderr = process.communicate()
-
-        if protos_path:
-            message = f"""Add folder content from {protos_path}."""
-        else:
-            message = f"Copy all files located into the {repository} repository from branch {branch_name}."
-
-        if dry_run:
-            process = subprocess.Popen(
-                ["git", "commit", "-am", message, "--dry-run"],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            )
-            stdout, stderr = process.communicate()
-            print("Dry-run synchronization output:")
-            print(stdout)
-        else:
-            process = subprocess.Popen(
-                ["git", "commit", "-am", message],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            )
-            stdout, stderr = process.communicate()
-
-            process = subprocess.Popen(
-                ["git", "push", "-u", "origin", branch_name],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-            )
-            stdout, stderr = process.communicate()
-
-            # Create pull request.
-            gh = github.Github(token)
-            repo = gh.get_repo(f"{organization}/{repository}")
-            pr = repo.create_pull(title=message, body=message, head=branch_name, base="main")
-
-        # Delete the git repository that was created.
-        parent_folder = os.path.dirname(os.getcwd())
-        os.chdir(parent_folder)
-        shutil.rmtree(os.path.join(parent_folder, repository), onerror=_on_rm_error)
-        os.chdir(os.path.dirname(os.getcwd()))
-
-    if not dry_run:
-        print("Synchronization Succeeded...")
-
-
-def _on_rm_error(func, path, exc_info):
-    # path contains the path of the file that couldn't be removed
-    # let's just assume that it's read-only and unlink it.
-    os.chmod(path, stat.S_IWRITE)
-    os.unlink(path)
-
-
-if __name__ == "__main__":
-    synchronize()
+import os
+import shutil
+import stat
+import subprocess
+import tempfile
+
+import github
+
+
+def synchronize(
+    manifest: str,
+    token: str = None,
+    repository: str = "synchronization-demo-public",
+    organization: str = "pyansys",
+    protos_path: str = r"ansys\api\test\v0",
+    dry_run: bool = True,
+):
+    """Synchronize the content of two different repositories.
+    - clone the content of the reference repository
+    - create a new branch
+    - add/ remove some folders/files.
+    - push the modification into the destination repository
+    - create a pull request to merge the modification into the main branch of the destination repository
+
+    """
+    # use secret
+    if not token:
+        token = os.environ.get("TOKEN")
+
+    user_name = os.environ.get("BOT_NAME")
+    user_email = os.environ.get("BOT_EMAIL")
+
+    branch_name = "sync/sync_branch"
+    origin_directory = os.path.join(os.getcwd())
+
+    # Create a temporary folder
+    with tempfile.TemporaryDirectory() as temp_dir:
+        os.chdir(temp_dir)
+
+        # Clone the repo.
+        process = subprocess.Popen(
+            ["git", "clone", f"https://{token}@github.com/{organization}/{repository}"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        stdout, stderr = process.communicate()
+
+        os.chdir(repository)
+
+        # Set credential
+        process = subprocess.Popen(
+            ["git", "config", "user.name", f"{user_name}"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        stdout, stderr = process.communicate()
+
+        process = subprocess.Popen(
+            ["git", "config", "user.email", f"{user_email}"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        stdout, stderr = process.communicate()
+
+        # Create a new branch.
+        try:
+            process = subprocess.Popen(
+                ["git", "checkout", "-b", branch_name],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            stdout, stderr = process.communicate()
+        except:
+            process = subprocess.Popen(
+                ["git", "checkout", branch_name],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            stdout, stderr = process.communicate()
+
+        # Read manifest
+        with open(manifest, "r") as f:
+            prohibited_extensions = f.read().splitlines()
+
+        # Add protos.
+        shutil.copytree(
+            os.path.join(origin_directory, protos_path),
+            os.path.join(os.getcwd(), protos_path),
+            ignore=shutil.ignore_patterns(*prohibited_extensions),
+        )
+
+        # unsafe, should add specific file or directory
+        process = subprocess.Popen(
+            ["git", "add", "--a"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        stdout, stderr = process.communicate()
+
+        if protos_path:
+            message = f"""Add folder content from {protos_path}."""
+        else:
+            message = f"Copy all files located into the {repository} repository from branch {branch_name}."
+
+        if dry_run:
+            process = subprocess.Popen(
+                ["git", "commit", "-am", message, "--dry-run"],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            stdout, stderr = process.communicate()
+            print("Dry-run synchronization output:")
+            print(stdout)
+        else:
+            process = subprocess.Popen(
+                ["git", "commit", "-am", message],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            stdout, stderr = process.communicate()
+
+            process = subprocess.Popen(
+                ["git", "push", "-u", "origin", branch_name],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+            stdout, stderr = process.communicate()
+
+            # Create pull request.
+            gh = github.Github(token)
+            repo = gh.get_repo(f"{organization}/{repository}")
+            pr = repo.create_pull(title=message, body=message, head=branch_name, base="main")
+
+        # Delete the git repository that was created.
+        parent_folder = os.path.dirname(os.getcwd())
+        os.chdir(parent_folder)
+        shutil.rmtree(os.path.join(parent_folder, repository), onerror=_on_rm_error)
+        os.chdir(os.path.dirname(os.getcwd()))
+
+    if not dry_run:
+        print("Synchronization Succeeded...")
+
+
+def _on_rm_error(func, path, exc_info):
+    # path contains the path of the file that couldn't be removed
+    # let's just assume that it's read-only and unlink it.
+    os.chmod(path, stat.S_IWRITE)
+    os.unlink(path)
+
+
+if __name__ == "__main__":
+    synchronize()
```

### Comparing `ansys-tools-repo-sync-0.1.8/pyproject.toml` & `ansys.tools.repo_sync-0.1.dev0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry]
-name = "ansys-tools-repo-sync"
-authors = ["ANSYS, Inc."]
-maintainers = ["PyAnsys developers <pyansys.support@ansys.com>"]
-readme = "README.rst"
-homepage = "https://github.com/ansys/ansys-tools-repo-sync"
-license = "MIT"
-classifiers = ["License :: OSI Approved :: MIT License"]
-version = "0.1.8"
-description = "Synchronize the content of two different repositories."
-
-
-packages = [
-    { include = "ansys"},
-]
-
-[tool.poetry.dependencies]
-python = ">=3.7"
-importlib-metadata = {version = "^4.0", python = "<3.8"}
-
-pre-commit = "^2.15.0"
-pygithub = "1.55"
-click = "^8.0.4"
-
-Sphinx =  {version="^4.4", optional=true}
-numpydoc =  {version="^1.2", optional=true}
-pyansys_sphinx_theme =  {version="^0.2", optional=true}
-sphinx-copybutton =  {version="^0.4", optional=true}
-
-codespell = {version="^2.1", optional=true}
-flake8 = {version="^3.9", optional=true}
-
-pytest = {version="^7.0", optional=true}
-pytest-cov = {version="^3.0", optional=true}
-
-[tool.codespell]
-skip="*.pyc,*.xml,*.txt,*.gif,*.png,*.jpg,*.js,*.html,*.doctree,*.ttf,*.woff,*.woff2,*.eot,*.mp4,*.inv,*.pickle,*.ipynb,flycheck*,./.git/*,./.hypothesis/*,*.yml,./docs/build/*,./docs/images/*,./dist/*,*~,.hypothesis*,./docs/source/examples/*,*cover,*.dat,*.mac"
-
-
-[tool.black]
-line-length = 120
-target-version = ['py37']
-
-[tool.pydocstyle]
-convention = "numpy"
-
-[tool.mypy]
-python_version = 3.7
-strict = true
-
-ignore_missing_imports = true
-
-
-[tool.poetry.extras]
-docs = ["Sphinx", "numpydoc", "pyansys_sphinx_theme", "sphinx-copybutton"]
-style = ["codespell", "flake8"]
-test = ["pytest", "pytest-cov"]
-
-[tool.poetry.scripts]
-repo-sync = "ansys.tools.repo_sync._cli:synchronize"
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
+name = "ansys.tools.repo_sync"
+authors = ["ANSYS, Inc."]
+maintainers = ["PyAnsys developers <pyansys.support@ansys.com>"]
+readme = "README.rst"
+homepage = "https://github.com/ansys/ansys-tools-repo-sync"
+license = "MIT"
+classifiers = ["License :: OSI Approved :: MIT License"]
+version = "0.1.dev0"
+description = "Synchronize the content of two different repositories."
+
+
+packages = [
+    { include = "ansys"},
+]
+
+[tool.poetry.dependencies]
+python = ">=3.7"
+importlib-metadata = {version = "^4.0", python = "<3.8"}
+
+pre-commit = "^2.15.0"
+pygithub = "1.55"
+
+Sphinx =  {version="^4.4", optional=true}
+numpydoc =  {version="^1.2", optional=true}
+pyansys_sphinx_theme =  {version="^0.2", optional=true}
+sphinx-copybutton =  {version="^0.4", optional=true}
+
+codespell = {version="^2.1", optional=true}
+flake8 = {version="^3.9", optional=true}
+
+pytest = {version="^7.0", optional=true}
+pytest-cov = {version="^3.0", optional=true}
+
+[tool.codespell]
+skip="*.pyc,*.xml,*.txt,*.gif,*.png,*.jpg,*.js,*.html,*.doctree,*.ttf,*.woff,*.woff2,*.eot,*.mp4,*.inv,*.pickle,*.ipynb,flycheck*,./.git/*,./.hypothesis/*,*.yml,./docs/build/*,./docs/images/*,./dist/*,*~,.hypothesis*,./docs/source/examples/*,*cover,*.dat,*.mac"
+
+
+[tool.black]
+line-length = 120
+target-version = ['py37']
+
+[tool.pydocstyle]
+convention = "numpy"
+
+[tool.mypy]
+python_version = 3.7
+strict = true
+
+ignore_missing_imports = true
+
+
+[tool.poetry.extras]
+docs = ["Sphinx", "numpydoc", "pyansys_sphinx_theme", "sphinx-copybutton"]
+style = ["codespell", "flake8"]
+test = ["pytest", "pytest-cov"]
```

### Comparing `ansys-tools-repo-sync-0.1.8/setup.py` & `ansys.tools.repo_sync-0.1.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,41 +4,37 @@
 packages = \
 ['ansys', 'ansys.tools.repo_sync']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.0.4,<9.0.0', 'pre-commit>=2.15.0,<3.0.0', 'pygithub==1.55']
+['pre-commit>=2.15.0,<3.0.0', 'pygithub==1.55']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0,<5.0'],
  'docs': ['Sphinx>=4.4,<5.0',
           'numpydoc>=1.2,<2.0',
           'pyansys_sphinx_theme>=0.2,<0.3',
           'sphinx-copybutton>=0.4,<0.5'],
  'style': ['codespell>=2.1,<3.0', 'flake8>=3.9,<4.0'],
  'test': ['pytest>=7.0,<8.0', 'pytest-cov>=3.0,<4.0']}
 
-entry_points = \
-{'console_scripts': ['repo-sync = ansys.tools.repo_sync._cli:synchronize']}
-
 setup_kwargs = {
-    'name': 'ansys-tools-repo-sync',
-    'version': '0.1.8',
+    'name': 'ansys.tools.repo-sync',
+    'version': '0.1.dev0',
     'description': 'Synchronize the content of two different repositories.',
-    'long_description': '*********************\nansys-tools-repo-sync\n*********************\n\nThe ``ansys-tools-repo-sync`` library is intended to synchronize the content\nof two different repositories.\n\nWhat does this library do?\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nFor instance, due to intellectual properties concerns, it might not be possible\nto expose publicly the entire content of a private repository.\nIts owner could decide to have a second repository, a public one.\nPart of the content for this public repo would come from the private repository.\n\n``ansys-tools-repo-sync`` allows you to do so by copying a folder and its content\nfrom one repo to the other.\nIn addition, it is possible to filter the type extension file authorized to be copied.\n\n.. image:: doc/images/repo_sync.png\n    :align: center\n\n\nHow to use it?\n~~~~~~~~~~~~~~\n\nA common usage for this tool consist to integrate it in one of your CI/CD pipeline or workflow.\nFirstly, the tool must be installed.\n\n.. code:: bash\n\n    pip install ansys-tools-repo-sync\n\n\nThen, it can be used in the considered workflow with the appropriate arguments.\n\nRun it as follows:\n\n.. code:: bash\n\n    repo-sync --manifest path_to_manifest_file --repository target-repository-name --token github_token --organization ansys --protos-path path_to_protos_directory --dry-run\n\n.. note::\n    The ``--dry-run`` flag can be set while establishing the entire\n    workflow for the first time. It helps preventing unnecessary commits\n    of sensitive data. It will print the content expected to be committed in the\n    public repository.\n\nIssues\n------\nTo post issues, questions, and code, go to `ansys-tools-repo-sync Issues\n<https://github.com/ansys/ansys-tools-repo-sync/issues>`_.\n\n\n\nLicense\n-------\n``ansys-tools-repo-sync`` is licensed under the MIT license.\n',
+    'long_description': '*********************\nansys-tools-repo-sync\n*********************\n\nThe ``ansys-tools-repo-sync`` library is intended to synchronize the content\nof two different repositories.\n\nWhat does this library do?\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nFor instance, due to intellectual properties concerns, it might not be possible\nto expose publicly the entire content of a private repository.\nIts owner could decide to have a second repository, a public one.\nPart of the content for this public repo would come from the private repository.\n\n``ansys-tools-repo-sync`` allows you to do so by copying a folder and its content\nfrom one repo to the other.\nIn addition, it is possible to filter the type extension file authorized to be copied.\n\n.. image:: doc/images/repo_sync.png\n    :align: center\n\n\nHow to use it?\n~~~~~~~~~~~~~~\n\nA common usage for this tool consist to integrate it in one of your CI/CD pipeline or workflow.\nFirstly, the tool must be installed.\n\n.. code:: bash\n\n    pip install ansys-tools-repo-sync\n\n\nThen, it can be used in the considered workflow with the appropriate arguments.\n\nRun it as follows:\n\n.. code:: yaml\n\n    python -c "from ansys.tools.repo_sync import synchronize"; synchronize(\n    manifest=os.path.join(ASSETS_DIRECTORY, "manifest.txt"),\n    token=TOKEN,\n    repository="ansys-tools-repo-sync",\n    organization="ansys",\n    protos_path=os.path.join("assets", "ansys", "api", "test", "v0"),\n    dry_run=True,\n    )"\n\n.. note::\n    The parameter ``dry_run`` can be set to ``True`` while establishing\n    the entire workflow for the first time. It helps preventing uncessary commits\n    of sensitive data. It will print the content expected to be committed in the\n    public repository.\n\nIssues\n------\nTo post issues, questions, and code, go to `ansys-tools-repo-sync Issues\n<https://github.com/ansys/ansys-tools-repo-sync/issues>`_.\n\n\n\nLicense\n-------\n``ansys-tools-repo-sync`` is licensed under the MIT license.\n',
     'author': 'ANSYS, Inc.',
     'author_email': None,
     'maintainer': 'PyAnsys developers',
     'maintainer_email': 'pyansys.support@ansys.com',
     'url': 'https://github.com/ansys/ansys-tools-repo-sync',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'entry_points': entry_points,
     'python_requires': '>=3.7',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ansys-tools-repo-sync-0.1.8/PKG-INFO` & `ansys.tools.repo_sync-0.1.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ansys-tools-repo-sync
-Version: 0.1.8
+Name: ansys.tools.repo-sync
+Version: 0.1.dev0
 Summary: Synchronize the content of two different repositories.
 Home-page: https://github.com/ansys/ansys-tools-repo-sync
 License: MIT
 Author: ANSYS, Inc.
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.support@ansys.com
 Requires-Python: >=3.7
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Provides-Extra: style
 Provides-Extra: test
 Requires-Dist: Sphinx (>=4.4,<5.0); extra == "docs"
-Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: codespell (>=2.1,<3.0); extra == "style"
 Requires-Dist: flake8 (>=3.9,<4.0); extra == "style"
 Requires-Dist: importlib-metadata (>=4.0,<5.0); python_version < "3.8"
 Requires-Dist: numpydoc (>=1.2,<2.0); extra == "docs"
 Requires-Dist: pre-commit (>=2.15.0,<3.0.0)
 Requires-Dist: pyansys_sphinx_theme (>=0.2,<0.3); extra == "docs"
 Requires-Dist: pygithub (==1.55)
@@ -65,21 +64,28 @@
     pip install ansys-tools-repo-sync
 
 
 Then, it can be used in the considered workflow with the appropriate arguments.
 
 Run it as follows:
 
-.. code:: bash
+.. code:: yaml
 
-    repo-sync --manifest path_to_manifest_file --repository target-repository-name --token github_token --organization ansys --protos-path path_to_protos_directory --dry-run
+    python -c "from ansys.tools.repo_sync import synchronize"; synchronize(
+    manifest=os.path.join(ASSETS_DIRECTORY, "manifest.txt"),
+    token=TOKEN,
+    repository="ansys-tools-repo-sync",
+    organization="ansys",
+    protos_path=os.path.join("assets", "ansys", "api", "test", "v0"),
+    dry_run=True,
+    )"
 
 .. note::
-    The ``--dry-run`` flag can be set while establishing the entire
-    workflow for the first time. It helps preventing unnecessary commits
+    The parameter ``dry_run`` can be set to ``True`` while establishing
+    the entire workflow for the first time. It helps preventing uncessary commits
     of sensitive data. It will print the content expected to be committed in the
     public repository.
 
 Issues
 ------
 To post issues, questions, and code, go to `ansys-tools-repo-sync Issues
 <https://github.com/ansys/ansys-tools-repo-sync/issues>`_.
```

