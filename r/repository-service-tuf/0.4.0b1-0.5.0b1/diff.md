# Comparing `tmp/repository_service_tuf-0.4.0b1.tar.gz` & `tmp/repository_service_tuf-0.5.0b1.tar.gz`

## Comparing `repository_service_tuf-0.4.0b1.tar` & `repository_service_tuf-0.5.0b1.tar`

### file list

```diff
@@ -1,83 +1,85 @@
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.gitignore
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.readthedocs.yaml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/LICENSE
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/MAINTAINERS.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/Makefile
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/Pipfile
--rw-r--r--   0        0        0    82238 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/Pipfile.lock
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/README.rst
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/pyproject.toml
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/requirements-dev.txt
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/requirements.txt
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tox.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/dependabot.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/task.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/PULL_REQUEST_TEMPLATE/pr.yml
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/workflows/cd.yml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/workflows/update-python-deps.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/requirements.txt
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C1.puml
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C2.puml
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C3.puml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/conf.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/INFO
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C1.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C2.png
--rw-r--r--   0        0        0   108509 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C3.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/design.rst
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/index.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/modules.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.admin.rst
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.key.rst
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.helpers.rst
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.rst
--rw-r--r--   0        0        0    79560 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/guide/index.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/__version__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/constants.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/__init__.py
--rw-r--r--   0        0        0    23494 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/ceremony.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/import_targets.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/login.py
--rw-r--r--   0        0        0    17959 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/metadata.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/token.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/key/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/key/generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/__init__.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/api_client.py
--rw-r--r--   0        0        0    16677 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/tuf.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/conftest.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/test_tuf_repository_service.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/README.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/root.json
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JimiHendrix.pub
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online.pub
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/test__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/__init__.py
--rw-r--r--   0        0        0    24147 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_ceremony.py
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_import_targets.py
--rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_login.py
--rw-r--r--   0        0        0    29849 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_metadata_update.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/key/test_generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/helpers/__init__.py
--rw-r--r--   0        0        0    30868 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/helpers/test_api_client.py
--rw-r--r--   0        0        0    28947 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/helpers/test_tuf.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.gitignore
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/LICENSE
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/MAINTAINERS.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/Makefile
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/Pipfile
+-rw-r--r--   0        0        0    82368 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/Pipfile.lock
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/README.rst
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/requirements-dev.txt
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/requirements.txt
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tox.ini
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/task.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/PULL_REQUEST_TEMPLATE/pr.yml
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/.github/workflows/update-python-deps.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/requirements.txt
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/diagrams/repository-service-tuf-cli-C1.puml
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/diagrams/repository-service-tuf-cli-C2.puml
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/diagrams/repository-service-tuf-cli-C3.puml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/_static/INFO
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/_static/repository-service-tuf-cli-C1.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/_static/repository-service-tuf-cli-C2.png
+-rw-r--r--   0        0        0   119579 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/_static/repository-service-tuf-cli-C3.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/design.rst
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/index.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/modules.rst
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.cli.admin.rst
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.cli.key.rst
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.cli.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.helpers.rst
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.rst
+-rw-r--r--   0        0        0    80258 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/docs/source/guide/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/__version__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/constants.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/__init__.py
+-rw-r--r--   0        0        0    23494 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/ceremony.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/import_targets.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/login.py
+-rw-r--r--   0        0        0    17959 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/metadata.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/token.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/key/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/key/generate.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/cli/key/info.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/helpers/__init__.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/helpers/api_client.py
+-rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/repository_service_tuf/helpers/tuf.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/conftest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/test_tuf_repository_service.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/README.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/root.json
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/JimiHendrix.pub
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/files/key_storage/online.pub
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/test__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/admin/__init__.py
+-rw-r--r--   0        0        0    24147 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_ceremony.py
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_import_targets.py
+-rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_login.py
+-rw-r--r--   0        0        0    29849 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_metadata_update.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/key/test_generate.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/cli/key/test_info.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/helpers/__init__.py
+-rw-r--r--   0        0        0    30868 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/helpers/test_api_client.py
+-rw-r--r--   0        0        0    29006 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/tests/unit/helpers/test_tuf.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 repository_service_tuf-0.5.0b1/PKG-INFO
```

### Comparing `repository_service_tuf-0.4.0b1/.gitignore` & `repository_service_tuf-0.5.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/.pre-commit-config.yaml` & `repository_service_tuf-0.5.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/.readthedocs.yaml` & `repository_service_tuf-0.5.0b1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/CODE_OF_CONDUCT.rst` & `repository_service_tuf-0.5.0b1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/CONTRIBUTING.rst` & `repository_service_tuf-0.5.0b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/LICENSE` & `repository_service_tuf-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/Pipfile` & `repository_service_tuf-0.5.0b1/Pipfile`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 name = "pypi"
 
 [packages]
 rich-click = "*"
 securesystemslib = {extras = ["crypto"], version = "*"}
 click = "*"
 rich = "*"
+auto-click-auto = "*"
 PyNaCl = "==1.5.0"
 requests = "*"
-tuf = "==2.0.0"
+tuf = "==3.0.0"
 dynaconf = {extras = ["ini"], version = "*"}
 isort = "*"
 sqlalchemy = "*"
 psycopg2 = "*"
 
 [dev-packages]
 black = "*"
```

### Comparing `repository_service_tuf-0.4.0b1/Pipfile.lock` & `repository_service_tuf-0.5.0b1/Pipfile.lock`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9634152421652421%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'fec217ba4e9309e9930dc69982b5d9029f3fff5b0e71ca7aa0b4a475a2a5dff2'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082', "*

 * *              "'sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9'], "*

 * *              "'version': '==2023.7.22'}, 'click': {'hashes': "*

 * *              "['sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd', "*

 * *           […]*

```diff
@@ -1,32 +1,40 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "cfa21df3cb514741120ccf93fa49e9082cb5dfa093cc161b508130e0418a0c32"
+            "sha256": "fec217ba4e9309e9930dc69982b5d9029f3fff5b0e71ca7aa0b4a475a2a5dff2"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
+        "auto-click-auto": {
+            "hashes": [
+                "sha256:3df95b442b557f7d85e0d29f3692bcaba7c5b8f45c7555e931074c0e71c6f70a",
+                "sha256:a68b4186630afef4a79b14f362090bb4a396a438fb676b29bc09a81cb4973b68"
+            ],
+            "index": "pypi",
+            "version": "==0.1.0a5"
+        },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -172,55 +180,55 @@
                 "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367",
-                "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"
+                "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd",
+                "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "index": "pypi",
-            "version": "==8.1.5"
+            "version": "==8.1.6"
         },
         "configobj": {
             "hashes": [
                 "sha256:6f704434a07dc4f4dc7c9a745172c1cad449feb548febd9f7fe362629c627a97",
                 "sha256:a7a8c6ab7daade85c3f329931a807c8aee750a2494363934f8ea84d8a54c87ea",
                 "sha256:d808d7e04e6f81fbb23d5ac2cd50e69ccbee58eaf9360eb89ede22d93216a314"
             ],
             "version": "==5.0.8"
         },
         "cryptography": {
             "hashes": [
-                "sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711",
-                "sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7",
-                "sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd",
-                "sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e",
-                "sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58",
-                "sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0",
-                "sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d",
-                "sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83",
-                "sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831",
-                "sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766",
-                "sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b",
-                "sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c",
-                "sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182",
-                "sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f",
-                "sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa",
-                "sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4",
-                "sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a",
-                "sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2",
-                "sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76",
-                "sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5",
-                "sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee",
-                "sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f",
-                "sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14"
+                "sha256:0d09fb5356f975974dbcb595ad2d178305e5050656affb7890a1583f5e02a306",
+                "sha256:23c2d778cf829f7d0ae180600b17e9fceea3c2ef8b31a99e3c694cbbf3a24b84",
+                "sha256:3fb248989b6363906827284cd20cca63bb1a757e0a2864d4c1682a985e3dca47",
+                "sha256:41d7aa7cdfded09b3d73a47f429c298e80796c8e825ddfadc84c8a7f12df212d",
+                "sha256:42cb413e01a5d36da9929baa9d70ca90d90b969269e5a12d39c1e0d475010116",
+                "sha256:4c2f0d35703d61002a2bbdcf15548ebb701cfdd83cdc12471d2bae80878a4207",
+                "sha256:4fd871184321100fb400d759ad0cddddf284c4b696568204d281c902fc7b0d81",
+                "sha256:5259cb659aa43005eb55a0e4ff2c825ca111a0da1814202c64d28a985d33b087",
+                "sha256:57a51b89f954f216a81c9d057bf1a24e2f36e764a1ca9a501a6964eb4a6800dd",
+                "sha256:652627a055cb52a84f8c448185922241dd5217443ca194d5739b44612c5e6507",
+                "sha256:67e120e9a577c64fe1f611e53b30b3e69744e5910ff3b6e97e935aeb96005858",
+                "sha256:6af1c6387c531cd364b72c28daa29232162010d952ceb7e5ca8e2827526aceae",
+                "sha256:6d192741113ef5e30d89dcb5b956ef4e1578f304708701b8b73d38e3e1461f34",
+                "sha256:7efe8041897fe7a50863e51b77789b657a133c75c3b094e51b5e4b5cec7bf906",
+                "sha256:84537453d57f55a50a5b6835622ee405816999a7113267739a1b4581f83535bd",
+                "sha256:8f09daa483aedea50d249ef98ed500569841d6498aa9c9f4b0531b9964658922",
+                "sha256:95dd7f261bb76948b52a5330ba5202b91a26fbac13ad0e9fc8a3ac04752058c7",
+                "sha256:a74fbcdb2a0d46fe00504f571a2a540532f4c188e6ccf26f1f178480117b33c4",
+                "sha256:a983e441a00a9d57a4d7c91b3116a37ae602907a7618b882c8013b5762e80574",
+                "sha256:ab8de0d091acbf778f74286f4989cf3d1528336af1b59f3e5d2ebca8b5fe49e1",
+                "sha256:aeb57c421b34af8f9fe830e1955bf493a86a7996cc1338fe41b30047d16e962c",
+                "sha256:ce785cf81a7bdade534297ef9e490ddff800d956625020ab2ec2780a556c313e",
+                "sha256:d0d651aa754ef58d75cec6edfbd21259d93810b73f6ec246436a21b7841908de"
             ],
-            "version": "==41.0.2"
+            "version": "==41.0.3"
         },
         "dynaconf": {
             "extras": [
                 "ini"
             ],
             "hashes": [
                 "sha256:791d8029c74548d57b0266aabd6557ebfff6540bffd7f58ba700f577c047c0f5",
@@ -325,45 +333,43 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "psycopg2": {
             "hashes": [
-                "sha256:11aca705ec888e4f4cea97289a0bf0f22a067a32614f6ef64fcf7b8bfbc53744",
-                "sha256:1861a53a6a0fd248e42ea37c957d36950da00266378746588eab4f4b5649e95f",
-                "sha256:2362ee4d07ac85ff0ad93e22c693d0f37ff63e28f0615a16b6635a645f4b9214",
-                "sha256:36c941a767341d11549c0fbdbb2bf5be2eda4caf87f65dfcd7d146828bd27f39",
-                "sha256:53f4ad0a3988f983e9b49a5d9765d663bbe84f508ed655affdb810af9d0972ad",
-                "sha256:869776630c04f335d4124f120b7fb377fe44b0a7645ab3c34b4ba42516951889",
-                "sha256:a8ad4a47f42aa6aec8d061fdae21eaed8d864d4bb0f0cade5ad32ca16fcd6258",
-                "sha256:b81fcb9ecfc584f661b71c889edeae70bae30d3ef74fa0ca388ecda50b1222b7",
-                "sha256:d24ead3716a7d093b90b27b3d73459fe8cd90fd7065cf43b3c40966221d8c394",
-                "sha256:ded2faa2e6dfb430af7713d87ab4abbfc764d8d7fb73eafe96a24155f906ebf5",
-                "sha256:f15158418fd826831b28585e2ab48ed8df2d0d98f502a2b4fe619e7d5ca29011",
-                "sha256:f75001a1cbbe523e00b0ef896a5a1ada2da93ccd752b7636db5a99bc57c44494",
-                "sha256:f7a7a5ee78ba7dc74265ba69e010ae89dae635eea0e97b055fb641a01a31d2b1"
+                "sha256:1a6a2d609bce44f78af4556bea0c62a5e7f05c23e5ea9c599e07678995609084",
+                "sha256:44d93a0109dfdf22fe399b419bcd7fa589d86895d3931b01fb321d74dadc68f1",
+                "sha256:8275abf628c6dc7ec834ea63f6f3846bf33518907a2b9b693d41fd063767a866",
+                "sha256:91e81a8333a0037babfc9fe6d11e997a9d4dac0f38c43074886b0d9dead94fe9",
+                "sha256:b22ed9c66da2589a664e0f1ca2465c29b75aaab36fa209d4fb916025fb9119e5",
+                "sha256:b6bd7d9d3a7a63faae6edf365f0ed0e9b0a1aaf1da3ca146e6b043fb3eb5d723",
+                "sha256:c7949770cafbd2f12cecc97dea410c514368908a103acf519f2a346134caa4d5",
+                "sha256:d1210fcf99aae6f728812d1d2240afc1dc44b9e6cba526a06fb8134f969957c2",
+                "sha256:d5c5297e2fbc8068d4255f1e606bfc9291f06f91ec31b2a0d4c536210ac5c0a2",
+                "sha256:e9b04cbef584310a1ac0f0d55bb623ca3244c87c51187645432e342de9ae81a8",
+                "sha256:f00cc35bd7119f1fed17b85bd1007855194dde2cbd8de01ab8ebb17487440ad8"
             ],
             "index": "pypi",
-            "version": "==2.9.6"
+            "version": "==2.9.7"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
-                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
+                "sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692",
+                "sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.15.1"
+            "version": "==2.16.1"
         },
         "pynacl": {
             "hashes": [
                 "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
                 "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
                 "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
                 "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
@@ -383,19 +389,19 @@
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "version": "==2.31.0"
         },
         "rich": {
             "hashes": [
-                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
-                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
+                "sha256:146a90b3b6b47cac4a73c12866a499e9817426423f57c5a66949c086191a8808",
+                "sha256:fb9d6c0a0f643c99eed3875b5377a184132ba9be4d61516a55273d3554d75a39"
             ],
             "index": "pypi",
-            "version": "==13.4.2"
+            "version": "==13.5.2"
         },
         "rich-click": {
             "hashes": [
                 "sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95",
                 "sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e"
             ],
             "index": "pypi",
@@ -413,87 +419,87 @@
             "version": "==0.28.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "sqlalchemy": {
             "hashes": [
-                "sha256:00aa050faf24ce5f2af643e2b86822fa1d7149649995f11bc1e769bbfbf9010b",
-                "sha256:09397a18733fa2a4c7680b746094f980060666ee549deafdb5e102a99ce4619b",
-                "sha256:0f7fdcce52cd882b559a57b484efc92e108efeeee89fab6b623aba1ac68aad2e",
-                "sha256:10514adc41fc8f5922728fbac13d401a1aefcf037f009e64ca3b92464e33bf0e",
-                "sha256:10e001a84f820fea2640e4500e12322b03afc31d8f4f6b813b44813b2a7c7e0d",
-                "sha256:194f2d5a7cb3739875c4d25b3fe288ab0b3dc33f7c857ba2845830c8c51170a0",
-                "sha256:1aac42a21a7fa6c9665392c840b295962992ddf40aecf0a88073bc5c76728117",
-                "sha256:1fb792051db66e09c200e7bc3bda3b1eb18a5b8eb153d2cedb2b14b56a68b8cb",
-                "sha256:2756485f49e7df5c2208bdc64263d19d23eba70666f14ad12d6d8278a2fff65f",
-                "sha256:2b791577c546b6bbd7b43953565fcb0a2fec63643ad605353dd48afbc3c48317",
-                "sha256:420bc6d06d4ae7fb6921524334689eebcbea7bf2005efef070a8562cc9527a37",
-                "sha256:45b07470571bda5ee7f5ec471271bbde97267cc8403fce05e280c36ea73f4754",
-                "sha256:4ebc542d2289c0b016d6945fd07a7e2e23f4abc41e731ac8ad18a9e0c2fd0ec2",
-                "sha256:556dc18e39b6edb76239acfd1c010e37395a54c7fde8c57481c15819a3ffb13e",
-                "sha256:589aba9a35869695b319ed76c6f673d896cd01a7ff78054be1596df7ad9b096f",
-                "sha256:5c95e3e7cc6285bf7ff263eabb0d3bfe3def9a1ff98124083d45e5ece72f4579",
-                "sha256:5dd574a37be388512c72fe0d7318cb8e31743a9b2699847a025e0c08c5bf579d",
-                "sha256:67fbb40db3985c0cfb942fe8853ad94a5e9702d2987dec03abadc2f3b6a24afb",
-                "sha256:6852cd34d96835e4c9091c1e6087325efb5b607b75fd9f7075616197d1c4688a",
-                "sha256:69ae0e9509c43474e33152abe1385b8954922544616426bf793481e1a37e094f",
-                "sha256:6c5bae4c288bda92a7550fe8de9e068c0a7cd56b1c5d888aae5b40f0e13b40bd",
-                "sha256:774bd401e7993452ba0596e741c0c4d6d22f882dd2a798993859181dbffadc62",
-                "sha256:79228a7b90d95957354f37b9d46f2cc8926262ae17b0d3ed8f36c892f2a37e06",
-                "sha256:7b8cba5a25e95041e3413d91f9e50616bcfaec95afa038ce7dc02efefe576745",
-                "sha256:7db97eabd440327c35b751d5ebf78a107f505586485159bcc87660da8bb1fdca",
-                "sha256:7ddd6d35c598af872f9a0a5bce7f7c4a1841684a72dab3302e3df7f17d1b5249",
-                "sha256:82edf3a6090554a83942cec79151d6b5eb96e63d143e80e4cf6671e5d772f6be",
-                "sha256:8b7b3ebfa9416c8eafaffa65216e229480c495e305a06ba176dcac32710744e6",
-                "sha256:8da677135eff43502b7afab5a1e641edfb2dc734ba7fc146e9b1b86817a728e2",
-                "sha256:908c850b98cac1e203ababd4ba76868d19ae0d7172cdc75d3f1b7829b16837d2",
-                "sha256:9da4ee8f711e077633730955c8f3cd2485c9abf5ea0f80aac23221a3224b9a8c",
-                "sha256:a6f1d8256d06f58e6ece150fbe05c63c7f9510df99ee8ac37423f5476a2cebb4",
-                "sha256:afb322ca05e2603deedbcd2e9910f11a3fd2f42bdeafe63018e5641945c7491c",
-                "sha256:b52c6741073de5a744d27329f9803938dcad5c9fee7e61690c705f72973f4175",
-                "sha256:ba633b51835036ff0f402c21f3ff567c565a22ff0a5732b060a68f4660e2a38f",
-                "sha256:bfa1a0f83bdf8061db8d17c2029454722043f1e4dd1b3d3d3120d1b54e75825a",
-                "sha256:bffd6cd47c2e68970039c0d3e355c9ed761d3ca727b204e63cd294cad0e3df90",
-                "sha256:d7a2c1e711ce59ac9d0bba780318bcd102d2958bb423209f24c6354d8c4da930",
-                "sha256:da46beef0ce882546d92b7b2e8deb9e04dbb8fec72945a8eb28b347ca46bc15a",
-                "sha256:ebdd2418ab4e2e26d572d9a1c03877f8514a9b7436729525aa571862507b3fea",
-                "sha256:fc44e50f9d5e96af1a561faa36863f9191f27364a4df3eb70bca66e9370480b6"
+                "sha256:024d2f67fb3ec697555e48caeb7147cfe2c08065a4f1a52d93c3d44fc8e6ad1c",
+                "sha256:0bf0fd65b50a330261ec7fe3d091dfc1c577483c96a9fa1e4323e932961aa1b5",
+                "sha256:16a310f5bc75a5b2ce7cb656d0e76eb13440b8354f927ff15cbaddd2523ee2d1",
+                "sha256:1d90ccc15ba1baa345796a8fb1965223ca7ded2d235ccbef80a47b85cea2d71a",
+                "sha256:22bafb1da60c24514c141a7ff852b52f9f573fb933b1e6b5263f0daa28ce6db9",
+                "sha256:2c69ce70047b801d2aba3e5ff3cba32014558966109fecab0c39d16c18510f15",
+                "sha256:2e7b69d9ced4b53310a87117824b23c509c6fc1f692aa7272d47561347e133b6",
+                "sha256:314145c1389b021a9ad5aa3a18bac6f5d939f9087d7fc5443be28cba19d2c972",
+                "sha256:3afa8a21a9046917b3a12ffe016ba7ebe7a55a6fc0c7d950beb303c735c3c3ad",
+                "sha256:430614f18443b58ceb9dedec323ecddc0abb2b34e79d03503b5a7579cd73a531",
+                "sha256:43699eb3f80920cc39a380c159ae21c8a8924fe071bccb68fc509e099420b148",
+                "sha256:539010665c90e60c4a1650afe4ab49ca100c74e6aef882466f1de6471d414be7",
+                "sha256:57d100a421d9ab4874f51285c059003292433c648df6abe6c9c904e5bd5b0828",
+                "sha256:5831138f0cc06b43edf5f99541c64adf0ab0d41f9a4471fd63b54ae18399e4de",
+                "sha256:584f66e5e1979a7a00f4935015840be627e31ca29ad13f49a6e51e97a3fb8cae",
+                "sha256:5d6afc41ca0ecf373366fd8e10aee2797128d3ae45eb8467b19da4899bcd1ee0",
+                "sha256:61ada5831db36d897e28eb95f0f81814525e0d7927fb51145526c4e63174920b",
+                "sha256:6b54d1ad7a162857bb7c8ef689049c7cd9eae2f38864fc096d62ae10bc100c7d",
+                "sha256:7351c05db355da112e056a7b731253cbeffab9dfdb3be1e895368513c7d70106",
+                "sha256:77a14fa20264af73ddcdb1e2b9c5a829b8cc6b8304d0f093271980e36c200a3f",
+                "sha256:851a37898a8a39783aab603c7348eb5b20d83c76a14766a43f56e6ad422d1ec8",
+                "sha256:89bc2b374ebee1a02fd2eae6fd0570b5ad897ee514e0f84c5c137c942772aa0c",
+                "sha256:8e712cfd2e07b801bc6b60fdf64853bc2bd0af33ca8fa46166a23fe11ce0dbb0",
+                "sha256:8f9eb4575bfa5afc4b066528302bf12083da3175f71b64a43a7c0badda2be365",
+                "sha256:8fc05b59142445a4efb9c1fd75c334b431d35c304b0e33f4fa0ff1ea4890f92e",
+                "sha256:96f0463573469579d32ad0c91929548d78314ef95c210a8115346271beeeaaa2",
+                "sha256:9deaae357edc2091a9ed5d25e9ee8bba98bcfae454b3911adeaf159c2e9ca9e3",
+                "sha256:a752b7a9aceb0ba173955d4f780c64ee15a1a991f1c52d307d6215c6c73b3a4c",
+                "sha256:ae7473a67cd82a41decfea58c0eac581209a0aa30f8bc9190926fbf628bb17f7",
+                "sha256:b15afbf5aa76f2241184c1d3b61af1a72ba31ce4161013d7cb5c4c2fca04fd6e",
+                "sha256:c896d4e6ab2eba2afa1d56be3d0b936c56d4666e789bfc59d6ae76e9fcf46145",
+                "sha256:cb4e688f6784427e5f9479d1a13617f573de8f7d4aa713ba82813bcd16e259d1",
+                "sha256:cda283700c984e699e8ef0fcc5c61f00c9d14b6f65a4f2767c97242513fcdd84",
+                "sha256:cf7b5e3856cbf1876da4e9d9715546fa26b6e0ba1a682d5ed2fc3ca4c7c3ec5b",
+                "sha256:d6894708eeb81f6d8193e996257223b6bb4041cb05a17cd5cf373ed836ef87a2",
+                "sha256:d8f2afd1aafded7362b397581772c670f20ea84d0a780b93a1a1529da7c3d369",
+                "sha256:dd4d410a76c3762511ae075d50f379ae09551d92525aa5bb307f8343bf7c2c12",
+                "sha256:eb60699de43ba1a1f77363f563bb2c652f7748127ba3a774f7cf2c7804aa0d3d",
+                "sha256:f469f15068cd8351826df4080ffe4cc6377c5bf7d29b5a07b0e717dddb4c7ea2",
+                "sha256:f82c310ddf97b04e1392c33cf9a70909e0ae10a7e2ddc1d64495e3abdc5d19fb",
+                "sha256:fa51ce4aea583b0c6b426f4b0563d3535c1c75986c4373a0987d84d22376585b"
             ],
             "index": "pypi",
-            "version": "==2.0.18"
+            "version": "==2.0.19"
         },
         "tuf": {
             "hashes": [
-                "sha256:1524b0fbd8504245f600f121daf86b8fdcb30df74410acc9655944c4868e461c",
-                "sha256:76e7f2a7aced84466865fac2a7127b6085afae51d4328af896fb46f952dd3a53"
+                "sha256:493f5e9dc60c6a216320a82e052f6bd6f4b12cf8dfafc90ce6de537545ccfa61",
+                "sha256:e8fb94cb38f472530d591c59e87f22698355a673231f5bf50d7d1da4842c0007"
             ],
             "index": "pypi",
-            "version": "==2.0.0"
+            "version": "==3.0.0"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
                 "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
-                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.3"
+            "version": "==2.0.4"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -559,35 +565,35 @@
                 "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "chardet": {
             "hashes": [
-                "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
-                "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
+                "sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7",
+                "sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==5.1.0"
+            "version": "==5.2.0"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
                 "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
                 "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
                 "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
@@ -664,19 +670,19 @@
                 "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367",
-                "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"
+                "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd",
+                "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "index": "pypi",
-            "version": "==8.1.5"
+            "version": "==8.1.6"
         },
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
@@ -746,34 +752,34 @@
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
             "version": "==7.2.7"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
+                "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "docutils": {
             "hashes": [
                 "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.18.1"
         },
         "editables": {
             "hashes": [
-                "sha256:dc322c42e7ccaf19600874035a4573898d88aadd07e177c239298135b75da772",
-                "sha256:dd430dcf41c78d1d68ebbb893e498b0a306b554be9e7cede73b1c876c6ddbc8d"
+                "sha256:309627d9b5c4adc0e668d8c6fa7bac1ba7c8c5d415c2d27f60f081f8e80d1de2",
+                "sha256:61e5ffa82629e0d8bfe09bc44a07db3c1ab8ed1ce78a6980732870f19b5e7d4c"
             ],
-            "markers": "python_version >= '3.1'",
-            "version": "==0.4"
+            "markers": "python_version > '3'",
+            "version": "==0.5"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
                 "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
@@ -785,19 +791,19 @@
                 "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
-                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
+                "sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23",
+                "sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5"
             ],
             "index": "pypi",
-            "version": "==6.0.0"
+            "version": "==6.1.0"
         },
         "gitdb": {
             "hashes": [
                 "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
             "markers": "python_version >= '3.7'",
@@ -817,19 +823,19 @@
                 "sha256:81f2e6063cdbdf17ea11cffe603dfa3fba781da0c127a2814ab1eb5b864de2c0"
             ],
             "index": "pypi",
             "version": "==0.22.0"
         },
         "identify": {
             "hashes": [
-                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
-                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
+                "sha256:7243800bce2f58404ed41b7c002e53d4d22bcf3ae1b7900c2d7aefd95394bf7f",
+                "sha256:c22a8ead0d4ca11f1edd6c9418c3220669b3b7533ada0a0ffa6cc0ef85cf9b54"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.5.24"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.5.26"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -1004,55 +1010,55 @@
             "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "markers": "python_version >= '3.1'",
+            "markers": "python_version > '3'",
             "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
-                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
-                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
+                "sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20",
+                "sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.1"
+            "version": "==0.11.2"
         },
         "pbr": {
             "hashes": [
                 "sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b",
                 "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"
             ],
             "markers": "python_version >= '2.6'",
             "version": "==5.11.1"
         },
         "pip": {
             "hashes": [
-                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
-                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
+                "sha256:7ccf472345f20d35bdc9d1841ff5f313260c2c33fe417f48c30ac46cccabf5be",
+                "sha256:fb0bd5435b3200c602b5bf61d2d43c2f13c02e29c1707567ae7fbc514eb9faf2"
             ],
             "index": "pypi",
-            "version": "==23.1.2"
+            "version": "==23.2.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c",
-                "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"
+                "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d",
+                "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.1"
+            "version": "==3.10.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.1'",
+            "markers": "python_version > '3'",
             "version": "==1.2.0"
         },
         "pre-commit": {
             "hashes": [
                 "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
                 "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
@@ -1065,35 +1071,35 @@
                 "sha256:e389b12b7073604be67845dbe32bf8297360ad9a609b24846fe15d86e0b7dc01"
             ],
             "index": "pypi",
             "version": "==1.0.9"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
-                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
+                "sha256:259bcc17857d8a8b3b4a2327324b79e5f020a13c16074670f9c8c8f872ea76d0",
+                "sha256:5d1013ba8dc7895b548be5afb05740ca82454fd899971563d2ef625d090326f8"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.10.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.11.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
-                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
+                "sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774",
+                "sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.1.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
-                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
+                "sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692",
+                "sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.15.1"
+            "version": "==2.16.1"
         },
         "pyproject-api": {
             "hashes": [
                 "sha256:14cf09828670c7b08842249c1f28c8ee6581b872e893f81b62d5465bec41502f",
                 "sha256:ffb5b2d7cad43f5b2688ab490de7c4d3f6f15e0b819cb588c4b771567c9729eb"
             ],
             "markers": "python_version >= '3.7'",
@@ -1113,73 +1119,73 @@
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
             "version": "==7.4.0"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "version": "==2.31.0"
         },
         "rich": {
             "hashes": [
-                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
-                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
+                "sha256:146a90b3b6b47cac4a73c12866a499e9817426423f57c5a66949c086191a8808",
+                "sha256:fb9d6c0a0f643c99eed3875b5377a184132ba9be4d61516a55273d3554d75a39"
             ],
             "index": "pypi",
-            "version": "==13.4.2"
+            "version": "==13.5.2"
         },
         "setuptools": {
             "hashes": [
                 "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
                 "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
@@ -1288,67 +1294,67 @@
             "version": "==5.1.0"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "markers": "python_version >= '3.1'",
+            "markers": "python_version > '3'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
                 "sha256:1b8f8ae08d6a5475cad9d508236c51ea060620126fd7c3c513d0f5c7f29cc776",
                 "sha256:5e2ad8845764706170d3dcaac171704513cc8a725655219acb62fe4380bdadda"
             ],
             "index": "pypi",
             "version": "==4.6.4"
         },
         "types-requests": {
             "hashes": [
-                "sha256:3de667cffa123ce698591de0ad7db034a5317457a596eb0b4944e5a9d9e8d1ac",
-                "sha256:afb06ef8f25ba83d59a1d424bd7a5a939082f94b94e90ab5e6116bd2559deaa3"
+                "sha256:56d181c85b5925cbc59f4489a57e72a8b2166f18273fd8ba7b6fe0c0b986f12a",
+                "sha256:6aa3f7faf0ea52d728bb18c0a0d1522d9bfd8c72d26ff6f61bfc3d06a411cf40"
             ],
             "index": "pypi",
-            "version": "==2.31.0.1"
+            "version": "==2.31.0.2"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
-                "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
+                "sha256:229b7f577c951b8c1b92c1bc2b2fdb0b49847bd2af6d1cc2a2e3dd340f3bda8f",
+                "sha256:9683bbb7fb72e32bfe9d2be6e04875fbe1b3eeec3cbb4ea231435aa7fd6b4f0e"
             ],
-            "version": "==1.26.25.13"
+            "version": "==1.26.25.14"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
                 "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
-                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+                "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11",
+                "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.3"
+            "version": "==2.0.4"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
-                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.1"
+            "version": "==20.24.2"
         },
         "zipp": {
             "hashes": [
-                "sha256:0b37c326d826d5ca35f2b9685cd750292740774ef16190008b00a0227c256fe0",
-                "sha256:857b158da2cbf427b376da1c24fd11faecbac5a4ac7523c3607f8a01f94c2ec0"
+                "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0",
+                "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.16.1"
+            "version": "==3.16.2"
         }
     }
 }
```

### Comparing `repository_service_tuf-0.4.0b1/README.rst` & `repository_service_tuf-0.5.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/pyproject.toml` & `repository_service_tuf-0.5.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,22 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "click",
+  "auto-click-auto",
   "dynaconf[ini]==3.1.9",
   "PyNaCl",
   "requests",
   "rich",
   "rich-click",
   "securesystemslib[crypto]",
-  "tuf==2.0.0",
+  "tuf==3.0.0",
 ]
 dynamic = ["version"]
 
 [tool.mypy]
 exclude = "docs/"
 
 [[tool.mypy.overrides]]
```

### Comparing `repository_service_tuf-0.4.0b1/requirements-dev.txt` & `repository_service_tuf-0.5.0b1/requirements-dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 -i https://pypi.org/simple
-alabaster==0.7.13; python_version >= '3.6'
-babel==2.12.1; python_version >= '3.7'
+alabaster==0.7.13 ; python_version >= '3.6'
+babel==2.12.1 ; python_version >= '3.7'
 bandit==1.7.5
 black==23.7.0
 build==0.10.0
-cachetools==5.3.1; python_version >= '3.7'
-certifi==2023.5.7; python_version >= '3.6'
-cfgv==3.3.1; python_full_version >= '3.6.1'
-chardet==5.1.0; python_version >= '3.7'
-charset-normalizer==3.2.0; python_full_version >= '3.7.0'
-click==8.1.5
-colorama==0.4.6; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
+cachetools==5.3.1 ; python_version >= '3.7'
+certifi==2023.7.22 ; python_version >= '3.6'
+cfgv==3.3.1 ; python_full_version >= '3.6.1'
+chardet==5.2.0 ; python_version >= '3.7'
+charset-normalizer==3.2.0 ; python_full_version >= '3.7.0'
+click==8.1.6
+colorama==0.4.6 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
 coverage==7.2.7
-distlib==0.3.6
-docutils==0.18.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-editables==0.4; python_version >= '3.1'
-exceptiongroup==1.1.2; python_version < '3.11'
-filelock==3.12.2; python_version >= '3.7'
-flake8==6.0.0
-gitdb==4.0.10; python_version >= '3.7'
-gitpython==3.1.32; python_version >= '3.7'
+distlib==0.3.7
+docutils==0.18.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+editables==0.5 ; python_version > '3'
+exceptiongroup==1.1.2 ; python_version < '3.11'
+filelock==3.12.2 ; python_version >= '3.7'
+flake8==6.1.0
+gitdb==4.0.10 ; python_version >= '3.7'
+gitpython==3.1.32 ; python_version >= '3.7'
 hatchling==0.22.0
-identify==2.5.24; python_version >= '3.7'
-idna==3.4; python_version >= '3.5'
-imagesize==1.4.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-importlib-metadata==6.8.0; python_version < '3.10'
-iniconfig==2.0.0; python_version >= '3.7'
+identify==2.5.26 ; python_version >= '3.8'
+idna==3.4 ; python_version >= '3.5'
+imagesize==1.4.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+importlib-metadata==6.8.0 ; python_version < '3.10'
+iniconfig==2.0.0 ; python_version >= '3.7'
 isort==5.12.0
-jinja2==3.1.2; python_version >= '3.7'
-markdown-it-py==3.0.0; python_version >= '3.8'
-markupsafe==2.1.3; python_version >= '3.7'
-mccabe==0.7.0; python_version >= '3.6'
-mdurl==0.1.2; python_version >= '3.7'
+jinja2==3.1.2 ; python_version >= '3.7'
+markdown-it-py==3.0.0 ; python_version >= '3.8'
+markupsafe==2.1.3 ; python_version >= '3.7'
+mccabe==0.7.0 ; python_version >= '3.6'
+mdurl==0.1.2 ; python_version >= '3.7'
 mypy==1.4.1
-mypy-extensions==1.0.0; python_version >= '3.5'
-nodeenv==1.8.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
-packaging==23.1; python_version >= '3.1'
-pathspec==0.11.1; python_version >= '3.7'
-pbr==5.11.1; python_version >= '2.6'
-pip==23.1.2
-platformdirs==3.8.1; python_version >= '3.7'
-pluggy==1.2.0; python_version >= '3.1'
+mypy-extensions==1.0.0 ; python_version >= '3.5'
+nodeenv==1.8.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
+packaging==23.1 ; python_version > '3'
+pathspec==0.11.2 ; python_version >= '3.7'
+pbr==5.11.1 ; python_version >= '2.6'
+pip==23.2.1
+platformdirs==3.10.0 ; python_version >= '3.7'
+pluggy==1.2.0 ; python_version > '3'
 pre-commit==3.3.3
 pretend==1.0.9
-pycodestyle==2.10.0; python_version >= '3.6'
-pyflakes==3.0.1; python_version >= '3.6'
-pygments==2.15.1; python_version >= '3.7'
-pyproject-api==1.5.3; python_version >= '3.7'
-pyproject-hooks==1.0.0; python_version >= '3.7'
+pycodestyle==2.11.0 ; python_version >= '3.8'
+pyflakes==3.1.0 ; python_version >= '3.8'
+pygments==2.16.1 ; python_version >= '3.7'
+pyproject-api==1.5.3 ; python_version >= '3.7'
+pyproject-hooks==1.0.0 ; python_version >= '3.7'
 pytest==7.4.0
-pyyaml==6.0; python_version >= '3.6'
+pyyaml==6.0.1 ; python_version >= '3.6'
 requests==2.31.0
-rich==13.4.2
-setuptools==68.0.0; python_version >= '3.7'
-smmap==5.0.0; python_version >= '3.6'
+rich==13.5.2
+setuptools==68.0.0 ; python_version >= '3.7'
+smmap==5.0.0 ; python_version >= '3.6'
 snowballstemmer==2.2.0
 sphinx==6.2.1
 sphinx-rtd-theme==1.2.2
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
-sphinxcontrib-jquery==4.1; python_version >= '2.7'
+sphinxcontrib-jquery==4.1 ; python_version >= '2.7'
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-plantuml==0.25
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-stevedore==5.1.0; python_version >= '3.8'
-tomli==2.0.1; python_version >= '3.1'
+stevedore==5.1.0 ; python_version >= '3.8'
+tomli==2.0.1 ; python_version > '3'
 tox==4.6.4
-types-requests==2.31.0.1
-types-urllib3==1.26.25.13
-typing-extensions==4.7.1; python_version >= '3.7'
-urllib3==2.0.3; python_version >= '3.7'
-virtualenv==20.23.1; python_version >= '3.7'
-zipp==3.16.1; python_version >= '3.8'
+types-requests==2.31.0.2
+types-urllib3==1.26.25.14
+typing-extensions==4.7.1 ; python_version >= '3.7'
+urllib3==2.0.4 ; python_version >= '3.7'
+virtualenv==20.24.2 ; python_version >= '3.7'
+zipp==3.16.2 ; python_version >= '3.8'
+auto-click-auto==0.1.0a5
 cffi==1.15.1
 configobj==5.0.8
-cryptography==41.0.2
+cryptography==41.0.3
 dynaconf[ini]==3.2.0
-greenlet==2.0.2; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
-psycopg2==2.9.6
+greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
+psycopg2==2.9.7
 pycparser==2.21
 pynacl==1.5.0
 rich-click==1.6.1
 securesystemslib[crypto]==0.28.0
-six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.18
-tuf==2.0.0
+six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
+sqlalchemy==2.0.19
+tuf==3.0.0
```

### Comparing `repository_service_tuf-0.4.0b1/requirements.txt` & `repository_service_tuf-0.5.0b1/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 -i https://pypi.org/simple
-certifi==2023.5.7; python_version >= '3.6'
+auto-click-auto==0.1.0a5
+certifi==2023.7.22 ; python_version >= '3.6'
 cffi==1.15.1
-charset-normalizer==3.2.0; python_full_version >= '3.7.0'
-click==8.1.5
+charset-normalizer==3.2.0 ; python_full_version >= '3.7.0'
+click==8.1.6
 configobj==5.0.8
-cryptography==41.0.2
+cryptography==41.0.3
 dynaconf[ini]==3.2.0
-greenlet==2.0.2; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
-idna==3.4; python_version >= '3.5'
+greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
+idna==3.4 ; python_version >= '3.5'
 isort==5.12.0
-markdown-it-py==3.0.0; python_version >= '3.8'
-mdurl==0.1.2; python_version >= '3.7'
-psycopg2==2.9.6
+markdown-it-py==3.0.0 ; python_version >= '3.8'
+mdurl==0.1.2 ; python_version >= '3.7'
+psycopg2==2.9.7
 pycparser==2.21
-pygments==2.15.1; python_version >= '3.7'
+pygments==2.16.1 ; python_version >= '3.7'
 pynacl==1.5.0
 requests==2.31.0
-rich==13.4.2
+rich==13.5.2
 rich-click==1.6.1
 securesystemslib[crypto]==0.28.0
-six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.18
-tuf==2.0.0
-typing-extensions==4.7.1; python_version >= '3.7'
-urllib3==2.0.3; python_version >= '3.7'
+six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
+sqlalchemy==2.0.19
+tuf==3.0.0
+typing-extensions==4.7.1 ; python_version >= '3.7'
+urllib3==2.0.4 ; python_version >= '3.7'
```

### Comparing `repository_service_tuf-0.4.0b1/tox.ini` & `repository_service_tuf-0.5.0b1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 [testenv:docs]
 deps = -r{toxinidir}/docs/requirements.txt
 allowlist_externals =
     plantuml
 commands =
     plantuml -o ../source/_static/ -tpng docs/diagrams/*.puml
-	sphinx-apidoc -o  docs/source/devel/ repository_service_tuf
+	sphinx-apidoc -f -o  docs/source/devel/ repository_service_tuf
 	sphinx-build -E -W -b html docs/source docs/build/html
 
 [gh-actions]
 python =
     3.9: py39,pep8,lint,typing,requirements,test,docs
     3.10: py310,pep8,lint,typing,requirements,test,docs
     3.11: py311,pep8,lint,typing,requirements,test,docs
```

### Comparing `repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/bug.yml` & `repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/other.yml` & `repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/other.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/task.yml` & `repository_service_tuf-0.5.0b1/.github/ISSUE_TEMPLATE/task.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/.github/PULL_REQUEST_TEMPLATE/pr.yml` & `repository_service_tuf-0.5.0b1/.github/PULL_REQUEST_TEMPLATE/pr.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/.github/workflows/cd.yml` & `repository_service_tuf-0.5.0b1/.github/workflows/cd.yml`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     steps:
       - name: Checkout release tag
         uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9
         with:
           ref: ${{ github.event.workflow_run.head_branch }}
 
       - name: Set up Python
-        uses: actions/setup-python@bd6b4b6205c4dbad673328db7b31b7fab9e241c0
+        uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1
         with:
           python-version: '3.x'
 
       - name: Install build dependency
         run: python3 -m pip install --upgrade pip build twine
 
       - name: Build binary wheel and source tarball
@@ -90,18 +90,18 @@
             })
 
       - name: Publish distribution 📦 to Test PyPI
         env:
           name: testpypi
           url: https://pypi.org/p/repository-service-tuf
         if: github.repository == 'repository-service-tuf/repository-service-tuf-cli'
-        uses: pypa/gh-action-pypi-publish@f5622bde02b04381239da3573277701ceca8f6a0
+        uses: pypa/gh-action-pypi-publish@f8c70e705ffc13c3b4d1221169b84f12a75d6ca8
         with:
           repository-url: https://test.pypi.org/legacy/
 
       - name: Publish binary wheel and source tarball 📦 on PyPI
         env:
           name: pypi
           url: https://pypi.org/p/repository-service-tuf
         # Only attempt PyPI upload in upstream repository
         if: github.repository == 'repository-service-tuf/repository-service-tuf-cli'
-        uses: pypa/gh-action-pypi-publish@f5622bde02b04381239da3573277701ceca8f6a0
+        uses: pypa/gh-action-pypi-publish@f8c70e705ffc13c3b4d1221169b84f12a75d6ca8
```

### Comparing `repository_service_tuf-0.4.0b1/.github/workflows/ci.yml` & `repository_service_tuf-0.5.0b1/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-versions: [ "3.9", "3.10", "3.11" ]
 
     steps:
     - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9
-    - uses: actions/setup-python@bd6b4b6205c4dbad673328db7b31b7fab9e241c0
+    - uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1
       with:
         python-version: ${{ matrix.python-versions }}
 
     - name: Install tox and coverage
       run: pip install tox tox-gh-actions build
 
     - name: Install build dependency
```

### Comparing `repository_service_tuf-0.4.0b1/.github/workflows/update-python-deps.yml` & `repository_service_tuf-0.5.0b1/.github/workflows/update-python-deps.yml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   update-dep:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-versions: [ "3.9" ]
     steps:
       - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9
-      - uses: actions/setup-python@bd6b4b6205c4dbad673328db7b31b7fab9e241c0
+      - uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1
         with:
           python-version: ${{ matrix.python-versions }}
       - name: Install prerequisites
         run: |
           pip install tox pipenv
       - name: Update dependencies
         run: |
```

### Comparing `repository_service_tuf-0.4.0b1/docs/Makefile` & `repository_service_tuf-0.5.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/make.bat` & `repository_service_tuf-0.5.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C1.puml` & `repository_service_tuf-0.5.0b1/docs/diagrams/repository-service-tuf-cli-C1.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C2.puml` & `repository_service_tuf-0.5.0b1/docs/diagrams/repository-service-tuf-cli-C2.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C3.puml` & `repository_service_tuf-0.5.0b1/docs/diagrams/repository-service-tuf-cli-C3.puml`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,18 @@
                     Container(update, "update")
                 }
                 Container(login, "login")
                 Container_Boundary(token, "token"){
                     Container(generate, "generate")
                 }
             }
+            Container_Boundary(key, "key") {
+                Container(key_generate, "generate")
+                Container(info, "info")
+            }
         }
         Container_Boundary(users, "helpers",) #LightBlue {
             Container(api_client, "api_client")
             Container_Boundary(tuf, "tuf",) #APPLICATION {
                 Container_Ext(python_tuf, "python-tuf")
             }
 
@@ -67,24 +71,27 @@
     }
 }
 Container(tuf_repository_service_api, "REPOSITORY-SERVICE-TUF-API", "HTTP REST API", $tags="queue") #APPLICATION
 
 Rel_R(user, trs_cli, "rstuf-cli", $tags="terminal")
 
 Rel(ceremony, tuf, " ")
+Rel(info, tuf, " ")
 Rel(ceremony, api_client, " ")
 Rel(update, tuf, " ")
 Rel(update, api_client, " ")
 Rel_R(generate, api_client, " ")
 Rel_L(token, click, " ")
 Rel(login, api_client, " ")
 Rel(api_client, requests, " ")
 Rel(dynaconf, user, " ", $tags="os")
 Rel(python_tuf, user, " ", $tags="os")
 Rel_U(ceremony, click, " ")
+Rel_U(key_generate, click, " ")
+Rel_U(info, click, " ")
 Rel_U(login, click, " ")
 Rel_U(update, click, " ")
 
 Rel(requests, tuf_repository_service_api, " ")
 
 HIDE_STEREOTYPE()
 @enduml
```

### Comparing `repository_service_tuf-0.4.0b1/docs/source/conf.py` & `repository_service_tuf-0.5.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C1.png` & `repository_service_tuf-0.5.0b1/docs/source/_static/repository-service-tuf-cli-C1.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C2.png` & `repository_service_tuf-0.5.0b1/docs/source/_static/repository-service-tuf-cli-C2.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/source/devel/design.rst` & `repository_service_tuf-0.5.0b1/docs/source/devel/design.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.admin.rst` & `repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.cli.admin.rst`

 * *Files 19% similar despite different names*

```diff
@@ -8,22 +8,38 @@
 --------------------------------------------------
 
 .. automodule:: repository_service_tuf.cli.admin.ceremony
    :members:
    :undoc-members:
    :show-inheritance:
 
+repository\_service\_tuf.cli.admin.import\_targets module
+---------------------------------------------------------
+
+.. automodule:: repository_service_tuf.cli.admin.import_targets
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 repository\_service\_tuf.cli.admin.login module
 -----------------------------------------------
 
 .. automodule:: repository_service_tuf.cli.admin.login
    :members:
    :undoc-members:
    :show-inheritance:
 
+repository\_service\_tuf.cli.admin.metadata module
+--------------------------------------------------
+
+.. automodule:: repository_service_tuf.cli.admin.metadata
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 repository\_service\_tuf.cli.admin.token module
 -----------------------------------------------
 
 .. automodule:: repository_service_tuf.cli.admin.token
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.helpers.rst` & `repository_service_tuf-0.5.0b1/docs/source/devel/repository_service_tuf.helpers.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/docs/source/guide/index.rst` & `repository_service_tuf-0.5.0b1/docs/source/guide/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -882,20 +882,21 @@
 
     ❯ rstuf key
 
     Usage: rstuf key [OPTIONS] COMMAND [ARGS]...
 
     Cryptographic Key Commands
 
-    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-    │ --help  -h    Show this message and exit.                                                                                        │
-    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-    │ generate                        Generate cryptographic keys using the `securesystemslib` library                                 │
-    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+    │ --help  -h    Show this message and exit.                                                        │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
+    │ generate     Generate cryptographic keys using the `securesystemslib` library                    │
+    │ info         Get key information                                                                 │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 
 .. rstuf-cli-key-generate
 
 Key Generation (``generate``)
 -----------------------------
 
@@ -918,8 +919,30 @@
 .. code::
 
     ❯ rstuf key generate
 
     Choose key type [ed25519/ecdsa/rsa] (ed25519): ed25519
     Enter the key's filename: (id_ed25519): id_ed25519
     Enter password to encrypt private key file 'id_ed25519':
-    Confirm:
+    Confirm:
+
+.. rstuf-cli-key-info
+
+Key Information (``info``)
+--------------------------
+
+Show relevant information about a key.
+
+.. code::
+
+    ❯ rstuf key info --help
+
+    Usage: rstuf key info [OPTIONS]
+
+    Show key information
+
+    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
+    │ --show-private        Show the private key. WARNING: use private key information carefully.      │
+    │ --help          -h    Show this message and exit.                                                │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+
+
```

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/constants.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/constants.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/__init__.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import os
 import pkgutil
 import re
 import sys
 from pathlib import Path
 
 import rich_click as click  # type: ignore
+from auto_click_auto import enable_click_shell_completion
+from auto_click_auto.constants import ShellType
 from rich.console import Console
 from rich.panel import Panel
 
 from repository_service_tuf import Dynaconf
 from repository_service_tuf.__version__ import version
 
 console = Console()
@@ -86,7 +88,15 @@
 for _, name, _ in pkgutil.walk_packages(  # type: ignore
     __path__, prefix=__name__ + "."
 ):
     if name in groups_required_auth and "--auth" not in sys.argv:
         continue
     else:
         importlib.import_module(name)
+
+# Enable tab completion for all available supported shells
+supported_shell_types = {
+    ShellType(shell) for shell in ShellType.get_all_values()
+}
+enable_click_shell_completion(
+    program_name=prog_name, shells=supported_shell_types
+)
```

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/ceremony.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/ceremony.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/import_targets.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/login.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/metadata.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/metadata.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/token.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/admin/token.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/key/generate_key.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/cli/key/generate.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/api_client.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/tuf.py` & `repository_service_tuf-0.5.0b1/repository_service_tuf/helpers/tuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,19 @@
     Error,
     FormatError,
     StorageError,
 )
 from securesystemslib.interface import (  # type: ignore
     import_privatekey_from_file,
 )
-from securesystemslib.signer import Signer, SSlibSigner  # type: ignore
+from securesystemslib.signer import Signer  # type: ignore
+from securesystemslib.signer import SSlibSigner  # type: ignore
+from securesystemslib.signer import SSlibKey as Key  # type: ignore
 from tuf.api.exceptions import UnsignedMetadataError
-from tuf.api.metadata import SPECIFICATION_VERSION, Key, Metadata, Role, Root
+from tuf.api.metadata import SPECIFICATION_VERSION, Metadata, Role, Root
 from tuf.api.serialization.json import JSONSerializer
 
 console = Console()
 
 SPEC_VERSION: str = ".".join(SPECIFICATION_VERSION)
 BINS: str = "bins"
```

### Comparing `repository_service_tuf-0.4.0b1/tests/conftest.py` & `repository_service_tuf-0.5.0b1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from datetime import datetime
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, List, Tuple
 
 import pytest  # type: ignore
 from click.testing import CliRunner  # type: ignore
 from dynaconf import Dynaconf
-from tuf.api.metadata import Key, Metadata, Root
+from securesystemslib.signer import SSlibKey as Key
+from tuf.api.metadata import Metadata, Root
 
 from repository_service_tuf.helpers.tuf import (
     BootstrapSetup,
     Roles,
     RootInfo,
     RSTUFKey,
     ServiceSettings,
```

### Comparing `repository_service_tuf-0.4.0b1/tests/test_tuf_repository_service.py` & `repository_service_tuf-0.5.0b1/tests/test_tuf_repository_service.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/files/root.json` & `repository_service_tuf-0.5.0b1/tests/files/root.json`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/files/key_storage/JanisJoplin.key` & `repository_service_tuf-0.5.0b1/tests/files/key_storage/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/files/key_storage/JimiHendrix.key` & `repository_service_tuf-0.5.0b1/tests/files/key_storage/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.key` & `repository_service_tuf-0.5.0b1/tests/files/key_storage/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.pub` & `repository_service_tuf-0.5.0b1/tests/files/key_storage/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/files/key_storage/online.key` & `repository_service_tuf-0.5.0b1/tests/files/key_storage/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/cli/test__init__.py` & `repository_service_tuf-0.5.0b1/tests/unit/cli/test__init__.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_ceremony.py` & `repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_ceremony.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_import_targets.py` & `repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_login.py` & `repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_metadata_update.py` & `repository_service_tuf-0.5.0b1/tests/unit/cli/admin/test_metadata_update.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/cli/key/test_generate_key.py` & `repository_service_tuf-0.5.0b1/tests/unit/cli/key/test_generate.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from unittest import mock
 from unittest.mock import patch
 
 import pretend
 import pytest
 from securesystemslib.exceptions import FormatError  # type: ignore
 
-from repository_service_tuf.cli.key import generate_key
-from repository_service_tuf.cli.key.generate_key import _verify_password
+from repository_service_tuf.cli.key import generate
+from repository_service_tuf.cli.key.generate import _verify_password
 from repository_service_tuf.constants import KeyType
 
 
 class TestGenerateInteraction:
     """Test the Key Generate Interaction"""
 
     @pytest.mark.parametrize("key_type", KeyType.get_all_members() + ["\n"])
@@ -22,15 +22,15 @@
         """
         Test that all `KeyType` enum members are possible input choices.
 
         Note: We also test that a default ('\n') key type value is set
         """
 
         test_result = client.invoke(
-            generate_key.generate,
+            generate.generate,
             input=key_type,  # Choose key type [ed25519/ecdsa/rsa] (ed25519)
         )
 
         assert (
             "Choose key type [ed25519/ecdsa/rsa] (ed25519):"
         ) in test_result.output
 
@@ -38,136 +38,128 @@
             "Please select one of the available options"
             not in test_result.output
         )
 
         assert test_result.exit_code == 1
 
     @pytest.mark.parametrize("key_type", KeyType.get_all_members() + ["test"])
-    def test_generate_key_types_generation(
-        self, key_type, client, monkeypatch
-    ) -> None:
+    def test_generate_types_generation(self, key_type, client) -> None:
         """
         Test that all `KeyType` enum members input choices call the appropriate
         keypair generate function
         """
 
         password = "test-password"
         filename = "test-filename"
         inputs = [
             key_type,  # Choose key type [ed25519/ecdsa/rsa] (ed25519)
             filename,  # Enter the keys' filename ...
             "n",  # Do you want to overwrite the existing 'test-filename' file?
         ]
 
-        generate_key._verify_password = pretend.call_recorder(
-            lambda a: password
-        )
+        generate._verify_password = pretend.call_recorder(lambda a: password)
 
-        mock_file_path = "repository_service_tuf.cli.key.generate_key."
+        mock_file_path = "repository_service_tuf.cli.key.generate."
         mocked_functions = {
             "ed25519": "_generate_and_write_ed25519_keypair",
             "ecdsa": "_generate_and_write_ecdsa_keypair",
             "rsa": "_generate_and_write_rsa_keypair",
         }
 
         if key_type in KeyType.get_all_members():
             with patch(
                 mock_file_path + mocked_functions[key_type],
                 return_value=None,
             ) as mock_keypair:
                 test_result = client.invoke(
-                    generate_key.generate,
+                    generate.generate,
                     input="\n".join(inputs),
                 )
 
                 mock_keypair.called_once()
                 assert test_result.exit_code == 0
 
         else:
             test_result = client.invoke(
-                generate_key.generate,
+                generate.generate,
                 input="\n".join(inputs),
             )
 
             assert test_result.exit_code == 1
 
     @pytest.mark.parametrize("filename", ["\n", "test-filename"])
-    def test_generate(self, filename: str, client, monkeypatch) -> None:
+    def test_generate(self, filename: str, client) -> None:
         """
         Test all the steps in the `generate` sub-command work as expected
 
         Note: We also test that a default ('\n') filename value is set
         """
 
         try:
             key_type = "rsa"
             password = "test-password"
             inputs = [
                 key_type,  # Choose key type [ed25519/ecdsa/rsa] (ed25519)
                 filename,  # Enter the keys' filename ...
             ]
 
-            generate_key._verify_password = pretend.call_recorder(
+            generate._verify_password = pretend.call_recorder(
                 lambda a: password
             )
 
             test_result = client.invoke(
-                generate_key.generate,
+                generate.generate,
                 input="\n".join(inputs),
             )
 
             # the default option for the filename
             if filename == "\n":
                 filepath = f"id_{key_type}"
             else:
                 filepath = filename
 
-            assert generate_key._verify_password.calls == [  # type: ignore
+            assert generate._verify_password.calls == [  # type: ignore
                 pretend.call(filepath)
             ]
 
             # password not shown in output
             assert password not in test_result.output
 
             assert test_result.exit_code == 0
 
         finally:
             # remove the generated keys
             Path(filepath).unlink(missing_ok=True)
             Path(filepath + ".pub").unlink(missing_ok=True)
 
-    def test_generate_file_overwrite(self, client, monkeypatch) -> None:
+    def test_generate_file_overwrite(self, client) -> None:
         """Test the 'overwrite file' prompt"""
 
         key_type = "rsa"
         password = "test-password"
         filename = "test-filename"
         inputs = [
             key_type,  # Choose key type [ed25519/ecdsa/rsa] (ed25519)
             filename,  # Enter the keys' filename ...
             "n",  # Do you want to overwrite the existing 'test-filename' file?
         ]
 
-        generate_key.os.path.isfile = pretend.call_recorder(
-            lambda *a, **kw: True
-        )
+        generate.os.path.isfile = pretend.call_recorder(lambda *a, **kw: True)
 
-        generate_key._verify_password = pretend.call_recorder(
-            lambda a: password
-        )
+        generate._verify_password = pretend.call_recorder(lambda a: password)
 
         test_result = client.invoke(
-            generate_key.generate,
+            generate.generate,
             input="\n".join(inputs),
         )
 
-        assert generate_key.os.path.isfile.calls == [pretend.call(filename)]  # type: ignore # noqa: E501
+        assert generate.os.path.isfile.calls == [pretend.call(filename)]  # type: ignore # noqa: E501
 
         # verify `_verify_password` is never called
-        assert generate_key._verify_password.calls == []  # type: ignore
+        assert generate._verify_password.calls == []  # type: ignore
 
         assert (
             f"Do you want to overwrite the existing '{filename}' file?"
             in test_result.output
         )
 
         assert "Key creation aborted." in test_result.output
@@ -177,32 +169,32 @@
 
         assert test_result.exit_code == 1
 
 
 class TestGenerateFunctions:
     """Test the Key Generate Functions"""
 
-    @mock.patch("repository_service_tuf.cli.key.generate_key.get_password")
+    @mock.patch("repository_service_tuf.cli.key.generate.get_password")
     def test__verify_password(self, mock_password, capsys) -> None:
         """
         Test that the password is verified correctly
         """
 
         mock_password.return_value = "test-password"
 
-        _verify_password("test-filename")
+        generate._verify_password("test-filename")
 
         captured = capsys.readouterr()
 
         assert (
             "encryption password must be 1 or more characters long\n"
             not in captured.out
         )
 
-    @mock.patch("repository_service_tuf.cli.key.generate_key.get_password")
+    @mock.patch("repository_service_tuf.cli.key.generate.get_password")
     def test__verify_password_empty_password(
         self, mock_password, capsys
     ) -> None:
         """
         Test that the password is verified correctly if it is empty at the
         first attempt
         """
@@ -213,18 +205,16 @@
 
         captured = capsys.readouterr()
 
         assert captured.out == (
             "encryption password must be 1 or more characters long\n"
         )
 
-    @mock.patch("repository_service_tuf.cli.key.generate_key.get_password")
-    def test__verify_password_not_string_password(
-        self, mock_password, capsys
-    ) -> None:
+    @mock.patch("repository_service_tuf.cli.key.generate.get_password")
+    def test__verify_password_not_string_password(self, mock_password) -> None:
         """
         Test that the password is verified correctly if it is a number at the
         first attempt
         """
 
         password = 123
         mock_password.side_effect = [password, "test-password"]
```

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/helpers/test_api_client.py` & `repository_service_tuf-0.5.0b1/tests/unit/helpers/test_api_client.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.4.0b1/tests/unit/helpers/test_tuf.py` & `repository_service_tuf-0.5.0b1/tests/unit/helpers/test_tuf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import copy
 import unittest.mock
 from datetime import datetime, timedelta
 from typing import Dict, List
 
 import pretend
 import pytest
+from securesystemslib.signer import SSlibKey as Key  # type: ignore
 from tuf.api.exceptions import UnsignedMetadataError
 
 from repository_service_tuf.constants import KeyType
 from repository_service_tuf.helpers import tuf
 from repository_service_tuf.helpers.tuf import (
-    Key,
     Metadata,
     Roles,
     Root,
     RootInfo,
     RSTUFKey,
     TUFManagement,
     load_key,
```

### Comparing `repository_service_tuf-0.4.0b1/PKG-INFO` & `repository_service_tuf-0.5.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: repository-service-tuf
-Version: 0.4.0b1
+Version: 0.5.0b1
 Summary: Repository Service for TUF Command Line Interface
 Author-email: Kairo de Araujo <kairo@dearaujo.nl>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
+Requires-Dist: auto-click-auto
 Requires-Dist: click
 Requires-Dist: dynaconf[ini]==3.1.9
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: rich-click
 Requires-Dist: securesystemslib[crypto]
-Requires-Dist: tuf==2.0.0
+Requires-Dist: tuf==3.0.0
 Provides-Extra: psycopg2
 Requires-Dist: psycopg2>=2.9.5; extra == 'psycopg2'
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=2.0.1; extra == 'sqlalchemy'
 Description-Content-Type: text/x-rst
 
 #################################################
```

