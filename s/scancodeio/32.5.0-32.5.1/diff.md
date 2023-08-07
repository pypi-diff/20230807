# Comparing `tmp/scancodeio-32.5.0.tar.gz` & `tmp/scancodeio-32.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scancodeio-32.5.0.tar", last modified: Wed Aug  2 20:07:41 2023, max compression
+gzip compressed data, was "scancodeio-32.5.1.tar", last modified: Mon Aug  7 15:43:47 2023, max compression
```

## Comparing `scancodeio-32.5.0.tar` & `scancodeio-32.5.1.tar`

### file list

```diff
@@ -1,466 +1,468 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.494755 scancodeio-32.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.502755 scancodeio-32.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 20:07:32.000000 scancodeio-32.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-08-02 20:07:32.000000 scancodeio-32.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-02 20:07:32.000000 scancodeio-32.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 20:07:32.000000 scancodeio-32.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-02 20:07:32.000000 scancodeio-32.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-08-02 20:07:32.000000 scancodeio-32.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 20:07:32.000000 scancodeio-32.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-02 20:07:41.566756 scancodeio-32.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-02 20:07:32.000000 scancodeio-32.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docker.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.506755 scancodeio-32.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/application-settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/built-in-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/command-line-interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/custom-pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/data-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/distros-os-images.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.510755 scancodeio-32.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   347827 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/license-clarity-scan-summary.png
--rw-r--r--   0 runner    (1001) docker     (123)   113257 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-download-results.png
--rw-r--r--   0 runner    (1001) docker     (123)    49405 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    59030 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-xlsx-packages.png
--rw-r--r--   0 runner    (1001) docker     (123)    56604 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/output-files-xlsx-resources.png
--rw-r--r--   0 runner    (1001) docker     (123)   161773 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-extra-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    45598 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-icon-link.png
--rw-r--r--   0 runner    (1001) docker     (123)    78178 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-packages-link.png
--rw-r--r--   0 runner    (1001) docker     (123)    47458 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-license-policies-results.png
--rw-r--r--   0 runner    (1001) docker     (123)   148235 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-errors-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-charts.png
--rw-r--r--   0 runner    (1001) docker     (123)   115814 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    86303 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-project-details.png
--rw-r--r--   0 runner    (1001) docker     (123)   152148 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-project-form.png
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-project-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    50351 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-projects-list.png
--rw-r--r--   0 runner    (1001) docker     (123)   165263 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-charts.png
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)   191624 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/tutorial-web-ui-run-log-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-archive-action.png
--rw-r--r--   0 runner    (1001) docker     (123)   127740 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-archive-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)   153488 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-create-project.png
--rw-r--r--   0 runner    (1001) docker     (123)    52651 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-delete-action.png
--rw-r--r--   0 runner    (1001) docker     (123)   108653 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-delete-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)    51714 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-project-details.png
--rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-project-list-empty.png
--rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-project-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    52920 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-reset-action.png
--rw-r--r--   0 runner    (1001) docker     (123)    93458 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/images/user-interface-reset-modal.png
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/output-files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/project-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/rest-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/scanpipe-concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/scanpipe-pipes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_api_analyze_package_archive.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_cli_analyze_codebase.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_cli_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_license_policies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_vulnerablecode_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_web_ui_analyze_docker_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/tutorial_web_ui_review_scan_results.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-02 20:07:32.000000 scancodeio-32.5.0/docs/user-interface.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.494755 scancodeio-32.5.0/etc/nginx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.510755 scancodeio-32.5.0/etc/nginx/conf.d/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/nginx/conf.d/default.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.510755 scancodeio-32.5.0/etc/nginx/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/nginx/examples/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.518755 scancodeio-32.5.0/etc/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/isc.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26418 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/lgpl-2.1-plus.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/python.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)  4956245 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-02 20:07:32.000000 scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz.ABOUT
--rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-08-02 20:07:32.000000 scancodeio-32.5.0/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scan.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.518755 scancodeio-32.5.0/scancodeio/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/scan.NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.522755 scancodeio-32.5.0/scancodeio/static/
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   422462 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.20.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.20.0.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)   368864 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ace-1.9.5.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/add-inputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/billboard-3.0.1-datalab.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   465309 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/billboard-3.0.1.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   207302 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/cc-by-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.css
--rw-r--r--   0 runner    (1001) docker     (123)   133121 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/highlight.js-10.6.0.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)    15888 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)    37374 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/htmx-1.7.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/htmx-1.7.0.min.js.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/static/ofl-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scancodeio/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scancodeio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-08-02 20:07:41.000000 scancodeio-32.5.0/scancodeio.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.522755 scancodeio-32.5.0/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.522755 scancodeio-32.5.0/scanpipe/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.526755 scancodeio-32.5.0/scanpipe/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/add-input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/add-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/archive-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/create-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/create-user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/delete-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/list-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/reset-project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/show-pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/management/commands/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.530755 scancodeio-32.5.0/scanpipe/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0002_run_id_and_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0003_remove_run_run_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0004_run_pipeline_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0005_project_input_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0008_package_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0009_discoveredpackage_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0010_codebaseresource_is_key_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0011_codebaseresource_is_media.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0012_run_scancodeio_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0013_project_is_archived.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0014_webhooksubscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0016_discoveredpackage_package_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0018_codebaseresource_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0019_auto_20220804_1836.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0020_alter_codebaseresource_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0021_codebaseresource_package_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0022_create_discovereddependencies_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0023_migrate_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0026_run_current_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0028_codebaserelation_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0033_project_notes_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0034_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0035_set_projects_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0036_alter_project_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0038_migrate_vulnerability_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   103111 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.530755 scancodeio-32.5.0/scanpipe/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/deploy_to_develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/docker_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/find_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/inspect_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/load_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/populate_purldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/root_filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/scan_codebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/scan_codebase_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipelines/scan_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/codebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/js.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/pathmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/purldb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/scancode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/pipes/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    72249 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/bom-1.4.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/jsf-0.82.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    45312 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/spdx-schema-2.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/schemas/spdx.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/vulnerablecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/pipes/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/templates/account/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/account/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/registration/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.534755 scancodeio-32.5.0/scanpipe/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.538756 scancodeio-32.5.0/scanpipe/templates/scanpipe/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/app_monitoring.html
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/attribution.html
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/error_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.542755 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_inputs_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/dropdown_hoverable.html
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/file_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filter_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filter_dropdown_choices_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filter_sort.html
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/help_dropdown_tooltip.html
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/license_clarity_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_view_thead.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/navbar_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_archive_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_codebase.html
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_download_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_downloads.html
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs_delete_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_list_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_pipelines.html
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_reset_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_summary_level.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_chart_column.html
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_path_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_status_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal_content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_status_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/scan_summary_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/search_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/package_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/package_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_charts.html
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/project_settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/relation_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.542755 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/field_default.html
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/field_for_package.html
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_default.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_image.html
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_relations.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tabset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.546756 scancodeio-32.5.0/scanpipe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.558756 scancodeio-32.5.0/scanpipe/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)   218206 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/archive.zip
--rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    85063 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (123)    82019 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    86996 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
--rw-r--r--   0 runner    (1001) docker     (123)    87965 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_tree.json
--rw-r--r--   0 runner    (1001) docker     (123)    88140 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    47288 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json
--rw-r--r--   0 runner    (1001) docker     (123)  1447917 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/centos.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)  5818290 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/centos_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.558756 scancodeio-32.5.0/scanpipe/tests/data/codebase/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/codebase/a.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/codebase/b.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/codebase/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.558756 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/missing_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/nested.cdx.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/tests/data/d2d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/
--rw-r--r--   0 runner    (1001) docker     (123)    56205 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
--rw-r--r--   0 runner    (1001) docker     (123)    37100 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/Baz.class
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/Baz.java
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/find_java_packages/Foo.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/
--rw-r--r--   0 runner    (1001) docker     (123)    21813 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
--rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.498755 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/unmain.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/main.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/unmain.js
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    54605 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/debian.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/debian_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)    57175 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    25250 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)   176984 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
--rw-r--r--   0 runner    (1001) docker     (123)    81029 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/flume-ng-node-d2d.json
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/foobar.qcow2.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    62008 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1674755 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)    16287 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/jvm/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/jvm/common.java
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/jvm/no-package.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/package.expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/poor_values.ABOUT
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.json
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    30726 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/notice.NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.562756 scancodeio-32.5.0/scanpipe/tests/data/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/outputs/expected_attribution.html
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/outputs/render_me.html
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/policies.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/data/scancode/
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/scancode/package_assembly_codebase.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/data/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/settings/scancode-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/data/windows-container-rootfs.tar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/profile_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/raise_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/register_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipelines/steps_as_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:41.566756 scancodeio-32.5.0/scanpipe/tests/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_codebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_cyclonedx.py
--rw-r--r--   0 runner    (1001) docker     (123)    27970 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26917 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_pathmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_rootfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_scancode.py
--rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/pipes/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/regen_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34966 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    24121 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    90466 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    39094 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    34599 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-08-02 20:07:32.000000 scancodeio-32.5.0/scanpipe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-02 20:07:41.570756 scancodeio-32.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-08-02 20:07:32.000000 scancodeio-32.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.997349 scancodeio-32.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.905342 scancodeio-32.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.913342 scancodeio-32.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-07 15:43:35.000000 scancodeio-32.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    40013 2023-08-07 15:43:35.000000 scancodeio-32.5.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-07 15:43:35.000000 scancodeio-32.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 15:43:35.000000 scancodeio-32.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-07 15:43:35.000000 scancodeio-32.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-08-07 15:43:35.000000 scancodeio-32.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-07 15:43:35.000000 scancodeio-32.5.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-07 15:43:46.997349 scancodeio-32.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-07 15:43:35.000000 scancodeio-32.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docker.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.917343 scancodeio-32.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/application-settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/automation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/built-in-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/command-line-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/custom-pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/data-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/distros-os-images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.925343 scancodeio-32.5.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   347827 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/license-clarity-scan-summary.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113257 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/output-files-download-results.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49405 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/output-files-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59030 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/output-files-xlsx-packages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56604 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/output-files-xlsx-resources.png
+-rw-r--r--   0 runner    (1001) docker     (123)   161773 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-find-vulnerabilities-extra-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45598 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-find-vulnerabilities-icon-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78178 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-find-vulnerabilities-packages-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47458 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-license-policies-results.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148235 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-errors-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-packages-charts.png
+-rw-r--r--   0 runner    (1001) docker     (123)   115814 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-packages-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86303 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   152148 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-project-form.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50351 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-projects-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   165263 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-resources-charts.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-resources-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)   191624 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/tutorial-web-ui-run-log-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-archive-action.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127740 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-archive-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)   153488 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-create-project.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52651 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-delete-action.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108653 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-delete-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51714 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-project-details.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-project-list-empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24533 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-project-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52920 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-reset-action.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93458 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/images/user-interface-reset-modal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/output-files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/project-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/rest-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/scanpipe-concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/scanpipe-pipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_api_analyze_package_archive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_cli_analyze_codebase.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_cli_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_license_policies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_vulnerablecode_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_web_ui_analyze_docker_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/tutorial_web_ui_review_scan_results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-07 15:43:35.000000 scancodeio-32.5.1/docs/user-interface.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.905342 scancodeio-32.5.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.905342 scancodeio-32.5.1/etc/nginx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.925343 scancodeio-32.5.1/etc/nginx/conf.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/nginx/conf.d/default.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.925343 scancodeio-32.5.1/etc/nginx/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/nginx/examples/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.933344 scancodeio-32.5.1/etc/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/isc.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26418 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/lgpl-2.1-plus.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-08-07 15:43:35.000000 scancodeio-32.5.1/etc/thirdparty/python.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)  4956245 2023-08-07 15:43:36.000000 scancodeio-32.5.1/etc/thirdparty/virtualenv.pyz
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-07 15:43:36.000000 scancodeio-32.5.1/etc/thirdparty/virtualenv.pyz.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2023-08-07 15:43:36.000000 scancodeio-32.5.1/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scan.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.933344 scancodeio-32.5.1/scancodeio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/scan.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.937344 scancodeio-32.5.1/scancodeio/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/ace-1.20.0-ext-searchbox.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   422462 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/ace-1.20.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/ace-1.20.0.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)   368864 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/ace-1.9.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/add-inputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/billboard-3.0.1-datalab.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   465309 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/billboard-3.0.1.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/billboard-3.0.1.pkgd.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   207302 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/bulma-0.9.4.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/bulma-0.9.4.min.css.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/bulma-toast-2.4.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/cc-by-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/highlight-10.6.0.css
+-rw-r--r--   0 runner    (1001) docker     (123)   133121 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/highlight-10.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/highlight.js-10.6.0.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)    15888 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/html5sortable-0.9.17.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)    37374 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/htmx-1.7.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/htmx-1.7.0.min.js.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/static/ofl-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scancodeio/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.997349 scancodeio-32.5.1/scancodeio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-08-07 15:43:46.000000 scancodeio-32.5.1/scancodeio.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.941344 scancodeio-32.5.1/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.941344 scancodeio-32.5.1/scanpipe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20043 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.905342 scancodeio-32.5.1/scanpipe/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.941344 scancodeio-32.5.1/scanpipe/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/add-input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/add-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/archive-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/create-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/create-user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/delete-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/list-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/reset-project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/show-pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/management/commands/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.949345 scancodeio-32.5.1/scanpipe/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0002_run_id_and_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0003_remove_run_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0004_run_pipeline_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0005_project_input_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0006_codebaseresource_compliance_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0008_package_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0009_discoveredpackage_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0010_codebaseresource_is_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0011_codebaseresource_is_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0012_run_scancodeio_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0013_project_is_archived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0014_webhooksubscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0016_discoveredpackage_package_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0018_codebaseresource_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0019_auto_20220804_1836.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0020_alter_codebaseresource_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0021_codebaseresource_package_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0022_create_discovereddependencies_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0023_migrate_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0024_remove_discoveredpackage_dependencies_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0026_run_current_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0028_codebaserelation_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0033_project_notes_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0034_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0035_set_projects_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0036_alter_project_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0038_migrate_vulnerability_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/0040_discovereddependency_affected_by_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103698 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.949345 scancodeio-32.5.1/scanpipe/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/deploy_to_develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/docker_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/find_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/inspect_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/load_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/populate_purldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/root_filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/scan_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/scan_codebase_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipelines/scan_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.953345 scancodeio-32.5.1/scanpipe/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/codebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30444 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/purldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/scancode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.953345 scancodeio-32.5.1/scanpipe/pipes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    72249 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/schemas/bom-1.4.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/schemas/jsf-0.82.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45312 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/schemas/spdx-schema-2.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/schemas/spdx.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/vulnerablecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/pipes/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.909342 scancodeio-32.5.1/scanpipe/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.953345 scancodeio-32.5.1/scanpipe/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/account/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.953345 scancodeio-32.5.1/scanpipe/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/registration/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.953345 scancodeio-32.5.1/scanpipe/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.957346 scancodeio-32.5.1/scanpipe/templates/scanpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/app_monitoring.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/attribution.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/dependency_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/dependency_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/error_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.961346 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/add_inputs_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/dropdown_hoverable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/file_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/filter_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/filter_dropdown_choices_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/filter_sort.html
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/filters_breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/help_dropdown_tooltip.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/license_clarity_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/list_view_thead.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/navbar_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/pagination_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/pagination_header_relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_archive_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_codebase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_download_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_downloads.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_inputs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_inputs_delete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_list_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_pipelines.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_reset_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_settings_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_summary_level.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/resource_chart_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/resource_file_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/resource_path_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/resource_status_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/run_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/run_modal_content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/run_status_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/scan_summary_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/search_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/package_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/package_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/project_charts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/project_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/project_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/project_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/project_settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/relation_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/resource_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/resource_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.965346 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/field_datafile_resource.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/field_default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/field_for_package.html
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_content_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_dependencies.html
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tabset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.965346 scancodeio-32.5.1/scanpipe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.985348 scancodeio-32.5.1/scanpipe/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/alpine_3_15_4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   218206 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/archive.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85063 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82183 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    86996 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    87965 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_tree.json
+-rw-r--r--   0 runner    (1001) docker     (123)    88140 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/basic-rootfs.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32303 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/basic-rootfs_root_filesystems.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1447917 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/centos.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  5818290 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/centos_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.985348 scancodeio-32.5.1/scanpipe/tests/data/codebase/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/codebase/a.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/codebase/b.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/codebase/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.989348 scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/missing_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/nested.cdx.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.909342 scancodeio-32.5.1/scanpipe/tests/data/d2d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.989348 scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    53745 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    37100 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/to-with-jar.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.989348 scancodeio-32.5.1/scanpipe/tests/data/d2d/find_java_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/find_java_packages/Baz.class
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/find_java_packages/Baz.java
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/find_java_packages/Foo.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.989348 scancodeio-32.5.1/scanpipe/tests/data/d2d/jars/
+-rw-r--r--   0 runner    (1001) docker     (123)    21813 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.909342 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.989348 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/from/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/from/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/from/unmain.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.989348 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/main.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/unmain.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/unmain.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    54933 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/debian.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/debian_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57175 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/decompose_l_u_8hpp_source.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-images.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25250 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   176984 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81029 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/flume-ng-node-d2d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/foobar.qcow2.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    62008 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/gcr_io_distroless_base.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1674755 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.993348 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16287 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.993348 scancodeio-32.5.1/scanpipe/tests/data/jvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/jvm/common.java
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/jvm/no-package.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.993348 scancodeio-32.5.1/scanpipe/tests/data/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/manifests/Django-4.0.8-py3-none-any.whl.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/manifests/package.expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/manifests/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/manifests/poor_values.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/manifests/toml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/manifests/toml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    30726 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/notice.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.993348 scancodeio-32.5.1/scanpipe/tests/data/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/outputs/expected_attribution.html
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/outputs/render_me.html
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/policies.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.993348 scancodeio-32.5.1/scanpipe/tests/data/scancode/
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/scancode/package_assembly_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/scancode/package_assembly_codebase.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.993348 scancodeio-32.5.1/scanpipe/tests/data/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/settings/scancode-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/data/windows-container-rootfs.tar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.997349 scancodeio-32.5.1/scanpipe/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipelines/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipelines/profile_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipelines/raise_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipelines/register_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipelines/steps_as_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:46.997349 scancodeio-32.5.1/scanpipe/tests/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_codebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_cyclonedx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28011 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26917 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_pathmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_scancode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_spdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/pipes/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/regen_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38166 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24121 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90466 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39095 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34599 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56812 2023-08-07 15:43:36.000000 scancodeio-32.5.1/scanpipe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-07 15:43:47.001349 scancodeio-32.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-08-07 15:43:36.000000 scancodeio-32.5.1/setup.py
```

### Comparing `scancodeio-32.5.0/.github/workflows/ci.yml` & `scancodeio-32.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/.github/workflows/pypi-release.yml` & `scancodeio-32.5.1/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/.gitignore` & `scancodeio-32.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/.readthedocs.yaml` & `scancodeio-32.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/CHANGELOG.rst` & `scancodeio-32.5.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 Changelog
 =========
 
+v32.5.1 (2023-08-07)
+--------------------
+
+Security release: This release addresses the security issue detailed below.
+We encourage all users of ScanCode.io to upgrade as soon as possible.
+
+- GHSA-2ggp-cmvm-f62f: Command injection in docker image fetch process
+  The ``fetch_docker_image`` function was subject to potential injection attack.
+  The user inputs are now sanitized before calling the subprocess function.
+  https://github.com/nexB/scancode.io/security/advisories/GHSA-2ggp-cmvm-f62f
+
+---
+
+- Add support for multiple input URLs, and adding multiple pipelines in the project
+  creation REST API.
+  https://github.com/nexB/scancode.io/issues/828
+
+- Update the ``fetch_vulnerabilities`` pipe to make the API requests by batch of purls.
+  https://github.com/nexB/scancode.io/issues/835
+
+- Add vulnerability support for discovered dependencies.
+  The dependency data is loaded using the ``find_vulnerabilities`` pipeline backed by
+  a VulnerableCode database.
+  https://github.com/nexB/scancode.io/issues/835
+
+- Fix root filesystem scanning for installed packages and archived Linux distributions.
+  Allows the scan to discover system packages from `rpmdb.sqlite` and other sources.
+  https://github.com/nexB/scancode.io/pull/840
+
 v32.5.0 (2023-08-02)
 --------------------
 
 WARNING: After upgrading the ScanCode.io codebase to this version,
 and following the ``docker compose build``,
 the permissions of the ``/var/scancodeio/`` directory of the Docker volumes require
 to be updated for the new ``app`` user, using:
```

### Comparing `scancodeio-32.5.0/Dockerfile` & `scancodeio-32.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/LICENSE` & `scancodeio-32.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/Makefile` & `scancodeio-32.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/NOTICE` & `scancodeio-32.5.1/NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/PKG-INFO` & `scancodeio-32.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scancodeio
-Version: 32.5.0
+Version: 32.5.1
 Summary: Automate software composition analysis pipelines
 Home-page: https://github.com/nexB/scancode.io
 Author: nexB Inc.
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,scan,license,package,dependency,copyright,filetype,author,extract,licensing,scancode,scanpipe,docker,rootfs,vm,virtual machine,pipeline,code analysis,container
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `scancodeio-32.5.0/README.rst` & `scancodeio-32.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docker-compose.yml` & `scancodeio-32.5.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/Makefile` & `scancodeio-32.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/application-settings.rst` & `scancodeio-32.5.1/docs/application-settings.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/built-in-pipelines.rst` & `scancodeio-32.5.1/docs/built-in-pipelines.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/command-line-interface.rst` & `scancodeio-32.5.1/docs/command-line-interface.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/conf.py` & `scancodeio-32.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/contributing.rst` & `scancodeio-32.5.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/custom-pipelines.rst` & `scancodeio-32.5.1/docs/custom-pipelines.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/data-models.rst` & `scancodeio-32.5.1/docs/data-models.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/distros-os-images.rst` & `scancodeio-32.5.1/docs/distros-os-images.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/faq.rst` & `scancodeio-32.5.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/license-clarity-scan-summary.png` & `scancodeio-32.5.1/docs/images/license-clarity-scan-summary.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/output-files-download-results.png` & `scancodeio-32.5.1/docs/images/output-files-download-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/output-files-projects-list.png` & `scancodeio-32.5.1/docs/images/output-files-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/output-files-xlsx-packages.png` & `scancodeio-32.5.1/docs/images/output-files-xlsx-packages.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/output-files-xlsx-resources.png` & `scancodeio-32.5.1/docs/images/output-files-xlsx-resources.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-extra-data.png` & `scancodeio-32.5.1/docs/images/tutorial-find-vulnerabilities-extra-data.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-icon-link.png` & `scancodeio-32.5.1/docs/images/tutorial-find-vulnerabilities-icon-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-find-vulnerabilities-packages-link.png` & `scancodeio-32.5.1/docs/images/tutorial-find-vulnerabilities-packages-link.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-license-policies-results.png` & `scancodeio-32.5.1/docs/images/tutorial-license-policies-results.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-errors-list.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-errors-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-charts.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-packages-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-packages-list.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-packages-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-project-details.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-project-form.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-project-form.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-project-list.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-projects-list.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-projects-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-charts.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-resources-charts.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-resources-filter.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-resources-filter.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/tutorial-web-ui-run-log-modal.png` & `scancodeio-32.5.1/docs/images/tutorial-web-ui-run-log-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-archive-action.png` & `scancodeio-32.5.1/docs/images/user-interface-archive-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-archive-modal.png` & `scancodeio-32.5.1/docs/images/user-interface-archive-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-create-project.png` & `scancodeio-32.5.1/docs/images/user-interface-create-project.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-delete-action.png` & `scancodeio-32.5.1/docs/images/user-interface-delete-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-delete-modal.png` & `scancodeio-32.5.1/docs/images/user-interface-delete-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-project-details.png` & `scancodeio-32.5.1/docs/images/user-interface-project-details.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-project-list-empty.png` & `scancodeio-32.5.1/docs/images/user-interface-project-list-empty.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-project-list.png` & `scancodeio-32.5.1/docs/images/user-interface-project-list.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-reset-action.png` & `scancodeio-32.5.1/docs/images/user-interface-reset-action.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/images/user-interface-reset-modal.png` & `scancodeio-32.5.1/docs/images/user-interface-reset-modal.png`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/index.rst` & `scancodeio-32.5.1/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     custom-pipelines
     scanpipe-pipes
     project-configuration
     data-models
     output-files
     command-line-interface
     rest-api
+    automation
     application-settings
     distros-os-images
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `scancodeio-32.5.0/docs/installation.rst` & `scancodeio-32.5.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/introduction.rst` & `scancodeio-32.5.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/make.bat` & `scancodeio-32.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/output-files.rst` & `scancodeio-32.5.1/docs/output-files.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/project-configuration.rst` & `scancodeio-32.5.1/docs/project-configuration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/rest-api.rst` & `scancodeio-32.5.1/docs/rest-api.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/scanpipe-concepts.rst` & `scancodeio-32.5.1/docs/scanpipe-concepts.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/scanpipe-pipes.rst` & `scancodeio-32.5.1/docs/scanpipe-pipes.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_api_analyze_package_archive.rst` & `scancodeio-32.5.1/docs/tutorial_api_analyze_package_archive.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_cli_analyze_codebase.rst` & `scancodeio-32.5.1/docs/tutorial_cli_analyze_codebase.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_cli_analyze_docker_image.rst` & `scancodeio-32.5.1/docs/tutorial_cli_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_license_policies.rst` & `scancodeio-32.5.1/docs/tutorial_license_policies.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_vulnerablecode_integration.rst` & `scancodeio-32.5.1/docs/tutorial_vulnerablecode_integration.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_web_ui_analyze_docker_image.rst` & `scancodeio-32.5.1/docs/tutorial_web_ui_analyze_docker_image.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/tutorial_web_ui_review_scan_results.rst` & `scancodeio-32.5.1/docs/tutorial_web_ui_review_scan_results.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/docs/user-interface.rst` & `scancodeio-32.5.1/docs/user-interface.rst`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/nginx/examples/ssl.conf` & `scancodeio-32.5.1/etc/nginx/examples/ssl.conf`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/apache-2.0.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/bsd-new.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/bsd-simplified.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/isc.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/isc.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/lgpl-2.1-plus.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/lgpl-2.1-plus.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/mit.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/python.LICENSE` & `scancodeio-32.5.1/etc/thirdparty/python.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz` & `scancodeio-32.5.1/etc/thirdparty/virtualenv.pyz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/etc/thirdparty/virtualenv.pyz.ABOUT` & `scancodeio-32.5.1/etc/thirdparty/virtualenv.pyz.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/__init__.py` & `scancodeio-32.5.1/scancodeio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import os
 import subprocess
 import sys
 import warnings
 from pathlib import Path
 
-VERSION = "32.5.0"
+VERSION = "32.5.1"
 
 PROJECT_DIR = Path(__file__).resolve().parent
 ROOT_DIR = PROJECT_DIR.parent
 SCAN_NOTICE = PROJECT_DIR.joinpath("scan.NOTICE").read_text()
 
 
 def get_version(version):
```

### Comparing `scancodeio-32.5.0/scancodeio/auth.py` & `scancodeio-32.5.1/scancodeio/auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/context_processors.py` & `scancodeio-32.5.1/scancodeio/context_processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 #
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
 from scancode_config import __version__ as scancode_toolkit_version
 
 from scancodeio import __version__ as scancodeio_version
+from scancodeio import settings
 
 
 def versions(request):
     return {
         "SCANCODEIO_VERSION": scancodeio_version.lstrip("v"),
         "SCANCODE_TOOLKIT_VERSION": scancode_toolkit_version,
+        "VULNERABLECODE_URL": settings.VULNERABLECODE_URL,
     }
```

### Comparing `scancodeio-32.5.0/scancodeio/licenses.py` & `scancodeio-32.5.1/scancodeio/licenses.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/settings.py` & `scancodeio-32.5.1/scancodeio/settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/ace-1.20.0-ext-searchbox.min.js` & `scancodeio-32.5.1/scancodeio/static/ace-1.20.0-ext-searchbox.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/ace-1.20.0.min.js` & `scancodeio-32.5.1/scancodeio/static/ace-1.20.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/ace-1.9.5.min.js` & `scancodeio-32.5.1/scancodeio/static/ace-1.9.5.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/add-inputs.js` & `scancodeio-32.5.1/scancodeio/static/add-inputs.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/billboard-3.0.1-datalab.min.css` & `scancodeio-32.5.1/scancodeio/static/billboard-3.0.1-datalab.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/billboard-3.0.1.pkgd.min.js` & `scancodeio-32.5.1/scancodeio/static/billboard-3.0.1.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/bsd-new.LICENSE` & `scancodeio-32.5.1/scancodeio/static/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/bsd-simplified.LICENSE` & `scancodeio-32.5.1/scancodeio/static/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css` & `scancodeio-32.5.1/scancodeio/static/bulma-0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/bulma-0.9.4.min.css.ABOUT` & `scancodeio-32.5.1/scancodeio/static/bulma-0.9.4.min.css.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js` & `scancodeio-32.5.1/scancodeio/static/bulma-toast-2.4.1.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT` & `scancodeio-32.5.1/scancodeio/static/bulma-toast-2.4.1.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/cc-by-4.0.LICENSE` & `scancodeio-32.5.1/scancodeio/static/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/favicon.ico` & `scancodeio-32.5.1/scancodeio/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.css` & `scancodeio-32.5.1/scancodeio/static/highlight-10.6.0.css`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/highlight-10.6.0.min.js` & `scancodeio-32.5.1/scancodeio/static/highlight-10.6.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js` & `scancodeio-32.5.1/scancodeio/static/html5sortable-0.9.17.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT` & `scancodeio-32.5.1/scancodeio/static/html5sortable-0.9.17.min.js.ABOUT`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/htmx-1.7.0.min.js` & `scancodeio-32.5.1/scancodeio/static/htmx-1.7.0.min.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/main.js` & `scancodeio-32.5.1/scancodeio/static/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/mit.LICENSE` & `scancodeio-32.5.1/scancodeio/static/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/static/ofl-1.1.LICENSE` & `scancodeio-32.5.1/scancodeio/static/ofl-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/urls.py` & `scancodeio-32.5.1/scancodeio/urls.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/worker.py` & `scancodeio-32.5.1/scancodeio/worker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio/wsgi.py` & `scancodeio-32.5.1/scancodeio/wsgi.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scancodeio.egg-info/SOURCES.txt` & `scancodeio-32.5.1/scancodeio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 setup.cfg
 setup.py
 .github/workflows/ci-docker.yml
 .github/workflows/ci.yml
 .github/workflows/pypi-release.yml
 docs/Makefile
 docs/application-settings.rst
+docs/automation.rst
 docs/built-in-pipelines.rst
 docs/changelog.rst
 docs/command-line-interface.rst
 docs/conf.py
 docs/contributing.rst
 docs/custom-pipelines.rst
 docs/data-models.rst
@@ -181,14 +182,15 @@
 scanpipe/migrations/0033_project_notes_project_settings.py
 scanpipe/migrations/0034_project_slug.py
 scanpipe/migrations/0035_set_projects_slug.py
 scanpipe/migrations/0036_alter_project_slug.py
 scanpipe/migrations/0037_discoveredpackage_vulnerability_field.py
 scanpipe/migrations/0038_migrate_vulnerability_data.py
 scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py
+scanpipe/migrations/0040_discovereddependency_affected_by_vulnerabilities.py
 scanpipe/migrations/__init__.py
 scanpipe/pipelines/__init__.py
 scanpipe/pipelines/deploy_to_develop.py
 scanpipe/pipelines/docker.py
 scanpipe/pipelines/docker_windows.py
 scanpipe/pipelines/find_vulnerabilities.py
 scanpipe/pipelines/inspect_manifest.py
```

### Comparing `scancodeio-32.5.0/scanpipe/__init__.py` & `scancodeio-32.5.1/scanpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/api/__init__.py` & `scancodeio-32.5.1/scanpipe/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/api/serializers.py` & `scancodeio-32.5.1/scanpipe/api/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,32 @@
         Load the pipeline field choices on the init class instead of the module
         import, which ensures all pipelines are first properly loaded.
         """
         super().__init__(*args, **kwargs)
         self.fields["pipeline"].choices = scanpipe_app.get_pipeline_choices()
 
 
+class OrderedMultipleChoiceField(serializers.MultipleChoiceField):
+    """Forcing outputs as list() in place of set() to keep the ordering integrity."""
+
+    def to_internal_value(self, data):
+        if isinstance(data, str) or not hasattr(data, "__iter__"):
+            self.fail("not_a_list", input_type=type(data).__name__)
+        if not self.allow_empty and len(data) == 0:
+            self.fail("empty")
+
+        return [
+            super(serializers.MultipleChoiceField, self).to_internal_value(item)
+            for item in data
+        ]
+
+    def to_representation(self, value):
+        return [self.choice_strings_to_values.get(str(item), item) for item in value]
+
+
 class RunSerializer(SerializerExcludeFieldsMixin, serializers.ModelSerializer):
     project = serializers.HyperlinkedRelatedField(
         view_name="project-detail", read_only=True
     )
 
     class Meta:
         model = Run
@@ -90,25 +108,25 @@
             "execution_time",
         ]
 
 
 class ProjectSerializer(
     ExcludeFromListViewMixin, PipelineChoicesMixin, serializers.ModelSerializer
 ):
-    pipeline = serializers.ChoiceField(
+    pipeline = OrderedMultipleChoiceField(
         choices=(),
         required=False,
         write_only=True,
     )
     execute_now = serializers.BooleanField(
         write_only=True,
         help_text="Execute pipeline now",
     )
     upload_file = serializers.FileField(write_only=True, required=False)
-    input_urls = serializers.CharField(
+    input_urls = serializers.ListField(
         write_only=True,
         required=False,
         style={"base_template": "textarea.html"},
     )
     webhook_url = serializers.CharField(write_only=True, required=False)
     next_run = serializers.CharField(source="get_next_run", read_only=True)
     runs = RunSerializer(many=True, read_only=True)
@@ -199,15 +217,15 @@
         Note that even when `execute_now` is True, the pipeline execution is always
         delayed after the actual database save and commit of the Project creation
         process, using the `transaction.on_commit` callback system.
         This ensures the Project data integrity before running any pipelines.
         """
         upload_file = validated_data.pop("upload_file", None)
         input_urls = validated_data.pop("input_urls", [])
-        pipeline = validated_data.pop("pipeline", None)
+        pipeline = validated_data.pop("pipeline", [])
         execute_now = validated_data.pop("execute_now", False)
         webhook_url = validated_data.pop("webhook_url", None)
 
         downloads, errors = fetch_urls(input_urls)
         if errors:
             raise serializers.ValidationError("Could not fetch: " + "\n".join(errors))
 
@@ -218,16 +236,16 @@
 
         if downloads:
             project.add_downloads(downloads)
 
         if webhook_url:
             project.add_webhook_subscription(webhook_url)
 
-        if pipeline:
-            project.add_pipeline(pipeline, execute_now)
+        for pipeline_name in pipeline:
+            project.add_pipeline(pipeline_name, execute_now)
 
         return project
 
 
 class CodebaseResourceSerializer(serializers.ModelSerializer):
     for_packages = serializers.JSONField()
     compliance_alert = serializers.CharField()
@@ -341,14 +359,15 @@
             "is_optional",
             "is_resolved",
             "dependency_uid",
             "for_package_uid",
             "datafile_path",
             "datasource_id",
             "package_type",
+            "affected_by_vulnerabilities",
         ]
 
 
 class CodebaseRelationSerializer(serializers.ModelSerializer):
     from_resource = serializers.ReadOnlyField(source="from_resource.path")
     to_resource = serializers.ReadOnlyField(source="to_resource.path")
```

### Comparing `scancodeio-32.5.0/scanpipe/api/views.py` & `scancodeio-32.5.1/scanpipe/api/views.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/apps.py` & `scancodeio-32.5.1/scanpipe/apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/filters.py` & `scancodeio-32.5.1/scanpipe/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,14 +559,15 @@
     dropdown_widget_fields = [
         "type",
         "scope",
         "is_runtime",
         "is_optional",
         "is_resolved",
         "datasource_id",
+        "is_vulnerable",
     ]
 
     search = django_filters.CharFilter(
         label="Search", field_name="name", lookup_expr="icontains"
     )
     sort = django_filters.OrderingFilter(
         label="Sort",
@@ -585,14 +586,15 @@
     purl = PackageURLFilter(label="Package URL")
     type = ParentAllValuesFilter()
     scope = ParentAllValuesFilter()
     datasource_id = ParentAllValuesFilter()
     is_runtime = StrictBooleanFilter()
     is_optional = StrictBooleanFilter()
     is_resolved = StrictBooleanFilter()
+    is_vulnerable = IsVulnerable(field_name="affected_by_vulnerabilities")
 
     class Meta:
         model = DiscoveredDependency
         fields = [
             "search",
             "purl",
             "dependency_uid",
@@ -603,14 +605,15 @@
             "qualifiers",
             "subpath",
             "scope",
             "is_runtime",
             "is_optional",
             "is_resolved",
             "datasource_id",
+            "is_vulnerable",
         ]
 
 
 class ErrorFilterSet(FilterSetUtilsMixin, django_filters.FilterSet):
     search = django_filters.CharFilter(
         label="Search", field_name="message", lookup_expr="icontains"
     )
```

### Comparing `scancodeio-32.5.0/scanpipe/forms.py` & `scancodeio-32.5.1/scanpipe/forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/__init__.py` & `scancodeio-32.5.1/scanpipe/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/add-input.py` & `scancodeio-32.5.1/scanpipe/management/commands/add-input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/add-pipeline.py` & `scancodeio-32.5.1/scanpipe/management/commands/add-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/archive-project.py` & `scancodeio-32.5.1/scanpipe/management/commands/archive-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/create-project.py` & `scancodeio-32.5.1/scanpipe/management/commands/create-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/create-user.py` & `scancodeio-32.5.1/scanpipe/management/commands/create-user.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/delete-project.py` & `scancodeio-32.5.1/scanpipe/management/commands/delete-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/execute.py` & `scancodeio-32.5.1/scanpipe/management/commands/execute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/graph.py` & `scancodeio-32.5.1/scanpipe/management/commands/graph.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/list-project.py` & `scancodeio-32.5.1/scanpipe/management/commands/list-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/output.py` & `scancodeio-32.5.1/scanpipe/management/commands/output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/reset-project.py` & `scancodeio-32.5.1/scanpipe/management/commands/reset-project.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/show-pipeline.py` & `scancodeio-32.5.1/scanpipe/management/commands/show-pipeline.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/management/commands/status.py` & `scancodeio-32.5.1/scanpipe/management/commands/status.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0001_initial.py` & `scancodeio-32.5.1/scanpipe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0002_run_id_and_log.py` & `scancodeio-32.5.1/scanpipe/migrations/0002_run_id_and_log.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0004_run_pipeline_name.py` & `scancodeio-32.5.1/scanpipe/migrations/0004_run_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0006_codebaseresource_compliance_alert.py` & `scancodeio-32.5.1/scanpipe/migrations/0006_codebaseresource_compliance_alert.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py` & `scancodeio-32.5.1/scanpipe/migrations/0007_resource_is_binary_is_text_is_archive.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0008_package_extra_data.py` & `scancodeio-32.5.1/scanpipe/migrations/0008_package_extra_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0013_project_is_archived.py` & `scancodeio-32.5.1/scanpipe/migrations/0013_project_is_archived.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0014_webhooksubscription.py` & `scancodeio-32.5.1/scanpipe/migrations/0014_webhooksubscription.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0015_alter_codebaseresource_project_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0017_alter_discoveredpackage_package_uid_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0019_auto_20220804_1836.py` & `scancodeio-32.5.1/scanpipe/migrations/0019_auto_20220804_1836.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0022_create_discovereddependencies_model.py` & `scancodeio-32.5.1/scanpipe/migrations/0022_create_discovereddependencies_model.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0023_migrate_dependencies.py` & `scancodeio-32.5.1/scanpipe/migrations/0023_migrate_dependencies.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0025_remove_discoveredpackage_last_modified_date_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0027_remove_webhooksubscription_sent_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0028_codebaserelation_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0028_codebaserelation_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0029_codebaseresource_scanpipe_co_type_ea1dd7_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py` & `scancodeio-32.5.1/scanpipe/migrations/0030_scancode_toolkit_v32_model_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py` & `scancodeio-32.5.1/scanpipe/migrations/0031_scancode_toolkit_v32_data_updates.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py` & `scancodeio-32.5.1/scanpipe/migrations/0032_scancode_toolkit_v32_post_data_migration.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0033_project_notes_project_settings.py` & `scancodeio-32.5.1/scanpipe/migrations/0033_project_notes_project_settings.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0035_set_projects_slug.py` & `scancodeio-32.5.1/scanpipe/migrations/0035_set_projects_slug.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0038_migrate_vulnerability_data.py` & `scancodeio-32.5.1/scanpipe/migrations/0038_migrate_vulnerability_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py` & `scancodeio-32.5.1/scanpipe/migrations/0039_discoveredpackage_compliance_alert_and_more.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/models.py` & `scancodeio-32.5.1/scanpipe/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1022,14 +1022,19 @@
 
     @cached_property
     def vulnerable_package_count(self):
         """Return the number of vulnerable packages related to this project."""
         return self.discoveredpackages.vulnerable().count()
 
     @cached_property
+    def vulnerable_dependency_count(self):
+        """Return the number of vulnerable dependencies related to this project."""
+        return self.discovereddependencies.vulnerable().count()
+
+    @cached_property
     def dependency_count(self):
         """Return the number of dependencies related to this project."""
         return self.discovereddependencies.count()
 
     @cached_property
     def error_count(self):
         """Return the number of errors related to this project."""
@@ -1940,14 +1945,21 @@
     def location_path(self):
         """Return the location of the resource as a Path instance."""
         # strip the leading / to allow joining this with the codebase_path
         path = Path(str(self.path).strip("/"))
         return self.project.codebase_path / path
 
     @property
+    def name_without_extension(self):
+        """Return the name of the resource without it's extension."""
+        if self.extension:
+            return self.name.rpartition(self.extension)[0]
+        return self.name
+
+    @property
     def location(self):
         """Return the location of the resource as a string."""
         return str(self.location_path)
 
     @property
     def is_file(self):
         """Return True, if the resource is a file."""
@@ -2234,19 +2246,39 @@
             ),
         ]
 
     def __str__(self):
         return f"{self.from_resource.pk} > {self.to_resource.pk} using {self.map_type}"
 
 
-class DiscoveredPackageQuerySet(PackageURLQuerySetMixin, ProjectRelatedQuerySet):
+class VulnerabilityMixin(models.Model):
+    """Add the vulnerability related fields and methods."""
+
+    affected_by_vulnerabilities = models.JSONField(blank=True, default=list)
+
+    @property
+    def is_vulnerable(self):
+        """Returns True if this instance is affected by vulnerabilities."""
+        return bool(self.affected_by_vulnerabilities)
+
+    class Meta:
+        abstract = True
+
+
+class VulnerabilityQuerySetMixin:
     def vulnerable(self):
         return self.filter(~Q(affected_by_vulnerabilities__in=EMPTY_VALUES))
 
 
+class DiscoveredPackageQuerySet(
+    VulnerabilityQuerySetMixin, PackageURLQuerySetMixin, ProjectRelatedQuerySet
+):
+    pass
+
+
 class AbstractPackage(models.Model):
     """These fields should be kept in line with `packagedcode.models.PackageData`."""
 
     filename = models.CharField(
         max_length=255,
         blank=True,
         help_text=_(
@@ -2435,28 +2467,14 @@
         help_text=_("A list of parties such as a person, project or organization."),
     )
 
     class Meta:
         abstract = True
 
 
-class VulnerabilityMixin(models.Model):
-    """Add the vulnerability related fields and methods."""
-
-    affected_by_vulnerabilities = models.JSONField(blank=True, default=list)
-
-    @property
-    def is_vulnerable(self):
-        """Returns True if this instance is affected by vulnerabilities."""
-        return bool(self.affected_by_vulnerabilities)
-
-    class Meta:
-        abstract = True
-
-
 class DiscoveredPackage(
     ProjectRelatedModel,
     ExtraDataFieldMixin,
     SaveProjectErrorMixin,
     UpdateFromDataMixin,
     HashFieldsMixin,
     PackageURLMixin,
@@ -2735,15 +2753,17 @@
             description=self.description,
             hashes=hashes,
             properties=properties,
             external_references=external_references,
         )
 
 
-class DiscoveredDependencyQuerySet(PackageURLQuerySetMixin, ProjectRelatedQuerySet):
+class DiscoveredDependencyQuerySet(
+    PackageURLQuerySetMixin, VulnerabilityQuerySetMixin, ProjectRelatedQuerySet
+):
     def prefetch_for_serializer(self):
         """
         Optimized prefetching for a QuerySet to be consumed by the
         `DiscoveredDependencySerializer`.
         Only the fields required by the serializer are fetched on the relations.
         """
         return self.prefetch_related(
@@ -2756,14 +2776,15 @@
         )
 
 
 class DiscoveredDependency(
     ProjectRelatedModel,
     SaveProjectErrorMixin,
     UpdateFromDataMixin,
+    VulnerabilityMixin,
     PackageURLMixin,
 ):
     """
     A project's Discovered Dependencies are records of the dependencies used by
     system and application packages discovered in the code under analysis.
     """
 
@@ -2941,15 +2962,15 @@
         )
 
     @property
     def spdx_id(self):
         return f"SPDXRef-scancodeio-{self._meta.model_name}-{self.dependency_uid}"
 
     def as_spdx(self):
-        """Return this Package as an SPDX Package entry."""
+        """Return this Dependency as an SPDX Package entry."""
         from scanpipe.pipes import spdx
 
         external_refs = []
 
         if package_url := self.package_url:
             external_refs.append(
                 spdx.ExternalRef(
```

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/__init__.py` & `scancodeio-32.5.1/scanpipe/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/deploy_to_develop.py` & `scancodeio-32.5.1/scanpipe/pipelines/deploy_to_develop.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,10 +171,9 @@
     def flag_mapped_resources_and_ignored_directories(self):
         """Flag all codebase resources that were mapped during the pipeline."""
         flag.flag_mapped_resources(self.project)
         flag.flag_ignored_directories(self.project)
 
     def scan_mapped_from_for_files(self):
         """Scan mapped ``from/`` files for copyrights, licenses, emails, and urls."""
-        resource_qs = self.project.codebaseresources
-        mapped_from_files = resource_qs.from_codebase().files().has_relation()
-        scancode.scan_for_files(self.project, mapped_from_files)
+        scan_files = d2d.get_from_files_for_scanning(self.project.codebaseresources)
+        scancode.scan_for_files(self.project, scan_files)
```

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/docker.py` & `scancodeio-32.5.1/scanpipe/pipelines/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/docker_windows.py` & `scancodeio-32.5.1/scanpipe/pipelines/docker_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/find_vulnerabilities.py` & `scancodeio-32.5.1/scanpipe/pipelines/find_vulnerabilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,31 +22,37 @@
 
 from scanpipe.pipelines import Pipeline
 from scanpipe.pipes import vulnerablecode
 
 
 class FindVulnerabilities(Pipeline):
     """
-    Find vulnerabilities for discovered packages in the VulnerableCode database.
+    Find vulnerabilities for packages and dependencies in the VulnerableCode database.
 
-    Vulnerability data is stored on each package instance.
+    Vulnerability data is stored on each package and dependency instance.
     """
 
     @classmethod
     def steps(cls):
         return (
             cls.check_vulnerablecode_service_availability,
-            cls.lookup_vulnerabilities,
+            cls.lookup_packages_vulnerabilities,
+            cls.lookup_dependencies_vulnerabilities,
         )
 
     def check_vulnerablecode_service_availability(self):
         """Check if the VulnerableCode service if configured and available."""
         if not vulnerablecode.is_configured():
             raise Exception("VulnerableCode is not configured.")
 
         if not vulnerablecode.is_available():
             raise Exception("VulnerableCode is not available.")
 
-    def lookup_vulnerabilities(self):
+    def lookup_packages_vulnerabilities(self):
         """Check for vulnerabilities for each of the project's discovered package."""
         packages = self.project.discoveredpackages.all()
-        vulnerablecode.fetch_vulnerabilities(packages)
+        vulnerablecode.fetch_vulnerabilities(packages, logger=self.log)
+
+    def lookup_dependencies_vulnerabilities(self):
+        """Check for vulnerabilities for each of the project's discovered dependency."""
+        dependencies = self.project.discovereddependencies.filter(is_resolved=True)
+        vulnerablecode.fetch_vulnerabilities(dependencies, logger=self.log)
```

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/inspect_manifest.py` & `scancodeio-32.5.1/scanpipe/pipelines/inspect_manifest.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/load_inventory.py` & `scancodeio-32.5.1/scanpipe/pipelines/load_inventory.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/populate_purldb.py` & `scancodeio-32.5.1/scanpipe/pipelines/populate_purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/root_filesystems.py` & `scancodeio-32.5.1/scanpipe/pipelines/root_filesystems.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/scan_codebase.py` & `scancodeio-32.5.1/scanpipe/pipelines/scan_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/scan_codebase_package.py` & `scancodeio-32.5.1/scanpipe/pipelines/scan_codebase_package.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipelines/scan_package.py` & `scancodeio-32.5.1/scanpipe/pipelines/scan_package.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/__init__.py` & `scancodeio-32.5.1/scanpipe/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/codebase.py` & `scancodeio-32.5.1/scanpipe/pipes/codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/compliance.py` & `scancodeio-32.5.1/scanpipe/pipes/compliance.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/cyclonedx.py` & `scancodeio-32.5.1/scanpipe/pipes/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/d2d.py` & `scancodeio-32.5.1/scanpipe/pipes/d2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,23 @@
         ]
         if subpath_matches:
             return subpath_matches
 
     return matches
 
 
+def get_from_files_for_scanning(resources):
+    """
+    Return resources in the "from/" side which has been mapped to the "to/"
+    side, but are not mapped using ABOUT files.
+    """
+    mapped_from_files = resources.from_codebase().files().has_relation()
+    return mapped_from_files.filter(~Q(status=flag.ABOUT_MAPPED))
+
+
 def _map_checksum_resource(to_resource, from_resources, checksum_field):
     checksum_value = getattr(to_resource, checksum_field)
     matches = from_resources.filter(**{checksum_field: checksum_value})
     for match in get_best_path_matches(to_resource, matches):
         pipes.make_relation(
             from_resource=match,
             to_resource=to_resource,
@@ -640,16 +649,16 @@
     for to_resource in codebase_resources:
         pipes.make_relation(
             from_resource=about_file_resource,
             to_resource=to_resource,
             map_type="about_file",
         )
 
-    codebase_resources.update(status=flag.MAPPED)
-    about_file_resource.update(status=flag.MAPPED)
+    codebase_resources.update(status=flag.ABOUT_MAPPED)
+    about_file_resource.update(status=flag.ABOUT_MAPPED)
 
 
 def map_about_files(project, logger=None):
     """Map ``from/`` .ABOUT files to their related ``to/`` resources."""
     project_resources = project.codebaseresources
     from_files = project_resources.files().from_codebase()
     from_about_files = from_files.filter(extension=".ABOUT")
@@ -660,22 +669,29 @@
             f"Mapping {from_about_files.count():,d} .ABOUT files found in the from/ "
             f"codebase."
         )
 
     for about_file_resource in from_about_files:
         _map_about_file_resource(project, about_file_resource, to_resources)
 
+        about_file_companions = (
+            about_file_resource.siblings()
+            .filter(name__startswith=about_file_resource.name_without_extension)
+            .filter(extension__in=[".LICENSE", ".NOTICE"])
+        )
+        about_file_companions.update(status=flag.ABOUT_MAPPED)
+
 
 def map_javascript_post_purldb_match(project, logger=None):
     """Map minified javascript file based on existing PurlDB match."""
     project_files = project.codebaseresources.files()
 
     to_resources = project_files.to_codebase()
 
-    to_resources_dot_map = to_resources.filter(status="matched-to-purldb").filter(
+    to_resources_dot_map = to_resources.filter(status=flag.MATCHED_TO_PURLDB).filter(
         extension=".map"
     )
 
     to_resources_minified = to_resources.no_status().filter(
         extension__in=[".css", ".js"]
     )
```

### Comparing `scancodeio-32.5.0/scanpipe/pipes/docker.py` & `scancodeio-32.5.1/scanpipe/pipes/docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/fetch.py` & `scancodeio-32.5.1/scanpipe/pipes/fetch.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # ScanCode.io is a free software code scanning tool from nexB Inc. and others.
 # Visit https://github.com/nexB/scancode.io for support and download.
 
 import cgi
 import json
 import logging
 import os
+import re
 import tempfile
 from collections import namedtuple
 from pathlib import Path
 from urllib.parse import urlparse
 
 import requests
 from commoncode import command
@@ -186,24 +187,27 @@
     """
     Fetch a docker image from the provided Docker image `docker_reference`
     docker:// reference URL. Return a `download` object.
 
     Docker references are documented here:
     https://github.com/containers/skopeo/blob/0faf16017/docs/skopeo.1.md#image-names
     """
+    whitelist = r"^docker://[a-zA-Z0-9_.:/@-]+$"
+    if not re.match(whitelist, docker_reference):
+        raise ValueError("Invalid Docker reference.")
+
     name = python_safe_name(docker_reference.replace("docker://", ""))
     filename = f"{name}.tar"
     download_directory = to or tempfile.mkdtemp()
     output_file = Path(download_directory, filename)
     target = f"docker-archive:{output_file}"
-
     skopeo_executable = _get_skopeo_location()
+
     platform_args = []
-    platform = get_docker_image_platform(docker_reference)
-    if platform:
+    if platform := get_docker_image_platform(docker_reference):
         os, arch, variant = platform
         if os:
             platform_args.append(f"--override-os={os}")
         if arch:
             platform_args.append(f"--override-arch={arch}")
         if variant:
             platform_args.append(f"--override-variant={variant}")
```

### Comparing `scancodeio-32.5.0/scanpipe/pipes/flag.py` & `scancodeio-32.5.1/scanpipe/pipes/flag.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 IGNORED_NOT_INTERESTING = "ignored-not-interesting"
 IGNORED_DEFAULT_IGNORES = "ignored-default-ignores"
 IGNORED_DATA_FILE_NO_CLUES = "ignored-data-file-no-clues"
 
 COMPLIANCE_LICENSES = "compliance-licenses"
 COMPLIANCE_SOURCEMIRROR = "compliance-sourcemirror"
 
+ABOUT_MAPPED = "about-mapped"
 MAPPED = "mapped"
 MATCHED_TO_PURLDB = "matched-to-purldb"
 TOO_MANY_MAPS = "too-many-maps"
 NO_JAVA_SOURCE = "no-java-source"
 
 
 def flag_empty_files(project):
```

### Comparing `scancodeio-32.5.0/scanpipe/pipes/input.py` & `scancodeio-32.5.1/scanpipe/pipes/input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/js.py` & `scancodeio-32.5.1/scanpipe/pipes/js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/jvm.py` & `scancodeio-32.5.1/scanpipe/pipes/jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/output.py` & `scancodeio-32.5.1/scanpipe/pipes/output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/pathmap.py` & `scancodeio-32.5.1/scanpipe/pipes/pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/purldb.py` & `scancodeio-32.5.1/scanpipe/pipes/purldb.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/resolve.py` & `scancodeio-32.5.1/scanpipe/pipes/resolve.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/rootfs.py` & `scancodeio-32.5.1/scanpipe/pipes/rootfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,16 @@
 
     missing_resources = created_package.missing_resources[:]
     modified_resources = created_package.modified_resources[:]
 
     codebase_resources = project.codebaseresources.all()
 
     for install_file in installed_files:
-        rootfs_path = pipes.normalize_path(install_file.path)
+        install_file_path = install_file.get_path(strip_root=True)
+        rootfs_path = pipes.normalize_path(install_file_path)
         logger.info(f"   installed file rootfs_path: {rootfs_path}")
 
         try:
             codebase_resource = codebase_resources.get(
                 rootfs_path=rootfs_path,
             )
         except ObjectDoesNotExist:
```

### Comparing `scancodeio-32.5.0/scanpipe/pipes/scancode.py` & `scancodeio-32.5.1/scanpipe/pipes/scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/schemas/bom-1.4.schema.json` & `scancodeio-32.5.1/scanpipe/pipes/schemas/bom-1.4.schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/schemas/jsf-0.82.schema.json` & `scancodeio-32.5.1/scanpipe/pipes/schemas/jsf-0.82.schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/schemas/spdx-schema-2.3.json` & `scancodeio-32.5.1/scanpipe/pipes/schemas/spdx-schema-2.3.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/schemas/spdx.schema.json` & `scancodeio-32.5.1/scanpipe/pipes/schemas/spdx.schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/spdx.py` & `scancodeio-32.5.1/scanpipe/pipes/spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/pipes/vulnerablecode.py` & `scancodeio-32.5.1/scanpipe/pipes/vulnerablecode.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,19 +68,30 @@
     except requests.exceptions.RequestException as request_exception:
         logger.debug(f"{label} is_available() error: {request_exception}")
         return False
 
     return response.status_code == requests.codes.ok
 
 
-def get_purls(packages):
+def chunked(iterable, chunk_size):
     """
-    Return the PURLs for the given list of `packages`.
-    Do not include qualifiers nor subpath when `base` is provided.
+    Break an `iterable` into lists of `chunk_size` length.
+
+    >>> list(chunked([1, 2, 3, 4, 5], 2))
+    [[1, 2], [3, 4], [5]]
+    >>> list(chunked([1, 2, 3, 4, 5], 3))
+    [[1, 2, 3], [4, 5]]
     """
+    for index in range(0, len(iterable), chunk_size):
+        end = index + chunk_size
+        yield iterable[index:end]
+
+
+def get_purls(packages):
+    """Return the PURLs for the given list of `packages`."""
     return [package_url for package in packages if (package_url := package.package_url)]
 
 
 def request_get(
     url,
     payload=None,
     timeout=None,
@@ -164,14 +175,15 @@
     api_url=VULNERABLECODE_API_URL,
 ):
     """Bulk search of vulnerabilities using the provided list of `purls`."""
     url = f"{api_url}packages/bulk_search"
 
     data = {
         "purls": purls,
+        "vulnerabilities_only": True,
     }
 
     logger.debug(f"VulnerableCode: url={url} purls_count={len(purls)}")
     return request_post(url, data, timeout)
 
 
 def bulk_search_by_cpes(
@@ -186,36 +198,37 @@
         "cpes": cpes,
     }
 
     logger.debug(f"VulnerableCode: url={url} cpes_count={len(cpes)}")
     return request_post(url, data, timeout)
 
 
-def get_unique_vulnerabilities(packages_data):
+def fetch_vulnerabilities(packages, chunk_size=1000, logger=logger.info):
     """
-    Return the unique instance of vulnerabilities for the provided ``packages_data``.
-
-    Note this should be implemented on the VulnerableCode side, see:
-    https://github.com/nexB/vulnerablecode/issues/1219#issuecomment-1620123301
+    Fetch and store vulnerabilities for each provided ``packages``.
+    The PURLs are used for the lookups in batch of ``chunk_size`` per request.
     """
-    if not packages_data:
-        return
-
-    unique_vulnerabilities = []
-    seen_vulnerability_ids = set()
-
-    for package_entry in packages_data:
-        for vulnerability in package_entry.get("affected_by_vulnerabilities", []):
-            vulnerability_id = vulnerability.get("vulnerability_id")
-            if vulnerability_id not in seen_vulnerability_ids:
-                unique_vulnerabilities.append(vulnerability)
-                seen_vulnerability_ids.add(vulnerability_id)
-
-    return unique_vulnerabilities
+    vulnerabilities_by_purl = {}
 
+    for purls_batch in chunked(get_purls(packages), chunk_size):
+        response_data = bulk_search_by_purl(purls_batch)
+        for vulnerability_data in response_data:
+            vulnerabilities_by_purl[vulnerability_data["purl"]] = vulnerability_data
 
-def fetch_vulnerabilities(packages):
-    """Fetch and store vulnerabilities for each provided ``packages``."""
+    unsaved_objects = []
     for package in packages:
-        if packages_data := get_vulnerabilities_by_purl(package.package_url):
-            if unique_vulnerabilities := get_unique_vulnerabilities(packages_data):
-                package.update(affected_by_vulnerabilities=unique_vulnerabilities)
+        if package_data := vulnerabilities_by_purl.get(package.package_url):
+            if affected_by := package_data.get("affected_by_vulnerabilities", []):
+                package.affected_by_vulnerabilities = affected_by
+                unsaved_objects.append(package)
+
+    if unsaved_objects:
+        model_class = unsaved_objects[0].__class__
+        model_class.objects.bulk_update(
+            objs=unsaved_objects,
+            fields=["affected_by_vulnerabilities"],
+            batch_size=1000,
+        )
+        logger(
+            f"{len(unsaved_objects)} {model_class._meta.verbose_name_plural} updated "
+            f"with vulnerability data."
+        )
```

### Comparing `scancodeio-32.5.0/scanpipe/pipes/windows.py` & `scancodeio-32.5.1/scanpipe/pipes/windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tasks.py` & `scancodeio-32.5.1/scanpipe/tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/account/profile.html` & `scancodeio-32.5.1/scanpipe/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/registration/login.html` & `scancodeio-32.5.1/scanpipe/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/rest_framework/api.html` & `scancodeio-32.5.1/scanpipe/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/app_monitoring.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/app_monitoring.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/attribution.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/base.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/base.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_detail.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/dependency_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/dependency_list.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/dependency_list.html`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     <table class="table is-bordered is-striped is-narrow is-hoverable is-fullwidth">
       {% include 'scanpipe/includes/list_view_thead.html' %}
       <tbody>
         {% for dependency in object_list %}
           <tr class="break-word">
             <td style="min-width: 300px;" title="{{ dependency.dependency_uid }}">
               <a href="{{ dependency.get_absolute_url }}">{{ dependency.purl }}</a>
+              {% if dependency.is_vulnerable %}
+                <a href="{{ dependency.get_absolute_url }}#vulnerabilities">
+                  <i class="fa-solid fa-bug fa-sm has-text-danger" title="Vulnerabilities"></i>
+                </a>
+              {% endif %}
             </td>
             <td>
               <a href="?type={{ dependency.type }}" class="is-black-link">{{ dependency.type }}</a>
             </td>
             <td>
               {{ dependency.extracted_requirement }}
             </td>
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
 { project.name }} - Dependencies{% endblock %} {% block content %}
 {% include 'scanpipe/includes/navbar_header.html' %}
 {% include 'scanpipe/includes/breadcrumb.html' with linked_project=True
 current="Dependencies" %} {% include 'scanpipe/includes/search_field.html' with
 extra_class="is-small" %}
 {% include 'scanpipe/includes/pagination_header.html' %} {% include 'scanpipe/
 includes/filters_breadcrumb.html' with filterset=filter only %}
-{               {               {                                {                {                     {                      {                      {% if                       {% if                             {
-{               {               {                                {                {                     {                      {                      dependency.for_package %} { dependency.datafile_resource %} { {
-dependency.purl dependency.type dependency.extracted_requirement dependency.scope dependency.is_runtime dependency.is_optional dependency.is_resolved {                           {                                 dependency.datasource_id
-}}              }}              }}                               }}               }}                    }}                     }}                     dependency.for_package.purl dependency.datafile_resource.name }}
-                                                                                                                                                      }} {% endif %}              }} {% endif %}
+{{_dependency.purl_}} {% {               {                                {                {                     {                      {                      {% if                       {% if                             {
+if                       {               {                                {                {                     {                      {                      dependency.for_package %} { dependency.datafile_resource %} { {
+dependency.is_vulnerable dependency.type dependency.extracted_requirement dependency.scope dependency.is_runtime dependency.is_optional dependency.is_resolved {                           {                                 dependency.datasource_id
+%}  {% endif %}          }}              }}                               }}               }}                    }}                     }}                     dependency.for_package.purl dependency.datafile_resource.name }}
+                                                                                                                                                               }} {% endif %}              }} {% endif %}
 No Dependencies found. Clear_search_and_filters
 {% if is_paginated %} {% include 'scanpipe/includes/pagination.html' with
 page_obj=page_obj %} {% endif %}
 {% endblock %}
```

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/error_list.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/error_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_inputs_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/add_inputs_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/add_pipeline_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/breadcrumb_detail_view.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/file_filter.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/file_filter.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/license_clarity_panel.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/license_clarity_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/list_actions_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/list_view_thead.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/list_view_thead.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/navbar_header.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/navbar_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/pagination_header.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/pagination_header.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_archive_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_archive_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_codebase.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_codebase.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_delete_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_download_dropdown.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_download_dropdown.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_downloads.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_downloads.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_inputs.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_inputs_delete_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_inputs_delete_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_list_table.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_list_table.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_pipelines.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_pipelines.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_reset_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_reset_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_settings_menu.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_settings_menu.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/project_summary_level.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/project_summary_level.html`

 * *Files 21% similar despite different names*

```diff
@@ -19,19 +19,25 @@
         {% endif %}
       </p>
     </div>
   </div>
   <div class="level-item has-text-centered">
     <div>
       <p class="heading">Dependencies</p>
-      <p class="{{ title_class }}">
+      <p class="{{ title_class }} is-flex is-align-items-center is-justify-content-center">
         {% if project.dependency_count %}
           <a href="{% url 'project_dependencies' project.slug %}">
             {{ project.dependency_count|intcomma }}
           </a>
+          {% if project.vulnerable_dependency_count %}
+            <a href="{% url 'project_dependencies' project.slug %}?is_vulnerable=yes" class="has-text-danger is-size-5 ml-2">
+              {{ project.vulnerable_dependency_count|intcomma }}
+              <i class="fa-solid fa-bug is-size-6"></i>
+            </a>
+          {% endif %}
         {% else %}
           <span>0</span>
         {% endif %}
       </p>
     </div>
   </div>
   <div class="level-item has-text-centered">
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
 {% load humanize %}
 Packages
 {% if project.package_count %} {{_project.package_count|intcomma_}} {% if
 project.vulnerable_package_count %}
 {{_project.vulnerable_package_count|intcomma_}}
  {% endif %} {% else %} 0 {% endif %}
 Dependencies
-{% if project.dependency_count %} {{_project.dependency_count|intcomma_}} {%
-else %} 0 {% endif %}
+{% if project.dependency_count %} {{_project.dependency_count|intcomma_}} {% if
+project.vulnerable_dependency_count %}
+{{_project.vulnerable_dependency_count|intcomma_}}
+ {% endif %} {% else %} 0 {% endif %}
 Resources
 {% if project.resource_count %} {{_project.resource_count|intcomma_}} {% else
 %} 0 {% endif %}
 {% if project.relation_count %}
 Relations
 {{_project.relation_count|intcomma_}}
 {% endif %}
```

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/resource_file_viewer.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/resource_file_viewer.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/run_modal.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_modal_content.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/run_modal_content.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/run_status_tag.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/run_status_tag.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/scan_summary_panel.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/scan_summary_panel.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/includes/search_field.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/includes/search_field.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/package_detail.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/package_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/package_list.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/package_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_charts.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/project_charts.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_detail.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/project_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_form.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/project_form.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_list.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/project_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/project_settings.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/project_settings.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/relation_list.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/relation_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_detail.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/resource_detail.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/resource_list.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/resource_list.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_dependencies.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_dependencies.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_packages.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_packages.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_relations.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_relations.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_resources.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_resources.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tab_vulnerabilities.html`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         <th style="width: 210px;">Aliases</th>
       </tr>
     </thead>
     <tbody>
       {% for vulnerability in tab_data.fields.affected_by_vulnerabilities.value %}
         <tr>
           <td>
-            <a href="{{ vulnerablecode_url }}vulnerabilities/{{ vulnerability.vulnerability_id }}" target="_blank">
+            <a href="{{ VULNERABLECODE_URL }}vulnerabilities/{{ vulnerability.vulnerability_id }}" target="_blank">
               {{ vulnerability.vulnerability_id }}
               <i class="fa-solid fa-up-right-from-square is-small"></i>
             </a>
           </td>
           <td>
             {{ vulnerability.summary }}
           </td>
```

### Comparing `scancodeio-32.5.0/scanpipe/templates/scanpipe/tabset/tabset.html` & `scancodeio-32.5.1/scanpipe/templates/scanpipe/tabset/tabset.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/__init__.py` & `scancodeio-32.5.1/scanpipe/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/alpine_3_15_4.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/alpine_3_15_4_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/archive.zip` & `scancodeio-32.5.1/scanpipe/tests/data/archive.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0.spdx.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_fixtures.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_load_inventory_expected.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666666%*

 * *Differences: {"'dependencies'": "{0: {'affected_by_vulnerabilities': []}, 1: {'affected_by_vulnerabilities': "*

 * *                   "[]}, 2: {'affected_by_vulnerabilities': []}, 3: "*

 * *                   "{'affected_by_vulnerabilities': []}}"}*

```diff
@@ -1,49 +1,53 @@
 {
     "dependencies": [
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "asgiref-3.3.0-py3-none-any.whl",
             "datasource_id": "pypi_wheel",
             "dependency_uid": "pkg:pypi/pytest?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "pytest; extra == \"tests\"",
             "for_package_uid": "pkg:pypi/asgiref@3.3.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/pytest",
             "scope": "tests"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "asgiref-3.3.0-py3-none-any.whl-extract/asgiref-3.3.0.dist-info/METADATA",
             "datasource_id": "pypi_wheel_metadata",
             "dependency_uid": "pkg:pypi/pytest?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "pytest; extra == \"tests\"",
             "for_package_uid": "pkg:pypi/asgiref@3.3.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/pytest",
             "scope": "tests"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "asgiref-3.3.0-py3-none-any.whl",
             "datasource_id": "pypi_wheel",
             "dependency_uid": "pkg:pypi/pytest-asyncio?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "pytest-asyncio; extra == \"tests\"",
             "for_package_uid": "pkg:pypi/asgiref@3.3.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/pytest-asyncio",
             "scope": "tests"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "asgiref-3.3.0-py3-none-any.whl-extract/asgiref-3.3.0.dist-info/METADATA",
             "datasource_id": "pypi_wheel_metadata",
             "dependency_uid": "pkg:pypi/pytest-asyncio?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "pytest-asyncio; extra == \"tests\"",
             "for_package_uid": "pkg:pypi/asgiref@3.3.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_scanpipe_output.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_toolkit_scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_tree.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_tree.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json` & `scancodeio-32.5.1/scanpipe/tests/data/asgiref-3.3.0_walk_test_fixtures.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/basic-rootfs.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/basic-rootfs_root_filesystems.json` & `scancodeio-32.5.1/scanpipe/tests/data/debian_scan_codebase.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724729064039408%*

 * *Differences: {"'files'": "{0: {'path': "*

 * *            "'debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/etc', "*

 * *            "'tag': 'img-c19c05-layer-01-8a6376'}, 1: {'path': "*

 * *            "'debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/etc/os-release', "*

 * *            "'tag': 'img-c19c05-layer-01-8a6376'}, 2: {'path': "*

 * *            "'debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr', "*

 * *            "'ta […]*

```diff
@@ -17,22 +17,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "etc",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/etc",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/etc",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -48,22 +48,22 @@
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "8589b473401e7ebcca5d97204405c887",
             "name": "os-release",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/etc/os-release",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/etc/os-release",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "29420ee3cb176f64209d5beddc5713133fa7c2d4",
             "sha256": "aa6ccd5b1ade06c11f679cc781bdd3158f1007266ea391ed98a1bbf365641fd4",
             "sha512": "",
             "status": "ignored-not-interesting",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -79,22 +79,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "usr",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/usr",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -110,22 +110,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "share",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/usr/share",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -141,22 +141,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "doc",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/usr/share/doc",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -172,172 +172,55 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "libncurses5",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libncurses5",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libncurses5",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": "",
             "extra_data": {},
-            "for_packages": [],
+            "for_packages": [
+                "pkg:deb/libncurses5@6.1-1ubuntu1.18.04?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
+            ],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "bd73d1dbbd2e6374358baa205d6d9e66",
             "name": "copyright",
-            "package_data": [
-                {
-                    "api_data_url": null,
-                    "bug_tracking_url": null,
-                    "code_view_url": null,
-                    "copyright": "Copyright (c) 1998-2016 Free Software Foundation, Inc.\nCopyright (c) 2001 by Pradeep Padala\nCopyright (c) 1994 X Consortium\nCopyright (c) 1980, 1991, 1992, 1993 The Regents of the University of California\nCopyright 1996-2007 by Thomas E. Dickey",
-                    "datasource_id": "debian_copyright_in_package",
-                    "declared_license_expression": "x11-fsf AND x11-xconsortium AND bsd-new",
-                    "declared_license_expression_spdx": "X11-distribute-modifications-variant AND X11 AND BSD-3-Clause",
-                    "dependencies": [],
-                    "description": null,
-                    "download_url": null,
-                    "extra_data": {},
-                    "extracted_license_statement": null,
-                    "file_references": [],
-                    "holder": "Free Software Foundation, Inc.\nPradeep Padala\nX Consortium\nThe Regents of the University of California\nThomas E. Dickey",
-                    "homepage_url": null,
-                    "keywords": [],
-                    "license_detections": [
-                        {
-                            "identifier": "x11_fsf-5f3d72c2-fa6a-2f7b-b859-17e7567c1724",
-                            "license_expression": "x11-fsf",
-                            "matches": [
-                                {
-                                    "end_line": 45,
-                                    "license_expression": "x11-fsf",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 200,
-                                    "matched_text": "Permission is hereby granted, free of charge, to any person obtaining a\ncopy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, distribute with modifications, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included\nin all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS\nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE ABOVE COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\nDAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\nOTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR\nTHE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\nExcept as contained in this notice, the name(s) of the above copyright\nholders shall not be used in advertising or otherwise to promote the\nsale, use or other dealings in this Software without prior written\nauthorization.",
-                                    "matcher": "2-aho",
-                                    "rule_identifier": "x11-fsf.LICENSE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/licenses/x11-fsf.LICENSE",
-                                    "score": 100.0,
-                                    "start_line": 23
-                                }
-                            ]
-                        },
-                        {
-                            "identifier": "x11_xconsortium-8bc3e205-5f29-ecad-90bc-2f492c65be46",
-                            "license_expression": "x11-xconsortium",
-                            "matches": [
-                                {
-                                    "end_line": 70,
-                                    "license_expression": "x11-xconsortium",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 201,
-                                    "matched_text": "Permission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to\ndeal in the Software without restriction, including without limitation the\nrights to use, copy, modify, merge, publish, distribute, sublicense, and/or\nsell copies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE\nX CONSORTIUM BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN\nAN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNEC-\nTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\nExcept as contained in this notice, the name of the X Consortium shall not\nbe used in advertising or otherwise to promote the sale, use or other deal-\nings in this Software without prior written authorization from the X Consor-\ntium.",
-                                    "matcher": "2-aho",
-                                    "rule_identifier": "x11-xconsortium_2.RULE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/x11-xconsortium_2.RULE",
-                                    "score": 100.0,
-                                    "start_line": 50
-                                }
-                            ]
-                        },
-                        {
-                            "identifier": "bsd_new-ccc98c3a-92d4-e7a3-e0ba-798328cb6b98",
-                            "license_expression": "bsd-new",
-                            "matches": [
-                                {
-                                    "end_line": 98,
-                                    "license_expression": "bsd-new",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 213,
-                                    "matched_text": "Redistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions\nare met:\n1. Redistributions of source code must retain the above copyright\n   notice, this list of conditions and the following disclaimer.\n2. Redistributions in binary form must reproduce the above copyright\n   notice, this list of conditions and the following disclaimer in the\n   documentation and/or other materials provided with the distribution.\n3. Neither the name of the University nor the names of its contributors\n   may be used to endorse or promote products derived from this software\n   without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE REGENTS AND CONTRIBUTORS ``AS IS'' AND\nANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE\nARE DISCLAIMED.  IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS\nOR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)\nHOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT\nLIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY\nOUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF\nSUCH DAMAGE.",
-                                    "matcher": "2-aho",
-                                    "rule_identifier": "bsd-new_19.RULE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/bsd-new_19.RULE",
-                                    "score": 100.0,
-                                    "start_line": 76
-                                }
-                            ]
-                        },
-                        {
-                            "identifier": "x11_fsf-c2b8535e-1b81-42d8-945b-b026f349228d",
-                            "license_expression": "x11-fsf",
-                            "matches": [
-                                {
-                                    "end_line": 127,
-                                    "license_expression": "x11-fsf",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 199,
-                                    "matched_text": "Permission is hereby granted, free of charge, to any person obtaining a\ncopy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be included\nin all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS\nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE ABOVE LISTED COPYRIGHT HOLDER(S) BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\nExcept as contained in this notice, the name(s) of the above copyright\nholders shall not be used in advertising or otherwise to promote the\nsale, use or other dealings in this Software without prior written\nauthorization.",
-                                    "matcher": "2-aho",
-                                    "rule_identifier": "x11-fsf_7.RULE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/x11-fsf_7.RULE",
-                                    "score": 100.0,
-                                    "start_line": 105
-                                }
-                            ]
-                        }
-                    ],
-                    "md5": null,
-                    "name": "libncurses5",
-                    "namespace": null,
-                    "notice_text": null,
-                    "other_license_detections": [],
-                    "other_license_expression": null,
-                    "other_license_expression_spdx": null,
-                    "parties": [],
-                    "primary_language": null,
-                    "purl": "pkg:deb/libncurses5",
-                    "qualifiers": {},
-                    "release_date": null,
-                    "repository_download_url": null,
-                    "repository_homepage_url": null,
-                    "sha1": null,
-                    "sha256": null,
-                    "sha512": null,
-                    "source_packages": [],
-                    "subpath": null,
-                    "type": "deb",
-                    "vcs_url": null,
-                    "version": null
-                }
-            ],
-            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libncurses5/copyright",
+            "package_data": [],
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libncurses5/copyright",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "3ffa530d4b2e0ef318cf12f68cb7106a255ea27b",
             "sha256": "b7606456c4e97c19c54c67c1887a705b4d44e5121c48c851b256aeb65e518a4c",
             "sha512": "",
-            "status": "application-package",
-            "tag": "",
+            "status": "system-package",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -353,141 +236,55 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "libndp0",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libndp0",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libndp0",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": "",
             "extra_data": {},
-            "for_packages": [],
+            "for_packages": [
+                "pkg:deb/libndp0@1.4-2ubuntu0.16.04.1?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
+            ],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "3f4ecdd67d5b9427cdc66847bdd11cf4",
             "name": "copyright",
-            "package_data": [
-                {
-                    "api_data_url": null,
-                    "bug_tracking_url": null,
-                    "code_view_url": null,
-                    "copyright": "Copyright 2013 Jiri Pirko <jiri@resnulli.us>\nCopyright 2014 Andrew Ayer <agwa@andrewayer.name>",
-                    "datasource_id": "debian_copyright_in_package",
-                    "declared_license_expression": "lgpl-2.1-plus AND lgpl-2.1",
-                    "declared_license_expression_spdx": "LGPL-2.1-or-later AND LGPL-2.1-only",
-                    "dependencies": [],
-                    "description": null,
-                    "download_url": null,
-                    "extra_data": {},
-                    "extracted_license_statement": "- LGPL-2.1+\n- LGPL-2.1+\n- LGPL-2.1+\n",
-                    "file_references": [],
-                    "holder": "Jiri Pirko\nAndrew Ayer",
-                    "homepage_url": null,
-                    "keywords": [],
-                    "license_detections": [],
-                    "md5": null,
-                    "name": "libndp0",
-                    "namespace": null,
-                    "notice_text": null,
-                    "other_license_detections": [
-                        {
-                            "identifier": "lgpl_2_1_plus_and_lgpl_2_1-1018860f-b475-01e3-bdd4-39bf3444650e",
-                            "license_expression": "lgpl-2.1-plus AND lgpl-2.1",
-                            "matches": [
-                                {
-                                    "end_line": 13,
-                                    "license_expression": "lgpl-2.1-plus",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 4,
-                                    "matched_text": "License: lgpl-2.1+",
-                                    "matcher": "1-hash",
-                                    "rule_identifier": "lgpl-2.1-plus_108.RULE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/lgpl-2.1-plus_108.RULE",
-                                    "score": 100.0,
-                                    "start_line": 13
-                                },
-                                {
-                                    "end_line": 26,
-                                    "license_expression": "lgpl-2.1-plus",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 117,
-                                    "matched_text": "This program is free software; you can redistribute it and/or modify it\nunder the terms of the GNU Lesser General Public License as published\nby the Free Software Foundation; either version 2.1 of the License, or\n(at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser\nGeneral Public License for more details.\n\nYou should have received a copy of the GNU Lesser General Public License\nalong with this program; if not, write to the Free Software Foundation,\nInc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA",
-                                    "matcher": "2-aho",
-                                    "rule_identifier": "lgpl-2.1-plus_93.RULE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/lgpl-2.1-plus_93.RULE",
-                                    "score": 100.0,
-                                    "start_line": 14
-                                },
-                                {
-                                    "end_line": 30,
-                                    "license_expression": "lgpl-2.1",
-                                    "match_coverage": 100.0,
-                                    "matched_length": 64,
-                                    "matched_text": "You should have received a copy of the GNU Lesser General Public License\nalong with this program; if not, write to the Free Software Foundation,\nInc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA\n\nOn Debian systems, the full text of the GNU Lesser General Public\nLicense version 2.1 can be found in the file\n`/usr/share/common-licenses/LGPL-2.1'.",
-                                    "matcher": "2-aho",
-                                    "rule_identifier": "lgpl-2.1_314.RULE",
-                                    "rule_relevance": 100,
-                                    "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/lgpl-2.1_314.RULE",
-                                    "score": 100.0,
-                                    "start_line": 24
-                                }
-                            ]
-                        }
-                    ],
-                    "other_license_expression": "lgpl-2.1-plus AND lgpl-2.1",
-                    "other_license_expression_spdx": "LGPL-2.1-or-later AND LGPL-2.1-only",
-                    "parties": [],
-                    "primary_language": null,
-                    "purl": "pkg:deb/libndp0",
-                    "qualifiers": {},
-                    "release_date": null,
-                    "repository_download_url": null,
-                    "repository_homepage_url": null,
-                    "sha1": null,
-                    "sha256": null,
-                    "sha512": null,
-                    "source_packages": [],
-                    "subpath": null,
-                    "type": "deb",
-                    "vcs_url": null,
-                    "version": null
-                }
-            ],
-            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libndp0/copyright",
+            "package_data": [],
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libndp0/copyright",
             "percentage_of_license_text": null,
             "programming_language": "Haxe",
             "sha1": "0d667249e3a0f605589e7607ae6cb29024ae59b5",
             "sha256": "0d9647d1bff837cc032a1e9db188a739e84d84911ef643a71a07dfa43174b821",
             "sha512": "",
-            "status": "application-package",
-            "tag": "",
+            "status": "system-package",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -503,22 +300,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "var",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -534,22 +331,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "lib",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var/lib",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -565,22 +362,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "dpkg",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -596,84 +393,88 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "info",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/info",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/info",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": ".md5sums",
             "extra_data": {},
-            "for_packages": [],
+            "for_packages": [
+                "pkg:deb/libncurses5@6.1-1ubuntu1.18.04?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
+            ],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "9d18792b91935a5849328cb368005ec9",
-            "name": "libncurses5_amd64.md5sums",
+            "name": "libncurses5:amd64.md5sums",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/info/libncurses5_amd64.md5sums",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/info/libncurses5:amd64.md5sums",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "e5ff875218d4f909576575b0471feb0e5230a861",
             "sha256": "341282e84c13a695b49b5429ea0c244a34bc59a243ab28ec6a096ff53a9997ff",
             "sha512": "",
-            "status": "no-licenses",
-            "tag": "",
+            "status": "system-package",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": ".md5sums",
             "extra_data": {},
-            "for_packages": [],
+            "for_packages": [
+                "pkg:deb/libndp0@1.4-2ubuntu0.16.04.1?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
+            ],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "7cb818062922c437df1902c18862455a",
-            "name": "libndp0_amd64.md5sums",
+            "name": "libndp0:amd64.md5sums",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/info/libndp0_amd64.md5sums",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/info/libndp0:amd64.md5sums",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "c212d44c6649df5ff13ec447f4fa30faf81fc490",
             "sha256": "1b85f767180b0c117c68faeb8e5b8ce16b22f8a124e2e0b6210bb6710b7a9f30",
             "sha512": "",
-            "status": "no-licenses",
-            "tag": "",
+            "status": "system-package",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -705,22 +506,22 @@
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "c84949a17802e6732fc604acc8627a4b",
             "name": "status",
             "package_data": [],
-            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/status",
+            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/status",
             "percentage_of_license_text": null,
             "programming_language": "Haxe",
             "sha1": "6694bbf252c85e79790e59e20e85aee306f0ac3c",
             "sha256": "90cd872bad55159aafb8d8abc3fe86182c3bcd8ebc26775866b97ccae0da3c0f",
             "sha512": "",
             "status": "no-licenses",
-            "tag": "",
+            "tag": "img-c19c05-layer-01-8a6376",
             "type": "file",
             "urls": [
                 {
                     "end_line": 19,
                     "start_line": 19,
                     "url": "https://invisible-island.net/ncurses/"
                 },
@@ -731,49 +532,97 @@
                 }
             ]
         }
     ],
     "headers": [
         {
             "extra_data": {
-                "root_filesystems": [
+                "images": [
                     {
+                        "architecture": "amd64",
+                        "author": null,
+                        "comment": null,
+                        "config_digest": "sha256:c19c05f449307813ca60986c794d08e6586c102b8e4c7d1b035f371ac329e4a6",
+                        "created": "2022-04-29T23:21:15.708209475Z",
                         "distro": {
-                            "architecture": null,
+                            "architecture": "amd64",
                             "bug_report_url": "https://bugs.debian.org/",
                             "build_id": null,
                             "cpe_name": null,
                             "documentation_url": null,
                             "extra_data": {},
                             "home_url": "https://www.debian.org/",
-                            "id_like": null,
+                            "id_like": [],
                             "identifier": "debian",
                             "logo": null,
                             "name": "Debian GNU/Linux",
                             "os": "linux",
                             "pretty_name": "Debian GNU/Linux 9 (stretch)",
                             "privacy_policy_url": null,
                             "support_url": "https://www.debian.org/support",
                             "variant": null,
                             "variant_id": null,
                             "version": "9 (stretch)",
                             "version_codename": null,
                             "version_id": "9"
                         },
-                        "name": "basic-rootfs.tar.gz-extract"
+                        "docker_version": "20.10.12",
+                        "history": [
+                            {
+                                "created": "2022-04-29T23:21:15.290486282Z",
+                                "created_by": "/bin/sh -c #(nop) ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / "
+                            },
+                            {
+                                "created": "2022-04-29T23:21:15.708209475Z",
+                                "created_by": "/bin/sh -c #(nop)  CMD [\"bash\"]",
+                                "empty_layer": true
+                            }
+                        ],
+                        "image_format": "docker",
+                        "image_id": "c19c05f449307813ca60986c794d08e6586c102b8e4c7d1b035f371ac329e4a6",
+                        "labels": {},
+                        "layers": [
+                            {
+                                "architecture": null,
+                                "archive_location": "debian.tar.gz-extract/96381e6a50cfd100d350668ea1e2ed5706e593593b459a7b66b06830721016da.tar",
+                                "author": null,
+                                "comment": null,
+                                "created": "2022-04-29T23:21:15.290486282Z",
+                                "created_by": "/bin/sh -c #(nop) ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / ",
+                                "docker_version": null,
+                                "extracted_location": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66",
+                                "is_empty_layer": false,
+                                "labels": [],
+                                "layer_id": "8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66",
+                                "os": null,
+                                "os_version": null,
+                                "sha256": "8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66",
+                                "variant": null
+                            }
+                        ],
+                        "os": "linux",
+                        "os_version": null,
+                        "sha256": null,
+                        "tags": [],
+                        "variant": null
                     }
                 ]
             },
-            "input_sources": [],
+            "input_sources": [
+                {
+                    "filename": "debian.tar.gz",
+                    "source": "https://download.url"
+                }
+            ],
             "notice": "Generated with ScanCode.io and provided on an \"AS IS\" BASIS, WITHOUT WARRANTIES\nOR CONDITIONS OF ANY KIND, either express or implied.\nNo content created from ScanCode.io should be considered or used as legal advice.\nConsult an Attorney for any legal advice.\nScanCode.io is a free software code scanning tool from nexB Inc. and others\nlicensed under the Apache License version 2.0.\nScanCode is a trademark of nexB Inc.\nVisit https://github.com/nexB/scancode.io for support and download.\n",
             "runs": [
                 {
-                    "description": "Analyze a Linux root filesystem, aka rootfs.",
+                    "description": "Analyze Docker images.",
                     "execution_time": null,
-                    "pipeline_name": "root_filesystems",
+                    "pipeline_name": "docker",
                     "scancodeio_version": "",
                     "status": "not_started",
                     "task_end_date": null,
                     "task_exitcode": null,
                     "task_id": null,
                     "task_output": "",
                     "task_start_date": null
@@ -791,14 +640,48 @@
             "copyright": "Copyright (c) 1998-2016 Free Software Foundation, Inc.\nCopyright (c) 2001 by Pradeep Padala\nCopyright (c) 1994 X Consortium\nCopyright (c) 1980, 1991, 1992, 1993 The Regents of the University of California\nCopyright 1996-2007 by Thomas E. Dickey",
             "datasource_id": "",
             "declared_license_expression": "x11-fsf AND x11-xconsortium AND bsd-new",
             "declared_license_expression_spdx": "X11-distribute-modifications-variant AND X11 AND BSD-3-Clause",
             "description": "shared libraries for terminal handling\n The ncurses library routines are a terminal-independent method of\n updating character screens with reasonable optimization.\n .\n This package contains the shared libraries necessary to run programs\n compiled with ncurses.",
             "download_url": "",
             "extra_data": {
+                "missing_file_references": [
+                    {
+                        "extra_data": {},
+                        "md5": "23c8a935fa4fc7290d55cc5df3ef56b1",
+                        "path": "lib/x86_64-linux-gnu/libncurses.so.5.9",
+                        "sha1": null,
+                        "sha256": null,
+                        "sha512": null
+                    },
+                    {
+                        "extra_data": {},
+                        "md5": "98b70f283324e89db5787a018a54adf4",
+                        "path": "usr/lib/x86_64-linux-gnu/libform.so.5.9",
+                        "sha1": null,
+                        "sha256": null,
+                        "sha512": null
+                    },
+                    {
+                        "extra_data": {},
+                        "md5": "e3a0f5154928da2da234920343ac14b2",
+                        "path": "usr/lib/x86_64-linux-gnu/libmenu.so.5.9",
+                        "sha1": null,
+                        "sha256": null,
+                        "sha512": null
+                    },
+                    {
+                        "extra_data": {},
+                        "md5": "a927e7d76753bb85f5a784b653d337d2",
+                        "path": "usr/lib/x86_64-linux-gnu/libpanel.so.5.9",
+                        "sha1": null,
+                        "sha256": null,
+                        "sha512": null
+                    }
+                ],
                 "multi_arch": "same"
             },
             "extracted_license_statement": "",
             "file_references": [],
             "holder": "Free Software Foundation, Inc.\nPradeep Padala\nX Consortium\nThe Regents of the University of California\nThomas E. Dickey",
             "homepage_url": "https://invisible-island.net/ncurses/",
             "keywords": [
@@ -879,17 +762,15 @@
                             "score": 100.0,
                             "start_line": 105
                         }
                     ]
                 }
             ],
             "md5": "",
-            "missing_resources": [
-                "/basic-rootfs.tar.gz-extract/usr/share/doc/libncurses5/copyright"
-            ],
+            "missing_resources": [],
             "modified_resources": [],
             "name": "libncurses5",
             "namespace": "",
             "notice_text": "",
             "other_license_detections": [],
             "other_license_expression": "",
             "other_license_expression_spdx": "",
@@ -928,28 +809,44 @@
             "copyright": "Copyright 2013 Jiri Pirko <jiri@resnulli.us>\nCopyright 2014 Andrew Ayer <agwa@andrewayer.name>",
             "datasource_id": "",
             "declared_license_expression": "lgpl-2.1-plus AND lgpl-2.1",
             "declared_license_expression_spdx": "LGPL-2.1-or-later AND LGPL-2.1-only",
             "description": "Library for Neighbor Discovery Protocol\n libndp is a library for the IPv6 Neighbor Discovery Protocol (NDP).  It\n contains functions for building and parsing NDP messages, and provides\n a high-level interface for sending and receiving NDP messages on a\n network interface.",
             "download_url": "",
             "extra_data": {
+                "missing_file_references": [
+                    {
+                        "extra_data": {},
+                        "md5": "5d26434efecc08048ab72357af804ef7",
+                        "path": "usr/lib/x86_64-linux-gnu/libndp.so.0.0.2",
+                        "sha1": null,
+                        "sha256": null,
+                        "sha512": null
+                    },
+                    {
+                        "extra_data": {},
+                        "md5": "60d977e0c9a9fb07c1f8ae3090ea6f48",
+                        "path": "usr/share/doc/libndp0/changelog.Debian.gz",
+                        "sha1": null,
+                        "sha256": null,
+                        "sha512": null
+                    }
+                ],
                 "multi_arch": "same"
             },
             "extracted_license_statement": "- LGPL-2.1+\n- LGPL-2.1+\n- LGPL-2.1+\n",
             "file_references": [],
             "holder": "Jiri Pirko\nAndrew Ayer",
             "homepage_url": "http://libndp.org",
             "keywords": [
                 "libs"
             ],
             "license_detections": [],
             "md5": "",
-            "missing_resources": [
-                "/basic-rootfs.tar.gz-extract/usr/share/doc/libndp0/copyright"
-            ],
+            "missing_resources": [],
             "modified_resources": [],
             "name": "libndp0",
             "namespace": "",
             "notice_text": "",
             "other_license_detections": [
                 {
                     "identifier": "lgpl_2_1_plus_and_lgpl_2_1-1018860f-b475-01e3-bdd4-39bf3444650e",
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/centos.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/centos.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/centos_scan_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/centos_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json` & `scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json` & `scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/asgiref-3.3.0.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/missing_schema.json` & `scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/missing_schema.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/cyclonedx/nested.cdx.json` & `scancodeio-32.5.1/scanpipe/tests/data/cyclonedx/nested.cdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/expected.json` & `scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/expected.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937304075235109%*

 * *Differences: {"'files'": "{2: {'path': 'from/flume-ng-node-1.9.0-sources.LICENSE', 'name': "*

 * *            "'flume-ng-node-1.9.0-sources.LICENSE', 'status': 'about-mapped'}, 3: {'path': "*

 * *            "'from/flume-ng-node-1.9.0-sources.NOTICE', 'name': "*

 * *            "'flume-ng-node-1.9.0-sources.NOTICE', 'status': 'about-mapped', 'extension': "*

 * *            "'.NOTICE', 'md5': 'efd2af60c8501931cb9c736b5ad74f65', 'sha1': "*

 * *            "'a81b09d9521597ebcaf0cc8b49ad7a8be8e4cc61', 'sha256': "*

 * *            "'9368a7d21e018f64ae332 […]*

```diff
@@ -34,134 +34,100 @@
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
+            "extension": ".ABOUT",
+            "extra_data": {},
+            "for_packages": [],
+            "holders": [],
+            "is_archive": false,
+            "is_binary": false,
+            "is_key_file": false,
+            "is_media": false,
+            "is_text": true,
+            "license_clues": [],
+            "license_detections": [],
+            "md5": "b1d5c62c364d4470557bfba7d0338758",
+            "name": "flume-ng-node-1.9.0-sources.ABOUT",
+            "package_data": [],
+            "path": "from/flume-ng-node-1.9.0-sources.ABOUT",
+            "percentage_of_license_text": null,
+            "programming_language": "",
+            "sha1": "828f79d9fc0619a5b869c46a54b10ee3573a00bb",
+            "sha256": "de514210e135dddffb6ace69aa5fe27e1873146e05eeb5b05c6de1f8c00b0010",
+            "sha512": "",
+            "status": "about-mapped",
+            "tag": "from",
+            "type": "file",
+            "urls": []
+        },
+        {
+            "authors": [],
+            "copyrights": [],
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
+            "emails": [],
             "extension": ".LICENSE",
             "extra_data": {},
             "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "2b42edef8fa55315f34f2370b4715ca9",
-            "name": "apache-2.0.LICENSE",
+            "name": "flume-ng-node-1.9.0-sources.LICENSE",
             "package_data": [],
-            "path": "from/apache-2.0.LICENSE",
+            "path": "from/flume-ng-node-1.9.0-sources.LICENSE",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "58853eb8199b5afe72a73a25fd8cf8c94285174b",
             "sha256": "43070e2d4e532684de521b885f385d0841030efa2b1a20bafb76133a5e1379c1",
             "sha512": "",
-            "status": "",
+            "status": "about-mapped",
             "tag": "from",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
-            "detected_license_expression": "apache-2.0",
-            "detected_license_expression_spdx": "Apache-2.0",
+            "detected_license_expression": "",
+            "detected_license_expression_spdx": "",
             "emails": [],
-            "extension": ".ABOUT",
+            "extension": ".NOTICE",
             "extra_data": {},
             "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
-            "license_detections": [
-                {
-                    "identifier": "apache_2_0-6ac1a8f1-4540-e467-4f69-5e1984b60129",
-                    "license_expression": "apache-2.0",
-                    "matches": [
-                        {
-                            "end_line": 8,
-                            "license_expression": "apache-2.0",
-                            "match_coverage": 100.0,
-                            "matched_length": 3,
-                            "matched_text": "license_expression: apache-2.0",
-                            "matcher": "2-aho",
-                            "rule_identifier": "spdx_license_id_apache-2.0_for_apache-2.0.RULE",
-                            "rule_relevance": 100,
-                            "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/spdx_license_id_apache-2.0_for_apache-2.0.RULE",
-                            "score": 100.0,
-                            "start_line": 8
-                        },
-                        {
-                            "end_line": 11,
-                            "license_expression": "apache-2.0",
-                            "match_coverage": 100.0,
-                            "matched_length": 3,
-                            "matched_text": "  - key: apache-2.0",
-                            "matcher": "2-aho",
-                            "rule_identifier": "spdx_license_id_apache-2.0_for_apache-2.0.RULE",
-                            "rule_relevance": 100,
-                            "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/spdx_license_id_apache-2.0_for_apache-2.0.RULE",
-                            "score": 100.0,
-                            "start_line": 11
-                        },
-                        {
-                            "end_line": 12,
-                            "license_expression": "apache-2.0",
-                            "match_coverage": 100.0,
-                            "matched_length": 5,
-                            "matched_text": "    name: Apache License 2.0",
-                            "matcher": "2-aho",
-                            "rule_identifier": "apache-2.0_1039.RULE",
-                            "rule_relevance": 100,
-                            "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/apache-2.0_1039.RULE",
-                            "score": 100.0,
-                            "start_line": 12
-                        },
-                        {
-                            "end_line": 13,
-                            "license_expression": "apache-2.0",
-                            "match_coverage": 100.0,
-                            "matched_length": 4,
-                            "matched_text": "    file: apache-2.0.LICENSE",
-                            "matcher": "2-aho",
-                            "rule_identifier": "apache-2.0_176.RULE",
-                            "rule_relevance": 100,
-                            "rule_url": "https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/apache-2.0_176.RULE",
-                            "score": 100.0,
-                            "start_line": 13
-                        }
-                    ]
-                }
-            ],
-            "md5": "5db9e5cfad2986d7f1e8cd7633100b16",
-            "name": "flume-ng-node-1.9.0-sources.ABOUT",
+            "license_detections": [],
+            "md5": "efd2af60c8501931cb9c736b5ad74f65",
+            "name": "flume-ng-node-1.9.0-sources.NOTICE",
             "package_data": [],
-            "path": "from/flume-ng-node-1.9.0-sources.ABOUT",
-            "percentage_of_license_text": 18.29,
+            "path": "from/flume-ng-node-1.9.0-sources.NOTICE",
+            "percentage_of_license_text": null,
             "programming_language": "",
-            "sha1": "5a8183c7d9d9dcc56c5c7a57ae6a30003917e810",
-            "sha256": "da45c05ba8f0a7e434759085ac7048a4d51c5cc19b6af1d34f932bcb4ed1ecb1",
+            "sha1": "a81b09d9521597ebcaf0cc8b49ad7a8be8e4cc61",
+            "sha256": "9368a7d21e018f64ae3327d2f25cd4d7693b2d85328e4bb680bcfcbd4c26b90e",
             "sha512": "",
-            "status": "scanned",
+            "status": "about-mapped",
             "tag": "from",
             "type": "file",
-            "urls": [
-                {
-                    "end_line": 6,
-                    "start_line": 6,
-                    "url": "https://repo1.maven.org/maven2/log4j/log4j/1.2.13/log4j-1.2.13.jar"
-                }
-            ]
+            "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
@@ -437,45 +403,14 @@
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
-            "extension": ".NOTICE",
-            "extra_data": {},
-            "for_packages": [],
-            "holders": [],
-            "is_archive": false,
-            "is_binary": false,
-            "is_key_file": false,
-            "is_media": false,
-            "is_text": true,
-            "license_clues": [],
-            "license_detections": [],
-            "md5": "efd2af60c8501931cb9c736b5ad74f65",
-            "name": "flume-ng-node.NOTICE",
-            "package_data": [],
-            "path": "from/flume-ng-node.NOTICE",
-            "percentage_of_license_text": null,
-            "programming_language": "",
-            "sha1": "a81b09d9521597ebcaf0cc8b49ad7a8be8e4cc61",
-            "sha256": "9368a7d21e018f64ae3327d2f25cd4d7693b2d85328e4bb680bcfcbd4c26b90e",
-            "sha512": "",
-            "status": "",
-            "tag": "from",
-            "type": "file",
-            "urls": []
-        },
-        {
-            "authors": [],
-            "copyrights": [],
-            "detected_license_expression": "",
-            "detected_license_expression_spdx": "",
-            "emails": [],
             "extension": "",
             "extra_data": {},
             "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
@@ -521,15 +456,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "ca11ec0e5e2b32a84d5e2a1c172913490135da5e",
             "sha256": "343fa72824f27352ce855681cd91c0282337e234c6bab58ce4c8510156e83959",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -554,15 +489,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -587,15 +522,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -620,15 +555,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/DEPENDENCIES",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "03d13af648281f4e4d66b1aca27ee6fff7262360",
             "sha256": "209c31ddfb4ffaabe574b9c4ec1954c6a87c64229ea25a00511d56a20ecc72e5",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -653,15 +588,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/LICENSE",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "2b8b815229aa8a61e483fb4ba0588b8b6c491890",
             "sha256": "cfc7749b96f63bd31c3c42b5c471bf756814053e847c10f3eb003417bc523d30",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -686,15 +621,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/MANIFEST.MF",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "d64b931d5eeea17c3b1357e19ab722fd47025bfb",
             "sha256": "8fad1ad63489ffafbfe841b9116aba142185567693e5c810dfd17c2e0d60ed68",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -719,15 +654,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/maven",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -752,15 +687,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/maven/org.apache.flume",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -785,15 +720,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/maven/org.apache.flume/flume-ng-node",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -818,15 +753,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/maven/org.apache.flume/flume-ng-node/pom.properties",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "53c1d3880a1bc54f7b2ef72c7c92f0db7d3a8134",
             "sha256": "0daf0d4a0c61b6016db1a07fd0d5d8ea7f581d7242caa3c4eb3fa61a6181fdd4",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -851,15 +786,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/META-INF/maven/org.apache.flume/flume-ng-node/pom.xml",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "b2124ffb0f6800b06523eac41b26e12a5cdf4819",
             "sha256": "0406069c2bf1f01be144ab40b339a18df1323fd9fd9e1624c4adb3a925b8eba2",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -884,15 +819,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -917,15 +852,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -950,15 +885,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -983,15 +918,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1016,15 +951,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/AbstractConfigurationProvider$ChannelComponent.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "494297b9de3242aa6f99d502deaa1862c215c3d0",
             "sha256": "82c21b7ea513225e776617968a6da4ffb5bdf79e9c2eda8eccdafd67da61fdfa",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1049,15 +984,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/AbstractConfigurationProvider.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "1061d965a8d13f2e61ab9e23aca2708de3df7cee",
             "sha256": "7d2362092801c41ab7e4bb43eed6a7c6491d8212b0925708fbe6038ea9040baa",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1082,15 +1017,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/AbstractZooKeeperConfigurationProvider.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "121d2a9e3fdbe3b949bdeb66a61e9294e37222e7",
             "sha256": "3e3f5fda945d39babd3eeff11d21b78516b23dd697b02732a802e45243116c18",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1115,15 +1050,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/Application$1.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "86a51d3717bf0fd00086c6ed2fc01f37921e6ba8",
             "sha256": "9b85cd8818bb8b7e85f7cafcf7f61670571827dd9e6f70d5bde40361a38b0fb9",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1148,15 +1083,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/Application.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "7d2dd1b4b0e9b58d2f0d7c0c2b88fe2fce911508",
             "sha256": "b18d17981bbcf8759835d887c708b672509584725b9c5bc77db252e9581ab32d",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1212,15 +1147,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/EnvVarResolverProperties.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "4adf3a0410bff19811067f79ba3bf0ea4cf850ed",
             "sha256": "b0b6d4accef26ba1da3538c7de3fde4fadd9dd76f3b6061c42e146b55115178d",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1245,15 +1180,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/MaterializedConfiguration.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "682b1c89b194ec29f44876ed158370d6bf84b202",
             "sha256": "2bd752945a4965f461e0d7c2c260c29723ec8ddfb8291919351cdccc055cfc7f",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1278,15 +1213,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/PollingPropertiesFileConfigurationProvider$FileWatcherRunnable.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "562c6e25e4e2597851d622b40f059292205c4fc0",
             "sha256": "54e730f3ce423be02ff36c1d39f5d08d6f02b7d85d85ddb78d58605cbb5ce231",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1311,15 +1246,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/PollingPropertiesFileConfigurationProvider.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "f6f10eff73c6fb6acc8a303865c9a8608775f91a",
             "sha256": "5bfc65d989ae3b6d28208e2544c1e35fdd433d59850eab3aa9426c8aac375893",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1344,15 +1279,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/PollingZooKeeperConfigurationProvider$1.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "ea35273795682e8743db87e7b797d7733b7f67aa",
             "sha256": "0256effde5dd0a68e1a14ca69ff08978cf1ae95408e611b7e6fdd6c9ae6ac2ac",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1377,15 +1312,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/PollingZooKeeperConfigurationProvider.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "f0fb3a43b268fdfa2c0cd05a2e60257119ef52be",
             "sha256": "6fe1921cfa4347536f91f897bbda41b8cd4833d0cbfa0a95d57912d174af664a",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1410,15 +1345,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/PropertiesFileConfigurationProvider.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "188009bab2fad19a25822c7c05fa36dbdb1400b2",
             "sha256": "b9494daaa7dc827b826f95cce51686797605933017924bc6836e74dfe955f54e",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1443,15 +1378,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/SimpleMaterializedConfiguration.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "3673714ed860323e184670f7fc99baaf2259e5dc",
             "sha256": "bed14cff0dd864f1f27b2b0ddcf7fbd8be0653572d9e3ac67a2e27f1b2132b78",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
@@ -1476,15 +1411,15 @@
             "package_data": [],
             "path": "to/flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/StaticZooKeeperConfigurationProvider.class",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "29e9db67892e08387b89d441cb71c2f9616e1c5d",
             "sha256": "0c5cc30415dc587696eccd3a521866990594abd863e81efa99d3ef7f6ba363cc",
             "sha512": "",
-            "status": "mapped",
+            "status": "about-mapped",
             "tag": "to",
             "type": "file",
             "urls": []
         }
     ],
     "headers": [
         {
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip` & `scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/from-with-about-file.zip`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 5921 bytes, number of entries: 4
--rw-------  2.0 unx    11356 bX defN 22-Aug-22 20:02 apache-2.0.LICENSE
--rw-r--r--  2.0 unx        6 bX defN 23-Jun-09 11:38 flume-ng-node.NOTICE
--rw-r--r--  2.0 unx      448 bX defN 23-Jul-13 22:57 flume-ng-node-1.9.0-sources.ABOUT
+Zip file size: 5986 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      480 bX defN 23-Aug-01 11:57 flume-ng-node-1.9.0-sources.ABOUT
 -rw-rw-r--  2.0 unx     2085 bX defN 23-Jul-13 23:03 flume-ng-node-1.9.0-sources.jar
-4 files, 13895 bytes uncompressed, 5071 bytes compressed:  63.5%
+-rw-------  2.0 unx    11356 bX defN 22-Aug-22 20:02 flume-ng-node-1.9.0-sources.LICENSE
+-rw-r--r--  2.0 unx        6 bX defN 23-Jun-09 11:38 flume-ng-node-1.9.0-sources.NOTICE
+4 files, 13927 bytes uncompressed, 5074 bytes compressed:  63.6%
```

#### zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: apache-2.0.LICENSE
+Filename: flume-ng-node-1.9.0-sources.ABOUT
 Comment: 
 
-Filename: flume-ng-node.NOTICE
+Filename: flume-ng-node-1.9.0-sources.jar
 Comment: 
 
-Filename: flume-ng-node-1.9.0-sources.ABOUT
+Filename: flume-ng-node-1.9.0-sources.LICENSE
 Comment: 
 
-Filename: flume-ng-node-1.9.0-sources.jar
+Filename: flume-ng-node-1.9.0-sources.NOTICE
 Comment: 
 
 Zip file comment:
```

#### flume-ng-node-1.9.0-sources.ABOUT

```diff
@@ -2,12 +2,12 @@
 ignored_resources:
   - flume-ng-node-1.9.0.jar-extract/org/apache/flume/node/ConfigurationProvider.class
 name: log4j
 version: 1.2.13
 download_url: https://repo1.maven.org/maven2/log4j/log4j/1.2.13/log4j-1.2.13.jar
 package_url: pkg:maven/log4j/log4j@1.2.13
 license_expression: apache-2.0
-notice_file: flume-ng-node.NOTICE
+notice_file: flume-ng-node-1.9.0-sources.NOTICE
 licenses:
   - key: apache-2.0
     name: Apache License 2.0
-    file: apache-2.0.LICENSE
+    file: flume-ng-node-1.9.0-sources.LICENSE
```

#### Comparing `apache-2.0.LICENSE` & `flume-ng-node-1.9.0-sources.LICENSE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d/about_files/to-with-jar.zip` & `scancodeio-32.5.1/scanpipe/tests/data/d2d/about_files/to-with-jar.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip` & `scancodeio-32.5.1/scanpipe/tests/data/d2d/jars/from-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip` & `scancodeio-32.5.1/scanpipe/tests/data/d2d/jars/to-flume-ng-node-1.9.0.zip`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/main.js` & `scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/from/main.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/from/unmain.js` & `scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/from/unmain.js`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/main.js.map` & `scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/main.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map` & `scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/no_path_unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/d2d-javascript/to/unmain.js.map` & `scancodeio-32.5.1/scanpipe/tests/data/d2d-javascript/to/unmain.js.map`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl` & `scancodeio-32.5.1/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/daglib-0.6.0-py3-none-any.whl_scan_codebase.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666668%*

 * *Differences: {"'dependencies'": "{0: {'affected_by_vulnerabilities': []}, 1: {'affected_by_vulnerabilities': "*

 * *                   "[]}, 2: {'affected_by_vulnerabilities': []}, 3: "*

 * *                   "{'affected_by_vulnerabilities': []}, 4: {'affected_by_vulnerabilities': []}, "*

 * *                   "5: {'affected_by_vulnerabilities': []}, 6: {'affected_by_vulnerabilities': "*

 * *                   "[]}, 7: {'affected_by_vulnerabilities': []}}"}*

```diff
@@ -1,101 +1,109 @@
 {
     "dependencies": [
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl",
             "datasource_id": "pypi_wheel",
             "dependency_uid": "pkg:pypi/dask?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "dask[delayed]<2023.0.0,>=2022.7.1",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": false,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/dask",
             "scope": "install"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl-extract/daglib-0.6.0.dist-info/METADATA",
             "datasource_id": "pypi_wheel_metadata",
             "dependency_uid": "pkg:pypi/dask?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "dask[delayed]<2023.0.0,>=2022.7.1",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": false,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/dask",
             "scope": "install"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl",
             "datasource_id": "pypi_wheel",
             "dependency_uid": "pkg:pypi/graphviz?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "graphviz<0.21,>=0.20; extra == \"graphviz\"",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/graphviz",
             "scope": "graphviz"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl-extract/daglib-0.6.0.dist-info/METADATA",
             "datasource_id": "pypi_wheel_metadata",
             "dependency_uid": "pkg:pypi/graphviz?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "graphviz<0.21,>=0.20; extra == \"graphviz\"",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/graphviz",
             "scope": "graphviz"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl",
             "datasource_id": "pypi_wheel",
             "dependency_uid": "pkg:pypi/ipycytoscape?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "ipycytoscape<2.0.0,>=1.3.3; extra == \"ipycytoscape\"",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/ipycytoscape",
             "scope": "ipycytoscape"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl-extract/daglib-0.6.0.dist-info/METADATA",
             "datasource_id": "pypi_wheel_metadata",
             "dependency_uid": "pkg:pypi/ipycytoscape?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "ipycytoscape<2.0.0,>=1.3.3; extra == \"ipycytoscape\"",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/ipycytoscape",
             "scope": "ipycytoscape"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl",
             "datasource_id": "pypi_wheel",
             "dependency_uid": "pkg:pypi/networkx?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "networkx<3.0.0,>=2.8.5",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": false,
             "is_resolved": false,
             "is_runtime": true,
             "package_type": "pypi",
             "purl": "pkg:pypi/networkx",
             "scope": "install"
         },
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "daglib-0.6.0-py3-none-any.whl-extract/daglib-0.6.0.dist-info/METADATA",
             "datasource_id": "pypi_wheel_metadata",
             "dependency_uid": "pkg:pypi/networkx?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "networkx<3.0.0,>=2.8.5",
             "for_package_uid": "pkg:pypi/daglib@0.6.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": false,
             "is_resolved": false,
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/debian.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/debian.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/debian_scan_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/basic-rootfs_root_filesystems.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9740944170771758%*

 * *Differences: {"'files'": "{0: {'path': 'basic-rootfs.tar.gz-extract/etc', 'tag': ''}, 1: {'path': "*

 * *            "'basic-rootfs.tar.gz-extract/etc/os-release', 'tag': ''}, 2: {'path': "*

 * *            "'basic-rootfs.tar.gz-extract/usr', 'tag': ''}, 3: {'path': "*

 * *            "'basic-rootfs.tar.gz-extract/usr/share', 'tag': ''}, 4: {'path': "*

 * *            "'basic-rootfs.tar.gz-extract/usr/share/doc', 'tag': ''}, 5: {'path': "*

 * *            "'basic-rootfs.tar.gz-extract/usr/share/doc/libncurses5', 'tag': ''}, 6: {'path': "*

 * *       […]*

```diff
@@ -17,22 +17,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "etc",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/etc",
+            "path": "basic-rootfs.tar.gz-extract/etc",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -48,22 +48,22 @@
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "8589b473401e7ebcca5d97204405c887",
             "name": "os-release",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/etc/os-release",
+            "path": "basic-rootfs.tar.gz-extract/etc/os-release",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "29420ee3cb176f64209d5beddc5713133fa7c2d4",
             "sha256": "aa6ccd5b1ade06c11f679cc781bdd3158f1007266ea391ed98a1bbf365641fd4",
             "sha512": "",
             "status": "ignored-not-interesting",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -79,22 +79,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "usr",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr",
+            "path": "basic-rootfs.tar.gz-extract/usr",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -110,22 +110,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "share",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share",
+            "path": "basic-rootfs.tar.gz-extract/usr/share",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -141,22 +141,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "doc",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc",
+            "path": "basic-rootfs.tar.gz-extract/usr/share/doc",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -172,55 +172,55 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "libncurses5",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libncurses5",
+            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libncurses5",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": "",
             "extra_data": {},
             "for_packages": [
-                "pkg:deb/libncurses5@6.1-1ubuntu1.18.04?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
+                "pkg:deb/libncurses5@6.1-1ubuntu1.18.04?architecture=amd64"
             ],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "bd73d1dbbd2e6374358baa205d6d9e66",
             "name": "copyright",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libncurses5/copyright",
+            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libncurses5/copyright",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "3ffa530d4b2e0ef318cf12f68cb7106a255ea27b",
             "sha256": "b7606456c4e97c19c54c67c1887a705b4d44e5121c48c851b256aeb65e518a4c",
             "sha512": "",
             "status": "system-package",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -236,55 +236,55 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "libndp0",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libndp0",
+            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libndp0",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": "",
             "extra_data": {},
             "for_packages": [
-                "pkg:deb/libndp0@1.4-2ubuntu0.16.04.1?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
+                "pkg:deb/libndp0@1.4-2ubuntu0.16.04.1?architecture=amd64"
             ],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "3f4ecdd67d5b9427cdc66847bdd11cf4",
             "name": "copyright",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/usr/share/doc/libndp0/copyright",
+            "path": "basic-rootfs.tar.gz-extract/usr/share/doc/libndp0/copyright",
             "percentage_of_license_text": null,
             "programming_language": "Haxe",
             "sha1": "0d667249e3a0f605589e7607ae6cb29024ae59b5",
             "sha256": "0d9647d1bff837cc032a1e9db188a739e84d84911ef643a71a07dfa43174b821",
             "sha512": "",
             "status": "system-package",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -300,22 +300,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "var",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var",
+            "path": "basic-rootfs.tar.gz-extract/var",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -331,22 +331,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "lib",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib",
+            "path": "basic-rootfs.tar.gz-extract/var/lib",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -362,22 +362,22 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "dpkg",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg",
+            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -393,88 +393,84 @@
             "is_media": false,
             "is_text": false,
             "license_clues": [],
             "license_detections": [],
             "md5": "",
             "name": "info",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/info",
+            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/info",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "",
             "sha256": "",
             "sha512": "",
             "status": "scanned",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "directory",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": ".md5sums",
             "extra_data": {},
-            "for_packages": [
-                "pkg:deb/libncurses5@6.1-1ubuntu1.18.04?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
-            ],
+            "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "9d18792b91935a5849328cb368005ec9",
-            "name": "libncurses5:amd64.md5sums",
+            "name": "libncurses5_amd64.md5sums",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/info/libncurses5:amd64.md5sums",
+            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/info/libncurses5_amd64.md5sums",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "e5ff875218d4f909576575b0471feb0e5230a861",
             "sha256": "341282e84c13a695b49b5429ea0c244a34bc59a243ab28ec6a096ff53a9997ff",
             "sha512": "",
-            "status": "system-package",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "status": "no-licenses",
+            "tag": "",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
             "detected_license_expression_spdx": "",
             "emails": [],
             "extension": ".md5sums",
             "extra_data": {},
-            "for_packages": [
-                "pkg:deb/libndp0@1.4-2ubuntu0.16.04.1?architecture=amd64&uuid=fixed-uid-done-for-testing-5642512d1758"
-            ],
+            "for_packages": [],
             "holders": [],
             "is_archive": false,
             "is_binary": false,
             "is_key_file": false,
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "7cb818062922c437df1902c18862455a",
-            "name": "libndp0:amd64.md5sums",
+            "name": "libndp0_amd64.md5sums",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/info/libndp0:amd64.md5sums",
+            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/info/libndp0_amd64.md5sums",
             "percentage_of_license_text": null,
             "programming_language": "",
             "sha1": "c212d44c6649df5ff13ec447f4fa30faf81fc490",
             "sha256": "1b85f767180b0c117c68faeb8e5b8ce16b22f8a124e2e0b6210bb6710b7a9f30",
             "sha512": "",
-            "status": "system-package",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "status": "no-licenses",
+            "tag": "",
             "type": "file",
             "urls": []
         },
         {
             "authors": [],
             "copyrights": [],
             "detected_license_expression": "",
@@ -506,22 +502,22 @@
             "is_media": false,
             "is_text": true,
             "license_clues": [],
             "license_detections": [],
             "md5": "c84949a17802e6732fc604acc8627a4b",
             "name": "status",
             "package_data": [],
-            "path": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66/var/lib/dpkg/status",
+            "path": "basic-rootfs.tar.gz-extract/var/lib/dpkg/status",
             "percentage_of_license_text": null,
             "programming_language": "Haxe",
             "sha1": "6694bbf252c85e79790e59e20e85aee306f0ac3c",
             "sha256": "90cd872bad55159aafb8d8abc3fe86182c3bcd8ebc26775866b97ccae0da3c0f",
             "sha512": "",
             "status": "no-licenses",
-            "tag": "img-c19c05-layer-01-8a6376",
+            "tag": "",
             "type": "file",
             "urls": [
                 {
                     "end_line": 19,
                     "start_line": 19,
                     "url": "https://invisible-island.net/ncurses/"
                 },
@@ -532,97 +528,49 @@
                 }
             ]
         }
     ],
     "headers": [
         {
             "extra_data": {
-                "images": [
+                "root_filesystems": [
                     {
-                        "architecture": "amd64",
-                        "author": null,
-                        "comment": null,
-                        "config_digest": "sha256:c19c05f449307813ca60986c794d08e6586c102b8e4c7d1b035f371ac329e4a6",
-                        "created": "2022-04-29T23:21:15.708209475Z",
                         "distro": {
-                            "architecture": "amd64",
+                            "architecture": null,
                             "bug_report_url": "https://bugs.debian.org/",
                             "build_id": null,
                             "cpe_name": null,
                             "documentation_url": null,
                             "extra_data": {},
                             "home_url": "https://www.debian.org/",
-                            "id_like": [],
+                            "id_like": null,
                             "identifier": "debian",
                             "logo": null,
                             "name": "Debian GNU/Linux",
                             "os": "linux",
                             "pretty_name": "Debian GNU/Linux 9 (stretch)",
                             "privacy_policy_url": null,
                             "support_url": "https://www.debian.org/support",
                             "variant": null,
                             "variant_id": null,
                             "version": "9 (stretch)",
                             "version_codename": null,
                             "version_id": "9"
                         },
-                        "docker_version": "20.10.12",
-                        "history": [
-                            {
-                                "created": "2022-04-29T23:21:15.290486282Z",
-                                "created_by": "/bin/sh -c #(nop) ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / "
-                            },
-                            {
-                                "created": "2022-04-29T23:21:15.708209475Z",
-                                "created_by": "/bin/sh -c #(nop)  CMD [\"bash\"]",
-                                "empty_layer": true
-                            }
-                        ],
-                        "image_format": "docker",
-                        "image_id": "c19c05f449307813ca60986c794d08e6586c102b8e4c7d1b035f371ac329e4a6",
-                        "labels": {},
-                        "layers": [
-                            {
-                                "architecture": null,
-                                "archive_location": "debian.tar.gz-extract/96381e6a50cfd100d350668ea1e2ed5706e593593b459a7b66b06830721016da.tar",
-                                "author": null,
-                                "comment": null,
-                                "created": "2022-04-29T23:21:15.290486282Z",
-                                "created_by": "/bin/sh -c #(nop) ADD file:37744639836b248c88f6e126619829290b45c233309538310e8fffb82e98eaf8 in / ",
-                                "docker_version": null,
-                                "extracted_location": "debian.tar.gz-extract/8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66",
-                                "is_empty_layer": false,
-                                "labels": [],
-                                "layer_id": "8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66",
-                                "os": null,
-                                "os_version": null,
-                                "sha256": "8a63761caf6d45e65b8e6cdc2e0c03c55625fd142ec3356b80a9ea4a34b11b66",
-                                "variant": null
-                            }
-                        ],
-                        "os": "linux",
-                        "os_version": null,
-                        "sha256": null,
-                        "tags": [],
-                        "variant": null
+                        "name": "basic-rootfs.tar.gz-extract"
                     }
                 ]
             },
-            "input_sources": [
-                {
-                    "filename": "debian.tar.gz",
-                    "source": "https://download.url"
-                }
-            ],
+            "input_sources": [],
             "notice": "Generated with ScanCode.io and provided on an \"AS IS\" BASIS, WITHOUT WARRANTIES\nOR CONDITIONS OF ANY KIND, either express or implied.\nNo content created from ScanCode.io should be considered or used as legal advice.\nConsult an Attorney for any legal advice.\nScanCode.io is a free software code scanning tool from nexB Inc. and others\nlicensed under the Apache License version 2.0.\nScanCode is a trademark of nexB Inc.\nVisit https://github.com/nexB/scancode.io for support and download.\n",
             "runs": [
                 {
-                    "description": "Analyze Docker images.",
+                    "description": "Analyze a Linux root filesystem, aka rootfs.",
                     "execution_time": null,
-                    "pipeline_name": "docker",
+                    "pipeline_name": "root_filesystems",
                     "scancodeio_version": "",
                     "status": "not_started",
                     "task_end_date": null,
                     "task_exitcode": null,
                     "task_id": null,
                     "task_output": "",
                     "task_start_date": null
@@ -640,48 +588,14 @@
             "copyright": "Copyright (c) 1998-2016 Free Software Foundation, Inc.\nCopyright (c) 2001 by Pradeep Padala\nCopyright (c) 1994 X Consortium\nCopyright (c) 1980, 1991, 1992, 1993 The Regents of the University of California\nCopyright 1996-2007 by Thomas E. Dickey",
             "datasource_id": "",
             "declared_license_expression": "x11-fsf AND x11-xconsortium AND bsd-new",
             "declared_license_expression_spdx": "X11-distribute-modifications-variant AND X11 AND BSD-3-Clause",
             "description": "shared libraries for terminal handling\n The ncurses library routines are a terminal-independent method of\n updating character screens with reasonable optimization.\n .\n This package contains the shared libraries necessary to run programs\n compiled with ncurses.",
             "download_url": "",
             "extra_data": {
-                "missing_file_references": [
-                    {
-                        "extra_data": {},
-                        "md5": "23c8a935fa4fc7290d55cc5df3ef56b1",
-                        "path": "lib/x86_64-linux-gnu/libncurses.so.5.9",
-                        "sha1": null,
-                        "sha256": null,
-                        "sha512": null
-                    },
-                    {
-                        "extra_data": {},
-                        "md5": "98b70f283324e89db5787a018a54adf4",
-                        "path": "usr/lib/x86_64-linux-gnu/libform.so.5.9",
-                        "sha1": null,
-                        "sha256": null,
-                        "sha512": null
-                    },
-                    {
-                        "extra_data": {},
-                        "md5": "e3a0f5154928da2da234920343ac14b2",
-                        "path": "usr/lib/x86_64-linux-gnu/libmenu.so.5.9",
-                        "sha1": null,
-                        "sha256": null,
-                        "sha512": null
-                    },
-                    {
-                        "extra_data": {},
-                        "md5": "a927e7d76753bb85f5a784b653d337d2",
-                        "path": "usr/lib/x86_64-linux-gnu/libpanel.so.5.9",
-                        "sha1": null,
-                        "sha256": null,
-                        "sha512": null
-                    }
-                ],
                 "multi_arch": "same"
             },
             "extracted_license_statement": "",
             "file_references": [],
             "holder": "Free Software Foundation, Inc.\nPradeep Padala\nX Consortium\nThe Regents of the University of California\nThomas E. Dickey",
             "homepage_url": "https://invisible-island.net/ncurses/",
             "keywords": [
@@ -809,32 +723,14 @@
             "copyright": "Copyright 2013 Jiri Pirko <jiri@resnulli.us>\nCopyright 2014 Andrew Ayer <agwa@andrewayer.name>",
             "datasource_id": "",
             "declared_license_expression": "lgpl-2.1-plus AND lgpl-2.1",
             "declared_license_expression_spdx": "LGPL-2.1-or-later AND LGPL-2.1-only",
             "description": "Library for Neighbor Discovery Protocol\n libndp is a library for the IPv6 Neighbor Discovery Protocol (NDP).  It\n contains functions for building and parsing NDP messages, and provides\n a high-level interface for sending and receiving NDP messages on a\n network interface.",
             "download_url": "",
             "extra_data": {
-                "missing_file_references": [
-                    {
-                        "extra_data": {},
-                        "md5": "5d26434efecc08048ab72357af804ef7",
-                        "path": "usr/lib/x86_64-linux-gnu/libndp.so.0.0.2",
-                        "sha1": null,
-                        "sha256": null,
-                        "sha512": null
-                    },
-                    {
-                        "extra_data": {},
-                        "md5": "60d977e0c9a9fb07c1f8ae3090ea6f48",
-                        "path": "usr/share/doc/libndp0/changelog.Debian.gz",
-                        "sha1": null,
-                        "sha256": null,
-                        "sha512": null
-                    }
-                ],
                 "multi_arch": "same"
             },
             "extracted_license_statement": "- LGPL-2.1+\n- LGPL-2.1+\n- LGPL-2.1+\n",
             "file_references": [],
             "holder": "Jiri Pirko\nAndrew Ayer",
             "homepage_url": "http://libndp.org",
             "keywords": [
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/decompose_l_u_8hpp_source.html` & `scancodeio-32.5.1/scanpipe/tests/data/decompose_l_u_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/docker-images.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json` & `scancodeio-32.5.1/scanpipe/tests/data/docker-images.tar.gz-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json` & `scancodeio-32.5.1/scanpipe/tests/data/docker-images.tar.gz-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz` & `scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json` & `scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-alpine.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz` & `scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json` & `scancodeio-32.5.1/scanpipe/tests/data/docker-mini-with-license-debian.tar.xz-docker-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/flume-ng-node-d2d.json` & `scancodeio-32.5.1/scanpipe/tests/data/flume-ng-node-d2d.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/foobar.qcow2.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/foobar.qcow2.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/gcr_io_distroless_base.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/gcr_io_distroless_base_scan_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar` & `scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/layer_with_links_missing_targets.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar` & `scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json` & `scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-1.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json` & `scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-data-2.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json` & `scancodeio-32.5.1/scanpipe/tests/data/image-with-symlinks/minitag.tar-expected-scan.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0.tgz` & `scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0.tgz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0_scan_codebase.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666666%*

 * *Differences: {"'dependencies'": "{0: {'affected_by_vulnerabilities': []}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "dependencies": [
         {
+            "affected_by_vulnerabilities": [],
             "datafile_path": "is-npm-1.0.0.tgz-extract/package/package.json",
             "datasource_id": "npm_package_json",
             "dependency_uid": "pkg:npm/ava?uuid=fixed-uid-done-for-testing-5642512d1758",
             "extracted_requirement": "0.0.3",
             "for_package_uid": "pkg:npm/is-npm@1.0.0?uuid=fixed-uid-done-for-testing-5642512d1758",
             "is_optional": true,
             "is_resolved": false,
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package.json` & `scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json` & `scancodeio-32.5.1/scanpipe/tests/data/is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/jvm/common.java` & `scancodeio-32.5.1/scanpipe/tests/data/jvm/common.java`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/manifests/package.expected.json` & `scancodeio-32.5.1/scanpipe/tests/data/manifests/package.expected.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/manifests/package.json` & `scancodeio-32.5.1/scanpipe/tests/data/manifests/package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.json` & `scancodeio-32.5.1/scanpipe/tests/data/manifests/toml.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/manifests/toml.spdx.json` & `scancodeio-32.5.1/scanpipe/tests/data/manifests/toml.spdx.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz` & `scancodeio-32.5.1/scanpipe/tests/data/multiple-is-npm-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json` & `scancodeio-32.5.1/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json` & `scancodeio-32.5.1/scanpipe/tests/data/multiple-is-npm-1.0.0_scan_package_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/notice.NOTICE` & `scancodeio-32.5.1/scanpipe/tests/data/notice.NOTICE`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx` & `scancodeio-32.5.1/scanpipe/tests/data/outputs/asgiref-3.6.0-output.xlsx`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/outputs/expected_attribution.html` & `scancodeio-32.5.1/scanpipe/tests/data/outputs/expected_attribution.html`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json` & `scancodeio-32.5.1/scanpipe/tests/data/scancode/is-npm-1.0.0_summary.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/scancode/package_assembly_codebase.json` & `scancodeio-32.5.1/scanpipe/tests/data/scancode/package_assembly_codebase.json`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/data/windows-container-rootfs.tar` & `scancodeio-32.5.1/scanpipe/tests/data/windows-container-rootfs.tar`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipelines/do_nothing.py` & `scancodeio-32.5.1/scanpipe/tests/pipelines/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipelines/profile_step.py` & `scancodeio-32.5.1/scanpipe/tests/pipelines/profile_step.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipelines/raise_exception.py` & `scancodeio-32.5.1/scanpipe/tests/pipelines/raise_exception.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipelines/register_from_file.py` & `scancodeio-32.5.1/scanpipe/tests/pipelines/register_from_file.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipelines/steps_as_attribute.py` & `scancodeio-32.5.1/scanpipe/tests/pipelines/steps_as_attribute.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_codebase.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_codebase.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_cyclonedx.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_d2d.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_d2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from unittest import mock
 
 from django.test import TestCase
 
 from scanpipe.models import CodebaseResource
 from scanpipe.models import Project
 from scanpipe.pipes import d2d
+from scanpipe.pipes import flag
 from scanpipe.pipes.input import copy_input
 from scanpipe.pipes.input import copy_inputs
 from scanpipe.tests import make_resource_file
 from scanpipe.tests import package_data1
 
 
 class ScanPipeD2DPipesTest(TestCase):
@@ -124,17 +125,17 @@
 
         path = "a.jar-extract/subpath/b.jar-extract/subpath/file.ext"
         self.assertEqual("subpath/file.ext", d2d.get_extracted_subpath(path))
 
     @mock.patch("scanpipe.pipes.purldb.match_package")
     def test_scanpipe_pipes_d2d_match_purldb(self, mock_match_package):
         to_1 = make_resource_file(self.project1, "to/package.jar", sha1="abcdef")
-        # The initial status will be updated to "matched-to-purldb"
+        # The initial status will be updated to flag.MATCHED_TO_PURLDB
         to_2 = make_resource_file(
-            self.project1, "to/package.jar-extract/a.class", status="mapped"
+            self.project1, "to/package.jar-extract/a.class", status=flag.MAPPED
         )
         to_3 = make_resource_file(self.project1, "to/package.jar-extract/b.class")
 
         package_data = package_data1.copy()
         package_data["uuid"] = uuid.uuid4()
         mock_match_package.return_value = [package_data]
 
@@ -152,15 +153,15 @@
 
         package = self.project1.discoveredpackages.get()
         self.assertEqual(package_data["name"], package.name)
         self.assertNotEqual(package_data["uuid"], package.uuid)
 
         for resource in [to_1, to_2, to_3]:
             resource.refresh_from_db()
-            self.assertEqual("matched-to-purldb", resource.status)
+            self.assertEqual(flag.MATCHED_TO_PURLDB, resource.status)
             self.assertEqual(package, resource.discovered_packages.get())
 
     def test_scanpipe_pipes_d2d_get_best_path_matches_same_name(self):
         to_1 = CodebaseResource(name="package-1.0.ext", path="to/package-1.0.ext")
         to_2 = CodebaseResource(name="package-2.0.ext", path="to/package-2.0.ext")
         from_1 = CodebaseResource(name="package-1.0.ext", path="from/package-1.0.ext")
         from_2 = CodebaseResource(name="package-2.0.ext", path="from/package-2.0.ext")
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_docker.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_docker.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_fetch.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,20 @@
         mock_run_command.assert_called_once()
         cmd = mock_run_command.call_args[0][0]
         self.assertTrue(cmd.startswith("skopeo copy --insecure-policy"))
         self.assertIn("docker://debian:10.9 docker-archive:/", cmd)
         self.assertIn("--override-os=linux --override-arch=amd64", cmd)
         self.assertTrue(cmd.endswith("debian_10_9.tar"))
 
+    def test_scanpipe_pipes_fetch_docker_image_string_injection_protection(self):
+        url = 'docker://;echo${IFS}"PoC"${IFS}"'
+        with self.assertRaises(ValueError) as cm:
+            fetch.fetch_docker_image(url)
+        self.assertEqual("Invalid Docker reference.", str(cm.exception))
+
     @mock.patch("requests.get")
     def test_scanpipe_pipes_fetch_fetch_urls(self, mock_get):
         urls = [
             "https://example.com/filename.zip",
             "https://example.com/archive.tar.gz",
         ]
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_flag.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_flag.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_input.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_input.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_js.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_js.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_jvm.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_jvm.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_output.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_output.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_pathmap.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_pathmap.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_pipes.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_pipes.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_resolve.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_resolve.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_rootfs.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_rootfs.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_scancode.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_scancode.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_spdx.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_spdx.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/pipes/test_windows.py` & `scancodeio-32.5.1/scanpipe/tests/pipes/test_windows.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/regen_test_data.py` & `scancodeio-32.5.1/scanpipe/tests/regen_test_data.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_api.py` & `scancodeio-32.5.1/scanpipe/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -299,14 +299,90 @@
         expected = {
             "filename": "archive.zip",
             "source": "https://example.com/archive.zip",
         }
         self.assertEqual([expected], response.data["input_sources"])
         self.assertEqual(["archive.zip"], response.data["input_root"])
 
+        mock_get.side_effect = [
+            mock.Mock(content=b"\x00", headers={}, status_code=200, url="archive.zip"),
+            mock.Mock(
+                content=b"\x00", headers={}, status_code=200, url="second.tar.gz"
+            ),
+        ]
+        data = {
+            "name": "Upload 2 archives",
+            "input_urls": [
+                "https://example.com/archive.zip",
+                "https://example.com/second.tar.gz",
+            ],
+        }
+        response = self.csrf_client.post(self.project_list_url, data)
+        self.assertEqual(status.HTTP_201_CREATED, response.status_code)
+        created_project_detail_url = response.data["url"]
+        response = self.csrf_client.get(created_project_detail_url)
+        expected = [
+            {"filename": "archive.zip", "source": "https://example.com/archive.zip"},
+            {
+                "filename": "second.tar.gz",
+                "source": "https://example.com/second.tar.gz",
+            },
+        ]
+        self.assertEqual(expected, response.data["input_sources"])
+        expected = ["archive.zip", "second.tar.gz"]
+        self.assertEqual(expected, sorted(response.data["input_root"]))
+
+    def test_scanpipe_api_project_create_multiple_pipelines(self):
+        data = {
+            "name": "Single string",
+            "pipeline": "docker",
+        }
+        response = self.csrf_client.post(self.project_list_url, data)
+        self.assertEqual(status.HTTP_201_CREATED, response.status_code)
+        self.assertEqual(1, len(response.data["runs"]))
+        self.assertEqual("docker", response.data["runs"][0]["pipeline_name"])
+        self.assertEqual("docker", response.data["next_run"])
+
+        data = {
+            "name": "Single list",
+            "pipeline": ["docker"],
+        }
+        response = self.csrf_client.post(self.project_list_url, data)
+        self.assertEqual(status.HTTP_201_CREATED, response.status_code)
+        self.assertEqual(1, len(response.data["runs"]))
+        self.assertEqual("docker", response.data["runs"][0]["pipeline_name"])
+        self.assertEqual("docker", response.data["next_run"])
+
+        data = {
+            "name": "Multi list",
+            "pipeline": ["docker", "scan_package"],
+        }
+        response = self.csrf_client.post(self.project_list_url, data)
+        self.assertEqual(status.HTTP_201_CREATED, response.status_code)
+        self.assertEqual(2, len(response.data["runs"]))
+        self.assertEqual("docker", response.data["runs"][0]["pipeline_name"])
+        self.assertEqual("scan_package", response.data["runs"][1]["pipeline_name"])
+        self.assertEqual("docker", response.data["next_run"])
+
+        data = {
+            "name": "Multi string",
+            "pipeline": "docker,scan_package",
+        }
+        response = self.csrf_client.post(self.project_list_url, data)
+        self.assertEqual(status.HTTP_400_BAD_REQUEST, response.status_code)
+        expected = {
+            "pipeline": [
+                ErrorDetail(
+                    string='"docker,scan_package" is not a valid choice.',
+                    code="invalid_choice",
+                )
+            ]
+        }
+        self.assertEqual(expected, response.data)
+
     def test_scanpipe_api_project_results_generator(self):
         results_generator = JSONResultsGenerator(self.project1)
         results = json.loads("".join(results_generator))
 
         expected = ["dependencies", "files", "headers", "packages", "relations"]
         self.assertEqual(expected, sorted(results.keys()))
 
@@ -748,14 +824,14 @@
         self.assertEqual(ProjectErrorSerializer, get_model_serializer(ProjectError))
 
         with self.assertRaises(LookupError):
             get_model_serializer(None)
 
     def test_scanpipe_api_serializer_get_serializer_fields(self):
         self.assertEqual(44, len(get_serializer_fields(DiscoveredPackage)))
-        self.assertEqual(11, len(get_serializer_fields(DiscoveredDependency)))
+        self.assertEqual(12, len(get_serializer_fields(DiscoveredDependency)))
         self.assertEqual(33, len(get_serializer_fields(CodebaseResource)))
         self.assertEqual(3, len(get_serializer_fields(CodebaseRelation)))
         self.assertEqual(6, len(get_serializer_fields(ProjectError)))
 
         with self.assertRaises(LookupError):
             get_serializer_fields(None)
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_apps.py` & `scancodeio-32.5.1/scanpipe/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_auth.py` & `scancodeio-32.5.1/scanpipe/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_commands.py` & `scancodeio-32.5.1/scanpipe/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_filters.py` & `scancodeio-32.5.1/scanpipe/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_forms.py` & `scancodeio-32.5.1/scanpipe/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_licenses.py` & `scancodeio-32.5.1/scanpipe/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_models.py` & `scancodeio-32.5.1/scanpipe/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_pipelines.py` & `scancodeio-32.5.1/scanpipe/tests/test_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -650,17 +650,17 @@
 
         self.assertEqual(18, project2.codebaseresources.count())
         self.assertEqual(2, project2.discoveredpackages.count())
         self.assertEqual(4, project2.discovereddependencies.count())
 
     @mock.patch("scanpipe.pipes.vulnerablecode.is_available")
     @mock.patch("scanpipe.pipes.vulnerablecode.is_configured")
-    @mock.patch("scanpipe.pipes.vulnerablecode.get_vulnerabilities_by_purl")
+    @mock.patch("scanpipe.pipes.vulnerablecode.bulk_search_by_purl")
     def test_scanpipe_find_vulnerabilities_pipeline_integration_test(
-        self, mock_get_vulnerabilities, mock_is_configured, mock_is_available
+        self, mock_bulk_search_by_purl, mock_is_configured, mock_is_available
     ):
         pipeline_name = "find_vulnerabilities"
         project1 = Project.objects.create(name="Analysis")
         package1 = DiscoveredPackage.create_from_data(project1, package_data1)
 
         run = project1.add_pipeline(pipeline_name)
         pipeline = run.make_pipeline_instance()
@@ -672,15 +672,15 @@
 
         run = project1.add_pipeline(pipeline_name)
         pipeline = run.make_pipeline_instance()
         mock_is_configured.return_value = True
         mock_is_available.return_value = True
         vulnerability_data = [
             {
-                "purl": "pkg:deb/debian/adduser@3.118",
+                "purl": "pkg:deb/debian/adduser@3.118?arch=all",
                 "affected_by_vulnerabilities": [
                     {
                         "vulnerability_id": "VCID-cah8-awtr-aaad",
                         "summary": "An issue was discovered.",
                     },
                 ],
             },
@@ -690,15 +690,15 @@
                     {
                         "vulnerability_id": "VCID-cah8-awtr-aaad",
                         "summary": "An issue was discovered.",
                     },
                 ],
             },
         ]
-        mock_get_vulnerabilities.return_value = vulnerability_data
+        mock_bulk_search_by_purl.return_value = vulnerability_data
 
         exitcode, out = pipeline.execute()
         self.assertEqual(0, exitcode, msg=out)
 
         package1.refresh_from_db()
         expected = vulnerability_data[0]["affected_by_vulnerabilities"]
         self.assertEqual(expected, package1.affected_by_vulnerabilities)
```

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_tasks.py` & `scancodeio-32.5.1/scanpipe/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/tests/test_views.py` & `scancodeio-32.5.1/scanpipe/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/urls.py` & `scancodeio-32.5.1/scanpipe/urls.py`

 * *Files identical despite different names*

### Comparing `scancodeio-32.5.0/scanpipe/views.py` & `scancodeio-32.5.1/scanpipe/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1154,15 +1154,18 @@
 ):
     model = DiscoveredDependency
     filterset_class = DependencyFilterSet
     template_name = "scanpipe/dependency_list.html"
     paginate_by = settings.SCANCODEIO_PAGINATE_BY.get("dependency", 100)
     prefetch_related = ["for_package", "datafile_resource"]
     table_columns = [
-        "package_url",
+        {
+            "field_name": "package_url",
+            "filter_fieldname": "is_vulnerable",
+        },
         {
             "field_name": "type",
             "label": "Package type",
             "filter_fieldname": "type",
         },
         "extracted_requirement",
         {
@@ -1578,19 +1581,14 @@
                 {"field_name": "extra_data", "render_func": render_as_yaml},
             ],
             "verbose_name": "Extra",
             "icon_class": "fa-solid fa-database",
         },
     }
 
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        context["vulnerablecode_url"] = settings.VULNERABLECODE_URL
-        return context
-
 
 class DiscoveredDependencyDetailsView(
     ConditionalLoginRequired,
     ProjectRelatedViewMixin,
     TabSetMixin,
     PrefetchRelatedViewMixin,
     generic.DetailView,
@@ -1626,14 +1624,19 @@
                 "for_package_uid",
                 "is_runtime",
                 "is_optional",
                 "is_resolved",
             ],
             "icon_class": "fa-solid fa-plus-square",
         },
+        "vulnerabilities": {
+            "fields": ["affected_by_vulnerabilities"],
+            "icon_class": "fa-solid fa-bug",
+            "template": "scanpipe/tabset/tab_vulnerabilities.html",
+        },
     }
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["dependency_data"] = DiscoveredDependencySerializer(self.object).data
         return context
```

### Comparing `scancodeio-32.5.0/setup.cfg` & `scancodeio-32.5.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scancodeio
-version = 32.5.0
+version = 32.5.1
 license = Apache-2.0
 description = Automate software composition analysis pipelines
 long_description = file:README.rst
 author = nexB Inc.
 author_email = info@aboutcode.org
 url = https://github.com/nexB/scancode.io
 classifiers = 
@@ -124,15 +124,15 @@
 ignore = E203,W503
 
 [pydocstyle]
 ignore = D1,D203,D205,D212,D400,D415
 
 [bumpver]
 version_pattern = "MAJOR.MINOR.PATCH"
-current_version = "32.5.0"
+current_version = "32.5.1"
 
 [bumpver:file_patterns]
 setup.cfg = 
 	version = {version}
 	current_version = "{version}"
 scancodeio/__init__.py = {version}
```

### Comparing `scancodeio-32.5.0/setup.py` & `scancodeio-32.5.1/setup.py`

 * *Files identical despite different names*

