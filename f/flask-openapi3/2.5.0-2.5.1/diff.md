# Comparing `tmp/flask-openapi3-2.5.0.tar.gz` & `tmp/flask-openapi3-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-openapi3-2.5.0.tar", last modified: Wed Aug  2 02:43:24 2023, max compression
+gzip compressed data, was "flask-openapi3-2.5.1.tar", last modified: Mon Aug  7 07:32:24 2023, max compression
```

## Comparing `flask-openapi3-2.5.0.tar` & `flask-openapi3-2.5.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.886635 flask-openapi3-2.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/api_blueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/api_view_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/async_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/custom_ui_templates_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/enum_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/header_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/image_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/init_oauth_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/just_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/nested_apiblueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/openapi_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/openapi_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/orjson_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/pydantic_custom_root_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/response_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/rest_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/servers_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/upload_file_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.886635 flask-openapi3-2.5.0/flask_openapi3/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/external_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/oauth_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/oauth_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/parameter_in_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/path_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security_scheme_in_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/server_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/style_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    24248 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.882635 flask-openapi3-2.5.0/flask_openapi3/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/css/swagger-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/swagger.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.886635 flask-openapi3-2.5.0/flask_openapi3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.454119 flask-openapi3-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-07 07:32:24.454119 flask-openapi3-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.438119 flask-openapi3-2.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/api_blueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/api_view_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/async_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/custom_ui_templates_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/enum_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/header_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/image_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/init_oauth_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/just_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/openapi_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/openapi_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/orjson_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/pydantic_custom_root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/response_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/rest_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/servers_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/examples/upload_file_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.442119 flask-openapi3-2.5.1/flask_openapi3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.450119 flask-openapi3-2.5.1/flask_openapi3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/oauth_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/oauth_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/parameter_in_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/security_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/security_scheme_in_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/server_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/style_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/models/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24248 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.450119 flask-openapi3-2.5.1/flask_openapi3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.430119 flask-openapi3-2.5.1/flask_openapi3/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.450119 flask-openapi3-2.5.1/flask_openapi3/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/css/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.450119 flask-openapi3-2.5.1/flask_openapi3/templates/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/images/apidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/images/rapidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/images/redoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/images/swagger.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.454119 flask-openapi3-2.5.1/flask_openapi3/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/js/rapidoc-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/js/redoc.standalone.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/flask_openapi3/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:32:24.442119 flask-openapi3-2.5.1/flask_openapi3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-07 07:32:24.000000 flask-openapi3-2.5.1/flask_openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-07 07:32:24.000000 flask-openapi3-2.5.1/flask_openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:32:24.000000 flask-openapi3-2.5.1/flask_openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:32:24.000000 flask-openapi3-2.5.1/flask_openapi3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-07 07:32:24.000000 flask-openapi3-2.5.1/flask_openapi3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 07:32:24.000000 flask-openapi3-2.5.1/flask_openapi3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 07:32:24.454119 flask-openapi3-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-07 07:32:14.000000 flask-openapi3-2.5.1/setup.py
```

### Comparing `flask-openapi3-2.5.0/CHANGELOG.md` & `flask-openapi3-2.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## v2.5.1 2023-08-07
+
+- [#95](https://github.com/luolingchun/flask-openapi3/pull/95) Added ability to deserialize complex form parameter objects. Thanks, BlackGad.
+
 ## v2.5.0 2023-08-02
 
 - [#79](https://github.com/luolingchun/flask-openapi3/discussions/79) Support `by_alias` in Model Config. Thanks, @candleindark.
 - [#82](https://github.com/luolingchun/flask-openapi3/issues/82) Fix parameter in url_prefix. Thanks, @riedgar-ms.
 - [#83](https://github.com/luolingchun/flask-openapi3/pull/83) Be able to change 422 validation errors to other http response status. Thanks, @CostcoFanboy.
 - [#86](https://github.com/luolingchun/flask-openapi3/issues/86) Responses key supports both string, int, and HTTPStatus. Thanks, @CostcoFanboy.
```

### Comparing `flask-openapi3-2.5.0/CONTRIBUTING.md` & `flask-openapi3-2.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/LICENSE.rst` & `flask-openapi3-2.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/PKG-INFO` & `flask-openapi3-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.5.0
+Version: 2.5.1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flask-openapi3-2.5.0/README.md` & `flask-openapi3-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/api_blueprint_demo.py` & `flask-openapi3-2.5.1/examples/api_blueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/api_view_demo.py` & `flask-openapi3-2.5.1/examples/api_view_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/async_demo.py` & `flask-openapi3-2.5.1/examples/async_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/custom_ui_templates_demo.py` & `flask-openapi3-2.5.1/examples/custom_ui_templates_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/enum_demo.py` & `flask-openapi3-2.5.1/examples/enum_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/header_demo.py` & `flask-openapi3-2.5.1/examples/header_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/init_oauth_demo.py` & `flask-openapi3-2.5.1/examples/init_oauth_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/nested_apiblueprint_demo.py` & `flask-openapi3-2.5.1/examples/nested_apiblueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/openapi_extensions.py` & `flask-openapi3-2.5.1/examples/openapi_extensions.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/openapi_extra.py` & `flask-openapi3-2.5.1/examples/openapi_extra.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/orjson_demo.py` & `flask-openapi3-2.5.1/examples/orjson_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/pydantic_custom_root_types.py` & `flask-openapi3-2.5.1/examples/pydantic_custom_root_types.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/response_demo.py` & `flask-openapi3-2.5.1/examples/response_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/rest_demo.py` & `flask-openapi3-2.5.1/examples/rest_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/servers_demo.py` & `flask-openapi3-2.5.1/examples/servers_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/simple_demo.py` & `flask-openapi3-2.5.1/examples/simple_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/examples/upload_file_demo.py` & `flask-openapi3-2.5.1/examples/upload_file_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/__init__.py` & `flask-openapi3-2.5.1/flask_openapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/blueprint.py` & `flask-openapi3-2.5.1/flask_openapi3/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/commands.py` & `flask-openapi3-2.5.1/flask_openapi3/commands.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/markdown.py` & `flask-openapi3-2.5.1/flask_openapi3/markdown.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/__init__.py` & `flask-openapi3-2.5.1/flask_openapi3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/callback.py` & `flask-openapi3-2.5.1/flask_openapi3/models/callback.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/components.py` & `flask-openapi3-2.5.1/flask_openapi3/models/components.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/encoding.py` & `flask-openapi3-2.5.1/flask_openapi3/models/encoding.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     """
     https://spec.openapis.org/oas/v3.0.3#encoding-object
     """
 
     contentType: Optional[str] = None
     headers: Optional[Dict[str, Union[Header, Reference]]] = None
     style: Optional[str] = None
-    explode: bool = False
+    explode: Optional[bool] = None
     allowReserved: bool = False
 
     class Config:
         extra = "allow"
```

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/file.py` & `flask-openapi3-2.5.1/flask_openapi3/models/file.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/info.py` & `flask-openapi3-2.5.1/flask_openapi3/models/info.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/link.py` & `flask-openapi3-2.5.1/flask_openapi3/models/link.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/media_type.py` & `flask-openapi3-2.5.1/flask_openapi3/models/media_type.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/operation.py` & `flask-openapi3-2.5.1/flask_openapi3/models/operation.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/parameter.py` & `flask-openapi3-2.5.1/flask_openapi3/models/parameter.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/path_item.py` & `flask-openapi3-2.5.1/flask_openapi3/models/path_item.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/response.py` & `flask-openapi3-2.5.1/flask_openapi3/models/response.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/schema.py` & `flask-openapi3-2.5.1/flask_openapi3/models/schema.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/security.py` & `flask-openapi3-2.5.1/flask_openapi3/models/security.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/security_scheme.py` & `flask-openapi3-2.5.1/flask_openapi3/models/security_scheme.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/models/validation_error.py` & `flask-openapi3-2.5.1/flask_openapi3/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/openapi.py` & `flask-openapi3-2.5.1/flask_openapi3/openapi.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/request.py` & `flask-openapi3-2.5.1/flask_openapi3/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,27 +50,41 @@
     for k, v in form.schema().get("properties", {}).items():
         if v.get("type") == "array":
             items = v.get("items", {})
             if items.get("type") == "string" and items.get("format") == "binary":
                 # List[FileStorage]
                 # eg: {"title": "Files", "type": "array", "items": {"format": "binary", "type": "string"}
                 value = request_files.getlist(k)
+            elif items.get("type") in ["object", "null", None]:
+                # list object, None, $ref, anyOf
+                value = []
+                for i in request_form.getlist(k):
+                    try:
+                        json_loads_result = json.loads(i)
+                    except JSONDecodeError:
+                        json_loads_result = i
+                    value.append(json_loads_result)
             else:
                 # List[str], List[int] ...
                 # eg: {"title": "Files", "type": "array", "items": {"type": "string"}
                 value = request_form.getlist(k)
+        elif v.get("type") in ["object", "null", None]:
+            # list object, None, $ref, anyOf
+            try:
+                value = json.loads(request_form.get(k)) if request_form.get(k) else None
+            except JSONDecodeError:
+                value = request_form.get(k)
         else:
             if v.get("format") == "binary":
                 # FileStorage
                 value = request_files.get(k)
             else:
                 # str, int ...
                 value = request_form.get(k)
-        if value is not None:
-            form_dict[k] = value
+        form_dict[k] = value
     func_kwargs.update({"form": form(**form_dict)})
 
 
 def _do_body(body, func_kwargs):
     obj = request.get_json(silent=True) or {}
     if isinstance(obj, str):
         try:
```

### Comparing `flask-openapi3-2.5.0/flask_openapi3/scaffold.py` & `flask-openapi3-2.5.1/flask_openapi3/scaffold.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/__init__.py` & `flask-openapi3-2.5.1/flask_openapi3/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/css/swagger-ui.css` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/apidoc.svg` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/images/apidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/rapidoc.svg` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/images/rapidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/redoc.svg` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/images/redoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/swagger.svg` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/rapidoc-min.js` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/js/rapidoc-min.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/redoc.standalone.js` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/js/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js` & `flask-openapi3-2.5.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/types.py` & `flask-openapi3-2.5.1/flask_openapi3/types.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3/utils.py` & `flask-openapi3-2.5.1/flask_openapi3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     assert properties, f"{form.__name__}'s properties cannot be empty."
 
     title = schema.get("title") or form.__name__
     components_schemas[title] = Schema(**schema)
     encoding = {}
     for k, v in properties.items():
         if v.get("type") == "array":
-            encoding[k] = Encoding(style="form")
+            encoding[k] = Encoding(style="form", explode=True)
     if extra_form:
         # Update encoding
         if extra_form.encoding:
             encoding.update(**extra_form.encoding)
         content = {
             "multipart/form-data": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
```

### Comparing `flask-openapi3-2.5.0/flask_openapi3/view.py` & `flask-openapi3-2.5.1/flask_openapi3/view.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/flask_openapi3.egg-info/PKG-INFO` & `flask-openapi3-2.5.1/flask_openapi3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.5.0
+Version: 2.5.1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flask-openapi3-2.5.0/flask_openapi3.egg-info/SOURCES.txt` & `flask-openapi3-2.5.1/flask_openapi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.5.0/setup.py` & `flask-openapi3-2.5.1/setup.py`

 * *Files identical despite different names*

