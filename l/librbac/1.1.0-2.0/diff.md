# Comparing `tmp/librbac-1.1.0.tar.gz` & `tmp/librbac-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librbac-1.1.0.tar", last modified: Tue Nov 29 06:13:42 2022, max compression
+gzip compressed data, was "librbac-2.0.tar", last modified: Mon Aug  7 08:52:53 2023, max compression
```

## Comparing `librbac-1.1.0.tar` & `librbac-2.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.418770 librbac-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     3459 2022-08-19 09:50:41.000000 librbac-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      290 2022-08-19 09:50:41.000000 librbac-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5943 2022-11-29 06:13:42.418770 librbac-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5113 2022-11-29 06:13:16.000000 librbac-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.363770 librbac-1.1.0/requirements/
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-08 11:50:55.000000 librbac-1.1.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-08-19 09:50:41.000000 librbac-1.1.0/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-29 06:13:42.418770 librbac-1.1.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2234 2022-11-08 11:50:55.000000 librbac-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.361770 librbac-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.382770 librbac-1.1.0/src/librbac/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      116 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.384770 librbac-1.1.0/src/librbac/backends/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4689 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/backends/base.py
--rw-r--r--   0 root         (0) root         (0)      667 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/backends/remote.py
--rw-r--r--   0 root         (0) root         (0)      484 2022-09-20 07:08:01.000000 librbac-1.1.0/src/librbac/config.py
--rw-r--r--   0 root         (0) root         (0)     1219 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.413770 librbac-1.1.0/src/librbac/drf/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/drf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/drf/permissions.py
--rw-r--r--   0 root         (0) root         (0)      794 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/drf/viewsets.py
--rw-r--r--   0 root         (0) root         (0)      610 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.414770 librbac-1.1.0/src/librbac/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 06:13:16.000000 librbac-1.1.0/src/librbac/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.414770 librbac-1.1.0/src/librbac/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 06:13:16.000000 librbac-1.1.0/src/librbac/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1766 2022-11-29 06:13:16.000000 librbac-1.1.0/src/librbac/management/commands/rbac.py
--rw-r--r--   0 root         (0) root         (0)     9584 2022-11-29 06:13:16.000000 librbac-1.1.0/src/librbac/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.414770 librbac-1.1.0/src/librbac/oidc/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/oidc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/oidc/auth.py
--rw-r--r--   0 root         (0) root         (0)     2082 2022-11-29 06:13:16.000000 librbac-1.1.0/src/librbac/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.417770 librbac-1.1.0/src/librbac/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1366 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/utils/jwt.py
--rw-r--r--   0 root         (0) root         (0)     1449 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/utils/management.py
--rw-r--r--   0 root         (0) root         (0)     1186 2022-08-19 09:50:41.000000 librbac-1.1.0/src/librbac/utils/rbac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-29 06:13:42.383770 librbac-1.1.0/src/librbac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5943 2022-11-29 06:13:42.000000 librbac-1.1.0/src/librbac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      892 2022-11-29 06:13:42.000000 librbac-1.1.0/src/librbac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-29 06:13:42.000000 librbac-1.1.0/src/librbac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-29 06:13:42.000000 librbac-1.1.0/src/librbac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-29 06:13:42.000000 librbac-1.1.0/src/librbac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      450 2022-11-29 06:13:42.000000 librbac-1.1.0/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.147437 librbac-2.0/
+-rw-r--r--   0 root         (0) root         (0)     3459 2022-08-19 09:50:41.000000 librbac-2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      290 2022-08-19 09:50:41.000000 librbac-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6744 2023-08-07 08:52:53.146438 librbac-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-08-07 08:52:41.000000 librbac-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.133437 librbac-2.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-08-07 08:52:41.000000 librbac-2.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-19 09:50:41.000000 librbac-2.0/requirements/prod.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 08:52:53.147437 librbac-2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2234 2022-11-08 11:50:55.000000 librbac-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.129437 librbac-2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.137437 librbac-2.0/src/librbac/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.140437 librbac-2.0/src/librbac/backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/backends/base.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/backends/local.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/backends/remote.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/config.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.141437 librbac-2.0/src/librbac/drf/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/drf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/drf/permissions.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/drf/viewsets.py
+-rw-r--r--   0 root         (0) root         (0)      610 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.142437 librbac-2.0/src/librbac/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 06:13:16.000000 librbac-2.0/src/librbac/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.142437 librbac-2.0/src/librbac/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-29 06:13:16.000000 librbac-2.0/src/librbac/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/management/commands/rbac.py
+-rw-r--r--   0 root         (0) root         (0)     8950 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.143437 librbac-2.0/src/librbac/oidc/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/oidc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/oidc/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.146438 librbac-2.0/src/librbac/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/utils/jwt.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2022-08-19 09:50:41.000000 librbac-2.0/src/librbac/utils/management.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-08-07 08:52:41.000000 librbac-2.0/src/librbac/utils/rbac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:52:53.139437 librbac-2.0/src/librbac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6744 2023-08-07 08:52:53.000000 librbac-2.0/src/librbac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      929 2023-08-07 08:52:53.000000 librbac-2.0/src/librbac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-08-07 08:52:53.000000 librbac-2.0/src/librbac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-08-07 08:52:53.000000 librbac-2.0/src/librbac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-07 08:52:53.000000 librbac-2.0/src/librbac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      446 2023-08-07 08:52:53.000000 librbac-2.0/version.conf
```

### Comparing `librbac-1.1.0/LICENSE` & `librbac-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `librbac-1.1.0/PKG-INFO` & `librbac-2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,16 @@
-Metadata-Version: 2.1
-Name: librbac
-Version: 1.1.0
-Summary: Общая библиотека контроля доступа для микросервисов
-Home-page: https://stash.bars-open.ru/projects/EDUEO/repos/librbac/
-Author: BARS Group
-Author-email: education_dev@bars-open.ru
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Web Environment
-Classifier: Natural Language :: Russian
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Общая библиотека контроля доступа для микросервисов
 
 ## Подключение
 settings.py:
     
     INSTALLED_APPS = [
-        'librbac',      # для management команд --list-permissions и --push-permissions
         ...
+        'testapp.core',
+        'librbac',      # для management команд --list-permissions и --push-permissions
     ]
     
     REST_FRAMEWORK = {
         'DEFAULT_AUTHENTICATION_CLASSES': (
             'oidc_auth.authentication.JSONWebTokenAuthentication',
         ),
     }
@@ -51,14 +31,42 @@
         # `aud` is only required, when you set it as an essential claim.
         'OIDC_CLAIMS_OPTIONS': {
             'iss': {
                 'essential': True,
             }
         },
     }
+    
+    RBAC_BACKEND = 'librbac.backends.remote.RemoteBackend'
+    """Путь до бэкенда RBAC"""
+    
+    
+    RBAC_PERMISSION_TOPIC = 'test.rbac.permission'
+    """Наименование топика в который публикуются события связанные с разрешениями."""
+
+
+testapp/&#95;&#95;init__.py:
+
+    from typing import TYPE_CHECKING
+    
+    from explicit.contrib.messagebus.event_registry import Registry
+    
+    
+    if TYPE_CHECKING:
+        from explicit.messagebus.messagebus import MessageBus  # noqa
+    
+    
+    default_app_config = f'{__package__}.apps.AppConfig'
+    
+    
+    bus: 'MessageBus'
+    
+    event_registry = Registry()
+
+
 
 testapp/apps.py:
 
     from django.apps.config import AppConfig as AppConfigBase
     
     from librbac.events import PermissionPushed
     from librbac.utils.management import is_in_management_command
@@ -67,38 +75,40 @@
     class AppConfig(AppConfigBase):
     
         name = __package__
     
         def _bootstrap(self):
             """Предоставление общей шины ядра."""
             from explicit.messagebus.messagebus import MessageBus
-            from auth.apps import core
+            from testapp import core
             from .unit_of_work import UnitOfWork
             uow = UnitOfWork()
             dependencies = dict(uow=uow)
             messagebus = MessageBus(**dependencies)
             core.bus = messagebus
     
         def _register_events(self):
             ...
     
         def _configure_rbac(self):
             from librbac import config
             from librbac.manager import rbac
             from testapp import core
+            from testapp.core import event_registry as registry
             from testapp.core.adapters import messaging
     
             class Config(config.IConfig):
                 bus = core.bus
                 adapter = messaging.adapter
+                event_registry = registry
 
             config.rbac_config = Config()
     
-            # не пушим разрешения в шину, если выполняется management команда
-            rbac.init(push_permissions=not is_in_management_command())
+            # не пушим разрешения в шину при старте. Этим занимается management команда.
+            rbac.init()
     
     
         def ready(self):
             self._bootstrap()
             self._register_events()
             self._configure_rbac()
```

### Comparing `librbac-1.1.0/setup.py` & `librbac-2.0/setup.py`

 * *Files identical despite different names*

### Comparing `librbac-1.1.0/src/librbac/backends/base.py` & `librbac-2.0/src/librbac/backends/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,15 @@
         for permission, title in self._manager.permissions.items():
             yield PermissionPushed(
                 namespace=permission.namespace,
                 resource=permission.resource,
                 action=permission.action,
                 scope=permission.scope,
                 title=title,
-                module=module_perm_group_mapping[
-                    PermissionGroup(permission.namespace, permission.resource)
-                ],
+                module=module_perm_group_mapping[PermissionGroup(permission.namespace, permission.resource)],
             )
 
     @abstractmethod
     def push_permission(self, event: PermissionPushed):
         """Обновляет одно разрешение в хранилище."""
 
     def push_permissions(self):
```

### Comparing `librbac-1.1.0/src/librbac/drf/viewsets.py` & `librbac-2.0/src/librbac/drf/viewsets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+from typing import TYPE_CHECKING
+from typing import Union
+
 from django.utils.decorators import classonlymethod
 
 from librbac.drf.permissions import HasAccess
 from librbac.types import Permission
 from librbac.types import TPermMapDict
 
 
+if TYPE_CHECKING:
+    from rest_framework.viewsets import GenericViewSet
+
+
 class RBACMixin:
 
     """Примесь для ViewSet'ов требующих контроля доступа."""
 
     perm_map: TPermMapDict
     """Сопоставление ViewSet'а и требуемых разрешений."""
 
     permission_classes = (
         HasAccess,
     )
 
     @classonlymethod
-    def as_view(cls, actions=None, **initkwargs):
+    def as_view(cls: Union['GenericViewSet', 'RBACMixin'], actions=None, **initkwargs):
         assert isinstance(cls.perm_map, dict)
         assert len(cls.perm_map)
         for action, perms in cls.perm_map.items():
             assert all(isinstance(p, Permission) for p in perms)
         return super().as_view(actions=actions, **initkwargs)
```

### Comparing `librbac-1.1.0/src/librbac/events.py` & `librbac-2.0/src/librbac/events.py`

 * *Files identical despite different names*

### Comparing `librbac-1.1.0/src/librbac/management/commands/rbac.py` & `librbac-2.0/src/librbac/management/commands/rbac.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         except ImportError as ie:
             raise CommandError(
                 'Не удалось импортировать настройки модуля. '
                 'Вероятно, система контроля доступа не сконфигурирована.'
             ) from ie
 
         if options['list_permissions']:
-            rbac.init(False)
+            rbac.init()
             self._write_line('namespace', 'resource', 'action', 'scope', 'title')
             for (namespace, resource, action, scope), title in rbac.permissions.items():
                 self._write_line(namespace, resource, action, scope, title)
         if options['push_permissions']:
             self.stdout.write('Сохранение загруженных разрешений в хранилище...')
             rbac.init(push_permissions=True)
             self.stdout.write('Завершено.')
```

### Comparing `librbac-1.1.0/src/librbac/manager.py` & `librbac-2.0/src/librbac/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.functional import cached_property
 
 from librbac.types import Permission
+from librbac.types import PermissionGroup
 from librbac.types import TRule
 from librbac.utils.rbac import _get_rbac_viewsets
 
 
 if TYPE_CHECKING:
     from rest_framework.viewsets import GenericViewSet
 
@@ -39,18 +40,17 @@
 class RBACManager(object):
 
     """Менеджер системы контроля доступа RBAC."""
 
     _msg_perm_not_found = 'Разрешение "{}" не востребовано'
 
     def __init__(self):
-        self.partitions = defaultdict(set)  # Разделы системы
-        self.groups = {}  # Группы разрешений
+        self.partitions: Dict[str, set[PermissionGroup]] = defaultdict(set)  # Разделы системы
         self.permissions: Dict[Permission, str] = {}
-        self.permission_dependencies = defaultdict(set)
+        self.permission_dependencies: Dict[Permission, Set[Permission, ...]] = defaultdict(set)
         self.permission_rules: dict[Permission, list[TRule]] = defaultdict(list)
 
     def _collect_partitions(self, permission_modules: Tuple[ModuleType, ...]):
         """Сбор информации о разделах системы.
 
         Разделами системы являются объединения групп разрешений.
         """
@@ -68,31 +68,14 @@
                     assert perm_group not in processed_groups, (
                         f'Группа разрешений "{perm_group}" уже '
                         f'закреплена за другим разделом системы.'
                     )
                     self.partitions[title].add(perm_group)
                     processed_groups.add(perm_group)
 
-    def _collect_groups(self, permission_modules: Tuple[ModuleType, ...]):
-        """Сбор информации о группах разрешений."""
-        self.groups.clear()
-
-        for module in permission_modules:
-            groups = getattr(module, 'groups', None)
-            if groups is None:
-                continue
-
-            for code, title in groups.items():
-                assert code not in self.groups, (
-                    f'Группа разрешений "{code}" ({title}) '
-                    'уже описана в другом приложении.'
-                )
-
-                self.groups[code] = title
-
     def _collect_permissions(
         self,
         permissions_modules: Tuple[ModuleType, ...]
     ):
         """Сбор разрешений системы."""
         self.permissions.clear()
 
@@ -151,15 +134,14 @@
                     assert callable(handler), handler
                     self.permission_rules[permission].append(handler)
 
     def _push_permissions(self):
         """
         Обновление списка разрешений в хранилище основе разрешений системы.
         """
-        # TODO: пропускать в миграциях
         self._backend.push_permissions()
 
     def get_dependent_permissions(
         self,
         permission: 'Permission',
         _result: Set = None
     ) -> Set[Permission]:
@@ -178,15 +160,15 @@
                 )
 
         if primary_permission:
             _result.remove(primary_permission)
 
         return _result
 
-    def init(self, push_permissions: bool = True):
+    def init(self, push_permissions: bool = False):
         """Инициализация модуля контроля доступа.
 
         1. Загружает из приложений системы списки правил и разрешений. Их поиск
            осуществляется в модуле ``permissions``.
         2. Для каждого правила и разрешения создает/обновляет запись
             в хранилище.
 
@@ -199,40 +181,39 @@
         self._collect_permissions(modules)
         self._collect_dependencies(modules)
 
         # Сбор обработчиков правил для разрешений системы
         self._collect_rules(modules)
 
         # Сбор групп разрешений и разделов системы
-        self._collect_groups(modules)
         self._collect_partitions(modules)
 
         if push_permissions:
             self._push_permissions()
 
     @cached_property
     def _backend(self):
-        backend_name = getattr(settings, 'RBAC_BACKEND', None) or (
-            __name__.rpartition('.')[0] + '.backends.remote.RemoteBackend'
-        )
+        from librbac import default_settings
+        backend_name = getattr(settings, 'RBAC_BACKEND', None) or getattr(default_settings, 'RBAC_BACKEND')
         module_name, class_name = backend_name.rsplit('.', 1)
 
         try:
             module = import_module(module_name)
         except ImportError as e:
+            module = import_module(module_name)
             raise ImproperlyConfigured(
                 f'Не удалось импортировать бэкенд RBAC {module_name}: "{e}"'
-            )
+            ) from e
 
         try:
             backend_class = getattr(module, class_name)
-        except AttributeError:
+        except AttributeError as e:
             raise ImproperlyConfigured(
                 f'Модуль "{module}" не содержит бэкенд RBAC"{class_name}"'
-            )
+            ) from e
         else:
             backend = backend_class(self)
 
         return backend
 
     def has_access(self, viewset: 'GenericViewSet', request) -> bool:
         """Проверяет наличие у пользователя доступа (с учётом правил)."""
```

### Comparing `librbac-1.1.0/src/librbac/oidc/auth.py` & `librbac-2.0/src/librbac/oidc/auth.py`

 * *Files identical despite different names*

### Comparing `librbac-1.1.0/src/librbac/types.py` & `librbac-2.0/src/librbac/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from typing import Optional
 from typing import Tuple
 from typing import TypedDict
 from typing import Union
 
 
 if TYPE_CHECKING:
-    from explicit.messagebus import MessageBus
-    from explicit.unit_of_work import AbstractUnitOfWork
     from rest_framework.request import Request
     from rest_framework.viewsets import GenericViewSet
 
 
 class PermissionGroup(NamedTuple):
 
     """Структура группы разрешений."""
@@ -58,17 +56,10 @@
         viewset: 'GenericViewSet',
         request: 'Request',
         user: TUser,
     ) -> bool:
         """Проверка доступа."""
 
 
-class TPermMapDict(TypedDict):
+TPermMapDict = dict[str, Tuple[Permission, ...]]
+"""Структура сопоставления разрешений с действиями во ViewSet'е."""
 
-    """Структура сопоставления разрешений с действиями во ViewSet'е."""
-
-    create: Tuple[Permission, ...]
-    retrieve: Tuple[Permission, ...]
-    update: Tuple[Permission, ...]
-    partial_update: Tuple[Permission, ...]
-    list: Tuple[Permission, ...]
-    destroy: Tuple[Permission, ...]
```

### Comparing `librbac-1.1.0/src/librbac/utils/jwt.py` & `librbac-2.0/src/librbac/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `librbac-1.1.0/src/librbac/utils/management.py` & `librbac-2.0/src/librbac/utils/management.py`

 * *Files identical despite different names*

### Comparing `librbac-1.1.0/src/librbac/utils/rbac.py` & `librbac-2.0/src/librbac/utils/rbac.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 from importlib import import_module
+from typing import TYPE_CHECKING
 from typing import Generator
 from typing import Set
 from typing import Type
+from typing import Union
 
 from django.conf import settings
+from django.core.exceptions import ImproperlyConfigured
 from rest_framework.viewsets import GenericViewSet
 
 
+if TYPE_CHECKING:
+    from librbac.drf.viewsets import RBACMixin
+
+
+def get_rbac_topic_permission() -> str:
+    from django.conf import settings
+    topic_attr = 'RBAC_PERMISSION_TOPIC'
+    from librbac import default_settings
+    topic_name = getattr(settings, topic_attr, None) or getattr(default_settings, topic_attr)
+    if not topic_name:
+        raise ImproperlyConfigured(
+            f'Необходимо указать {topic_attr} в настройках.'
+        )
+    return topic_name
+
+
 def get_all_viewsets(
     urlpatterns,
     viewsets=None
 ) -> Set[Type[GenericViewSet]]:
     """Находит и возвращает все ViewSet'ы системы."""
     viewsets = viewsets if viewsets is not None else set()
     for pattern in urlpatterns:
@@ -20,14 +39,14 @@
             if cls := getattr(pattern.callback, 'cls', None):
                 if issubclass(cls, GenericViewSet):
                     viewsets.add(cls)
 
     return viewsets
 
 
-def _get_rbac_viewsets() -> Generator[GenericViewSet, None, None]:
+def _get_rbac_viewsets() -> Generator[Union[GenericViewSet, 'RBACMixin'], None, None]:
     """Возвращает ViewSet'ы системы, доступ к которым нужно проверять."""
     from librbac.drf.viewsets import RBACMixin
     urlpatterns = import_module(settings.ROOT_URLCONF).urlpatterns
     for viewset in get_all_viewsets(urlpatterns):
         if issubclass(viewset, RBACMixin):
             yield viewset
```

### Comparing `librbac-1.1.0/src/librbac.egg-info/PKG-INFO` & `librbac-2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librbac
-Version: 1.1.0
+Version: 2.0
 Summary: Общая библиотека контроля доступа для микросервисов
 Home-page: https://stash.bars-open.ru/projects/EDUEO/repos/librbac/
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
@@ -21,16 +21,17 @@
 
 # Общая библиотека контроля доступа для микросервисов
 
 ## Подключение
 settings.py:
     
     INSTALLED_APPS = [
-        'librbac',      # для management команд --list-permissions и --push-permissions
         ...
+        'testapp.core',
+        'librbac',      # для management команд --list-permissions и --push-permissions
     ]
     
     REST_FRAMEWORK = {
         'DEFAULT_AUTHENTICATION_CLASSES': (
             'oidc_auth.authentication.JSONWebTokenAuthentication',
         ),
     }
@@ -51,14 +52,42 @@
         # `aud` is only required, when you set it as an essential claim.
         'OIDC_CLAIMS_OPTIONS': {
             'iss': {
                 'essential': True,
             }
         },
     }
+    
+    RBAC_BACKEND = 'librbac.backends.remote.RemoteBackend'
+    """Путь до бэкенда RBAC"""
+    
+    
+    RBAC_PERMISSION_TOPIC = 'test.rbac.permission'
+    """Наименование топика в который публикуются события связанные с разрешениями."""
+
+
+testapp/&#95;&#95;init__.py:
+
+    from typing import TYPE_CHECKING
+    
+    from explicit.contrib.messagebus.event_registry import Registry
+    
+    
+    if TYPE_CHECKING:
+        from explicit.messagebus.messagebus import MessageBus  # noqa
+    
+    
+    default_app_config = f'{__package__}.apps.AppConfig'
+    
+    
+    bus: 'MessageBus'
+    
+    event_registry = Registry()
+
+
 
 testapp/apps.py:
 
     from django.apps.config import AppConfig as AppConfigBase
     
     from librbac.events import PermissionPushed
     from librbac.utils.management import is_in_management_command
@@ -67,38 +96,40 @@
     class AppConfig(AppConfigBase):
     
         name = __package__
     
         def _bootstrap(self):
             """Предоставление общей шины ядра."""
             from explicit.messagebus.messagebus import MessageBus
-            from auth.apps import core
+            from testapp import core
             from .unit_of_work import UnitOfWork
             uow = UnitOfWork()
             dependencies = dict(uow=uow)
             messagebus = MessageBus(**dependencies)
             core.bus = messagebus
     
         def _register_events(self):
             ...
     
         def _configure_rbac(self):
             from librbac import config
             from librbac.manager import rbac
             from testapp import core
+            from testapp.core import event_registry as registry
             from testapp.core.adapters import messaging
     
             class Config(config.IConfig):
                 bus = core.bus
                 adapter = messaging.adapter
+                event_registry = registry
 
             config.rbac_config = Config()
     
-            # не пушим разрешения в шину, если выполняется management команда
-            rbac.init(push_permissions=not is_in_management_command())
+            # не пушим разрешения в шину при старте. Этим занимается management команда.
+            rbac.init()
     
     
         def ready(self):
             self._bootstrap()
             self._register_events()
             self._configure_rbac()
```

### Comparing `librbac-1.1.0/src/librbac.egg-info/SOURCES.txt` & `librbac-2.0/src/librbac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 setup.py
 version.conf
 requirements/base.txt
 requirements/prod.txt
 src/librbac/__init__.py
 src/librbac/apps.py
 src/librbac/config.py
-src/librbac/constants.py
+src/librbac/default_settings.py
 src/librbac/events.py
 src/librbac/manager.py
 src/librbac/types.py
 src/librbac.egg-info/PKG-INFO
 src/librbac.egg-info/SOURCES.txt
 src/librbac.egg-info/dependency_links.txt
 src/librbac.egg-info/requires.txt
 src/librbac.egg-info/top_level.txt
 src/librbac/backends/__init__.py
 src/librbac/backends/base.py
+src/librbac/backends/local.py
 src/librbac/backends/remote.py
 src/librbac/drf/__init__.py
 src/librbac/drf/permissions.py
 src/librbac/drf/viewsets.py
 src/librbac/management/__init__.py
 src/librbac/management/commands/__init__.py
 src/librbac/management/commands/rbac.py
```

