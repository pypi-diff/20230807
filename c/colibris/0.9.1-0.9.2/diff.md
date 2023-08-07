# Comparing `tmp/colibris-0.9.1.tar.gz` & `tmp/colibris-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colibris-0.9.1.tar", last modified: Tue Nov  5 22:52:28 2019, max compression
+gzip compressed data, was "dist/colibris-0.9.2.tar", last modified: Wed Sep  2 08:51:19 2020, max compression
```

## Comparing `colibris-0.9.1.tar` & `colibris-0.9.2.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2019-11-05 22:52:28.000000 colibris-0.9.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2019-11-05 22:52:19.000000 colibris-0.9.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      825 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/api/envelope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1819 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/api/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2764 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/app.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1459 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/apikey.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2161 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3898 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/cookie.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      311 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3050 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/jwt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1280 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authentication/null.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/authorization/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      356 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      370 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/null.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2311 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/rights.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      995 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/authorization/role.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/cache/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      884 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/cache/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      301 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/cache/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1307 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/cache/locmem.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      806 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/cache/redis.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1280 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1252 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/base.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      558 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/makemigrations.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      276 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/migrate.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      269 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/runserver.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      312 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/runworker.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      438 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/shell.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2050 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/commands/test.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/conf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3558 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/conf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1506 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/conf/backends.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3620 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/conf/schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1131 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/conf/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/docs/openapi/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      252 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      330 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/docs/openapi/swagger/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      665 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/favicon-16x16.png
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      628 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/favicon-32x32.png
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1566 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/index.html
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2388 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/oauth2-redirect.html
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   971256 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-bundle.js
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)  4143331 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-bundle.js.map
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   291088 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)  1297846 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js.map
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   141676 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.css
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   482550 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.css.map
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   393813 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.js
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)  1476127 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.js.map
--rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/docs/openapi/views.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/email/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      635 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/email/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/email/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/email/console.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4022 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/email/message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1649 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/email/smtp.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/middleware/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/middleware/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2606 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/middleware/auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2310 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/middleware/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      887 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/monkey.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1433 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/pagination.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/persist/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1770 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/persist/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2613 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/persist/backends.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/persist/models.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/schemas/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       90 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/schemas/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      929 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/schemas/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      484 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/schemas/fields.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/shortcuts.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/skeleton/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/Dockerfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)      188 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/Pipfile
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/skeleton/__packagename__/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      409 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/constants.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      127 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/manage.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/skeleton/__packagename__/migrations/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/migrations/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      454 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/routes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      643 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      882 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/skeleton/__packagename__/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/static/.keep
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/skeleton/__packagename__/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/templates/.keep
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/skeleton/__packagename__/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      347 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/tests/fixtures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      458 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/tests/test_auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      444 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/tests/test_health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2216 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/__packagename__/views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      188 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/docker-compose.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1550 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/skeleton/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2132 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/startproject.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/taskqueue/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      898 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/taskqueue/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/taskqueue/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/taskqueue/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3123 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/taskqueue/rq.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/template/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/template/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/template/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      421 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/template/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1664 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/template/jinja2.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      455 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/test/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/test/fixtures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/test/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1188 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2148 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1523 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris/views/filtering/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/filtering/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3567 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/filtering/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/filtering/fields.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/filtering/operators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      317 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/generic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2556 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/mixins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1243 2019-11-05 22:52:19.000000 colibris-0.9.1/colibris/views/model.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4651 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2019-11-05 22:52:28.000000 colibris-0.9.1/colibris.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2019-11-05 22:52:28.000000 colibris-0.9.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1601 2019-11-05 22:52:19.000000 colibris-0.9.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/conftest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/tests/functional/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/functional/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2451 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/functional/fixtures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1040 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/functional/test_manage.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1416 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/functional/test_skeleton.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/tests/unit/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/tests/unit/authorization/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/authorization/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/authorization/fixtures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2170 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/authorization/test_permissions_class.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/authorization/test_rights_backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      825 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/authorization/test_role_backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3254 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/authorization/test_view_permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1901 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/fixtures.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:28.000000 colibris-0.9.1/tests/unit/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/views/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2082 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/views/test_api_view.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6159 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/views/test_model_view.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5655 2019-11-05 22:52:19.000000 colibris-0.9.1/tests/unit/views/test_model_view_filtering.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2020-09-02 08:51:19.000000 colibris-0.9.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2020-09-02 08:51:12.000000 colibris-0.9.2/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      825 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/api/envelope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1819 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/api/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2764 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/app.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1459 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/apikey.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2161 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3898 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/cookie.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      311 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3050 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/jwt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1280 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authentication/null.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/authorization/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      356 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      370 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/null.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2311 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/rights.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      995 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/authorization/role.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/cache/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      884 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/cache/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      301 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/cache/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1307 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/cache/locmem.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      806 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/cache/redis.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1280 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1252 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/base.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      558 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/makemigrations.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      276 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/migrate.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      269 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/runserver.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      312 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/runworker.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      438 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/shell.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2050 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/commands/test.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/conf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3558 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/conf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1506 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/conf/backends.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3620 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/conf/schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1131 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/conf/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/docs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/docs/openapi/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      252 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      330 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/docs/openapi/swagger/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      665 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/favicon-16x16.png
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      628 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/favicon-32x32.png
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1566 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/index.html
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2388 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/oauth2-redirect.html
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)   971256 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-bundle.js
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)  4143331 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-bundle.js.map
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)   291088 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)  1297846 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js.map
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)   141676 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.css
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)   482550 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.css.map
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)   393813 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.js
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)  1476127 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.js.map
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/docs/openapi/views.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/email/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      635 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/email/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/email/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/email/console.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4022 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/email/message.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1649 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/email/smtp.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/middleware/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/middleware/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2606 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/middleware/auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2310 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/middleware/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      887 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/monkey.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1433 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/pagination.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/persist/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1770 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/persist/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2613 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/persist/backends.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/persist/models.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/schemas/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       90 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/schemas/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      929 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/schemas/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      484 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/schemas/fields.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/shortcuts.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/skeleton/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/Dockerfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      188 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/Pipfile
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/skeleton/__packagename__/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      409 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/constants.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      127 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/manage.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/skeleton/__packagename__/migrations/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/migrations/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      454 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/routes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      643 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      882 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/skeleton/__packagename__/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/static/.keep
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/skeleton/__packagename__/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/templates/.keep
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/skeleton/__packagename__/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      347 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/tests/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      458 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/tests/test_auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      444 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/tests/test_health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2216 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/__packagename__/views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      188 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/docker-compose.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1550 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/skeleton/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2132 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/startproject.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/taskqueue/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      898 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/taskqueue/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/taskqueue/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/taskqueue/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3123 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/taskqueue/rq.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/template/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/template/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/template/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      421 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/template/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1664 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/template/jinja2.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      455 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/test/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/test/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      504 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/test/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1188 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2148 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1523 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/base.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris/views/filtering/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/filtering/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3567 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/filtering/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/filtering/fields.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/filtering/operators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      317 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/generic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2556 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1243 2020-09-02 08:51:12.000000 colibris-0.9.2/colibris/views/model.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4651 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2020-09-02 08:51:19.000000 colibris-0.9.2/colibris.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2020-09-02 08:51:19.000000 colibris-0.9.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1594 2020-09-02 08:51:12.000000 colibris-0.9.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/conftest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/tests/functional/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/functional/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2451 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/functional/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1040 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/functional/test_manage.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1416 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/functional/test_skeleton.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/tests/unit/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/tests/unit/authorization/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/authorization/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/authorization/fixtures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2170 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/authorization/test_permissions_class.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1274 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/authorization/test_rights_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      825 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/authorization/test_role_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3254 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/authorization/test_view_permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1901 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/fixtures.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:19.000000 colibris-0.9.2/tests/unit/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/views/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2082 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/views/test_api_view.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6159 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/views/test_model_view.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5655 2020-09-02 08:51:12.000000 colibris-0.9.2/tests/unit/views/test_model_view_filtering.py
```

### Comparing `colibris-0.9.1/PKG-INFO` & `colibris-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colibris
-Version: 0.9.1
+Version: 0.9.2
 Summary: A lightweight framework for RESTful microservices
 Home-page: https://github.com/colibris-framework/colibris
 Author: The Colibris Team
 License: BSD
 Description: # Colibris Framework
```

### Comparing `colibris-0.9.1/README.md` & `colibris-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/__init__.py` & `colibris-0.9.2/colibris/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from colibris import conf
 from colibris import email
 from colibris import persist
 from colibris import taskqueue
 from colibris import template
 
 
-VERSION = '0.9.1'
+VERSION = '0.9.2'
 
 
 def setup():
     authentication.setup()
     authorization.setup()
     cache.setup()
     email.setup()
```

### Comparing `colibris-0.9.1/colibris/api/envelope.py` & `colibris-0.9.2/colibris/api/envelope.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/api/exceptions.py` & `colibris-0.9.2/colibris/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/app.py` & `colibris-0.9.2/colibris/app.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authentication/__init__.py` & `colibris-0.9.2/colibris/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authentication/apikey.py` & `colibris-0.9.2/colibris/authentication/apikey.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authentication/base.py` & `colibris-0.9.2/colibris/authentication/base.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authentication/cookie.py` & `colibris-0.9.2/colibris/authentication/cookie.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authentication/jwt.py` & `colibris-0.9.2/colibris/authentication/jwt.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authentication/model.py` & `colibris-0.9.2/colibris/authentication/model.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authorization/permissions.py` & `colibris-0.9.2/colibris/authorization/permissions.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authorization/rights.py` & `colibris-0.9.2/colibris/authorization/rights.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/authorization/role.py` & `colibris-0.9.2/colibris/authorization/role.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/cache/__init__.py` & `colibris-0.9.2/colibris/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/cache/locmem.py` & `colibris-0.9.2/colibris/cache/locmem.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/cache/redis.py` & `colibris-0.9.2/colibris/cache/redis.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/commands/__init__.py` & `colibris-0.9.2/colibris/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/commands/base.py` & `colibris-0.9.2/colibris/commands/base.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/commands/makemigrations.py` & `colibris-0.9.2/colibris/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/commands/test.py` & `colibris-0.9.2/colibris/commands/test.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/conf/__init__.py` & `colibris-0.9.2/colibris/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/conf/backends.py` & `colibris-0.9.2/colibris/conf/backends.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/conf/schemas.py` & `colibris-0.9.2/colibris/conf/schemas.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/conf/settings.py` & `colibris-0.9.2/colibris/conf/settings.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/favicon-16x16.png` & `colibris-0.9.2/colibris/docs/openapi/swagger/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/favicon-32x32.png` & `colibris-0.9.2/colibris/docs/openapi/swagger/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/index.html` & `colibris-0.9.2/colibris/docs/openapi/swagger/index.html`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/oauth2-redirect.html` & `colibris-0.9.2/colibris/docs/openapi/swagger/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-bundle.js` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-bundle.js.map` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js.map` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.css` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.css.map` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.js` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/swagger/swagger-ui.js.map` & `colibris-0.9.2/colibris/docs/openapi/swagger/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/docs/openapi/views.py` & `colibris-0.9.2/colibris/docs/openapi/views.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/email/__init__.py` & `colibris-0.9.2/colibris/email/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/email/console.py` & `colibris-0.9.2/colibris/email/console.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/email/message.py` & `colibris-0.9.2/colibris/email/message.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/email/smtp.py` & `colibris-0.9.2/colibris/email/smtp.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/middleware/auth.py` & `colibris-0.9.2/colibris/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/middleware/errors.py` & `colibris-0.9.2/colibris/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/monkey.py` & `colibris-0.9.2/colibris/monkey.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/pagination.py` & `colibris-0.9.2/colibris/pagination.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/persist/__init__.py` & `colibris-0.9.2/colibris/persist/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/persist/backends.py` & `colibris-0.9.2/colibris/persist/backends.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/schemas/base.py` & `colibris-0.9.2/colibris/schemas/base.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/shortcuts.py` & `colibris-0.9.2/colibris/shortcuts.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/skeleton/.gitignore` & `colibris-0.9.2/colibris/skeleton/.gitignore`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/skeleton/Dockerfile` & `colibris-0.9.2/colibris/skeleton/Dockerfile`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/skeleton/__packagename__/schemas.py` & `colibris-0.9.2/colibris/skeleton/__packagename__/schemas.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/skeleton/__packagename__/settings.py` & `colibris-0.9.2/colibris/skeleton/__packagename__/settings.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/skeleton/__packagename__/views.py` & `colibris-0.9.2/colibris/skeleton/__packagename__/views.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/skeleton/setup.py` & `colibris-0.9.2/colibris/skeleton/setup.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/startproject.py` & `colibris-0.9.2/colibris/startproject.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/taskqueue/__init__.py` & `colibris-0.9.2/colibris/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/taskqueue/rq.py` & `colibris-0.9.2/colibris/taskqueue/rq.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/template/__init__.py` & `colibris-0.9.2/colibris/template/__init__.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/template/jinja2.py` & `colibris-0.9.2/colibris/template/jinja2.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/utils.py` & `colibris-0.9.2/colibris/utils.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/views/api.py` & `colibris-0.9.2/colibris/views/api.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/views/base.py` & `colibris-0.9.2/colibris/views/base.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/views/filtering/base.py` & `colibris-0.9.2/colibris/views/filtering/base.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/views/filtering/fields.py` & `colibris-0.9.2/colibris/views/filtering/fields.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/views/mixins.py` & `colibris-0.9.2/colibris/views/mixins.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris/views/model.py` & `colibris-0.9.2/colibris/views/model.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/colibris.egg-info/PKG-INFO` & `colibris-0.9.2/colibris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colibris
-Version: 0.9.1
+Version: 0.9.2
 Summary: A lightweight framework for RESTful microservices
 Home-page: https://github.com/colibris-framework/colibris
 Author: The Colibris Team
 License: BSD
 Description: # Colibris Framework
```

### Comparing `colibris-0.9.1/colibris.egg-info/SOURCES.txt` & `colibris-0.9.2/colibris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/setup.py` & `colibris-0.9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,24 @@
     return 'unknown'
 
 
 setup(
     name='colibris',
     version=find_version(),
     install_requires=[
-        'aiohttp>=3.5.0,<=3.5.4',
+        'aiohttp>=3.5.0,<3.7',
         'aiohttp-apispec>=1.5',
         'apispec>=3.0.0',
         'async-timeout',
-        'marshmallow>=3.0.0b19,<=3.0.0rc7',
-        'marshmallow_peewee==2.3.0',
+        'marshmallow>=3.0.0b19,<3.8',
+        'marshmallow_peewee>=2.3.0,<3.1',
         'peewee>=3.9',
-        'peewee-migrate==1.1.6',
+        'peewee-migrate>=1.1.6',
         'python-dotenv',
-        'webargs>=5.2.0,<=5.3.2'
+        'webargs>=5.2.0,<6.0'
     ],
     url='https://github.com/colibris-framework/colibris',
     license='BSD',
     description='A lightweight framework for RESTful microservices',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='The Colibris Team',
```

### Comparing `colibris-0.9.1/tests/functional/fixtures.py` & `colibris-0.9.2/tests/functional/fixtures.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/functional/test_manage.py` & `colibris-0.9.2/tests/functional/test_manage.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/functional/test_skeleton.py` & `colibris-0.9.2/tests/functional/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/authorization/test_permissions_class.py` & `colibris-0.9.2/tests/unit/authorization/test_permissions_class.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/authorization/test_rights_backend.py` & `colibris-0.9.2/tests/unit/authorization/test_rights_backend.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/authorization/test_role_backend.py` & `colibris-0.9.2/tests/unit/authorization/test_role_backend.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/authorization/test_view_permissions.py` & `colibris-0.9.2/tests/unit/authorization/test_view_permissions.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/fixtures.py` & `colibris-0.9.2/tests/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/views/test_api_view.py` & `colibris-0.9.2/tests/unit/views/test_api_view.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/views/test_model_view.py` & `colibris-0.9.2/tests/unit/views/test_model_view.py`

 * *Files identical despite different names*

### Comparing `colibris-0.9.1/tests/unit/views/test_model_view_filtering.py` & `colibris-0.9.2/tests/unit/views/test_model_view_filtering.py`

 * *Files identical despite different names*

