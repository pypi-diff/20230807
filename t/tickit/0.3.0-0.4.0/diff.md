# Comparing `tmp/tickit-0.3.0.tar.gz` & `tmp/tickit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickit-0.3.0.tar", last modified: Thu Jul 20 14:54:59 2023, max compression
+gzip compressed data, was "tickit-0.4.0.tar", last modified: Mon Aug  7 14:30:25 2023, max compression
```

## Comparing `tickit-0.3.0.tar` & `tickit-0.4.0.tar`

### file list

```diff
@@ -1,257 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 14:54:49.000000 tickit-0.3.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 14:54:49.000000 tickit-0.3.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.716578 tickit-0.3.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 14:54:49.000000 tickit-0.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-20 14:54:49.000000 tickit-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-20 14:54:49.000000 tickit-0.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 14:54:49.000000 tickit-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-07-20 14:54:59.756579 tickit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-20 14:54:49.000000 tickit-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 14:54:49.000000 tickit-0.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/framework-details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/how-component-updates-are-ordered.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/why-tickit.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/example-systems.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-create-device-amplifier.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-device-simulation-cpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-overview-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-dag.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-overview-with-system-simulation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-simulation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-system-simulation-cpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/framework-summary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/wiring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/how-to/use-command-wrappers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/how-to/use-epics-adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.736578 tickit-0.3.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/create-a-device.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/creating-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/running-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/use-composed-adapter.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.716578 tickit-0.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.736578 tickit-0.3.0/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/amplifier.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/counter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/http-and-zeromq-devices.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/http-device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/isolated-device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/nested.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/shutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/sunk-tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/sunk-trampoline.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.736578 tickit-0.3.0/examples/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/amplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/http_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/isolated_device.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/isolated_record.db
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/remote_controlled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/zeromq_push_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-20 14:54:49.000000 tickit-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:54:59.756579 tickit-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.716578 tickit-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/composed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/epicsadapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/epicsadapter/ioc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/httpadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/command/command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/command/regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/servers/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/adapters/zeromq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/zeromq/push_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/system_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/event_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/slave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/iobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/byte_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/configuration/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/configuration/tagged_union.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/topic_naming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/interpreters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/command/test_command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/command/test_regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/endpoints/test_http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/servers/test_tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/test_epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/test_epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/test_epicsadapter/test_epics_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/test_httpadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/zeromq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/zeromq/test_push_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/components/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/components/test_device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/components/test_system_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/schedulers/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/schedulers/test_master_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/schedulers/test_slave_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/test_event_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/test_ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/sim.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/state_interfaces/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/state_interfaces/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/state_interfaces/test_state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/devices/test_iobox.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/devices/test_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/devices/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/configuration/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_byte_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.030800 tickit-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.982800 tickit-0.4.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-07 14:30:13.000000 tickit-0.4.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 14:30:13.000000 tickit-0.4.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 14:30:13.000000 tickit-0.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.982800 tickit-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.970800 tickit-0.4.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.982800 tickit-0.4.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.982800 tickit-0.4.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-07 14:30:13.000000 tickit-0.4.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-07 14:30:13.000000 tickit-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-07 14:30:13.000000 tickit-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 14:30:13.000000 tickit-0.4.0/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-07 14:30:13.000000 tickit-0.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 14:30:13.000000 tickit-0.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-07 14:30:13.000000 tickit-0.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-07 14:30:13.000000 tickit-0.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 14:30:13.000000 tickit-0.4.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-07 14:30:13.000000 tickit-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 14:30:13.000000 tickit-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 14:30:13.000000 tickit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-08-07 14:30:25.030800 tickit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-08-07 14:30:13.000000 tickit-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 14:30:13.000000 tickit-0.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.986800 tickit-0.4.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/explanations/framework-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/explanations/how-component-updates-are-ordered.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/explanations/why-tickit.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.990800 tickit-0.4.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.990800 tickit-0.4.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.990800 tickit-0.4.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/example-systems.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-create-device-amplifier.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-device-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-overview-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-simple-dag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-simple-overview-with-system-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-simple-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-simple-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/images/tickit-system-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/framework-summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/system-simulation-adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/explanations/wiring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/how-to/use-epics-adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/tutorials/create-a-device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/tutorials/creating-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/tutorials/running-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-08-07 14:30:13.000000 tickit-0.4.0/docs/user/tutorials/use-command-adapter.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.974799 tickit-0.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.994800 tickit-0.4.0/examples/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/adapters/http_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/adapters/system_simulation_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/adapters/system_simulation_adapter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/adapters/zeromq_push_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.998800 tickit-0.4.0/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/amplifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/counter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/http-and-zeromq-ioboxes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/http-iobox.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/isolated-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/nested-amplifier-with-system-adapter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/shutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/sunk-tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/configs/sunk-trampoline.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.002800 tickit-0.4.0/examples/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/amplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/isolated_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/remote_controlled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-08-07 14:30:13.000000 tickit-0.4.0/examples/devices/trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-08-07 14:30:13.000000 tickit-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:30:25.030800 tickit-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:24.974799 tickit-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.002800 tickit-0.4.0/src/tickit/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.006800 tickit-0.4.0/src/tickit/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/epics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.006800 tickit-0.4.0/src/tickit/adapters/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/io/epics_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/io/http_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/io/tcp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/io/zeromq_push_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.006800 tickit-0.4.0/src/tickit/adapters/specifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/specifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/specifications/http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/specifications/regex_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/adapters/zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.006800 tickit-0.4.0/src/tickit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.010800 tickit-0.4.0/src/tickit/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/components/device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/components/system_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.010800 tickit-0.4.0/src/tickit/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/event_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.010800 tickit-0.4.0/src/tickit/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/schedulers/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/schedulers/slave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/management/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.014800 tickit-0.4.0/src/tickit/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/state_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/state_interfaces/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/state_interfaces/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/state_interfaces/state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/core/typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.014800 tickit-0.4.0/src/tickit/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/devices/iobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/devices/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/devices/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.014800 tickit-0.4.0/src/tickit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/byte_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.018800 tickit-0.4.0/src/tickit/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/configuration/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/configuration/tagged_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-07 14:30:13.000000 tickit-0.4.0/src/tickit/utils/topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.002800 tickit-0.4.0/src/tickit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 14:30:24.000000 tickit-0.4.0/src/tickit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.018800 tickit-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.018800 tickit-0.4.0/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.022800 tickit-0.4.0/tests/adapters/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/io/test_epics_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/io/test_http_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/io/test_tcp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/io/test_zeromq_push_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.022800 tickit-0.4.0/tests/adapters/specifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/specifications/test_http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/specifications/test_regex_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/test_epics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/test_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/adapters/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.022800 tickit-0.4.0/tests/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.022800 tickit-0.4.0/tests/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/components/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/components/test_device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/components/test_system_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.026800 tickit-0.4.0/tests/core/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.026800 tickit-0.4.0/tests/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/management/schedulers/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/management/schedulers/test_master_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/management/schedulers/test_slave_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/management/test_event_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/management/test_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/sim.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.026800 tickit-0.4.0/tests/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/state_interfaces/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/state_interfaces/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/state_interfaces/test_state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/core/test_typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.026800 tickit-0.4.0/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/devices/test_iobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/devices/test_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/devices/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.030800 tickit-0.4.0/tests/system_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.030800 tickit-0.4.0/tests/system_tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/system_tests/configs/nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/system_tests/configs/test_with_master.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/system_tests/test_with_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/system_tests/test_with_master_and_slave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.030800 tickit-0.4.0/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:30:25.030800 tickit-0.4.0/tests/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/utils/configuration/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/utils/test_byte_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/utils/test_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/utils/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-07 14:30:13.000000 tickit-0.4.0/tests/utils/test_topic_naming.py
```

### Comparing `tickit-0.3.0/.devcontainer/devcontainer.json` & `tickit-0.4.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.github/CONTRIBUTING.rst` & `tickit-0.4.0/.github/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ------------
 
 The code in this repository conforms to standards set by the following tools:
 
 - black_ for code formatting
 - flake8_ for style checks
 - isort_ for import ordering
-- mypy_ for static type checking
+- pyright_ for static type checking
 
 Developers guide
 ----------------
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
```

### Comparing `tickit-0.3.0/.github/actions/install_requirements/action.yml` & `tickit-0.4.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.github/dependabot.yml` & `tickit-0.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.github/pages/make_switcher.py` & `tickit-0.4.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.github/workflows/code.yml` & `tickit-0.4.0/.github/workflows/code.yml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
       - name: Install python packages
         uses: ./.github/actions/install_requirements
         with:
           requirements_file: requirements-dev-3.x.txt
           install_options: -e .[dev]
 
       - name: Lint
-        run: tox -e pre-commit,mypy
+        run: tox -e pre-commit,pyright
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
```

### Comparing `tickit-0.3.0/.github/workflows/docs.yml` & `tickit-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.github/workflows/docs_clean.yml` & `tickit-0.4.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.github/workflows/linkcheck.yml` & `tickit-0.4.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.gitignore` & `tickit-0.4.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 cov.xml
 .pytest_cache/
-.mypy_cache/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `tickit-0.3.0/.gitlab-ci.yml` & `tickit-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.vscode/launch.json` & `tickit-0.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/.vscode/settings.json` & `tickit-0.4.0/.vscode/settings.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'python.analysis.diagnosticSeverityOverrides'": "OrderedDict([('reportMissingModuleSource', "*

 * *                                                  "'none')])",*

 * * "'python.analysis.typeCheckingMode'": "'basic'",*

 * * 'delete': "['python.linting.mypyEnabled']"}*

```diff
@@ -1,17 +1,20 @@
 {
     "editor.codeActionsOnSave": {
         "source.organizeImports": true
     },
     "editor.defaultFormatter": "ms-python.python",
     "editor.formatOnSave": true,
+    "python.analysis.diagnosticSeverityOverrides": {
+        "reportMissingModuleSource": "none"
+    },
+    "python.analysis.typeCheckingMode": "basic",
     "python.formatting.provider": "black",
     "python.languageServer": "Pylance",
     "python.linting.enabled": true,
     "python.linting.flake8Enabled": true,
-    "python.linting.mypyEnabled": true,
     "python.linting.pydocstyleEnabled": true,
     "python.linting.pylintEnabled": false,
     "python.testing.pytestArgs": [],
     "python.testing.pytestEnabled": true,
     "python.testing.unittestEnabled": false
 }
```

### Comparing `tickit-0.3.0/CHANGELOG.rst` & `tickit-0.4.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/Dockerfile` & `tickit-0.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/LICENSE` & `tickit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/PKG-INFO` & `tickit-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -292,16 +292,19 @@
                 name=self.name,
                 device=CounterDevice(),
                 )
 
     class CounterDevice(Device):
         """A simple device which increments a value."""
 
-        Inputs: TypedDict = TypedDict("Inputs", {})
-        Outputs: TypedDict = TypedDict("Outputs", {"value":int})
+        class Inputs(TypedDict):
+            ...
+
+        class Outputs(TypedDict):
+            value: int
 
         def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
             self._value = initial_value
             self.callback_period = SimTime(callback_period)
             LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
```

### Comparing `tickit-0.3.0/README.rst` & `tickit-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,19 @@
                 name=self.name,
                 device=CounterDevice(),
                 )
 
     class CounterDevice(Device):
         """A simple device which increments a value."""
 
-        Inputs: TypedDict = TypedDict("Inputs", {})
-        Outputs: TypedDict = TypedDict("Outputs", {"value":int})
+        class Inputs(TypedDict):
+            ...
+
+        class Outputs(TypedDict):
+            value: int
 
         def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
             self._value = initial_value
             self.callback_period = SimTime(callback_period)
             LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
```

### Comparing `tickit-0.3.0/docs/_static/theme_overrides.css` & `tickit-0.4.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/conf.py` & `tickit-0.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 # Common links that should be available on every page
 rst_epilog = """
 .. _Diamond Light Source: http://www.diamond.ac.uk
 .. _black: https://github.com/psf/black
 .. _flake8: https://flake8.pycqa.org/en/latest/
 .. _isort: https://github.com/PyCQA/isort
-.. _mypy: http://mypy-lang.org/
+.. _pyright: https://microsoft.github.io/pyright/#/
 .. _pre-commit: https://pre-commit.com/
 """
 
 # Ignore localhost links for periodic check that links in docs are valid
 linkcheck_ignore = [r"http://localhost:\d+/"]
 
 # Set copy-button to ignore python and bash prompts
```

### Comparing `tickit-0.3.0/docs/developer/explanations/decisions.rst` & `tickit-0.4.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/explanations/framework-details.rst` & `tickit-0.4.0/docs/developer/explanations/framework-details.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/explanations/how-component-updates-are-ordered.rst` & `tickit-0.4.0/docs/developer/explanations/how-component-updates-are-ordered.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/explanations/why-tickit.rst` & `tickit-0.4.0/docs/developer/explanations/why-tickit.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/how-to/build-docs.rst` & `tickit-0.4.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/how-to/lint.rst` & `tickit-0.4.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/how-to/make-release.rst` & `tickit-0.4.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/how-to/pin-requirements.rst` & `tickit-0.4.0/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/how-to/test-container.rst` & `tickit-0.4.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/how-to/update-tools.rst` & `tickit-0.4.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/index.rst` & `tickit-0.4.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/developer/reference/standards.rst` & `tickit-0.4.0/docs/developer/reference/standards.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 --------------
 
 The code in this repository conforms to standards set by the following tools:
 
 - black_ for code formatting
 - flake8_ for style checks
 - isort_ for import ordering
-- mypy_ for static type checking
+- pyright_ for static type checking
 
 .. seealso::
 
     How-to guides `../how-to/lint` and `../how-to/static-analysis`
 
 .. _documentation_standards:
```

### Comparing `tickit-0.3.0/docs/developer/tutorials/dev-install.rst` & `tickit-0.4.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/example-systems.drawio.svg` & `tickit-0.4.0/docs/images/example-systems.drawio.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-create-device-amplifier.svg` & `tickit-0.4.0/docs/images/tickit-create-device-amplifier.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-device-simulation-cpt.svg` & `tickit-0.4.0/docs/images/tickit-device-simulation-cpt.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-logo.ico` & `tickit-0.4.0/docs/images/tickit-logo.ico`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-logo.svg` & `tickit-0.4.0/docs/images/tickit-logo.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-overview-full.svg` & `tickit-0.4.0/docs/images/tickit-overview-full.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-simple-dag.svg` & `tickit-0.4.0/docs/images/tickit-simple-dag.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-simple-overview-with-system-simulation.svg` & `tickit-0.4.0/docs/images/tickit-simple-overview-with-system-simulation.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-simple-overview.svg` & `tickit-0.4.0/docs/images/tickit-simple-overview.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-simple-simulation.svg` & `tickit-0.4.0/docs/images/tickit-simple-simulation.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/images/tickit-system-simulation-cpt.svg` & `tickit-0.4.0/docs/images/tickit-system-simulation-cpt.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/index.rst` & `tickit-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/explanations/adapters.rst` & `tickit-0.4.0/docs/user/explanations/adapters.rst`

 * *Files 24% similar despite different names*

```diff
@@ -3,51 +3,46 @@
 
 Adapters are user implemented classes associated with a device which facilitate
 interactions between that device and components external to the simulation.
 Adapters allow us to influence the device from outside the simulation, such as
 using a TCP client to alter a parameter on a device. A device may have multiple
 adapters simultaneously.
 
-There are four adapters included in the framework:
+Adapters are implemented within `AdapterContainer` and these containers are added
+to the device or system simulations. An AdapterContainer simply takes an adapter and
+an appropriate `AdapterIo`. When the container is run, it sets up the io with the 
+specific adapter.
 
-#. `Composed adapter`_
+- The Adapter contains the device specific interface for a given io type.
+- The `AdapterIo` contains IO logic which is agnositc to the details of the device.
+
+There are four adapter types included in the framework:
+
+#. `Command adapter`_
 #. `ZMQ adapter`_
 #. `HTTP adapter`_
 #. `EPICS adapter`_
 
-Composed adapter
-----------------
-The composed adapter acts to implement a server and an interpreter. It delegates
-the hosting of an external messaging protocol to a server and message handling
-to an interpreter.
-
-Tickit currently includes one server implementation, a TCP server, and one
-interpreter, the command interpreter.
-
-The command interpreter is a generic interpreter which identifies commands from
-incoming messages. Commands are defined via decoration of adapter methods and
-the only such command type currently is a `RegexCommand`. This matches incoming
-messages to regex patterns and processes the command appropriately.
-
-Tickit also includes three interpreter wrappers for the command interpreter.
-These wrap the command interpreter to allow for more complex message handling
-and can be used with the composed adapter in the same way.
 
-Users may implement their own servers and interpreters and then use the composed
-adapter to utilise them for the device.
+Command adapter
+----------------
+The command adapter identifies and handles commands from incoming messages and is 
+utilised with `TcpIo`. Commands are defined via decoration of adapter methods and the
+only such command type currently is a `RegexCommand`. This matches incoming messages to
+regex patterns and processes the command appropriately.
 
 
 ZMQ adapter
 -----------
 An adapter for use on a ZeroMQ data stream.
 
 
 HTTP adapter
 ------------
-An adapter that hosts an HTTP server, e.g. for devices with REST APIs.
+An adapter that utilises HTTP endpoints for the `HttpIo`.
 
 
 EPICS adapter
 -------------
 An adapter implementation that acts as an EPICS IOC. It utilises pythonSoftIOC
 create an IOC in the process which hosts PVs which can be linked to attributes
 on the device.
```

### Comparing `tickit-0.3.0/docs/user/explanations/components.rst` & `tickit-0.4.0/docs/user/explanations/components.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/explanations/devices.rst` & `tickit-0.4.0/docs/user/explanations/devices.rst`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 
 .. code-block:: python
 
     class RandomTrampolineDevice(Device):
     """A trivial toy device which produced a random output and requests a callback."""
 
         #: An empty typed mapping of device inputs
-        Inputs: TypedDict = TypedDict("Inputs", {})
+        class Inputs(TypedDict):
+            ...
         #: A typed mapping containing the 'output' output value
-        Outputs: TypedDict = TypedDict("Outputs", {"output": int})
+        class Outputs(TypedDict):
+            output: int
 
         def __init__(self, callback_period: int = int(1e9)) -> None:
             self.callback_period = SimTime(callback_period)
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
             """The update method which produces a random output and requests a callback.
 
@@ -41,8 +43,8 @@
                 RandomTrampolineDevice.Outputs(output=output),
                 SimTime(time + self.callback_period),
             )
 
 
 Logic can be implemented into the device via device methods. For an example of
 this look at the ``ShutterDevice``. It acts to attenuate the flux of any incoming
-value.
+value.
```

### Comparing `tickit-0.3.0/docs/user/explanations/framework-summary.rst` & `tickit-0.4.0/docs/user/explanations/framework-summary.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/explanations/glossary.rst` & `tickit-0.4.0/docs/user/explanations/glossary.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/explanations/wiring.rst` & `tickit-0.4.0/docs/user/explanations/wiring.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/how-to/use-epics-adapter.rst` & `tickit-0.4.0/docs/user/how-to/use-epics-adapter.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,36 +31,46 @@
 
         initial_gain: float = 2.5
         initial_current: float = 0.0
         db_file: str = "path/to/record.db"
         ioc_name: str = "FEMTO"
 
         def __call__(self) -> Component:  # noqa: D102
+            device=FemtoDevice(
+                initial_gain=self.initial_gain,
+                initial_current=self.initial_current,
+                )
+            adapters = [
+                AdapterContainer(
+                    FemtoAdapter(device),
+                    EpicsIo(self.ioc_name),
+                ),
+            ]
             return DeviceSimulation(
                 name=self.name,
-                device=FemtoDevice(
-                    initial_gain=self.initial_gain, initial_current=self.initial_current
-                ),
-                adapters=[FemtoAdapter(db_file=self.db_file, ioc_name=self.ioc_name)],
+                device=device,
+                adapters=adapters,
             )
 
 
 However, any PV you wish to directly link to a device attribute you must override
 and provide the necessary methods to get and set that attribute.
 
 See again the femto device. It is a signal amplifier that takes an input and
 outputs a current.
 
 .. code-block:: python
 
     class FemtoDevice(Device):
         """Electronic signal amplifier."""
 
-        Inputs: TypedDict = TypedDict("Inputs", {"input": float})
-        Outputs: TypedDict = TypedDict("Outputs", {"current": float})
+        class Inputs(TypedDict):
+            input: float
+        class Outputs(TypedDict):
+            current: float
 
         def __init__(
             self,
             initial_gain: float,
             initial_current: float,
         ) -> None:
             self.gain: float = initial_gain
@@ -104,21 +114,25 @@
 .. code-block:: python
 
     class FemtoAdapter(EpicsAdapter):
         """The adapter for the Femto device."""
 
         device: FemtoDevice
 
+        def __init__(self, device: AmplifierDevice) -> None:
+            super().__init__()
+            self.device = device
+
         async def callback(self, value) -> None:
             """Device callback function.
             Args:
                 value (float): The value to set the gain to.
             """
             self.device.set_gain(value)
-            await self.raise_interrupt()
+            await self.interrupt()
 
         def on_db_load(self) -> None:
             """Customises records that have been loaded in to suit the simulation."""
             builder.aOut(
                 "GAIN", initial_value=self.device.get_gain(), on_update=self.callback
             )
             self.link_input_on_interrupt(builder.aIn("GAIN_RBV"), self.device.get_gain)
```

### Comparing `tickit-0.3.0/docs/user/index.rst` & `tickit-0.4.0/docs/user/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -13,28 +13,27 @@
             :caption: Tutorials
             :maxdepth: 1
 
             tutorials/installation
             tutorials/running-a-simulation
             tutorials/creating-a-simulation
             tutorials/create-a-device
-            tutorials/use-composed-adapter
+            tutorials/use-command-adapter
 
         +++
 
         Tutorials for installation and typical usage. New users start here.
 
     .. grid-item-card:: :material-regular:`directions;3em`
 
         .. toctree::
             :caption: How-to Guides
             :maxdepth: 1
 
             how-to/use-epics-adapter
-            how-to/use-command-wrappers
 
         +++
 
         Practical step-by-step guides for the more experienced user.
 
     .. grid-item-card:: :material-regular:`info;3em`
 
@@ -42,14 +41,15 @@
             :caption: Explanations
             :maxdepth: 1
 
             explanations/framework-summary
             explanations/components
             explanations/devices
             explanations/adapters
+            explanations/system-simulation-adapters
             explanations/wiring
             explanations/glossary
 
         +++
 
         Explanations of how the library works and why it works that way.
```

### Comparing `tickit-0.3.0/docs/user/reference/api.rst` & `tickit-0.4.0/docs/user/reference/api.rst`

 * *Files 22% similar despite different names*

```diff
@@ -27,20 +27,15 @@
 
     .. automodule:: tickit.core.device
         :members:
 
         ``tickit.core.device``
         ----------------------
     
-    .. automodule:: tickit.core.runner
-        :members:
 
-        ``tickit.core.runner``
-        ----------------------
-    
     .. automodule:: tickit.core.typedefs
         :members:
 
         ``tickit.core.typedefs``
         ------------------------
     
 
@@ -142,116 +137,92 @@
 
 
 .. automodule:: tickit.adapters
 
     ``tickit.adapters``
     -------------------
 
-    .. automodule:: tickit.adapters.interpreters
-
-        ``tickit.adapters.interpreters``
-        --------------------------------
-
-        .. automodule:: tickit.adapters.interpreters.command
-
-            ``tickit.adapters.interpreters.command``
-            ----------------------------------------
-
-            .. automodule:: tickit.adapters.interpreters.command.command_interpreter
-                :members:
-
-                ``tickit.adapters.interpreters.command.command_interpreter``
-                ------------------------------------------------------------
-
-            .. automodule:: tickit.adapters.interpreters.command.regex_command
-                :members:
-
-                ``tickit.adapters.interpreters.command.regex_command``
-                ------------------------------------------------------
+    .. automodule:: tickit.adapters.io
 
+        ``tickit.adapters.io``
+        ----------------------
 
-        .. automodule:: tickit.adapters.interpreters.endpoints
-
-            ``tickit.adapters.interpreters.endpoints``
-            ------------------------------------------
+        .. automodule:: tickit.adapters.io.tcp_io
+            :members:
 
-            .. automodule:: tickit.adapters.interpreters.endpoints.http_endpoint
-                :members:
+            ``tickit.adapters.io.tcp_io``
+            -----------------------------
 
-                ``tickit.adapters.interpreters.endpoints.http_endpoint``
-                --------------------------------------------------------
+        .. automodule:: tickit.adapters.io.http_io
+            :members:
 
+            ``tickit.adapters.io.http_io``
+            ------------------------------
         
-        .. automodule:: tickit.adapters.interpreters.wrappers
-
-            ``tickit.adapters.interpreters.wrappers``
-            -----------------------------------------
-
-            .. automodule:: tickit.adapters.interpreters.wrappers.beheading_interpreter
-                :members:
-
-                ``tickit.adapters.interpreters.wrappers.beheading_interpreter``
-                ---------------------------------------------------------------
+        .. automodule:: tickit.adapters.io.epics_io
+            :members:
 
-            .. automodule:: tickit.adapters.interpreters.wrappers.joining_interpreter
-                :members:
+            ``tickit.adapters.io.epics_io``
+            -------------------------------
+        
+        .. automodule:: tickit.adapters.io.zeromq_push_io
+            :members:
 
-                ``tickit.adapters.interpreters.wrappers.joining_interpreter``
-                -------------------------------------------------------------
-            
-            .. automodule:: tickit.adapters.interpreters.wrappers.splitting_interpreter
-                :members:
+            ``tickit.adapters.io.zeromq_push_io``
+            -------------------------------------
+        
 
-                ``tickit.adapters.interpreters.wrappers.splitting_interpreter``
-                ---------------------------------------------------------------
+    .. automodule:: tickit.adapters.specifications
 
+        ``tickit.adapters.specifications``
+        ----------------------------------
 
-    .. automodule:: tickit.adapters.servers
+        .. automodule:: tickit.adapters.specifications.http_endpoint
+            :members:
 
-        ``tickit.adapters.servers``
-        ---------------------------
+            ``tickit.adapters.specifications.http_endpoint``
+            ------------------------------------------------
 
-        .. automodule:: tickit.adapters.servers.tcp
+        .. automodule:: tickit.adapters.specifications.regex_command
             :members:
 
-            ``tickit.adapters.servers.tcp``
-            -------------------------------
+            ``tickit.adapters.specifications.regex_command``
+            ------------------------------------------------
 
 
-    .. automodule:: tickit.adapters.composed
+    .. automodule:: tickit.adapters.epics
         :members:
         
-        ``tickit.adapters.composed``
-        ----------------------------
-
+        ``tickit.adapters.epics``
+        -------------------------
 
-    .. automodule:: tickit.adapters.httpadapter
+    .. automodule:: tickit.adapters.http
         :members:
         
-        ``tickit.adapters.httpadapter``
-        -------------------------------
-
+        ``tickit.adapters.http``
+        ------------------------
 
-    .. automodule:: tickit.adapters.zeromq.push_adapter
+    
+    .. automodule:: tickit.adapters.tcp
         :members:
         
-        ``tickit.adapters.zeromq.push_adapter``
-        ---------------------------------------
-
-
-    .. automodule:: tickit.adapters.epicsadapter
-
-        ``tickit.adapters.epicsadapter``
-        --------------------------------
-
-        .. automodule:: tickit.adapters.epicsadapter.adapter
-            :members:
+        ``tickit.adapters.tcp``
+        -----------------------
+    
+    .. automodule:: tickit.adapters.zmq
+        :members:
+        
+        ``tickit.adapters.zmq``
+        -----------------------
 
-            ``tickit.adapters.epicsadapter.adapter``
-            ----------------------------------------
+    .. automodule:: tickit.adapters.system
+        :members:
+        
+        ``tickit.adapters.system``
+        --------------------------
 
 
 
 .. automodule:: tickit.devices
 
     ``tickit.devices``
     ------------------
```

### Comparing `tickit-0.3.0/docs/user/tutorials/create-a-device.rst` & `tickit-0.4.0/docs/user/tutorials/create-a-device.rst`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 
     from tickit.core.device import Device, DeviceUpdate
     from tickit.core.typedefs import SimTime
 
 
     class AmplifierDevice(Device):
 
-    Inputs: TypedDict = TypedDict("Inputs", {})
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    class Inputs(TypedDict):
+        ...
+    class Outputs(TypedDict):
+        ...
 
     def __init__(self) -> None:
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
 
         return DeviceUpdate(self.Outputs(), None)
 
@@ -55,16 +57,18 @@
 
     from tickit.core.device import Device, DeviceUpdate
     from tickit.core.typedefs import SimTime
 
 
     class AmplifierDevice(Device):
 
-    Inputs: TypedDict = TypedDict("Inputs", {})
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    class Inputs(TypedDict):
+        ...
+    class Outputs(TypedDict):
+        ...
 
     def __init__(self, initial_amplification: float = 2) -> None:
             self.amplification = initial_amplification
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
 
         return DeviceUpdate(self.Outputs(), None)
@@ -91,16 +95,18 @@
 
     from tickit.core.device import Device, DeviceUpdate
     from tickit.core.typedefs import SimTime
 
 
     class AmplifierDevice(Device):
 
-        Inputs: TypedDict = TypedDict("Inputs", {"initial_signal":float})
-        Outputs: TypedDict = TypedDict("Outputs", {"amplified_signal":float})
+        class Inputs(TypedDict):
+            initial_signal: float
+        class Outputs(TypedDict):
+            amplified_signal: float
 
         def __init__(self, initial_amplification: float = 2.0) -> None:
             self.amplification = initial_amplification
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
             amplified_value = inputs["initial_signal"] * self.amplification
             return DeviceUpdate(self.Outputs(amplified_signal=amplified_value), None)
@@ -147,42 +153,42 @@
 
 .. code-block:: yaml
 
     - type: tickit.devices.source.Source
       name: source
       inputs: {}
       value: 10.0
-    - type: amp.Amplifier
+    - type: amplifier.Amplifier
       name: amp
       inputs:
         initial_signal:
           component: source
           port: value
       initial_amplification: 2.0
     - type: tickit.devices.sink.Sink
       name: sink
       inputs:
         input:
           component: amp
           port: amplified_signal
 
 
-Where in ``amp.Amplifier`` ``amp`` is the name of the ``.py`` file the amplifier
+Where in ``amplifier.Amplifier`` ``amplifier`` is the name of the ``.py`` file the amplifier
 is written in, and Amplifier is the name of the `ComponentConfig` for the amplifier.
 
 .. seealso::
     See the :doc:`Creating a Simulation<../tutorials/creating-a-simulation>` tutorial for a walk-through of creating simulation
     configurations.
 
 
 Finally, to run the simulation:
 
 .. code-block:: bash
 
-    python -m tickit all amp_conf.yaml
+    python -m tickit all amplifier.yaml
 
 Once run, we expect to see an output akin to:
 
 .. code-block:: bash
 
     DEBUG:asyncio:Using selector: EpollSelector
     DEBUG:tickit.core.management.ticker:Doing tick @ 0
@@ -203,8 +209,8 @@
     in a single or across multiple processes.
 
 
 Interact with the device
 ------------------------
 
 Now we have a device it is likely we want to interact with it. This can be achieved
-externally using adapters. A guide on how to do this can be found :doc:`here.<use-composed-adapter>`
+externally using adapters. A guide on how to do this can be found :doc:`here.<use-command-adapter>`
```

### Comparing `tickit-0.3.0/docs/user/tutorials/creating-a-simulation.rst` & `tickit-0.4.0/docs/user/tutorials/creating-a-simulation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/tutorials/installation.rst` & `tickit-0.4.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/tutorials/running-a-simulation.rst` & `tickit-0.4.0/docs/user/tutorials/running-a-simulation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/docs/user/tutorials/use-composed-adapter.rst` & `tickit-0.4.0/docs/user/tutorials/use-command-adapter.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,161 @@
 Using an Adapter
 ================
 
 This tutorial shows how to use a simple adapter to externally interact with a
 device in the tickit framework.
 
-We will use a `ComposedAdapter` which will act as a simple TCP interface to the
+We will use a `CommandAdapter` which will act as a simple TCP interface to the
 ``Amplifier`` device we created in the previous how-to.
 
 .. seealso::
     See the `Creating a Device` how-to for a walk-through of creating the Amplifier
     device.
 
-We will be using a composed adapter with a TCP server and the command interpreter.
 For more information on adapters see :doc:`here<../explanations/adapters>`.
 
 Initialise Adapter
 ------------------
 
-We shall begin using the same ``amp.py`` file from the ``Amplifier`` device. In
-that file add a new ``AmplifierAdapter`` class which inherits `ComposedAdapter`.
-Within ``AmplifierAdapter`` we need to assign the ``AmplifierDevice`` as a class
-member, and initialise the server and interpreter like so:
+We shall begin using the same ``amplifier.py`` file from the ``Amplifier`` device. In
+that file add a new ``AmplifierAdapter`` class which inherits `CommandAdapter`.
+
 
 .. code-block:: python
 
-    from tickit.adapters.composed import ComposedAdapter
-    from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
-    from tickit.adapters.servers.tcp import TcpServer
+    from tickit.adapters.tcp import CommandAdapter
     from tickit.utils.byte_format import ByteFormat
 
 
-    class AmplifierAdapter(ComposedAdapter):
+    class AmplifierAdapter(CommandAdapter):
         device: AmplifierDevice
 
-        def __init__(
-            self,
-            host: str = "localhost",
-            port: int = 25565,
-        ) -> None:
-            super().__init__(
-                TcpServer(host, port, ByteFormat(b"%b\r\n")),
-                CommandInterpreter(),
-            )
+        def __init__(self, device: AmplifierDevice) -> None:
+            super().__init__()
+            self.device = device
 
 
 Adapter Commands
 ----------------
 
 Now we have an adapter for our device, we need to tell it how to identify commands.
-When using the `CommandInterpreter`, commands may be registered by decorating an
-adapter method with a command register.
+Commands are registered by decorating an adapter method with a command register.
 
 We shall create two methods, one which returns the current amplification of the
 device, and another which sets a new value for the amplification.
 
 We shall begin by creating a method which returns the current value of the
 amplification. To do this we register it as a `RegexCommand` which is called by
 sending ``A?``. Since reading a device value will not alter the device state we
 shall set ``interrupt`` to ``False``. We shall also specify that the byte encoded
 message should be decoded to a string prior to matching using the ``utf-8`` standard.
 
 .. code-block:: python
 
-    from tickit.adapters.interpreters.command.regex_command import RegexCommand
+    from tickit.adapters.specifications import RegexCommand
 
-    class AmplifierAdapter(ComposedAdapter):
+    class AmplifierAdapter(CommandAdapter):
 
          ...
 
         @RegexCommand(r"A\?", False, "utf-8")
         async def get_amplification(self) -> bytes:
             return str(self.device.amplification).encode("utf-8")
 
 
 We shall now add a method which sets a new value for the amplification when
 ``A=(\d+\.?\d*)`` is received, where ``\d+\.?\d*`` denotes a decimal number and the
 parentheses form the capture group from which the argument is extracted.
 
 .. code-block:: python
 
-    class AmplifierAdapter(ComposedAdapter):
+    class AmplifierAdapter(CommandAdapter):
 
         ...
 
         @RegexCommand(r"A=(\d+\.?\d*)", True, "utf-8")
         async def set_amplification(self, amplification: float) -> None:
             self.device.amplification = amplification
 
 
-In its entirety your adapter should look as below.
+We also optionally want to have messages formatted more nicely so can set the
+``_byte_format`` to something slightly more readable. In its entirety your
+adapter should look as below.
 
 .. code-block:: python
 
-    from tickit.adapters.composed import ComposedAdapter
-    from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
-    from tickit.adapters.interpreters.command.regex_command import RegexCommand
-    from tickit.adapters.servers.tcp import TcpServer
+    from tickit.adapters.tcp import CommandAdapter
     from tickit.utils.byte_format import ByteFormat
+    from tickit.adapters.specifications import RegexCommand
 
-
-    class AmplifierAdapter(ComposedAdapter):
+    class AmplifierAdapter(CommandAdapter):
         device: AmplifierDevice
+        _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
-        def __init__(
-            self,
-            host: str = "localhost",
-            port: int = 25565,
-        ) -> None:
-            super().__init__(
-                TcpServer(host, port, ByteFormat(b"%b\r\n")),
-                CommandInterpreter(),
-            )
+        def __init__(self, device: AmplifierDevice) -> None:
+            super().__init__()
+            self.device = device
 
         @RegexCommand(r"A\?", False, "utf-8")
         async def get_amplification(self) -> bytes:
             return str(self.device.amplification).encode("utf-8")
 
         @RegexCommand(r"A=(\d+\.?\d*)", True, "utf-8")
         async def set_amplification(self, amplification: float) -> None:
             self.device.amplification = amplification
 
 
 Include the Adapter
 -------------------
 
 In order to now use this adapter to control our device we need to include it in
-our amplifier `ComponentConfig`. To do this we simply add it to the arguments of
-`DeviceSimulation`.
+our amplifier `ComponentConfig`. To do this we first construct an `AdapterContainer`
+with our ``AmplifierAdapter`` and the appropriate `AdapterIo`. In this case `TcpIo`.
+Once this is done we simply add it to the arguments of `DeviceSimulation`. 
 
 .. code-block:: python
 
     @pydantic.v1.dataclasses.dataclass
     class Amplifier(ComponentConfig):
+        """Amplifier you can set the amplification value of over TCP."""
+
         initial_amplification: int
+        host: str = "localhost"
+        port: int = 25565
 
-        def __call__(self) -> Component:
+        def __call__(self) -> Component:  # noqa: D102
+            device = AmplifierDevice(
+                initial_amplification=self.initial_amplification,
+            )
+            adapters = [
+                AdapterContainer(
+                    AmplifierAdapter(device),
+                    TcpIo(
+                        self.host,
+                        self.port,
+                    )
+            ]
             return DeviceSimulation(
                 name=self.name,
-                device=AmplifierDevice(
-                    initial_amplification=self.initial_amplification,
-                ),
-                adapters=[AmplifierAdapter()],
+                device=device,
+                adapters=adapters,
             )
 
 It is possible to add many adapters to a device, for example a composed and an epics
 adapter. To do this simply list them.
 
 
 Using the Adapter
 -----------------
 
 The simulation can be run the same as before using the yaml.
 
 .. code-block:: bash
 
-    python -m tickit all amp_conf.yaml
+    python -m tickit all amplifier.yaml
 
 Additionally, we will start a telnet client which communicates with the TcpServer of
 the adapter, this may be performed by running the following command:
 
 .. code-block:: bash
 
     telnet localhost 25565
```

### Comparing `tickit-0.3.0/examples/configs/nested.yaml` & `tickit-0.4.0/examples/configs/nested.yaml`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/examples/devices/amplifier.py` & `tickit-0.4.0/examples/devices/isolated_device.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,146 @@
+from typing import TypedDict
+
 import pydantic.v1.dataclasses
-from typing_extensions import TypedDict
+from softioc import builder
 
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
-from tickit.adapters.interpreters.command.regex_command import RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
+from tickit.adapters.epics import EpicsAdapter
+from tickit.adapters.io import EpicsIo, TcpIo
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
 
 
-class AmplifierDevice(Device):
-    """Amplifier device which multiplies an input signal by an amplification value."""
+class IsolatedBoxDevice(Device):
+    """Isolated device which stores a float value.
+
+    The device has no inputs or outputs and interacts solely through adapters.
+    """
+
+    class Inputs(TypedDict):
+        ...
 
-    Inputs: TypedDict = TypedDict("Inputs", {"initial_signal": float})
-    Outputs: TypedDict = TypedDict("Outputs", {"amplified_signal": float})
+    class Outputs(TypedDict):
+        ...
 
-    def __init__(self, initial_amplification: float = 2) -> None:
-        """Amplifier constructor which configures the initial amplification.
+    def __init__(self, initial_value: float = 2) -> None:
+        """Constructor which configures the initial value
 
         Args:
-            initial_amplification (float): The inital value of amplification of the
-                device. Defaults to 2.
+            initial_value (int): The inital value of the device. Defaults to 2.
         """
-        self.amplification = initial_amplification
+        self.value = initial_value
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-        """Update method that amplifies input signal and produces scaled output signal.
-
-        This update method multiplies the input signal by the amplification value and
-        returns a device update with this new scaled signal as an output.
+        """Update method that outputs nothing.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
-                The produced update event which contains the value of the new amplified
-                signal.
+                The produced update event which contains nothing.
         """
-        amplified_value = inputs["initial_signal"] * self.amplification
-        return DeviceUpdate(self.Outputs(amplified_signal=amplified_value), None)
+        return DeviceUpdate(self.Outputs(), None)
+
+    def get_value(self):
+        """Returns the value set for the device, required for the epics adapter."""
+        return self.value
 
+    def set_value(self, value: float):
+        """Sets the value for the device, required for the epics adapter."""
+        self.value = value
 
-class AmplifierAdapter(ComposedAdapter):
-    """A composed adapter which gets and sets the value of amplification."""
 
-    device: AmplifierDevice
+class IsolatedBoxTCPAdapter(CommandAdapter):
+    """A composed adapter which allows getting and setting the value of the device."""
+
+    device: IsolatedBoxDevice
+    _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
     def __init__(
         self,
-        host: str = "localhost",
-        port: int = 25565,
+        device: IsolatedBoxDevice,
     ) -> None:
-        """Instantiate a composed amplifier adapter with a configured TCP server.
+        super().__init__()
+        self.device = device
 
-        Args:
-            host (Optional[str]): The host address of the TcpServer. Defaults to
-                "localhost".
-            port (Optional[int]): The bound port of the TcpServer. Defaults to 25565.
+    @RegexCommand(r"v\?", False, "utf-8")
+    async def get_value(self) -> bytes:
+        """Regex string command which returns the utf-8 encoded value.
 
+        Returns:
+            bytes: The utf-8 encoded value.
         """
-        super().__init__(
-            TcpServer(host, port, ByteFormat(b"%b\r\n")),
-            CommandInterpreter(),
-        )
+        return str(self.device.value).encode("utf-8")
 
-    @RegexCommand(r"A\?", False, "utf-8")
-    async def get_amplification(self) -> bytes:
-        """Regex string command which returns the utf-8 encoded value of amplification.
+    @RegexCommand(r"v=(\d+\.?\d*)", True, "utf-8")
+    async def set_value(self, value: float) -> None:
+        """Regex string command which sets the value
 
-        Returns:
-            bytes: The utf-8 encoded value of amplification.
+        Args:
+            value (float): The desired new value.
         """
-        return str(self.device.amplification).encode("utf-8")
+        self.device.value = value
+
+
+class IsolatedBoxEpicsAdapter(EpicsAdapter):
+    """IsolatedBox adapter to allow interaction using an EPICS interface."""
+
+    device: IsolatedBoxDevice
+
+    def __init__(self, device: IsolatedBoxDevice) -> None:
+        super().__init__()
+        self.device = device
 
-    @RegexCommand(r"A=(\d+\.?\d*)", True, "utf-8")
-    async def set_amplification(self, amplification: float) -> None:
-        """Regex string command which sets the value of amplification.
+    async def callback(self, value) -> None:
+        """Device callback function.
 
         Args:
-            amplification (float): The desired value of amplification.
+            value (float): The value to set the device to.
         """
-        self.device.amplification = amplification
+        self.device.set_value(value)
+        await self.interrupt()
+
+    def on_db_load(self) -> None:
+        """Customises records that have been loaded in to suit the simulation."""
+        builder.aOut("VALUE", initial_value=self.device.value, on_update=self.callback)
+        self.link_input_on_interrupt(builder.aIn("VALUE_RBV"), self.device.get_value)
 
 
 @pydantic.v1.dataclasses.dataclass
-class Amplifier(ComponentConfig):
-    """Amplifier you can set the amplification value of over TCP."""
+class IsolatedBox(ComponentConfig):
+    """Isolated box device you can change the value of either over TCP or via EPICS."""
 
-    initial_amplification: int
+    initial_value: float
+    port: int
+    ioc_name: str
+    host: str = "localhost"
 
     def __call__(self) -> Component:  # noqa: D102
+        device = IsolatedBoxDevice(
+            initial_value=self.initial_value,
+        )
+        adapters = [
+            AdapterContainer(
+                IsolatedBoxTCPAdapter(device),
+                TcpIo(
+                    self.host,
+                    self.port,
+                ),
+            ),
+            AdapterContainer(
+                IsolatedBoxEpicsAdapter(device),
+                EpicsIo("ISOLATED_IOC"),
+            ),
+        ]
         return DeviceSimulation(
             name=self.name,
-            device=AmplifierDevice(
-                initial_amplification=self.initial_amplification,
-            ),
-            adapters=[AmplifierAdapter()],
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-0.3.0/examples/devices/counter.py` & `tickit-0.4.0/examples/devices/counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,20 @@
         return DeviceSimulation(name=self.name, device=CounterDevice())
 
 
 class CounterDevice(Device):
     """A simple device which increments a value."""
 
     #: An empty typed mapping of input values
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the 'value' output value
-    Outputs: TypedDict = TypedDict("Outputs", {"value": int})
+    class Outputs(TypedDict):
+        value: int
 
     def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
         """A constructor of the counter, which increments the input value.
 
         Args:
             initial_value (Any): The initial value of the counter.
             callback_period (int): The simulation time callback period of the device
```

### Comparing `tickit-0.3.0/examples/devices/http_device.py` & `tickit-0.4.0/examples/adapters/http_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,73 @@
 import pydantic.v1.dataclasses
 from aiohttp import web
 
-from tickit.adapters.httpadapter import HttpAdapter
-from tickit.adapters.interpreters.endpoints.http_endpoint import HttpEndpoint
+from tickit.adapters.http import HttpAdapter
+from tickit.adapters.io.http_io import HttpIo
+from tickit.adapters.specifications import HttpEndpoint
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.devices.iobox import IoBoxDevice
 
 
 class IoBoxHttpAdapter(HttpAdapter):
     """An adapter for an IoBox that allows reads and writes via REST calls"""
 
-    device: IoBoxDevice
+    io_box: IoBoxDevice
+
+    def __init__(self, io_box: IoBoxDevice) -> None:
+        self.io_box = io_box
 
     @HttpEndpoint.put("/memory/{address}", interrupt=True)
     async def write_to_address(self, request: web.Request) -> web.Response:
         """A HTTP endpoint for sending a command to the example HTTP device.
 
         Args:
             request (web.Request): [description]
 
         Returns:
             web.Response: [description]
         """
         address = request.match_info["address"]
         new_value = (await request.json())["value"]
-        self.device.write(address, new_value)
+        self.io_box.write(address, new_value)
         return web.json_response({address: new_value})
 
     @HttpEndpoint.get("/memory/{address}")
     async def read_from_address(self, request: web.Request) -> web.Response:
         """A HTTP endpoint for requesting data from the example HTTP device.
 
         Args:
             request (web.Request): [description]
 
         Returns:
             web.Response: [description]
         """
         address = request.match_info["address"]
-        value = self.device.read(address)
+        value = self.io_box.read(address)
         return web.json_response({address: value})
 
 
 @pydantic.v1.dataclasses.dataclass
-class ExampleHTTPDevice(ComponentConfig):
+class ExampleHttpDevice(ComponentConfig):
     """Example HTTP device."""
 
     host: str = "localhost"
     port: int = 8080
 
     def __call__(self) -> Component:  # noqa: D102
+        device = IoBoxDevice()
+        adapters = [
+            AdapterContainer(
+                IoBoxHttpAdapter(device),
+                HttpIo(
+                    self.host,
+                    self.port,
+                ),
+            )
+        ]
         return DeviceSimulation(
             name=self.name,
-            device=IoBoxDevice(),
-            adapters=[IoBoxHttpAdapter(self.host, self.port)],
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-0.3.0/examples/devices/remote_controlled.py` & `tickit-0.4.0/examples/devices/remote_controlled.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import asyncio
 import logging
 import struct
 from typing import AsyncIterable, Optional, TypedDict
 
 import pydantic.v1.dataclasses
 
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
-from tickit.core.adapter import Server
+from tickit.adapters.io.tcp_io import TcpIo
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
 
 LOGGER = logging.getLogger(__name__)
 
 
 class RemoteControlledDevice(Device):
     """A trivial toy device which is controlled by an adapter."""
 
     #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the 'observed' output value
-    Outputs: TypedDict = TypedDict("Outputs", {"observed": float})
+    class Outputs(TypedDict):
+        observed: float
 
     def __init__(
         self,
         initial_observed: float = 0,
         initial_unobserved: float = 42,
         initial_hidden: float = 3.14,
     ) -> None:
@@ -57,36 +60,24 @@
             DeviceUpdate[Outputs]:
                 The produced update event which contains the observed value, the device
                 never requests a callback.
         """
         return DeviceUpdate(self.Outputs(observed=self.observed), None)
 
 
-class RemoteControlledAdapter(ComposedAdapter[bytes]):
+class RemoteControlledAdapter(CommandAdapter):
     """A trivial composed adapter which gets and sets device properties."""
 
     device: RemoteControlledDevice
+    _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
-    def __init__(
-        self,
-        server: Server,
-    ) -> None:
-        """A constructor of the Shutter adapter, which builds the configured server.
-
-        Args:
-            device (Device): The device which this adapter is attached to.
-            raise_interrupt (Callable): A callback to request that the device is
-                updated immediately.
-            server (Server): The immutable data container used to configure a
-                server.
-        """
-        super().__init__(
-            server,
-            CommandInterpreter(),
-        )
+    def __init__(self, device: RemoteControlledDevice, format: ByteFormat) -> None:
+        super().__init__()
+        self.device = device
+        self._byte_format = format
 
     async def on_connect(self) -> AsyncIterable[Optional[bytes]]:
         """Continiously sends the unobserved value to the client.
 
         Returns:
             AsyncIterable[bytes]:
                 An asynchronous iterable which regularly outputs the unobserved value.
@@ -223,15 +214,28 @@
             yield f"Observed is {self.device.observed}".encode("utf-8")
 
 
 @pydantic.v1.dataclasses.dataclass
 class RemoteControlled(ComponentConfig):
     """Thing you can poke over TCP."""
 
-    format: ByteFormat = ByteFormat(b"%b\r\n")
+    format: ByteFormat
 
     def __call__(self) -> Component:  # noqa: D102
+        device = RemoteControlledDevice()
+        adapters = [
+            AdapterContainer(
+                RemoteControlledAdapter(
+                    device,
+                    format=self.format,
+                ),
+                TcpIo(
+                    host="localhost",
+                    port=25565,
+                ),
+            )
+        ]
         return DeviceSimulation(
             name=self.name,
-            device=RemoteControlledDevice(),
-            adapters=[RemoteControlledAdapter(TcpServer())],
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-0.3.0/examples/devices/shutter.py` & `tickit-0.4.0/examples/devices/shutter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from random import random
 from typing import Optional, TypedDict
 
 import pydantic.v1.dataclasses
 
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
-from tickit.adapters.interpreters.command.regex_command import RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
+from tickit.adapters.io.tcp_io import TcpIo
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
 
 
@@ -20,17 +20,20 @@
     A toy device which produces an output flux which is downscaled from the input flux
     according to an internal state position. The position may be altered by setting new
     a target which will be matched by position over a period of time determined by the
     rate.
     """
 
     #: A typed mapping containing the 'flux' input value
-    Inputs: TypedDict = TypedDict("Inputs", {"flux": float})
+    class Inputs(TypedDict):
+        flux: float
+
     #: A typed mapping containing the 'flux' output value
-    Outputs: TypedDict = TypedDict("Outputs", {"flux": float})
+    class Outputs(TypedDict):
+        flux: float
 
     def __init__(
         self, default_position: float, initial_position: Optional[float] = None
     ) -> None:
         """A Shutter constructor which configures the initial and default position.
 
         Args:
@@ -96,38 +99,24 @@
         call_at = (
             None if self.position == self.target_position else SimTime(time + int(1e8))
         )
         output_flux = inputs["flux"] * self.position
         return DeviceUpdate(self.Outputs(flux=output_flux), call_at)
 
 
-class ShutterAdapter(ComposedAdapter):
+class ShutterAdapter(CommandAdapter):
     """A toy composed adapter which gets shutter position and target and sets target."""
 
     device: ShutterDevice
 
-    def __init__(
-        self,
-        host: str = "localhost",
-        port: int = 25565,
-    ) -> None:
-        """A Shutter which instantiates a TcpServer with configured host and port.
+    _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
-        Args:
-            device (Device): The device which this adapter is attached to
-            raise_interrupt (Callable): A callback to request that the device is
-                updated immediately.
-            host (Optional[str]): The host address of the TcpServer. Defaults to
-                "localhost".
-            port (Optional[int]): The bound port of the TcpServer. Defaults to 25565.
-        """
-        super().__init__(
-            TcpServer(host, port, ByteFormat(b"%b\r\n")),
-            CommandInterpreter(),
-        )
+    def __init__(self, device: ShutterDevice) -> None:
+        super().__init__()
+        self.device = device
 
     @RegexCommand(r"P\?", False, "utf-8")
     async def get_position(self) -> bytes:
         """A regex string command which returns the utf-8 encoded value of position.
 
         Returns:
             bytes: The utf-8 encoded value of position.
@@ -160,15 +149,25 @@
 
     default_position: float
     initial_position: Optional[float] = None
     host: str = "localhost"
     port: int = 25565
 
     def __call__(self) -> Component:  # noqa: D102
+        device = ShutterDevice(
+            default_position=self.default_position,
+            initial_position=self.initial_position,
+        )
+        adapters = [
+            AdapterContainer(
+                ShutterAdapter(device),
+                TcpIo(
+                    self.host,
+                    self.port,
+                ),
+            )
+        ]
         return DeviceSimulation(
             name=self.name,
-            device=ShutterDevice(
-                default_position=self.default_position,
-                initial_position=self.initial_position,
-            ),
-            adapters=[ShutterAdapter(host=self.host, port=self.port)],
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-0.3.0/examples/devices/trampoline.py` & `tickit-0.4.0/examples/devices/trampoline.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class TrampolineDevice(Device):
     """A trivial toy device which requests a callback every update."""
 
     #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: An empty typed mapping of device outputs
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    class Outputs(TypedDict):
+        ...
 
     def __init__(self, callback_period: int = int(1e9)) -> None:
         """A constructor of the sink which configures the device callback period.
 
         Args:
             callback_period (int): The simulation time callback period of the device
                 (in nanoseconds). Defaults to int(1e9).
@@ -51,17 +54,20 @@
         )
 
 
 class RandomTrampolineDevice(Device):
     """A trivial toy device which produced a random output and requests a callback."""
 
     #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the 'output' output value
-    Outputs: TypedDict = TypedDict("Outputs", {"output": int})
+    class Outputs(TypedDict):
+        output: int
 
     def __init__(self, callback_period: int = int(1e9)) -> None:
         """A constructor of the sink which configures the device callback period.
 
         Args:
             callback_period (int): The simulation time callback period of the device
                 (in nanoseconds). Defaults to int(1e9).
```

### Comparing `tickit-0.3.0/examples/devices/zeromq_push_device.py` & `tickit-0.4.0/examples/adapters/zeromq_push_adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,61 @@
+import asyncio
 from dataclasses import field
 from typing import Optional, Set
 
 import pydantic.v1.dataclasses
 
-from tickit.adapters.zeromq.push_adapter import (
-    SocketFactory,
-    ZeroMqPushAdapter,
-    create_zmq_push_socket,
-)
+from tickit.adapters.io.zeromq_push_io import ZeroMqPushIo, create_zmq_push_socket
+from tickit.adapters.zmq import ZeroMqPushAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.devices.iobox import IoBoxDevice
 
 
 class IoBoxZeroMqAdapter(ZeroMqPushAdapter):
-    """An Eiger adapter which parses the commands sent to the HTTP server."""
+    """An ZMQ adapter which publishes writes to the devices memory."""
 
     device: IoBoxDevice[str, int]
     _addresses_to_publish: Set[str]
+    _message_queue: asyncio.Queue
 
     def __init__(
         self,
-        host: str = "127.0.0.1",
-        port: int = 5555,
-        socket_factory: Optional[SocketFactory] = create_zmq_push_socket,
+        device: IoBoxDevice,
         addresses_to_publish: Optional[Set[str]] = None,
     ) -> None:
-        super().__init__(host, port, socket_factory)
+        self.device = device
         self._addresses_to_publish = addresses_to_publish or set()
+        self._message_queue = asyncio.Queue()
 
-    def after_update(self):
+    def after_update(self) -> None:
         for address in self._addresses_to_publish:
             value = self.device.read(address)
-            self.send_message([{address: value}])
+            self.add_message_to_stream([{address: value}])
 
 
 @pydantic.v1.dataclasses.dataclass
 class ExampleZeroMqPusher(ComponentConfig):
     """Device that can publish writes to its memory over a zeromq socket."""
 
     host: str = "127.0.0.1"
     port: int = 5555
     addresses_to_publish: Set[str] = field(default_factory=lambda: {"foo", "bar"})
 
     def __call__(self) -> Component:  # noqa: D102
+        device = IoBoxDevice()
+        adapters = [
+            AdapterContainer(
+                IoBoxZeroMqAdapter(device),
+                ZeroMqPushIo(
+                    self.host,
+                    self.port,
+                    socket_factory=create_zmq_push_socket,
+                ),
+            ),
+        ]
         return DeviceSimulation(
             name=self.name,
-            device=IoBoxDevice(),
-            adapters=[IoBoxZeroMqAdapter()],
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-0.3.0/pyproject.toml` & `tickit-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,33 +17,32 @@
     "aiozmq",
     "immutables",
     "pydantic>=2.0",
     "pyyaml",
     "pyzmq",
     "softioc",
     "typing_extensions",
-    "click==8.1.3",
+    "click!=8.1.4,!=8.1.5", #https://github.com/pallets/click/issues/2558
 
 ] # Add project dependencies here, e.g. ["click", "numpy"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "black",
-    "mypy",
+    "pyright",
     "flake8-isort",
     "Flake8-pyproject",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "pytest-cov",
-    "pytest-mypy",
     "pytest-flake8",
     "pytest-black",
     "pytest-asyncio",
     "pytest-pydocstyle",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
@@ -64,16 +63,16 @@
 email = "callum.forrester@diamond.ac.uk"
 name = "Callum Forrester"
 
 
 [tool.setuptools_scm]
 write_to = "src/tickit/_version.py"
 
-[tool.mypy]
-ignore_missing_imports = true # Ignore missing stubs in imported modules
+[tool.pyright]
+reportMissingImports = false # Ignore missing stubs in imported modules
 
 [tool.isort]
 float_to_top = true
 profile = "black"
 skip=["setup.py","conf.py","build"]
 
 [tool.flake8]
@@ -118,23 +117,23 @@
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
 
-[testenv:{pre-commit,mypy,pytest,docs}]
+[testenv:{pre-commit,pyright,pytest,docs}]
 # Don't create a virtualenv for the command, requires tox-direct plugin
 direct = True
 passenv = *
 allowlist_externals =
     pytest
     pre-commit
-    mypy
+    pyright
     sphinx-build
     sphinx-autobuild
 commands =
     pytest: pytest {posargs}
-    mypy: mypy src tests {posargs}
+    pyright: pyright src tests {posargs}
     pre-commit: pre-commit run --all-files {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
```

### Comparing `tickit-0.3.0/src/tickit/adapters/epicsadapter/adapter.py` & `tickit-0.4.0/src/tickit/adapters/epics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,78 @@
-import os
-import re
+import asyncio
+import itertools
+import logging
 from abc import abstractmethod
 from dataclasses import dataclass
-from tempfile import NamedTemporaryFile
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Set
 
-from softioc import builder, softioc
+from softioc import asyncio_dispatcher, builder, softioc
 
-from tickit.core.adapter import Adapter, RaiseInterrupt
-from tickit.core.device import Device
+from tickit.core.adapter import RaiseInterrupt
 
-from .ioc_manager import notify_adapter_ready, register_adapter
+LOGGER = logging.getLogger(__name__)
+
+#: Name for the global Tickit IOC, will prefix some meta PVs.
+_TICKIT_IOC_NAME: str = "TICKIT_IOC"
+
+#: Ids of all adapters currently registered but not ready.
+_REGISTERED_ADAPTER_IDS: Set[int] = set()
+
+#: Iterator of unique IDs for new adapters
+_ID_COUNTER: itertools.count = itertools.count()
+
+
+def register_adapter() -> int:
+    """Register a new adapter that may be creating records for the process-wide IOC.
+
+    The IOC will not be initialized until all registered adapters have notified that
+    they are ready.
+
+    Returns:
+        int: A unique ID for this adapter to use when notifying that it is ready.
+    """
+    adapter_id = next(_ID_COUNTER)
+    LOGGER.debug(f"New IOC adapter registering with ID: {adapter_id}")
+    _REGISTERED_ADAPTER_IDS.add(adapter_id)
+    return adapter_id
+
+
+def notify_adapter_ready(adapter_id: int) -> None:
+    """Notify the builder that a particular adapter has made all the records it needs.
+
+    Once all registered adapters have notified, the IOC will start.
+
+    Args:
+        adapter_id (int): Unique ID of the adapter
+    """
+    _REGISTERED_ADAPTER_IDS.remove(adapter_id)
+    LOGGER.debug(f"IOC adapter #{adapter_id} reports ready")
+    if not _REGISTERED_ADAPTER_IDS:
+        LOGGER.debug("All registered adapters are ready, starting IOC")
+        _build_and_run_ioc()
+
+
+def _build_and_run_ioc() -> None:
+    """Build an EPICS python soft IOC for the adapter."""
+    LOGGER.debug("Initializing database")
+
+    # Records become immutable after this point
+    builder.SetDeviceName(_TICKIT_IOC_NAME)
+    softioc.devIocStats(_TICKIT_IOC_NAME)
+    builder.LoadDatabase()
+
+    LOGGER.debug("Starting IOC")
+    event_loop = asyncio.get_event_loop()
+    dispatcher = asyncio_dispatcher.AsyncioDispatcher(event_loop)
+    softioc.iocInit(dispatcher)
+    # dbl directly prints out all record names, so we have to check
+    # the log level in order to only do it in DEBUG.
+    if LOGGER.level <= logging.DEBUG:
+        softioc.dbl()  # type: ignore
+    LOGGER.debug("IOC started")
 
 
 @dataclass(frozen=True)
 class InputRecord:
     """A data container representing an EPICS input record."""
 
     name: str
@@ -25,71 +83,35 @@
 @dataclass
 class OutputRecord:
     """A data container representing an EPICS output record."""
 
     name: str
 
 
-class EpicsAdapter(Adapter):
-    """An adapter implementation which acts as an EPICS IOC.
-
-    This is optionally initialised from an EPICS database (db) file
-    but can be customised in code by implementing on_db_load.
-    """
-
-    def __init__(self, ioc_name: str, db_file: Optional[str] = None) -> None:
-        """An EpicsAdapter constructor which stores the db_file path and the IOC name.
+class EpicsAdapter:
+    """An adapter interface for the EpicsIo."""
 
-        Args:
-            ioc_name (str): The name of the EPICS IOC.
-            db_file (str, optional): The path to the db_file.
-        """
-        self.db_file = db_file
-        self.ioc_name = ioc_name
-        self.interrupt_records: Dict[InputRecord, Callable[[], Any]] = {}
-        self.ioc_num = register_adapter()
+    interrupt_records: Dict[InputRecord, Callable[[], Any]] = {}
+    interrupt: RaiseInterrupt
 
     def link_input_on_interrupt(
         self, record: InputRecord, getter: Callable[[], Any]
     ) -> None:
         """Adds a record and a getter to the mapping of interrupting records.
 
         Args:
             record (InputRecord): The record to be added.
             getter (Callable[[], Any]): The getter handle.
         """
         self.interrupt_records[record] = getter
 
+    @abstractmethod
+    def on_db_load(self) -> None:
+        """Customises records that have been loaded in to suit the simulation."""
+        raise NotImplementedError
+
     def after_update(self) -> None:
         """Updates IOC records immediately following a device update."""
         for record, getter in self.interrupt_records.items():
             current_value = getter()
             record.set(current_value)
             print(f"Record {record.name} updated to : {current_value}")
-
-    @abstractmethod
-    def on_db_load(self) -> None:
-        """Customises records that have been loaded in to suit the simulation."""
-        raise NotImplementedError
-
-    def load_records_without_DTYP_fields(self):
-        """Load records from database file without DTYP fields."""
-        with open(self.db_file, "rb") as inp:
-            with NamedTemporaryFile(suffix=".db", delete=False) as out:
-                for line in inp.readlines():
-                    if not re.match(rb"\s*field\s*\(\s*DTYP", line):
-                        out.write(line)
-
-        softioc.dbLoadDatabase(out.name, substitutions=f"device={self.ioc_name}")
-        os.unlink(out.name)
-
-    async def run_forever(
-        self, device: Device, raise_interrupt: RaiseInterrupt
-    ) -> None:
-        """Runs the server continuously."""
-        await super().run_forever(device, raise_interrupt)
-        builder.SetDeviceName(self.ioc_name)
-        if self.db_file:
-            self.load_records_without_DTYP_fields()
-        self.on_db_load()
-        builder.UnsetDevice()
-        notify_adapter_ready(self.ioc_num)
```

### Comparing `tickit-0.3.0/src/tickit/adapters/httpadapter.py` & `tickit-0.4.0/src/tickit/adapters/io/http_io.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import asyncio
 import logging
-from dataclasses import dataclass
-from inspect import getmembers
-from typing import Awaitable, Callable, Iterable, Optional
+from typing import Awaitable, Callable, Iterable, Optional, Tuple
 
 from aiohttp import web
 from aiohttp.web_routedef import RouteDef
 
-from tickit.adapters.interpreters.endpoints.http_endpoint import HttpEndpoint
-from tickit.core.adapter import Adapter, RaiseInterrupt
-from tickit.core.device import Device
+from tickit.adapters.http import HttpAdapter
+from tickit.adapters.specifications import HttpEndpoint
+from tickit.core.adapter import AdapterIo, RaiseInterrupt
 
 LOGGER = logging.getLogger(__name__)
 
 
-@dataclass
-class HttpAdapter(Adapter):
-    """An adapter implementation which delegates to a server and sets up endpoints.
+class HttpIo(AdapterIo[HttpAdapter]):
+    """An AdapterIo implementation which delegates to a server and sets up endpoints.
 
-    An adapter implementation which delegates the hosting of an http requests to a
-    server and sets up the endpoints for said server.
+    An AdapterIo implementation which delegates the hosting of an http requests to a
+    server and sets up the endpoints for said server from a HttpAdapter.
     """
 
-    host: str = "localhost"
-    port: int = 8080
+    host: str
+    port: int
 
-    _stopped: Optional[asyncio.Event] = None
-    _ready: Optional[asyncio.Event] = None
+    _stopped: Optional[asyncio.Event]
+    _ready: Optional[asyncio.Event]
 
-    async def run_forever(
-        self, device: Device, raise_interrupt: RaiseInterrupt
+    def __init__(
+        self,
+        host: str = "localhost",
+        port: int = 8080,
     ) -> None:
-        """Runs the server continuously."""
-        await super().run_forever(device, raise_interrupt)
+        self.host = host
+        self.port = port
+        self._stopped = None
+        self._ready = None
 
+    async def setup(
+        self, adapter: HttpAdapter, raise_interrupt: RaiseInterrupt
+    ) -> None:
         self._ensure_stopped_event().clear()
-        await self._start_server()
+        endpoints = adapter.get_endpoints()
+        await self._start_server(endpoints, raise_interrupt)
         self._ensure_ready_event().set()
         try:
             await self._ensure_stopped_event().wait()
         except asyncio.CancelledError:
             await self.stop()
 
     async def wait_until_ready(self, timeout: float = 1.0) -> None:
@@ -63,41 +68,37 @@
         return self._stopped
 
     def _ensure_ready_event(self) -> asyncio.Event:
         if self._ready is None:
             self._ready = asyncio.Event()
         return self._ready
 
-    async def _start_server(self):
+    async def _start_server(
+        self,
+        endpoints: Iterable[Tuple[HttpEndpoint, Callable]],
+        raise_interrupt: RaiseInterrupt,
+    ):
         LOGGER.debug(f"Starting HTTP server... {self}")
         self.app = web.Application()
-        self.app.add_routes(list(self.endpoints()))
+        definitions = self.create_route_definitions(endpoints, raise_interrupt)
+        self.app.add_routes(list(definitions))
         runner = web.AppRunner(self.app)
         await runner.setup()
         self.site = web.TCPSite(runner, host=self.host, port=self.port)
         await self.site.start()
 
-    def endpoints(self) -> Iterable[RouteDef]:
-        """Returns list of endpoints.
-
-        Fetches the defined HTTP endpoints in the device adapter, parses them and
-        then yields them.
-
-        Returns:
-            Iterable[HttpEndpoint]: The list of defined endpoints
-
-        Yields:
-            Iterator[Iterable[HttpEndpoint]]: The iterator of the defined endpoints
-        """
-        for _, func in getmembers(self):
-            endpoint = getattr(func, "__endpoint__", None)  # type: ignore
-            if endpoint is not None and isinstance(endpoint, HttpEndpoint):
-                if endpoint.interrupt:
-                    func = _with_posthoc_task(func, self.raise_interrupt)
-                yield endpoint.define(func)
+    def create_route_definitions(
+        self,
+        endpoints: Iterable[Tuple[HttpEndpoint, Callable]],
+        raise_interrupt: RaiseInterrupt,
+    ) -> Iterable[RouteDef]:
+        for endpoint, func in endpoints:
+            if endpoint.interrupt:
+                func = _with_posthoc_task(func, raise_interrupt)
+            yield endpoint.define(func)
 
 
 def _with_posthoc_task(
     func: Callable[[web.Request], Awaitable[web.Response]],
     afterwards: Callable[[], Awaitable[None]],
 ) -> Callable[[web.Request], Awaitable[web.Response]]:
     # @functools.wraps
```

### Comparing `tickit-0.3.0/src/tickit/adapters/interpreters/command/command_interpreter.py` & `tickit-0.4.0/src/tickit/adapters/tcp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from abc import abstractmethod
 from inspect import getmembers
 from typing import (
     AnyStr,
     AsyncIterable,
+    AsyncIterator,
     Optional,
     Protocol,
     Sequence,
     Tuple,
     get_type_hints,
     runtime_checkable,
 )
 
-from tickit.adapters.interpreters.utils import wrap_as_async_iterable
-from tickit.core.adapter import Adapter, Interpreter
+from tickit.adapters.utils import wrap_as_async_iterator
+from tickit.core.adapter import Interpreter, RaiseInterrupt
+from tickit.utils.byte_format import ByteFormat
 
 
 @runtime_checkable
 class Command(Protocol):
     """An interface for interpretable commands."""
 
     #: A flag which indicates whether calling of the method should trigger an interrupt
@@ -36,63 +38,94 @@
             Optional[Sequence[AnyStr]]:
                 A sequence of arguments extracted from the message if matched,
                 otherwise None.
         """
         pass
 
 
-class CommandInterpreter(Interpreter[AnyStr]):
-    """An interpreter which routes to commands registered to adapter methods.
+class CommandAdapter(Interpreter[AnyStr]):
+    """An adapter which routes to commands registered to adapter methods.
 
-    An interpreter which attempts to parse messages according to the parse method of
+    An adapter which attempts to parse messages according to the parse method of
     commands registered against adapter methods, if a match is found the method is
     called with the parsed arguments.
     """
 
-    @staticmethod
-    async def unknown_command() -> AsyncIterable[bytes]:
-        """An asynchronous iterable of containing a single unknown command reply.
+    _byte_format: ByteFormat = ByteFormat(b"%b")
+
+    @property
+    def byte_format(self) -> ByteFormat:
+        return self._byte_format
+
+    def after_update(self) -> None:
+        ...
+
+    async def handle_message(
+        self,
+        message: AnyStr,
+        raise_interrupt: RaiseInterrupt,
+    ) -> AsyncIterable[Optional[AnyStr]]:
+        """Delegates message handling to the adapter, raises interrupt if requested.
+
+        Args:
+            message (T): The message from the server to be handled.
 
         Returns:
-            AsyncIterable[bytes]:
-                An asynchronous iterable of containing a single unknown command reply:
-                "Request does not match any known command".
+            AsyncIterable[Optional[T]]: An asynchronous iterable of reply messages.
         """
-        yield b"Request does not match any known command"
+        reply, interrupt = await self.handle(message)
+        if interrupt:
+            await raise_interrupt()
+        return reply
 
-    async def handle(
-        self, adapter: Adapter, message: AnyStr
-    ) -> Tuple[AsyncIterable[AnyStr], bool]:
+    async def handle(self, message: AnyStr) -> Tuple[AsyncIterator[AnyStr], bool]:
         """Matches the message to an adapter command and calls the corresponding method.
 
         An asynchronous method which handles a message by attempting to match the
         message against each of the registered commands, if a match is found the
         corresponding command is called and its reply is returned with an asynchronous
-        iterable wrapper if required. If no match is found the unknown command message
+        iterator wrapper if required. If no match is found the unknown command message
         is returned with no request for interrupt.
 
         Args:
             adapter (Adapter): The adapter in which the function should be executed
             message (bytes): The message to be handled.
 
         Returns:
-            Tuple[AsyncIterable[Union[str, bytes]], bool]:
-                A tuple of the asynchronous iterable of reply messages and a flag
+            Tuple[AsyncIterator[Union[str, bytes]], bool]:
+                A tuple of the asynchronous iterator of reply messages and a flag
                 indicating whether an interrupt should be raised by the adapter.
         """
-        for _, method in getmembers(adapter):
+        for _, method in getmembers(self):
             command = getattr(method, "__command__", None)
             if command is None:
                 continue
             args = command.parse(message)
             if args is None:
                 continue
             args = (
                 argtype(arg)
                 for arg, argtype in zip(args, get_type_hints(method).values())
             )
             resp = await method(*args)
-            if not isinstance(resp, AsyncIterable):
-                resp = wrap_as_async_iterable(resp)
+            if not isinstance(resp, AsyncIterator):
+                resp = wrap_as_async_iterator(resp)
             return resp, command.interrupt
-        resp = CommandInterpreter.unknown_command()
-        return resp, False
+
+        msg = "Request does not match any known command"
+        # This is a pain but the message needs to match the input message
+        # TODO: Fix command interpreters' handling of bytes vs str
+        if isinstance(message, bytes):
+            resp = wrap_as_async_iterator(msg.encode("utf-8"))
+            return resp, False
+        else:
+            resp = wrap_as_async_iterator(msg)
+            return resp, False
+
+    async def on_connect(self) -> AsyncIterable[Optional[AnyStr]]:
+        """Overridable asynchronous iterable which yields messages on client connection.
+
+        Returns:
+            AsyncIterable[Optional[T]]: An asynchronous iterable of messages.
+        """
+        if False:
+            yield None
```

### Comparing `tickit-0.3.0/src/tickit/adapters/interpreters/command/regex_command.py` & `tickit-0.4.0/src/tickit/adapters/specifications/regex_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import re
-from dataclasses import dataclass
+from dataclasses import InitVar, dataclass, field
+from re import Pattern, compile
 from typing import AnyStr, Callable, Generic, Optional, Sequence
 
 
-@dataclass(frozen=True)
+@dataclass
 class RegexCommand(Generic[AnyStr]):
     """A decorator to register an adapter method as a regex parsed command.
 
     Args:
         regex (Union[bytes, str]): The regular expression pattern which must be
             matched in full, with groups used to extract command arguments.
         interrupt (bool): A flag indicating whether calling of the method should
@@ -16,17 +16,34 @@
             based interpretation. Defaults to None.
 
     Returns:
         Callable:
             A decorator which registers the adapter method as a message handler.
     """
 
-    regex: AnyStr
+    regex: InitVar[AnyStr]
     interrupt: bool = False
-    format: Optional[str] = None
+    format: InitVar[Optional[str]] = None
+    pattern: Pattern[AnyStr] = field(init=False)
+    convert: Callable[[bytes], AnyStr] = field(init=False)
+
+    def __post_init__(self, regex: AnyStr, format: Optional[str]):
+        # The type checking fails here as it can't determine that the return
+        # type matches the regex type. The isinstance should narrow the AnyStr
+        # type but doesn't
+        if isinstance(regex, str):
+            if format is None:
+                raise ValueError(
+                    "If regex is a string, format is required to decode input"
+                )
+            self.convert = lambda b: b.decode(format).strip()  # type: ignore
+        else:
+            self.convert = lambda b: b  # type: ignore
+
+        self.pattern = compile(regex)
 
     def __call__(self, func: Callable) -> Callable:
         """A decorator which registers the adapter method as a message handler.
 
         Args:
             func (Callable): The adapter method to be registered as a command.
 
@@ -47,13 +64,12 @@
             data (bytes): The message data to be parsed.
 
         Returns:
             Optional[Sequence[AnyStr]]:
                 If a full match is found a sequence of function arguments is returned,
                 otherwise the method returns None.
         """
-        message = data.decode(self.format, "ignore").strip() if self.format else data
-        if isinstance(message, type(self.regex)):
-            match = re.fullmatch(self.regex, message)
-            if match:
-                return match.groups()
+        message = self.convert(data)
+        match = self.pattern.fullmatch(message)
+        if match:
+            return match.groups()
         return None
```

### Comparing `tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/http_endpoint.py` & `tickit-0.4.0/src/tickit/adapters/specifications/http_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import AnyStr, Awaitable, Callable, Generic
+from typing import AnyStr, Awaitable, Callable, Generic, Optional
 
 from aiohttp import web
 from aiohttp.web_response import StreamResponse
 from aiohttp.web_routedef import RouteDef
 
 
 @dataclass(frozen=True)
@@ -22,17 +22,16 @@
         Callable:
             A decorator which registers the adapter method as an endpoint.
     """
 
     path: str
     method: str
     interrupt: bool = False
+    func: Optional[Callable[[web.Request], web.Response]] = None
 
-    # Type signature can become more specific if support is dropped for
-    # Python 3.7, see https://github.com/python/mypy/issues/708
     def __call__(self, func: Callable) -> Callable:
         """Decorate a function for HTTP routing.
 
         Args:
             func: The adapter method to be registered as an endpoint.
 
         Returns:
```

### Comparing `tickit-0.3.0/src/tickit/adapters/interpreters/utils.py` & `tickit-0.4.0/src/tickit/adapters/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import AnyStr, AsyncIterable, Iterable
+from collections.abc import AsyncIterator
+from typing import AnyStr, Iterable
 
 
-async def wrap_as_async_iterable(message: AnyStr) -> AsyncIterable[AnyStr]:
-    """Wraps a message in an asynchronous iterable.
+async def wrap_as_async_iterator(message: AnyStr) -> AsyncIterator[AnyStr]:
+    """Wraps a message in an asynchronous iterator.
 
     Args:
         message (AnyStr): A singular message.
 
     Returns:
-        AsyncIterable[AnyStr]: An asynchronous iterable containing the message.
+        AsyncIterator[AnyStr]: An asynchronous iterator containing the message.
     """
     yield message
 
 
-async def wrap_messages_as_async_iterable(
+async def wrap_messages_as_async_iterator(
     messages: Iterable[AnyStr],
-) -> AsyncIterable[AnyStr]:
-    """Wraps a message in an asynchronous iterable.
+) -> AsyncIterator[AnyStr]:
+    """Wraps a message in an asynchronous iterator.
 
     Args:
         message (AnyStr): An iterable containing a number of messages.
 
     Returns:
-        AsyncIterable[AnyStr]: An asynchronous iterable containing the messages.
+        AsyncIterator[AnyStr]: An asynchronous iterator containing the messages.
     """
     for message in messages:
         yield message
```

### Comparing `tickit-0.3.0/src/tickit/adapters/servers/tcp.py` & `tickit-0.4.0/src/tickit/adapters/io/tcp_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 import asyncio
 import logging
 from asyncio.streams import StreamReader, StreamWriter
 from typing import AsyncIterable, Awaitable, Callable, List, Optional
 
-from tickit.core.adapter import Server
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterIo, RaiseInterrupt
 from tickit.utils.byte_format import ByteFormat
 
 LOGGER = logging.getLogger(__name__)
 
 
-class TcpServer(Server[bytes]):
-    """A configurable tcp server with delegated message handling for use in adapters."""
+class TcpIo(AdapterIo[CommandAdapter]):
+    """An AdapterIo implementation which delegates to a tcp server.
 
-    def __init__(
-        self,
-        host: str = "localhost",
-        port: int = 25565,
-        format: ByteFormat = ByteFormat(b"%b"),
-    ) -> None:
-        """The TcpServer constructor which takes a host, port and format byte string.
+    An AdapterIo implementation which delegates the hosting of an external messaging
+    protocol to a server and utilises message handling from a CommandAdapter.
+    """
 
-        Args:
-            host (str): The host name which the server should be run under.
-            port (int): The port number which the server should listen to.
-            format (ByteFormat): A formatting string for messages sent by the server,
-                allowing for the prepending and appending of data. Defaults to b"%b".
-        """
+    host: str
+    port: int
+
+    def __init__(self, host: str, port: int) -> None:
         self.host = host
         self.port = port
-        self.format = format.format
 
-    async def run_forever(
-        self,
-        on_connect: Callable[[], AsyncIterable[Optional[bytes]]],
-        handler: Callable[[bytes], Awaitable[AsyncIterable[Optional[bytes]]]],
+    async def setup(
+        self, adapter: CommandAdapter, raise_interrupt: RaiseInterrupt
     ) -> None:
-        """Runs the TCP server indefinitely on the configured host and port.
-
-        An asynchronous method used to run the server indefinitely on the configured
-        host and port. Upon client connection, messages from the on_connect iterable
-        will be sent. Upon receiving a message the server will delegate handling of it
-        to the handler. Replies will be formatted according to the configured format
-        string.
-
-        Args:
-            on_connect (Callable[[], AsyncIterable[bytes]]): An asynchronous iterable
-                of messages to be sent upon client connection.
-            handler (Callable[[bytes], Awaitable[AsyncIterable[bytes]]]): An
-                asynchronous message handler which returns an asynchronous iterable of
-                replies.
-        """
-        handle = self._generate_handle_function(on_connect, handler)
+        handle = self._generate_handle_function(
+            adapter.on_connect,
+            adapter.handle_message,
+            raise_interrupt,
+            adapter.byte_format,
+        )
 
         server = await asyncio.start_server(handle, self.host, self.port)
 
-        async with server:
-            await server.serve_forever()
+        async def run_forever() -> None:
+            async with server:
+                await server.serve_forever()
+
+        asyncio.create_task(run_forever())
 
     def _generate_handle_function(
         self,
         on_connect: Callable[[], AsyncIterable[Optional[bytes]]],
-        handler: Callable[[bytes], Awaitable[AsyncIterable[Optional[bytes]]]],
+        handler: Callable[
+            [bytes, RaiseInterrupt], Awaitable[AsyncIterable[Optional[bytes]]]
+        ],
+        raise_interrupt: RaiseInterrupt,
+        format: ByteFormat,
     ) -> Callable[[StreamReader, StreamWriter], Awaitable[None]]:
         """Generates the handle function to be passed to the server.
 
         The handle function is generated from the specified functions. Its purpose is
         to define how the server will respond to incoming messages.
 
         Args:
@@ -78,26 +67,35 @@
 
         async def handle(reader: StreamReader, writer: StreamWriter) -> None:
             async def reply(replies: AsyncIterable[Optional[bytes]]) -> None:
                 async for reply in replies:
                     if reply is None:
                         continue
                     LOGGER.debug(f"Replying with {reply!r}")
-                    writer.write(self.format % reply)
+                    writer.write(format.format % reply)
                     if writer.is_closing():
                         break
                     await writer.drain()
 
             tasks.append(asyncio.create_task(reply(on_connect())))
 
             while True:
                 data: bytes = await reader.read(1024)
                 if data == b"":
                     break
                 addr = writer.get_extra_info("peername")
 
                 LOGGER.debug(f"Received {data!r} from {addr}")
-                tasks.append(asyncio.create_task(reply(await handler(data))))
+                tasks.append(
+                    asyncio.create_task(
+                        reply(
+                            await handler(
+                                data,
+                                raise_interrupt,
+                            )
+                        )
+                    )
+                )
 
             await asyncio.wait(tasks)
 
         return handle
```

### Comparing `tickit-0.3.0/src/tickit/adapters/zeromq/push_adapter.py` & `tickit-0.4.0/src/tickit/adapters/io/zeromq_push_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,84 @@
 import asyncio
 import json
 import logging
-from typing import (
-    Any,
-    Iterable,
-    Mapping,
-    Optional,
-    Protocol,
-    Sequence,
-    Union,
-    runtime_checkable,
-)
+from typing import Iterable, Optional, Protocol, runtime_checkable
 
 import aiozmq
 import zmq
 from pydantic.v1 import BaseModel
 
-from tickit.core.adapter import Adapter, RaiseInterrupt
-from tickit.core.device import Device
+from tickit.adapters.zmq import (
+    ZeroMqMessage,
+    ZeroMqPushAdapter,
+    _MessagePart,
+    _SerializableMessagePart,
+    _ZeroMqInternalMessage,
+)
+from tickit.core.adapter import AdapterIo, RaiseInterrupt
 
 LOGGER = logging.getLogger(__name__)
 
 
-_MessagePart = Union[bytes, zmq.Frame, memoryview]
-_SerializableMessagePart = Union[
-    _MessagePart,
-    str,
-    Mapping[str, Any],
-    BaseModel,
-]
-
-_ZeroMqInternalMessage = Sequence[_MessagePart]
-ZeroMqMessage = Sequence[_SerializableMessagePart]
-# SocketFactory = Callable[[], Awaitable[aiozmq.ZmqStream]]
-
-
 @runtime_checkable
 class SocketFactory(Protocol):
     async def __call__(self, __host: str, __port: int) -> aiozmq.ZmqStream:
         ...
 
 
 async def create_zmq_push_socket(host: str, port: int) -> aiozmq.ZmqStream:
     addr = f"tcp://{host}:{port}"
     return await aiozmq.create_zmq_stream(zmq.PUSH, connect=addr, bind=addr)
 
 
-class ZeroMqPushAdapter(Adapter):
-    """An adapter for a ZeroMQ data stream."""
+class ZeroMqPushIo(AdapterIo[ZeroMqPushAdapter]):
+    """AdapterIo for a ZeroMQ data stream."""
 
     _host: str
     _port: int
     _socket: Optional[aiozmq.ZmqStream]
     _socket_factory: SocketFactory
     _socket_lock: asyncio.Lock
+    _task: Optional[asyncio.Task]
 
     def __init__(
         self,
         host: str = "127.0.0.1",
         port: int = 5555,
         socket_factory: SocketFactory = create_zmq_push_socket,
     ) -> None:
         """Initialize with default values."""
         super().__init__()
         self._host = host
         self._port = port
         self._socket = None
         self._socket_factory = socket_factory
         self._socket_lock = asyncio.Lock()
+        self._task = None
 
-    async def run_forever(
-        self,
-        device: Device,
-        raise_interrupt: RaiseInterrupt,
+    async def setup(
+        self, adapter: ZeroMqPushAdapter, raise_interrupt: RaiseInterrupt
     ) -> None:
-        """Runs the ZeroMQ adapter continuously."""
-        await super().run_forever(device, raise_interrupt)
-
         try:
             await self._ensure_socket()
+            self._task = asyncio.create_task(self.send_messages_forever(adapter))
         except asyncio.CancelledError:
-            if self._socket is not None:
-                self._socket.close()
-                await self._socket.drain()
+            await self.shutdown()
+
+    async def shutdown(self) -> None:
+        if self._task:
+            self._task.cancel()
+        if self._socket is not None:
+            self._socket.close()
+            await self._socket.drain()
+
+    async def send_messages_forever(self, adapter: ZeroMqPushAdapter) -> None:
+        while True:
+            message = await adapter.next_message()
+            await self.send_message(message)
 
     def send_message_sequence_soon(
         self,
         messages: Iterable[ZeroMqMessage],
     ) -> None:
         async def send_message_sequence() -> None:
             for message in messages:
```

### Comparing `tickit-0.3.0/src/tickit/cli.py` & `tickit-0.4.0/src/tickit/cli.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/adapter.py` & `tickit-0.4.0/src/tickit/core/state_interfaces/kafka.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,84 @@
-from abc import ABC, abstractmethod
-from typing import (
-    Any,
-    AsyncIterable,
-    Awaitable,
-    Callable,
-    Generic,
-    Optional,
-    Tuple,
-    TypeVar,
-)
-
-from typing_extensions import Protocol
-
-from tickit.core.device import Device
-
-#: Message type
-T = TypeVar("T")
-
-
-# https://github.com/python/mypy/issues/708#issuecomment-647124281
-class RaiseInterrupt(Protocol):
-    """A raise_interrupt function that should be passed to `Adapter`."""
-
-    async def __call__(self) -> None:
-        """The actual call signature."""
-        pass
-
-
-class Adapter:
-    """An interface for types which implement device adapters."""
-
-    device: Device
-    raise_interrupt: RaiseInterrupt
-
-    def __getattr__(self, name: str) -> Any:
-        """Improve error message for getting attributes before `run_forever`."""
-        if name in ("device", "raise_interrupt"):
-            raise RuntimeError(
-                "Can't get self.device or self.raise_interrupt before run_forever()"
-            )
-        return super().__getattribute__(name)
-
-    async def run_forever(
-        self, device: Device, raise_interrupt: RaiseInterrupt
-    ) -> None:
-        """An asynchronous method allowing indefinite running of core adapter logic.
-
-        An asynchronous method allowing for indefinite running of core adapter logic
-        (typically the hosting of a protocol server and the interpretation of commands
-        which are supplied via it).
-        """
-        self.device = device
-        self.raise_interrupt = raise_interrupt
+import asyncio
+from typing import Awaitable, Callable, Generic, Iterable, TypeVar
+
+import yaml
+from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
+from yaml.loader import Loader
 
-    def after_update(self):
-        """A method which is called immediately after the device updates."""
+from tickit.core.state_interfaces import state_interface
 
+#: A consumable value
+C = TypeVar("C")
+#: A producible value
+P = TypeVar("P")
 
-class Interpreter(ABC, Generic[T]):
-    """An interface for types which handle messages received by an adapter."""
 
-    @abstractmethod
-    async def handle(
-        self, adapter: Adapter, message: T
-    ) -> Tuple[AsyncIterable[T], bool]:
-        """An asynchronous method which handles messages received by an adapter.
+@state_interface.add("kafka", True)
+class KafkaStateConsumer(Generic[C]):
+    """A kafka implementation of the StateConsumer protocol.
 
-        An asynchronous method which handles messages received by an adapter, replies
-        are sent as an asynchronous iterable to support setting of continuous readback,
-        stand alone replies should be wrapped in an asynchronous iterable of length one.
+    A kafka implementation of the StateConsumer protocol, this consumer can subscribe
+    to kafka topics, upon receiving a message the consumer passes the value to the
+    callback function passed during initialization, if a topic is subscribed to which
+    does not yet exist it is created.
+    """
+
+    def __init__(self, callback: Callable[[C], Awaitable[None]]) -> None:
+        """Creates an AIOKafka Consumer and begins consuming subscribed topics.
 
         Args:
-            adapter (Adapter): The adapter which is delegating message handling.
-            message (T): The message received by the adapter.
+            callback (Callable[[C], Awaitable[None]]): An asynchronous handler function
+                for consumed values.
+        """
+        self.consumer = AIOKafkaConsumer(
+            None,
+            auto_offset_reset="earliest",
+            value_deserializer=lambda m: yaml.load(m.decode("utf-8"), Loader=Loader),
+        )
+        self.callback = callback
+        asyncio.create_task(self._run_forever())
+
+    async def _run_forever(self) -> None:
+        """Starts the consumer and waits for messages to arrive."""
+        await self.consumer.start()
+        while True:
+            async for message in self.consumer:
+                if message.value is not None:
+                    await self.callback(message.value)
 
-        Returns:
-            Tuple[AsyncIterable[T], bool]: A tuple containing both an asynchronous
-                iterable of reply messages and an interrupt flag.
+    async def subscribe(self, topics: Iterable[str]):
+        """Subscribes the consumer to the given topics.
+
+        Subscribes the consumer to the given topics, new messages are passed to the
+        callback.
+
+        Args:
+            topics (Iterable[str]): An iterable of topics to subscribe to.
         """
+        self.consumer.subscribe(topics)
 
 
-class Server(Generic[T]):
-    """An interface for types which implement an external messaging protocol."""
+@state_interface.add("kafka", True)
+class KafkaStateProducer(Generic[P]):
+    """A kafka implementation of the StateProducer protocol.
+
+    A kafka implementation of the StateProducer protocol, this producer can produce a
+    value to a kafka topic, if the topic does not yet exist it is created.
+    """
+
+    def __init__(self) -> None:
+        """Creates and starts and AIOKafka Producer."""
+        self.producer = AIOKafkaProducer(
+            value_serializer=lambda m: yaml.dump(m).encode("utf-8")
+        )
+        self._start = asyncio.create_task(self.producer.start())
 
-    async def run_forever(
-        self,
-        on_connect: Callable[[], AsyncIterable[Optional[T]]],
-        handler: Callable[[T], Awaitable[AsyncIterable[Optional[T]]]],
-    ) -> None:
-        """An asynchronous method allowing indefinite running of core server logic.
+    async def produce(self, topic: str, value: P) -> None:
+        """Produces a value to the provided topic.
 
         Args:
-            on_connect (Callable[[], AsyncIterable[Optional[T]]]): An asynchronous
-                iterable of messages to be sent once a client connects.
-            handler (Callable[[T], Awaitable[AsyncIterable[Optional[T]]]]): An
-                asynchronous method used to handle received messages, returning an
-                asynchronous iterable of replies.
+            topic (str): The topic to which the value should be sent.
+            value (P): The value to send to the provided topic.
         """
+        await self._start
+        await self.producer.send(topic, value)
```

### Comparing `tickit-0.3.0/src/tickit/core/components/component.py` & `tickit-0.4.0/src/tickit/core/components/component.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/components/device_simulation.py` & `tickit-0.4.0/src/tickit/core/components/device_simulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
 import logging
 from dataclasses import dataclass, field
 from typing import Awaitable, Callable, Dict, Hashable, List, Mapping, Type, cast
 
 from immutables import Map
 
-from tickit.core.adapter import Adapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import BaseComponent
 from tickit.core.device import Device, DeviceUpdate
-from tickit.core.runner import run_all
 from tickit.core.state_interfaces import StateConsumer, StateProducer
 from tickit.core.typedefs import Changes, ComponentID, SimTime, State
 
 InterruptHandler = Callable[[], Awaitable[None]]
 
 
 LOGGER = logging.getLogger(__name__)
@@ -25,27 +24,27 @@
     A component which thinly wraps a device and the corresponding adapters, this
     component delegates core behaviour to the update method of the device, whilst
     allowing adapters to raise interrupts.
     """
 
     name: ComponentID
     device: Device
-    adapters: List[Adapter] = field(default_factory=list)
+    adapters: List[AdapterContainer] = field(default_factory=list)
     last_outputs: State = field(init=False, default_factory=lambda: State({}))
     device_inputs: Dict[str, Hashable] = field(init=False, default_factory=dict)
     _tasks: List[asyncio.Task] = field(default_factory=list)
 
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
         """Set up state interfaces, run adapters and blocks until any complete."""
-        self._tasks = run_all(
-            adapter.run_forever(self.device, self.raise_interrupt)
+        self._tasks = [
+            asyncio.create_task(adapter.run_forever(self.raise_interrupt))
             for adapter in self.adapters
-        )
+        ]
 
         await super().run_forever(state_consumer, state_producer)
         if self._tasks:
             await asyncio.wait(self._tasks)
 
     async def on_tick(self, time: SimTime, changes: Changes) -> None:
         """Delegates core behaviour to the device and calls adapter on_update.
@@ -64,15 +63,15 @@
             **self.device_inputs,
             **cast(Mapping[str, Hashable], changes),
         }
         device_update: DeviceUpdate = self.device.update(
             SimTime(time), self.device_inputs
         )
         for adapter in self.adapters:
-            adapter.after_update()
+            adapter.adapter.after_update()
         out_changes = Changes(
             Map(
                 {
                     k: v
                     for k, v in device_update.outputs.items()
                     if k not in self.last_outputs or not self.last_outputs[k] == v
                 }
```

### Comparing `tickit-0.3.0/src/tickit/core/components/system_simulation.py` & `tickit-0.4.0/src/tickit/core/components/system_simulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
 import logging
 from dataclasses import dataclass, field
-from typing import Dict, List, Type
+from typing import Dict, List, Optional, Type
 
 import pydantic.v1.dataclasses
 
+from tickit.adapters.system import BaseSystemSimulationAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import BaseComponent, Component, ComponentConfig
 from tickit.core.management.event_router import InverseWiring
 from tickit.core.management.schedulers.slave import SlaveScheduler
-from tickit.core.runner import run_all
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import Changes, ComponentID, ComponentPort, PortID, SimTime
 from tickit.utils.topic_naming import output_topic
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -30,14 +31,16 @@
     #: A list of immutable component configuration data containers, used to
     #: construct internal components.
     components: List[ComponentConfig]
     #: A mapping of outputs which the system simulation exposes and the
     #: corresponding output of an internal component.
     expose: Dict[PortID, ComponentPort]
 
+    adapter: Optional[AdapterContainer[BaseSystemSimulationAdapter]] = None
+
     _tasks: List[asyncio.Task] = field(default_factory=list)
 
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
         """Sets up state interfaces, the scheduler, and components to run continuously.
 
@@ -49,19 +52,29 @@
         self.scheduler = SlaveScheduler(
             inverse_wiring,
             state_consumer,
             state_producer,
             self.expose,
             self.raise_interrupt,
         )
-        self._tasks = run_all(
-            component().run_forever(state_consumer, state_producer)
-            for component in self.components
-        ) + run_all([self.scheduler.run_forever()])
+        components = {config.name: config() for config in self.components}
+
+        self._tasks = [
+            asyncio.create_task(component.run_forever(state_consumer, state_producer))
+            for component in components.values()
+        ] + [asyncio.create_task(self.scheduler.run_forever())]
+
+        if self.adapter:
+            self.adapter.adapter.setup_adapter(components, self.scheduler._wiring)
+            self._tasks.append(
+                asyncio.create_task(self.adapter.run_forever(self.raise_interrupt))
+            )
+
         await super().run_forever(state_consumer, state_producer)
+
         if self._tasks:
             await asyncio.wait(self._tasks)
 
     async def on_tick(self, time: SimTime, changes: Changes) -> None:
         """Delegates core behaviour to the slave scheduler.
 
         An asynchronous method which delegates core behaviour of computing changes and
```

### Comparing `tickit-0.3.0/src/tickit/core/device.py` & `tickit-0.4.0/src/tickit/core/device.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/management/event_router.py` & `tickit-0.4.0/src/tickit/core/management/event_router.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/management/schedulers/base.py` & `tickit-0.4.0/src/tickit/core/management/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/management/schedulers/master.py` & `tickit-0.4.0/src/tickit/core/management/schedulers/master.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/management/schedulers/slave.py` & `tickit-0.4.0/src/tickit/core/management/schedulers/slave.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/management/ticker.py` & `tickit-0.4.0/src/tickit/core/management/ticker.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/simulation.py` & `tickit-0.4.0/src/tickit/core/simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/state_interfaces/internal.py` & `tickit-0.4.0/src/tickit/core/state_interfaces/internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/core/state_interfaces/state_interface.py` & `tickit-0.4.0/src/tickit/core/state_interfaces/state_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Dict,
     Iterable,
     Protocol,
     Set,
     Tuple,
     Type,
     TypeVar,
+    Union,
     runtime_checkable,
 )
 from warnings import warn
 
 #: A consumable value
 C = TypeVar("C", covariant=True)
 #: A producible value
@@ -69,16 +70,15 @@
             topic (str): The topic to which the value should be sent.
             value (P): The value to send to the provided topic.
         """
         pass
 
 
 #: The union of StateConsumer and StateProducer
-StateInterface = TypeVar("StateInterface", StateConsumer, StateProducer)
-
+StateInterface = TypeVar("StateInterface", bound=Union[StateConsumer, StateProducer])
 
 consumers: Dict[str, Tuple[Type[StateConsumer], bool]] = dict()
 producers: Dict[str, Tuple[Type[StateProducer], bool]] = dict()
 
 
 def add(
     name: str, external: bool
```

### Comparing `tickit-0.3.0/src/tickit/core/typedefs.py` & `tickit-0.4.0/src/tickit/core/typedefs.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/devices/iobox.py` & `tickit-0.4.0/src/tickit/devices/iobox.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,21 +49,20 @@
     The envisioned use of this class is where you wish to simulate a network
     interface but the internal hardware logic is either not needed or very simple.
     A custom adapter can be made for the network interface and can simply
     read and write to an IoBox.
     """
 
     #: A typed mapping containing the 'input' input value
-    Inputs: TypedDict = TypedDict(
-        "Inputs", {"updates": NotRequired[List[Tuple[Any, Any]]]}
-    )
-    #: An empty typed mapping of device outputs
-    Outputs: TypedDict = TypedDict(
-        "Outputs", {"updates": NotRequired[List[Tuple[Any, Any]]]}
-    )
+    class Inputs(TypedDict):
+        updates: NotRequired[List[Tuple[Any, Any]]]
+
+    #: A typed mapping of device outputs
+    class Outputs(TypedDict):
+        updates: NotRequired[List[Tuple[Any, Any]]]
 
     _memory: Dict[A, V]
     _change_buffer: List[Tuple[A, V]]
 
     def __init__(self) -> None:  # noqa: D107
         self._memory = {}
         self._change_buffer = []
```

### Comparing `tickit-0.3.0/src/tickit/devices/sink.py` & `tickit-0.4.0/src/tickit/devices/sink.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class SinkDevice(Device):
     """A simple device which can take any input and produces no output."""
 
     #: A typed mapping containing the 'input' input value
-    Inputs: TypedDict = TypedDict("Inputs", {"input": Any})
+    class Inputs(TypedDict):
+        input: Any
+
     #: An empty typed mapping of device outputs
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    class Outputs(TypedDict):
+        ...
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
         """The update method which logs the inputs and produces no outputs.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
```

### Comparing `tickit-0.3.0/src/tickit/devices/source.py` & `tickit-0.4.0/src/tickit/devices/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class SourceDevice(Device):
     """A simple device which produces a pre-configured value."""
 
     #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the 'value' output value
-    Outputs: TypedDict = TypedDict("Outputs", {"value": Any})
+    class Outputs(TypedDict):
+        value: Any
 
     def __init__(self, value: Any) -> None:
         """A constructor of the source, which takes the pre-configured output value.
 
         Args:
             value (Any): A pre-configured output value.
         """
```

### Comparing `tickit-0.3.0/src/tickit/utils/configuration/loading.py` & `tickit-0.4.0/src/tickit/utils/configuration/loading.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit/utils/configuration/tagged_union.py` & `tickit-0.4.0/src/tickit/utils/configuration/tagged_union.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         # Keep track of inheriting classes in super class
         super_cls._ref_classes.add(cls)
 
         # Add a discriminator field to the class so it can
         # be identified when deserializing.
         cls.__annotations__ = {
             **getattr(cls, "__annotations__", {}),
-            discriminator: Literal[cls_name],
+            # Literal is supposed to only accept literal strings but we need to
+            # set it dynamically
+            discriminator: Literal[cls_name],  # type: ignore
         }
         setattr(cls, discriminator, field(default=cls_name, repr=False))
 
     def __get_validators__(cls) -> Any:
         yield cls.__validate__
 
     def __validate__(cls, v: Any) -> Any:
```

### Comparing `tickit-0.3.0/src/tickit/utils/topic_naming.py` & `tickit-0.4.0/src/tickit/utils/topic_naming.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/src/tickit.egg-info/PKG-INFO` & `tickit-0.4.0/src/tickit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -292,16 +292,19 @@
                 name=self.name,
                 device=CounterDevice(),
                 )
 
     class CounterDevice(Device):
         """A simple device which increments a value."""
 
-        Inputs: TypedDict = TypedDict("Inputs", {})
-        Outputs: TypedDict = TypedDict("Outputs", {"value":int})
+        class Inputs(TypedDict):
+            ...
+
+        class Outputs(TypedDict):
+            value: int
 
         def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
             self._value = initial_value
             self.callback_period = SimTime(callback_period)
             LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
```

### Comparing `tickit-0.3.0/src/tickit.egg-info/SOURCES.txt` & `tickit-0.4.0/src/tickit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -58,77 +58,72 @@
 docs/images/tickit-system-simulation-cpt.svg
 docs/user/index.rst
 docs/user/explanations/adapters.rst
 docs/user/explanations/components.rst
 docs/user/explanations/devices.rst
 docs/user/explanations/framework-summary.rst
 docs/user/explanations/glossary.rst
+docs/user/explanations/system-simulation-adapters.rst
 docs/user/explanations/wiring.rst
-docs/user/how-to/use-command-wrappers.rst
 docs/user/how-to/use-epics-adapter.rst
 docs/user/reference/api.rst
 docs/user/tutorials/create-a-device.rst
 docs/user/tutorials/creating-a-simulation.rst
 docs/user/tutorials/installation.rst
 docs/user/tutorials/running-a-simulation.rst
-docs/user/tutorials/use-composed-adapter.rst
+docs/user/tutorials/use-command-adapter.rst
+examples/adapters/http_adapter.py
+examples/adapters/system_simulation_adapter.py
+examples/adapters/system_simulation_adapter_config.py
+examples/adapters/zeromq_push_adapter.py
 examples/configs/amplifier.yaml
 examples/configs/counter.yaml
-examples/configs/http-and-zeromq-devices.yaml
-examples/configs/http-device.yaml
+examples/configs/http-and-zeromq-ioboxes.yaml
+examples/configs/http-iobox.yaml
 examples/configs/isolated-device.yaml
+examples/configs/nested-amplifier-with-system-adapter.yaml
 examples/configs/nested.yaml
 examples/configs/shutter.yaml
 examples/configs/sunk-tcp.yaml
 examples/configs/sunk-trampoline.yaml
 examples/devices/__init__.py
 examples/devices/amplifier.py
 examples/devices/counter.py
-examples/devices/http_device.py
 examples/devices/isolated_device.py
-examples/devices/isolated_record.db
 examples/devices/remote_controlled.py
 examples/devices/shutter.py
 examples/devices/trampoline.py
-examples/devices/zeromq_push_device.py
 src/tickit/__init__.py
 src/tickit/__main__.py
 src/tickit/_version.py
 src/tickit/cli.py
 src/tickit.egg-info/PKG-INFO
 src/tickit.egg-info/SOURCES.txt
 src/tickit.egg-info/dependency_links.txt
 src/tickit.egg-info/entry_points.txt
 src/tickit.egg-info/requires.txt
 src/tickit.egg-info/top_level.txt
 src/tickit/adapters/__init__.py
-src/tickit/adapters/composed.py
-src/tickit/adapters/httpadapter.py
-src/tickit/adapters/epicsadapter/__init__.py
-src/tickit/adapters/epicsadapter/adapter.py
-src/tickit/adapters/epicsadapter/ioc_manager.py
-src/tickit/adapters/interpreters/__init__.py
-src/tickit/adapters/interpreters/utils.py
-src/tickit/adapters/interpreters/command/__init__.py
-src/tickit/adapters/interpreters/command/command_interpreter.py
-src/tickit/adapters/interpreters/command/regex_command.py
-src/tickit/adapters/interpreters/endpoints/__init__.py
-src/tickit/adapters/interpreters/endpoints/http_endpoint.py
-src/tickit/adapters/interpreters/wrappers/__init__.py
-src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
-src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
-src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
-src/tickit/adapters/servers/__init__.py
-src/tickit/adapters/servers/tcp.py
-src/tickit/adapters/zeromq/__init__.py
-src/tickit/adapters/zeromq/push_adapter.py
+src/tickit/adapters/epics.py
+src/tickit/adapters/http.py
+src/tickit/adapters/system.py
+src/tickit/adapters/tcp.py
+src/tickit/adapters/utils.py
+src/tickit/adapters/zmq.py
+src/tickit/adapters/io/__init__.py
+src/tickit/adapters/io/epics_io.py
+src/tickit/adapters/io/http_io.py
+src/tickit/adapters/io/tcp_io.py
+src/tickit/adapters/io/zeromq_push_io.py
+src/tickit/adapters/specifications/__init__.py
+src/tickit/adapters/specifications/http_endpoint.py
+src/tickit/adapters/specifications/regex_command.py
 src/tickit/core/__init__.py
 src/tickit/core/adapter.py
 src/tickit/core/device.py
-src/tickit/core/runner.py
 src/tickit/core/simulation.py
 src/tickit/core/typedefs.py
 src/tickit/core/components/__init__.py
 src/tickit/core/components/component.py
 src/tickit/core/components/device_simulation.py
 src/tickit/core/components/system_simulation.py
 src/tickit/core/management/__init__.py
@@ -151,30 +146,27 @@
 src/tickit/utils/singleton.py
 src/tickit/utils/topic_naming.py
 src/tickit/utils/configuration/__init__.py
 src/tickit/utils/configuration/loading.py
 src/tickit/utils/configuration/tagged_union.py
 tests/conftest.py
 tests/test_cli.py
-tests/adapters/test_httpadapter.py
-tests/adapters/interpreters/test_utils.py
-tests/adapters/interpreters/command/test_command_interpreter.py
-tests/adapters/interpreters/command/test_regex_command.py
-tests/adapters/interpreters/endpoints/test_http_endpoint.py
-tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
-tests/adapters/interpreters/wrappers/test_joining_interpreter.py
-tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
-tests/adapters/servers/test_tcp.py
-tests/adapters/test_epicsadapter/__init__.py
-tests/adapters/test_epicsadapter/test_epics_adapter.py
-tests/adapters/zeromq/__init__.py
-tests/adapters/zeromq/test_push_adapter.py
+tests/adapters/test_epics.py
+tests/adapters/test_http.py
+tests/adapters/test_system.py
+tests/adapters/test_tcp.py
+tests/adapters/test_utils.py
+tests/adapters/io/test_epics_io.py
+tests/adapters/io/test_http_io.py
+tests/adapters/io/test_tcp_io.py
+tests/adapters/io/test_zeromq_push_io.py
+tests/adapters/specifications/test_http_endpoint.py
+tests/adapters/specifications/test_regex_command.py
 tests/core/sim.yaml
 tests/core/test_device.py
-tests/core/test_runner.py
 tests/core/test_simulation.py
 tests/core/test_typedefs.py
 tests/core/components/test_component.py
 tests/core/components/test_device_simulation.py
 tests/core/components/test_system_simulation.py
 tests/core/management/test_event_router.py
 tests/core/management/test_ticker.py
@@ -183,12 +175,16 @@
 tests/core/management/schedulers/test_slave_scheduler.py
 tests/core/state_interfaces/test_internal.py
 tests/core/state_interfaces/test_kafka.py
 tests/core/state_interfaces/test_state_interface.py
 tests/devices/test_iobox.py
 tests/devices/test_sink.py
 tests/devices/test_source.py
+tests/system_tests/test_with_master.py
+tests/system_tests/test_with_master_and_slave.py
+tests/system_tests/configs/nested.yaml
+tests/system_tests/configs/test_with_master.yaml
 tests/utils/test_byte_format.py
 tests/utils/test_configurable.py
 tests/utils/test_singleton.py
 tests/utils/test_topic_naming.py
 tests/utils/configuration/test_loading.py
```

### Comparing `tickit-0.3.0/tests/adapters/interpreters/command/test_command_interpreter.py` & `tickit-0.4.0/tests/adapters/test_tcp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from dataclasses import dataclass
-from typing import Callable, Optional, Sequence
+from typing import AnyStr, Callable, Optional, Sequence
 
 import pytest
 from mock import AsyncMock, MagicMock, patch
 
-from tickit.adapters.interpreters.command import CommandInterpreter
-from tickit.adapters.interpreters.command.command_interpreter import Command
-from tickit.core.adapter import Adapter
+from tickit.adapters.tcp import Command, CommandAdapter
+from tickit.core.device import Device
 
-_GET_TYPE_HINTS = (
-    "tickit.adapters.interpreters.command.command_interpreter.get_type_hints"
-)
+_GET_TYPE_HINTS = "tickit.adapters.tcp.get_type_hints"
+
+
+class ExampleAdapter(CommandAdapter):
+    device: Device
+
+    def test_method(self) -> None:
+        pass
 
 
 @pytest.fixture
-def command_interpreter():
-    return CommandInterpreter()
+def adapter() -> CommandAdapter:
+    command_adapter = ExampleAdapter()
+    return command_adapter
 
 
 @pytest.fixture
 def TestCommand():
     @dataclass(frozen=True)
     class TestCommand:
         command: bytes
@@ -38,139 +43,114 @@
 
 
 @patch(
     _GET_TYPE_HINTS,
     lambda _: {"arg1": str, "arg2": str},
 )
 @pytest.mark.asyncio
-async def test_command_interpreter_handle_calls_func_with_args(
-    command_interpreter: CommandInterpreter,
-):
-    test_adapter = MagicMock(
-        Adapter,
-        test_method=AsyncMock(
-            __command__=MagicMock(
-                Command,
-                interrupt=False,
-                parse=MagicMock(return_value=("arg1", "arg2")),
-            ),
+async def test_command_adapter_handle_calls_func_with_args(adapter: ExampleAdapter):
+    assert adapter is not None
+
+    adapter.test_method = AsyncMock(
+        __command__=MagicMock(
+            Command,
+            interrupt=False,
+            parse=MagicMock(return_value=("arg1", "arg2")),
         ),
     )
-    await command_interpreter.handle(test_adapter, b"\x01")
-    test_adapter.test_method.assert_awaited_once_with("arg1", "arg2")
+
+    await adapter.handle(b"\x01")
+
+    adapter.test_method.assert_awaited_once_with("arg1", "arg2")
 
 
 @patch(
     _GET_TYPE_HINTS,
     lambda _: {"arg1": str, "arg2": str},
 )
 @pytest.mark.asyncio
-async def test_command_interpreter_handle_returns_iterable_reply(
-    command_interpreter: CommandInterpreter,
-):
+async def test_command_adapter_handle_returns_iterable_reply(adapter: ExampleAdapter):
     reply = AsyncMock(__aiter__=MagicMock(), __anext__=AsyncMock())
-    test_adapter = MagicMock(
-        Adapter,
-        test_method=AsyncMock(
-            __command__=MagicMock(
-                Command,
-                interrupt=False,
-                parse=MagicMock(return_value=("arg1", "arg2")),
-            ),
-            return_value=reply,
+    adapter.test_method = AsyncMock(
+        __command__=MagicMock(
+            Command,
+            interrupt=False,
+            parse=MagicMock(return_value=("arg1", "arg2")),
         ),
+        return_value=reply,
     )
-    assert reply == (await command_interpreter.handle(test_adapter, b"\x01"))[0]
+    assert reply == (await adapter.handle(b"\x01"))[0]
 
 
 @patch(
     _GET_TYPE_HINTS,
     lambda _: {"arg1": str, "arg2": str},
 )
 @pytest.mark.asyncio
-async def test_command_interpreter_handle_wraps_non_iterable_reply(
-    command_interpreter: CommandInterpreter,
-):
+async def test_command_adapter_handle_wraps_non_iterable_reply(adapter: ExampleAdapter):
     reply = MagicMock("TestReply")
-    test_adapter = MagicMock(
-        Adapter,
-        test_method=AsyncMock(
-            __command__=MagicMock(
-                Command,
-                interrupt=False,
-                parse=MagicMock(return_value=("arg1", "arg2")),
-            ),
-            return_value=reply,
+    adapter.test_method = AsyncMock(
+        __command__=MagicMock(
+            Command,
+            interrupt=False,
+            parse=MagicMock(return_value=("arg1", "arg2")),
         ),
+        return_value=reply,
     )
-    assert (
-        reply
-        == await (await command_interpreter.handle(test_adapter, b"\x01"))[0]
-        .__aiter__()
-        .__anext__()
-    )
+    assert reply == await (await adapter.handle(b"\x01"))[0].__aiter__().__anext__()
 
 
 @patch(
     _GET_TYPE_HINTS,
     lambda _: {"arg1": str, "arg2": str},
 )
 @pytest.mark.asyncio
 @pytest.mark.parametrize("interrupt", [True, False])
-async def test_command_interpreter_handle_returns_interrupt(
-    command_interpreter: CommandInterpreter, interrupt: bool
+async def test_command_adapter_handle_returns_interrupt(
+    adapter: ExampleAdapter, interrupt: bool
 ):
-    test_adapter = MagicMock(
-        Adapter,
-        test_method=AsyncMock(
-            __command__=MagicMock(
-                Command,
-                interrupt=interrupt,
-                parse=MagicMock(return_value=("arg1", "arg2")),
-            ),
-            return_value="DummyReply",
+    adapter.test_method = AsyncMock(
+        __command__=MagicMock(
+            Command,
+            interrupt=interrupt,
+            parse=MagicMock(return_value=("arg1", "arg2")),
         ),
+        return_value="DummyReply",
     )
-    assert interrupt == (await command_interpreter.handle(test_adapter, b"\x01"))[1]
+    assert interrupt == (await adapter.handle(b"\x01"))[1]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("interrupt", [True, False])
-async def test_command_interpreter_handle_skips_unparsed(
-    command_interpreter: CommandInterpreter, interrupt: bool
+async def test_command_adapter_handle_skips_unparsed(
+    adapter: ExampleAdapter, interrupt: bool
 ):
-    test_adapter = MagicMock(
-        Adapter,
-        test_method=AsyncMock(
-            __command__=MagicMock(
-                Command, interrupt=interrupt, parse=MagicMock(return_value=None)
-            ),
-            return_value="DummyReply",
+    adapter.test_method = AsyncMock(
+        __command__=MagicMock(
+            Command, interrupt=interrupt, parse=MagicMock(return_value=None)
         ),
+        return_value="DummyReply",
     )
     assert (
         b"Request does not match any known command"
-        == await (
-            await command_interpreter.handle(
-                test_adapter, "TestCommand".encode("utf-8")
-            )
-        )[0]
+        == await (await adapter.handle("TestCommand".encode("utf-8")))[0]
         .__aiter__()
         .__anext__()
     )
 
 
 @pytest.mark.asyncio
-async def test_command_interpreter_handle_returns_message_for_no_commands(
-    command_interpreter: CommandInterpreter,
-):
-    test_adapter = MagicMock(Adapter)
-    assert (
-        b"Request does not match any known command"
-        == await (
-            await command_interpreter.handle(
-                test_adapter, "TestCommand".encode("utf-8")
-            )
-        )[0]
-        .__aiter__()
-        .__anext__()
-    )
+@pytest.mark.parametrize(
+    "command, response_message",
+    [
+        ("UnknownString", "Request does not match any known command"),
+        (b"UnknownBytes", b"Request does not match any known command"),
+    ],
+)
+async def test_command_adapter_handle_returns_message_for_no_commands(
+    adapter: ExampleAdapter,
+    command: AnyStr,
+    response_message: AnyStr,
+):
+    response = await adapter.handle(command)
+    message = await response[0].__anext__()
+    assert message == response_message
```

### Comparing `tickit-0.3.0/tests/adapters/interpreters/command/test_regex_command.py` & `tickit-0.4.0/tests/adapters/specifications/test_regex_command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import AnyStr, Optional, Tuple
 
 import pytest
 
-from tickit.adapters.interpreters.command import RegexCommand
+from tickit.adapters.specifications import RegexCommand
 
 
 @pytest.fixture
 def regex_command(regex: AnyStr, interrupt: bool, format: Optional[str]):
     return RegexCommand(regex, interrupt, format)
 
 
 def test_regex_command_registers_command():
     class TestAdapter:
-        @RegexCommand("test")
+        @RegexCommand("test", format="utf-8")
         def test_method():
             pass
 
     assert isinstance(TestAdapter.test_method.__command__, RegexCommand)
 
 
 @pytest.mark.parametrize(
@@ -41,13 +41,15 @@
             False,
             "utf-8",
             r"TestMessage42".encode("utf-8"),
             ("42",),
         ),
         (b"\\x01", False, None, b"\x01", tuple()),
         (b"\\x01(.)", False, None, b"\x01\x02", (b"\x02",)),
+        (r"Test\((\d)\)", False, "utf-8", "Test(4)\n".encode("utf-8"), ("4",)),
+        (r"Test\((\d)\)", False, "utf-8", "Test(3)\r\n".encode("utf-8"), ("3",)),
     ],
 )
 def test_regex_command_parse_match_returns_args(
     regex_command: RegexCommand, message: bytes, expected: Tuple[object]
 ):
     assert expected == regex_command.parse(message)
```

### Comparing `tickit-0.3.0/tests/adapters/test_httpadapter.py` & `tickit-0.4.0/tests/adapters/io/test_http_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import aiohttp
 import pytest
 import pytest_asyncio
 from aiohttp import web
 from mock import Mock
 from mock.mock import create_autospec
 
-from tickit.adapters.httpadapter import HttpAdapter
-from tickit.adapters.interpreters.endpoints.http_endpoint import HttpEndpoint
-from tickit.core.adapter import RaiseInterrupt
+from tickit.adapters.http import HttpAdapter
+from tickit.adapters.io.http_io import HttpIo
+from tickit.adapters.specifications import HttpEndpoint
+from tickit.core.adapter import AdapterContainer, RaiseInterrupt
 from tickit.core.device import Device
 
 ISSUE_LINK = "https://github.com/dls-controls/tickit/issues/111"
 REQUEST_TIMEOUT = 0.5
 
 
 @pytest.fixture
@@ -75,44 +76,65 @@
     async def put_interrupt(self, request: web.Request) -> web.Response:
         name = request.match_info["name"]
         value = (await request.json())["value"]
         return web.json_response({"entity": name, "value": value})
 
 
 @pytest.fixture
-def adapter() -> HttpAdapter:
+def adapter_container() -> AdapterContainer:
     http_adapter = ExampleAdapter()
-    return http_adapter
+    http_io = HttpIo()
+    return AdapterContainer(http_adapter, http_io)
 
 
 @pytest_asyncio.fixture
 async def adapter_task(
-    adapter: HttpAdapter,
+    adapter_container: AdapterContainer,
     mock_raise_interrupt: RaiseInterrupt,
     mock_device: Device,
     event_loop: asyncio.BaseEventLoop,
 ):
-    task = event_loop.create_task(
-        adapter.run_forever(mock_device, mock_raise_interrupt)
+    adapter_container_running = event_loop.create_task(
+        adapter_container.run_forever(mock_raise_interrupt)
     )
-    await adapter.wait_until_ready()
-    yield task
-    await adapter.stop()
-    await asyncio.wait_for(task, timeout=10.0)
-    assert task.done()
+
+    assert isinstance(adapter_container.io, HttpIo)
+
+    adapter_container_ready = event_loop.create_task(
+        adapter_container.io.wait_until_ready()
+    )
+
+    # either wait until the task has an exception or it's ready.
+    done, _ = await asyncio.wait(
+        [adapter_container_running, adapter_container_ready],
+        return_when=asyncio.tasks.FIRST_COMPLETED,
+    )
+
+    if adapter_container_running in done:
+        exception = adapter_container_running.exception()
+        if exception is not None:
+            raise exception
+
+        raise Exception("adapter.run_forever should not finish without an exception")
+
+    yield adapter_container_running
+    await adapter_container.io.stop()
+    await asyncio.wait_for(adapter_container_running, timeout=10.0)
+    assert adapter_container_running.done()
 
 
 @pytest_asyncio.fixture
-async def adapter_url(adapter_task: asyncio.Task, adapter: HttpAdapter):
-    yield f"http://localhost:{adapter.port}"
+async def adapter_url(adapter_task: asyncio.Task, adapter_container: AdapterContainer):
+    assert isinstance(adapter_container.io, HttpIo)
+    yield f"http://localhost:{adapter_container.io.port}"
 
 
 @pytest.mark.asyncio
 async def test_shuts_down_server_on_cancel(
-    adapter: HttpAdapter,
+    adapter_container: AdapterContainer,
     adapter_task: asyncio.Task,
     adapter_url: str,
 ):
     # Verify server is up
     await assert_server_is_up(adapter_url)
 
     # Cancel task
@@ -124,41 +146,41 @@
 
     # Verify server is now down
     await assert_server_is_down(adapter_url)
 
 
 @pytest.mark.asyncio
 async def test_stop_is_idempotent(
-    adapter: HttpAdapter,
+    adapter_container: AdapterContainer,
     adapter_task: asyncio.Task,
     adapter_url: str,
     mock_raise_interrupt: RaiseInterrupt,
     mock_device: Device,
 ) -> None:
     # First ensure the server is working, then stop it and
     # ensure it is no longer working
     await assert_server_is_up(adapter_url)
-    await adapter.stop()
+    assert isinstance(adapter_container.io, HttpIo)
+    await adapter_container.io.stop()
     await adapter_task
     assert adapter_task.done()
     await assert_server_is_down(adapter_url)
 
     for i in range(2):
         # Then start it again and check it is working
         new_task = asyncio.create_task(
-            adapter.run_forever(
-                mock_device,
+            adapter_container.run_forever(
                 mock_raise_interrupt,
             )
         )
-        await adapter.wait_until_ready()
+        await adapter_container.io.wait_until_ready()
         await assert_server_is_up(adapter_url)
 
         # Finally stop it one more time and check it is stopped
-        await adapter.stop()
+        await adapter_container.io.stop()
         await new_task
         assert new_task.done()
         await assert_server_is_down(adapter_url)
 
 
 async def assert_server_is_up(adapter_url: str) -> None:
     url = f"{adapter_url}/foo"
```

### Comparing `tickit-0.3.0/tests/adapters/zeromq/test_push_adapter.py` & `tickit-0.4.0/tests/adapters/io/test_zeromq_push_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 import asyncio
-from typing import Sequence
+from typing import AsyncGenerator, Sequence
 
 import aiozmq
 import pytest
 import pytest_asyncio
-from mock import MagicMock, Mock
-from mock.mock import AsyncMock, create_autospec
+from mock import AsyncMock, MagicMock, Mock
 from pydantic.v1 import BaseModel
 
-from tickit.adapters.zeromq.push_adapter import (
-    SocketFactory,
-    ZeroMqMessage,
-    ZeroMqPushAdapter,
-)
-from tickit.core.adapter import RaiseInterrupt
-from tickit.core.device import Device
+from tickit.adapters.io.zeromq_push_io import SocketFactory, ZeroMqMessage, ZeroMqPushIo
+from tickit.adapters.zmq import ZeroMqPushAdapter
+from tickit.core.adapter import AdapterContainer, RaiseInterrupt
 
-_HOST = "test.host"
-_PORT = 12345
-
-
-@pytest.fixture
-def mock_device() -> Device:
-    return create_autospec(Device)
+_HOST = "127.0.0.1"
+_PORT = 5530
 
 
 @pytest.fixture
 def mock_raise_interrupt() -> RaiseInterrupt:
     async def raise_interrupt():
         return False
 
@@ -52,45 +42,47 @@
         return mock_socket
 
     factory = AsyncMock()
     factory.side_effect = make_socket
     return factory
 
 
-@pytest.fixture
-def zeromq_adapter(mock_socket_factory: aiozmq.ZmqStream) -> ZeroMqPushAdapter:
-    return ZeroMqPushAdapter(
+@pytest_asyncio.fixture
+async def io(mock_socket_factory: AsyncMock) -> AsyncGenerator[ZeroMqPushIo, None]:
+    io = ZeroMqPushIo(
         host=_HOST,
         port=_PORT,
         socket_factory=mock_socket_factory,
     )
+    yield io
+    await io.shutdown()
 
 
-@pytest_asyncio.fixture
-async def running_zeromq_adapter(
-    zeromq_adapter: ZeroMqPushAdapter,
-    socket_created: asyncio.Event,
-    mock_device: Device,
-    mock_raise_interrupt: RaiseInterrupt,
-) -> ZeroMqPushAdapter:
-    asyncio.create_task(zeromq_adapter.run_forever(mock_device, mock_raise_interrupt))
-    await asyncio.wait_for(socket_created.wait(), timeout=2.0)
-    return zeromq_adapter
+@pytest.fixture
+def adapter() -> ZeroMqPushAdapter:
+    return ZeroMqPushAdapter()
+
+
+@pytest.fixture
+def zeromq_adapter_container(
+    adapter: ZeroMqPushAdapter,
+    io: ZeroMqPushIo,
+) -> AdapterContainer:
+    return AdapterContainer(adapter, io)
 
 
 @pytest.mark.asyncio
 async def test_socket_not_created_until_run_forever(
-    zeromq_adapter: ZeroMqPushAdapter,
+    zeromq_adapter_container: AdapterContainer,
     mock_socket_factory: AsyncMock,
     socket_created: asyncio.Event,
-    mock_device: Device,
     mock_raise_interrupt: RaiseInterrupt,
 ) -> None:
     mock_socket_factory.assert_not_called()
-    asyncio.create_task(zeromq_adapter.run_forever(mock_device, mock_raise_interrupt))
+    asyncio.create_task(zeromq_adapter_container.run_forever(mock_raise_interrupt))
     await asyncio.wait_for(socket_created.wait(), timeout=2.0)
     mock_socket_factory.assert_called_once_with(_HOST, _PORT)
 
 
 class SimpleMessage(BaseModel):
     foo: int
     bar: str
@@ -116,40 +108,54 @@
     (
         [NestedMessage(foo=1, bar=SubMessage(baz=False))],
         [b'{"foo": 1, "bar": {"baz": false}}'],
     ),
 ]
 
 
+@pytest_asyncio.fixture
+async def running_zeromq_adapter(
+    zeromq_adapter_container: AdapterContainer,
+    socket_created: asyncio.Event,
+    mock_raise_interrupt: RaiseInterrupt,
+) -> AdapterContainer:
+    asyncio.create_task(zeromq_adapter_container.run_forever(mock_raise_interrupt))
+    await asyncio.wait_for(socket_created.wait(), timeout=2.0)
+    return zeromq_adapter_container
+
+
 @pytest.mark.asyncio
 @pytest.mark.parametrize("message,serialized_message", MESSGAGES)
 async def test_serializes_and_sends_message(
-    running_zeromq_adapter: ZeroMqPushAdapter,
+    running_zeromq_adapter: AdapterContainer,
     mock_socket: MagicMock,
     message: ZeroMqMessage,
     serialized_message: Sequence[bytes],
 ) -> None:
-    await running_zeromq_adapter.send_message(message)
+    assert isinstance(running_zeromq_adapter.io, ZeroMqPushIo)
+    await running_zeromq_adapter.io.send_message(message)
     mock_socket.write.assert_called_once_with(serialized_message)
 
 
 @pytest.mark.asyncio
 async def test_socket_cleaned_up_on_cancel(
-    mock_device: Device,
+    adapter: ZeroMqPushAdapter,
+    io: ZeroMqPushIo,
     mock_raise_interrupt: RaiseInterrupt,
 ) -> None:
-    adapter_a = ZeroMqPushAdapter()
-    adapter_b = ZeroMqPushAdapter()
-    for adapter in (adapter_a, adapter_b):
+    adapter_a = AdapterContainer(adapter, io)
+    adapter_b = AdapterContainer(adapter, io)
+
+    for container in (adapter_a, adapter_b):
         task = asyncio.create_task(
-            adapter.run_forever(
-                mock_device,
+            container.run_forever(
                 mock_raise_interrupt,
             )
         )
-        await adapter.send_message([b"test"])
+        assert isinstance(container.io, ZeroMqPushIo)
+        await container.io.send_message([b"test"])
         task.cancel()
         try:
             await task
         except asyncio.CancelledError:
             pass
         assert task.done()
```

### Comparing `tickit-0.3.0/tests/conftest.py` & `tickit-0.4.0/tests/system_tests/test_with_master.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 import asyncio
-import signal
-import sys
-from subprocess import PIPE, STDOUT, Popen
+from asyncio import AbstractEventLoop
+from pathlib import Path
+from typing import List, cast
 
+import mock
 import pytest
 import pytest_asyncio
+from mock import create_autospec
 
+from tickit.core.components.component import Component, ComponentConfig
+from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.management.event_router import InverseWiring
 from tickit.core.management.schedulers.master import MasterScheduler
-from tickit.core.runner import run_all_forever
 from tickit.core.state_interfaces.state_interface import get_interface
+from tickit.core.typedefs import ComponentException, ComponentID, PortID
+from tickit.devices.sink import SinkDevice
 from tickit.utils.configuration.loading import read_configs
 
 
-# https://docs.pytest.org/en/latest/example/parametrize.html#indirect-parametrization
 @pytest.fixture
-def tickit_process(request):
-    """Subprocess that runs ``tickit all <config_path>``."""
-    config_path: str = request.param
-    proc = Popen(
-        [sys.executable, "-m", "tickit", "all", config_path],
-        stdout=PIPE,
-        stderr=STDOUT,
-        text=True,
-    )
-    # Wait for IOC to be up
-    while True:
-        if "complete" in proc.stdout.readline():
-            break
-    yield proc
-    proc.send_signal(signal.SIGINT)
-    print(proc.communicate()[0])
+def configs_from_yaml() -> List[ComponentConfig]:
+    path_to_yaml = Path(__file__).parent / "configs" / "test_with_master.yaml"
+    return read_configs(path_to_yaml)
+
+
+@pytest.fixture
+def wiring(configs_from_yaml: List[ComponentConfig]) -> InverseWiring:
+    return InverseWiring.from_component_configs(configs_from_yaml)
+
+
+@pytest.fixture
+def components(configs_from_yaml) -> List[Component]:
+    return [config() for config in configs_from_yaml]
 
 
 @pytest_asyncio.fixture
-async def tickit_task(request):
-    """Task that runs ``tickit all <config_path>``."""
-    config_path: str = request.param
-    configs = read_configs(config_path)
-    inverse_wiring = InverseWiring.from_component_configs(configs)
-    scheduler = MasterScheduler(inverse_wiring, *get_interface("internal"))
-    t = asyncio.Task(
-        run_all_forever(
-            [c().run_forever(*get_interface("internal")) for c in configs]
-            + [scheduler.run_forever()]
+async def master_scheduler(
+    wiring: InverseWiring,
+    components: List[Component],
+    event_loop: AbstractEventLoop,
+):
+    with mock.patch(
+        "tickit.devices.sink.SinkDevice.update",
+        return_value=create_autospec(SinkDevice.update),
+    ):
+        scheduler = MasterScheduler(wiring, *get_interface("internal"))
+
+        assert scheduler.running.is_set() is False
+        run_task = event_loop.create_task(
+            asyncio.wait(
+                [
+                    event_loop.create_task(
+                        component.run_forever(*get_interface("internal"))
+                    )
+                    for component in components
+                ]
+                + [event_loop.create_task(scheduler.run_forever())]
+            )
+        )
+
+        yield scheduler
+
+    exception_task = event_loop.create_task(
+        scheduler.handle_component_exception(
+            ComponentException(
+                source=ComponentID("sim"), error=Exception(), traceback=""
+            )
         )
     )
-    # TODO: would like to await all_servers_running() here
-    await asyncio.sleep(0.5)
-    yield t
-    tasks = asyncio.tasks.all_tasks()
-    for task in tasks:
-        task.cancel()
-    try:
-        await t
-    except asyncio.CancelledError:
-        pass
 
+    await asyncio.gather(run_task, exception_task)
+    assert scheduler.running.is_set() is False
 
-@pytest.fixture
-def event_loop():
-    """Manage instance of event loop for runner test cases."""
-    try:
-        loop = asyncio.get_running_loop()
-    except RuntimeError:
-        loop = asyncio.new_event_loop()
-    yield loop
-    loop.close()
+
+@pytest.mark.asyncio
+async def test_sink_has_captured_value(
+    components: List[Component],
+    master_scheduler: MasterScheduler,
+):
+    await asyncio.wait_for(master_scheduler.running.wait(), timeout=2.0)
+
+    sink = cast(DeviceSimulation, components[1])
+
+    await asyncio.wait_for(master_scheduler.ticker.finished.wait(), timeout=2.0)
+
+    sunk_value = master_scheduler.ticker.inputs[ComponentID("sink")]
+
+    mocked_update = cast(mock.MagicMock, sink.device.update)
+    mocked_update.assert_called_once_with(0, sunk_value)
+    assert sunk_value.get(PortID("input")) == 42
```

### Comparing `tickit-0.3.0/tests/core/components/test_component.py` & `tickit-0.4.0/tests/core/components/test_component.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/components/test_device_simulation.py` & `tickit-0.4.0/tests/core/components/test_device_simulation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import asyncio
-from typing import AsyncGenerator, Iterable
+from typing import Iterable
 
 import pytest
 from immutables import Map
-from mock import AsyncMock, Mock, create_autospec, patch
+from mock import AsyncMock, MagicMock, Mock, create_autospec, patch
 
-from tickit.core.adapter import Adapter
+from tickit.adapters.io.tcp_io import TcpIo
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     Changes,
     ComponentID,
     Input,
     Output,
@@ -23,16 +24,29 @@
 @pytest.fixture
 def source() -> SourceDevice:
     source = SourceDevice(value=42)
     return source
 
 
 @pytest.fixture
-def mock_adapter() -> Mock:
-    return create_autospec(Adapter)
+def adapter() -> CommandAdapter:
+    adapter = CommandAdapter()
+    adapter.after_update = MagicMock()
+    return adapter
+
+
+@pytest.fixture
+def io() -> TcpIo:
+    return create_autospec(TcpIo)
+
+
+@pytest.fixture
+def adapter_container(adapter: CommandAdapter, io: TcpIo) -> AdapterContainer:
+    container = AdapterContainer(adapter, io)
+    return container
 
 
 @pytest.fixture
 def mock_state_producer_type() -> Mock:
     mock: Mock = create_autospec(StateProducer, instance=False)
     mock.return_value = create_autospec(StateProducer, instance=True)
     return mock
@@ -48,58 +62,45 @@
     with patch(
         "tickit.core.components.device_simulation.asyncio.wait", autospec=True
     ) as mock:
         yield mock
 
 
 @pytest.fixture
-async def patch_run_all() -> AsyncGenerator[Mock, None]:
-    with patch(
-        "tickit.core.components.device_simulation.run_all", autospec=True
-    ) as mock:
-        mock.return_value = [asyncio.create_task(asyncio.sleep(0))]
-        yield mock
-
-
-@pytest.fixture
 def device_simulation(
     source: SourceDevice,
-    mock_adapter: Adapter,
+    adapter_container: AdapterContainer,
 ) -> DeviceSimulation:
     return DeviceSimulation(
         name=ComponentID("test_device_simulation"),
         device=source,
-        adapters=[mock_adapter],
+        adapters=[adapter_container],
     )
 
 
 def test_device_simulation_constructor(device_simulation: DeviceSimulation):
     pass
 
 
 @pytest.mark.asyncio
 async def test_device_simulation_run_forever_method(
     device_simulation: DeviceSimulation,
     mock_state_producer_type: Mock,
     mock_state_consumer_type: Mock,
     patch_asyncio_wait: Mock,
 ):
-    with patch(
-        "tickit.core.components.device_simulation.run_all", autospec=True
-    ) as mock_all:
-        mock_all.return_value = [asyncio.create_task(asyncio.sleep(0))]
-        await device_simulation.run_forever(
-            mock_state_consumer_type, mock_state_producer_type
-        )
-        patch_asyncio_wait.assert_awaited_once_with(mock_all.return_value)
+    await device_simulation.run_forever(
+        mock_state_consumer_type, mock_state_producer_type  # type: ignore
+    )
+    patch_asyncio_wait.assert_awaited_once()
 
     changes = Changes(Map({PortID("foo"): 43}))
     await device_simulation.on_tick(SimTime(1), changes)
 
-    device_simulation.adapters[0].after_update.assert_called_once()  # type: ignore
+    device_simulation.adapters[0].adapter.after_update.assert_called_once()  # type: ignore # noqa: E501,
     assert device_simulation.last_outputs == {"value": 42}
     device_simulation.state_producer.produce.assert_awaited_once_with(  # type: ignore
         "tickit-test_device_simulation-out",
         Output(
             source=ComponentID("test_device_simulation"),
             time=SimTime(1),
             changes=Map({"value": 42}),  # type: ignore
```

### Comparing `tickit-0.3.0/tests/core/components/test_system_simulation.py` & `tickit-0.4.0/tests/core/components/test_system_simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import AsyncGenerator, Iterable
+from typing import Iterable
 
 import pytest
 from immutables import Map
 from mock import AsyncMock, Mock, patch
 from mock.mock import create_autospec
 
 from tickit.core.components.component import Component
@@ -73,23 +73,14 @@
 def patch_asyncio() -> Iterable[Mock]:
     with patch(
         "tickit.core.components.system_simulation.asyncio", autospec=True
     ) as mock:
         yield mock
 
 
-@pytest.fixture
-async def patch_run_all() -> AsyncGenerator[Mock, None]:
-    with patch(
-        "tickit.core.components.system_simulation.run_all", autospec=True
-    ) as mock:
-        mock.return_value = [asyncio.create_task(asyncio.sleep(0))]
-        yield mock
-
-
 @pytest.mark.asyncio
 async def test_system_simulation_methods(
     system_simulation: SystemSimulationComponent,
     mock_state_producer_type: Mock,
     mock_state_consumer_type: Mock,
 ):
     """Test the 'run_forever' and 'on_tick' methods.
```

### Comparing `tickit-0.3.0/tests/core/management/schedulers/test_base_scheduler.py` & `tickit-0.4.0/tests/core/management/schedulers/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/management/schedulers/test_master_scheduler.py` & `tickit-0.4.0/tests/core/management/schedulers/test_master_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/management/schedulers/test_slave_scheduler.py` & `tickit-0.4.0/tests/core/management/schedulers/test_slave_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/management/test_event_router.py` & `tickit-0.4.0/tests/core/management/test_event_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,31 +96,31 @@
 @pytest.fixture
 def event_router(wiring):
     return EventRouter(wiring)
 
 
 def test_wiring_unknown_out_dev(wiring_struct_4_1):
     wiring = Wiring(wiring_struct_4_1)
-    assert dict() == wiring["Out3"]
+    assert dict() == wiring[ComponentID("Out3")]
 
 
 def test_wiring_unknown_out_io(wiring_struct_4_1):
     wiring = Wiring(wiring_struct_4_1)
-    assert set() == wiring["Out1"]["Out1>2"]
+    assert set() == wiring[ComponentID("Out1")][PortID("Out1>2")]
 
 
 def test_inverse_wiring_unknown_in_dev(inverse_wiring_struct_4_1):
     inverse_wiring = InverseWiring(inverse_wiring_struct_4_1)
-    assert dict() == inverse_wiring["In2"]
+    assert dict() == inverse_wiring[ComponentID("In2")]
 
 
 def test_inverse_wiring_unknown_in_io(inverse_wiring_struct_4_1):
     inverse_wiring = InverseWiring(inverse_wiring_struct_4_1)
     with pytest.raises(KeyError):
-        inverse_wiring["In1"]["In1<3"]
+        inverse_wiring[ComponentID("In1")][PortID("In1<3")]
 
 
 def test_event_router_component_tree(event_router: EventRouter):
     assert {
         "Iso1": set(),
         "In1": set(),
         "Out1": {"Mid1"},
```

### Comparing `tickit-0.3.0/tests/core/management/test_ticker.py` & `tickit-0.4.0/tests/core/management/test_ticker.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/state_interfaces/test_internal.py` & `tickit-0.4.0/tests/core/state_interfaces/test_internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/state_interfaces/test_kafka.py` & `tickit-0.4.0/tests/core/state_interfaces/test_kafka.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/state_interfaces/test_state_interface.py` & `tickit-0.4.0/tests/core/state_interfaces/test_state_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
     add("Test", False)(TestStateConsumer)
     add("Test", False)(TestStateProducer)
     assert "Test" in interfaces()
 
 
 def test_add_non_interface_warns():
     with pytest.warns(RuntimeWarning):
-        add("Test", False)(type("TestClass", tuple(), dict()))
+        # ignore intentionally wrong type
+        add("Test", False)(type("TestClass", (), {}))  # type: ignore
 
 
 def test_get_returns_consumer(TestStateConsumer, TestStateProducer):
     add("Test", False)(TestStateConsumer)
     add("Test", False)(TestStateProducer)
     consumer, _ = get_interface("Test")
     assert consumer == TestStateConsumer
```

### Comparing `tickit-0.3.0/tests/core/test_simulation.py` & `tickit-0.4.0/tests/core/test_simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/core/test_typedefs.py` & `tickit-0.4.0/tests/core/test_typedefs.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/devices/test_iobox.py` & `tickit-0.4.0/tests/devices/test_iobox.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,26 +25,29 @@
     box.update(SimTime(0), {})
     assert "bar" == box.read(4)
 
 
 def test_outputs_change(box: IoBoxDevice[int, Any]) -> None:
     box.write(4, "foo")
     update = box.update(SimTime(0), {})
+    assert "updates" in update.outputs
     assert update.outputs["updates"] == [(4, "foo")]
 
 
 def test_outputs_only_last_changes(box: IoBoxDevice[int, Any]) -> None:
     box.write(4, "foo")
     box.update(SimTime(0), {})
     box.write(3, "bar")
     update = box.update(SimTime(0), {})
+    assert "updates" in update.outputs
     assert update.outputs["updates"] == [(3, "bar")]
 
 
 def test_writes_input(box: IoBoxDevice[int, Any]) -> None:
     box.update(SimTime(0), {"updates": [(4, "foo")]})
     assert box.read(4) == "foo"
 
 
 def test_propagates_input(box: IoBoxDevice[int, Any]) -> None:
     update = box.update(SimTime(0), {"updates": [(4, "foo")]})
+    assert "updates" in update.outputs
     assert update.outputs["updates"] == [(4, "foo")]
```

### Comparing `tickit-0.3.0/tests/devices/test_sink.py` & `tickit-0.4.0/tests/devices/test_sink.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/devices/test_source.py` & `tickit-0.4.0/tests/devices/test_source.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/test_cli.py` & `tickit-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/utils/configuration/test_loading.py` & `tickit-0.4.0/tests/utils/configuration/test_loading.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/utils/test_configurable.py` & `tickit-0.4.0/tests/utils/test_configurable.py`

 * *Files identical despite different names*

### Comparing `tickit-0.3.0/tests/utils/test_singleton.py` & `tickit-0.4.0/tests/utils/test_singleton.py`

 * *Files identical despite different names*

