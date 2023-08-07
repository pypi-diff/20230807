# Comparing `tmp/traits-6.4.1.tar.gz` & `tmp/traits-6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traits-6.4.1.tar", last modified: Fri Aug 12 11:16:25 2022, max compression
+gzip compressed data, was "traits-6.4.2.tar", last modified: Mon Aug  7 10:47:53 2023, max compression
```

## Comparing `traits-6.4.1.tar` & `traits-6.4.2.tar`

### file list

```diff
@@ -1,460 +1,458 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.828029 traits-6.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)    74621 2022-08-12 11:16:17.000000 traits-6.4.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    19467 2022-08-12 11:16:17.000000 traits-6.4.1/LICENSE-CC-BY-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-08-12 11:16:17.000000 traits-6.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-08-12 11:16:17.000000 traits-6.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-08-12 11:16:25.828029 traits-6.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-08-12 11:16:17.000000 traits-6.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.776028 traits-6.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-08-12 11:16:17.000000 traits-6.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6472 2022-08-12 11:16:17.000000 traits-6.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.776028 traits-6.4.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.776028 traits-6.4.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    13514 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/_static/e-logo-rev.png
--rw-r--r--   0 runner    (1001) docker     (121)    10134 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/_static/et.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.776028 traits-6.4.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/_templates/search.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8778 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.780028 traits-6.4.1/docs/source/traits_api_reference/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/base_trait_handler.rst
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/constants.rst
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/ctrait.rst
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/ctraits.rst
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/editor_factories.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/has_traits.rst
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/interface_checker.rst
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_converters.rst
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_dict_object.rst
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_factory.rst
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_handler.rst
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_handlers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_list_object.rst
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_notifiers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_numeric.rst
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_set_object.rst
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_type.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5026 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/trait_types.rst
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits.adaptation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits.etsconfig.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits.observation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits.rst
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits.testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits.util.rst
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/traits_listener.rst
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_api_reference/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.780028 traits-6.4.1/docs/source/traits_tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_tutorial/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.780028 traits-6.4.1/docs/source/traits_user_manual/
--rw-r--r--   0 runner    (1001) docker     (121)    58499 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/appendix.rst
--rw-r--r--   0 runner    (1001) docker     (121)    22616 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/custom.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/debugging.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11089 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/deferring.rst
--rw-r--r--   0 runner    (1001) docker     (121)    47034 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/defining.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.780028 traits-6.4.1/docs/source/traits_user_manual/images/
--rw-r--r--   0 runner    (1001) docker     (121)    33452 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/images/adaptation.png
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13734 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/internals.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7265 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34475 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/listening.rst
--rw-r--r--   0 runner    (1001) docker     (121)    22455 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/notification.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5081 2022-08-12 11:16:17.000000 traits-6.4.1/docs/source/traits_user_manual/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.780028 traits-6.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-08-12 11:16:17.000000 traits-6.4.1/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.780028 traits-6.4.1/examples/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/default.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.784029 traits-6.4.1/examples/tutorials/doc_examples/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/default.css
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/doc_examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.788029 traits-6.4.1/examples/tutorials/doc_examples/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/adapt_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/add_class_trait.py
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/all_traits_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/all_wildcard.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/bad_self_ref.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/cached_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/circular_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/configure_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/custom_traithandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/deferring_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/delegate.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/disallow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/dynamic_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/instance_trait_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/interface_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/interface_implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/lesson.desc
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/list_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/mapped.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/minimal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/object_trait_attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/observe_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/observe_different_events.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/observe_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/observe_optional.py
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/observe_post_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/override_default.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/post_init_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/prototype_prefix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/simple_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/static_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/temp_wildcard.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/this.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/trait_reuse.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/trait_subclass.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/traitprefixmap.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/transient_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/use_custom_th.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/widget.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard_all.py
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/examples/wizard.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/doc_examples/lesson.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.788029 traits-6.4.1/examples/tutorials/introduction/
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/0_introduction.py
--rw-r--r--   0 runner    (1001) docker     (121)     6555 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/1_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6101 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/2_initialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/3_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6436 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/4_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/5_documentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/6_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/default.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/introduction/images/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/images/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  2225122 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/images/sample_0001.png
--rw-r--r--   0 runner    (1001) docker     (121)  2236536 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/images/sample_0002.png
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/introduction/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/traits_4.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/traits_4.0/decorators/
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/decorators/on_trait_change.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/decorators/tutorial.desc
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/default.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/traits_4.0/delegation/
--rw-r--r--   0 runner    (1001) docker     (121)     5246 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/delegation/delegation.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/delegation/tutorial.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/traits_4.0/extended_trait_change/
--rw-r--r--   0 runner    (1001) docker     (121)    11792 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/extended_trait_change/extended_trait_change.py
--rw-r--r--   0 runner    (1001) docker     (121)     8055 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/extended_trait_change/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/extended_trait_change/tutorial.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/traits_4.0/getstate_setstate/
--rw-r--r--   0 runner    (1001) docker     (121)     7271 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/getstate_setstate/getstate.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/getstate_setstate/tutorial.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.792029 traits-6.4.1/examples/tutorials/traits_4.0/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/interfaces/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/interfaces/tutorial.desc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.796028 traits-6.4.1/examples/tutorials/traits_4.0/trait_types/
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/trait_types/core_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     8620 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/trait_types/new_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/trait_types/trait_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/trait_types/tutorial.desc
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/traits_4.0/tutorial.desc
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-08-12 11:16:17.000000 traits-6.4.1/examples/tutorials/tutor.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-08-12 11:16:17.000000 traits-6.4.1/image_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-08-12 11:16:17.000000 traits-6.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-12 11:16:25.828029 traits-6.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    10596 2022-08-12 11:16:17.000000 traits-6.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.796028 traits-6.4.1/traits/
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-08-12 11:16:17.000000 traits-6.4.1/traits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits/adaptation/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/adaptation_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    15471 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/adaptation_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/adaptation_offer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits/adaptation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/abc_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     4350 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     3622 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/interface_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/lazy_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)    16189 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/test_adaptation_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/test_adaptation_offer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4251 2022-08-12 11:16:17.000000 traits-6.4.1/traits/adaptation/tests/test_global_adaptation_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-08-12 11:16:17.000000 traits-6.4.1/traits/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6369 2022-08-12 11:16:17.000000 traits-6.4.1/traits/base_trait_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     6601 2022-08-12 11:16:17.000000 traits-6.4.1/traits/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8422 2022-08-12 11:16:17.000000 traits-6.4.1/traits/ctrait.py
--rw-r--r--   0 runner    (1001) docker     (121)   186232 2022-08-12 11:16:17.000000 traits-6.4.1/traits/ctraits.c
--rw-r--r--   0 runner    (1001) docker     (121)     5808 2022-08-12 11:16:17.000000 traits-6.4.1/traits/editor_factories.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits/etsconfig/
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-08-12 11:16:17.000000 traits-6.4.1/traits/etsconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-12 11:16:17.000000 traits-6.4.1/traits/etsconfig/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    17087 2022-08-12 11:16:17.000000 traits-6.4.1/traits/etsconfig/etsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits/etsconfig/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/etsconfig/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13919 2022-08-12 11:16:17.000000 traits-6.4.1/traits/etsconfig/tests/test_etsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/_etsdemo_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits/examples/introduction/
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/0_introduction.py
--rw-r--r--   0 runner    (1001) docker     (121)     6555 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/1_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6101 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/2_initialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/3_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6436 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/4_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/5_documentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/6_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/default.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.804029 traits-6.4.1/traits/examples/introduction/images/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/images/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  2225122 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/images/sample_0001.png
--rw-r--r--   0 runner    (1001) docker     (121)  2236536 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/images/sample_0002.png
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/introduction/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.808029 traits-6.4.1/traits/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-12 11:16:17.000000 traits-6.4.1/traits/examples/tests/test_etsdemo_info.py
--rw-r--r--   0 runner    (1001) docker     (121)   139421 2022-08-12 11:16:17.000000 traits-6.4.1/traits/has_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     5881 2022-08-12 11:16:17.000000 traits-6.4.1/traits/interface_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.808029 traits-6.4.1/traits/observation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_anytrait_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_dict_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     6804 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_dict_item_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_dsl_grammar.lark
--rw-r--r--   0 runner    (1001) docker     (121)     6333 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_filtered_trait_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)    85541 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_generated_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4166 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_has_traits_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_i_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     7484 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_i_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_list_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_list_item_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7198 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_named_trait_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5980 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_observe.py
--rw-r--r--   0 runner    (1001) docker     (121)     7106 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_observer_change_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_observer_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_set_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     6616 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_set_item_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4292 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     8303 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_trait_added_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_trait_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     8226 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/_trait_event_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    18056 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/i_observable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3074 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/observe.py
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.812029 traits-6.4.1/traits/observation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_dict_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     9329 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_dict_item_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)    24817 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (121)    11096 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_filtered_trait_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_generated_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     9363 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_has_traits_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_list_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_list_item_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    18502 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_named_trait_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17808 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_observe.py
--rw-r--r--   0 runner    (1001) docker     (121)    19447 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_observer_change_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_observer_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_set_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_set_item_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9447 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_trait_added_observer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_trait_change_event.py
--rw-r--r--   0 runner    (1001) docker     (121)    15889 2022-08-12 11:16:17.000000 traits-6.4.1/traits/observation/tests/test_trait_event_notifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.812029 traits-6.4.1/traits/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/doctest_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/nose_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/optional_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.812029 traits-6.4.1/traits/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/tests/test_nose_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/tests/test_optional_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)    14710 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/tests/test_unittest_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    17821 2022-08-12 11:16:17.000000 traits-6.4.1/traits/testing/unittest_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.824029 traits-6.4.1/traits/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17669 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/check_observe_timing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5663 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/check_timing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.776028 traits-6.4.1/traits/tests/test-data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.824029 traits-6.4.1/traits/tests/test-data/historical-pickles/
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/README
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/generate_pickles.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p0-float-ctrait.pkl
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p1-float-ctrait.pkl
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p2-float-ctrait.pkl
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p3-float-ctrait.pkl
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p4-float-ctrait.pkl
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p5-float-ctrait.pkl
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_any.py
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_anytrait_static_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     6078 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_array_or_none.py
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_automatic_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_class_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     8547 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_configure_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_container_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     9089 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_copy_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_copyable_trait_names.py
--rw-r--r--   0 runner    (1001) docker     (121)    11887 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_ctraits.py
--rw-r--r--   0 runner    (1001) docker     (121)     4950 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_cythonized_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     5318 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     8716 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_delegate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_deprecated_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_dynamic_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_dynamic_trait_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     7032 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_editor_factories.py
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_event_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     4816 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7607 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_extended_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)    34856 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_extended_trait_change.py
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5766 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_float.py
--rw-r--r--   0 runner    (1001) docker     (121)     9399 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_float_range.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_get_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_has_required_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)    27431 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_has_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_historical_unpickling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_int_range_long.py
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_integer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9396 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_integer_range.py
--rw-r--r--   0 runner    (1001) docker     (121)    11554 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_interface_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    14911 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_keyword_args.py
--rw-r--r--   0 runner    (1001) docker     (121)    10807 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     8250 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_list_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_long_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_new_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_none.py
--rw-r--r--   0 runner    (1001) docker     (121)    25872 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_observe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_pickle_validated_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_prefix_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     7884 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_prefix_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_property_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)    16114 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_property_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_python_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_range.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (121)    21325 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     8607 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_rich_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_special_event_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3917 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_static_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_str_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     5051 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_sync_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_change_event_tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6914 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_cycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_default_initializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_dict_list_set_event.py
--rw-r--r--   0 runner    (1001) docker     (121)    16701 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_dict_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_get_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     6251 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    51961 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_list_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_prefix_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    16958 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_set_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     5582 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_trait_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    34145 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)    15385 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_traits_listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_ui_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_undefined.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_unicode_traits.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_validated_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_view_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/test_weak_ref.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-08-12 11:16:17.000000 traits-6.4.1/traits/tests/tuple_test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10102 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4365 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    17835 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_dict_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    43060 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    27609 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_list_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    24970 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14876 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)    16770 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_set_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    19936 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_type.py
--rw-r--r--   0 runner    (1001) docker     (121)   160251 2022-08-12 11:16:17.000000 traits-6.4.1/traits/trait_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    26880 2022-08-12 11:16:17.000000 traits-6.4.1/traits/traits.py
--rw-r--r--   0 runner    (1001) docker     (121)    43252 2022-08-12 11:16:17.000000 traits-6.4.1/traits/traits_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.824029 traits-6.4.1/traits/util/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/_traitsui_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/async_trait_wait.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/camel_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     4069 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/clean_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)    10853 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/event_tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/home_directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/import_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.828029 traits-6.4.1/traits/util/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2626 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_async_trait_wait.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_camel_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_clean_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_import_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_message_records.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_record_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_record_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     7281 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_trait_documenter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_traitsui_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/tests/test_weakidddict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/toposort.py
--rw-r--r--   0 runner    (1001) docker     (121)     7037 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/trait_documenter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-08-12 11:16:17.000000 traits-6.4.1/traits/util/weakiddict.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-08-12 11:16:25.000000 traits-6.4.1/traits/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 11:16:25.800029 traits-6.4.1/traits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17055 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-12 11:16:25.000000 traits-6.4.1/traits.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.062248 traits-6.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    74950 2023-08-07 10:47:36.000000 traits-6.4.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-08-07 10:47:36.000000 traits-6.4.2/LICENSE-CC-BY-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-07 10:47:36.000000 traits-6.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-07 10:47:36.000000 traits-6.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-07 10:47:53.062248 traits-6.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-07 10:47:36.000000 traits-6.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.954246 traits-6.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-07 10:47:36.000000 traits-6.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-08-07 10:47:36.000000 traits-6.4.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.954246 traits-6.4.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.954246 traits-6.4.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/_static/e-logo-rev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/_static/et.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.954246 traits-6.4.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/_templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.962246 traits-6.4.2/docs/source/traits_api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/base_trait_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/ctrait.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/ctraits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/editor_factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/has_traits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/interface_checker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_converters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_dict_object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_list_object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_notifiers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_numeric.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_set_object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/trait_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits.adaptation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits.etsconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits.observation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits.testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits.util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/traits_listener.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_api_reference/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.962246 traits-6.4.2/docs/source/traits_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_tutorial/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.966246 traits-6.4.2/docs/source/traits_user_manual/
+-rw-r--r--   0 runner    (1001) docker     (123)    58499 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/appendix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/deferring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47034 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/defining.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.966246 traits-6.4.2/docs/source/traits_user_manual/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/images/adaptation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/listening.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22455 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/notification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-08-07 10:47:36.000000 traits-6.4.2/docs/source/traits_user_manual/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.966246 traits-6.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 10:47:36.000000 traits-6.4.2/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.966246 traits-6.4.2/examples/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/default.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.966246 traits-6.4.2/examples/tutorials/doc_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/doc_examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.978247 traits-6.4.2/examples/tutorials/doc_examples/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/adapt_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/add_class_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/all_traits_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/all_wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/bad_self_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/cached_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/circular_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/configure_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/custom_traithandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/deferring_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/disallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/dynamic_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/instance_trait_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/interface_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/interface_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/lesson.desc
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/list_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/minimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/object_trait_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/observe_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/observe_different_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/observe_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/observe_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/observe_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/override_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/post_init_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/prototype_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/simple_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/static_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/temp_wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/this.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/trait_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/trait_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/traitprefixmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/transient_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/use_custom_th.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/examples/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/doc_examples/lesson.desc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.982247 traits-6.4.2/examples/tutorials/introduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/0_introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/1_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/2_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/3_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/4_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/5_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/6_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/default.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.986247 traits-6.4.2/examples/tutorials/introduction/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/introduction/images/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2225122 2023-08-07 10:47:37.000000 traits-6.4.2/examples/tutorials/introduction/images/sample_0001.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2236536 2023-08-07 10:47:37.000000 traits-6.4.2/examples/tutorials/introduction/images/sample_0002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-07 10:47:37.000000 traits-6.4.2/examples/tutorials/introduction/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.990247 traits-6.4.2/examples/tutorials/traits_4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.990247 traits-6.4.2/examples/tutorials/traits_4.0/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/decorators/on_trait_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/decorators/tutorial.desc
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/default.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.990247 traits-6.4.2/examples/tutorials/traits_4.0/delegation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/delegation/delegation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/delegation/tutorial.desc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.990247 traits-6.4.2/examples/tutorials/traits_4.0/extended_trait_change/
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/extended_trait_change/extended_trait_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/extended_trait_change/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/extended_trait_change/tutorial.desc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.990247 traits-6.4.2/examples/tutorials/traits_4.0/getstate_setstate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/getstate_setstate/getstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/getstate_setstate/tutorial.desc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.990247 traits-6.4.2/examples/tutorials/traits_4.0/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/interfaces/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/interfaces/tutorial.desc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.994247 traits-6.4.2/examples/tutorials/traits_4.0/trait_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/trait_types/core_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/trait_types/new_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/trait_types/trait_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/trait_types/tutorial.desc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/traits_4.0/tutorial.desc
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-07 10:47:36.000000 traits-6.4.2/examples/tutorials/tutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-07 10:47:36.000000 traits-6.4.2/image_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 10:47:36.000000 traits-6.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-07 10:47:53.062248 traits-6.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-08-07 10:47:36.000000 traits-6.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.998247 traits-6.4.2/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-07 10:47:36.000000 traits-6.4.2/traits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.002247 traits-6.4.2/traits/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/adaptation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/adaptation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/adaptation_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.006247 traits-6.4.2/traits/adaptation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/abc_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/interface_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/lazy_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/test_adaptation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/test_adaptation_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-08-07 10:47:36.000000 traits-6.4.2/traits/adaptation/tests/test_global_adaptation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-08-07 10:47:36.000000 traits-6.4.2/traits/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-07 10:47:36.000000 traits-6.4.2/traits/base_trait_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-07 10:47:36.000000 traits-6.4.2/traits/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-07 10:47:36.000000 traits-6.4.2/traits/ctrait.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186232 2023-08-07 10:47:36.000000 traits-6.4.2/traits/ctraits.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-07 10:47:36.000000 traits-6.4.2/traits/editor_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.006247 traits-6.4.2/traits/etsconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-07 10:47:36.000000 traits-6.4.2/traits/etsconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 10:47:36.000000 traits-6.4.2/traits/etsconfig/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-08-07 10:47:36.000000 traits-6.4.2/traits/etsconfig/etsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.006247 traits-6.4.2/traits/etsconfig/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:36.000000 traits-6.4.2/traits/etsconfig/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-08-07 10:47:36.000000 traits-6.4.2/traits/etsconfig/tests/test_etsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.006247 traits-6.4.2/traits/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/_etsdemo_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.010247 traits-6.4.2/traits/examples/introduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/0_introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/1_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/2_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/3_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/4_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/5_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/6_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/default.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.010247 traits-6.4.2/traits/examples/introduction/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 10:47:36.000000 traits-6.4.2/traits/examples/introduction/images/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2225122 2023-08-07 10:47:37.000000 traits-6.4.2/traits/examples/introduction/images/sample_0001.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2236536 2023-08-07 10:47:37.000000 traits-6.4.2/traits/examples/introduction/images/sample_0002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-07 10:47:37.000000 traits-6.4.2/traits/examples/introduction/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.014247 traits-6.4.2/traits/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:37.000000 traits-6.4.2/traits/examples/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-07 10:47:37.000000 traits-6.4.2/traits/examples/tests/test_etsdemo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139222 2023-08-07 10:47:37.000000 traits-6.4.2/traits/has_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-08-07 10:47:37.000000 traits-6.4.2/traits/interface_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.022247 traits-6.4.2/traits/observation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_anytrait_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_dict_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_dict_item_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_dsl_grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_filtered_trait_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85541 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_generated_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_has_traits_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_i_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_i_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_list_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_list_item_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_named_trait_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_observe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_observer_change_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_observer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_set_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_set_item_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_trait_added_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_trait_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/_trait_event_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/i_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/observe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.026247 traits-6.4.2/traits/observation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_dict_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_dict_item_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_filtered_trait_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_generated_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_has_traits_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_list_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_list_item_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18502 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_named_trait_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_observe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19447 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_observer_change_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_observer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_set_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_set_item_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_trait_added_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_trait_change_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-08-07 10:47:37.000000 traits-6.4.2/traits/observation/tests/test_trait_event_notifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.030247 traits-6.4.2/traits/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/doctest_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/nose_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/optional_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.030247 traits-6.4.2/traits/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/tests/test_nose_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/tests/test_optional_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/tests/test_unittest_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-08-07 10:47:37.000000 traits-6.4.2/traits/testing/unittest_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.054248 traits-6.4.2/traits/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/check_observe_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/check_timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:52.950246 traits-6.4.2/traits/tests/test-data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.054248 traits-6.4.2/traits/tests/test-data/historical-pickles/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/generate_pickles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p0-float-ctrait.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p1-float-ctrait.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p2-float-ctrait.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p3-float-ctrait.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p4-float-ctrait.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test-data/historical-pickles/hipt-t5.2.0-p5-float-ctrait.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_anytrait_static_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_array_or_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_automatic_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_class_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_configure_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_container_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_copy_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_copyable_trait_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_ctraits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_cythonized_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_deprecated_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_dynamic_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_dynamic_trait_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_editor_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_event_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_extended_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34856 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_extended_trait_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_float_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_get_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_has_required_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_has_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_historical_unpickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_int_range_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_integer_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_interface_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_keyword_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_list_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_long_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_new_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_observe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_pickle_validated_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_prefix_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_prefix_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_property_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_property_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_python_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_rich_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_special_event_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_static_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_str_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_sync_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_change_event_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_default_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_dict_list_set_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_dict_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_get_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51961 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_prefix_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_set_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_trait_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34145 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_traits_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_ui_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_unicode_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_validated_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_view_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/test_weak_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-07 10:47:37.000000 traits-6.4.2/traits/tests/tuple_test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_dict_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43060 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27609 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24970 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_set_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160251 2023-08-07 10:47:37.000000 traits-6.4.2/traits/trait_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-08-07 10:47:37.000000 traits-6.4.2/traits/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43252 2023-08-07 10:47:37.000000 traits-6.4.2/traits/traits_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.058248 traits-6.4.2/traits/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/async_trait_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/camel_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/clean_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/event_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/home_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/import_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.062248 traits-6.4.2/traits/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_async_trait_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_camel_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_clean_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_import_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_message_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_record_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_record_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_trait_documenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/tests/test_weakidddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/toposort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/trait_documenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-07 10:47:37.000000 traits-6.4.2/traits/util/weakiddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-07 10:47:52.000000 traits-6.4.2/traits/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:47:53.002247 traits-6.4.2/traits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16979 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 10:47:52.000000 traits-6.4.2/traits.egg-info/top_level.txt
```

### Comparing `traits-6.4.1/CHANGES.rst` & `traits-6.4.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,4664 +1,4685 @@
 00000000: 5472 6169 7473 2043 4841 4e47 454c 4f47  Traits CHANGELOG
 00000010: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
-00000020: 3d0a 0a52 656c 6561 7365 2036 2e34 2e31  =..Release 6.4.1
+00000020: 3d0a 0a52 656c 6561 7365 2036 2e34 2e32  =..Release 6.4.2
 00000030: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
-00000040: 5265 6c65 6173 6564 3a20 3230 3232 2d30  Released: 2022-0
-00000050: 382d 3132 0a0a 5468 6973 2069 7320 6120  8-12..This is a 
+00000040: 5265 6c65 6173 6564 3a20 3230 3233 2d30  Released: 2023-0
+00000050: 382d 3037 0a0a 5468 6973 2069 7320 6120  8-07..This is a 
 00000060: 6275 6766 6978 2072 656c 6561 7365 2074  bugfix release t
-00000070: 6861 7420 6669 7865 7320 7768 6565 6c20  hat fixes wheel 
-00000080: 6275 696c 6473 206f 6e20 5079 7468 6f6e  builds on Python
-00000090: 2033 2e31 3120 616e 640a 6669 7865 7320   3.11 and.fixes 
-000000a0: 736f 6d65 2064 6973 7472 6962 7574 696f  some distributio
-000000b0: 6e20 616e 6420 7465 7374 696e 6720 6973  n and testing is
-000000c0: 7375 6573 2077 6974 6820 7479 7069 6e67  sues with typing
-000000d0: 2073 7475 6273 2e0a 0a46 6978 6573 0a7e   stubs...Fixes.~
-000000e0: 7e7e 7e7e 0a2a 2055 7064 6174 6520 6060  ~~~~.* Update ``
-000000f0: 6369 6275 696c 6477 6865 656c 6060 2074  cibuildwheel`` t
-00000100: 6f20 7468 6520 6c61 7465 7374 2076 6572  o the latest ver
-00000110: 7369 6f6e 2073 6f20 7468 6174 2077 6520  sion so that we 
-00000120: 6765 7420 7768 6565 6c73 2066 6f72 0a20  get wheels for. 
-00000130: 2050 7974 686f 6e20 332e 3131 2e20 2823   Python 3.11. (#
-00000140: 3137 3131 290a 2a20 5265 6e61 6d65 2060  1711).* Rename `
-00000150: 6072 6571 7569 7265 735f 6e75 6d70 795f  `requires_numpy_
-00000160: 7465 7374 696e 6760 6020 6465 636f 7261  testing`` decora
-00000170: 746f 7220 746f 2060 6072 6571 7569 7265  tor to ``require
-00000180: 735f 6e75 6d70 795f 7479 7069 6e67 6060  s_numpy_typing``
-00000190: 2c0a 2020 616e 6420 6861 7665 2069 7420  ,.  and have it 
-000001a0: 6368 6563 6b20 666f 7220 6060 6e75 6d70  check for ``nump
-000001b0: 792e 7479 7069 6e67 6060 2c20 6e6f 7420  y.typing``, not 
-000001c0: 6060 6e75 6d70 792e 7465 7374 696e 6760  ``numpy.testing`
-000001d0: 602e 2028 2331 3731 3029 0a2a 2046 6978  `. (#1710).* Fix
-000001e0: 206d 6973 7369 6e67 2060 606e 756d 7079   missing ``numpy
-000001f0: 5f65 7861 6d70 6c65 7360 6020 6469 7265  _examples`` dire
-00000200: 6374 6f72 7920 696e 2074 7261 6974 732d  ctory in traits-
-00000210: 7374 7562 7320 7061 636b 6167 6520 6461  stubs package da
-00000220: 7461 2e0a 2020 2823 3137 3039 290a 0a0a  ta..  (#1709)...
-00000230: 5265 6c65 6173 6520 362e 342e 300a 2d2d  Release 6.4.0.--
-00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 656c  -----------..Rel
-00000250: 6561 7365 643a 2032 3032 322d 3038 2d31  eased: 2022-08-1
-00000260: 320a 0a54 7261 6974 7320 362e 3420 6973  2..Traits 6.4 is
-00000270: 2061 206d 696e 6f72 2066 6561 7475 7265   a minor feature
-00000280: 2072 656c 6561 7365 206f 6620 5472 6169   release of Trai
-00000290: 7473 2c20 7768 6963 6820 666f 6375 7365  ts, which focuse
-000002a0: 7320 6d61 696e 6c79 206f 6e20 7479 7069  s mainly on typi
-000002b0: 6e67 0a73 7475 6220 616e 6420 646f 6375  ng.stub and docu
-000002c0: 6d65 6e74 6174 696f 6e20 7570 6461 7465  mentation update
-000002d0: 732e 0a0a 4d69 6772 6174 696e 6720 6672  s...Migrating fr
-000002e0: 6f6d 2054 7261 6974 7320 362e 330a 7e7e  om Traits 6.3.~~
-000002f0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00000300: 7e7e 7e7e 7e7e 7e0a 0a54 7261 6974 7320  ~~~~~~~..Traits 
-00000310: 362e 3420 7368 6f75 6c64 2062 6520 6c61  6.4 should be la
-00000320: 7267 656c 7920 6261 636b 7761 7264 7320  rgely backwards 
-00000330: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
-00000340: 5472 6169 7473 2036 2e33 2c20 6275 7420  Traits 6.3, but 
-00000350: 7468 6572 650a 6172 6520 6120 636f 7570  there.are a coup
-00000360: 6c65 206f 6620 7468 696e 6773 2074 6f20  le of things to 
-00000370: 7761 7463 6820 6f75 7420 666f 722e 0a0a  watch out for...
-00000380: 2a20 5265 6d69 6e64 6572 3a20 7768 696c  * Reminder: whil
-00000390: 6520 7468 6520 6060 4569 7468 6572 6060  e the ``Either``
-000003a0: 2061 6e64 2060 6054 7261 6974 6060 2074   and ``Trait`` t
-000003b0: 7261 6974 2074 7970 6573 2061 7265 206e  rait types are n
-000003c0: 6f74 2079 6574 2066 6f72 6d61 6c6c 790a  ot yet formally.
-000003d0: 2020 6465 7072 6563 6174 6564 2c20 7468    deprecated, th
-000003e0: 6520 696e 7465 6e74 696f 6e20 6973 2074  e intention is t
-000003f0: 6f20 6576 656e 7475 616c 6c79 2064 6570  o eventually dep
-00000400: 7265 6361 7465 2061 6e64 2072 656d 6f76  recate and remov
-00000410: 6520 7468 656d 2e0a 2020 5072 6f6a 6563  e them..  Projec
-00000420: 7473 2061 7265 2065 6e63 6f75 7261 6765  ts are encourage
-00000430: 6420 746f 2075 7064 6174 6520 7468 6569  d to update thei
-00000440: 7220 636f 6465 2074 6f20 7573 6520 6060  r code to use ``
-00000450: 556e 696f 6e60 6020 696e 7374 6561 642e  Union`` instead.
-00000460: 0a2a 2053 696d 696c 6172 6c79 2c20 616e  .* Similarly, an
-00000470: 7920 7573 6573 206f 6620 7468 6520 6060  y uses of the ``
-00000480: 556e 6963 6f64 6560 6020 7472 6169 7420  Unicode`` trait 
-00000490: 7479 7065 2069 6e20 796f 7572 2070 726f  type in your pro
-000004a0: 6a65 6374 2073 686f 756c 640a 2020 6265  ject should.  be
-000004b0: 2072 6570 6c61 6365 6420 7769 7468 2060   replaced with `
-000004c0: 6053 7472 6060 2e0a 2a20 5661 6c69 6461  `Str``..* Valida
-000004d0: 7469 6f6e 206f 6620 6974 656d 7320 7769  tion of items wi
-000004e0: 7468 696e 2061 2063 6f6e 7461 696e 6572  thin a container
-000004f0: 2028 652e 672e 2c20 6060 666f 6f73 203d   (e.g., ``foos =
-00000500: 204c 6973 7428 4d79 5472 6169 7454 7970   List(MyTraitTyp
-00000510: 6529 6060 290a 2020 6e6f 7720 616c 7761  e)``).  now alwa
-00000520: 7973 206d 6174 6368 6573 2074 6865 2076  ys matches the v
-00000530: 616c 6964 6174 696f 6e20 7573 6564 2066  alidation used f
-00000540: 6f72 2074 6865 2069 7465 6d20 7472 6169  or the item trai
-00000550: 7420 6174 2074 6f70 206c 6576 656c 2028  t at top level (
-00000560: 652e 672e 2c0a 2020 6060 666f 6f20 3d20  e.g.,.  ``foo = 
-00000570: 4d79 5472 6169 7454 7970 6560 6029 2e20  MyTraitType``). 
-00000580: 5072 6576 696f 7573 6c79 2c20 7468 6520  Previously, the 
-00000590: 7661 6c69 6461 7469 6f6e 206d 6574 686f  validation metho
-000005a0: 6473 2075 7365 6420 636f 756c 6420 6469  ds used could di
-000005b0: 6666 6572 2c0a 2020 7468 616e 6b73 2074  ffer,.  thanks t
-000005c0: 6f20 6120 6275 6720 696e 2074 6865 2063  o a bug in the c
-000005d0: 6f6e 7461 696e 6572 2069 6d70 6c65 6d65  ontainer impleme
-000005e0: 6e74 6174 696f 6e73 2e20 466f 7220 6d6f  ntations. For mo
-000005f0: 7374 2074 7261 6974 2074 7970 6573 2074  st trait types t
-00000600: 6869 730a 2020 7769 6c6c 206d 616b 6520  his.  will make 
-00000610: 6e6f 2064 6966 6665 7265 6e63 652c 2062  no difference, b
-00000620: 7574 2066 6f72 2074 6865 2060 6054 7570  ut for the ``Tup
-00000630: 6c65 6060 2074 7261 6974 2074 7970 6520  le`` trait type 
-00000640: 7468 6973 2063 6861 6e67 6520 6861 7320  this change has 
-00000650: 7468 650a 2020 636f 6e73 6571 7565 6e63  the.  consequenc
-00000660: 6520 7468 6174 206c 6973 7473 2077 696c  e that lists wil
-00000670: 6c20 6e6f 206c 6f6e 6765 7220 6265 2061  l no longer be a
-00000680: 6363 6570 7465 6420 6173 2076 616c 6964  ccepted as valid
-00000690: 2066 6f72 2060 6054 7570 6c65 6060 0a20   for ``Tuple``. 
-000006a0: 2074 7261 6974 7320 696e 7369 6465 206c   traits inside l
-000006b0: 6973 7420 6974 656d 732e 2053 6565 2069  ist items. See i
-000006c0: 7373 7565 2023 3136 3139 2061 6e64 2050  ssue #1619 and P
-000006d0: 5220 2331 3632 3520 666f 7220 6d6f 7265  R #1625 for more
-000006e0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2a20   information..* 
-000006f0: 5265 6c61 7465 6420 746f 2074 6865 2061  Related to the a
-00000700: 626f 7665 3a20 6120 746f 702d 6c65 7665  bove: a top-leve
-00000710: 6c20 6060 5475 706c 6528 2960 6020 7472  l ``Tuple()`` tr
-00000720: 6169 7420 6465 636c 6172 6174 696f 6e20  ait declaration 
-00000730: 6375 7272 656e 746c 790a 2020 6163 6365  currently.  acce
-00000740: 7074 7320 5079 7468 6f6e 2060 606c 6973  pts Python ``lis
-00000750: 7460 6020 6f62 6a65 6374 732c 2077 6869  t`` objects, whi
-00000760: 6c65 2061 2060 6054 7570 6c65 6060 2064  le a ``Tuple`` d
-00000770: 6563 6c61 7261 7469 6f6e 2077 6974 6820  eclaration with 
-00000780: 6578 706c 6963 6974 0a20 2069 7465 6d20  explicit.  item 
-00000790: 7479 7065 7320 2866 6f72 2065 7861 6d70  types (for examp
-000007a0: 6c65 2060 6054 7570 6c65 2849 6e74 2829  le ``Tuple(Int()
-000007b0: 2c20 496e 7428 2929 6060 2920 646f 6573  , Int())``) does
-000007c0: 206e 6f74 2e20 5468 6520 7375 7070 6f72   not. The suppor
-000007d0: 7420 666f 720a 2020 6060 6c69 7374 6060  t for.  ``list``
-000007e0: 206f 626a 6563 7473 2069 6e20 706c 6169   objects in plai
-000007f0: 6e20 6060 5475 706c 6528 2960 6020 6973  n ``Tuple()`` is
-00000800: 2064 6570 7265 6361 7465 642c 2061 6e64   deprecated, and
-00000810: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
-00000820: 2069 6e20 610a 2020 6675 7475 7265 2076   in a.  future v
-00000830: 6572 7369 6f6e 206f 6620 5472 6169 7473  ersion of Traits
-00000840: 2e20 5365 6520 5052 2023 3136 3237 2066  . See PR #1627 f
-00000850: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00000860: 696f 6e2e 0a0a 4465 7461 696c 6564 2050  ion...Detailed P
-00000870: 522d 6279 2d50 5220 6368 616e 6765 730a  R-by-PR changes.
-00000880: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00000890: 7e7e 7e7e 7e7e 7e7e 7e0a 0a54 6865 2066  ~~~~~~~~~..The f
-000008a0: 6f6c 6c6f 7769 6e67 2070 656f 706c 6520  ollowing people 
-000008b0: 636f 6e74 7269 6275 7465 6420 636f 6465  contributed code
-000008c0: 2063 6861 6e67 6573 2066 6f72 2074 6869   changes for thi
-000008d0: 7320 7265 6c65 6173 653a 0a0a 2a20 4361  s release:..* Ca
-000008e0: 696f 2041 6769 616e 690a 2a20 5374 6576  io Agiani.* Stev
-000008f0: 6520 416c 6c65 6e0a 2a20 4d61 726b 2044  e Allen.* Mark D
-00000900: 6963 6b69 6e73 6f6e 0a2a 2053 6169 2052  ickinson.* Sai R
-00000910: 6168 756c 2050 6f72 7572 690a 2a20 436f  ahul Poruri.* Co
-00000920: 7272 616e 2057 6562 7374 6572 0a0a 4665  rran Webster..Fe
-00000930: 6174 7572 6573 0a7e 7e7e 7e7e 7e7e 7e0a  atures.~~~~~~~~.
-00000940: 2a20 6060 4554 5343 6f6e 6669 6760 6020  * ``ETSConfig`` 
-00000950: 6174 7472 6962 7574 6573 206e 6f77 2073  attributes now s
-00000960: 7570 706f 7274 2064 656c 6574 696f 6e2e  upport deletion.
-00000970: 2054 6869 7320 6d61 6b65 7320 6974 2065   This makes it e
-00000980: 6173 6965 7220 746f 206d 616b 650a 2020  asier to make.  
-00000990: 7465 6d70 6f72 6172 7920 6368 616e 6765  temporary change
-000009a0: 7320 746f 2060 6045 5453 436f 6e66 6967  s to ``ETSConfig
-000009b0: 6060 2061 7474 7269 6275 7465 7320 6475  `` attributes du
-000009c0: 7269 6e67 2075 6e69 7420 7465 7374 696e  ring unit testin
-000009d0: 672e 2028 2331 3637 302c 0a20 2023 3136  g. (#1670,.  #16
-000009e0: 3836 290a 2a20 6060 436f 6d70 6c65 7860  86).* ``Complex`
-000009f0: 6020 7472 6169 7420 7479 7065 2076 616c  ` trait type val
-00000a00: 6964 6174 696f 6e20 6973 206e 6f77 206d  idation is now m
-00000a10: 6f72 6520 6c65 6e69 656e 743a 2061 6e79  ore lenient: any
-00000a20: 2074 7970 6520 7468 6174 0a20 2069 6d70   type that.  imp
-00000a30: 6c65 6d65 6e74 7320 6060 5f5f 636f 6d70  lements ``__comp
-00000a40: 6c65 785f 5f60 6020 7769 6c6c 2062 6520  lex__`` will be 
-00000a50: 6163 6365 7074 6564 2e20 2823 3135 3934  accepted. (#1594
-00000a60: 290a 2a20 6060 4261 7365 466c 6f61 7460  ).* ``BaseFloat`
-00000a70: 6020 7661 6c69 6461 7469 6f6e 2069 7320  ` validation is 
-00000a80: 6e6f 7720 6d6f 7265 206c 656e 6965 6e74  now more lenient
-00000a90: 2c20 616e 6420 6d61 7463 6865 7320 6060  , and matches ``
-00000aa0: 466c 6f61 7460 600a 2020 7661 6c69 6461  Float``.  valida
-00000ab0: 7469 6f6e 3a20 6060 4261 7365 466c 6f61  tion: ``BaseFloa
-00000ac0: 7460 6020 6e6f 7720 616c 736f 2061 6363  t`` now also acc
-00000ad0: 6570 7473 206f 626a 6563 7473 2077 686f  epts objects who
-00000ae0: 7365 2074 7970 6520 6861 7320 616e 0a20  se type has an. 
-00000af0: 2060 605f 5f69 6e64 6578 5f5f 6060 206d   ``__index__`` m
-00000b00: 6574 686f 642e 2028 2331 3539 3529 0a0a  ethod. (#1595)..
-00000b10: 4368 616e 6765 730a 7e7e 7e7e 7e7e 7e0a  Changes.~~~~~~~.
-00000b20: 2a20 416e 2060 6065 6e75 6d65 7261 7465  * An ``enumerate
-00000b30: 6060 2061 6c69 6173 2068 6173 2062 6565  `` alias has bee
-00000b40: 6e20 7265 6d6f 7665 6420 6672 6f6d 2060  n removed from `
-00000b50: 6074 7261 6974 732e 7472 6169 745f 6261  `traits.trait_ba
-00000b60: 7365 6060 2e20 496e 2074 6865 0a20 2075  se``. In the.  u
-00000b70: 6e6c 696b 656c 7920 6576 656e 7420 6f66  nlikely event of
-00000b80: 2063 6f64 6520 7468 6174 2069 6d70 6f72   code that impor
-00000b90: 7473 2060 6065 6e75 6d65 7261 7465 6060  ts ``enumerate``
-00000ba0: 2066 726f 6d20 6060 7472 6169 7473 2e74   from ``traits.t
-00000bb0: 7261 6974 5f62 6173 6560 602c 0a20 2075  rait_base``,.  u
-00000bc0: 7365 2074 6865 2062 7569 6c74 2d69 6e20  se the built-in 
-00000bd0: 6060 656e 756d 6572 6174 6560 6020 696e  ``enumerate`` in
-00000be0: 7374 6561 642e 2028 2331 3638 3129 0a2a  stead. (#1681).*
-00000bf0: 2046 6173 7420 7661 6c69 6461 7469 6f6e   Fast validation
-00000c00: 2074 7570 6c65 7320 6060 696e 745f 6661   tuples ``int_fa
-00000c10: 7374 5f76 616c 6964 6174 6560 602c 2060  st_validate``, `
-00000c20: 6066 6c6f 6174 5f66 6173 745f 7661 6c69  `float_fast_vali
-00000c30: 6461 7465 6060 2061 6e64 0a20 2060 6063  date`` and.  ``c
-00000c40: 6f6d 706c 6578 5f66 6173 745f 7661 6c69  omplex_fast_vali
-00000c50: 6461 7465 6060 2068 6176 6520 6265 656e  date`` have been
-00000c60: 2072 656d 6f76 6564 2066 726f 6d20 7468   removed from th
-00000c70: 6520 6060 7472 6169 7473 2e74 7261 6974  e ``traits.trait
-00000c80: 5f74 7970 6573 6060 0a20 206d 6f64 756c  _types``.  modul
-00000c90: 652e 2028 2331 3630 3129 0a0a 4669 7865  e. (#1601)..Fixe
-00000ca0: 730a 7e7e 7e7e 7e0a 2a20 6060 5472 6169  s.~~~~~.* ``Trai
-00000cb0: 744c 6973 744f 626a 6563 7460 602c 2060  tListObject``, `
-00000cc0: 6054 7261 6974 4469 6374 6060 206f 626a  `TraitDict`` obj
-00000cd0: 6563 7420 616e 6420 6060 5472 6169 7453  ect and ``TraitS
-00000ce0: 6574 4f62 6a65 6374 6060 206e 6f77 2075  etObject`` now u
-00000cf0: 7365 2074 6865 0a20 2060 6076 616c 6964  se the.  ``valid
-00000d00: 6174 6560 6020 6d65 7468 6f64 206f 6620  ate`` method of 
-00000d10: 7468 6520 6170 7072 6f70 7269 6174 6520  the appropriate 
-00000d20: 6060 4354 7261 6974 6060 2069 6e73 7461  ``CTrait`` insta
-00000d30: 6e63 6573 2074 6f20 7661 6c69 6461 7465  nces to validate
-00000d40: 0a20 2069 7465 6d73 2c20 6b65 7973 2061  .  items, keys a
-00000d50: 6e64 2076 616c 7565 732e 2050 7265 7669  nd values. Previ
-00000d60: 6f75 736c 7920 7468 6520 6861 6e64 6c65  ously the handle
-00000d70: 7227 7320 6060 7661 6c69 6461 7465 6060  r's ``validate``
-00000d80: 206d 6574 686f 6420 7761 730a 2020 7573   method was.  us
-00000d90: 6564 3b20 7468 6973 2067 6176 6520 6275  ed; this gave bu
-00000da0: 6767 7920 6265 6861 7669 6f75 7220 696e  ggy behaviour in
-00000db0: 2063 6173 6573 2077 6865 7265 2074 6865   cases where the
-00000dc0: 2068 616e 646c 6572 2773 2060 6076 616c   handler's ``val
-00000dd0: 6964 6174 6560 600a 2020 6d65 7468 6f64  idate``.  method
-00000de0: 2064 6966 6665 7265 6420 6672 6f6d 2074   differed from t
-00000df0: 6865 2061 6374 7561 6c20 7661 6c69 6461  he actual valida
-00000e00: 7469 6f6e 2069 6e20 7573 652e 2028 2331  tion in use. (#1
-00000e10: 3632 3529 0a2a 2046 6978 2073 7065 6369  625).* Fix speci
-00000e20: 6669 6361 7469 6f6e 206f 6620 6060 6465  fication of ``de
-00000e30: 6661 756c 745f 7661 6c75 6560 6020 7468  fault_value`` th
-00000e40: 6174 2069 6e63 6f72 7265 6374 6c79 2064  at incorrectly d
-00000e50: 6973 7265 6761 7264 6564 0a20 2060 6064  isregarded.  ``d
-00000e60: 6566 6175 6c74 5f76 616c 7565 5f74 7970  efault_value_typ
-00000e70: 6560 602e 2028 2331 3633 3129 0a2a 2046  e``. (#1631).* F
-00000e80: 6978 2069 6e63 6f72 7265 6374 2072 6573  ix incorrect res
-00000e90: 756c 7473 2066 726f 6d20 2060 6063 6c6f  ults from  ``clo
-00000ea0: 6e65 5f74 7261 6974 7360 6020 6170 706c  ne_traits`` appl
-00000eb0: 6965 6420 746f 2060 604c 6973 7460 602c  ied to ``List``,
-00000ec0: 2060 6044 6963 7460 600a 2020 616e 6420   ``Dict``.  and 
-00000ed0: 6060 5365 7460 6020 7472 6169 7473 2e20  ``Set`` traits. 
-00000ee0: 2823 3136 3234 290a 2a20 5468 6520 6060  (#1624).* The ``
-00000ef0: 6669 6e64 5f72 6573 6f75 7263 6560 6020  find_resource`` 
-00000f00: 616e 6420 6060 7374 6f72 655f 7265 736f  and ``store_reso
-00000f10: 7572 6365 6060 2074 6573 7473 2061 7265  urce`` tests are
-00000f20: 206e 6f77 2073 6b69 7070 6564 0a20 2069   now skipped.  i
-00000f30: 6620 7468 6520 6060 706b 675f 7265 736f  f the ``pkg_reso
-00000f40: 7572 6365 7360 6020 6d6f 6475 6c65 2069  urces`` module i
-00000f50: 7320 6e6f 7420 7072 6573 656e 7420 696e  s not present in
-00000f60: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
-00000f70: 2e20 2823 3136 3739 290a 2a20 416e 2060  . (#1679).* An `
-00000f80: 6045 5453 436f 6e66 6967 6060 2074 6573  `ETSConfig`` tes
-00000f90: 7420 6861 7320 6265 656e 2072 656e 616d  t has been renam
-00000fa0: 6564 2073 6f20 7468 6174 2069 7427 7320  ed so that it's 
-00000fb0: 7072 6f70 6572 6c79 2070 6963 6b65 6420  properly picked 
-00000fc0: 7570 0a20 2062 7920 7468 6520 7465 7374  up.  by the test
-00000fd0: 2072 756e 6e65 722e 2028 2331 3637 3129   runner. (#1671)
-00000fe0: 0a2a 2046 6978 2073 6f6d 6520 6060 4554  .* Fix some ``ET
-00000ff0: 5343 6f6e 6669 6760 6020 7465 7374 7320  SConfig`` tests 
-00001000: 7468 6174 2061 7373 756d 6520 756e 6974  that assume unit
-00001010: 7465 7374 2061 7320 7468 6520 7465 7374  test as the test
-00001020: 2072 756e 6e65 722e 2028 2331 3638 3329   runner. (#1683)
-00001030: 0a2a 2052 656e 616d 6520 7661 7269 6f75  .* Rename variou
-00001040: 7320 7465 7374 2d72 656c 6174 6564 2063  s test-related c
-00001050: 6c61 7373 6573 2074 6f20 6176 6f69 6420  lasses to avoid 
-00001060: 7079 7465 7374 2074 7279 696e 6720 746f  pytest trying to
-00001070: 2068 6172 7665 7374 2074 6573 740a 2020   harvest test.  
-00001080: 6d65 7468 6f64 7320 6672 6f6d 2074 6865  methods from the
-00001090: 6d2e 2028 2331 3638 3429 0a2a 204f 7665  m. (#1684).* Ove
-000010a0: 7272 6964 696e 6720 6120 6465 6661 756c  rriding a defaul
-000010b0: 7420 666f 7220 6120 6060 4c69 7374 6060  t for a ``List``
-000010c0: 206f 7220 6f74 6865 7220 636f 6c6c 6563   or other collec
-000010d0: 7469 6f6e 2074 7261 6974 2069 6e20 6120  tion trait in a 
-000010e0: 7375 6263 6c61 7373 0a20 206e 6f77 2077  subclass.  now w
-000010f0: 6f72 6b73 2061 7320 6578 7065 6374 6564  orks as expected
-00001100: 2e20 5072 6576 696f 7573 6c79 2c20 7468  . Previously, th
-00001110: 6520 6265 6861 7669 6f75 7220 7761 7320  e behaviour was 
-00001120: 756e 7573 6162 6c79 2062 7567 6779 2e20  unusably buggy. 
-00001130: 2823 3136 3435 290a 0a44 6570 7265 6361  (#1645)..Depreca
-00001140: 7469 6f6e 730a 7e7e 7e7e 7e7e 7e7e 7e7e  tions.~~~~~~~~~~
-00001150: 7e7e 0a2a 2060 6054 7570 6c65 6060 2074  ~~.* ``Tuple`` t
-00001160: 7261 6974 7320 6375 7272 656e 746c 7920  raits currently 
-00001170: 6163 6365 7074 2050 7974 686f 6e20 6060  accept Python ``
-00001180: 6c69 7374 6060 206f 626a 6563 7473 2069  list`` objects i
-00001190: 6e20 736f 6d65 2028 6275 740a 2020 6e6f  n some (but.  no
-000011a0: 7420 616c 6c29 2063 6972 6375 6d73 7461  t all) circumsta
-000011b0: 6e63 6573 2e20 5468 6174 2066 6561 7475  nces. That featu
-000011c0: 7265 2069 7320 6465 7072 6563 6174 6564  re is deprecated
-000011d0: 2c20 616e 6420 7769 6c6c 2062 6520 7265  , and will be re
-000011e0: 6d6f 7665 640a 2020 696e 2061 2066 7574  moved.  in a fut
-000011f0: 7572 6520 7665 7273 696f 6e20 6f66 2054  ure version of T
-00001200: 7261 6974 732e 2028 2331 3632 3729 0a0a  raits. (#1627)..
-00001210: 5479 7065 2073 7475 6273 0a7e 7e7e 7e7e  Type stubs.~~~~~
-00001220: 7e7e 7e7e 7e0a 2a20 4164 6420 7374 7562  ~~~~~.* Add stub
-00001230: 7320 666f 7220 6060 4172 7261 7960 602c  s for ``Array``,
-00001240: 2060 6041 7272 6179 4f72 4e6f 6e65 6060   ``ArrayOrNone``
-00001250: 2c20 616e 6420 6060 4341 7272 6179 6060  , and ``CArray``
-00001260: 2e20 2823 3136 3832 290a 2a20 4669 7820  . (#1682).* Fix 
-00001270: 7661 7269 6f75 7320 7374 7562 7320 666f  various stubs fo
-00001280: 7220 6060 7472 6169 7473 2e74 7261 6974  r ``traits.trait
-00001290: 5f74 7970 6573 6060 3b20 6164 6420 7374  _types``; add st
-000012a0: 7562 7320 666f 720a 2020 6060 7472 6169  ubs for.  ``trai
-000012b0: 7473 2e63 7472 6169 7473 6060 2e20 2823  ts.ctraits``. (#
-000012c0: 3136 3631 290a 2a20 4669 7820 7468 6174  1661).* Fix that
-000012d0: 2060 6054 7261 6974 4572 726f 7260 6020   ``TraitError`` 
-000012e0: 7374 7562 7320 7765 7265 6e27 7420 6578  stubs weren't ex
-000012f0: 706f 7365 6420 6174 2060 6074 7261 6974  posed at ``trait
-00001300: 732e 6170 6960 6020 6c65 7665 6c2e 0a20  s.api`` level.. 
-00001310: 2028 2331 3635 3829 0a2a 204d 616b 6520   (#1658).* Make 
-00001320: 6060 496e 7460 6020 616e 6420 6060 466c  ``Int`` and ``Fl
-00001330: 6f61 7460 6020 7479 7065 2073 7475 6273  oat`` type stubs
-00001340: 206d 6f72 6520 6163 6375 7261 7465 2e20   more accurate. 
-00001350: 2823 3136 3536 290a 2a20 4669 7820 696e  (#1656).* Fix in
-00001360: 636f 7272 6563 7420 7479 7065 2073 7475  correct type stu
-00001370: 6273 2066 6f72 2074 6865 2060 6044 6963  bs for the ``Dic
-00001380: 7460 6020 7472 6169 7420 7479 7065 2e20  t`` trait type. 
-00001390: 2823 3136 3535 290a 0a44 6f63 756d 656e  (#1655)..Documen
-000013a0: 7461 7469 6f6e 0a7e 7e7e 7e7e 7e7e 7e7e  tation.~~~~~~~~~
-000013b0: 7e7e 7e7e 0a2a 204d 616b 6520 6060 4554  ~~~~.* Make ``ET
-000013c0: 5343 6f6e 6669 6760 6020 636c 6173 7320  SConfig`` class 
-000013d0: 646f 6375 6d65 6e74 6174 696f 6e20 7669  documentation vi
-000013e0: 7369 626c 6520 696e 2074 6865 2041 5049  sible in the API
-000013f0: 2064 6f63 732e 2028 2331 3638 3829 0a2a   docs. (#1688).*
-00001400: 2041 6464 2063 6f70 7920 6275 7474 6f6e   Add copy button
-00001410: 7320 746f 2063 6f64 6520 7361 6d70 6c65  s to code sample
-00001420: 7320 696e 2064 6f63 756d 656e 7461 7469  s in documentati
-00001430: 6f6e 2e20 2823 3136 3531 2c20 2331 3635  on. (#1651, #165
-00001440: 3329 0a2a 2044 6f63 756d 656e 7420 6060  3).* Document ``
-00001450: 4461 7465 6060 2c20 6060 4461 7465 7469  Date``, ``Dateti
-00001460: 6d65 6060 2061 6e64 2060 6054 696d 6560  me`` and ``Time`
-00001470: 6020 7472 6169 7420 7479 7065 732e 2028  ` trait types. (
-00001480: 2331 3634 3129 0a2a 2046 6978 2073 6f6d  #1641).* Fix som
-00001490: 6520 6d69 7373 696e 6720 6d65 6e74 696f  e missing mentio
-000014a0: 6e73 206f 6620 6060 5365 7460 6020 696e  ns of ``Set`` in
-000014b0: 206e 6f74 6966 6963 6174 696f 6e20 646f   notification do
-000014c0: 6373 2e20 2823 3136 3138 290a 2a20 446f  cs. (#1618).* Do
-000014d0: 6375 6d65 6e74 2074 6865 2060 6027 736f  cument the ``'so
-000014e0: 6d65 5f74 7261 6974 2e2d 2760 6020 7061  me_trait.-'`` pa
-000014f0: 7474 6572 6e20 666f 7220 6060 6f6e 5f74  ttern for ``on_t
-00001500: 7261 6974 5f63 6861 6e67 6560 602e 2028  rait_change``. (
-00001510: 2331 3539 3229 0a2a 2044 6f63 756d 656e  #1592).* Documen
-00001520: 7420 7468 6174 2060 6045 6974 6865 7260  t that ``Either`
-00001530: 6020 7368 6f75 6c64 206e 6f74 2062 6520  ` should not be 
-00001540: 7573 6564 2069 6e20 6e65 7720 636f 6465  used in new code
-00001550: 2e20 2823 3136 3939 290a 2a20 446f 6375  . (#1699).* Docu
-00001560: 6d65 6e74 2074 6861 7420 6060 5472 6169  ment that ``Trai
-00001570: 7450 7265 6669 784d 6170 6060 2061 6e64  tPrefixMap`` and
-00001580: 2060 6054 7261 6974 5072 6566 6978 4c69   ``TraitPrefixLi
-00001590: 7374 6060 2061 7265 2064 6570 7265 6361  st`` are depreca
-000015a0: 7465 642e 0a20 2028 2331 3730 3229 0a2a  ted..  (#1702).*
-000015b0: 2044 6f63 756d 656e 7420 7468 6174 2074   Document that t
-000015c0: 6865 2054 7261 6974 2066 6163 746f 7279  he Trait factory
-000015d0: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
-000015e0: 206e 6f74 2062 6520 7573 6564 2069 6e20   not be used in 
-000015f0: 6e65 7720 636f 6465 2e0a 2020 2823 3137  new code..  (#17
-00001600: 3030 290a 2a20 4d69 7363 656c 6c61 6e65  00).* Miscellane
-00001610: 6f75 7320 6d69 6e6f 7220 6669 7865 732e  ous minor fixes.
-00001620: 2028 2331 3538 332c 2023 3136 3131 2c20   (#1583, #1611, 
-00001630: 2331 3635 322c 2023 3136 3830 290a 0a42  #1652, #1680)..B
-00001640: 7569 6c64 2061 6e64 2063 6f6e 7469 6e75  uild and continu
-00001650: 6f75 7320 696e 7465 6772 6174 696f 6e0a  ous integration.
-00001660: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001670: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001680: 0a2a 2044 6f6e 2774 2063 6f6c 6c65 6374  .* Don't collect
-00001690: 2074 7261 6974 732d 7374 7562 7320 7465   traits-stubs te
-000016a0: 7374 7320 756e 6465 7220 7079 7465 7374  sts under pytest
-000016b0: 2e20 4173 2061 2072 6573 756c 7420 6f66  . As a result of
-000016c0: 2074 6869 730a 2020 616e 6420 6f74 6865   this.  and othe
-000016d0: 7220 6669 7865 732c 2074 6865 2074 6573  r fixes, the tes
-000016e0: 7420 7375 6974 6520 6e6f 7720 7061 7373  t suite now pass
-000016f0: 6573 2075 6e64 6572 2070 7974 6573 742e  es under pytest.
-00001700: 2028 2331 3639 3029 0a2a 2055 7064 6174   (#1690).* Updat
-00001710: 6520 6060 6574 7374 6f6f 6c2e 7079 6060  e ``etstool.py``
-00001720: 2066 6f72 2050 7974 686f 6e20 332e 3820   for Python 3.8 
-00001730: 7375 7070 6f72 742e 2050 7974 686f 6e20  support. Python 
-00001740: 332e 3820 6973 206e 6f77 2074 6865 0a20  3.8 is now the. 
-00001750: 2064 6566 6175 6c74 2050 7974 686f 6e20   default Python 
-00001760: 7665 7273 696f 6e20 666f 7220 6275 696c  version for buil
-00001770: 6473 2e20 2823 3136 3934 290a 2a20 5573  ds. (#1694).* Us
-00001780: 6520 5079 5369 6465 3620 666f 7220 5079  e PySide6 for Py
-00001790: 7468 6f6e 203e 3d20 332e 3820 696e 7374  thon >= 3.8 inst
-000017a0: 6561 6420 6f66 2050 7953 6964 6532 2069  ead of PySide2 i
-000017b0: 6e20 4349 2074 6573 7469 6e67 2e20 2823  n CI testing. (#
-000017c0: 3136 3835 290a 2a20 4164 6420 6060 7079  1685).* Add ``py
-000017d0: 7072 6f6a 6563 742e 746f 6d6c 6060 2066  project.toml`` f
-000017e0: 696c 6573 2066 6f72 2062 6f74 6820 5472  iles for both Tr
-000017f0: 6169 7473 2061 6e64 2074 7261 6974 732d  aits and traits-
-00001800: 7374 7562 732e 2028 2331 3638 392c 2023  stubs. (#1689, #
-00001810: 3136 3736 290a 2a20 4164 6420 5079 7468  1676).* Add Pyth
-00001820: 6f6e 2033 2e31 3120 746f 2073 6f6d 6520  on 3.11 to some 
-00001830: 776f 726b 666c 6f77 2072 756e 732e 2028  workflow runs. (
-00001840: 2331 3630 302c 2023 3136 3630 2c20 2331  #1600, #1660, #1
-00001850: 3637 3429 0a2a 2041 6464 2050 7974 686f  674).* Add Pytho
-00001860: 6e20 332e 3130 2074 6f20 696e 7374 616c  n 3.10 to instal
-00001870: 6c2d 6672 6f6d 2d50 7950 4920 776f 726b  l-from-PyPI work
-00001880: 666c 6f77 2e20 2823 3135 3736 290a 2a20  flow. (#1576).* 
-00001890: 416c 6c6f 7720 7275 6e6e 696e 6720 7468  Allow running th
-000018a0: 6520 6d61 696e 2074 6573 7420 776f 726b  e main test work
-000018b0: 666c 6f77 206d 616e 7561 6c6c 792e 2028  flow manually. (
-000018c0: 2331 3630 3729 0a2a 2053 7769 7463 6820  #1607).* Switch 
-000018d0: 536c 6163 6b20 6368 616e 6e65 6c20 7573  Slack channel us
-000018e0: 6564 2074 6f20 7265 706f 7274 2047 6974  ed to report Git
-000018f0: 4875 6220 4163 7469 6f6e 7320 6661 696c  Hub Actions fail
-00001900: 7572 6573 2e20 2823 3136 3530 290a 2a20  ures. (#1650).* 
-00001910: 4578 636c 7564 6520 6060 6275 696c 6460  Exclude ``build`
-00001920: 6020 6469 7265 6374 6f72 7920 696e 2066  ` directory in f
-00001930: 6c61 6b65 3820 636f 6e66 6967 7572 6174  lake8 configurat
-00001940: 696f 6e2e 2028 2331 3633 3529 0a2a 2052  ion. (#1635).* R
-00001950: 652d 696e 636c 7564 6520 4e75 6d50 7920  e-include NumPy 
-00001960: 6173 2061 2074 6573 7420 6465 7065 6e64  as a test depend
-00001970: 656e 6379 206f 6e20 5079 7468 6f6e 2033  ency on Python 3
-00001980: 2e31 302e 2028 2331 3539 3329 0a0a 4d61  .10. (#1593)..Ma
-00001990: 696e 7465 6e61 6e63 6520 616e 6420 7265  intenance and re
-000019a0: 6661 6374 6f72 696e 670a 7e7e 7e7e 7e7e  factoring.~~~~~~
-000019b0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-000019c0: 7e7e 7e7e 7e0a 2a20 6060 2e67 6974 6967  ~~~~~.* ``.gitig
-000019d0: 6e6f 7265 6060 2063 6c65 616e 7570 2061  nore`` cleanup a
-000019e0: 6e64 2075 7064 6174 6573 2e20 2823 3136  nd updates. (#16
-000019f0: 3738 2c20 2331 3638 3729 0a2a 2052 6574  78, #1687).* Ret
-00001a00: 7572 6e20 6060 5079 4572 725f 466f 726d  urn ``PyErr_Form
-00001a10: 6174 6060 2063 616c 6c73 2069 6e20 6060  at`` calls in ``
-00001a20: 7472 6169 7473 2f63 7472 6169 7473 2e63  traits/ctraits.c
-00001a30: 6060 2e20 2823 3136 3430 290a 2a20 5570  ``. (#1640).* Up
-00001a40: 6461 7465 2063 6f70 7972 6967 6874 2068  date copyright h
-00001a50: 6561 6465 7220 656e 6420 7965 6172 2074  eader end year t
-00001a60: 6f20 3230 3232 2e20 2823 3136 3132 290a  o 2022. (#1612).
-00001a70: 2a20 5468 6520 6060 6369 2d73 7263 2d72  * The ``ci-src-r
-00001a80: 6571 7569 7265 6d65 6e74 732e 7478 7460  equirements.txt`
-00001a90: 6020 6669 6c65 2069 736e 2774 2075 7365  ` file isn't use
-00001aa0: 643b 2072 656d 6f76 6520 6974 2e20 2823  d; remove it. (#
-00001ab0: 3136 3032 290a 0a0a 5265 6c65 6173 6520  1602)...Release 
-00001ac0: 362e 332e 320a 2d2d 2d2d 2d2d 2d2d 2d2d  6.3.2.----------
-00001ad0: 2d2d 2d0a 0a52 656c 6561 7365 643a 2032  ---..Released: 2
-00001ae0: 3032 312d 3131 2d31 300a 0a54 7261 6974  021-11-10..Trait
-00001af0: 7320 362e 332e 3220 6973 2061 2062 7567  s 6.3.2 is a bug
-00001b00: 6669 7820 7265 6c65 6173 652c 2066 6978  fix release, fix
-00001b10: 696e 6720 616e 2069 7373 7565 2077 6974  ing an issue wit
-00001b20: 6820 6475 706c 6963 6174 650a 6e6f 7469  h duplicate.noti
-00001b30: 6669 6361 7469 6f6e 7320 6672 6f6d 2060  fications from `
-00001b40: 6050 726f 7065 7274 7960 6020 7472 6169  `Property`` trai
-00001b50: 7473 2075 7369 6e67 2074 6865 2060 606f  ts using the ``o
-00001b60: 6273 6572 7665 6060 2066 7261 6d65 776f  bserve`` framewo
-00001b70: 726b 2e0a 0a0a 4669 7865 730a 7e7e 7e7e  rk....Fixes.~~~~
-00001b80: 7e0a 0a2a 2046 6978 2074 6861 7420 6060  ~..* Fix that ``
-00001b90: 5072 6f70 6572 7479 6060 2074 7261 6974  Property`` trait
-00001ba0: 7320 7573 696e 6720 6060 6f62 7365 7276  s using ``observ
-00001bb0: 6560 6020 6d65 7461 6461 7461 2063 6f75  e`` metadata cou
-00001bc0: 6c64 2062 6520 6669 7265 640a 2020 7477  ld be fired.  tw
-00001bd0: 6963 6520 696e 2073 7562 636c 6173 7365  ice in subclasse
-00001be0: 732e 2028 2331 3538 3729 0a0a 0a52 656c  s. (#1587)...Rel
-00001bf0: 6561 7365 2036 2e33 2e31 0a2d 2d2d 2d2d  ease 6.3.1.-----
-00001c00: 2d2d 2d2d 2d2d 2d2d 0a0a 5265 6c65 6173  --------..Releas
-00001c10: 6564 3a20 3230 3231 2d31 302d 3132 0a0a  ed: 2021-10-12..
-00001c20: 5472 6169 7473 2036 2e33 2e31 2069 7320  Traits 6.3.1 is 
-00001c30: 6120 6275 6766 6978 2072 656c 6561 7365  a bugfix release
-00001c40: 2c20 6669 7869 6e67 2061 6e20 696e 636f  , fixing an inco
-00001c50: 6d70 6174 6962 696c 6974 7920 6265 7477  mpatibility betw
-00001c60: 6565 6e0a 5472 6169 7473 2036 2e33 2e30  een.Traits 6.3.0
-00001c70: 2061 6e64 204d 6179 6176 6920 3c3d 2034   and Mayavi <= 4
-00001c80: 2e37 2e33 2e0a 0a46 6978 6573 0a7e 7e7e  .7.3...Fixes.~~~
-00001c90: 7e7e 0a0a 2a20 4d61 6b65 2060 6050 7265  ~~..* Make ``Pre
-00001ca0: 6669 784d 6170 2e5f 6d61 7060 6020 6176  fixMap._map`` av
-00001cb0: 6169 6c61 626c 6520 6167 6169 6e2c 2066  ailable again, f
-00001cc0: 6f72 2063 6f6d 7061 7469 6269 6c69 7479  or compatibility
-00001cd0: 2077 6974 6820 4d61 7961 7669 2e0a 2020   with Mayavi..  
-00001ce0: 2823 3135 3738 290a 0a0a 5265 6c65 6173  (#1578)...Releas
-00001cf0: 6520 362e 332e 300a 2d2d 2d2d 2d2d 2d2d  e 6.3.0.--------
-00001d00: 2d2d 2d2d 2d0a 0a52 656c 6561 7365 643a  -----..Released:
-00001d10: 2032 3032 312d 3130 2d30 380a 0a54 7261   2021-10-08..Tra
-00001d20: 6974 7320 362e 3320 6973 2074 6865 206c  its 6.3 is the l
-00001d30: 6174 6573 7420 6665 6174 7572 6520 7265  atest feature re
-00001d40: 6c65 6173 6520 696e 2074 6865 2054 7261  lease in the Tra
-00001d50: 6974 7320 3620 7365 7269 6573 2c20 7769  its 6 series, wi
-00001d60: 7468 2073 6576 6572 616c 0a69 6d70 726f  th several.impro
-00001d70: 7665 6d65 6e74 7320 616e 6420 6669 7865  vements and fixe
-00001d80: 7320 6f76 6572 2054 7261 6974 7320 362e  s over Traits 6.
-00001d90: 322e 0a0a 0a48 6967 686c 6967 6874 7320  2....Highlights 
-00001da0: 6f66 2074 6869 7320 7265 6c65 6173 650a  of this release.
-00001db0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001dc0: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20 5468  ~~~~~~~~~~..* Th
-00001dd0: 6572 6520 6861 7665 2062 6565 6e20 7661  ere have been va
-00001de0: 7269 6f75 7320 6d69 6e6f 7220 7065 7266  rious minor perf
-00001df0: 6f72 6d61 6e63 6520 696d 7072 6f76 656d  ormance improvem
-00001e00: 656e 7473 2074 6f20 7468 6520 636f 7265  ents to the core
-00001e10: 0a20 2060 606f 6e5f 7472 6169 745f 6368  .  ``on_trait_ch
-00001e20: 616e 6765 6060 2061 6e64 2060 606f 6273  ange`` and ``obs
-00001e30: 6572 7665 6060 206d 6163 6869 6e65 7279  erve`` machinery
-00001e40: 2e20 5468 6573 6520 6d61 7920 696d 7072  . These may impr
-00001e50: 6f76 650a 2020 7374 6172 7475 7020 7469  ove.  startup ti
-00001e60: 6d65 2066 6f72 2073 6f6d 6520 5472 6169  me for some Trai
-00001e70: 7473 2d75 7369 6e67 2061 7070 6c69 6361  ts-using applica
-00001e80: 7469 6f6e 732e 0a2a 2054 6865 2060 606f  tions..* The ``o
-00001e90: 6273 6572 7665 6060 206d 696e 692d 6c61  bserve`` mini-la
-00001ea0: 6e67 7561 6765 206e 6f77 2068 6173 2069  nguage now has i
-00001eb0: 6e2d 6c61 6e67 7561 6765 2073 7570 706f  n-language suppo
-00001ec0: 7274 2066 6f72 206c 6973 7465 6e69 6e67  rt for listening
-00001ed0: 0a20 2074 6f20 616c 6c20 7472 6169 7473  .  to all traits
-00001ee0: 2c20 7573 696e 6720 7468 6520 6060 2a60  , using the ``*`
-00001ef0: 6020 6368 6172 6163 7465 722e 0a2a 2053  ` character..* S
-00001f00: 7570 706f 7274 2066 6f72 2050 7974 686f  upport for Pytho
-00001f10: 6e20 332e 3130 2068 6173 2062 6565 6e20  n 3.10 has been 
-00001f20: 6164 6465 642e 0a0a 0a4d 6967 7261 7469  added....Migrati
-00001f30: 6f6e 2067 7569 6465 0a7e 7e7e 7e7e 7e7e  on guide.~~~~~~~
-00001f40: 7e7e 7e7e 7e7e 7e7e 0a0a 5472 6169 7473  ~~~~~~~~..Traits
-00001f50: 2036 2e33 2069 7320 696e 7465 6e64 6564   6.3 is intended
-00001f60: 2074 6f20 6265 2066 756c 6c79 2062 6163   to be fully bac
-00001f70: 6b77 6172 6473 2063 6f6d 7061 7469 626c  kwards compatibl
-00001f80: 6520 7769 7468 2054 7261 6974 7320 362e  e with Traits 6.
-00001f90: 322c 2061 6e64 0a6d 6f73 7420 7072 6f6a  2, and.most proj
-00001fa0: 6563 7473 2073 686f 756c 6420 6861 7665  ects should have
-00001fb0: 206e 6f20 6469 6666 6963 756c 7469 6573   no difficulties
-00001fc0: 2075 7067 7261 6469 6e67 2e20 486f 7765   upgrading. Howe
-00001fd0: 7665 722c 2079 6f75 206d 6179 2073 6565  ver, you may see
-00001fe0: 0a73 6f6d 6520 6e65 7720 6465 7072 6563  .some new deprec
-00001ff0: 6174 696f 6e20 7761 726e 696e 6773 2066  ation warnings f
-00002000: 6f72 2065 7869 7374 696e 6720 636f 6465  or existing code
-00002010: 2c20 7761 726e 696e 6720 6162 6f75 7420  , warning about 
-00002020: 6265 6861 7669 6f75 720a 7468 6174 2077  behaviour.that w
-00002030: 696c 6c20 6265 2063 6861 6e67 6564 2069  ill be changed i
-00002040: 6e20 5472 6169 7473 2037 2e30 2e20 5468  n Traits 7.0. Th
-00002050: 6572 6520 6172 6520 7477 6f20 7061 7274  ere are two part
-00002060: 6963 756c 6172 2073 6574 7320 6f66 2063  icular sets of c
-00002070: 6861 6e67 6573 0a74 6f20 6c6f 6f6b 206f  hanges.to look o
-00002080: 7574 2066 6f72 3a0a 0a2a 2053 7461 7274  ut for:..* Start
-00002090: 696e 6720 7769 7468 2054 7261 6974 7320  ing with Traits 
-000020a0: 372e 302c 2074 6865 2060 6041 6e79 6060  7.0, the ``Any``
-000020b0: 2074 7261 6974 2074 7970 6520 7769 6c6c   trait type will
-000020c0: 2074 7265 6174 2061 2064 6566 6175 6c74   treat a default
-000020d0: 0a20 2076 616c 7565 206f 6620 7479 7065  .  value of type
-000020e0: 2060 606c 6973 7460 6020 6f72 2060 6064   ``list`` or ``d
-000020f0: 6963 7460 6020 6469 6666 6572 656e 746c  ict`` differentl
-00002100: 792e 2043 7572 7265 6e74 6c79 2c20 696e  y. Currently, in
-00002110: 7374 616e 6365 7320 6f66 0a20 2060 606c  stances of.  ``l
-00002120: 6973 7460 6020 616e 6420 6060 6469 6374  ist`` and ``dict
-00002130: 6060 2061 7265 2073 7065 6369 616c 2d63  `` are special-c
-00002140: 6173 6564 2c20 616e 6420 6120 7065 722d  ased, and a per-
-00002150: 696e 7374 616e 6365 2063 6f70 7920 6f66  instance copy of
-00002160: 2074 6865 0a20 2064 6566 6175 6c74 2069   the.  default i
-00002170: 7320 7072 6f76 6964 6564 2074 6f20 6561  s provided to ea
-00002180: 6368 2060 6048 6173 5472 6169 7473 6060  ch ``HasTraits``
-00002190: 2069 6e73 7461 6e63 652e 2049 6e20 5472   instance. In Tr
-000021a0: 6169 7473 2037 2e30 2c20 7468 6973 0a20  aits 7.0, this. 
-000021b0: 2073 7065 6369 616c 2d63 6173 696e 6720   special-casing 
-000021c0: 7769 6c6c 2062 6520 7265 6d6f 7665 642c  will be removed,
-000021d0: 2061 6e64 2074 6865 2064 6566 6175 6c74   and the default
-000021e0: 2076 616c 7565 2077 696c 6c20 6265 2073   value will be s
-000021f0: 6861 7265 6420 6265 7477 6565 6e0a 2020  hared between.  
-00002200: 616c 6c20 696e 7374 616e 6365 732e 2046  all instances. F
-00002210: 6f72 2074 6865 2036 2e33 2072 656c 6561  or the 6.3 relea
-00002220: 7365 206f 6620 5472 6169 7473 2c20 6120  se of Traits, a 
-00002230: 6465 7072 6563 6174 696f 6e20 7761 726e  deprecation warn
-00002240: 696e 6720 6973 2069 7373 7565 640a 2020  ing is issued.  
-00002250: 7768 656e 6576 6572 2061 2074 7261 6974  whenever a trait
-00002260: 2064 6566 696e 6974 696f 6e20 6f66 2074   definition of t
-00002270: 6865 2066 6f72 6d20 6060 416e 7928 5b31  he form ``Any([1
-00002280: 2c20 322c 2033 5d29 6060 206f 7220 6060  , 2, 3])`` or ``
-00002290: 416e 7928 7b7d 2960 600a 2020 6973 2065  Any({})``.  is e
-000022a0: 6e63 6f75 6e74 6572 6564 2e20 5573 6572  ncountered. User
-000022b0: 7320 6361 6e20 7265 7461 696e 2074 6865  s can retain the
-000022c0: 2065 7869 7374 696e 6720 6265 6861 7669   existing behavi
-000022d0: 6f75 7220 616e 6420 7375 7070 7265 7373  our and suppress
-000022e0: 2074 6865 0a20 2077 6172 6e69 6e67 2062   the.  warning b
-000022f0: 7920 6368 616e 6769 6e67 2074 6865 6972  y changing their
-00002300: 2063 6f64 6520 746f 2075 7365 2074 6865   code to use the
-00002310: 206e 6577 2060 6066 6163 746f 7279 6060   new ``factory``
-00002320: 2061 7267 756d 656e 7420 746f 2074 6865   argument to the
-00002330: 0a20 2060 6041 6e79 6060 2074 7261 6974  .  ``Any`` trait
-00002340: 2074 7970 652c 2066 6f72 2065 7861 6d70   type, for examp
-00002350: 6c65 2072 6570 6c61 6369 6e67 2061 2074  le replacing a t
-00002360: 7261 6974 2064 6563 6c61 7261 7469 6f6e  rait declaration
-00002370: 2060 6066 6f6f 203d 0a20 2041 6e79 287b   ``foo =.  Any({
-00002380: 7d29 6060 2077 6974 6820 6060 666f 6f20  })`` with ``foo 
-00002390: 3d20 416e 7928 6661 6374 6f72 793d 6469  = Any(factory=di
-000023a0: 6374 2960 602c 2061 6e64 2061 2074 7261  ct)``, and a tra
-000023b0: 6974 2064 6563 6c61 7261 7469 6f6e 2060  it declaration `
-000023c0: 6066 6f6f 203d 0a20 2041 6e79 285b 312c  `foo =.  Any([1,
-000023d0: 2032 2c20 335d 2960 6020 7769 7468 2060   2, 3])`` with `
-000023e0: 6066 6f6f 203d 2041 6e79 2866 6163 746f  `foo = Any(facto
-000023f0: 7279 3d6c 6973 742c 2061 7267 733d 285b  ry=list, args=([
-00002400: 312c 2032 2c20 335d 2c29 2960 602e 0a0a  1, 2, 3],))``...
-00002410: 2a20 5374 6172 7469 6e67 2077 6974 6820  * Starting with 
-00002420: 5472 6169 7473 2037 2e30 2c20 7468 6520  Traits 7.0, the 
-00002430: 6060 4461 7465 6060 2074 7261 6974 2074  ``Date`` trait t
-00002440: 7970 6520 7769 6c6c 206e 6f20 6c6f 6e67  ype will no long
-00002450: 6572 2061 6363 6570 740a 2020 6060 6461  er accept.  ``da
-00002460: 7465 7469 6d65 6060 2069 6e73 7461 6e63  tetime`` instanc
-00002470: 6573 2062 7920 6465 6661 756c 742e 2054  es by default. T
-00002480: 7261 6974 7320 362e 3320 7769 6c6c 2069  raits 6.3 will i
-00002490: 7373 7565 2061 2064 6570 7265 6361 7469  ssue a deprecati
-000024a0: 6f6e 0a20 2077 6172 6e69 6e67 2077 6865  on.  warning whe
-000024b0: 6e65 7665 7220 6120 6060 6461 7465 7469  never a ``dateti
-000024c0: 6d65 6060 2069 6e73 7461 6e63 6520 6973  me`` instance is
-000024d0: 2061 7373 6967 6e65 6420 6173 2061 2076   assigned as a v
-000024e0: 616c 7565 2066 6f72 0a20 2061 2060 6044  alue for.  a ``D
-000024f0: 6174 6560 6020 7472 6169 742e 2054 6865  ate`` trait. The
-00002500: 2065 7869 7374 696e 6720 6265 6861 7669   existing behavi
-00002510: 6f75 7220 6361 6e20 6265 2070 7265 7365  our can be prese
-00002520: 7276 6564 2061 6e64 2074 6865 2077 6172  rved and the war
-00002530: 6e69 6e67 0a20 2073 696c 656e 6365 6420  ning.  silenced 
-00002540: 6279 2075 7369 6e67 2060 6044 6174 6528  by using ``Date(
-00002550: 616c 6c6f 775f 6461 7465 7469 6d65 3d54  allow_datetime=T
-00002560: 7275 6529 6060 3b20 616c 7465 726e 6174  rue)``; alternat
-00002570: 6976 656c 792c 2079 6f75 2063 616e 0a20  ively, you can. 
-00002580: 2075 7365 2060 6044 6174 6528 616c 6c6f   use ``Date(allo
-00002590: 775f 6461 7465 7469 6d65 3d46 616c 7365  w_datetime=False
-000025a0: 2960 6020 746f 2061 646f 7074 2074 6865  )`` to adopt the
-000025b0: 2054 7261 6974 7320 372e 3020 6265 6861   Traits 7.0 beha
-000025c0: 7669 6f75 720a 2020 7269 6768 7420 6e6f  viour.  right no
-000025d0: 772e 0a0a 0a44 6574 6169 6c65 6420 5052  w....Detailed PR
-000025e0: 2d62 792d 5052 2063 6861 6e67 6573 0a7e  -by-PR changes.~
-000025f0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00002600: 7e7e 7e7e 7e7e 7e7e 0a0a 4f76 6572 2038  ~~~~~~~~..Over 8
-00002610: 3020 7075 6c6c 2072 6571 7565 7374 7320  0 pull requests 
-00002620: 7765 6e74 2069 6e74 6f20 7468 6973 2072  went into this r
-00002630: 656c 6561 7365 2e20 5468 6520 666f 6c6c  elease. The foll
-00002640: 6f77 696e 6720 7065 6f70 6c65 2063 6f6e  owing people con
-00002650: 7472 6962 7574 6564 0a74 6f20 7468 6520  tributed.to the 
-00002660: 7265 6c65 6173 653a 0a0a 2a20 3078 666c  release:..* 0xfl
-00002670: 6f74 7573 0a2a 2041 6172 6f6e 2041 7972  otus.* Aaron Ayr
-00002680: 6573 0a2a 204b 6974 2043 686f 690a 2a20  es.* Kit Choi.* 
-00002690: 4d61 726b 2044 6963 6b69 6e73 6f6e 0a2a  Mark Dickinson.*
-000026a0: 2043 6869 676f 7a69 6520 4e72 690a 2a20   Chigozie Nri.* 
-000026b0: 506f 7275 7269 2053 6169 2052 6168 756c  Poruri Sai Rahul
-000026c0: 0a2a 2043 6f72 7261 6e20 5765 6273 7465  .* Corran Webste
-000026d0: 720a 2a20 4a6f 686e 2057 6967 6769 6e73  r.* John Wiggins
-000026e0: 0a2a 2050 6574 6572 205a 6168 656d 737a  .* Peter Zahemsz
-000026f0: 6b79 0a0a 5468 616e 6b20 796f 7520 746f  ky..Thank you to
-00002700: 2061 6c6c 2077 686f 2063 6f6e 7472 6962   all who contrib
-00002710: 7574 6564 210a 0a0a 4665 6174 7572 6573  uted!...Features
-00002720: 0a7e 7e7e 7e7e 7e7e 7e0a 0a2a 2054 6865  .~~~~~~~~..* The
-00002730: 2060 606f 6273 6572 7665 6060 206d 696e   ``observe`` min
-00002740: 692d 6c61 6e67 7561 6765 206e 6f77 2073  i-language now s
-00002750: 7570 706f 7274 7320 7573 6520 6f66 2060  upports use of `
-00002760: 6022 2a22 6060 2066 6f72 206c 6973 7465  `"*"`` for liste
-00002770: 6e69 6e67 2074 6f0a 2020 616c 6c20 7472  ning to.  all tr
-00002780: 6169 7473 206f 6e20 6120 6060 4861 7354  aits on a ``HasT
-00002790: 7261 6974 7360 6020 6f62 6a65 6374 2e20  raits`` object. 
-000027a0: 4375 7272 656e 746c 7920 7468 6973 2073  Currently this s
-000027b0: 7570 706f 7274 2069 7320 6c69 6d69 7465  upport is limite
-000027c0: 6420 746f 0a20 2063 6173 6573 2077 6865  d to.  cases whe
-000027d0: 7265 2074 6865 2060 6022 2a22 6060 2061  re the ``"*"`` a
-000027e0: 7070 6561 7273 2069 6e20 6120 7465 726d  ppears in a term
-000027f0: 696e 616c 2070 6f73 6974 696f 6e2e 2046  inal position. F
-00002800: 6f72 2065 7861 6d70 6c65 2c0a 2020 6060  or example,.  ``
-00002810: 6f62 7365 7276 6528 2266 6f6f 3a2a 2229  observe("foo:*")
-00002820: 6060 2069 7320 7375 7070 6f72 7465 642c  `` is supported,
-00002830: 2062 7574 2060 606f 6273 6572 7665 2822   but ``observe("
-00002840: 2a3a 666f 6f22 2960 6020 6973 206e 6f74  *:foo")`` is not
-00002850: 2e0a 2020 2823 3134 3936 2c20 2331 3532  ..  (#1496, #152
-00002860: 3529 0a2a 2054 6865 2060 6041 6e79 6060  5).* The ``Any``
-00002870: 2074 7261 6974 2074 7970 6520 6e6f 7720   trait type now 
-00002880: 7375 7070 6f72 7473 2061 2060 6066 6163  supports a ``fac
-00002890: 746f 7279 6060 2061 7267 756d 656e 7420  tory`` argument 
-000028a0: 2877 6974 6820 6163 636f 6d70 616e 7969  (with accompanyi
-000028b0: 6e67 0a20 2060 6061 7267 7360 6020 616e  ng.  ``args`` an
-000028c0: 6420 6060 6b77 6060 2061 7267 756d 656e  d ``kw`` argumen
-000028d0: 7473 292e 2054 6869 7320 6361 6e20 6265  ts). This can be
-000028e0: 2075 7365 6420 746f 2073 7065 6369 6679   used to specify
-000028f0: 2061 2070 6572 2d69 6e73 7461 6e63 650a   a per-instance.
-00002900: 2020 6465 6661 756c 742c 2066 6f72 2065    default, for e
-00002910: 7861 6d70 6c65 2077 6974 6820 6060 416e  xample with ``An
-00002920: 7928 6661 6374 6f72 793d 6469 6374 2960  y(factory=dict)`
-00002930: 602e 2028 2331 3535 372c 2023 3135 3538  `. (#1557, #1558
-00002940: 290a 2a20 5468 6520 6060 4465 6661 756c  ).* The ``Defaul
-00002950: 7456 616c 7565 6060 2065 6e75 6d65 7261  tValue`` enumera
-00002960: 7469 6f6e 2068 6173 2061 206e 6577 206d  tion has a new m
-00002970: 656d 6265 7220 6060 4465 6661 756c 7456  ember ``DefaultV
-00002980: 616c 7565 2e64 6973 616c 6c6f 7760 600a  alue.disallow``.
-00002990: 2020 696e 7465 6e64 6564 2074 6f20 6265    intended to be
-000029a0: 2075 7365 6420 666f 7220 7472 6169 7420   used for trait 
-000029b0: 7479 7065 7320 7468 6174 2064 6f6e 2774  types that don't
-000029c0: 2068 6176 6520 6120 6d65 616e 696e 6766   have a meaningf
-000029d0: 756c 2064 6566 6175 6c74 2e20 466f 720a  ul default. For.
-000029e0: 2020 7472 6169 7473 2075 7369 6e67 2074    traits using t
-000029f0: 6869 7320 6465 6661 756c 7420 7661 6c75  his default valu
-00002a00: 6520 7479 7065 2c20 616e 2061 7474 656d  e type, an attem
-00002a10: 7074 2074 6f20 7265 7472 6965 7665 2074  pt to retrieve t
-00002a20: 6865 0a20 2063 6f72 7265 7370 6f6e 6469  he.  correspondi
-00002a30: 6e67 2064 6566 6175 6c74 2075 7369 6e67  ng default using
-00002a40: 2060 6064 6566 6175 6c74 5f76 616c 7565   ``default_value
-00002a50: 5f66 6f72 6060 2077 696c 6c20 7261 6973  _for`` will rais
-00002a60: 6520 6060 5661 6c75 6545 7272 6f72 6060  e ``ValueError``
-00002a70: 2e0a 2020 2823 3135 3436 290a 2a20 5768  ..  (#1546).* Wh
-00002a80: 656e 2061 206d 6574 686f 6420 6973 2064  en a method is d
-00002a90: 6563 6f72 6174 6564 2077 6974 6820 616e  ecorated with an
-00002aa0: 2060 606f 6273 6572 7665 6060 2064 6563   ``observe`` dec
-00002ab0: 6f72 6174 6f72 2c20 7468 6520 6d65 7468  orator, the meth
-00002ac0: 6f64 0a20 2073 6967 6e61 7475 7265 2069  od.  signature i
-00002ad0: 7320 6e6f 7720 6368 6563 6b65 642c 2061  s now checked, a
-00002ae0: 6e64 2061 2077 6172 6e69 6e67 2069 7373  nd a warning iss
-00002af0: 7565 6420 6966 2069 7420 646f 6573 6e27  ued if it doesn'
-00002b00: 7420 6d61 7463 6820 7468 650a 2020 6578  t match the.  ex
-00002b10: 7065 6374 6564 2073 6967 6e61 7475 7265  pected signature
-00002b20: 2e20 5468 6973 2073 686f 756c 6420 6361  . This should ca
-00002b30: 7463 6820 7468 6520 636f 6d6d 6f6e 2065  tch the common e
-00002b40: 7272 6f72 206f 6620 666f 7267 6574 7469  rror of forgetti
-00002b50: 6e67 2074 6f0a 2020 7072 6f76 6964 6520  ng to.  provide 
-00002b60: 7468 6520 6060 6576 656e 7460 6020 7061  the ``event`` pa
-00002b70: 7261 6d65 7465 722e 2028 2331 3532 3929  rameter. (#1529)
-00002b80: 0a2a 2049 6e20 6060 4554 5354 6f6f 6c6b  .* In ``ETSToolk
-00002b90: 6974 6060 2c20 7468 6520 6060 2271 7422  it``, the ``"qt"
-00002ba0: 6060 2074 6f6f 6c6b 6974 206e 616d 6520  `` toolkit name 
-00002bb0: 6973 206e 6f77 2073 7570 706f 7274 6564  is now supported
-00002bc0: 2061 7320 6120 7379 6e6f 6e79 6d0a 2020   as a synonym.  
-00002bd0: 666f 7220 6060 2271 7434 2260 602e 2028  for ``"qt4"``. (
-00002be0: 2331 3433 3629 0a2a 2054 6865 2060 6044  #1436).* The ``D
-00002bf0: 6174 6560 602c 2060 6044 6174 6574 696d  ate``, ``Datetim
-00002c00: 6560 6020 616e 6420 6060 5469 6d65 6060  e`` and ``Time``
-00002c10: 2074 7261 6974 2074 7970 6573 2068 6176   trait types hav
-00002c20: 6520 6120 6e65 7720 6172 6775 6d65 6e74  e a new argument
-00002c30: 0a20 2060 6061 6c6c 6f77 5f6e 6f6e 6560  .  ``allow_none`
-00002c40: 602e 2049 6e20 7468 6520 6675 7475 7265  `. In the future
-00002c50: 2c20 7468 6573 6520 7472 6169 7420 7479  , these trait ty
-00002c60: 7065 7320 7769 6c6c 206e 6f74 2061 6363  pes will not acc
-00002c70: 6570 7420 6060 4e6f 6e65 6060 0a20 2075  ept ``None``.  u
-00002c80: 6e6c 6573 7320 6060 616c 6c6f 775f 6e6f  nless ``allow_no
-00002c90: 6e65 3d54 7275 6560 6020 6973 2073 7065  ne=True`` is spe
-00002ca0: 6369 6669 6564 2e20 2823 3134 3332 290a  cified. (#1432).
-00002cb0: 2a20 5468 6520 6060 4461 7465 6060 2074  * The ``Date`` t
-00002cc0: 7261 6974 2074 7970 6520 6861 7320 6120  rait type has a 
-00002cd0: 6e65 7720 6172 6775 6d65 6e74 2060 6061  new argument ``a
-00002ce0: 6c6c 6f77 5f64 6174 6574 696d 6560 602e  llow_datetime``.
-00002cf0: 2049 6e20 7468 6520 6675 7475 7265 2c0a   In the future,.
-00002d00: 2020 6060 6461 7465 7469 6d65 6060 2069    ``datetime`` i
-00002d10: 6e73 7461 6e63 6573 2077 696c 6c20 6e6f  nstances will no
-00002d20: 7420 6265 2076 616c 6964 2076 616c 7565  t be valid value
-00002d30: 7320 666f 7220 6120 6060 4461 7465 6060  s for a ``Date``
-00002d40: 2074 7261 6974 2075 6e6c 6573 730a 2020   trait unless.  
-00002d50: 6060 616c 6c6f 775f 6461 7465 7469 6d65  ``allow_datetime
-00002d60: 3d54 7275 6560 6020 6973 2073 7065 6369  =True`` is speci
-00002d70: 6669 6564 2e20 2823 3134 3239 290a 0a0a  fied. (#1429)...
-00002d80: 5065 7266 6f72 6d61 6e63 650a 7e7e 7e7e  Performance.~~~~
-00002d90: 7e7e 7e7e 7e7e 7e0a 0a2a 2054 6865 2060  ~~~~~~~..* The `
-00002da0: 604f 6273 6572 7665 7247 7261 7068 6060  `ObserverGraph``
-00002db0: 2069 6e73 7461 6e63 6573 2074 6861 7420   instances that 
-00002dc0: 7265 7375 6c74 2066 726f 6d20 636f 6d70  result from comp
-00002dd0: 696c 696e 670a 2020 6060 4f62 7365 7276  iling.  ``Observ
-00002de0: 6572 4578 7072 6573 7369 6f6e 6060 206f  erExpression`` o
-00002df0: 626a 6563 7473 2061 6e64 206f 6273 6572  bjects and obser
-00002e00: 7665 206d 696e 692d 6c61 6e67 7561 6765  ve mini-language
-00002e10: 2073 7472 696e 6773 2061 7265 206e 6f77   strings are now
-00002e20: 0a20 2063 6163 6865 642e 2054 6869 7320  .  cached. This 
-00002e30: 7368 6f75 6c64 2073 7065 6564 2075 7020  should speed up 
-00002e40: 6372 6561 7469 6f6e 2061 6e64 2069 6e73  creation and ins
-00002e50: 7461 6e74 6961 7469 6f6e 206f 6620 6060  tantiation of ``
-00002e60: 4861 7354 7261 6974 7360 600a 2020 7375  HasTraits``.  su
-00002e70: 6263 6c61 7373 6573 2074 6861 7420 696e  bclasses that in
-00002e80: 766f 6c76 6520 6c69 7374 656e 696e 6720  volve listening 
-00002e90: 666f 7220 7468 6520 7361 6d65 2070 6174  for the same pat
-00002ea0: 7465 726e 2069 6e20 6d75 6c74 6970 6c65  tern in multiple
-00002eb0: 2070 6c61 6365 732e 0a20 2028 2331 3531   places..  (#151
-00002ec0: 362c 2023 3135 3238 290a 2a20 5468 6520  6, #1528).* The 
-00002ed0: 6571 7561 6c69 7479 2064 6566 696e 6974  equality definit
-00002ee0: 696f 6e20 6f6e 2060 604f 6273 6572 7665  ion on ``Observe
-00002ef0: 7245 7870 7265 7373 696f 6e60 6020 6861  rExpression`` ha
-00002f00: 7320 6265 656e 2073 696d 706c 6966 6965  s been simplifie
-00002f10: 642e 0a20 2028 2331 3531 3729 0a2a 2054  d..  (#1517).* T
-00002f20: 6865 2060 604f 6273 6572 7665 7245 7870  he ``ObserverExp
-00002f30: 7265 7373 696f 6e60 602c 2060 604f 6273  ression``, ``Obs
-00002f40: 6572 7665 7247 7261 7068 6060 2061 6e64  erverGraph`` and
-00002f50: 2072 656c 6174 6564 0a20 2063 6c61 7373   related.  class
-00002f60: 6573 206e 6f77 2075 7365 2060 605f 5f73  es now use ``__s
-00002f70: 6c6f 7473 5f5f 6060 2074 6f20 696d 7072  lots__`` to impr
-00002f80: 6f76 6520 7370 6565 6420 616e 6420 6d65  ove speed and me
-00002f90: 6d6f 7279 2075 7365 2e20 2823 3135 3133  mory use. (#1513
-00002fa0: 2c20 2331 3531 3529 0a2a 2054 6865 2060  , #1515).* The `
-00002fb0: 606f 6e5f 7472 6169 745f 6368 616e 6765  `on_trait_change
-00002fc0: 6060 206d 6574 686f 6420 6861 7320 6265  `` method has be
-00002fd0: 656e 2073 7065 6420 7570 2062 7920 616c  en sped up by al
-00002fe0: 6d6f 7374 2061 2066 6163 746f 7220 6f66  most a factor of
-00002ff0: 2074 776f 2c0a 2020 6279 2072 656d 6f76   two,.  by remov
-00003000: 696e 6720 756e 6e65 6365 7373 6172 7920  ing unnecessary 
-00003010: 696e 7465 726e 616c 2075 7361 6765 206f  internal usage o
-00003020: 6620 5472 6169 7473 2069 6e20 7468 6520  f Traits in the 
-00003030: 7061 7273 696e 6720 616e 6420 6c69 7374  parsing and list
-00003040: 656e 6572 0a20 2066 756e 6374 696f 6e61  ener.  functiona
-00003050: 6c69 7479 2e20 2823 3134 3930 2c20 2331  lity. (#1490, #1
-00003060: 3439 312c 2023 3134 3932 2c20 2331 3439  491, #1492, #149
-00003070: 3329 0a0a 0a43 6861 6e67 6573 0a7e 7e7e  3)...Changes.~~~
-00003080: 7e7e 7e7e 0a0a 2a20 416e 2069 6e76 616c  ~~~~..* An inval
-00003090: 6964 2073 7461 7469 6320 6465 6661 756c  id static defaul
-000030a0: 7420 7661 6c75 6520 696e 2061 2060 6050  t value in a ``P
-000030b0: 7265 6669 784c 6973 7460 6020 6f72 2060  refixList`` or `
-000030c0: 6050 7265 6669 784d 6170 6060 2074 7261  `PrefixMap`` tra
-000030d0: 6974 0a20 2064 6563 6c61 7261 7469 6f6e  it.  declaration
-000030e0: 206e 6f77 2072 6169 7365 7320 6060 5661   now raises ``Va
-000030f0: 6c75 6545 7272 6f72 6060 2072 6174 6865  lueError`` rathe
-00003100: 7220 7468 616e 2060 6054 7261 6974 4572  r than ``TraitEr
-00003110: 726f 7260 602e 2028 2331 3536 3429 0a2a  ror``. (#1564).*
-00003120: 2060 6050 7265 6669 784c 6973 7460 6020   ``PrefixList`` 
-00003130: 616e 6420 6060 5072 6566 6978 4d61 7060  and ``PrefixMap`
-00003140: 6020 6e6f 206c 6f6e 6765 7220 6361 6368  ` no longer cach
-00003150: 6520 636f 6d70 6c65 7469 6f6e 732e 2028  e completions. (
-00003160: 2331 3536 3429 0a2a 2041 2066 6169 6c75  #1564).* A failu
-00003170: 7265 2074 6f20 7061 7273 6520 616e 2060  re to parse an `
-00003180: 606f 6273 6572 7665 6060 206d 696e 692d  `observe`` mini-
-00003190: 6c61 6e67 7561 6765 2073 7472 696e 6720  language string 
-000031a0: 6e6f 7720 7261 6973 6573 0a20 2060 6056  now raises.  ``V
-000031b0: 616c 7565 4572 726f 7260 6020 7261 7468  alueError`` rath
-000031c0: 6572 2074 6861 6e20 6060 4c61 726b 4572  er than ``LarkEr
-000031d0: 726f 7260 602e 2028 2331 3530 3729 0a2a  ror``. (#1507).*
-000031e0: 2054 6865 2060 604e 6f74 6966 6965 724e   The ``NotifierN
-000031f0: 6f74 466f 756e 6460 6020 6578 6365 7074  otFound`` except
-00003200: 696f 6e20 6973 206e 6f77 2070 7562 6c69  ion is now publi
-00003210: 7368 6564 2069 6e0a 2020 6060 7472 6169  shed in.  ``trai
-00003220: 7473 2e6f 6273 6572 7661 7469 6f6e 2e61  ts.observation.a
-00003230: 7069 6060 2e20 2823 3134 3938 290a 2a20  pi``. (#1498).* 
-00003240: 416e 2061 7474 656d 7074 2074 6f20 6163  An attempt to ac
-00003250: 6365 7373 2061 206e 6f6e 6578 6973 7465  cess a nonexiste
-00003260: 6e74 2022 6475 6e64 6572 2220 6174 7472  nt "dunder" attr
-00003270: 6962 7574 6520 2861 6e20 6174 7472 6962  ibute (an attrib
-00003280: 7574 6520 7768 6f73 650a 2020 6e61 6d65  ute whose.  name
-00003290: 2073 7461 7274 7320 616e 6420 656e 6473   starts and ends
-000032a0: 2077 6974 6820 225f 5f22 2920 6f6e 2061   with "__") on a
-000032b0: 2060 6043 5472 6169 7460 6020 696e 7374   ``CTrait`` inst
-000032c0: 616e 6365 2077 696c 6c20 6e6f 7720 7261  ance will now ra
-000032d0: 6973 650a 2020 6060 4174 7472 6962 7574  ise.  ``Attribut
-000032e0: 6545 7272 6f72 6060 2e20 5072 6576 696f  eError``. Previo
-000032f0: 7573 6c79 2c20 6974 2077 6f75 6c64 2072  usly, it would r
-00003300: 6574 7572 6e20 6060 4e6f 6e65 6060 2e20  eturn ``None``. 
-00003310: 2823 3134 3639 2c20 2331 3437 342c 0a20  (#1469, #1474,. 
-00003320: 2023 3134 3737 290a 0a0a 4465 7072 6563   #1477)...Deprec
-00003330: 6174 696f 6e73 0a7e 7e7e 7e7e 7e7e 7e7e  ations.~~~~~~~~~
-00003340: 7e7e 7e0a 0a2a 2054 6865 2060 6041 6e79  ~~~..* The ``Any
-00003350: 6060 2074 7261 6974 2074 7970 6520 6375  `` trait type cu
-00003360: 7272 656e 746c 7920 696d 706c 6963 6974  rrently implicit
-00003370: 6c79 206d 616b 6573 2061 2070 6572 2d60  ly makes a per-`
-00003380: 6048 6173 5472 6169 7473 6060 2d69 6e73  `HasTraits``-ins
-00003390: 7461 6e63 650a 2020 636f 7079 206f 6620  tance.  copy of 
-000033a0: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
-000033b0: 6520 6966 2074 6861 7420 7661 6c75 6520  e if that value 
-000033c0: 6973 2061 6e20 696e 7374 616e 6365 206f  is an instance o
-000033d0: 6620 6569 7468 6572 2060 606c 6973 7460  f either ``list`
-000033e0: 6020 6f72 0a20 2060 6064 6963 7460 602e  ` or.  ``dict``.
-000033f0: 2054 6869 7320 6265 6861 7669 6f75 7220   This behaviour 
-00003400: 6973 2064 6570 7265 6361 7465 642c 2061  is deprecated, a
-00003410: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
-00003420: 6564 2069 6e20 5472 6169 7473 2037 2e30  ed in Traits 7.0
-00003430: 2e0a 2020 466f 7220 6120 7065 722d 696e  ..  For a per-in
-00003440: 7374 616e 6365 2064 6566 6175 6c74 2c20  stance default, 
-00003450: 7573 6520 7468 6520 6e65 7720 6060 6661  use the new ``fa
-00003460: 6374 6f72 7960 6020 6172 6775 6d65 6e74  ctory`` argument
-00003470: 2074 6f20 6060 416e 7960 600a 2020 696e   to ``Any``.  in
-00003480: 7374 6561 642e 2028 2331 3534 382c 2023  stead. (#1548, #
-00003490: 3135 3332 290a 2a20 5468 6520 6060 4461  1532).* The ``Da
-000034a0: 7465 6060 2c20 6060 4461 7465 7469 6d65  te``, ``Datetime
-000034b0: 6060 2061 6e64 2060 6054 696d 6560 6020  `` and ``Time`` 
-000034c0: 7472 6169 7420 7479 7065 7320 7769 6c6c  trait types will
-000034d0: 206e 6f20 6c6f 6e67 6572 2061 6363 6570   no longer accep
-000034e0: 740a 2020 6060 4e6f 6e65 6060 2061 7320  t.  ``None`` as 
-000034f0: 6120 7661 6c69 6420 7472 6169 7420 7661  a valid trait va
-00003500: 6c75 6520 696e 2074 6865 2066 7574 7572  lue in the futur
-00003510: 652e 2054 6f20 6b65 6570 2074 6865 2065  e. To keep the e
-00003520: 7869 7374 696e 670a 2020 6265 6861 7669  xisting.  behavi
-00003530: 6f75 722c 2075 7365 2074 6865 206e 6577  our, use the new
-00003540: 2060 6061 6c6c 6f77 5f6e 6f6e 6560 6020   ``allow_none`` 
-00003550: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
-00003560: 2074 6f20 7468 6573 6520 7472 6169 7420   to these trait 
-00003570: 7479 7065 732e 0a20 2028 2331 3434 3429  types..  (#1444)
-00003580: 0a2a 2054 6865 2060 6044 6174 6560 6020  .* The ``Date`` 
-00003590: 7472 6169 7420 7479 7065 2077 696c 6c20  trait type will 
-000035a0: 6e6f 206c 6f6e 6765 7220 6163 6365 7074  no longer accept
-000035b0: 2060 6064 6174 6574 696d 6560 6020 696e   ``datetime`` in
-000035c0: 7374 616e 6365 7320 6279 0a20 2064 6566  stances by.  def
-000035d0: 6175 6c74 2069 6e20 7468 6520 6675 7475  ault in the futu
-000035e0: 7265 2e20 546f 206b 6565 7020 7468 6520  re. To keep the 
-000035f0: 6578 6973 7469 6e67 2062 6568 6176 696f  existing behavio
-00003600: 7572 2c20 7573 6520 7468 6520 6e65 770a  ur, use the new.
-00003610: 2020 6060 616c 6c6f 775f 6461 7465 7469    ``allow_dateti
-00003620: 6d65 6060 206b 6579 776f 7264 2061 7267  me`` keyword arg
-00003630: 756d 656e 742e 2028 2331 3434 3129 0a2a  ument. (#1441).*
-00003640: 2054 6865 2060 6053 796d 626f 6c60 6020   The ``Symbol`` 
-00003650: 7472 6169 7420 7479 7065 2069 7320 6465  trait type is de
-00003660: 7072 6563 6174 6564 2e20 466f 7220 7265  precated. For re
-00003670: 736f 6c75 7469 6f6e 206f 6620 6120 7374  solution of a st
-00003680: 7269 6e67 0a20 2072 6570 7265 7365 6e74  ring.  represent
-00003690: 696e 6720 6120 7061 636b 6167 652f 6d6f  ing a package/mo
-000036a0: 6475 6c65 2f6f 626a 6563 7420 636f 6d62  dule/object comb
-000036b0: 696e 6174 696f 6e2c 2075 7365 2060 6069  ination, use ``i
-000036c0: 6d70 6f72 745f 7379 6d62 6f6c 6060 0a20  mport_symbol``. 
-000036d0: 2069 6e73 7465 6164 2e20 2823 3135 3432   instead. (#1542
-000036e0: 290a 2a20 5468 6520 6060 4d65 7461 4861  ).* The ``MetaHa
-000036f0: 7354 7261 6974 732e 6164 645f 6c69 7374  sTraits.add_list
-00003700: 656e 6572 6060 2061 6e64 2060 604d 6574  ener`` and ``Met
-00003710: 6148 6173 5472 6169 7473 2e72 656d 6f76  aHasTraits.remov
-00003720: 655f 6c69 7374 656e 6572 6060 0a20 206d  e_listener``.  m
-00003730: 6574 686f 6473 2061 7265 2064 6570 7265  ethods are depre
-00003740: 6361 7465 642e 2028 2331 3535 3029 0a2a  cated. (#1550).*
-00003750: 2054 6865 2060 6063 6c65 616e 5f66 696c   The ``clean_fil
-00003760: 656e 616d 6560 6020 616e 6420 6060 636c  ename`` and ``cl
-00003770: 6561 6e5f 7469 6d65 7374 616d 7060 6020  ean_timestamp`` 
-00003780: 7574 696c 6974 6965 7320 6172 6520 6465  utilities are de
-00003790: 7072 6563 6174 6564 2e20 4966 0a20 2079  precated. If.  y
-000037a0: 6f75 206e 6565 6420 7468 6573 6520 7574  ou need these ut
-000037b0: 696c 6974 6965 7320 696e 2079 6f75 7220  ilities in your 
-000037c0: 6f77 6e20 7072 6f6a 6563 742c 2079 6f75  own project, you
-000037d0: 2772 6520 6164 7669 7365 6420 746f 2063  're advised to c
-000037e0: 6f70 7920 7468 650a 2020 636f 6465 2064  opy the.  code d
-000037f0: 6972 6563 746c 7920 696e 746f 2079 6f75  irectly into you
-00003800: 7220 7072 6f6a 6563 742e 2028 2331 3532  r project. (#152
-00003810: 3729 0a2a 2054 6865 2060 6066 696e 645f  7).* The ``find_
-00003820: 7265 736f 7572 6365 6060 2061 6e64 2060  resource`` and `
-00003830: 6073 746f 7265 5f72 6573 6f75 7263 6560  `store_resource`
-00003840: 6020 6675 6e63 7469 6f6e 7320 6172 6520  ` functions are 
-00003850: 6465 7072 6563 6174 6564 2e20 4e65 770a  deprecated. New.
-00003860: 2020 636f 6465 2073 686f 756c 6420 7573    code should us
-00003870: 6520 6060 696d 706f 7274 6c69 622e 7265  e ``importlib.re
-00003880: 736f 7572 6365 7360 6020 6f72 2060 6069  sources`` or ``i
-00003890: 6d70 6f72 746c 6962 5f72 6573 6f75 7263  mportlib_resourc
-000038a0: 6573 6060 2069 6e73 7465 6164 0a20 206f  es`` instead.  o
-000038b0: 6620 6569 7468 6572 206f 6620 7468 6573  f either of thes
-000038c0: 6520 6675 6e63 7469 6f6e 732e 2028 2331  e functions. (#1
-000038d0: 3530 3129 0a0a 0a46 6978 6573 0a7e 7e7e  501)...Fixes.~~~
-000038e0: 7e7e 0a0a 2a20 496e 7661 6c69 6420 6173  ~~..* Invalid as
-000038f0: 7369 676e 6d65 6e74 7320 746f 2060 6050  signments to ``P
-00003900: 7265 6669 784c 6973 7460 6020 616e 6420  refixList`` and 
-00003910: 6060 5072 6566 6978 4d61 7060 6020 7472  ``PrefixMap`` tr
-00003920: 6169 7473 2070 726f 6475 6365 640a 2020  aits produced.  
-00003930: 616e 2075 6e6e 6563 6573 7361 7269 6c79  an unnecessarily
-00003940: 206e 6573 7465 6420 6578 6365 7074 696f   nested exceptio
-00003950: 6e2e 2054 6869 7320 6861 7320 6265 656e  n. This has been
-00003960: 2066 6978 6564 2e20 2823 3135 3634 290a   fixed. (#1564).
-00003970: 2a20 416e 2060 606f 6273 6572 7665 6060  * An ``observe``
-00003980: 2d64 6563 6f72 6174 6564 206c 6973 7465  -decorated liste
-00003990: 6e65 7220 6d65 7468 6f64 2077 686f 7365  ner method whose
-000039a0: 206e 616d 6520 6861 7320 7468 6520 7370   name has the sp
-000039b0: 6563 6961 6c20 666f 726d 0a20 2060 6022  ecial form.  ``"
-000039c0: 5f74 7261 6974 6e61 6d65 5f63 6861 6e67  _traitname_chang
-000039d0: 6564 2260 6020 7769 6c6c 206e 6f20 6c6f  ed"`` will no lo
-000039e0: 6e67 6572 2062 6520 7472 6967 6765 7265  nger be triggere
-000039f0: 6420 626f 7468 2061 7320 6173 2072 6573  d both as as res
-00003a00: 756c 740a 2020 6f66 2074 6865 2060 606f  ult.  of the ``o
-00003a10: 6273 6572 7665 6060 2064 6563 6f72 6174  bserve`` decorat
-00003a20: 6f72 202a 616e 642a 2074 6865 2073 7065  or *and* the spe
-00003a30: 6369 616c 206e 616d 696e 673a 2069 7420  cial naming: it 
-00003a40: 7769 6c6c 206f 6e6c 7920 6265 0a20 2074  will only be.  t
-00003a50: 7269 6767 6572 6564 2076 6961 2074 6865  riggered via the
-00003a60: 2060 606f 6273 6572 7665 6060 2064 6563   ``observe`` dec
-00003a70: 6f72 6174 6f72 2e20 2823 3135 3630 290a  orator. (#1560).
-00003a80: 2a20 5468 6520 6060 6465 6c65 6761 7465  * The ``delegate
-00003a90: 6060 2070 6172 616d 6574 6572 2077 6173  `` parameter was
-00003aa0: 206d 6973 7479 7065 6420 696e 2074 6865   mistyped in the
-00003ab0: 2074 7970 696e 6720 7374 7562 7320 666f   typing stubs fo
-00003ac0: 7220 7468 650a 2020 6060 4465 6c65 6761  r the.  ``Delega
-00003ad0: 7465 6060 2074 7261 6974 2074 7970 652e  te`` trait type.
-00003ae0: 2054 6869 7320 6861 7320 6265 656e 2066   This has been f
-00003af0: 6978 6564 2e20 2823 3135 3536 290a 2a20  ixed. (#1556).* 
-00003b00: 5468 6520 6060 4675 6e63 7469 6f6e 6060  The ``Function``
-00003b10: 2061 6e64 2060 604d 6574 686f 6460 6020   and ``Method`` 
-00003b20: 7472 6169 7420 7479 7065 7320 7769 6c6c  trait types will
-00003b30: 206e 6f20 6c6f 6e67 6572 2066 6169 6c20   no longer fail 
-00003b40: 7768 656e 0a20 2061 7267 756d 656e 7473  when.  arguments
-00003b50: 2061 7265 2070 6173 7365 642e 204e 6f74   are passed. Not
-00003b60: 6520 7468 6174 2074 6865 7365 2074 7261  e that these tra
-00003b70: 6974 2074 7970 6573 2061 7265 2061 6c72  it types are alr
-00003b80: 6561 6479 2064 6570 7265 6361 7465 642c  eady deprecated,
-00003b90: 2061 6e64 0a20 2073 686f 756c 6420 6e6f   and.  should no
-00003ba0: 7420 6265 2075 7365 6420 696e 206e 6577  t be used in new
-00003bb0: 2063 6f64 652e 2028 2331 3534 3329 0a2a   code. (#1543).*
-00003bc0: 2049 6e6e 6572 2074 7261 6974 7320 6f66   Inner traits of
-00003bd0: 2061 2060 6055 6e69 6f6e 6060 2074 7261   a ``Union`` tra
-00003be0: 6974 2061 7265 206e 6f77 2076 616c 6964  it are now valid
-00003bf0: 6174 6564 2070 726f 7065 726c 792e 2050  ated properly. P
-00003c00: 7265 7669 6f75 736c 792c 2069 6e0a 2020  reviously, in.  
-00003c10: 7472 6169 7420 6465 636c 6172 6174 696f  trait declaratio
-00003c20: 6e73 206c 696b 6520 6060 666f 6f20 3d20  ns like ``foo = 
-00003c30: 556e 696f 6e28 4c69 7374 2849 6e74 292c  Union(List(Int),
-00003c40: 2053 7472 2960 602c 2074 6865 206c 6973   Str)``, the lis
-00003c50: 7420 656e 7472 6965 730a 2020 776f 756c  t entries.  woul
-00003c60: 6420 6e6f 7420 6265 2076 616c 6964 6174  d not be validat
-00003c70: 6564 2e20 2823 3135 3232 2c20 2331 3533  ed. (#1522, #153
-00003c80: 3429 0a2a 2054 7261 6974 7320 7769 7468  4).* Traits with
-00003c90: 2061 2064 796e 616d 6963 2064 6566 6175   a dynamic defau
-00003ca0: 6c74 2074 6861 7420 6170 7065 6172 2061  lt that appear a
-00003cb0: 7320 696e 6e65 7220 7472 6169 7473 206f  s inner traits o
-00003cc0: 6620 6120 6060 5475 706c 6560 600a 2020  f a ``Tuple``.  
-00003cd0: 7472 6169 7420 6172 6520 6e6f 7720 7661  trait are now va
-00003ce0: 6c69 6461 7465 6420 7072 6f70 6572 6c79  lidated properly
-00003cf0: 2e20 2823 3135 3231 290a 2a20 4120 706f  . (#1521).* A po
-00003d00: 7465 6e74 6961 6c20 7261 6365 2063 6f6e  tential race con
-00003d10: 6469 7469 6f6e 2069 6e20 6060 4c69 7374  dition in ``List
-00003d20: 656e 6572 4861 6e64 6c65 7260 6020 6861  enerHandler`` ha
-00003d30: 7320 6265 656e 2066 6978 6564 2e20 5468  s been fixed. Th
-00003d40: 650a 2020 7261 6365 2063 6f6e 6469 7469  e.  race conditi
-00003d50: 6f6e 2069 7320 6861 7264 2074 6f20 6578  on is hard to ex
-00003d60: 6572 6369 7365 2061 6e64 2068 6173 206e  ercise and has n
-00003d70: 6f74 2062 6565 6e20 7769 746e 6573 7365  ot been witnesse
-00003d80: 6420 696e 2074 6865 2077 696c 642e 0a20  d in the wild.. 
-00003d90: 2028 2331 3439 3529 0a2a 2055 7365 206f   (#1495).* Use o
-00003da0: 6620 6060 6164 645f 636c 6173 735f 7472  f ``add_class_tr
-00003db0: 6169 7460 6020 746f 2061 6464 2061 2060  ait`` to add a `
-00003dc0: 604c 6973 7460 6020 7472 6169 7420 7761  `List`` trait wa
-00003dd0: 7320 6272 6f6b 656e 2069 6e20 7468 6520  s broken in the 
-00003de0: 7072 6573 656e 6365 0a20 206f 6620 7375  presence.  of su
-00003df0: 6263 6c61 7373 6573 2e20 5468 6973 2068  bclasses. This h
-00003e00: 6173 2062 6565 6e20 6669 7865 642e 2028  as been fixed. (
-00003e10: 2331 3436 3129 0a2a 2041 2075 7365 206f  #1461).* A use o
-00003e20: 6620 7468 6520 2864 6570 7265 6361 7465  f the (deprecate
-00003e30: 6429 2060 6064 6973 7475 7469 6c73 6060  d) ``distutils``
-00003e40: 206c 6962 7261 7279 2068 6173 2062 6565   library has bee
-00003e50: 6e20 7265 706c 6163 6564 2077 6974 680a  n replaced with.
-00003e60: 2020 6060 7379 7363 6f6e 6669 6760 602e    ``sysconfig``.
-00003e70: 2028 2331 3435 3229 0a2a 2044 796e 616d   (#1452).* Dynam
-00003e80: 6963 2064 6566 6175 6c74 2068 616e 6469  ic default handi
-00003e90: 6e67 2068 6173 2062 6565 6e20 6669 7865  ng has been fixe
-00003ea0: 6420 696e 2074 6865 2060 605f 696e 7374  d in the ``_inst
-00003eb0: 616e 6365 5f68 616e 646c 6572 5f66 6163  ance_handler_fac
-00003ec0: 746f 7279 6060 0a20 2075 7365 6420 6279  tory``.  used by
-00003ed0: 2074 6865 2054 7261 6974 7355 4920 6060   the TraitsUI ``
-00003ee0: 5461 626c 6545 6469 746f 7260 602e 2028  TableEditor``. (
-00003ef0: 2331 3434 362c 2023 3134 3530 290a 2a20  #1446, #1450).* 
-00003f00: 5468 6520 7472 6169 7420 6465 7363 7269  The trait descri
-00003f10: 7074 696f 6e73 2028 7468 6520 2269 6e66  ptions (the "inf
-00003f20: 6f22 2074 6578 7429 2066 6f72 2074 6865  o" text) for the
-00003f30: 2060 6046 696c 6560 6020 616e 6420 6060   ``File`` and ``
-00003f40: 4469 7265 6374 6f72 7960 600a 2020 7472  Directory``.  tr
-00003f50: 6169 7473 2068 6176 6520 6265 656e 2066  aits have been f
-00003f60: 6978 6564 2074 6f20 6176 6f69 6420 6769  ixed to avoid gi
-00003f70: 7669 6e67 2061 206d 6973 6c65 6164 696e  ving a misleadin
-00003f80: 6720 6572 726f 7220 6d65 7373 6167 6520  g error message 
-00003f90: 7768 656e 0a20 2060 6065 7869 7374 733d  when.  ``exists=
-00003fa0: 5472 7565 6060 2e20 2823 3134 3430 290a  True``. (#1440).
-00003fb0: 2a20 436c 6f6e 6573 206f 6620 6060 4261  * Clones of ``Ba
-00003fc0: 7365 496e 7374 616e 6365 6060 2074 7261  seInstance`` tra
-00003fd0: 6974 7320 6469 646e 2774 2063 6f72 7265  its didn't corre
-00003fe0: 6374 6c79 2072 6573 7065 6374 2074 6865  ctly respect the
-00003ff0: 2060 6061 6c6c 6f77 5f6e 6f6e 6560 600a   ``allow_none``.
-00004000: 2020 7061 7261 6d65 7465 722e 2054 6869    parameter. Thi
-00004010: 7320 6973 206e 6f77 2066 6978 6564 2e20  s is now fixed. 
-00004020: 2823 3134 3333 290a 2a20 416e 206f 7574  (#1433).* An out
-00004030: 6461 7465 6420 7265 6665 7265 6e63 6520  dated reference 
-00004040: 746f 2074 6865 2022 7079 676c 6574 2220  to the "pyglet" 
-00004050: 4b69 7661 2062 6163 6b65 6e64 2068 6173  Kiva backend has
-00004060: 2062 6565 6e20 7265 6d6f 7665 642e 2028   been removed. (
-00004070: 2331 3433 3129 0a0a 0a44 6f63 756d 656e  #1431)...Documen
-00004080: 7461 7469 6f6e 0a7e 7e7e 7e7e 7e7e 7e7e  tation.~~~~~~~~~
-00004090: 7e7e 7e7e 0a0a 2a20 4272 6965 6620 696e  ~~~~..* Brief in
-000040a0: 7374 616c 6c61 7469 6f6e 2064 6f63 7320  stallation docs 
-000040b0: 6861 7665 2062 6565 6e20 6164 6465 642e  have been added.
-000040c0: 2028 2331 3535 3929 0a2a 204f 6363 7572   (#1559).* Occur
-000040d0: 7265 6e63 6573 206f 6620 6060 416e 7928  rences of ``Any(
-000040e0: 736f 6d65 5f6c 6973 7429 6060 2069 6e20  some_list)`` in 
-000040f0: 646f 6373 2068 6176 6520 6265 656e 2072  docs have been r
-00004100: 6570 6c61 6365 642e 2028 2331 3534 3729  eplaced. (#1547)
-00004110: 0a2a 2054 6865 2064 6f63 756d 656e 7461  .* The documenta
-00004120: 7469 6f6e 2066 6f72 2060 6073 796e 635f  tion for ``sync_
-00004130: 7472 6169 7460 6020 6861 7320 6265 656e  trait`` has been
-00004140: 2075 7064 6174 6564 2074 6f20 6e6f 7465   updated to note
-00004150: 2074 6861 7420 6974 206f 6e6c 790a 2020   that it only.  
-00004160: 7379 6e63 6872 6f6e 6973 6573 2069 7465  synchronises ite
-00004170: 6d73 2066 6f72 2060 604c 6973 7460 6020  ms for ``List`` 
-00004180: 7472 6169 7473 2c20 6e6f 7420 666f 7220  traits, not for 
-00004190: 6060 4469 6374 6060 2061 6e64 2060 6053  ``Dict`` and ``S
-000041a0: 6574 6060 2074 7261 6974 732e 0a20 2028  et`` traits..  (
-000041b0: 2331 3531 3929 0a2a 2041 2063 6f6e 6669  #1519).* A confi
-000041c0: 6775 7261 7469 6f6e 2066 696c 6520 666f  guration file fo
-000041d0: 7220 5265 6164 2074 6865 2044 6f63 7320  r Read the Docs 
-000041e0: 6861 7320 6265 656e 2061 6464 6564 2e20  has been added. 
-000041f0: 2823 3134 3738 290a 2a20 4120 6060 4465  (#1478).* A ``De
-00004200: 7072 6563 6174 696f 6e57 6172 6e69 6e67  precationWarning
-00004210: 6060 2061 7269 7369 6e67 2066 726f 6d20  `` arising from 
-00004220: 616e 2075 6e6e 6563 6573 7361 7279 206f  an unnecessary o
-00004230: 7665 7272 6964 6520 6f66 2074 6865 0a20  verride of the. 
-00004240: 2060 6061 6464 5f63 6f6e 7465 6e74 6060   ``add_content``
-00004250: 206d 6574 686f 6420 696e 2074 6865 2060   method in the `
-00004260: 6054 7261 6974 446f 6375 6d65 6e74 6572  `TraitDocumenter
-00004270: 6060 2068 6173 2062 6565 6e20 6669 7865  `` has been fixe
-00004280: 642e 2028 2331 3437 3529 0a2a 2054 6865  d. (#1475).* The
-00004290: 2053 7068 696e 7820 7665 7273 696f 6e20   Sphinx version 
-000042a0: 7761 7320 7465 6d70 6f72 6172 696c 7920  was temporarily 
-000042b0: 7069 6e6e 6564 2074 6f20 6176 6f69 6420  pinned to avoid 
-000042c0: 6275 696c 6420 6661 696c 7572 6573 2061  build failures a
-000042d0: 7269 7369 6e67 0a20 2066 726f 6d20 6275  rising.  from bu
-000042e0: 6773 2069 6e20 5370 6869 6e78 2034 2e30  gs in Sphinx 4.0
-000042f0: 2e31 2e20 5468 6174 2070 696e 2068 6173  .1. That pin has
-00004300: 2073 696e 6365 2062 6565 6e20 7265 7665   since been reve
-00004310: 7274 6564 2e0a 2020 2823 3134 3731 2c20  rted..  (#1471, 
-00004320: 2331 3436 3229 0a2a 2056 6172 696f 7573  #1462).* Various
-00004330: 2064 6f63 7374 7269 6e67 2066 6978 6573   docstring fixes
-00004340: 2068 6176 6520 6265 656e 2061 7070 6c69   have been appli
-00004350: 6564 2e20 2823 3134 3638 2c20 2331 3436  ed. (#1468, #146
-00004360: 3529 0a2a 2056 6172 696f 7573 2074 7970  5).* Various typ
-00004370: 6f20 6669 7865 7320 6861 7665 2062 6565  o fixes have bee
-00004380: 6e20 6170 706c 6965 642e 2028 2331 3435  n applied. (#145
-00004390: 382c 2023 3134 3432 290a 2a20 5265 6665  8, #1442).* Refe
-000043a0: 7265 6e63 6573 2074 6f20 6060 4861 7354  rences to ``HasT
-000043b0: 7261 6974 732e 7365 7460 6020 6861 7665  raits.set`` have
-000043c0: 2062 6565 6e20 7265 706c 6163 6564 2077   been replaced w
-000043d0: 6974 680a 2020 6060 4861 7354 7261 6974  ith.  ``HasTrait
-000043e0: 732e 7472 6169 745f 7365 7460 602e 2028  s.trait_set``. (
-000043f0: 2331 3435 3129 0a2a 2053 6f6d 6520 6973  #1451).* Some is
-00004400: 7375 6573 2077 6974 6820 7468 6520 7475  sues with the tu
-00004410: 746f 7269 616c 2043 5353 2075 7365 6420  torial CSS used 
-00004420: 696e 2074 6865 2045 5453 2064 656d 6f20  in the ETS demo 
-00004430: 6170 706c 6963 6174 696f 6e20 6861 7665  application have
-00004440: 2062 6565 6e0a 2020 6669 7865 643b 2074   been.  fixed; t
-00004450: 6865 2063 6f6c 6f75 7220 7363 6865 6d65  he colour scheme
-00004460: 2068 6173 2062 6565 6e20 6368 616e 6765   has been change
-00004470: 6420 746f 2045 6e74 686f 7567 6874 2063  d to Enthought c
-00004480: 6f6c 6f75 7273 2e20 2823 3134 3231 2c0a  olours. (#1421,.
-00004490: 2020 2331 3431 3929 0a0a 0a43 6c65 616e    #1419)...Clean
-000044a0: 7570 2061 6e64 2072 6566 6163 746f 7269  up and refactori
-000044b0: 6e67 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ng.~~~~~~~~~~~~~
-000044c0: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20 416c  ~~~~~~~~~~..* Al
-000044d0: 6c20 6275 696c 742d 696e 2054 7261 6974  l built-in Trait
-000044e0: 5479 7065 2073 7562 636c 6173 7365 7320  Type subclasses 
-000044f0: 6e6f 7720 7072 6f76 6964 6520 7468 6520  now provide the 
-00004500: 6465 6661 756c 7420 7661 6c75 6520 7479  default value ty
-00004510: 7065 2064 6972 6563 746c 790a 2020 7261  pe directly.  ra
-00004520: 7468 6572 2074 6861 6e20 696e 6665 7272  ther than inferr
-00004530: 696e 6720 6974 2e20 2823 3135 3535 2c20  ing it. (#1555, 
-00004540: 2331 3533 362c 2023 3135 3331 2c20 2331  #1536, #1531, #1
-00004550: 3533 392c 2023 3135 3332 2c20 2331 3534  539, #1532, #154
-00004560: 3029 0a2a 2054 6865 2060 6074 7261 6974  0).* The ``trait
-00004570: 5f61 6464 6564 6060 2061 6e64 2060 6074  _added`` and ``t
-00004580: 7261 6974 5f6d 6f64 6966 6965 6460 6020  rait_modified`` 
-00004590: 7472 6169 7473 206f 6e20 6060 4861 7354  traits on ``HasT
-000045a0: 7261 6974 7360 6020 6e6f 770a 2020 6861  raits`` now.  ha
-000045b0: 7665 2070 726f 7065 7220 7472 6169 7420  ve proper trait 
-000045c0: 7479 7065 2064 6563 6c61 7261 7469 6f6e  type declaration
-000045d0: 732e 2028 2331 3535 3229 0a2a 2052 6564  s. (#1552).* Red
-000045e0: 756e 6461 6e74 2060 6075 6e69 7474 6573  undant ``unittes
-000045f0: 742e 6d61 696e 2062 6c6f 636b 7360 6020  t.main blocks`` 
-00004600: 6861 7665 2062 6565 6e20 7265 6d6f 7665  have been remove
-00004610: 642e 2028 2331 3534 3529 0a2a 2053 7479  d. (#1545).* Sty
-00004620: 6c65 2066 6978 6573 2068 6176 6520 6265  le fixes have be
-00004630: 656e 2061 7070 6c69 6564 2074 6f20 6060  en applied to ``
-00004640: 7472 6169 745f 7479 7065 732e 7079 6960  trait_types.pyi`
-00004650: 602e 2028 2331 3532 3329 0a2a 2060 604f  `. (#1523).* ``O
-00004660: 6273 6572 7665 7245 7870 7265 7373 696f  bserverExpressio
-00004670: 6e60 6020 616e 6420 6f74 6865 7220 6b65  n`` and other ke
-00004680: 7920 6f62 7365 7276 6174 696f 6e20 636c  y observation cl
-00004690: 6173 7365 7320 6e6f 7720 6861 7665 206d  asses now have m
-000046a0: 6f72 650a 2020 6465 6275 672d 6672 6965  ore.  debug-frie
-000046b0: 6e64 6c79 2060 6072 6570 7260 6020 696d  ndly ``repr`` im
-000046c0: 706c 656d 656e 7461 7469 6f6e 732e 2028  plementations. (
-000046d0: 2331 3531 3429 0a2a 2054 6865 2060 606f  #1514).* The ``o
-000046e0: 6273 6572 7665 7260 6020 7061 7273 696e  bserver`` parsin
-000046f0: 6720 696e 7465 726e 616c 7320 6861 7665  g internals have
-00004700: 2062 6565 6e20 7265 776f 726b 6564 2074   been reworked t
-00004710: 6f20 6d61 6b65 0a20 2060 604f 6273 6572  o make.  ``Obser
-00004720: 7665 7247 7261 7068 6060 2074 6865 206b  verGraph`` the k
-00004730: 6579 2022 636f 6d70 696c 6564 2220 6f62  ey "compiled" ob
-00004740: 6a65 6374 2074 6861 7420 7468 6520 7265  ject that the re
-00004750: 7374 206f 6620 5472 6169 7473 2063 6172  st of Traits car
-00004760: 6573 0a20 2061 626f 7574 2c20 7261 7468  es.  about, rath
-00004770: 6572 2074 6861 6e20 6060 4f62 7365 7276  er than ``Observ
-00004780: 6572 4578 7072 6573 7369 6f6e 6060 2e20  erExpression``. 
-00004790: 2823 3135 3132 290a 2a20 5468 6520 6772  (#1512).* The gr
-000047a0: 616d 6d61 7220 616e 6420 7061 7273 6572  ammar and parser
-000047b0: 2066 6f72 2074 6865 206f 6273 6572 7665   for the observe
-000047c0: 206d 696e 692d 6c61 6e67 7561 6765 2068   mini-language h
-000047d0: 6176 6520 6265 656e 2073 696d 706c 6966  ave been simplif
-000047e0: 6965 642e 0a20 2028 2331 3530 3629 0a2a  ied..  (#1506).*
-000047f0: 2043 6f6e 6675 7369 6f6e 2062 6574 7765   Confusion betwe
-00004800: 656e 2022 616e 795f 7472 6169 7422 2061  en "any_trait" a
-00004810: 6e64 2022 616e 7974 7261 6974 2220 696e  nd "anytrait" in
-00004820: 206e 6f6e 2d75 7365 722d 6661 6369 6e67   non-user-facing
-00004830: 0a20 2066 756e 6374 696f 6e73 2061 6e64  .  functions and
-00004840: 2063 6c61 7373 6573 2068 6173 2062 6565   classes has bee
-00004850: 6e20 636c 6561 6e65 6420 7570 2e20 2823  n cleaned up. (#
-00004860: 3134 3937 290a 2a20 556e 6e65 6365 7373  1497).* Unnecess
-00004870: 6172 7920 6060 6e6f 7161 6060 206d 6172  ary ``noqa`` mar
-00004880: 6b65 7273 2068 6176 6520 6265 656e 2072  kers have been r
-00004890: 656d 6f76 6564 2e20 2823 3134 3939 290a  emoved. (#1499).
-000048a0: 2a20 4120 7573 6520 6f66 2074 6865 2060  * A use of the `
-000048b0: 6070 726f 7065 7274 7960 6020 6361 6c6c  `property`` call
-000048c0: 6162 6c65 2068 6173 2062 6565 6e20 7265  able has been re
-000048d0: 706c 6163 6564 2077 6974 6820 6120 6060  placed with a ``
-000048e0: 7072 6f70 6572 7479 6060 0a20 2064 6563  property``.  dec
-000048f0: 6f72 6174 6f72 2e20 2823 3134 3730 290a  orator. (#1470).
-00004900: 2a20 4120 6261 6420 6f62 7365 7276 652d  * A bad observe-
-00004910: 6465 636f 7261 7465 6420 6c69 7374 656e  decorated listen
-00004920: 6572 2073 6967 6e61 7475 7265 2069 6e20  er signature in 
-00004930: 6120 7465 7374 2068 6173 2062 6565 6e20  a test has been 
-00004940: 6669 7865 642e 2028 2331 3533 3029 0a0a  fixed. (#1530)..
-00004950: 0a42 7569 6c64 2061 6e64 2064 6576 656c  .Build and devel
-00004960: 6f70 6d65 6e74 2077 6f72 6b66 6c6f 770a  opment workflow.
-00004970: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00004980: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a  ~~~~~~~~~~~~~~..
-00004990: 2a20 5079 7468 6f6e 2033 2e31 3020 6973  * Python 3.10 is
-000049a0: 2073 7570 706f 7274 6564 2061 6e64 2074   supported and t
-000049b0: 6573 7465 642c 2061 6e64 2077 6865 656c  ested, and wheel
-000049c0: 7320 6172 6520 6275 696c 7420 666f 7220  s are built for 
-000049d0: 5079 7468 6f6e 2033 2e31 302e 0a20 2028  Python 3.10..  (
-000049e0: 2331 3432 352c 2023 3135 3637 2c20 2331  #1425, #1567, #1
-000049f0: 3536 392c 2023 3135 3731 290a 2a20 5768  569, #1571).* Wh
-00004a00: 6565 6c73 2061 7265 206e 6f77 2062 7569  eels are now bui
-00004a10: 6c74 2066 6f72 204c 696e 7578 2f61 6172  lt for Linux/aar
-00004a20: 6368 3634 2e20 2823 3135 3637 290a 2a20  ch64. (#1567).* 
-00004a30: 556e 6976 6572 7361 6c20 7768 6565 6c73  Universal wheels
-00004a40: 2061 7265 206e 6f77 2062 7569 6c74 2066   are now built f
-00004a50: 6f72 206d 6163 4f53 2c20 746f 2073 7570  or macOS, to sup
-00004a60: 706f 7274 2041 7070 6c65 2053 696c 6963  port Apple Silic
-00004a70: 6f6e 2e20 2823 3135 3637 290a 2a20 4372  on. (#1567).* Cr
-00004a80: 6f6e 206a 6f62 7320 6e6f 7720 7365 6e64  on jobs now send
-00004a90: 2066 6169 6c75 7265 2f73 7563 6365 7373   failure/success
-00004aa0: 2053 6c61 636b 206e 6f74 6966 6963 6174   Slack notificat
-00004ab0: 696f 6e73 2074 6f20 456e 7468 6f75 6768  ions to Enthough
-00004ac0: 7427 730a 2020 696e 7465 726e 616c 2063  t's.  internal c
-00004ad0: 6861 6e6e 656c 2e20 2823 3134 3831 290a  hannel. (#1481).
-00004ae0: 2a20 416c 6c20 6372 6f6e 206a 6f62 7320  * All cron jobs 
-00004af0: 6e6f 7720 696e 636c 7564 6520 6120 6060  now include a ``
-00004b00: 776f 726b 666c 6f77 5f64 6973 7061 7463  workflow_dispatc
-00004b10: 6860 6020 7472 6967 6765 722e 2028 2331  h`` trigger. (#1
-00004b20: 3438 3029 0a2a 2054 6865 206d 6169 6e20  480).* The main 
-00004b30: 6465 7665 6c6f 706d 656e 7420 6272 616e  development bran
-00004b40: 6368 2069 7320 6e6f 7720 6361 6c6c 6564  ch is now called
-00004b50: 2022 6d61 696e 2220 7261 7468 6572 2074   "main" rather t
-00004b60: 6861 6e20 226d 6173 7465 7222 2e0a 2020  han "master"..  
-00004b70: 2823 3134 3637 290a 2a20 4175 746f 6d61  (#1467).* Automa
-00004b80: 7465 6420 7465 7374 7320 6861 7665 2062  ted tests have b
-00004b90: 6565 6e20 6164 6465 6420 666f 7220 5079  een added for Py
-00004ba0: 5049 2077 6865 656c 732e 2028 2331 3431  PI wheels. (#141
-00004bb0: 3729 0a0a 0a52 656c 6561 7365 2036 2e32  7)...Release 6.2
-00004bc0: 2e30 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .0.-------------
-00004bd0: 0a0a 5265 6c65 6173 6564 3a20 3230 3231  ..Released: 2021
-00004be0: 2d30 312d 3231 0a0a 5468 6520 5472 6169  -01-21..The Trai
-00004bf0: 7473 206c 6962 7261 7279 2069 7320 6120  ts library is a 
-00004c00: 666f 756e 6461 7469 6f6e 616c 2063 6f6d  foundational com
-00004c10: 706f 6e65 6e74 206f 6620 7468 6520 456e  ponent of the En
-00004c20: 7468 6f75 6768 7420 546f 6f6c 2053 7569  thought Tool Sui
-00004c30: 7465 2e20 4974 0a70 726f 7669 6465 7320  te. It.provides 
-00004c40: 6f62 7365 7276 6162 6c65 2c20 7479 7065  observable, type
-00004c50: 6420 6174 7472 6962 7574 6573 2066 6f72  d attributes for
-00004c60: 2050 7974 686f 6e20 636c 6173 7365 732c   Python classes,
-00004c70: 206d 616b 696e 6720 7468 6f73 6520 636c   making those cl
-00004c80: 6173 7365 730a 7375 6974 6162 6c65 2066  asses.suitable f
-00004c90: 6f72 2065 7665 6e74 2d64 7269 7665 6e20  or event-driven 
-00004ca0: 6461 7461 666c 6f77 2070 726f 6772 616d  dataflow program
-00004cb0: 6d69 6e67 2061 6e64 2066 6f72 2069 6d6d  ming and for imm
-00004cc0: 6564 6961 7465 2075 7365 2061 7320 6d6f  ediate use as mo
-00004cd0: 6465 6c73 0a66 6f72 2067 7261 7068 6963  dels.for graphic
-00004ce0: 616c 2075 7365 7220 696e 7465 7266 6163  al user interfac
-00004cf0: 6573 2c20 6c69 6b65 2074 686f 7365 2070  es, like those p
-00004d00: 726f 7669 6465 6420 6279 2074 6865 2054  rovided by the T
-00004d10: 7261 6974 7355 4920 6c69 6272 6172 792e  raitsUI library.
-00004d20: 0a0a 5472 6169 7473 2036 2e32 2069 7320  ..Traits 6.2 is 
-00004d30: 7468 6520 6c61 7465 7374 2066 6561 7475  the latest featu
-00004d40: 7265 2072 656c 6561 7365 2069 6e20 7468  re release in th
-00004d50: 6520 5472 6169 7473 2036 2073 6572 6965  e Traits 6 serie
-00004d60: 732c 2077 6974 6820 7365 7665 7261 6c0a  s, with several.
-00004d70: 696d 7072 6f76 656d 656e 7473 2061 6e64  improvements and
-00004d80: 2066 6978 6573 206f 7665 7220 5472 6169   fixes over Trai
-00004d90: 7473 2036 2e31 2e0a 0a48 6967 686c 6967  ts 6.1...Highlig
-00004da0: 6874 7320 6f66 2074 6869 7320 7265 6c65  hts of this rele
-00004db0: 6173 650a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ase.~~~~~~~~~~~~
-00004dc0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a  ~~~~~~~~~~~~~~..
-00004dd0: 2a20 5468 6520 5472 6169 7473 2065 7861  * The Traits exa
-00004de0: 6d70 6c65 7320 6172 6520 6e6f 7720 6469  mples are now di
-00004df0: 7374 7269 6275 7465 6420 6173 2070 6172  stributed as par
-00004e00: 7420 6f66 2074 6865 2054 7261 6974 7320  t of the Traits 
-00004e10: 6567 672c 2061 6e64 0a20 2061 7265 2063  egg, and.  are c
-00004e20: 6f6e 7472 6962 7574 6564 2074 6f20 7468  ontributed to th
-00004e30: 6520 6060 6574 7364 656d 6f60 6020 6170  e ``etsdemo`` ap
-00004e40: 706c 6963 6174 696f 6e2e 2028 5468 6520  plication. (The 
-00004e50: 6c61 7474 6572 2063 616e 2062 650a 2020  latter can be.  
-00004e60: 696e 7374 616c 6c65 6420 6672 6f6d 2050  installed from P
-00004e70: 7950 4920 7769 7468 2060 6070 6970 2069  yPI with ``pip i
-00004e80: 6e73 7461 6c6c 2065 7473 6465 6d6f 6060  nstall etsdemo``
-00004e90: 2e29 0a2a 2050 6572 666f 726d 616e 6365  .).* Performance
-00004ea0: 206f 6620 7468 6520 6060 6f62 7365 7276   of the ``observ
-00004eb0: 6560 6020 6672 616d 6577 6f72 6b20 6861  e`` framework ha
-00004ec0: 7320 6265 656e 2073 6967 6e69 6669 6361  s been significa
-00004ed0: 6e74 6c79 2069 6d70 726f 7665 642e 0a2a  ntly improved..*
-00004ee0: 2049 7427 7320 6e6f 206c 6f6e 6765 7220   It's no longer 
-00004ef0: 6e65 6365 7373 6172 7920 746f 2073 7065  necessary to spe
-00004f00: 6369 6679 2061 2074 7261 6974 2063 6f6d  cify a trait com
-00004f10: 7061 7269 736f 6e20 6d6f 6465 206f 660a  parison mode of.
-00004f20: 2020 6060 436f 6d70 6172 6973 6f6e 4d6f    ``ComparisonMo
-00004f30: 6465 2e69 6465 6e74 6974 7960 6020 7768  de.identity`` wh
-00004f40: 656e 2075 7369 6e67 2060 606f 6273 6572  en using ``obser
-00004f50: 7665 6060 2074 6f20 6f62 7365 7276 6520  ve`` to observe 
-00004f60: 6974 656d 730a 2020 696e 2061 2060 604c  items.  in a ``L
-00004f70: 6973 7460 602c 2060 6044 6963 7460 6020  ist``, ``Dict`` 
-00004f80: 6f72 2060 6053 6574 6060 2e0a 2a20 5375  or ``Set``..* Su
-00004f90: 7070 6f72 7420 666f 7220 5079 7468 6f6e  pport for Python
-00004fa0: 2033 2e35 2068 6173 2062 6565 6e20 6472   3.5 has been dr
-00004fb0: 6f70 7065 642e 0a2a 2057 6865 6e20 696d  opped..* When im
-00004fc0: 706f 7274 696e 6720 6672 6f6d 2054 7261  porting from Tra
-00004fd0: 6974 732c 2079 6f75 2073 686f 756c 6420  its, you should 
-00004fe0: 616c 7761 7973 2069 6d70 6f72 7420 6672  always import fr
-00004ff0: 6f6d 206f 6e65 206f 6620 7468 6520 6060  om one of the ``
-00005000: 6170 6960 600a 2020 6d6f 6475 6c65 7320  api``.  modules 
-00005010: 2866 6f72 2065 7861 6d70 6c65 2c20 6060  (for example, ``
-00005020: 7472 6169 7473 2e61 7069 6060 2c20 6060  traits.api``, ``
-00005030: 7472 6169 7473 2e61 6461 7074 6174 696f  traits.adaptatio
-00005040: 6e2e 6170 6960 602c 2065 7463 2e29 2054  n.api``, etc.) T
-00005050: 6869 730a 2020 7265 636f 6d6d 656e 6461  his.  recommenda
-00005060: 7469 6f6e 2068 6173 206e 6f77 2062 6565  tion has now bee
-00005070: 6e20 6d61 6465 2065 7870 6c69 6369 7420  n made explicit 
-00005080: 696e 2074 6865 2064 6f63 756d 656e 7461  in the documenta
-00005090: 7469 6f6e 2e20 4966 2079 6f75 2066 696e  tion. If you fin
-000050a0: 640a 2020 736f 6d65 7468 696e 6720 796f  d.  something yo
-000050b0: 7520 6e65 6564 2074 6861 7427 7320 6e6f  u need that's no
-000050c0: 7420 6176 6169 6c61 626c 6520 6672 6f6d  t available from
-000050d0: 206f 6e65 206f 6620 7468 6520 6060 6170   one of the ``ap
-000050e0: 6960 6020 6d6f 6475 6c65 732c 0a20 2070  i`` modules,.  p
-000050f0: 6c65 6173 6520 6c65 7420 7468 6520 5472  lease let the Tr
-00005100: 6169 7473 2064 6576 656c 6f70 6572 7320  aits developers 
-00005110: 6b6e 6f77 2e0a 0a0a 4465 7461 696c 6564  know....Detailed
-00005120: 2050 522d 6279 2d50 5220 6368 616e 6765   PR-by-PR change
-00005130: 730a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  s.~~~~~~~~~~~~~~
-00005140: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a4d 6f72  ~~~~~~~~~~~..Mor
-00005150: 6520 7468 616e 2036 3020 5052 7320 7765  e than 60 PRs we
-00005160: 6e74 2069 6e74 6f20 7468 6973 2072 656c  nt into this rel
-00005170: 6561 7365 2e20 5468 6520 666f 6c6c 6f77  ease. The follow
-00005180: 696e 6720 7065 6f70 6c65 2063 6f6e 7472  ing people contr
-00005190: 6962 7574 6564 2074 6f0a 7468 6973 2072  ibuted to.this r
-000051a0: 656c 6561 7365 3a0a 0a2a 2041 6172 6f6e  elease:..* Aaron
-000051b0: 2041 7972 6573 0a2a 2041 6c65 7861 6e64   Ayres.* Alexand
-000051c0: 7265 2043 6861 626f 742d 4c65 636c 6572  re Chabot-Lecler
-000051d0: 630a 2a20 4b69 7420 4368 6f69 0a2a 204d  c.* Kit Choi.* M
-000051e0: 6172 6b20 4469 636b 696e 736f 6e0a 2a20  ark Dickinson.* 
-000051f0: 4b65 7669 6e20 4475 6666 0a2a 2047 6c65  Kevin Duff.* Gle
-00005200: 6e20 4772 616e 7a6f 770a 2a20 4d61 7474  n Granzow.* Matt
-00005210: 2048 616e 636f 636b 0a2a 2052 6168 756c   Hancock.* Rahul
-00005220: 2050 6f72 7572 690a 2a20 4572 6963 2050   Poruri.* Eric P
-00005230: 7265 7374 6174 0a2a 204b 7579 6120 5461  restat.* Kuya Ta
-00005240: 6b61 6d69 0a2a 2048 7567 6f20 7661 6e20  kami.* Hugo van 
-00005250: 4b65 6d65 6e61 6465 0a2a 2041 6469 7479  Kemenade.* Adity
-00005260: 6120 5661 7473 0a2a 2043 6f72 7261 6e20  a Vats.* Corran 
-00005270: 5765 6273 7465 720a 0a0a 4665 6174 7572  Webster...Featur
-00005280: 6573 0a7e 7e7e 7e7e 7e7e 7e0a 0a2a 2054  es.~~~~~~~~..* T
-00005290: 6865 2060 6050 726f 7065 7274 7960 6020  he ``Property`` 
-000052a0: 7472 6169 7420 7479 7065 206e 6f77 2073  trait type now s
-000052b0: 7570 706f 7274 7320 7468 6520 6060 6f62  upports the ``ob
-000052c0: 7365 7276 6560 6020 6b65 7977 6f72 642e  serve`` keyword.
-000052d0: 2028 2331 3137 352c 0a20 2023 3134 3030   (#1175,.  #1400
-000052e0: 290a 2a20 4164 6420 6060 7c3d 6060 2073  ).* Add ``|=`` s
-000052f0: 7570 706f 7274 2074 6f20 5472 6169 7444  upport to TraitD
-00005300: 6963 7420 666f 7220 5079 7468 6f6e 2033  ict for Python 3
-00005310: 2e39 2061 6e64 206c 6174 6572 2e20 2823  .9 and later. (#
-00005320: 3133 3036 290a 2a20 4164 6420 6361 7374  1306).* Add cast
-00005330: 696e 6720 6b65 7977 6f72 6420 746f 206e  ing keyword to n
-00005340: 756d 6572 6963 2061 7272 6179 2074 7970  umeric array typ
-00005350: 6573 2e20 2823 3534 3729 0a2a 2054 6865  es. (#547).* The
-00005360: 2054 7261 6974 7320 6578 616d 706c 6573   Traits examples
-00005370: 2061 7265 206e 6f77 2070 6172 7420 6f66   are now part of
-00005380: 2074 6865 2054 7261 6974 7320 7061 636b   the Traits pack
-00005390: 6167 652c 2061 6e64 2073 6f20 6172 650a  age, and so are.
-000053a0: 2020 636f 6e74 7269 6275 7465 6420 746f    contributed to
-000053b0: 2060 6065 7473 6465 6d6f 6060 2e20 2823   ``etsdemo``. (#
-000053c0: 3132 3735 290a 2a20 5468 6520 5472 6169  1275).* The Trai
-000053d0: 7473 2065 7861 6d70 6c65 7320 7061 636b  ts examples pack
-000053e0: 6167 6520 6e6f 7720 696e 636c 7564 6573  age now includes
-000053f0: 2061 2062 6567 696e 6e65 7227 7320 7475   a beginner's tu
-00005400: 746f 7269 616c 2e20 2823 3130 3631 290a  torial. (#1061).
-00005410: 0a0a 5065 7266 6f72 6d61 6e63 650a 7e7e  ..Performance.~~
-00005420: 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a 2050 6172  ~~~~~~~~~..* Par
-00005430: 7369 6e67 206f 6620 7468 6520 6060 6f62  sing of the ``ob
-00005440: 7365 7276 6560 6020 7374 7269 6e67 2077  serve`` string w
-00005450: 6173 2070 7265 7669 6f75 736c 7920 6120  as previously a 
-00005460: 7065 7266 6f72 6d61 6e63 6520 626f 7474  performance bott
-00005470: 6c65 6e65 636b 2e0a 2020 5468 6973 2068  leneck..  This h
-00005480: 6173 2062 6565 6e20 6669 7865 642c 2062  as been fixed, b
-00005490: 7920 7265 6d6f 7669 6e67 2073 6f6d 6520  y removing some 
-000054a0: 7265 6475 6e64 616e 7420 7061 7273 696e  redundant parsin
-000054b0: 6720 6361 6c6c 7320 616e 6420 6279 2063  g calls and by c
-000054c0: 6163 6869 6e67 0a20 2070 6172 7369 6e67  aching.  parsing
-000054d0: 2072 6573 756c 7473 2e20 2823 3133 3433   results. (#1343
-000054e0: 2c20 2331 3334 342c 2023 3133 3435 290a  , #1344, #1345).
-000054f0: 0a0a 4368 616e 6765 730a 7e7e 7e7e 7e7e  ..Changes.~~~~~~
-00005500: 7e0a 0a2a 2054 6865 2060 604e 6f44 6566  ~..* The ``NoDef
-00005510: 6175 6c74 5370 6563 6966 6965 6460 6020  aultSpecified`` 
-00005520: 636f 6e73 7461 6e74 2028 7573 6564 2061  constant (used a
-00005530: 7320 6120 6465 6661 756c 7420 7661 6c75  s a default valu
-00005540: 6520 666f 720a 2020 7468 6520 6060 5472  e for.  the ``Tr
-00005550: 6169 7454 7970 6560 6020 6060 6465 6661  aitType`` ``defa
-00005560: 756c 745f 7661 6c75 6560 6020 6172 6775  ult_value`` argu
-00005570: 6d65 6e74 2920 6973 206e 6f77 2070 7562  ment) is now pub
-00005580: 6c69 632c 206d 6164 650a 2020 6176 6169  lic, made.  avai
-00005590: 6c61 626c 6520 6672 6f6d 2060 6074 7261  lable from ``tra
-000055a0: 6974 732e 6170 6960 602e 2028 2331 3338  its.api``. (#138
-000055b0: 342c 2023 3133 3830 2c20 2331 3337 3829  4, #1380, #1378)
-000055c0: 0a2a 2054 6865 2064 6570 7265 6361 7469  .* The deprecati
-000055d0: 6f6e 206f 6620 7468 6520 6060 5472 6169  on of the ``Trai
-000055e0: 744d 6170 6060 2074 7261 6974 2074 7970  tMap`` trait typ
-000055f0: 6520 6861 7320 6265 656e 2072 6576 6572  e has been rever
-00005600: 7365 642c 2062 6563 6175 7365 0a20 2074  sed, because.  t
-00005610: 6865 7265 2061 7265 2065 7869 7374 696e  here are existin
-00005620: 6720 7573 6573 206f 6620 6060 5472 6169  g uses of ``Trai
-00005630: 744d 6170 6060 2074 6861 7420 6172 6520  tMap`` that are 
-00005640: 6861 7264 2074 6f20 7265 706c 6163 652e  hard to replace.
-00005650: 0a20 204e 6576 6572 7468 656c 6573 732c  .  Nevertheless,
-00005660: 2069 7420 6973 2073 7469 6c6c 206e 6f74   it is still not
-00005670: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00005680: 7573 6520 6060 5472 6169 744d 6170 6060  use ``TraitMap``
-00005690: 2069 6e20 6e65 7720 636f 6465 2e0a 2020   in new code..  
-000056a0: 5573 6520 6060 4d61 7060 6020 696e 7374  Use ``Map`` inst
-000056b0: 6561 642e 2028 2331 3336 3529 0a2a 2041  ead. (#1365).* A
-000056c0: 6e20 6174 7465 6d70 7420 746f 2075 7365  n attempt to use
-000056d0: 2060 6050 7265 6669 784c 6973 7460 6020   ``PrefixList`` 
-000056e0: 7769 7468 2061 6e20 656d 7074 7920 6c69  with an empty li
-000056f0: 7374 2c20 6f72 2060 6050 7265 6669 784d  st, or ``PrefixM
-00005700: 6170 6060 206f 720a 2020 6060 4d61 7060  ap`` or.  ``Map`
-00005710: 6020 7769 7468 2061 6e20 656d 7074 7920  ` with an empty 
-00005720: 6469 6374 696f 6e61 7279 2c20 6e6f 7720  dictionary, now 
-00005730: 7261 6973 6573 2060 6056 616c 7565 4572  raises ``ValueEr
-00005740: 726f 7260 602e 2041 7320 6120 7265 7375  ror``. As a resu
-00005750: 6c74 2c0a 2020 7468 6520 6465 6661 756c  lt,.  the defaul
-00005760: 7420 6465 6661 756c 7420 7661 6c75 6520  t default value 
-00005770: 2877 6869 6368 2075 7365 6420 746f 2062  (which used to b
-00005780: 6520 6060 4e6f 6e65 6060 2920 6973 2061  e ``None``) is a
-00005790: 6c77 6179 7320 7661 6c69 642e 0a20 2028  lways valid..  (
-000057a0: 2331 3335 3129 0a2a 2060 6054 7261 6974  #1351).* ``Trait
-000057b0: 4c69 7374 4576 656e 7460 6020 6172 6775  ListEvent`` argu
-000057c0: 6d65 6e74 7320 6172 6520 6e6f 7720 6b65  ments are now ke
-000057d0: 7977 6f72 6420 6f6e 6c79 2e20 2823 3133  yword only. (#13
-000057e0: 3436 290a 2a20 4974 2773 206e 6f20 6c6f  46).* It's no lo
-000057f0: 6e67 6572 206e 6563 6573 7361 7279 2074  nger necessary t
-00005800: 6f20 7370 6563 6966 7920 6120 7472 6169  o specify a trai
-00005810: 7420 636f 6d70 6172 6973 6f6e 206d 6f64  t comparison mod
-00005820: 6520 6f66 0a20 2060 6043 6f6d 7061 7269  e of.  ``Compari
-00005830: 736f 6e4d 6f64 652e 6964 656e 7469 7479  sonMode.identity
-00005840: 6060 2077 6865 6e20 7573 696e 6720 6060  `` when using ``
-00005850: 6f62 7365 7276 6560 6020 746f 206f 6273  observe`` to obs
-00005860: 6572 7665 2069 7465 6d73 0a20 2069 6e20  erve items.  in 
-00005870: 6120 6060 4c69 7374 6060 2c20 6060 4469  a ``List``, ``Di
-00005880: 6374 6060 206f 7220 6060 5365 7460 602e  ct`` or ``Set``.
-00005890: 2028 2331 3136 352c 2023 3133 3238 2c20   (#1165, #1328, 
-000058a0: 2331 3234 3029 0a0a 0a44 6570 7265 6361  #1240)...Depreca
-000058b0: 7469 6f6e 730a 7e7e 7e7e 7e7e 7e7e 7e7e  tions.~~~~~~~~~~
-000058c0: 7e7e 0a0a 2a20 5468 6520 6060 4675 6e63  ~~..* The ``Func
-000058d0: 7469 6f6e 6060 2061 6e64 2060 604d 6574  tion`` and ``Met
-000058e0: 686f 6460 6020 7472 6169 7420 7479 7065  hod`` trait type
-000058f0: 7320 6172 6520 6465 7072 6563 6174 6564  s are deprecated
-00005900: 2e20 5573 650a 2020 6060 4361 6c6c 6162  . Use.  ``Callab
-00005910: 6c65 6060 206f 7220 6060 496e 7374 616e  le`` or ``Instan
-00005920: 6365 6060 2069 6e73 7465 6164 2e20 2823  ce`` instead. (#
-00005930: 3133 3939 2c20 2331 3339 3729 0a2a 2054  1399, #1397).* T
-00005940: 6865 2060 6065 6469 7460 6020 7061 7261  he ``edit`` para
-00005950: 6d65 7465 7220 746f 2060 6063 6f6e 6669  meter to ``confi
-00005960: 6775 7265 5f74 7261 6974 7360 6020 6861  gure_traits`` ha
-00005970: 7320 6265 656e 2064 6570 7265 6361 7465  s been deprecate
-00005980: 642e 2028 2331 3331 3129 0a2a 2054 6865  d. (#1311).* The
-00005990: 2060 6055 6e69 7474 6573 7454 6f6f 6c73   ``UnittestTools
-000059a0: 2e5f 6361 7463 685f 7761 726e 696e 6773  ._catch_warnings
-000059b0: 6060 2066 756e 6374 696f 6e20 6861 7320  `` function has 
-000059c0: 6265 656e 2064 6570 7265 6361 7465 642e  been deprecated.
-000059d0: 2028 2331 3331 3029 0a2a 2054 6865 2075   (#1310).* The u
-000059e0: 7365 206f 6620 7468 6520 6060 4348 4543  se of the ``CHEC
-000059f0: 4b5f 494e 5445 5246 4143 4553 6060 2067  K_INTERFACES`` g
-00005a00: 6c6f 6261 6c20 7661 7269 6162 6c65 2066  lobal variable f
-00005a10: 6f72 2061 7574 6f6d 6174 6564 0a20 2069  or automated.  i
-00005a20: 6e74 6572 6661 6365 2063 6865 636b 696e  nterface checkin
-00005a30: 6720 6861 7320 6265 656e 2064 6570 7265  g has been depre
-00005a40: 6361 7465 642e 2028 2331 3233 3129 0a0a  cated. (#1231)..
-00005a50: 0a46 6978 6573 0a7e 7e7e 7e7e 0a0a 2a20  .Fixes.~~~~~..* 
-00005a60: 4e6f 6e2d 6060 5472 6169 7445 7272 6f72  Non-``TraitError
-00005a70: 6060 2065 7863 6570 7469 6f6e 7320 7261  `` exceptions ra
-00005a80: 6973 6564 2064 7572 696e 6720 6060 5475  ised during ``Tu
-00005a90: 706c 6560 6020 7661 6c69 6461 7469 6f6e  ple`` validation
-00005aa0: 2061 7265 206e 6f77 0a20 2070 726f 7061   are now.  propa
-00005ab0: 6761 7465 642e 2050 7265 7669 6f75 736c  gated. Previousl
-00005ac0: 7920 7468 6579 2077 6572 6520 636f 6e76  y they were conv
-00005ad0: 6572 7465 6420 696e 746f 2060 6054 7261  erted into ``Tra
-00005ae0: 6974 4572 726f 7260 602e 2028 2331 3339  itError``. (#139
-00005af0: 3329 0a2a 2044 796e 616d 6963 2060 6052  3).* Dynamic ``R
-00005b00: 616e 6765 6060 2061 6e64 2060 6045 6e75  ange`` and ``Enu
-00005b10: 6d60 6020 7472 6169 7473 2061 7265 206e  m`` traits are n
-00005b20: 6f77 2070 726f 7065 726c 7920 7661 6c69  ow properly vali
-00005b30: 6461 7465 640a 2020 7768 656e 2069 6e73  dated.  when ins
-00005b40: 6964 6520 6120 636f 6e74 6169 6e65 7220  ide a container 
-00005b50: 2866 6f72 2065 7861 6d70 6c65 2060 6054  (for example ``T
-00005b60: 7570 6c65 6060 206f 7220 6060 4c69 7374  uple`` or ``List
-00005b70: 6060 292e 2050 7265 7669 6f75 736c 790a  ``). Previously.
-00005b80: 2020 6e6f 2076 616c 6964 6174 696f 6e20    no validation 
-00005b90: 7761 7320 7065 7266 6f72 6d65 642e 2028  was performed. (
-00005ba0: 2331 3338 382c 2023 3133 3932 290a 2a20  #1388, #1392).* 
-00005bb0: 5265 6d6f 7665 2074 6865 2075 6e75 7365  Remove the unuse
-00005bc0: 6420 6d6f 6475 6c65 2d6c 6576 656c 2063  d module-level c
-00005bd0: 6f6e 7374 616e 7420 6060 7472 6169 7473  onstant ``traits
-00005be0: 2e68 6173 5f74 7261 6974 732e 456d 7074  .has_traits.Empt
-00005bf0: 794c 6973 7460 602e 0a20 2028 2331 3336  yList``..  (#136
-00005c00: 3629 0a2a 2044 6f6e 2774 2068 6172 642d  6).* Don't hard-
-00005c10: 636f 6465 2063 6c61 7373 206e 616d 6573  code class names
-00005c20: 2069 6e20 6060 5f5f 7265 7072 5f5f 6060   in ``__repr__``
-00005c30: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-00005c40: 206f 660a 2020 6060 5472 6169 744c 6973   of.  ``TraitLis
-00005c50: 7445 7665 6e74 6060 2c20 6060 5472 6169  tEvent``, ``Trai
-00005c60: 7453 6574 4576 656e 7460 6020 616e 6420  tSetEvent`` and 
-00005c70: 6060 5472 6169 7444 6963 7445 7665 6e74  ``TraitDictEvent
-00005c80: 6060 2e20 2823 3133 3335 290a 2a20 446f  ``. (#1335).* Do
-00005c90: 6e27 7420 6e6f 7469 6679 206f 6e20 656d  n't notify on em
-00005ca0: 7074 7920 6060 7570 6461 7465 6060 5c20  pty ``update``\ 
-00005cb0: 7320 6f66 2060 6044 6963 7460 6020 7472  s of ``Dict`` tr
-00005cc0: 6169 7473 2e20 2823 3133 3038 290a 2a20  aits. (#1308).* 
-00005cd0: 4669 7820 6578 6365 7074 696f 6e20 7261  Fix exception ra
-00005ce0: 6973 6564 2077 6865 6e20 6173 7369 676e  ised when assign
-00005cf0: 696e 6720 6120 4e75 6d50 7920 6172 7261  ing a NumPy arra
-00005d00: 7920 746f 2061 2060 604c 6973 7460 600a  y to a ``List``.
-00005d10: 2020 7472 6169 742e 2028 2331 3237 3829    trait. (#1278)
-00005d20: 0a2a 2046 6978 2075 7365 7320 6f66 2064  .* Fix uses of d
-00005d30: 6570 7265 6361 7465 6420 6060 6c6f 6767  eprecated ``logg
-00005d40: 6572 2e77 6172 6e60 6020 6675 6e63 7469  er.warn`` functi
-00005d50: 6f6e 2e20 2823 3132 3833 290a 2a20 4669  on. (#1283).* Fi
-00005d60: 7820 6120 6261 6420 6060 496e 7374 616e  x a bad ``Instan
-00005d70: 6365 6060 2074 7261 6974 2064 6563 6c61  ce`` trait decla
-00005d80: 7261 7469 6f6e 2066 6f72 2061 2070 7269  ration for a pri
-00005d90: 7661 7465 2074 7261 6974 2069 6e0a 2020  vate trait in.  
-00005da0: 7468 6520 6060 5f54 7261 6974 4368 616e  the ``_TraitChan
-00005db0: 6765 436f 6c6c 6563 746f 7260 6020 636c  geCollector`` cl
-00005dc0: 6173 732e 2028 2331 3431 3129 0a0a 0a44  ass. (#1411)...D
-00005dd0: 6f63 756d 656e 7461 7469 6f6e 0a7e 7e7e  ocumentation.~~~
-00005de0: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20 4164  ~~~~~~~~~~..* Ad
-00005df0: 6420 2254 7574 6f72 6961 6c22 2073 6563  d "Tutorial" sec
-00005e00: 7469 6f6e 2074 6f20 7468 6520 6d61 696e  tion to the main
-00005e10: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
-00005e20: 6261 7365 6420 6f6e 2074 6865 0a20 206e  based on the.  n
-00005e30: 6577 2060 6074 7261 6974 732e 6578 616d  ew ``traits.exam
-00005e40: 706c 6573 6060 2074 7574 6f72 6961 6c20  ples`` tutorial 
-00005e50: 636f 6e74 656e 742e 2028 2331 3337 3429  content. (#1374)
-00005e60: 0a2a 2043 6c61 7269 6679 2074 6861 7420  .* Clarify that 
-00005e70: 6f6e 6c79 2074 6865 2060 6061 7069 6060  only the ``api``
-00005e80: 206d 6f64 756c 6573 2073 686f 756c 6420   modules should 
-00005e90: 6265 2075 7365 6420 666f 7220 696d 706f  be used for impo
-00005ea0: 7274 732e 2028 2331 3338 3729 0a2a 2055  rts. (#1387).* U
-00005eb0: 7064 6174 6520 636f 7079 7269 6768 7420  pdate copyright 
-00005ec0: 6865 6164 6572 2065 6e64 2079 6561 7273  header end years
-00005ed0: 2e20 2823 3133 3736 290a 2a20 5570 6461  . (#1376).* Upda
-00005ee0: 7465 2063 6f6e 7465 6e74 7320 6f66 2060  te contents of `
-00005ef0: 6069 6d61 6765 5f4c 4943 454e 5345 2e74  `image_LICENSE.t
-00005f00: 7874 6060 2e20 2823 3133 3632 290a 2a20  xt``. (#1362).* 
-00005f10: 5265 6d6f 7665 206d 656e 7469 6f6e 7320  Remove mentions 
-00005f20: 6f66 2074 6865 2072 656d 6f76 6564 2066  of the removed f
-00005f30: 756e 6374 696f 6e73 2060 6061 6461 7074  unctions ``adapt
-00005f40: 7360 6020 616e 6420 6060 696d 706c 656d  s`` and ``implem
-00005f50: 656e 7473 6060 2066 726f 6d0a 2020 7468  ents`` from.  th
-00005f60: 6520 6578 616d 706c 6573 2061 6e64 2074  e examples and t
-00005f70: 7574 6f72 6961 6c2e 2028 2331 3336 3729  utorial. (#1367)
-00005f80: 0a2a 204d 6f76 6520 5472 6169 7473 2069  .* Move Traits i
-00005f90: 6e74 726f 6475 6374 696f 6e20 6465 7363  ntroduction desc
-00005fa0: 7269 7074 696f 6e20 746f 2060 6069 6e64  ription to ``ind
-00005fb0: 6578 2e72 7374 6060 2e20 2823 3133 3538  ex.rst``. (#1358
-00005fc0: 290a 2a20 4669 7820 7061 7468 2074 6f20  ).* Fix path to 
-00005fd0: 456e 7468 6f75 6768 7420 6c6f 676f 2077  Enthought logo w
-00005fe0: 6865 6e20 6275 696c 6469 6e67 2064 6f63  hen building doc
-00005ff0: 7365 742e 2028 2331 3238 3529 0a2a 2046  set. (#1285).* F
-00006000: 6978 2074 6865 2060 6074 7261 6974 5f64  ix the ``trait_d
-00006010: 6f63 756d 656e 7465 7260 6020 6578 7465  ocumenter`` exte
-00006020: 6e73 696f 6e20 746f 2062 6520 6c65 7373  nsion to be less
-00006030: 2066 7261 6769 6c65 2e20 2823 3132 3437   fragile. (#1247
-00006040: 290a 2a20 4164 6420 7573 6572 206d 616e  ).* Add user man
-00006050: 7561 6c20 646f 6375 6d65 6e74 6174 696f  ual documentatio
-00006060: 6e20 666f 7220 7468 6520 6060 496e 7374  n for the ``Inst
-00006070: 616e 6365 6060 2074 7261 6974 2074 7970  ance`` trait typ
-00006080: 652e 2028 2331 3339 3529 0a2a 2044 6f63  e. (#1395).* Doc
-00006090: 756d 656e 7420 7468 6174 2074 6865 2060  ument that the `
-000060a0: 604c 6973 7460 602c 2060 6044 6963 7460  `List``, ``Dict`
-000060b0: 6020 616e 6420 6060 5365 7460 6020 7472  ` and ``Set`` tr
-000060c0: 6169 7420 7479 7065 7320 636f 7079 206f  ait types copy o
-000060d0: 6e0a 2020 6173 7369 676e 6d65 6e74 2e20  n.  assignment. 
-000060e0: 2823 3134 3032 290a 2a20 5661 7269 6f75  (#1402).* Variou
-000060f0: 7320 6f74 6865 7220 6d69 6e6f 7220 696d  s other minor im
-00006100: 7072 6f76 656d 656e 7473 2c20 7479 706f  provements, typo
-00006110: 2066 6978 6573 2c20 616e 6420 6f74 6865   fixes, and othe
-00006120: 7220 646f 6375 6d65 6e74 6174 696f 6e20  r documentation 
-00006130: 6669 7865 732e 0a20 2028 2331 3339 362c  fixes..  (#1396,
-00006140: 2023 3133 3833 2c20 2331 3338 312c 2023   #1383, #1381, #
-00006150: 3133 3834 2c20 2331 3239 322c 2023 3133  1384, #1292, #13
-00006160: 3535 2c20 2331 3335 302c 2023 3133 3139  55, #1350, #1319
-00006170: 2c20 2331 3239 322c 2023 3134 3031 290a  , #1292, #1401).
-00006180: 0a0a 436c 6561 6e75 7020 616e 6420 6f74  ..Cleanup and ot
-00006190: 6865 7220 6d61 696e 7465 6e61 6e63 650a  her maintenance.
-000061a0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-000061b0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a  ~~~~~~~~~~~~~..*
-000061c0: 2052 656d 6f76 6520 6465 6164 2063 6f64   Remove dead cod
-000061d0: 652e 2028 2331 3238 3129 0a2a 2055 7064  e. (#1281).* Upd
-000061e0: 6174 6520 6060 7375 7065 7260 6020 7573  ate ``super`` us
-000061f0: 6167 6520 746f 2074 6865 2075 7375 616c  age to the usual
-00006200: 2050 7974 686f 6e20 3320 6172 6775 6d65   Python 3 argume
-00006210: 6e74 2d6c 6573 7320 7061 7474 6572 6e2e  nt-less pattern.
-00006220: 2028 2331 3238 3029 0a2a 2052 656d 6f76   (#1280).* Remov
-00006230: 6520 7065 722d 696d 706f 7274 2060 6023  e per-import ``#
-00006240: 206e 6f71 6160 6020 636f 6d6d 656e 7473   noqa`` comments
-00006250: 2069 6e20 6060 6170 6960 6020 6d6f 6475   in ``api`` modu
-00006260: 6c65 7320 696e 2066 6176 6f75 7220 6f66  les in favour of
-00006270: 0a20 2070 6572 2d66 696c 6520 6967 6e6f  .  per-file igno
-00006280: 7265 7320 696e 2074 6865 2060 6066 6c61  res in the ``fla
-00006290: 6b65 3860 6020 636f 6e66 6967 7572 6174  ke8`` configurat
-000062a0: 696f 6e2e 2028 2331 3236 3929 0a2a 2052  ion. (#1269).* R
-000062b0: 656d 6f76 6520 6f75 742d 6f66 2d64 6174  emove out-of-dat
-000062c0: 6520 616e 6420 6e6f 6e2d 6675 6e63 7469  e and non-functi
-000062d0: 6f6e 616c 2063 6f76 6572 6167 6520 6261  onal coverage ba
-000062e0: 6467 6520 6672 6f6d 2052 4541 444d 452e  dge from README.
-000062f0: 2028 2331 3236 3329 0a2a 2052 656e 616d   (#1263).* Renam
-00006300: 6520 6060 5f69 5f6f 6273 6572 7661 626c  e ``_i_observabl
-00006310: 6560 6020 6d6f 6475 6c65 2074 6f20 6060  e`` module to ``
-00006320: 695f 6f62 7365 7276 6162 6c65 6060 2e20  i_observable``. 
-00006330: 2823 3132 3936 290a 2a20 5265 6661 6374  (#1296).* Refact
-00006340: 6f72 2061 6e64 2073 696d 706c 6966 7920  or and simplify 
-00006350: 6d65 7468 6f64 2063 6865 636b 732e 2028  method checks. (
-00006360: 2331 3137 3629 0a2a 2046 6978 2074 7970  #1176).* Fix typ
-00006370: 6f20 696e 206f 7074 696f 6e61 6c5f 6465  o in optional_de
-00006380: 7065 6e64 656e 6369 6573 2063 6f6d 6d65  pendencies comme
-00006390: 6e74 2e20 2823 3132 3335 290a 2a20 5573  nt. (#1235).* Us
-000063a0: 6520 436f 6d70 6172 6973 6f6e 4d6f 6465  e ComparisonMode
-000063b0: 2063 6f6e 7374 616e 7473 2069 6e73 7465   constants inste
-000063c0: 6164 206f 6620 6d61 6769 6320 6e75 6d62  ad of magic numb
-000063d0: 6572 732e 2028 2331 3232 3929 0a0a 0a54  ers. (#1229)...T
-000063e0: 6573 7420 7375 6974 650a 7e7e 7e7e 7e7e  est suite.~~~~~~
-000063f0: 7e7e 7e7e 0a0a 2a20 5072 6576 656e 7420  ~~~~..* Prevent 
-00006400: 7465 7374 5f65 6e75 6d20 6661 696c 7572  test_enum failur
-00006410: 6573 2069 6620 7472 6169 7473 7569 206f  es if traitsui o
-00006420: 7220 4755 4920 746f 6f6c 6b69 7420 6172  r GUI toolkit ar
-00006430: 6520 6e6f 7420 696e 7374 616c 6c65 642e  e not installed.
-00006440: 0a20 2028 2331 3334 3929 0a2a 2054 6573  .  (#1349).* Tes
-00006450: 7473 2074 6861 7420 7265 7175 6972 6520  ts that require 
-00006460: 6060 706b 675f 7265 736f 7572 6365 7360  ``pkg_resources`
-00006470: 6020 6172 6520 736b 6970 7065 6420 6966  ` are skipped if
-00006480: 2060 6073 6574 7570 746f 6f6c 7360 6020   ``setuptools`` 
-00006490: 6973 206e 6f74 0a20 2069 6e73 7461 6c6c  is not.  install
-000064a0: 6564 2e20 2823 3133 3031 290a 2a20 4669  ed. (#1301).* Fi
-000064b0: 7820 616e 206f 7264 6572 2d64 6570 656e  x an order-depen
-000064c0: 6465 6e63 7920 6275 6720 696e 2074 6865  dency bug in the
-000064d0: 2060 6074 6573 745f 7375 6263 6c61 7373   ``test_subclass
-000064e0: 6573 5f77 6561 6b72 6566 6060 2072 6567  es_weakref`` reg
-000064f0: 7265 7373 696f 6e0a 2020 7465 7374 2e20  ression.  test. 
-00006500: 2823 3132 3930 290a 2a20 4669 7820 6120  (#1290).* Fix a 
-00006510: 7479 706f 2069 6e20 6120 7465 7374 206d  typo in a test m
-00006520: 6574 686f 6420 6e61 6d65 2e20 2823 3133  ethod name. (#13
-00006530: 3039 290a 2a20 5661 7269 6f75 7320 6164  09).* Various ad
-00006540: 6469 7469 6f6e 616c 206f 7220 696d 7072  ditional or impr
-00006550: 6f76 6564 2074 6573 7473 2066 6f72 2065  oved tests for e
-00006560: 7869 7374 696e 6720 636f 6465 2e0a 2020  xisting code..  
-00006570: 2823 3133 3539 2c20 2331 3333 362c 2023  (#1359, #1336, #
-00006580: 3133 3330 2c20 2331 3234 382c 2023 3132  1330, #1248, #12
-00006590: 3235 2c20 2331 3230 382c 2023 3132 3039  25, #1208, #1209
-000065a0: 290a 0a0a 4275 696c 6420 616e 6420 6465  )...Build and de
-000065b0: 7665 6c6f 706d 656e 7420 776f 726b 666c  velopment workfl
-000065c0: 6f77 2063 6861 6e67 6573 0a7e 7e7e 7e7e  ow changes.~~~~~
-000065d0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-000065e0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-000065f0: 7e0a 0a2a 2054 7261 6974 7320 6e6f 7720  ~..* Traits now 
-00006600: 7573 6573 2047 6974 4875 6220 4163 7469  uses GitHub Acti
-00006610: 6f6e 7320 666f 7220 636f 6e74 696e 756f  ons for continuo
-00006620: 7573 2069 6e74 6567 7261 7469 6f6e 2e20  us integration. 
-00006630: 5468 6520 5472 6176 6973 2043 490a 2020  The Travis CI.  
-00006640: 616e 6420 4170 7076 6579 6f72 2063 6f6e  and Appveyor con
-00006650: 6669 6775 7261 7469 6f6e 7320 6861 7665  figurations have
-00006660: 2062 6565 6e20 7265 6d6f 7665 642e 2028   been removed. (
-00006670: 2331 3239 362c 2023 3133 3630 290a 2a20  #1296, #1360).* 
-00006680: 4349 2072 756e 7320 6172 6520 6e6f 206c  CI runs are no l
-00006690: 6f6e 6765 7220 6261 7365 6420 6f6e 2045  onger based on E
-000066a0: 444d 2e20 2823 3837 3829 0a2a 204e 6577  DM. (#878).* New
-000066b0: 2043 4920 7275 6e20 666f 7220 7468 6520   CI run for the 
-000066c0: 636f 7265 2074 6573 7420 7375 6974 652c  core test suite,
-000066d0: 2077 6974 686f 7574 2061 6e79 206f 7074   without any opt
-000066e0: 696f 6e61 6c20 6465 7065 6e64 656e 6369  ional dependenci
-000066f0: 6573 2e0a 2020 2823 3133 3134 290a 2a20  es..  (#1314).* 
-00006700: 5465 7374 2050 7974 686f 6e20 332e 3920  Test Python 3.9 
-00006710: 696e 2074 6865 2063 6f6e 7469 6e75 6f75  in the continuou
-00006720: 7320 696e 7465 6772 6174 696f 6e20 2861  s integration (a
-00006730: 6e64 2064 726f 7020 7465 7374 7320 666f  nd drop tests fo
-00006740: 7220 5079 7468 6f6e 0a20 2033 2e35 2061  r Python.  3.5 a
-00006750: 6e64 206f 6c64 6572 292e 2028 2331 3332  nd older). (#132
-00006760: 362c 2023 3133 3133 2c20 2c20 2331 3330  6, #1313, , #130
-00006770: 3329 0a2a 204d 616b 6520 6060 7472 6169  3).* Make ``trai
-00006780: 7473 2e65 7861 6d70 6c65 7360 6020 696e  ts.examples`` in
-00006790: 746f 2061 2070 6163 6b61 6765 2e20 2823  to a package. (#
-000067a0: 3133 3438 290a 2a20 4d61 6b65 2065 7861  1348).* Make exa
-000067b0: 6d70 6c65 7320 6469 7265 6374 6f72 6965  mples directorie
-000067c0: 7320 6060 666c 616b 6538 6060 2d63 6c65  s ``flake8``-cle
-000067d0: 616e 2e20 2823 3133 3533 290a 2a20 4669  an. (#1353).* Fi
-000067e0: 7820 6578 616d 706c 6573 2070 6163 6b61  x examples packa
-000067f0: 6769 6e67 206e 6974 2e20 2823 3133 3633  ging nit. (#1363
-00006800: 290a 2a20 5375 7070 6f72 7420 6060 2d68  ).* Support ``-h
-00006810: 6060 2066 6f72 2067 6574 7469 6e67 2068  `` for getting h
-00006820: 656c 7020 696e 2060 6065 7473 746f 6f6c  elp in ``etstool
-00006830: 2e70 7960 602e 2028 2331 3334 3729 0a2a  .py``. (#1347).*
-00006840: 2041 6464 2060 6073 6865 6c6c 6060 2063   Add ``shell`` c
-00006850: 6f6d 6d61 6e64 2074 6f20 6060 6574 7374  ommand to ``etst
-00006860: 6f6f 6c2e 7079 6060 2e20 2823 3132 3933  ool.py``. (#1293
-00006870: 290a 2a20 5573 6520 7468 6520 6060 666c  ).* Use the ``fl
-00006880: 616b 6538 5f65 7473 6060 2070 6163 6b61  ake8_ets`` packa
-00006890: 6765 2069 6e20 706c 6163 6520 6f66 2074  ge in place of t
-000068a0: 6865 206c 6f63 616c 2060 6063 6f70 7972  he local ``copyr
-000068b0: 6967 6874 5f68 6561 6465 7260 600a 2020  ight_header``.  
-000068c0: 7061 636b 6167 652e 0a20 2054 6865 2060  package..  The `
-000068d0: 6063 6f70 7972 6967 6874 5f68 6561 6465  `copyright_heade
-000068e0: 7260 6020 7061 636b 6167 6520 6861 7320  r`` package has 
-000068f0: 6265 656e 2072 656d 6f76 6564 2e20 2823  been removed. (#
-00006900: 3133 3431 290a 2a20 4164 6420 7363 7269  1341).* Add scri
-00006910: 7074 2060 6063 6865 636b 5f6f 6273 6572  pt ``check_obser
-00006920: 7665 5f74 696d 696e 672e 7079 6060 2074  ve_timing.py`` t
-00006930: 6f20 6265 6e63 686d 6172 6b20 7065 7266  o benchmark perf
-00006940: 6f72 6d61 6e63 6520 6f66 0a20 2060 606f  ormance of.  ``o
-00006950: 6273 6572 7665 6060 2074 6f20 636f 6d70  bserve`` to comp
-00006960: 6172 6520 7769 7468 2060 606f 6e5f 7472  are with ``on_tr
-00006970: 6169 745f 6368 616e 6765 6060 2e20 2823  ait_change``. (#
-00006980: 3133 3331 290a 2a20 436f 7272 6563 7420  1331).* Correct 
-00006990: 7468 6520 6d69 6e69 6d75 6d20 5370 6869  the minimum Sphi
-000069a0: 6e78 2076 6572 7369 6f6e 2069 6e20 5245  nx version in RE
-000069b0: 4144 4d45 2e20 2823 3132 3136 2c20 2331  ADME. (#1216, #1
-000069c0: 3332 3029 0a2a 2052 6573 7472 6963 7420  320).* Restrict 
-000069d0: 5370 6869 6e78 2076 6572 7369 6f6e 2074  Sphinx version t
-000069e0: 6f20 6176 6f69 6420 6275 6767 7920 7665  o avoid buggy ve
-000069f0: 7273 696f 6e73 2e20 2823 3132 3736 290a  rsions. (#1276).
-00006a00: 2a20 4d61 6b65 2060 606d 7970 7960 6020  * Make ``mypy`` 
-00006a10: 616e 206f 7074 696f 6e61 6c20 6465 7065  an optional depe
-00006a20: 6e64 656e 6379 2e20 2823 3132 3839 290a  ndency. (#1289).
-00006a30: 2a20 5370 6565 6420 7570 2043 4920 6275  * Speed up CI bu
-00006a40: 696c 6473 2066 6f72 2054 7261 7669 7320  ilds for Travis 
-00006a50: 616e 6420 4170 7076 6579 6f72 2062 7920  and Appveyor by 
-00006a60: 6361 6368 696e 6720 7468 6520 6060 7069  caching the ``pi
-00006a70: 7060 6020 6469 7265 6374 6f72 790a 2020  p`` directory.  
-00006a80: 286e 6f77 2072 6564 756e 6461 6e74 292e  (now redundant).
-00006a90: 2028 2331 3234 3129 0a2a 2041 6464 2061   (#1241).* Add a
-00006aa0: 7574 6f6d 6174 6564 2077 6865 656c 2061  utomated wheel a
-00006ab0: 6e64 2073 6469 7374 2062 7569 6c64 696e  nd sdist buildin
-00006ac0: 6720 666f 7220 5472 6169 7473 2072 656c  g for Traits rel
-00006ad0: 6561 7365 732e 2028 2331 3430 342c 2023  eases. (#1404, #
-00006ae0: 3132 3931 290a 2a20 4164 6420 6372 6f6e  1291).* Add cron
-00006af0: 2d6a 6f62 2077 6f72 6b66 6c6f 7720 746f  -job workflow to
-00006b00: 2072 6567 756c 6172 6c79 2074 6573 7420   regularly test 
-00006b10: 696e 7374 616c 6c20 6f66 2074 6865 206c  install of the l
-00006b20: 6174 6573 7420 7265 6c65 6173 6573 0a20  atest releases. 
-00006b30: 2066 726f 6d20 5079 5049 2e20 2823 3134   from PyPI. (#14
-00006b40: 3036 290a 0a0a 5265 6c65 6173 6520 362e  06)...Release 6.
-00006b50: 312e 310a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  1.1.------------
-00006b60: 2d0a 0a52 656c 6561 7365 643a 2032 3032  -..Released: 202
-00006b70: 302d 3037 2d32 330a 0a54 7261 6974 7320  0-07-23..Traits 
-00006b80: 362e 312e 3120 6973 2061 2062 7567 6669  6.1.1 is a bugfi
-00006b90: 7820 7265 6c65 6173 6520 6669 7869 6e67  x release fixing
-00006ba0: 2061 2068 616e 6466 756c 206f 6620 6d69   a handful of mi
-00006bb0: 6e6f 7220 646f 6375 6d65 6e74 6174 696f  nor documentatio
-00006bc0: 6e20 616e 640a 7465 7374 2d72 656c 6174  n and.test-relat
-00006bd0: 6564 2069 7373 7565 7320 7769 7468 2074  ed issues with t
-00006be0: 6865 2054 7261 6974 7320 362e 312e 3020  he Traits 6.1.0 
-00006bf0: 7265 6c65 6173 652e 2054 6865 7265 2061  release. There a
-00006c00: 7265 206e 6f20 4150 492d 6272 6561 6b69  re no API-breaki
-00006c10: 6e67 0a63 6861 6e67 6573 2069 6e20 7468  ng.changes in th
-00006c20: 6973 2072 656c 6561 7365 2e20 4974 2773  is release. It's
-00006c30: 2072 6563 6f6d 6d65 6e64 6564 2074 6861   recommended tha
-00006c40: 7420 616c 6c20 7573 6572 7320 6f66 2054  t all users of T
-00006c50: 7261 6974 7320 362e 312e 300a 7570 6772  raits 6.1.0.upgr
-00006c60: 6164 6520 746f 2054 7261 6974 7320 362e  ade to Traits 6.
-00006c70: 312e 312e 0a0a 4669 7865 730a 7e7e 7e7e  1.1...Fixes.~~~~
-00006c80: 7e0a 0a2a 2044 6f6e 2774 206d 7574 6174  ~..* Don't mutat
-00006c90: 6520 676c 6f62 616c 2073 7461 7465 2061  e global state a
-00006ca0: 7420 696d 706f 7274 2074 696d 6520 696e  t import time in
-00006cb0: 2061 2074 6573 7420 6d6f 6475 6c65 2e20   a test module. 
-00006cc0: 2823 3132 3232 290a 2a20 5374 616e 6461  (#1222).* Standa
-00006cd0: 7264 697a 6520 616e 6420 6669 7820 636f  rdize and fix co
-00006ce0: 7079 7269 6768 7420 7965 6172 7320 696e  pyright years in
-00006cf0: 2073 6f75 7263 6520 6669 6c65 732e 2028   source files. (
-00006d00: 2331 3232 372c 2023 3131 3938 290a 2a20  #1227, #1198).* 
-00006d10: 4669 7820 7472 6169 742d 646f 6375 6d65  Fix trait-docume
-00006d20: 6e74 6572 2065 7874 656e 7369 6f6e 2074  nter extension t
-00006d30: 6573 7473 2066 6f72 2053 7068 696e 7820  ests for Sphinx 
-00006d40: 332e 312e 2028 2331 3230 3629 0a2a 2046  3.1. (#1206).* F
-00006d50: 6978 2074 7261 6974 2d64 6f63 756d 656e  ix trait-documen
-00006d60: 7465 7220 6578 7465 6e73 696f 6e20 746f  ter extension to
-00006d70: 2068 616e 646c 6520 7072 6f70 6572 7469   handle properti
-00006d80: 6573 2063 6f72 7265 6374 6c79 2e20 2823  es correctly. (#
-00006d90: 3132 3436 290a 0a44 6f63 756d 656e 7461  1246)..Documenta
-00006da0: 7469 6f6e 2066 6978 6573 0a7e 7e7e 7e7e  tion fixes.~~~~~
-00006db0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a  ~~~~~~~~~~~~~~..
-00006dc0: 2a20 4578 7061 6e64 2075 7365 7220 6d61  * Expand user ma
-00006dd0: 6e75 616c 2074 6f20 6d65 6e74 696f 6e20  nual to mention 
-00006de0: 6469 7370 6174 6368 2e20 2823 3131 3935  dispatch. (#1195
-00006df0: 290a 2a20 4669 7820 736f 6d65 2073 7065  ).* Fix some spe
-00006e00: 6c6c 696e 6720 616e 6420 6772 616d 6d61  lling and gramma
-00006e10: 7220 6572 726f 7273 2069 6e20 7468 6520  r errors in the 
-00006e20: 7573 6572 206d 616e 7561 6c2e 2028 2331  user manual. (#1
-00006e30: 3231 3029 0a2a 2046 6978 2064 6573 6372  210).* Fix descr
-00006e40: 6970 7469 6f6e 2069 6e20 5245 4144 4d45  iption in README
-00006e50: 2074 6f20 6d61 7463 6820 7468 6520 6f6e   to match the on
-00006e60: 6520 696e 2074 6865 2073 6574 7570 2073  e in the setup s
-00006e70: 6372 6970 742e 2028 2331 3231 3929 0a2a  cript. (#1219).*
-00006e80: 2055 7064 6174 6520 5079 5049 206c 696e   Update PyPI lin
-00006e90: 6b73 2061 6e64 2063 6170 6974 616c 697a  ks and capitaliz
-00006ea0: 6174 696f 6e20 696e 2052 4541 444d 452e  ation in README.
-00006eb0: 7273 742e 2028 2331 3235 3029 0a2a 2046  rst. (#1250).* F
-00006ec0: 6978 2075 7365 7220 6d61 6e75 616c 206d  ix user manual m
-00006ed0: 656e 7469 6f6e 696e 6720 6120 6e6f 6e65  entioning a none
-00006ee0: 7869 7374 696e 6720 6665 6174 7572 6520  xisting feature 
-00006ef0: 696e 206d 6574 6164 6174 6120 6669 6c74  in metadata filt
-00006f00: 6572 2e20 2823 3132 3037 290a 2a20 4669  er. (#1207).* Fi
-00006f10: 7820 7479 706f 2069 6e20 636f 6d6d 656e  x typo in commen
-00006f20: 7420 696e 206f 7074 696f 6e61 6c5f 6465  t in optional_de
-00006f30: 7065 6e64 656e 6369 6573 2e20 2823 3132  pendencies. (#12
-00006f40: 3335 290a 0a0a 5265 6c65 6173 6520 362e  35)...Release 6.
-00006f50: 312e 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  1.0.------------
-00006f60: 2d0a 0a52 656c 6561 7365 643a 2032 3032  -..Released: 202
-00006f70: 302d 3036 2d30 350a 0a54 6865 2054 7261  0-06-05..The Tra
-00006f80: 6974 7320 6c69 6272 6172 7920 6973 2061  its library is a
-00006f90: 2066 6f75 6e64 6174 696f 6e61 6c20 636f   foundational co
-00006fa0: 6d70 6f6e 656e 7420 6f66 2074 6865 2045  mponent of the E
-00006fb0: 6e74 686f 7567 6874 2054 6f6f 6c20 5375  nthought Tool Su
-00006fc0: 6974 652e 2049 740a 7072 6f76 6964 6573  ite. It.provides
-00006fd0: 206f 6273 6572 7661 626c 652c 2074 7970   observable, typ
-00006fe0: 6564 2061 7474 7269 6275 7465 7320 666f  ed attributes fo
-00006ff0: 7220 5079 7468 6f6e 2063 6c61 7373 6573  r Python classes
-00007000: 2c20 6d61 6b69 6e67 2074 686f 7365 2063  , making those c
-00007010: 6c61 7373 6573 0a73 7569 7461 626c 6520  lasses.suitable 
-00007020: 666f 7220 6576 656e 742d 6472 6976 656e  for event-driven
-00007030: 2064 6174 6166 6c6f 7720 7072 6f67 7261   dataflow progra
-00007040: 6d6d 696e 6720 616e 6420 666f 7220 696d  mming and for im
-00007050: 6d65 6469 6174 6520 7573 6520 6173 206d  mediate use as m
-00007060: 6f64 656c 730a 666f 7220 6772 6170 6869  odels.for graphi
-00007070: 6361 6c20 7573 6572 2069 6e74 6572 6661  cal user interfa
-00007080: 6365 732c 206c 696b 6520 7468 6f73 6520  ces, like those 
-00007090: 7072 6f76 6964 6564 2062 7920 7468 6520  provided by the 
-000070a0: 5472 6169 7473 5549 206c 6962 7261 7279  TraitsUI library
-000070b0: 2e0a 0a54 7261 6974 7320 362e 3120 6973  ...Traits 6.1 is
-000070c0: 2074 6865 206c 6174 6573 7420 6665 6174   the latest feat
-000070d0: 7572 6520 7265 6c65 6173 6520 696e 2074  ure release in t
-000070e0: 6865 2054 7261 6974 7320 3620 7365 7269  he Traits 6 seri
-000070f0: 6573 2c20 616e 6420 636f 6e74 6169 6e73  es, and contains
-00007100: 0a73 6576 6572 616c 206d 616a 6f72 2069  .several major i
-00007110: 6d70 726f 7665 6d65 6e74 732e 0a0a 4869  mprovements...Hi
-00007120: 6768 6c69 6768 7473 206f 6620 7468 6973  ghlights of this
-00007130: 2072 656c 6561 7365 0a7e 7e7e 7e7e 7e7e   release.~~~~~~~
-00007140: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00007150: 7e7e 7e0a 0a2a 2041 206e 6577 203a 6d6f  ~~~..* A new :mo
-00007160: 643a 606f 6273 6572 7661 7469 6f6e 203c  d:`observation <
-00007170: 7472 6169 7473 2e6f 6273 6572 7661 7469  traits.observati
-00007180: 6f6e 3e60 2066 7261 6d65 776f 726b 2066  on>` framework f
-00007190: 6f72 206f 6273 6572 7669 6e67 2074 7261  or observing tra
-000071a0: 6974 6564 0a20 2061 7474 7269 6275 7465  ited.  attribute
-000071b0: 7320 616e 6420 6f74 6865 7220 6f62 7365  s and other obse
-000071c0: 7276 6162 6c65 206f 626a 6563 7473 2068  rvable objects h
-000071d0: 6173 2062 6565 6e20 696e 7472 6f64 7563  as been introduc
-000071e0: 6564 2e20 5468 6973 2069 7320 696e 7465  ed. This is inte
-000071f0: 6e64 6564 0a20 2074 6f20 7072 6f76 6964  nded.  to provid
-00007200: 6520 6120 6675 6c6c 2072 6570 6c61 6365  e a full replace
-00007210: 6d65 6e74 2066 6f72 2074 6865 2065 7869  ment for the exi
-00007220: 7374 696e 6720 3a66 756e 633a 606f 6e5f  sting :func:`on_
-00007230: 7472 6169 745f 6368 616e 6765 600a 2020  trait_change`.  
-00007240: 6d65 6368 616e 6973 6d2c 2061 6e64 2061  mechanism, and a
-00007250: 696d 7320 746f 2066 6978 2061 206e 756d  ims to fix a num
-00007260: 6265 7220 6f66 2066 756e 6461 6d65 6e74  ber of fundament
-00007270: 616c 2066 6c61 7773 2061 6e64 206c 696d  al flaws and lim
-00007280: 6974 6174 696f 6e73 206f 660a 2020 7468  itations of.  th
-00007290: 6174 206d 6563 6861 6e69 736d 2e20 5365  at mechanism. Se
-000072a0: 6520 7468 6520 3a72 6566 3a60 6f62 7365  e the :ref:`obse
-000072b0: 7276 652d 6e6f 7469 6669 6361 7469 6f6e  rve-notification
-000072c0: 6020 7365 6374 696f 6e20 6f66 0a20 2074  ` section of.  t
-000072d0: 6865 2075 7365 7220 6d61 6e75 616c 2066  he user manual f
-000072e0: 6f72 2061 6e20 696e 7472 6f64 7563 7469  or an introducti
-000072f0: 6f6e 2074 6f20 7468 6973 2066 7261 6d65  on to this frame
-00007300: 776f 726b 2e0a 0a2a 204e 6577 203a 636c  work...* New :cl
-00007310: 6173 733a 607e 7472 6169 7473 2e74 7261  ass:`~traits.tra
-00007320: 6974 5f6c 6973 745f 6f62 6a65 6374 2e54  it_list_object.T
-00007330: 7261 6974 4c69 7374 602c 0a20 203a 636c  raitList`,.  :cl
-00007340: 6173 733a 607e 7472 6169 7473 2e74 7261  ass:`~traits.tra
-00007350: 6974 5f64 6963 745f 6f62 6a65 6374 2e54  it_dict_object.T
-00007360: 7261 6974 4469 6374 6020 616e 640a 2020  raitDict` and.  
-00007370: 3a63 6c61 7373 3a60 7e74 7261 6974 732e  :class:`~traits.
-00007380: 7472 6169 745f 7365 745f 6f62 6a65 6374  trait_set_object
-00007390: 2e54 7261 6974 5365 7460 2063 6c61 7373  .TraitSet` class
-000073a0: 6573 2068 6176 6520 6265 656e 2061 6464  es have been add
-000073b0: 6564 2c0a 2020 7375 6263 6c61 7373 696e  ed,.  subclassin
-000073c0: 6720 5079 7468 6f6e 2773 2062 7569 6c74  g Python's built
-000073d0: 2d69 6e20 3a63 6c61 7373 3a60 7079 7468  -in :class:`pyth
-000073e0: 6f6e 3a6c 6973 7460 2c20 3a63 6c61 7373  on:list`, :class
-000073f0: 3a60 7079 7468 6f6e 3a64 6963 7460 2061  :`python:dict` a
-00007400: 6e64 0a20 203a 636c 6173 733a 6070 7974  nd.  :class:`pyt
-00007410: 686f 6e3a 7365 7460 2028 7265 7370 6563  hon:set` (respec
-00007420: 7469 7665 6c79 292e 2049 6e73 7461 6e63  tively). Instanc
-00007430: 6573 206f 6620 7468 6573 6520 636c 6173  es of these clas
-00007440: 7365 7320 6172 6520 6f62 7365 7276 6162  ses are observab
-00007450: 6c65 0a20 206f 626a 6563 7473 2069 6e20  le.  objects in 
-00007460: 7468 6569 7220 6f77 6e20 7269 6768 742c  their own right,
-00007470: 2061 6e64 2069 7427 7320 706f 7373 6962   and it's possib
-00007480: 6c65 2074 6f20 6174 7461 6368 206f 6273  le to attach obs
-00007490: 6572 7665 7273 2074 6f20 7468 656d 0a20  ervers to them. 
-000074a0: 2064 6972 6563 746c 792e 2054 6865 7365   directly. These
-000074b0: 2063 6c61 7373 6573 2077 6572 6520 7072   classes were pr
-000074c0: 696d 6172 696c 7920 696e 7472 6f64 7563  imarily introduc
-000074d0: 6564 2074 6f20 7375 7070 6f72 7420 7468  ed to support th
-000074e0: 6520 6e65 770a 2020 6f62 7365 7276 6174  e new.  observat
-000074f0: 696f 6e20 6672 616d 6577 6f72 6b2c 2061  ion framework, a
-00007500: 6e64 2061 7265 206e 6f74 2065 7870 6563  nd are not expec
-00007510: 7465 6420 746f 2062 6520 7573 6564 2064  ted to be used d
-00007520: 6972 6563 746c 792e 2054 6865 2041 5049  irectly. The API
-00007530: 2066 6f72 0a20 2074 6865 7365 206f 626a   for.  these obj
-00007540: 6563 7473 2061 6e64 2074 6865 6972 206e  ects and their n
-00007550: 6f74 6966 6963 6174 696f 6e20 7379 7374  otification syst
-00007560: 656d 2069 7320 7072 6f76 6973 696f 6e61  em is provisiona
-00007570: 6c2c 2061 6e64 206d 6179 2063 6861 6e67  l, and may chang
-00007580: 6520 696e 0a20 2061 2066 7574 7572 6520  e in.  a future 
-00007590: 5472 6169 7473 2072 656c 6561 7365 2e0a  Traits release..
-000075a0: 0a2a 2041 206e 6577 203a 636c 6173 733a  .* A new :class:
-000075b0: 602e 556e 696f 6e60 2074 7261 6974 2074  `.Union` trait t
-000075c0: 7970 6520 6861 7320 6265 656e 2061 6464  ype has been add
-000075d0: 6564 2e20 5468 6973 2069 7320 696e 7465  ed. This is inte
-000075e0: 6e64 6564 2061 7320 610a 2020 7369 6d70  nded as a.  simp
-000075f0: 6c65 7220 7265 706c 6163 656d 656e 7420  ler replacement 
-00007600: 666f 7220 7468 6520 6578 6973 7469 6e67  for the existing
-00007610: 203a 636c 6173 733a 602e 4569 7468 6572   :class:`.Either
-00007620: 6020 7472 6169 7420 7479 7065 2c20 7768  ` trait type, wh
-00007630: 6963 680a 2020 7769 6c6c 2065 7665 6e74  ich.  will event
-00007640: 7561 6c6c 7920 6265 2064 6570 7265 6361  ually be depreca
-00007650: 7465 642e 0a0a 2a20 4e65 7720 3a63 6c61  ted...* New :cla
-00007660: 7373 3a60 2e50 7265 6669 784c 6973 7460  ss:`.PrefixList`
-00007670: 2c20 3a63 6c61 7373 3a60 2e50 7265 6669  , :class:`.Prefi
-00007680: 784d 6170 6020 616e 6420 3a63 6c61 7373  xMap` and :class
-00007690: 3a60 2e4d 6170 6020 7472 6169 7420 7479  :`.Map` trait ty
-000076a0: 7065 730a 2020 6861 7665 2062 6565 6e20  pes.  have been 
-000076b0: 6164 6465 642e 2054 6865 7365 2072 6570  added. These rep
-000076c0: 6c61 6365 2074 6865 2065 7869 7374 696e  lace the existin
-000076d0: 6720 3a63 6c61 7373 3a60 2e54 7261 6974  g :class:`.Trait
-000076e0: 5072 6566 6978 4c69 7374 602c 0a20 203a  PrefixList`,.  :
-000076f0: 636c 6173 733a 602e 5472 6169 7450 7265  class:`.TraitPre
-00007700: 6669 784d 6170 6020 616e 6420 3a63 6c61  fixMap` and :cla
-00007710: 7373 3a60 2e54 7261 6974 4d61 7060 2073  ss:`.TraitMap` s
-00007720: 7562 636c 6173 7365 7320 6f66 0a20 203a  ubclasses of.  :
-00007730: 636c 6173 733a 602e 5472 6169 7448 616e  class:`.TraitHan
-00007740: 646c 6572 602c 2077 6869 6368 2061 7265  dler`, which are
-00007750: 2064 6570 7265 6361 7465 642e 0a0a 2a20   deprecated...* 
-00007760: 5479 7069 6e67 2073 7475 6273 2066 6f72  Typing stubs for
-00007770: 2074 6865 2054 7261 6974 7320 6c69 6272   the Traits libr
-00007780: 6172 7920 6861 7665 2062 6565 6e20 6164  ary have been ad
-00007790: 6465 6420 696e 2061 0a20 2060 6074 7261  ded in a.  ``tra
-000077a0: 6974 732d 7374 7562 7360 6020 7061 636b  its-stubs`` pack
-000077b0: 6167 652c 2077 6869 6368 2077 696c 6c20  age, which will 
-000077c0: 6265 2072 656c 6561 7365 6420 7365 7061  be released sepa
-000077d0: 7261 7465 6c79 2074 6f20 5079 5049 2e20  rately to PyPI. 
-000077e0: 5468 6973 0a20 2073 686f 756c 6420 6865  This.  should he
-000077f0: 6c70 2073 7570 706f 7274 2054 7261 6974  lp support Trait
-00007800: 732d 7573 696e 6720 7072 6f6a 6563 7473  s-using projects
-00007810: 2074 6861 7420 7761 6e74 2074 6f20 6d61   that want to ma
-00007820: 6b65 2075 7365 206f 6620 7479 7065 0a20  ke use of type. 
-00007830: 2061 6e6e 6f74 6174 696f 6e73 2061 6e64   annotations and
-00007840: 2074 7970 6520 6368 6563 6b65 7273 206c   type checkers l
-00007850: 696b 6520 606d 7970 7920 3c68 7474 703a  ike `mypy <http:
-00007860: 2f2f 6d79 7079 2d6c 616e 672e 6f72 672f  //mypy-lang.org/
-00007870: 3e60 5f2e 0a0a 0a4e 6f74 6573 206f 6e20  >`_....Notes on 
-00007880: 7570 6772 6164 696e 670a 7e7e 7e7e 7e7e  upgrading.~~~~~~
-00007890: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4173  ~~~~~~~~~~~~..As
-000078a0: 2066 6172 2061 7320 706f 7373 6962 6c65   far as possible
-000078b0: 2c20 5472 6169 7473 2036 2e31 2069 7320  , Traits 6.1 is 
-000078c0: 6261 636b 7761 7264 7320 636f 6d70 6174  backwards compat
-000078d0: 6962 6c65 2077 6974 6820 5472 6169 7473  ible with Traits
-000078e0: 2036 2e30 2e0a 486f 7765 7665 722c 2074   6.0..However, t
-000078f0: 6865 7265 2061 7265 2061 2066 6577 2074  here are a few t
-00007900: 6869 6e67 7320 746f 2062 6520 6177 6172  hings to be awar
-00007910: 6520 6f66 2077 6865 6e20 7570 6772 6164  e of when upgrad
-00007920: 696e 672e 0a0a 2a20 5472 6169 7473 2036  ing...* Traits 6
-00007930: 2e31 2069 7320 6e6f 7420 636f 6d70 6174  .1 is not compat
-00007940: 6962 6c65 2077 6974 6820 5472 6169 7473  ible with Traits
-00007950: 5549 2076 6572 7369 6f6e 7320 6f6c 6465  UI versions olde
-00007960: 7220 7468 616e 2054 7261 6974 7355 4920  r than TraitsUI 
-00007970: 372e 302e 0a20 2041 2063 6f6d 6269 6e61  7.0..  A combina
-00007980: 7469 6f6e 206f 6620 5472 6169 7473 2036  tion of Traits 6
-00007990: 2e31 206f 7220 6c61 7465 7220 7769 7468  .1 or later with
-000079a0: 2054 7261 6974 7355 4920 362e 7820 6f72   TraitsUI 6.x or
-000079b0: 2065 6172 6c69 6572 2077 696c 6c20 6661   earlier will fa
-000079c0: 696c 0a20 2074 6f20 7072 6f70 6572 6c79  il.  to properly
-000079d0: 2072 6563 6f67 6e69 7365 203a 636c 6173   recognise :clas
-000079e0: 733a 607e 7472 6169 7473 7569 2e76 6965  s:`~traitsui.vie
-000079f0: 772e 5669 6577 6020 636c 6173 7320 7661  w.View` class va
-00007a00: 7269 6162 6c65 7320 6173 0a20 2054 7261  riables as.  Tra
-00007a10: 6974 7355 4920 7669 6577 732c 2061 6e64  itsUI views, and
-00007a20: 2061 6e20 6572 726f 7220 7769 6c6c 2062   an error will b
-00007a30: 6520 7261 6973 6564 2069 6620 796f 7520  e raised if you 
-00007a40: 6174 7465 6d70 7420 746f 2063 7265 6174  attempt to creat
-00007a50: 6520 610a 2020 5472 6169 7473 5549 2076  e a.  TraitsUI v
-00007a60: 6965 772e 0a0a 2a20 5472 6169 7473 206e  iew...* Traits n
-00007a70: 6f77 2064 6f65 7320 6e6f 206c 6f67 6769  ow does no loggi
-00007a80: 6e67 2063 6f6e 6669 6775 7261 7469 6f6e  ng configuration
-00007a90: 2061 7420 616c 6c2c 206c 6561 7669 6e67   at all, leaving
-00007aa0: 2061 6c6c 2073 7563 680a 2020 636f 6e66   all such.  conf
-00007ab0: 6967 7572 6174 696f 6e20 746f 2074 6865  iguration to the
-00007ac0: 2061 7070 6c69 6361 7469 6f6e 2e0a 0a20   application... 
-00007ad0: 2049 6e20 6d6f 7265 2064 6574 6169 6c3a   In more detail:
-00007ae0: 2074 7261 6974 206e 6f74 6966 6963 6174   trait notificat
-00007af0: 696f 6e20 6861 6e64 6c65 7273 2073 686f  ion handlers sho
-00007b00: 756c 6420 6e6f 7420 7261 6973 6520 6578  uld not raise ex
-00007b10: 6365 7074 696f 6e73 2069 6e0a 2020 6e6f  ceptions in.  no
-00007b20: 726d 616c 2075 7365 2c20 736f 2061 6e20  rmal use, so an 
-00007b30: 6578 6365 7074 696f 6e20 6973 206c 6f67  exception is log
-00007b40: 6765 6420 7768 656e 6576 6572 2061 2074  ged whenever a t
-00007b50: 7261 6974 206e 6f74 6966 6963 6174 696f  rait notificatio
-00007b60: 6e20 6861 6e64 6c65 720a 2020 7261 6973  n handler.  rais
-00007b70: 6573 2e20 5468 6973 2070 6172 7420 6f66  es. This part of
-00007b80: 2074 6865 2062 6568 6176 696f 7572 2068   the behaviour h
-00007b90: 6173 206e 6f74 2063 6861 6e67 6564 2e20  as not changed. 
-00007ba0: 5768 6174 202a 6861 732a 2063 6861 6e67  What *has* chang
-00007bb0: 6564 2069 7320 7468 650a 2020 7761 7920  ed is the.  way 
-00007bc0: 7468 6174 206c 6f67 6765 6420 6578 6365  that logged exce
-00007bd0: 7074 696f 6e20 6973 2068 616e 646c 6564  ption is handled
-00007be0: 2075 6e64 6572 2064 6566 6175 6c74 2065   under default e
-00007bf0: 7863 6570 7469 6f6e 2068 616e 646c 696e  xception handlin
-00007c00: 672e 0a0a 2020 5072 6576 696f 7573 6c79  g...  Previously
-00007c10: 2c20 5472 6169 7473 2061 6464 6564 2061  , Traits added a
-00007c20: 203a 636c 6173 733a 607e 6c6f 6767 696e   :class:`~loggin
-00007c30: 672e 5374 7265 616d 4861 6e64 6c65 7260  g.StreamHandler`
-00007c40: 2074 6f20 7468 650a 2020 746f 702d 6c65   to the.  top-le
-00007c50: 7665 6c20 6060 2274 7261 6974 7322 6060  vel ``"traits"``
-00007c60: 206c 6f67 6765 722c 2073 6f20 7468 6174   logger, so that
-00007c70: 2074 7261 6974 206e 6f74 6966 6963 6174   trait notificat
-00007c80: 696f 6e20 6578 6365 7074 696f 6e73 2077  ion exceptions w
-00007c90: 6f75 6c64 0a20 2061 6c77 6179 7320 6265  ould.  always be
-00007ca0: 2076 6973 6962 6c65 2e20 5472 6169 7473   visible. Traits
-00007cb0: 2061 6c73 6f20 6164 6465 6420 6120 3a63   also added a :c
-00007cc0: 6c61 7373 3a60 7e6c 6f67 6769 6e67 2e4e  lass:`~logging.N
-00007cd0: 756c 6c48 616e 646c 6572 6020 746f 2074  ullHandler` to t
-00007ce0: 6861 740a 2020 6c6f 6767 6572 2e20 426f  hat.  logger. Bo
-00007cf0: 7468 206f 6620 7468 6f73 6520 6861 6e64  th of those hand
-00007d00: 6c65 7273 2068 6176 6520 6e6f 7720 6265  lers have now be
-00007d10: 656e 2072 656d 6f76 6564 2e20 5765 206e  en removed. We n
-00007d20: 6f77 2072 656c 7920 6f6e 0a20 2050 7974  ow rely on.  Pyt
-00007d30: 686f 6e27 7320 2268 616e 646c 6572 206f  hon's "handler o
-00007d40: 6620 6c61 7374 2072 6573 6f72 7422 2c20  f last resort", 
-00007d50: 7768 6963 6820 7769 6c6c 2063 6f6e 7469  which will conti
-00007d60: 6e75 6520 746f 206d 616b 6520 6e6f 7469  nue to make noti
-00007d70: 6669 6361 7469 6f6e 0a20 2065 7863 6570  fication.  excep
-00007d80: 7469 6f6e 7320 746f 2074 6865 2075 7365  tions to the use
-00007d90: 7220 7669 7369 626c 6520 696e 2074 6865  r visible in the
-00007da0: 2061 6273 656e 6365 206f 6620 616e 7920   absence of any 
-00007db0: 6170 706c 6963 6174 696f 6e2d 6c65 7665  application-leve
-00007dc0: 6c0a 2020 6c6f 6720 636f 6e66 6967 7572  l.  log configur
-00007dd0: 6174 696f 6e2e 0a0a 2a20 5768 656e 206c  ation...* When l
-00007de0: 6973 7465 6e69 6e67 2066 6f72 2063 6861  istening for cha
-00007df0: 6e67 6573 2074 6f20 7468 6520 6974 656d  nges to the item
-00007e00: 7320 6f66 2061 203a 636c 6173 733a 602e  s of a :class:`.
-00007e10: 4c69 7374 6020 7472 6169 742c 2061 6e20  List` trait, an 
-00007e20: 696e 6465 780a 2020 6f72 2073 6c69 6365  index.  or slice
-00007e30: 2073 6574 206f 7065 7261 7469 6f6e 206e   set operation n
-00007e40: 6f20 6c6f 6e67 6572 2070 6572 666f 726d  o longer perform
-00007e50: 7320 616e 2065 7175 616c 6974 7920 6368  s an equality ch
-00007e60: 6563 6b20 6265 7477 6565 6e20 7468 650a  eck between the.
-00007e70: 2020 7265 706c 6163 6564 2065 6c65 6d65    replaced eleme
-00007e80: 6e74 7320 616e 6420 7468 6520 7265 706c  nts and the repl
-00007e90: 6163 656d 656e 7420 656c 656d 656e 7473  acement elements
-00007ea0: 2077 6865 6e20 6465 6369 6469 6e67 2077   when deciding w
-00007eb0: 6865 7468 6572 2074 6f20 6973 7375 650a  hether to issue.
-00007ec0: 2020 6120 6e6f 7469 6669 6361 7469 6f6e    a notification
-00007ed0: 3b20 696e 7374 6561 642c 2061 206e 6f74  ; instead, a not
-00007ee0: 6966 6963 6174 696f 6e20 6973 2061 6c77  ification is alw
-00007ef0: 6179 7320 6973 7375 6564 2069 6620 6174  ays issued if at
-00007f00: 206c 6561 7374 206f 6e65 0a20 2065 6c65   least one.  ele
-00007f10: 6d65 6e74 2077 6173 2072 6570 6c61 6365  ment was replace
-00007f20: 642e 2046 6f72 2065 7861 6d70 6c65 2c20  d. For example, 
-00007f30: 636f 6e73 6964 6572 2074 6865 2066 6f6c  consider the fol
-00007f40: 6c6f 7769 6e67 2063 6c61 7373 3a3a 0a0a  lowing class::..
-00007f50: 2020 2020 636c 6173 7320 5365 6c65 6374      class Select
-00007f60: 696f 6e28 4861 7354 7261 6974 7329 3a0a  ion(HasTraits):.
-00007f70: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-00007f80: 3d20 4c69 7374 2849 6e74 290a 0a20 2020  = List(Int)..   
-00007f90: 2020 2020 2040 6f6e 5f74 7261 6974 5f63       @on_trait_c
-00007fa0: 6861 6e67 6528 2269 6e64 6963 6573 5f69  hange("indices_i
-00007fb0: 7465 6d73 2229 0a20 2020 2020 2020 2064  tems").        d
-00007fc0: 6566 2072 6570 6f72 745f 6368 616e 6765  ef report_change
-00007fd0: 2873 656c 662c 2065 7665 6e74 293a 0a20  (self, event):. 
-00007fe0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00007ff0: 2822 496e 6469 6365 7320 6368 616e 6765  ("Indices change
-00008000: 643a 2022 2c20 6576 656e 7429 0a0a 2020  d: ", event)..  
-00008010: 5768 656e 2072 6570 6c61 6369 6e67 2074  When replacing t
-00008020: 6865 2060 3860 2077 6974 6820 7468 6520  he `8` with the 
-00008030: 7361 6d65 2069 6e74 6567 6572 2c20 7765  same integer, we
-00008040: 2067 6574 2074 6869 7320 6265 6861 7669   get this behavi
-00008050: 6f72 3a3a 0a0a 2020 2020 3e3e 3e20 7365  or::..    >>> se
-00008060: 6c65 6374 696f 6e20 3d20 5365 6c65 6374  lection = Select
-00008070: 696f 6e28 696e 6469 6365 733d 5b32 2c20  ion(indices=[2, 
-00008080: 352c 2038 5d29 0a20 2020 203e 3e3e 2073  5, 8]).    >>> s
-00008090: 656c 6563 7469 6f6e 2e69 6e64 6963 6573  election.indices
-000080a0: 5b32 5d20 3d20 380a 2020 2020 496e 6469  [2] = 8.    Indi
-000080b0: 6365 7320 6368 616e 6765 643a 2020 5472  ces changed:  Tr
-000080c0: 6169 744c 6973 7445 7665 6e74 2869 6e64  aitListEvent(ind
-000080d0: 6578 3d32 2c20 7265 6d6f 7665 643d 5b38  ex=2, removed=[8
-000080e0: 5d2c 2061 6464 6564 3d5b 385d 290a 0a20  ], added=[8]).. 
-000080f0: 2050 7265 7669 6f75 736c 792c 206e 6f20   Previously, no 
-00008100: 6e6f 7469 6669 6361 7469 6f6e 2077 6f75  notification wou
-00008110: 6c64 2068 6176 6520 6265 656e 2069 7373  ld have been iss
-00008120: 7565 642e 0a0a 2a20 5468 6520 3a66 756e  ued...* The :fun
-00008130: 633a 602e 436f 6c6f 7260 2c20 3a66 756e  c:`.Color`, :fun
-00008140: 633a 602e 5247 4243 6f6c 6f72 6020 616e  c:`.RGBColor` an
-00008150: 6420 3a66 756e 633a 602e 466f 6e74 6020  d :func:`.Font` 
-00008160: 7472 6169 7420 6661 6374 6f72 6965 730a  trait factories.
-00008170: 2020 6861 7665 206d 6f76 6564 2074 6f20    have moved to 
-00008180: 5472 6169 7473 5549 2c20 616e 6420 7368  TraitsUI, and sh
-00008190: 6f75 6c64 2062 6520 696d 706f 7274 6564  ould be imported
-000081a0: 2066 726f 6d20 7468 6572 6520 7261 7468   from there rath
-000081b0: 6572 2074 6861 6e20 6672 6f6d 0a20 2054  er than from.  T
-000081c0: 7261 6974 732e 2046 6f72 2062 6163 6b77  raits. For backw
-000081d0: 6172 6473 2063 6f6d 7061 7469 6269 6c69  ards compatibili
-000081e0: 7479 2c20 7468 6520 6661 6374 6f72 6965  ty, the factorie
-000081f0: 7320 6172 6520 7374 696c 6c0a 2020 6176  s are still.  av
-00008200: 6169 6c61 626c 6520 696e 2054 7261 6974  ailable in Trait
-00008210: 732c 2062 7574 2074 6865 7920 6172 6520  s, but they are 
-00008220: 6465 7072 6563 6174 6564 2061 6e64 2077  deprecated and w
-00008230: 696c 6c20 6576 656e 7475 616c 6c79 0a20  ill eventually. 
-00008240: 2062 6520 7265 6d6f 7665 642e 0a0a 2a20   be removed...* 
-00008250: 4173 2061 2072 656d 696e 6465 722c 2074  As a reminder, t
-00008260: 6865 203a 6461 7461 3a60 2e55 6e69 636f  he :data:`.Unico
-00008270: 6465 6020 616e 6420 3a64 6174 613a 602e  de` and :data:`.
-00008280: 4c6f 6e67 6020 7472 6169 7420 7479 7065  Long` trait type
-00008290: 7320 6172 650a 2020 6465 7072 6563 6174  s are.  deprecat
-000082a0: 6564 2073 696e 6365 2054 7261 6974 7320  ed since Traits 
-000082b0: 362e 302e 2050 6c65 6173 6520 7265 706c  6.0. Please repl
-000082c0: 6163 6520 7573 6573 2077 6974 6820 3a63  ace uses with :c
-000082d0: 6c61 7373 3a60 2e53 7472 6020 616e 640a  lass:`.Str` and.
-000082e0: 2020 3a63 6c61 7373 3a60 2e49 6e74 6020    :class:`.Int` 
-000082f0: 7265 7370 6563 7469 7665 6c79 2e20 546f  respectively. To
-00008300: 2061 766f 6964 2065 7863 6573 7369 7665   avoid excessive
-00008310: 206e 6f69 7365 2069 6e20 5472 6169 7473   noise in Traits
-00008320: 2d75 7369 6e67 0a20 2070 726f 6a65 6374  -using.  project
-00008330: 732c 2054 7261 6974 7320 646f 6573 206e  s, Traits does n
-00008340: 6f74 2079 6574 2069 7373 7565 2064 6570  ot yet issue dep
-00008350: 7265 6361 7469 6f6e 2077 6172 6e69 6e67  recation warning
-00008360: 7320 666f 7220 6578 6973 7469 6e67 2075  s for existing u
-00008370: 7365 7320 6f66 0a20 203a 6461 7461 3a60  ses of.  :data:`
-00008380: 2e55 6e69 636f 6465 6020 616e 6420 3a64  .Unicode` and :d
-00008390: 6174 613a 602e 4c6f 6e67 602e 2054 686f  ata:`.Long`. Tho
-000083a0: 7365 2077 6172 6e69 6e67 7320 7769 6c6c  se warnings will
-000083b0: 2062 6520 696e 7472 6f64 7563 6564 2069   be introduced i
-000083c0: 6e20 610a 2020 6675 7475 7265 2054 7261  n a.  future Tra
-000083d0: 6974 7320 7265 6c65 6173 652c 2070 7269  its release, pri
-000083e0: 6f72 2074 6f20 7468 6520 7265 6d6f 7661  or to the remova
-000083f0: 6c20 6f66 2074 6865 7365 2074 7261 6974  l of these trait
-00008400: 2074 7970 6573 2e0a 0a0a 5065 6e64 696e   types....Pendin
-00008410: 6720 6465 7072 6563 6174 696f 6e73 0a7e  g deprecations.~
-00008420: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00008430: 7e7e 7e0a 0a49 6e20 6164 6469 7469 6f6e  ~~~..In addition
-00008440: 2074 6f20 7468 6520 6465 7072 6563 6174   to the deprecat
-00008450: 696f 6e73 206c 6973 7465 6420 696e 2074  ions listed in t
-00008460: 6865 2063 6861 6e67 656c 6f67 2062 656c  he changelog bel
-00008470: 6f77 2c20 736f 6d65 2070 6172 7473 206f  ow, some parts o
-00008480: 660a 7468 6520 5472 6169 7473 206c 6962  f.the Traits lib
-00008490: 7261 7279 2061 7265 206e 6f74 2079 6574  rary are not yet
-000084a0: 2066 6f72 6d61 6c6c 7920 6465 7072 6563   formally deprec
-000084b0: 6174 6564 2c20 6275 7420 6172 6520 6c69  ated, but are li
-000084c0: 6b65 6c79 2074 6f20 6265 0a64 6570 7265  kely to be.depre
-000084d0: 6361 7465 6420 6265 666f 7265 2054 7261  cated before Tra
-000084e0: 6974 7320 372e 302e 2055 7365 7273 2073  its 7.0. Users s
-000084f0: 686f 756c 6420 6265 2061 7761 7265 206f  hould be aware o
-00008500: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
-00008510: 706f 7373 6962 6c65 0a66 7574 7572 6520  possible.future 
-00008520: 6368 616e 6765 733a 0a0a 2a20 5468 6520  changes:..* The 
-00008530: 3a63 6c61 7373 3a60 2e45 6974 6865 7260  :class:`.Either`
-00008540: 2074 7261 6974 2074 7970 6520 7769 6c6c   trait type will
-00008550: 2065 7665 6e74 7561 6c6c 7920 6265 2064   eventually be d
-00008560: 6570 7265 6361 7465 642e 2057 6865 7265  eprecated. Where
-00008570: 0a20 2070 6f73 7369 626c 652c 2075 7365  .  possible, use
-00008580: 203a 636c 6173 733a 602e 556e 696f 6e60   :class:`.Union`
-00008590: 2069 6e73 7465 6164 2e20 5768 656e 2072   instead. When r
-000085a0: 6570 6c61 6369 6e67 2075 7365 7320 6f66  eplacing uses of
-000085b0: 0a20 203a 636c 6173 733a 602e 4569 7468  .  :class:`.Eith
-000085c0: 6572 6020 7769 7468 203a 636c 6173 733a  er` with :class:
-000085d0: 602e 556e 696f 6e60 2c20 6e6f 7465 2074  `.Union`, note t
-000085e0: 6861 7420 7468 6572 6520 6172 6520 736f  hat there are so
-000085f0: 6d65 2073 6967 6e69 6669 6361 6e74 0a20  me significant. 
-00008600: 2041 5049 2061 6e64 2062 6568 6176 696f   API and behavio
-00008610: 7261 6c20 6469 6666 6572 656e 6365 7320  ral differences 
-00008620: 6265 7477 6565 6e20 7468 6520 7477 6f20  between the two 
-00008630: 7472 6169 7420 7479 7065 732c 2070 6172  trait types, par
-00008640: 7469 6375 6c61 726c 7920 7769 7468 0a20  ticularly with. 
-00008650: 2072 6573 7065 6374 2074 6f20 6861 6e64   respect to hand
-00008660: 6c69 6e67 206f 6620 6465 6661 756c 7473  ling of defaults
-00008670: 2e20 5365 6520 3a72 6566 3a60 6d69 6772  . See :ref:`migr
-00008680: 6174 696f 6e5f 6569 7468 6572 5f74 6f5f  ation_either_to_
-00008690: 756e 696f 6e60 2066 6f72 0a20 206d 6f72  union` for.  mor
-000086a0: 6520 6465 7461 696c 732e 0a0a 2a20 5468  e details...* Th
-000086b0: 6520 6060 7472 6169 745f 6d6f 6469 6669  e ``trait_modifi
-000086c0: 6564 6060 2065 7665 6e74 2074 7261 6974  ed`` event trait
-000086d0: 2074 6861 7427 7320 7072 6573 656e 7420   that's present 
-000086e0: 6f6e 2061 6c6c 203a 636c 6173 733a 602e  on all :class:`.
-000086f0: 4861 7354 7261 6974 7360 0a20 2073 7562  HasTraits`.  sub
-00008700: 636c 6173 7365 7320 7769 6c6c 2065 7665  classes will eve
-00008710: 6e74 7561 6c6c 7920 6265 2072 656d 6f76  ntually be remov
-00008720: 6564 2e20 5573 6572 7320 7368 6f75 6c64  ed. Users should
-00008730: 206e 6f74 2072 656c 7920 6f6e 2069 7420   not rely on it 
-00008740: 6265 696e 670a 2020 7072 6573 656e 7420  being.  present 
-00008750: 696e 2061 6e20 6f62 6a65 6374 2773 2060  in an object's `
-00008760: 6063 6c61 7373 5f74 7261 6974 7360 6020  `class_traits`` 
-00008770: 6469 6374 696f 6e61 7279 2e0a 0a2a 2054  dictionary...* T
-00008780: 7261 6974 206e 616d 6573 2073 7461 7274  rait names start
-00008790: 696e 6720 7769 7468 2060 6074 7261 6974  ing with ``trait
-000087a0: 6060 2c20 6060 7472 6169 7473 6060 2c20  ``, ``traits``, 
-000087b0: 6060 5f74 7261 6974 6060 206f 720a 2020  ``_trait`` or.  
-000087c0: 6060 5f74 7261 6974 7360 6020 6d61 7920  ``_traits`` may 
-000087d0: 6265 636f 6d65 2072 6573 6572 7665 6420  become reserved 
-000087e0: 666f 7220 7573 6520 6279 2045 5453 2061  for use by ETS a
-000087f0: 7420 736f 6d65 2070 6f69 6e74 2069 6e20  t some point in 
-00008800: 7468 6520 6675 7475 7265 2e0a 2020 4176  the future..  Av
-00008810: 6f69 6420 7573 696e 6720 7468 6573 6520  oid using these 
-00008820: 6e61 6d65 7320 666f 7220 796f 7572 206f  names for your o
-00008830: 776e 2074 7261 6974 732e 0a0a 4465 7461  wn traits...Deta
-00008840: 696c 6564 2050 522d 6279 2d50 5220 6368  iled PR-by-PR ch
-00008850: 616e 6765 730a 7e7e 7e7e 7e7e 7e7e 7e7e  anges.~~~~~~~~~~
-00008860: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
-00008870: 0a4d 6f72 6520 7468 616e 2031 3630 2050  .More than 160 P
-00008880: 5273 2077 656e 7420 696e 746f 2074 6869  Rs went into thi
-00008890: 7320 7265 6c65 6173 652e 2054 6865 2066  s release. The f
-000088a0: 6f6c 6c6f 7769 6e67 2070 656f 706c 6520  ollowing people 
-000088b0: 636f 6e74 7269 6275 7465 640a 636f 6465  contributed.code
-000088c0: 2063 6861 6e67 6573 2066 6f72 2074 6869   changes for thi
-000088d0: 7320 7265 6c65 6173 653a 0a0a 2a20 4965  s release:..* Ie
-000088e0: 7661 2043 6572 6e79 7465 0a2a 204b 6974  va Cernyte.* Kit
-000088f0: 2059 616e 2043 686f 690a 2a20 4d61 7869   Yan Choi.* Maxi
-00008900: 6d65 2043 6f73 7461 6c6f 6e67 610a 2a20  me Costalonga.* 
-00008910: 4d61 726b 2044 6963 6b69 6e73 6f6e 0a2a  Mark Dickinson.*
-00008920: 204d 6174 7420 4861 6e63 6f63 6b0a 2a20   Matt Hancock.* 
-00008930: 4d69 6468 756e 204d 6164 6875 736f 6f64  Midhun Madhusood
-00008940: 616e 616e 0a2a 2053 686f 6562 204d 6f68  anan.* Shoeb Moh
-00008950: 616d 6d65 640a 2a20 4672 616e 6b6c 696e  ammed.* Franklin
-00008960: 2056 656e 7475 7261 0a2a 2043 6f72 7261   Ventura.* Corra
-00008970: 6e20 5765 6273 7465 720a 0a46 6561 7475  n Webster..Featu
-00008980: 7265 730a 7e7e 7e7e 7e7e 7e7e 0a0a 2a20  res.~~~~~~~~..* 
-00008990: 4164 6420 6060 6f73 2e50 6174 684c 696b  Add ``os.PathLik
-000089a0: 6560 6020 7375 7070 6f72 7420 666f 7220  e`` support for 
-000089b0: 6060 4469 7265 6374 6f72 7960 6020 7472  ``Directory`` tr
-000089c0: 6169 7473 2e20 2823 3836 3729 0a2a 2041  aits. (#867).* A
-000089d0: 6464 2060 6055 6e69 6f6e 6060 2074 7261  dd ``Union`` tra
-000089e0: 6974 2074 7970 652e 2028 2337 3739 2c20  it type. (#779, 
-000089f0: 2331 3130 332c 2023 3131 3037 2c20 2331  #1103, #1107, #1
-00008a00: 3131 362c 2023 3131 3135 290a 2a20 4164  116, #1115).* Ad
-00008a10: 6420 6060 5072 6566 6978 4c69 7374 6060  d ``PrefixList``
-00008a20: 2074 7261 6974 2074 7970 652e 2028 2338   trait type. (#8
-00008a30: 3731 2c20 2331 3134 322c 2023 3131 3434  71, #1142, #1144
-00008a40: 2c20 2331 3134 3729 0a2a 2041 6464 2060  , #1147).* Add `
-00008a50: 6061 6c6c 6f77 5f6e 6f6e 6560 6020 666c  `allow_none`` fl
-00008a60: 6167 2066 6f72 2060 6043 616c 6c61 626c  ag for ``Callabl
-00008a70: 6560 6020 7472 6169 742e 2028 2338 3835  e`` trait. (#885
-00008a80: 290a 2a20 4164 6420 7375 7070 6f72 7420  ).* Add support 
-00008a90: 666f 7220 7479 7065 2061 6e6e 6f74 6174  for type annotat
-00008aa0: 696f 6e2e 2028 2339 3034 2c20 2331 3036  ion. (#904, #106
-00008ab0: 3429 0a2a 2041 6c6c 6f77 206d 7574 6162  4).* Allow mutab
-00008ac0: 6c65 2076 616c 7565 7320 696e 2060 6043  le values in ``C
-00008ad0: 6f6e 7374 616e 7460 6020 7472 6169 742e  onstant`` trait.
-00008ae0: 2028 2339 3239 290a 2a20 4164 6420 6060   (#929).* Add ``
-00008af0: 4d61 7060 6020 616e 6420 6060 5072 6566  Map`` and ``Pref
-00008b00: 6978 4d61 7060 6020 7472 6169 7420 7479  ixMap`` trait ty
-00008b10: 7065 732e 2028 2338 3836 2c20 2339 3533  pes. (#886, #953
-00008b20: 2c20 2339 3536 2c20 2339 3730 2c20 2331  , #956, #970, #1
-00008b30: 3133 392c 0a20 2023 3131 3839 290a 2a20  139,.  #1189).* 
-00008b40: 4164 6420 6060 5472 6169 744c 6973 7460  Add ``TraitList`
-00008b50: 6020 6173 2074 6865 2062 6173 6520 6c69  ` as the base li
-00008b60: 7374 206f 626a 6563 7420 7468 6174 2063  st object that c
-00008b70: 616e 2070 6572 666f 726d 2076 616c 6964  an perform valid
-00008b80: 6174 696f 6e0a 2020 616e 6420 656d 6974  ation.  and emit
-00008b90: 2063 6861 6e67 6520 6e6f 7469 6669 6361   change notifica
-00008ba0: 7469 6f6e 732e 2028 2339 3132 2c20 2339  tions. (#912, #9
-00008bb0: 3831 2c20 2339 3834 2c20 2339 3839 2c20  81, #984, #989, 
-00008bc0: 2339 3939 2c20 2331 3030 332c 2023 3130  #999, #1003, #10
-00008bd0: 3131 2c0a 2020 2331 3032 362c 2023 3130  11,.  #1026, #10
-00008be0: 3039 2c20 2331 3034 302c 2023 3131 3732  09, #1040, #1172
-00008bf0: 2c20 2331 3137 3329 0a2a 2041 6464 2060  , #1173).* Add `
-00008c00: 6054 7261 6974 4469 6374 6060 2061 7320  `TraitDict`` as 
-00008c10: 7468 6520 6261 7365 2064 6963 7420 6f62  the base dict ob
-00008c20: 6a65 6374 2074 6861 7420 6361 6e20 7065  ject that can pe
-00008c30: 7266 6f72 6d20 7661 6c69 6461 7469 6f6e  rform validation
-00008c40: 2061 6e64 0a20 2065 6d69 7420 6368 616e   and.  emit chan
-00008c50: 6765 206e 6f74 6966 6963 6174 696f 6e73  ge notifications
-00008c60: 2e20 2823 3931 3329 0a2a 2041 6464 2060  . (#913).* Add `
-00008c70: 6054 7261 6974 5365 7460 6020 6173 2074  `TraitSet`` as t
-00008c80: 6865 2062 6173 6520 7365 7420 6f62 6a65  he base set obje
-00008c90: 6374 2074 6861 7420 6361 6e20 7065 7266  ct that can perf
-00008ca0: 6f72 6d20 7661 6c69 6461 7469 6f6e 2061  orm validation a
-00008cb0: 6e64 0a20 2065 6d69 7420 6368 616e 6765  nd.  emit change
-00008cc0: 206e 6f74 6966 6963 6174 696f 6e73 2e20   notifications. 
-00008cd0: 2823 3932 322c 2023 3130 3433 290a 2a20  (#922, #1043).* 
-00008ce0: 496d 706c 656d 656e 7420 6060 6f62 7365  Implement ``obse
-00008cf0: 7276 6560 6020 746f 2073 7570 6572 7365  rve`` to superse
-00008d00: 6465 2060 606f 6e5f 7472 6169 745f 6368  de ``on_trait_ch
-00008d10: 616e 6765 6060 2066 6f72 206f 6273 6572  ange`` for obser
-00008d20: 7669 6e67 2074 7261 6974 0a20 2063 6861  ving trait.  cha
-00008d30: 6e67 6573 2e20 2823 3937 362c 2023 3130  nges. (#976, #10
-00008d40: 3030 2c20 2331 3030 372c 2023 3130 3635  00, #1007, #1065
-00008d50: 2c20 2331 3032 332c 2023 3130 3636 2c20  , #1023, #1066, 
-00008d60: 2331 3037 302c 2023 3130 3639 2c20 2331  #1070, #1069, #1
-00008d70: 3036 372c 0a20 2023 3130 3830 2c20 2331  067,.  #1080, #1
-00008d80: 3038 322c 2023 3130 3739 2c20 2331 3037  082, #1079, #107
-00008d90: 312c 2023 3130 3732 2c20 2331 3037 352c  1, #1072, #1075,
-00008da0: 2023 3130 3835 2c20 2331 3038 392c 2023   #1085, #1089, #
-00008db0: 3130 3738 2c20 2331 3039 332c 2023 3130  1078, #1093, #10
-00008dc0: 3836 2c0a 2020 2331 3037 372c 2023 3130  86,.  #1077, #10
-00008dd0: 3935 2c20 2331 3130 322c 2023 3131 3038  95, #1102, #1108
-00008de0: 2c20 2331 3131 302c 2023 3131 3132 2c20  , #1110, #1112, 
-00008df0: 2331 3131 372c 2023 3131 3138 2c20 2331  #1117, #1118, #1
-00008e00: 3132 332c 2023 3131 3235 2c20 2331 3132  123, #1125, #112
-00008e10: 362c 0a20 2023 3131 3238 2c20 2331 3132  6,.  #1128, #112
-00008e20: 392c 2023 3131 3335 2c20 2331 3135 3629  9, #1135, #1156)
-00008e30: 0a0a 4368 616e 6765 730a 7e7e 7e7e 7e7e  ..Changes.~~~~~~
-00008e40: 7e0a 0a2a 2047 5549 2061 7070 6c69 6361  ~..* GUI applica
-00008e50: 7469 6f6e 7320 7573 696e 6720 5472 6169  tions using Trai
-00008e60: 7473 2036 2e31 2077 696c 6c20 7265 7175  ts 6.1 will requ
-00008e70: 6972 6520 5472 6169 7473 5549 203e 3d20  ire TraitsUI >= 
-00008e80: 372e 302e 2028 2331 3133 3429 0a2a 2060  7.0. (#1134).* `
-00008e90: 6054 7261 6974 5365 7445 7665 6e74 6060  `TraitSetEvent``
-00008ea0: 2061 6e64 2060 6054 7261 6974 4469 6374   and ``TraitDict
-00008eb0: 4576 656e 7460 6020 696e 6974 6961 6c69  Event`` initiali
-00008ec0: 7a61 7469 6f6e 2061 7267 756d 656e 7473  zation arguments
-00008ed0: 2061 7265 206e 6f77 0a20 206b 6579 776f   are now.  keywo
-00008ee0: 7264 2d6f 6e6c 792e 2028 2331 3033 3629  rd-only. (#1036)
-00008ef0: 0a2a 2060 6054 7261 6974 4c69 7374 4f62  .* ``TraitListOb
-00008f00: 6a65 6374 6060 2077 696c 6c20 6e6f 206c  ject`` will no l
-00008f10: 6f6e 6765 7220 736b 6970 206e 6f74 6966  onger skip notif
-00008f20: 6963 6174 696f 6e73 2065 7665 6e20 6966  ications even if
-00008f30: 206d 7574 6174 696f 6e73 0a20 2072 6573   mutations.  res
-00008f40: 756c 7420 696e 2063 6f6e 7465 6e74 2074  ult in content t
-00008f50: 6861 7420 636f 6d70 6172 6573 2065 7175  hat compares equ
-00008f60: 616c 6c79 2074 6f20 7468 6520 6f6c 6420  ally to the old 
-00008f70: 7661 6c75 6573 2e20 2823 3130 3236 290a  values. (#1026).
-00008f80: 2a20 6060 5472 6169 744c 6973 7445 7665  * ``TraitListEve
-00008f90: 6e74 2e69 6e64 6578 6060 2072 6570 6f72  nt.index`` repor
-00008fa0: 7465 6420 6279 206d 7574 6174 696f 6e73  ted by mutations
-00008fb0: 2074 6f20 6120 6c69 7374 2069 7320 6e6f   to a list is no
-00008fc0: 7720 6e6f 726d 616c 697a 6564 2e0a 2020  w normalized..  
-00008fd0: 2823 3130 3039 290a 2a20 5468 6520 6465  (#1009).* The de
-00008fe0: 6661 756c 7420 6e6f 7469 6669 6361 7469  fault notificati
-00008ff0: 6f6e 2065 7272 6f72 2068 616e 646c 6572  on error handler
-00009000: 2066 6f72 2054 7261 6974 7320 6e6f 206c   for Traits no l
-00009010: 6f6e 6765 7220 636f 6e66 6967 7572 6573  onger configures
-00009020: 0a20 206c 6f67 6769 6e67 2c20 616e 6420  .  logging, and 
-00009030: 7468 6520 746f 702d 6c65 7665 6c20 6060  the top-level ``
-00009040: 4e75 6c6c 4861 6e64 6c65 7260 6020 6c6f  NullHandler`` lo
-00009050: 6720 6861 6e64 6c65 7220 6861 7320 6265  g handler has be
-00009060: 656e 2072 656d 6f76 6564 2e0a 2020 2823  en removed..  (#
-00009070: 3131 3631 290a 0a46 6978 6573 0a7e 7e7e  1161)..Fixes.~~~
-00009080: 7e7e 0a2a 2041 6c6c 6f77 2061 7373 6967  ~~.* Allow assig
-00009090: 6e69 6e67 204e 6f6e 6520 746f 2060 6043  ning None to ``C
-000090a0: 5472 6169 742e 706f 7374 5f73 6574 6174  Trait.post_setat
-000090b0: 7472 6060 2e20 2823 3833 3329 0a2a 2046  tr``. (#833).* F
-000090c0: 6978 2072 6566 6572 656e 6365 2063 6f75  ix reference cou
-000090d0: 6e74 2065 7272 6f72 2e20 2823 3930 3729  nt error. (#907)
-000090e0: 0a2a 2049 6d70 726f 7665 2060 6048 6173  .* Improve ``Has
-000090f0: 5472 6169 7473 6060 2069 6e74 726f 7370  Traits`` introsp
-00009100: 6563 7469 6f6e 2077 6974 6820 6060 6469  ection with ``di
-00009110: 7228 2960 602e 2028 2339 3237 290a 2a20  r()``. (#927).* 
-00009120: 4669 7820 7468 6520 6461 7465 7469 6d65  Fix the datetime
-00009130: 2d74 6f2d 7374 7220 636f 6e76 6572 7465  -to-str converte
-00009140: 7273 2075 7365 6420 696e 2060 6044 6174  rs used in ``Dat
-00009150: 6574 696d 6545 6469 746f 7260 602e 2028  etimeEditor``. (
-00009160: 2339 3337 290a 2a20 5261 6973 6520 6060  #937).* Raise ``
-00009170: 5472 6169 744e 6f74 6966 6963 6174 696f  TraitNotificatio
-00009180: 6e45 7272 6f72 6060 206f 6e20 7472 6169  nError`` on trai
-00009190: 6c69 6e67 2063 6f6d 6d61 2069 6e20 6060  ling comma in ``
-000091a0: 6f6e 5f74 7261 6974 5f63 6861 6e67 6560  on_trait_change`
-000091b0: 602e 0a20 2028 2339 3236 290a 2a20 4669  `..  (#926).* Fi
-000091c0: 7820 6578 6365 7074 696f 6e20 7377 616c  x exception swal
-000091d0: 6c6f 7769 6e67 2062 7920 5472 6169 7420  lowing by Trait 
-000091e0: 6174 7472 6962 7574 6520 6163 6365 7373  attribute access
-000091f0: 2e20 2823 3935 392c 2023 3936 3029 0a2a  . (#959, #960).*
-00009200: 2041 6c6c 6f77 2063 6f6c 6c65 6374 696f   Allow collectio
-00009210: 6e73 2069 6e20 7661 6c69 6420 7661 6c75  ns in valid valu
-00009220: 6573 2066 6f72 2060 6045 6e75 6d60 6020  es for ``Enum`` 
-00009230: 7472 6169 742e 2028 2338 3839 290a 2a20  trait. (#889).* 
-00009240: 4669 7820 6060 5472 6169 7445 7272 6f72  Fix ``TraitError
-00009250: 6060 2077 6865 6e20 6d75 7461 7469 6e67  `` when mutating
-00009260: 2061 206c 6973 742f 6469 6374 2f73 6574   a list/dict/set
-00009270: 2069 6e73 6964 6520 616e 6f74 6865 7220   inside another 
-00009280: 636f 6e74 6169 6e65 722e 0a20 2028 2331  container..  (#1
-00009290: 3031 3829 0a2a 2046 6978 2073 6574 7469  018).* Fix setti
-000092a0: 6e67 2064 6566 6175 6c74 2076 616c 7565  ng default value
-000092b0: 7320 7669 6120 6479 6e61 6d69 6320 6465  s via dynamic de
-000092c0: 6661 756c 7420 6d65 7468 6f64 7320 6f72  fault methods or
-000092d0: 206f 7665 7272 6964 696e 6720 7472 6169   overriding trai
-000092e0: 7420 696e 0a20 2073 7562 636c 6173 7365  t in.  subclasse
-000092f0: 7320 666f 7220 6d61 7070 6564 2074 7261  s for mapped tra
-00009300: 6974 732c 2075 7365 6420 6279 2060 604d  its, used by ``M
-00009310: 6170 6060 2c20 6060 4578 7072 6573 7369  ap``, ``Expressi
-00009320: 6f6e 6060 2c20 6060 5072 6566 6978 4d61  on``, ``PrefixMa
-00009330: 7060 602e 0a20 2028 2331 3039 312c 2023  p``..  (#1091, #
-00009340: 3131 3838 290a 2a20 4669 7820 7365 7474  1188).* Fix sett
-00009350: 696e 6720 6465 6661 756c 7420 7661 6c75  ing default valu
-00009360: 6573 2076 6961 2064 796e 616d 6963 2064  es via dynamic d
-00009370: 6566 6175 6c74 206d 6574 686f 6473 206f  efault methods o
-00009380: 7220 6f76 6572 7269 6469 6e67 2074 7261  r overriding tra
-00009390: 6974 2069 6e0a 2020 7375 6263 6c61 7373  it in.  subclass
-000093a0: 6573 2066 6f72 2060 6045 7870 7265 7373  es for ``Express
-000093b0: 696f 6e60 6020 616e 6420 6060 4164 6170  ion`` and ``Adap
-000093c0: 7473 546f 6060 2e20 2823 3130 3838 2c20  tsTo``. (#1088, 
-000093d0: 2331 3131 392c 2023 3131 3532 290a 0a44  #1119, #1152)..D
-000093e0: 6570 7265 6361 7469 6f6e 730a 7e7e 7e7e  eprecations.~~~~
-000093f0: 7e7e 7e7e 7e7e 7e7e 0a0a 2a20 6060 7472  ~~~~~~~~..* ``tr
-00009400: 6169 7473 2e74 6573 7469 6e67 2e6e 6f73  aits.testing.nos
-00009410: 655f 746f 6f6c 7360 6020 6973 2064 6570  e_tools`` is dep
-00009420: 7265 6361 7465 642e 2028 2338 3830 290a  recated. (#880).
-00009430: 2a20 6060 5369 6e67 6c65 746f 6e48 6173  * ``SingletonHas
-00009440: 5472 6169 7473 6060 2c20 6060 5369 6e67  Traits``, ``Sing
-00009450: 6c65 746f 6e48 6173 5374 7269 6374 5472  letonHasStrictTr
-00009460: 6169 7473 6060 2061 6e64 0a20 2060 6053  aits`` and.  ``S
-00009470: 696e 676c 6574 6f6e 4861 7350 7269 7661  ingletonHasPriva
-00009480: 7465 5472 6169 7473 6060 2061 7265 2064  teTraits`` are d
-00009490: 6570 7265 6361 7465 642e 2028 2338 3837  eprecated. (#887
-000094a0: 290a 2a20 6060 5472 6169 744d 6170 6060  ).* ``TraitMap``
-000094b0: 2069 7320 6465 7072 6563 6174 6564 2c20   is deprecated, 
-000094c0: 7573 6520 6060 4d61 7060 6020 696e 7374  use ``Map`` inst
-000094d0: 6561 642e 2028 2339 3734 290a 2a20 6060  ead. (#974).* ``
-000094e0: 5472 6169 7450 7265 6669 784d 6170 6060  TraitPrefixMap``
-000094f0: 2069 7320 6465 7072 6563 6174 6564 2c20   is deprecated, 
-00009500: 7573 6520 6060 5072 6566 6978 4d61 7060  use ``PrefixMap`
-00009510: 6020 696e 7374 6561 642e 2028 2339 3734  ` instead. (#974
-00009520: 290a 2a20 6060 5472 6169 7450 7265 6669  ).* ``TraitPrefi
-00009530: 784c 6973 7460 6020 6973 2064 6570 7265  xList`` is depre
-00009540: 6361 7465 642c 2075 7365 2060 6050 7265  cated, use ``Pre
-00009550: 6669 784c 6973 7460 602e 2028 2339 3734  fixList``. (#974
-00009560: 290a 2a20 6060 436f 6c6f 7260 602c 2060  ).* ``Color``, `
-00009570: 6052 4247 436f 6c6f 7260 6020 616e 6420  `RBGColor`` and 
-00009580: 6060 466f 6e74 6060 2061 7265 206e 6f77  ``Font`` are now
-00009590: 2064 6570 7265 6361 7465 642e 2055 7365   deprecated. Use
-000095a0: 2074 6865 206f 6e65 7320 6672 6f6d 0a20   the ones from. 
-000095b0: 2054 7261 6974 7355 4920 696e 7374 6561   TraitsUI instea
-000095c0: 642e 2028 2331 3032 3229 0a0a 5265 6d6f  d. (#1022)..Remo
-000095d0: 7661 6c73 0a7e 7e7e 7e7e 7e7e 7e0a 0a2a  vals.~~~~~~~~..*
-000095e0: 2060 6074 7261 6974 735f 7375 7065 7260   ``traits_super`
-000095f0: 6020 6973 2072 656d 6f76 6564 2e20 2823  ` is removed. (#
-00009600: 3130 3135 290a 0a44 6f63 756d 656e 7461  1015)..Documenta
-00009610: 7469 6f6e 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  tion.~~~~~~~~~~~
-00009620: 7e7e 0a0a 2a20 4164 6420 6465 7461 696c  ~~..* Add detail
-00009630: 7320 6f6e 2063 7265 6174 696e 6720 6375  s on creating cu
-00009640: 7374 6f6d 2074 7261 6974 2070 726f 7065  stom trait prope
-00009650: 7274 6965 732e 2028 2333 3837 290a 2a20  rties. (#387).* 
-00009660: 4372 6f73 7320 7265 6665 7265 6e63 6520  Cross reference 
-00009670: 7370 6563 6961 6c20 6861 6e64 6c65 7220  special handler 
-00009680: 7369 676e 6174 7572 6573 2066 6f72 206c  signatures for l
-00009690: 6973 7465 6e69 6e67 2074 6f20 6e65 7374  istening to nest
-000096a0: 6564 2061 7474 7269 6275 7465 730a 2020  ed attributes.  
-000096b0: 696e 206c 6973 7420 616e 6420 6469 6374  in list and dict
-000096c0: 2e20 2823 3839 3429 0a2a 2052 6570 6c61  . (#894).* Repla
-000096d0: 6365 2027 5472 6169 7473 2035 2720 7769  ce 'Traits 5' wi
-000096e0: 7468 2027 5472 6169 7473 2036 2720 696e  th 'Traits 6' in
-000096f0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00009700: 6f6e 2e20 2823 3930 3329 0a2a 2055 7365  on. (#903).* Use
-00009710: 206d 616a 6f72 2e6d 696e 6f72 2076 6572   major.minor ver
-00009720: 7369 6f6e 2069 6e20 646f 6375 6d65 6e74  sion in document
-00009730: 6174 696f 6e2e 2028 2331 3132 3429 0a2a  ation. (#1124).*
-00009740: 2041 6464 2069 6e69 7469 616c 2064 6f63   Add initial doc
-00009750: 756d 656e 7461 7469 6f6e 206f 6e20 5472  umentation on Tr
-00009760: 6169 7473 2069 6e74 6572 6e61 6c73 2e20  aits internals. 
-00009770: 2823 3935 3829 0a2a 2046 6978 2065 7861  (#958).* Fix exa
-00009780: 6d70 6c65 2063 6c61 7373 2060 604f 6464  mple class ``Odd
-00009790: 496e 7460 602e 2028 2339 3733 290a 2a20  Int``. (#973).* 
-000097a0: 4164 6420 446f 7320 616e 6420 446f 6e74  Add Dos and Dont
-000097b0: 7320 666f 7220 7772 6974 696e 6720 6368  s for writing ch
-000097c0: 616e 6765 2068 616e 646c 6572 732e 2028  ange handlers. (
-000097d0: 2331 3031 3729 0a2a 2043 6c61 7269 6679  #1017).* Clarify
-000097e0: 2077 6865 6e20 6465 6661 756c 7420 696e   when default in
-000097f0: 6974 6961 6c69 7a65 7220 6973 2063 616c  itializer is cal
-00009800: 6c65 6420 616e 6420 7768 656e 2068 616e  led and when han
-00009810: 646c 6572 7320 6172 6520 7265 6769 7374  dlers are regist
-00009820: 6572 6564 2e0a 2020 2823 3130 3139 290a  ered..  (#1019).
-00009830: 2a20 4669 7820 646f 6375 6d65 6e74 6174  * Fix documentat
-00009840: 696f 6e20 7265 6e64 6572 696e 6720 6973  ion rendering is
-00009850: 7375 6573 2061 6e64 2066 726f 6e74 206d  sues and front m
-00009860: 6174 7465 722e 2028 2331 3033 392c 2023  atter. (#1039, #
-00009870: 3130 3533 290a 2a20 436c 6172 6966 7920  1053).* Clarify 
-00009880: 7768 656e 2064 796e 616d 6963 2064 6566  when dynamic def
-00009890: 6175 6c74 2076 616c 7565 7320 6172 6520  ault values are 
-000098a0: 636f 6e73 6964 6572 6564 2074 6f20 6861  considered to ha
-000098b0: 7665 2065 7869 7374 6564 2e20 2823 3130  ve existed. (#10
-000098c0: 3638 290a 2a20 4578 7061 6e64 2075 7365  68).* Expand use
-000098d0: 7220 6d61 6e75 616c 206f 6e20 636f 6e74  r manual on cont
-000098e0: 6169 6e65 7220 7472 6169 7473 2061 6e64  ainer traits and
-000098f0: 206f 626a 6563 7473 2e20 2823 3130 3538   objects. (#1058
-00009900: 290a 2a20 4164 6420 696e 7465 7273 7068  ).* Add intersph
-00009910: 696e 7820 7375 7070 6f72 7420 746f 2063  inx support to c
-00009920: 6f6e 6669 6775 7261 7469 6f6e 2e20 2823  onfiguration. (#
-00009930: 3131 3336 290a 2a20 4164 6420 7573 6572  1136).* Add user
-00009940: 206d 616e 7561 6c20 7365 6374 696f 6e20   manual section 
-00009950: 6f6e 2074 6865 206e 6577 2060 606f 6273  on the new ``obs
-00009960: 6572 7665 6060 206e 6f74 6966 6963 6174  erve`` notificat
-00009970: 696f 6e20 7379 7374 656d 2e20 2823 3130  ion system. (#10
-00009980: 3630 2c0a 2020 2331 3134 302c 2023 3131  60,.  #1140, #11
-00009990: 3433 290a 2a20 4164 6420 7573 6572 206d  43).* Add user m
-000099a0: 616e 7561 6c20 7365 6374 696f 6e20 6f6e  anual section on
-000099b0: 2074 6865 2060 6055 6e69 6f6e 6060 2074   the ``Union`` t
-000099c0: 7261 6974 2074 7970 6520 616e 6420 686f  rait type and ho
-000099d0: 7720 746f 206d 6967 7261 7465 2066 726f  w to migrate fro
-000099e0: 6d0a 2020 6060 4569 7468 6572 6060 2028  m.  ``Either`` (
-000099f0: 2337 3739 2c20 2331 3135 332c 2023 3131  #779, #1153, #11
-00009a00: 3632 290a 2a20 4f74 6865 7220 6d69 6e6f  62).* Other mino
-00009a10: 7220 636c 6561 6e75 7073 2061 6e64 2066  r cleanups and f
-00009a20: 6978 6573 2e20 2823 3934 392c 2023 3131  ixes. (#949, #11
-00009a30: 3431 2c20 2331 3137 3829 0a0a 5465 7374  41, #1178)..Test
-00009a40: 2073 7569 7465 0a7e 7e7e 7e7e 7e7e 7e7e   suite.~~~~~~~~~
-00009a50: 7e0a 0a2a 2041 6c6c 6f77 2074 6573 7473  ~..* Allow tests
-00009a60: 2074 6f20 6265 2073 6b69 7070 6564 2069   to be skipped i
-00009a70: 6620 5472 6169 7473 5549 2069 7320 6e6f  f TraitsUI is no
-00009a80: 7420 696e 7374 616c 6c65 642e 2028 2331  t installed. (#1
-00009a90: 3033 3829 0a2a 2041 6464 2060 6065 7874  038).* Add ``ext
-00009aa0: 7261 735f 7265 7175 6972 6560 6020 656e  ras_require`` en
-00009ab0: 7472 7920 666f 7220 7465 7374 696e 672e  try for testing.
-00009ac0: 2028 2338 3739 290a 2a20 4164 6420 7465   (#879).* Add te
-00009ad0: 7374 7320 666f 7220 7061 7273 696e 6720  sts for parsing 
-00009ae0: 6060 6f6e 5f74 7261 6974 5f63 6861 6e67  ``on_trait_chang
-00009af0: 6560 6020 6d69 6e69 2d6c 616e 6775 6167  e`` mini-languag
-00009b00: 652e 2028 2339 3231 290a 2a20 4669 7820  e. (#921).* Fix 
-00009b10: 6120 6d69 7373 696e 6720 696d 706f 7274  a missing import
-00009b20: 2074 6f20 616c 6c6f 7720 6120 7465 7374   to allow a test
-00009b30: 206d 6f64 756c 6520 746f 2062 6520 7275   module to be ru
-00009b40: 6e20 7374 616e 6461 6c6f 6e65 2e20 2823  n standalone. (#
-00009b50: 3936 3129 0a2a 2041 6464 2061 2047 5549  961).* Add a GUI
-00009b60: 2074 6573 7420 666f 7220 6060 456e 756d   test for ``Enum
-00009b70: 2e63 7265 6174 655f 6564 6974 6f72 6060  .create_editor``
-00009b80: 2e20 2823 3938 3829 0a2a 2046 6978 2073  . (#988).* Fix s
-00009b90: 6f6d 6520 6d6f 6475 6c65 2d6c 6576 656c  ome module-level
-00009ba0: 2060 6044 6570 7265 6361 7469 6f6e 5761   ``DeprecationWa
-00009bb0: 726e 696e 6760 6020 6d65 7373 6167 6573  rning`` messages
-00009bc0: 2e20 2823 3131 3537 290a 0a42 7569 6c64  . (#1157)..Build
-00009bd0: 2061 6e64 2063 6f6e 7469 6e75 6f75 7320   and continuous 
-00009be0: 696e 7465 6772 6174 696f 6e0a 7e7e 7e7e  integration.~~~~
-00009bf0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00009c00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a2a 2043  ~~~~~~~~~~~~.* C
-00009c10: 4920 6e6f 206c 6f6e 6765 7220 7275 6e73  I no longer runs
-00009c20: 206f 6e20 5079 7468 6f6e 2033 2e35 2028   on Python 3.5 (
-00009c30: 2331 3034 3429 0a2a 2041 6464 2063 6f6e  #1044).* Add con
-00009c40: 6669 676f 626a 2064 6570 656e 6465 6e63  figobj dependenc
-00009c50: 7920 616e 6420 7265 6d6f 7665 2072 656d  y and remove rem
-00009c60: 6169 6e69 6e67 2033 2e35 2072 6566 6572  aining 3.5 refer
-00009c70: 656e 6365 7320 696e 0a20 2060 6065 7473  ences in.  ``ets
-00009c80: 746f 6f6c 2e70 7960 602e 2028 2331 3035  tool.py``. (#105
-00009c90: 3129 0a2a 2043 6f64 6563 6f76 2072 6570  1).* Codecov rep
-00009ca0: 6f72 7473 2061 7265 206e 6f20 6c6f 6e67  orts are no long
-00009cb0: 6572 2072 6574 7269 6576 6564 2066 6f72  er retrieved for
-00009cc0: 2070 756c 6c20 7265 7175 6573 7473 2e20   pull requests. 
-00009cd0: 2823 3131 3039 290a 2a20 4349 2074 6573  (#1109).* CI tes
-00009ce0: 7473 2072 6571 7569 7269 6e67 2061 2047  ts requiring a G
-00009cf0: 5549 2061 7265 206e 6f77 2072 756e 2061  UI are now run a
-00009d00: 6761 696e 7374 2050 7951 7435 2072 6174  gainst PyQt5 rat
-00009d10: 6865 7220 7468 616e 2050 7951 7434 2e0a  her than PyQt4..
-00009d20: 2020 2823 3131 3237 290a 2a20 4164 6420    (#1127).* Add 
-00009d30: 536c 6163 6b20 6e6f 7469 6669 6361 7469  Slack notificati
-00009d40: 6f6e 7320 666f 7220 4349 2e20 2823 3130  ons for CI. (#10
-00009d50: 3734 290a 2a20 4669 7820 616e 6420 696d  74).* Fix and im
-00009d60: 7072 6f76 6520 7661 7269 6f75 7320 6060  prove various ``
-00009d70: 7365 7475 702e 7079 6060 2070 6163 6b61  setup.py`` packa
-00009d80: 6765 206d 6574 6164 6174 6120 6669 656c  ge metadata fiel
-00009d90: 6473 2e20 2823 3131 3835 290a 0a4d 6169  ds. (#1185)..Mai
-00009da0: 6e74 656e 616e 6365 2061 6e64 2063 6f64  ntenance and cod
-00009db0: 6520 6f72 6761 6e69 7a61 7469 6f6e 0a7e  e organization.~
-00009dc0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00009dd0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00009de0: 0a0a 2a20 5265 6661 6374 6f72 2043 4861  ..* Refactor CHa
-00009df0: 7354 7261 6974 7320 6060 7472 6169 7473  sTraits ``traits
-00009e00: 5f69 6e69 7465 6460 6020 6d65 7468 6f64  _inited`` method
-00009e10: 2e20 2823 3834 3229 0a2a 2041 6464 2073  . (#842).* Add s
-00009e20: 7570 706f 7274 2066 6f72 2070 7265 7265  upport for prere
-00009e30: 6c65 6173 6520 7365 6374 696f 6e20 696e  lease section in
-00009e40: 2076 6572 7369 6f6e 2e20 2823 3836 3429   version. (#864)
-00009e50: 0a2a 2052 656e 616d 6520 636f 6d70 6172  .* Rename compar
-00009e60: 6973 6f6e 206d 6f64 6520 696e 7465 6765  ison mode intege
-00009e70: 7220 636f 6e73 7461 6e74 7320 696e 2060  r constants in `
-00009e80: 6063 7472 6169 7473 2e63 6060 2e20 2823  `ctraits.c``. (#
-00009e90: 3836 3229 0a2a 2046 6f6c 6c6f 7720 6265  862).* Follow be
-00009ea0: 7374 2070 7261 6374 6963 6573 2077 6865  st practices whe
-00009eb0: 6e20 6f70 656e 696e 6720 6669 6c65 732e  n opening files.
-00009ec0: 2028 2338 3732 290a 2a20 496e 6974 6961   (#872).* Initia
-00009ed0: 6c69 7a65 2060 6063 5472 6169 7460 6020  lize ``cTrait`` 
-00009ee0: 6060 6765 7461 7474 7260 602c 2060 6073  ``getattr``, ``s
-00009ef0: 6574 6174 7472 6060 2068 616e 646c 6572  etattr`` handler
-00009f00: 7320 696e 2060 6074 705f 6e65 7760 602e  s in ``tp_new``.
-00009f10: 2028 2338 3735 290a 2a20 4368 6563 6b20   (#875).* Check 
-00009f20: 6060 7472 6169 745f 6368 616e 6765 5f6e  ``trait_change_n
-00009f30: 6f74 6966 7960 6020 6561 726c 7920 696e  otify`` early in
-00009f40: 2060 6063 616c 6c5f 6e6f 7469 6669 6572   ``call_notifier
-00009f50: 7360 602e 2028 2339 3137 290a 2a20 5265  s``. (#917).* Re
-00009f60: 6661 6374 6f72 2060 6063 7472 6169 7473  factor ``ctraits
-00009f70: 2e63 6060 2066 6f72 2063 616c 6c69 6e67  .c`` for calling
-00009f80: 2074 7261 6974 2061 6e64 206f 626a 6563   trait and objec
-00009f90: 7420 6e6f 7469 6669 6572 732e 2028 2339  t notifiers. (#9
-00009fa0: 3138 290a 2a20 6060 4261 7365 456e 756d  18).* ``BaseEnum
-00009fb0: 6060 2061 6e64 2060 6045 6e75 6d60 6020  `` and ``Enum`` 
-00009fc0: 6669 7865 7320 616e 6420 636c 6561 6e75  fixes and cleanu
-00009fd0: 702e 2028 2339 3638 290a 2a20 5370 6c69  p. (#968).* Spli
-00009fe0: 7420 6060 6374 7261 6974 7360 6020 7072  t ``ctraits`` pr
-00009ff0: 6f70 6572 7479 2061 7069 2074 6f20 6060  operty api to ``
-0000a000: 5f73 6574 5f70 726f 7065 7274 7960 6020  _set_property`` 
-0000a010: 616e 6420 6060 5f67 6574 5f70 726f 7065  and ``_get_prope
-0000a020: 7274 7960 602e 0a20 2028 2339 3637 290a  rty``..  (#967).
-0000a030: 2a20 4669 7820 6f76 6572 636f 6d70 6c69  * Fix overcompli
-0000a040: 6361 7465 6420 6060 5f5f 6465 6570 636f  cated ``__deepco
-0000a050: 7079 5f5f 6060 2069 6d70 6c65 6d65 6e74  py__`` implement
-0000a060: 6174 696f 6e2e 2028 2339 3932 290a 2a20  ation. (#992).* 
-0000a070: 4164 6420 6060 5f5f 7265 7072 5f5f 6060  Add ``__repr__``
-0000a080: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-0000a090: 666f 7220 6060 5472 6169 744c 6973 7445  for ``TraitListE
-0000a0a0: 7665 6e74 6060 2c20 6060 5472 6169 7444  vent``, ``TraitD
-0000a0b0: 6963 7445 7665 6e74 6060 0a20 2061 6e64  ictEvent``.  and
-0000a0c0: 2060 6054 7261 6974 5365 7445 7665 6e74   ``TraitSetEvent
-0000a0d0: 6060 2e20 2823 3130 3036 2c20 2331 3134  ``. (#1006, #114
-0000a0e0: 382c 2023 3131 3439 290a 2a20 5265 6d6f  8, #1149).* Remo
-0000a0f0: 7665 2063 6163 6869 6e67 206f 6620 6564  ve caching of ed
-0000a100: 6974 6f72 2066 6163 746f 7269 6573 2e20  itor factories. 
-0000a110: 2823 3130 3332 290a 2a20 5265 6d6f 7665  (#1032).* Remove
-0000a120: 2063 6f6e 6469 7469 6f6e 616c 2074 7261   conditional tra
-0000a130: 6974 7375 6920 696d 706f 7274 732e 2028  itsui imports. (
-0000a140: 2331 3033 3329 0a2a 2052 656d 6f76 6520  #1033).* Remove 
-0000a150: 636f 6465 2064 7570 6c69 6361 7469 6f6e  code duplication
-0000a160: 2069 6e20 6060 7475 746f 722e 7079 6060   in ``tutor.py``
-0000a170: 2e20 2823 3130 3334 290a 2a20 4669 7820  . (#1034).* Fix 
-0000a180: 636f 7272 6563 746e 6573 7320 696e 2060  correctness in `
-0000a190: 6045 6e75 6d60 6020 6465 6661 756c 7420  `Enum`` default 
-0000a1a0: 7472 6169 7473 7569 2065 6469 746f 722e  traitsui editor.
-0000a1b0: 2028 2331 3031 3229 0a2a 2055 7365 2060   (#1012).* Use `
-0000a1c0: 604e 554c 4c60 6020 666f 7220 7a65 726f  `NULL`` for zero
-0000a1d0: 2d61 7267 756d 656e 7420 6060 5079 4f62  -argument ``PyOb
-0000a1e0: 6a65 6374 5f43 616c 6c4d 6574 686f 6460  ject_CallMethod`
-0000a1f0: 6020 666f 726d 6174 2e20 2823 3131 3030  ` format. (#1100
-0000a200: 290a 2a20 4d69 7363 656c 6c61 6e65 6f75  ).* Miscellaneou
-0000a210: 7320 6f74 6865 7220 6d69 6e6f 7220 6669  s other minor fi
-0000a220: 7865 732c 2072 6566 6163 746f 7269 6e67  xes, refactoring
-0000a230: 7320 616e 6420 636c 6561 6e75 7073 2e20  s and cleanups. 
-0000a240: 2823 3837 342c 2023 3838 322c 0a20 2023  (#874, #882,.  #
-0000a250: 3931 352c 2023 3932 302c 2023 3932 332c  915, #920, #923,
-0000a260: 2023 3932 342c 2023 3933 352c 2023 3933   #924, #935, #93
-0000a270: 392c 2023 3934 342c 2023 3935 302c 2023  9, #944, #950, #
-0000a280: 3936 3429 0a0a 0a52 656c 6561 7365 2036  964)...Release 6
-0000a290: 2e30 2e30 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .0.0.-----------
-0000a2a0: 2d2d 0a0a 5265 6c65 6173 6564 3a20 3230  --..Released: 20
-0000a2b0: 3230 2d30 322d 3134 0a0a 4e6f 2063 6861  20-02-14..No cha
-0000a2c0: 6e67 6573 2073 696e 6365 2074 6865 2036  nges since the 6
-0000a2d0: 2e30 2e30 7263 3020 7265 6c65 6173 6520  .0.0rc0 release 
-0000a2e0: 6361 6e64 6964 6174 652e 0a0a 0a52 656c  candidate....Rel
-0000a2f0: 6561 7365 2036 2e30 2e30 7263 300a 2d2d  ease 6.0.0rc0.--
-0000a300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-0000a310: 5265 6c65 6173 6564 3a20 3230 3230 2d30  Released: 2020-0
-0000a320: 312d 3330 0a0a 5265 6c65 6173 6520 6e6f  1-30..Release no
-0000a330: 7465 730a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  tes.~~~~~~~~~~~~
-0000a340: 7e0a 0a54 7261 6974 7320 362e 3020 6973  ~..Traits 6.0 is
-0000a350: 2061 206d 616a 6f72 2075 7064 6174 6520   a major update 
-0000a360: 746f 2074 6865 2054 7261 6974 7320 7061  to the Traits pa
-0000a370: 636b 6167 652c 2077 6974 6820 6120 6e75  ckage, with a nu
-0000a380: 6d62 6572 206f 660a 6261 636b 7761 7264  mber of.backward
-0000a390: 2069 6e63 6f6d 7061 7469 626c 6520 6368   incompatible ch
-0000a3a0: 616e 6765 7320 6672 6f6d 2069 7473 2070  anges from its p
-0000a3b0: 7265 6465 6365 7373 6f72 2e20 4e6f 7461  redecessor. Nota
-0000a3c0: 626c 6520 6368 616e 6765 733a 0a0a 2a20  ble changes:..* 
-0000a3d0: 5079 7468 6f6e 2032 2e37 2069 7320 6e6f  Python 2.7 is no
-0000a3e0: 206c 6f6e 6765 7220 7375 7070 6f72 7465   longer supporte
-0000a3f0: 643b 2054 7261 6974 7320 362e 3020 7265  d; Traits 6.0 re
-0000a400: 7175 6972 6573 2050 7974 686f 6e20 332e  quires Python 3.
-0000a410: 3520 6f72 206c 6174 6572 2e0a 2a20 5472  5 or later..* Tr
-0000a420: 6169 7420 7479 7065 7320 7265 6c61 7465  ait types relate
-0000a430: 6420 746f 2050 7974 686f 6e20 3220 2866  d to Python 2 (f
-0000a440: 6f72 2065 7861 6d70 6c65 2060 6055 6e69  or example ``Uni
-0000a450: 636f 6465 6060 2061 6e64 2060 604c 6f6e  code`` and ``Lon
-0000a460: 6760 6029 2068 6176 650a 2020 6265 656e  g``) have.  been
-0000a470: 2064 6570 7265 6361 7465 6420 696e 2066   deprecated in f
-0000a480: 6176 6f75 7220 6f66 2074 6865 6972 2050  avour of their P
-0000a490: 7974 686f 6e20 3320 6571 7569 7661 6c65  ython 3 equivale
-0000a4a0: 6e74 7320 2866 6f72 2065 7861 6d70 6c65  nts (for example
-0000a4b0: 2060 6053 7472 6060 0a20 2061 6e64 2060   ``Str``.  and `
-0000a4c0: 6049 6e74 6060 292e 0a2a 204d 616e 7920  `Int``)..* Many 
-0000a4d0: 6c69 7474 6c65 2d75 7365 6420 6869 7374  little-used hist
-0000a4e0: 6f72 6963 616c 2066 6561 7475 7265 7320  orical features 
-0000a4f0: 6f66 2054 7261 6974 7320 6861 7665 2062  of Traits have b
-0000a500: 6565 6e20 6465 7072 6563 6174 6564 2c20  een deprecated, 
-0000a510: 616e 640a 2020 6172 6520 7363 6865 6475  and.  are schedu
-0000a520: 6c65 6420 666f 7220 7265 6d6f 7661 6c20  led for removal 
-0000a530: 696e 2054 7261 6974 7320 372e 302e 0a2a  in Traits 7.0..*
-0000a540: 2053 6f6d 6520 6869 7374 6f72 6963 616c   Some historical
-0000a550: 2066 6561 7475 7265 7320 6f66 2054 7261   features of Tra
-0000a560: 6974 7320 7468 6174 2068 6164 206e 6f20  its that had no 
-0000a570: 6576 6964 656e 6365 206f 6620 6578 7465  evidence of exte
-0000a580: 726e 616c 2075 7361 6765 0a20 2077 6572  rnal usage.  wer
-0000a590: 6520 7265 6d6f 7665 6420 696e 2054 7261  e removed in Tra
-0000a5a0: 6974 7320 362e 302e 0a2a 2049 6e74 726f  its 6.0..* Intro
-0000a5b0: 7370 6563 7469 6f6e 206f 6620 6060 4354  spection of ``CT
-0000a5c0: 7261 6974 6060 2061 6e64 2060 6048 6173  rait`` and ``Has
-0000a5d0: 5472 6169 7473 6060 206f 626a 6563 7473  Traits`` objects
-0000a5e0: 2069 7320 6772 6561 746c 7920 696d 7072   is greatly impr
-0000a5f0: 6f76 6564 2e0a 2020 416c 6c20 6f66 2074  oved..  All of t
-0000a600: 6865 2069 6e74 6572 6e61 6c20 7374 6174  he internal stat
-0000a610: 6520 7468 6174 2077 6173 2070 7265 7669  e that was previ
-0000a620: 6f75 736c 7920 6869 6464 656e 2077 6974  ously hidden wit
-0000a630: 6869 6e20 7468 6520 4320 6578 7465 6e73  hin the C extens
-0000a640: 696f 6e0a 2020 6973 206e 6f77 2061 6363  ion.  is now acc
-0000a650: 6573 7369 626c 6520 6672 6f6d 2050 7974  essible from Pyt
-0000a660: 686f 6e2e 0a2a 2054 6865 2054 7261 6974  hon..* The Trait
-0000a670: 7320 636f 6465 6261 7365 2068 6173 2075  s codebase has u
-0000a680: 6e64 6572 676f 6e65 2073 6f6d 6520 7369  ndergone some si
-0000a690: 676e 6966 6963 616e 7420 7265 6f72 6761  gnificant reorga
-0000a6a0: 6e69 7a61 7469 6f6e 732c 0a20 2072 6566  nizations,.  ref
-0000a6b0: 6f72 6d61 7474 696e 6773 2061 6e64 2073  ormattings and s
-0000a6c0: 7479 6c65 2063 6c65 616e 7570 7320 746f  tyle cleanups to
-0000a6d0: 206d 616b 6520 6974 2065 6173 6965 7220   make it easier 
-0000a6e0: 746f 2077 6f72 6b20 7769 7468 2c20 616e  to work with, an
-0000a6f0: 640a 2020 746f 2069 6d70 726f 7665 2074  d.  to improve t
-0000a700: 6865 2073 6570 6172 6174 696f 6e20 6265  he separation be
-0000a710: 7477 6565 6e20 5472 6169 7473 2061 6e64  tween Traits and
-0000a720: 2054 7261 6974 7355 492e 0a2a 2054 6869   TraitsUI..* Thi
-0000a730: 7320 7265 6c65 6173 6520 7761 7320 666f  s release was fo
-0000a740: 6375 7365 6420 6d61 696e 6c79 206f 6e20  cused mainly on 
-0000a750: 636c 6561 6e75 7020 616e 6420 6275 6766  cleanup and bugf
-0000a760: 6978 696e 672e 204e 6576 6572 7468 656c  ixing. Neverthel
-0000a770: 6573 732c 0a20 2069 7420 636f 6e74 6169  ess,.  it contai
-0000a780: 6e73 2061 2073 7072 696e 6b6c 696e 6720  ns a sprinkling 
-0000a790: 6f66 206e 6577 2066 6561 7475 7265 732e  of new features.
-0000a7a0: 2054 6865 7265 2773 2061 206e 6577 2060   There's a new `
-0000a7b0: 6044 6174 6574 696d 6560 600a 2020 7472  `Datetime``.  tr
-0000a7c0: 6169 7420 7479 7065 2e20 5468 6520 6060  ait type. The ``
-0000a7d0: 456e 756d 6060 2074 7261 6974 2074 7970  Enum`` trait typ
-0000a7e0: 6520 6e6f 7720 7375 7070 6f72 7473 2050  e now supports P
-0000a7f0: 7974 686f 6e20 656e 756d 6572 6174 696f  ython enumeratio
-0000a800: 6e73 2e0a 2020 5468 6520 6060 4669 6c65  ns..  The ``File
-0000a810: 6060 2074 7261 6974 2074 7970 6520 7375  `` trait type su
-0000a820: 7070 6f72 7473 2070 6174 682d 6c69 6b65  pports path-like
-0000a830: 206f 626a 6563 7473 2e0a 0a4d 6f72 6520   objects...More 
-0000a840: 7468 616e 2031 3530 2050 5273 2077 656e  than 150 PRs wen
-0000a850: 7420 696e 746f 2074 6869 7320 7265 6c65  t into this rele
-0000a860: 6173 652e 2054 6865 2066 6f6c 6c6f 7769  ase. The followi
-0000a870: 6e67 2070 656f 706c 6520 636f 6e74 7269  ng people contri
-0000a880: 6275 7465 640a 636f 6465 2063 6861 6e67  buted.code chang
-0000a890: 6573 2066 6f72 2074 6869 7320 7265 6c65  es for this rele
-0000a8a0: 6173 653a 0a0a 2a20 4b69 7420 5961 6e20  ase:..* Kit Yan 
-0000a8b0: 4368 6f69 0a2a 204d 6172 6b20 4469 636b  Choi.* Mark Dick
-0000a8c0: 696e 736f 6e0a 2a20 4b65 7669 6e20 4475  inson.* Kevin Du
-0000a8d0: 6666 0a2a 2052 6f62 6572 7420 4b65 726e  ff.* Robert Kern
-0000a8e0: 0a2a 204d 6964 6875 6e20 4d61 6468 7573  .* Midhun Madhus
-0000a8f0: 6f6f 6461 6e61 6e0a 2a20 5368 6f65 6220  oodanan.* Shoeb 
-0000a900: 4d6f 6861 6d6d 6564 0a2a 2053 6169 2052  Mohammed.* Sai R
-0000a910: 6168 756c 2050 6f72 7572 690a 2a20 436f  ahul Poruri.* Co
-0000a920: 7272 616e 2057 6562 7374 6572 0a2a 204a  rran Webster.* J
-0000a930: 6f68 6e20 5769 6767 696e 730a 0a50 6f72  ohn Wiggins..Por
-0000a940: 7469 6e67 2067 7569 6465 0a7e 7e7e 7e7e  ting guide.~~~~~
-0000a950: 7e7e 7e7e 7e7e 7e7e 0a0a 466f 7220 7468  ~~~~~~~~..For th
-0000a960: 6520 6d6f 7374 2070 6172 742c 2065 7869  e most part, exi
-0000a970: 7374 696e 6720 636f 6465 2074 6861 7420  sting code that 
-0000a980: 776f 726b 7320 7769 7468 2054 7261 6974  works with Trait
-0000a990: 7320 352e 322e 3020 7368 6f75 6c64 0a63  s 5.2.0 should.c
-0000a9a0: 6f6e 7469 6e75 6520 746f 2077 6f72 6b20  ontinue to work 
-0000a9b0: 7769 7468 2054 7261 6974 7320 362e 302e  with Traits 6.0.
-0000a9c0: 3020 7769 7468 6f75 7420 6368 616e 6765  0 without change
-0000a9d0: 732e 2048 6f77 6576 6572 2c20 7468 6572  s. However, ther
-0000a9e0: 650a 6172 6520 736f 6d65 2070 6f74 656e  e.are some poten
-0000a9f0: 7469 616c 6c79 2062 7265 616b 696e 6720  tially breaking 
-0000aa00: 6368 616e 6765 7320 696e 2054 7261 6974  changes in Trait
-0000aa10: 7320 362e 302e 302c 2061 6e64 2077 6520  s 6.0.0, and we 
-0000aa20: 7265 636f 6d6d 656e 640a 6170 706c 7969  recommend.applyi
-0000aa30: 6e67 2063 6175 7469 6f6e 2077 6865 6e20  ng caution when 
-0000aa40: 7570 6772 6164 696e 672e 0a0a 4865 7265  upgrading...Here
-0000aa50: 2773 2061 2067 7569 6465 2074 6f20 6465  's a guide to de
-0000aa60: 616c 696e 6720 7769 7468 2073 6f6d 6520  aling with some 
-0000aa70: 6f66 2074 6865 2070 6f74 656e 7469 616c  of the potential
-0000aa80: 6c79 2062 7265 616b 696e 6720 6368 616e  ly breaking chan
-0000aa90: 6765 732e 0a0a 2a20 5468 6520 6060 556e  ges...* The ``Un
-0000aaa0: 6963 6f64 6560 6020 616e 6420 6060 4355  icode`` and ``CU
-0000aab0: 6e69 636f 6465 6060 2074 7261 6974 2074  nicode`` trait t
-0000aac0: 7970 6573 2061 7265 206e 6f77 2073 696d  ypes are now sim
-0000aad0: 706c 7920 7379 6e6f 6e79 6d73 2066 6f72  ply synonyms for
-0000aae0: 0a20 2060 6053 7472 6060 2061 6e64 2060  .  ``Str`` and `
-0000aaf0: 6043 5374 7260 602e 2060 6055 6e69 636f  `CStr``. ``Unico
-0000ab00: 6465 6060 2061 6e64 2060 6043 556e 6963  de`` and ``CUnic
-0000ab10: 6f64 6560 6020 6172 6520 636f 6e73 6964  ode`` are consid
-0000ab20: 6572 6564 2064 6570 7265 6361 7465 642e  ered deprecated.
-0000ab30: 0a20 2046 6f72 206e 6f77 2c20 6e6f 2064  .  For now, no d
-0000ab40: 6570 7265 6361 7469 6f6e 2077 6172 6e69  eprecation warni
-0000ab50: 6e67 2069 7320 6973 7375 6564 206f 6e20  ng is issued on 
-0000ab60: 7573 6520 6f66 2074 6865 7365 2064 6570  use of these dep
-0000ab70: 7265 6361 7465 6420 7472 6169 740a 2020  recated trait.  
-0000ab80: 7479 7065 732c 2062 7574 2069 6e20 5472  types, but in Tr
-0000ab90: 6169 7473 2036 2e31 2e30 2061 6e64 206c  aits 6.1.0 and l
-0000aba0: 6174 6572 2c20 7761 726e 696e 6773 206d  ater, warnings m
-0000abb0: 6179 2062 6520 6973 7375 6564 2c20 616e  ay be issued, an
-0000abc0: 6420 696e 2054 7261 6974 730a 2020 372e  d in Traits.  7.
-0000abd0: 302e 3020 7468 6573 6520 7472 6169 7420  0.0 these trait 
-0000abe0: 7479 7065 7320 6d61 7920 6265 2072 656d  types may be rem
-0000abf0: 6f76 6564 2e20 4974 2773 2072 6563 6f6d  oved. It's recom
-0000ac00: 6d65 6e64 6564 2074 6861 7420 7573 6572  mended that user
-0000ac10: 7320 7570 6461 7465 0a20 2061 6c6c 2075  s update.  all u
-0000ac20: 7365 7320 6f66 2060 6055 6e69 636f 6465  ses of ``Unicode
-0000ac30: 6060 2074 6f20 6060 5374 7260 6020 616e  `` to ``Str`` an
-0000ac40: 6420 6060 4355 6e69 636f 6465 6060 2074  d ``CUnicode`` t
-0000ac50: 6f20 6060 4353 7472 6060 2074 6f20 6176  o ``CStr`` to av
-0000ac60: 6f69 640a 2020 7761 726e 696e 6773 206f  oid.  warnings o
-0000ac70: 7220 6572 726f 7273 2069 6e20 7468 6520  r errors in the 
-0000ac80: 6675 7475 7265 2e0a 0a2a 2053 696d 696c  future...* Simil
-0000ac90: 6172 6c79 2c20 6060 4c6f 6e67 6060 2061  arly, ``Long`` a
-0000aca0: 6e64 2060 6043 4c6f 6e67 6060 2061 7265  nd ``CLong`` are
-0000acb0: 206e 6f77 2073 796e 6f6e 796d 7320 666f   now synonyms fo
-0000acc0: 7220 6060 496e 7460 6020 616e 6420 6060  r ``Int`` and ``
-0000acd0: 4349 6e74 6060 2e0a 2020 5468 6520 7361  CInt``..  The sa
-0000ace0: 6d65 2072 6563 6f6d 6d65 6e64 6174 696f  me recommendatio
-0000acf0: 6e73 2061 7070 6c79 2061 7320 666f 7220  ns apply as for 
-0000ad00: 7468 6520 6060 556e 6963 6f64 6560 6020  the ``Unicode`` 
-0000ad10: 2f20 6060 5374 7260 6020 7472 6169 7420  / ``Str`` trait 
-0000ad20: 7479 7065 732e 0a0a 2a20 5573 6573 206f  types...* Uses o
-0000ad30: 6620 6060 4e4f 5f43 4f4d 5041 5245 6060  f ``NO_COMPARE``
-0000ad40: 2c20 6060 4f42 4a45 4354 5f49 4445 4e54  , ``OBJECT_IDENT
-0000ad50: 4954 595f 434f 4d50 4152 4560 6020 616e  ITY_COMPARE`` an
-0000ad60: 6420 6060 5249 4348 5f43 4f4d 5041 5245  d ``RICH_COMPARE
-0000ad70: 6060 0a20 2073 686f 756c 6420 6265 2072  ``.  should be r
-0000ad80: 6570 6c61 6365 6420 7769 7468 2074 6865  eplaced with the
-0000ad90: 2061 7070 726f 7072 6961 7465 2060 6043   appropriate ``C
-0000ada0: 6f6d 7061 7269 736f 6e4d 6f64 6560 6020  omparisonMode`` 
-0000adb0: 656e 756d 6572 6174 696f 6e0a 2020 6d65  enumeration.  me
-0000adc0: 6d62 6572 732e 0a0a 2a20 5468 6520 7661  mbers...* The va
-0000add0: 6c69 6461 7469 6f6e 2066 6f72 2061 2060  lidation for a `
-0000ade0: 6049 6e73 7461 6e63 6528 4953 6f6d 6549  `Instance(ISomeI
-0000adf0: 6e74 6572 6661 6365 2960 6020 7472 6169  nterface)`` trai
-0000ae00: 7420 7479 7065 2068 6173 2063 6861 6e67  t type has chang
-0000ae10: 6564 2c0a 2020 7768 6572 6520 6060 4953  ed,.  where ``IS
-0000ae20: 6f6d 6549 6e74 6572 6661 6365 6060 2069  omeInterface`` i
-0000ae30: 7320 6120 7375 6263 6c61 7373 206f 6620  s a subclass of 
-0000ae40: 6060 496e 7465 7266 6163 6560 602e 2050  ``Interface``. P
-0000ae50: 7265 7669 6f75 736c 792c 2061 6e0a 2020  reviously, an.  
-0000ae60: 6173 7369 676e 6d65 6e74 2074 6f20 7375  assignment to su
-0000ae70: 6368 2061 2074 7261 6974 2076 616c 6964  ch a trait valid
-0000ae80: 6174 6564 2074 6865 2074 7970 6520 6f66  ated the type of
-0000ae90: 2074 6865 2061 7373 6967 6e65 6420 7661   the assigned va
-0000aea0: 6c75 6520 6167 6169 6e73 740a 2020 7468  lue against.  th
-0000aeb0: 6520 696e 7465 7266 6163 652c 206d 6574  e interface, met
-0000aec0: 686f 6420 6279 206d 6574 686f 642e 204e  hod by method. N
-0000aed0: 6f77 2061 6e20 6060 6973 696e 7374 616e  ow an ``isinstan
-0000aee0: 6365 6060 2063 6865 636b 2069 7320 7065  ce`` check is pe
-0000aef0: 7266 6f72 6d65 640a 2020 6167 6169 6e73  rformed.  agains
-0000af00: 7420 7468 6520 696e 7465 7266 6163 6520  t the interface 
-0000af10: 696e 7374 6561 642e 204d 616b 6520 7375  instead. Make su
-0000af20: 7265 2074 6861 7420 636c 6173 7365 7320  re that classes 
-0000af30: 696d 706c 656d 656e 7469 6e67 2061 2067  implementing a g
-0000af40: 6976 656e 0a20 2069 6e74 6572 6661 6365  iven.  interface
-0000af50: 2068 6176 6520 7468 6520 6170 7072 6f70   have the approp
-0000af60: 7269 6174 6520 6060 7072 6f76 6964 6573  riate ``provides
-0000af70: 6060 2064 6563 6f72 6174 6f72 2e0a 0a20  `` decorator... 
-0000af80: 204f 6e65 206e 6f74 6162 6c65 2073 6964   One notable sid
-0000af90: 652d 6566 6665 6374 206f 6620 7468 6520  e-effect of the 
-0000afa0: 6162 6f76 6520 6368 616e 6765 2069 7320  above change is 
-0000afb0: 7468 6174 2070 6c61 696e 2060 606d 6f63  that plain ``moc
-0000afc0: 6b2e 4d6f 636b 6060 0a20 2069 6e73 7461  k.Mock``.  insta
-0000afd0: 6e63 6573 2063 616e 206e 6f20 6c6f 6e67  nces can no long
-0000afe0: 6572 2062 6520 6173 7369 676e 6564 2074  er be assigned t
-0000aff0: 6f20 6060 496e 7374 616e 6365 2849 536f  o ``Instance(ISo
-0000b000: 6d65 496e 7465 7266 6163 6529 6060 2074  meInterface)`` t
-0000b010: 7261 6974 732e 0a20 2054 6f20 6765 7420  raits..  To get 
-0000b020: 6172 6f75 6e64 2074 6869 732c 2075 7365  around this, use
-0000b030: 2060 6073 7065 633d 4953 6f6d 6549 6e74   ``spec=ISomeInt
-0000b040: 6572 6661 6365 6060 2077 6865 6e20 6372  erface`` when cr
-0000b050: 6561 7469 6e67 2079 6f75 7220 6d6f 636b  eating your mock
-0000b060: 0a20 206f 626a 6563 742e 0a0a 2020 5468  .  object...  Th
-0000b070: 6973 2063 6861 6e67 6520 646f 6573 206e  is change does n
-0000b080: 6f74 2061 6666 6563 7420 6060 496e 7374  ot affect ``Inst
-0000b090: 616e 6365 6060 2074 7261 6974 7320 666f  ance`` traits fo
-0000b0a0: 7220 6e6f 6e2d 696e 7465 7266 6163 6520  r non-interface 
-0000b0b0: 636c 6173 7365 732e 0a0a 2a20 5468 6520  classes...* The 
-0000b0c0: 666f 726d 6174 206f 6620 6060 5472 6169  format of ``Trai
-0000b0d0: 744c 6973 7445 7665 6e74 7360 6020 6861  tListEvents`` ha
-0000b0e0: 7320 6368 616e 6765 643a 2066 6f72 206c  s changed: for l
-0000b0f0: 6973 7420 6576 656e 7473 2067 656e 6572  ist events gener
-0000b100: 6174 6564 2066 726f 6d0a 2020 6120 736c  ated from.  a sl
-0000b110: 6963 6520 7365 7420 6f72 2073 6c69 6365  ice set or slice
-0000b120: 2064 656c 6574 6520 6f70 6572 6174 696f   delete operatio
-0000b130: 6e20 7768 6572 6520 7468 6174 2073 6c69  n where that sli
-0000b140: 6365 2068 6164 2061 2073 7465 7020 6f74  ce had a step ot
-0000b150: 6865 720a 2020 7468 616e 2060 6031 6060  her.  than ``1``
-0000b160: 2c20 7468 6520 6060 6164 6465 6460 6020  , the ``added`` 
-0000b170: 616e 6420 6060 7265 6d6f 7665 6460 6020  and ``removed`` 
-0000b180: 6669 656c 6473 206f 6620 7468 6520 6576  fields of the ev
-0000b190: 656e 7420 6861 6420 616e 2065 7874 7261  ent had an extra
-0000b1a0: 0a20 206c 6576 656c 206f 6620 6c69 7374  .  level of list
-0000b1b0: 2077 7261 7070 696e 6720 2866 6f72 2065   wrapping (for e
-0000b1c0: 7861 6d70 6c65 2c20 6060 6164 6465 6460  xample, ``added`
-0000b1d0: 6020 6d69 6768 7420 6265 2060 605b 5b31  ` might be ``[[1
-0000b1e0: 2c20 322c 2033 5d5d 6060 0a20 2069 6e73  , 2, 3]]``.  ins
-0000b1f0: 7465 6164 206f 6620 6060 5b31 2c20 322c  tead of ``[1, 2,
-0000b200: 2033 5d60 6029 2e20 496e 2054 7261 6974   3]``). In Trait
-0000b210: 7320 362e 302c 2074 6869 7320 6578 7472  s 6.0, this extr
-0000b220: 6120 7772 6170 7069 6e67 2068 6173 2062  a wrapping has b
-0000b230: 6565 6e0a 2020 7265 6d6f 7665 642e 2054  een.  removed. T
-0000b240: 6865 7265 206d 6179 2062 6520 6578 6973  here may be exis
-0000b250: 7469 6e67 2063 6f64 6520 7468 6174 2073  ting code that s
-0000b260: 7065 6369 616c 2d63 6173 6564 2074 6865  pecial-cased the
-0000b270: 2065 7874 7261 2077 7261 7070 696e 672e   extra wrapping.
-0000b280: 0a0a 2a20 4d61 6e79 2063 6c61 7373 6573  ..* Many classes
-0000b290: 2061 6e64 2066 756e 6374 696f 6e73 2068   and functions h
-0000b2a0: 6176 6520 6d6f 7665 6420 6172 6f75 6e64  ave moved around
-0000b2b0: 2077 6974 6869 6e20 7468 6520 5472 6169   within the Trai
-0000b2c0: 7473 2063 6f64 6562 6173 652e 0a20 2049  ts codebase..  I
-0000b2d0: 6620 796f 7520 6861 7665 2063 6f64 6520  f you have code 
-0000b2e0: 7468 6174 2069 6d70 6f72 7473 2064 6972  that imports dir
-0000b2f0: 6563 746c 7920 6672 6f6d 2054 7261 6974  ectly from Trait
-0000b300: 7320 6d6f 6475 6c65 7320 616e 6420 7375  s modules and su
-0000b310: 6270 6163 6b61 6765 730a 2020 696e 7374  bpackages.  inst
-0000b320: 6561 6420 6f66 2066 726f 6d20 6060 7472  ead of from ``tr
-0000b330: 6169 7473 2e61 7069 6060 206f 7220 7468  aits.api`` or th
-0000b340: 6520 6f74 6865 7220 7375 6270 6163 6b61  e other subpacka
-0000b350: 6765 2060 6061 7069 6060 206d 6f64 756c  ge ``api`` modul
-0000b360: 6573 2c20 736f 6d65 0a20 206f 6620 7468  es, some.  of th
-0000b370: 6f73 6520 696d 706f 7274 7320 6d61 7920  ose imports may 
-0000b380: 6661 696c 2e20 546f 2061 766f 6964 2070  fail. To avoid p
-0000b390: 6f74 656e 7469 616c 2066 6f72 2060 6049  otential for ``I
-0000b3a0: 6d70 6f72 7445 7272 6f72 6060 732c 2079  mportError``s, y
-0000b3b0: 6f75 0a20 2073 686f 756c 6420 696d 706f  ou.  should impo
-0000b3c0: 7274 2066 726f 6d20 6060 7472 6169 7473  rt from ``traits
-0000b3d0: 2e61 7069 6060 2077 6865 6e65 7665 7220  .api`` whenever 
-0000b3e0: 706f 7373 6962 6c65 2e20 4966 2079 6f75  possible. If you
-0000b3f0: 2066 696e 6420 796f 7572 7365 6c66 0a20   find yourself. 
-0000b400: 206e 6565 6469 6e67 2073 6f6d 6520 7069   needing some pi
-0000b410: 6563 6520 6f66 2054 7261 6974 7320 6675  ece of Traits fu
-0000b420: 6e63 7469 6f6e 616c 6974 7920 7468 6174  nctionality that
-0000b430: 2069 736e 2774 2065 7870 6f73 6564 2069   isn't exposed i
-0000b440: 6e0a 2020 6060 7472 6169 7473 2e61 7069  n.  ``traits.api
-0000b450: 6060 2c20 616e 6420 796f 7520 7468 696e  ``, and you thin
-0000b460: 6b20 6974 2073 686f 756c 6420 6265 2c20  k it should be, 
-0000b470: 706c 6561 7365 206f 7065 6e20 616e 2069  please open an i
-0000b480: 7373 7565 206f 6e20 7468 650a 2020 5472  ssue on the.  Tr
-0000b490: 6169 7473 2062 7567 2074 7261 636b 6572  aits bug tracker
-0000b4a0: 2e0a 0a46 6561 7475 7265 730a 7e7e 7e7e  ...Features.~~~~
-0000b4b0: 7e7e 7e7e 0a0a 2a20 4164 6420 6e65 7720  ~~~~..* Add new 
-0000b4c0: 6060 4461 7465 7469 6d65 6060 2074 7261  ``Datetime`` tra
-0000b4d0: 6974 2074 7970 652e 2028 2337 3337 2c20  it type. (#737, 
-0000b4e0: 2338 3134 2c20 2338 3133 2c20 2338 3135  #814, #813, #815
-0000b4f0: 2c20 2338 3438 290a 2a20 5375 7070 6f72  , #848).* Suppor
-0000b500: 7420 5079 7468 6f6e 2045 6e75 6d73 2061  t Python Enums a
-0000b510: 7320 7661 6c75 6520 7365 7473 2066 6f72  s value sets for
-0000b520: 2074 6865 2060 6045 6e75 6d60 6020 7472   the ``Enum`` tr
-0000b530: 6169 742e 2028 2336 3835 2c20 2338 3238  ait. (#685, #828
-0000b540: 2c20 2338 3535 290a 2a20 4164 6420 6060  , #855).* Add ``
-0000b550: 5375 6263 6c61 7373 6060 2061 6c69 6173  Subclass`` alias
-0000b560: 2066 6f72 2074 6865 2060 6054 7970 6560   for the ``Type`
-0000b570: 6020 7472 6169 7420 7479 7065 2e20 2823  ` trait type. (#
-0000b580: 3733 3929 0a2a 2041 6464 2070 6174 682d  739).* Add path-
-0000b590: 6c69 6b65 2073 7570 706f 7274 2066 6f72  like support for
-0000b5a0: 2074 6865 2060 6046 696c 6560 6020 7472   the ``File`` tr
-0000b5b0: 6169 742e 2028 2337 3336 290a 2a20 4164  ait. (#736).* Ad
-0000b5c0: 6420 6e65 7720 6060 436f 6d70 6172 6973  d new ``Comparis
-0000b5d0: 6f6e 4d6f 6465 6060 2065 6e75 6d65 7261  onMode`` enumera
-0000b5e0: 7469 6f6e 2074 7970 6520 746f 2072 6570  tion type to rep
-0000b5f0: 6c61 6365 2074 6865 206f 6c64 0a20 2060  lace the old.  `
-0000b600: 604e 4f5f 434f 4d50 4152 4560 602c 2060  `NO_COMPARE``, `
-0000b610: 604f 424a 4543 545f 4944 454e 5449 5459  `OBJECT_IDENTITY
-0000b620: 5f43 4f4d 5041 5245 6060 2061 6e64 2060  _COMPARE`` and `
-0000b630: 6052 4943 485f 434f 4d50 4152 4560 600a  `RICH_COMPARE``.
-0000b640: 2020 636f 6e73 7461 6e74 732e 2054 6865    constants. The
-0000b650: 206f 6c64 2063 6f6e 7374 616e 7473 2061   old constants a
-0000b660: 7265 2064 6570 7265 6361 7465 642e 2028  re deprecated. (
-0000b670: 2338 3330 2c20 2337 3139 2c20 2336 3830  #830, #719, #680
-0000b680: 290a 2a20 4164 6420 6661 7374 2076 616c  ).* Add fast val
-0000b690: 6964 6174 696f 6e20 666f 7220 6060 4361  idation for ``Ca
-0000b6a0: 6c6c 6162 6c65 6060 2074 7261 6974 2074  llable`` trait t
-0000b6b0: 7970 653b 2069 6e74 726f 6475 6365 0a20  ype; introduce. 
-0000b6c0: 206e 6577 2060 6042 6173 6543 616c 6c61   new ``BaseCalla
-0000b6d0: 626c 6560 6020 7472 6169 7420 7479 7065  ble`` trait type
-0000b6e0: 2066 6f72 2073 7562 636c 6173 7369 6e67   for subclassing
-0000b6f0: 2070 7572 706f 7365 732e 0a20 2028 2337   purposes..  (#7
-0000b700: 3938 2c20 2337 3935 2c20 2337 3637 290a  98, #795, #767).
-0000b710: 2a20 4164 6420 6060 4354 7261 6974 2e63  * Add ``CTrait.c
-0000b720: 6f6d 7061 7269 736f 6e5f 6d6f 6465 6060  omparison_mode``
-0000b730: 2070 726f 7065 7274 7920 746f 2061 6c6c   property to all
-0000b740: 6f77 2069 6e73 7065 6374 696f 6e20 616e  ow inspection an
-0000b750: 640a 2020 6d6f 6469 6669 6361 7469 6f6e  d.  modification
-0000b760: 206f 6620 6120 7472 6169 7427 7320 636f   of a trait's co
-0000b770: 6d70 6172 6973 6f6e 206d 6f64 652e 2028  mparison mode. (
-0000b780: 2337 3538 2c20 2337 3335 290a 2a20 4164  #758, #735).* Ad
-0000b790: 6420 6060 6173 5f63 7472 6169 7460 6020  d ``as_ctrait`` 
-0000b7a0: 636f 6e76 6572 7465 7220 6675 6e63 7469  converter functi
-0000b7b0: 6f6e 2074 6f20 6060 7472 6169 7473 2e61  on to ``traits.a
-0000b7c0: 7069 6060 2e20 5468 6973 2066 756e 6374  pi``. This funct
-0000b7d0: 696f 6e0a 2020 636f 6e76 6572 7473 2061  ion.  converts a
-0000b7e0: 2074 7261 6974 2d6c 696b 6520 6f62 6a65   trait-like obje
-0000b7f0: 6374 206f 7220 7479 7065 2074 6f20 6120  ct or type to a 
-0000b800: 6060 4354 7261 6974 6060 2c20 7261 6973  ``CTrait``, rais
-0000b810: 696e 6720 6060 5479 7065 4572 726f 7260  ing ``TypeError`
-0000b820: 600a 2020 666f 7220 6f62 6a65 6374 7320  `.  for objects 
-0000b830: 7468 6174 2063 616e 2774 2062 6520 696e  that can't be in
-0000b840: 7465 7270 7265 7465 6420 6173 2061 2060  terpreted as a `
-0000b850: 6043 5472 6169 7460 602e 2049 7427 7320  `CTrait``. It's 
-0000b860: 696e 7465 6e64 6564 0a20 2066 6f72 2075  intended.  for u
-0000b870: 7365 2062 7920 7573 6572 7320 7768 6f20  se by users who 
-0000b880: 7761 6e74 2074 6f20 6372 6561 7465 2074  want to create t
-0000b890: 6865 6972 206f 776e 2070 6172 616d 6574  heir own paramet
-0000b8a0: 6572 6973 6564 2074 7261 6974 0a20 2074  erised trait.  t
-0000b8b0: 7970 6573 2e0a 0a20 2054 6865 2060 6061  ypes...  The ``a
-0000b8c0: 735f 6374 7261 6974 6060 2066 6561 7475  s_ctrait`` featu
-0000b8d0: 7265 2063 6f6d 6573 2077 6974 682c 2061  re comes with, a
-0000b8e0: 6e64 2072 656c 6965 7320 7570 6f6e 2c20  nd relies upon, 
-0000b8f0: 6120 6e65 7720 696e 666f 726d 616c 0a20  a new informal. 
-0000b900: 2069 6e74 6572 6661 6365 3a20 6f62 6a65   interface: obje
-0000b910: 6374 7320 7468 6174 2063 616e 2062 6520  cts that can be 
-0000b920: 636f 6e76 6572 7465 6420 746f 2073 6f6d  converted to som
-0000b930: 6574 6869 6e67 206f 6620 7479 7065 2060  ething of type `
-0000b940: 6043 5472 6169 7460 6020 6361 6e0a 2020  `CTrait`` can.  
-0000b950: 7072 6f76 6964 6520 616e 207a 6572 6f2d  provide an zero-
-0000b960: 6172 6775 6d65 6e74 2060 6061 735f 6374  argument ``as_ct
-0000b970: 7261 6974 6060 206d 6574 686f 6420 7468  rait`` method th
-0000b980: 6174 2072 6574 7572 6e73 2061 206e 6577  at returns a new
-0000b990: 2060 6043 5472 6169 7460 602e 0a20 2054   ``CTrait``..  T
-0000b9a0: 7970 6573 2063 616e 2070 726f 7669 6465  ypes can provide
-0000b9b0: 2061 6e20 6060 696e 7374 616e 7469 6174   an ``instantiat
-0000b9c0: 655f 616e 645f 6765 745f 6374 7261 6974  e_and_get_ctrait
-0000b9d0: 6060 206d 6574 686f 642c 2077 6869 6368  `` method, which
-0000b9e0: 2077 6865 6e0a 2020 6361 6c6c 6564 2077   when.  called w
-0000b9f0: 6974 6820 6e6f 2061 7267 756d 656e 7473  ith no arguments
-0000ba00: 2070 726f 7669 6465 7320 6120 6e65 7720   provides a new 
-0000ba10: 6060 4354 7261 6974 6060 2066 6f72 2074  ``CTrait`` for t
-0000ba20: 6861 7420 7479 7065 2e0a 2020 2823 3738  hat type..  (#78
-0000ba30: 332c 2023 3739 3429 0a2a 2041 6464 2061  3, #794).* Add a
-0000ba40: 206e 6577 2060 6048 6173 5472 6169 7473   new ``HasTraits
-0000ba50: 2e5f 636c 6173 735f 7472 6169 7473 6060  ._class_traits``
-0000ba60: 206d 6574 686f 6420 666f 7220 696e 7472   method for intr
-0000ba70: 6f73 7065 6374 696f 6e20 6f66 2061 6e0a  ospection of an.
-0000ba80: 2020 6f62 6a65 6374 2773 2063 6c61 7373    object's class
-0000ba90: 2074 7261 6974 732e 2054 6869 7320 7061   traits. This pa
-0000baa0: 7261 6c6c 656c 7320 7468 6520 6578 6973  rallels the exis
-0000bab0: 7469 6e67 0a20 2060 6048 6173 5472 6169  ting.  ``HasTrai
-0000bac0: 7473 2e5f 696e 7374 616e 6365 5f74 7261  ts._instance_tra
-0000bad0: 6974 7360 6020 6d65 7468 6f64 2e20 5468  its`` method. Th
-0000bae0: 6973 206d 6574 686f 6420 6973 2069 6e74  is method is int
-0000baf0: 656e 6465 6420 666f 7220 7573 6520 696e  ended for use in
-0000bb00: 0a20 2064 6562 7567 6769 6e67 2e20 4974  .  debugging. It
-0000bb10: 2773 206e 6f74 2072 6563 6f6d 6d65 6e64  's not recommend
-0000bb20: 6564 2066 6f72 2075 7365 7273 2074 6f20  ed for users to 
-0000bb30: 6d6f 6469 6679 2074 6865 2072 6574 7572  modify the retur
-0000bb40: 6e65 6420 6469 6374 696f 6e61 7279 2e0a  ned dictionary..
-0000bb50: 2020 2823 3730 3229 0a2a 2041 6464 2060    (#702).* Add `
-0000bb60: 6043 5472 6169 742e 7365 745f 6465 6661  `CTrait.set_defa
-0000bb70: 756c 745f 7661 6c75 6560 6020 6d65 7468  ult_value`` meth
-0000bb80: 6f64 2066 6f72 2073 6574 7469 6e67 2069  od for setting i
-0000bb90: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-0000bba0: 2074 6865 0a20 2064 6566 6175 6c74 206f   the.  default o
-0000bbb0: 6620 6120 6060 4354 7261 6974 6060 2e20  f a ``CTrait``. 
-0000bbc0: 5468 6973 2070 726f 7669 6465 7320 616e  This provides an
-0000bbd0: 2061 6c74 6572 6e61 7469 7665 2074 6f20   alternative to 
-0000bbe0: 7468 6520 7072 6576 696f 7573 206d 6574  the previous met
-0000bbf0: 686f 640a 2020 6f66 2075 7369 6e67 2060  hod.  of using `
-0000bc00: 6043 5472 6169 742e 6465 6661 756c 745f  `CTrait.default_
-0000bc10: 7661 6c75 6560 602e 2054 6865 2075 7365  value``. The use
-0000bc20: 206f 6620 6060 4354 7261 6974 2e64 6566   of ``CTrait.def
-0000bc30: 6175 6c74 5f76 616c 7565 6060 2074 6f20  ault_value`` to 
-0000bc40: 7365 740a 2020 2872 6174 6865 7220 7468  set.  (rather th
-0000bc50: 616e 2067 6574 2920 6465 6661 756c 7420  an get) default 
-0000bc60: 696e 666f 726d 6174 696f 6e20 6973 2064  information is d
-0000bc70: 6570 7265 6361 7465 642e 2028 2336 3230  eprecated. (#620
-0000bc80: 290a 2a20 4164 6420 6e65 7720 6d65 7468  ).* Add new meth
-0000bc90: 6f64 7320 6060 4861 7354 7261 6974 732e  ods ``HasTraits.
-0000bca0: 5f74 7261 6974 5f6e 6f74 6966 6963 6174  _trait_notificat
-0000bcb0: 696f 6e73 5f65 6e61 626c 6564 6060 2c0a  ions_enabled``,.
-0000bcc0: 2020 6060 4861 7354 7261 6974 732e 5f74    ``HasTraits._t
-0000bcd0: 7261 6974 5f6e 6f74 6966 6963 6174 696f  rait_notificatio
-0000bce0: 6e73 5f76 6574 6f65 6460 6020 746f 2061  ns_vetoed`` to a
-0000bcf0: 6c6c 6f77 2069 6e74 726f 7370 6563 7469  llow introspecti
-0000bd00: 6f6e 206f 6620 7468 650a 2020 6e6f 7469  on of the.  noti
-0000bd10: 6669 6361 7469 6f6e 7320 7374 6174 6573  fications states
-0000bd20: 2073 6574 2062 7920 7468 6520 6578 6973   set by the exis
-0000bd30: 7469 6e67 206d 6574 686f 6473 0a20 2060  ting methods.  `
-0000bd40: 6048 6173 5472 6169 7473 2e5f 7472 6169  `HasTraits._trai
-0000bd50: 745f 6368 616e 6765 5f6e 6f74 6966 7960  t_change_notify`
-0000bd60: 6020 616e 6420 6060 4861 7354 7261 6974  ` and ``HasTrait
-0000bd70: 732e 5f74 7261 6974 5f76 6574 6f5f 6e6f  s._trait_veto_no
-0000bd80: 7469 6679 6060 2e0a 2020 2823 3730 3429  tify``..  (#704)
-0000bd90: 0a2a 2041 6464 2060 6054 7261 6974 4b69  .* Add ``TraitKi
-0000bda0: 6e64 6060 2c20 6060 5661 6c69 6461 7465  nd``, ``Validate
-0000bdb0: 5472 6169 7460 6020 616e 6420 6060 4465  Trait`` and ``De
-0000bdc0: 6661 756c 7456 616c 7565 6060 2050 7974  faultValue`` Pyt
-0000bdd0: 686f 6e20 656e 756d 6572 6174 696f 6e0a  hon enumeration.
-0000bde0: 2020 7479 7065 7320 746f 2072 6570 6c61    types to repla
-0000bdf0: 6365 2070 7265 7669 6f75 7320 7573 6573  ce previous uses
-0000be00: 206f 6620 6d61 6769 6320 696e 7465 6765   of magic intege
-0000be10: 7273 2077 6974 6869 6e20 7468 6520 5472  rs within the Tr
-0000be20: 6169 7473 2063 6f64 6562 6173 652e 0a20  aits codebase.. 
-0000be30: 2028 2336 3830 2c20 2338 3537 290a 2a20   (#680, #857).* 
-0000be40: 5468 6520 7661 7269 6f75 7320 6060 4354  The various ``CT
-0000be50: 7261 6974 6060 2069 6e74 6572 6e61 6c20  rait`` internal 
-0000be60: 666c 6167 7320 6172 6520 6e6f 7720 6578  flags are now ex
-0000be70: 706f 7365 6420 746f 2050 7974 686f 6e20  posed to Python 
-0000be80: 6173 0a20 2070 726f 7065 7274 6965 733a  as.  properties:
-0000be90: 2060 6043 5472 6169 742e 6973 5f70 726f   ``CTrait.is_pro
-0000bea0: 7065 7274 7960 6020 2872 6561 642d 6f6e  perty`` (read-on
-0000beb0: 6c79 292c 2060 6043 5472 6169 742e 6d6f  ly), ``CTrait.mo
-0000bec0: 6469 6679 5f64 656c 6567 6174 6560 602c  dify_delegate``,
-0000bed0: 0a20 2060 6043 5472 6169 742e 7365 7461  .  ``CTrait.seta
-0000bee0: 7474 725f 6f72 6967 696e 616c 5f76 616c  ttr_original_val
-0000bef0: 7565 6060 2c20 6060 4354 7261 6974 2e70  ue``, ``CTrait.p
-0000bf00: 6f73 745f 7365 7461 7474 725f 6f72 6967  ost_setattr_orig
-0000bf10: 696e 616c 5f76 616c 7565 6060 2c0a 2020  inal_value``,.  
-0000bf20: 6060 4354 7261 6974 2e69 735f 6d61 7070  ``CTrait.is_mapp
-0000bf30: 6564 6060 2c20 616e 6420 6060 4354 7261  ed``, and ``CTra
-0000bf40: 6974 2e63 6f6d 7061 7269 736f 6e5f 6d6f  it.comparison_mo
-0000bf50: 6465 6060 2e20 2823 3636 362c 2023 3639  de``. (#666, #69
-0000bf60: 3329 0a0a 4368 616e 6765 730a 7e7e 7e7e  3)..Changes.~~~~
-0000bf70: 7e7e 7e0a 0a2a 2057 6865 6e20 7069 636b  ~~~..* When pick
-0000bf80: 6c69 6e67 2061 2060 6043 5472 6169 7460  ling a ``CTrait`
-0000bf90: 602c 2074 6865 2060 6070 795f 706f 7374  `, the ``py_post
-0000bfa0: 5f73 6574 6174 7472 6060 2061 6e64 2060  _setattr`` and `
-0000bfb0: 6070 795f 7661 6c69 6461 7465 6060 0a20  `py_validate``. 
-0000bfc0: 2066 6965 6c64 7320 6172 6520 7069 636b   fields are pick
-0000bfd0: 6c65 6420 6469 7265 6374 6c79 2e20 5072  led directly. Pr
-0000bfe0: 6576 696f 7573 6c79 2c20 6361 6c6c 6162  eviously, callab
-0000bff0: 6c65 7320 666f 7220 7468 6f73 6520 6669  les for those fi
-0000c000: 656c 6473 2077 6572 650a 2020 7265 706c  elds were.  repl
-0000c010: 6163 6564 2077 6974 6820 6120 6060 2d31  aced with a ``-1
-0000c020: 6060 2073 656e 7469 6e65 6c20 6f6e 2070  `` sentinel on p
-0000c030: 6963 6b6c 696e 672e 2028 2337 3830 290a  ickling. (#780).
-0000c040: 2a20 4120 6060 5472 6169 744c 6973 7445  * A ``TraitListE
-0000c050: 7665 6e74 6060 2069 7320 6e6f 206c 6f6e  vent`` is no lon
-0000c060: 6765 7220 656d 6974 7465 6420 666f 7220  ger emitted for 
-0000c070: 6120 736c 6963 6520 6465 6c65 7469 6f6e  a slice deletion
-0000c080: 2077 6869 6368 0a20 2064 6f65 736e 2774   which.  doesn't
-0000c090: 2063 6861 6e67 6520 7468 6520 636f 6e74   change the cont
-0000c0a0: 656e 7473 206f 6620 7468 6520 6c69 7374  ents of the list
-0000c0b0: 2e20 2846 6f72 2065 7861 6d70 6c65 2c20  . (For example, 
-0000c0c0: 6064 656c 206f 626a 2e6d 796c 6973 745b  `del obj.mylist[
-0000c0d0: 323a 5d60 0a20 206f 6e20 6120 6c69 7374  2:]`.  on a list
-0000c0e0: 2074 6861 7420 6f6e 6c79 2068 6173 2032   that only has 2
-0000c0f0: 2065 6c65 6d65 6e74 732e 2920 2823 3734   elements.) (#74
-0000c100: 3029 0a2a 2054 6865 2060 6061 6464 6564  0).* The ``added
-0000c110: 6060 2061 6e64 2060 6072 656d 6f76 6564  `` and ``removed
-0000c120: 6060 2061 7474 7269 6275 7465 7320 6f6e  `` attributes on
-0000c130: 2061 2060 6054 7261 6974 4c69 7374 4576   a ``TraitListEv
-0000c140: 656e 7460 6020 6172 6520 6e6f 770a 2020  ent`` are now.  
-0000c150: 616c 7761 7973 206c 6973 7473 2063 6f6e  always lists con
-0000c160: 7461 696e 696e 6720 7468 6520 6164 6465  taining the adde
-0000c170: 6420 6f72 2072 656d 6f76 6564 2065 6c65  d or removed ele
-0000c180: 6d65 6e74 732e 2050 7265 7669 6f75 736c  ments. Previousl
-0000c190: 792c 2074 686f 7365 0a20 206c 6973 7473  y, those.  lists
-0000c1a0: 2077 6572 6520 6e65 7374 6564 2069 6e73   were nested ins
-0000c1b0: 6964 6520 616e 6f74 6865 7220 6c69 7374  ide another list
-0000c1c0: 2069 6e20 736f 6d65 2063 6173 6573 2e20   in some cases. 
-0000c1d0: 2823 3737 3129 0a2a 2043 6861 6e67 6520  (#771).* Change 
-0000c1e0: 6060 496e 7374 616e 6365 2849 536f 6d65  ``Instance(ISome
-0000c1f0: 496e 7465 7266 6163 6529 6060 2074 6f20  Interface)`` to 
-0000c200: 7573 6520 616e 2060 6069 7369 6e73 7461  use an ``isinsta
-0000c210: 6e63 6560 6020 6368 6563 6b20 6f6e 0a20  nce`` check on. 
-0000c220: 2074 7261 6974 2073 6574 2069 6e73 7465   trait set inste
-0000c230: 6164 206f 6620 7573 696e 6720 7468 6520  ad of using the 
-0000c240: 6479 6e61 6d69 6320 696e 7465 7266 6163  dynamic interfac
-0000c250: 6520 6368 6563 6b65 722e 2028 2336 3330  e checker. (#630
-0000c260: 290a 2a20 4372 6561 7465 2061 6e20 6e65  ).* Create an ne
-0000c270: 7720 6060 4162 7374 7261 6374 5669 6577  w ``AbstractView
-0000c280: 456c 656d 656e 7460 6020 6162 7374 7261  Element`` abstra
-0000c290: 6374 2062 6173 6520 636c 6173 732c 2061  ct base class, a
-0000c2a0: 6e64 2072 6567 6973 7465 720a 2020 7468  nd register.  th
-0000c2b0: 6520 5472 6169 7473 5549 2060 6056 6965  e TraitsUI ``Vie
-0000c2c0: 7745 6c65 6d65 6e74 6060 2061 7320 696d  wElement`` as im
-0000c2d0: 706c 656d 656e 7469 6e67 2069 742e 2054  plementing it. T
-0000c2e0: 6869 7320 7061 7665 7320 7468 6520 7761  his paves the wa
-0000c2f0: 7920 666f 720a 2020 7265 6d6f 7661 6c20  y for.  removal 
-0000c300: 6f66 2054 7261 6974 7320 5549 2069 6d70  of Traits UI imp
-0000c310: 6f72 7473 2066 726f 6d20 5472 6169 7473  orts from Traits
-0000c320: 2e20 2823 3631 3729 0a2a 2060 6056 6965  . (#617).* ``Vie
-0000c330: 7745 6c65 6d65 6e74 7360 6020 6172 6520  wElements`` are 
-0000c340: 6e6f 7720 636f 6d70 7574 6564 206c 617a  now computed laz
-0000c350: 696c 792c 2069 6e73 7465 6164 206f 6620  ily, instead of 
-0000c360: 6174 2060 6048 6173 5472 6169 7473 6060  at ``HasTraits``
-0000c370: 0a20 2073 7562 636c 6173 7320 6372 6561  .  subclass crea
-0000c380: 7469 6f6e 2074 696d 652e 2054 6869 7320  tion time. This 
-0000c390: 7265 6d6f 7665 7320 6120 6060 7472 6169  removes a ``trai
-0000c3a0: 7473 7569 6060 2069 6d70 6f72 7420 6672  tsui`` import fr
-0000c3b0: 6f6d 0a20 2074 6865 2060 6074 7261 6974  om.  the ``trait
-0000c3c0: 2e68 6173 5f74 7261 6974 7360 6020 6d6f  .has_traits`` mo
-0000c3d0: 6475 6c65 2e20 2823 3631 3429 0a2a 2054  dule. (#614).* T
-0000c3e0: 6865 2060 6074 7261 6974 732e 7574 696c  he ``traits.util
-0000c3f0: 2e63 6c65 616e 5f66 696c 656e 616d 6560  .clean_filename`
-0000c400: 6020 7574 696c 6974 7920 6e6f 7720 7573  ` utility now us
-0000c410: 6573 2061 2064 6966 6665 7265 6e74 2061  es a different a
-0000c420: 6c67 6f72 6974 686d 2c0a 2020 616e 6420  lgorithm,.  and 
-0000c430: 7368 6f75 6c64 2064 6f20 6120 6265 7474  should do a bett
-0000c440: 6572 206a 6f62 2077 6974 6820 6163 6365  er job with acce
-0000c450: 6e74 6564 2061 6e64 2055 6e69 636f 6465  nted and Unicode
-0000c460: 2074 6578 742e 2028 2335 3839 290a 2a20   text. (#589).* 
-0000c470: 466c 6f61 7469 6e67 2d70 6f69 6e74 2061  Floating-point a
-0000c480: 6e64 2069 6e74 6567 6572 2063 6865 636b  nd integer check
-0000c490: 7320 6172 6520 6e6f 7720 6d6f 7265 2063  s are now more c
-0000c4a0: 6f6e 7369 7374 656e 7420 6265 7477 6565  onsistent betwee
-0000c4b0: 6e20 636c 6173 7365 732e 0a20 2049 6e20  n classes..  In 
-0000c4c0: 7061 7274 6963 756c 6172 2c20 6060 4261  particular, ``Ba
-0000c4d0: 7365 496e 7460 6020 7661 6c69 6461 7469  seInt`` validati
-0000c4e0: 6f6e 206e 6f77 206d 6174 6368 6573 2060  on now matches `
-0000c4f0: 6049 6e74 6060 2076 616c 6964 6174 696f  `Int`` validatio
-0000c500: 6e2c 2061 6e64 0a20 2060 6052 616e 6765  n, and.  ``Range
-0000c510: 6060 2074 7970 6520 6368 6563 6b73 206e  `` type checks n
-0000c520: 6f77 206d 6174 6368 2074 686f 7365 2075  ow match those u
-0000c530: 7365 6420 696e 2060 6049 6e74 6060 2061  sed in ``Int`` a
-0000c540: 6e64 2060 6046 6c6f 6174 6060 2e20 2823  nd ``Float``. (#
-0000c550: 3538 3829 0a2a 2041 6e20 6578 6365 7074  588).* An except
-0000c560: 696f 6e20 6f74 6865 7220 7468 616e 2060  ion other than `
-0000c570: 6054 7261 6974 4572 726f 7260 6020 7261  `TraitError`` ra
-0000c580: 6973 6564 2064 7572 696e 6720 7661 6c69  ised during vali
-0000c590: 6461 7469 6f6e 206f 6620 610a 2020 636f  dation of a.  co
-0000c5a0: 6d70 6f75 6e64 2074 7261 6974 2077 696c  mpound trait wil
-0000c5b0: 6c20 6e6f 7720 6265 2070 726f 7061 6761  l now be propaga
-0000c5c0: 7465 642e 2050 7265 7669 6f75 736c 792c  ted. Previously,
-0000c5d0: 2074 6861 7420 6578 6365 7074 696f 6e20   that exception 
-0000c5e0: 776f 756c 640a 2020 6265 2073 7761 6c6c  would.  be swall
-0000c5f0: 6f77 6564 2e20 2823 3538 3129 0a2a 2054  owed. (#581).* T
-0000c600: 7261 6974 7320 6e6f 206c 6f6e 6765 7220  raits no longer 
-0000c610: 6861 7320 6120 7275 6e74 696d 6520 6465  has a runtime de
-0000c620: 7065 6e64 656e 6379 206f 6e20 7468 6520  pendency on the 
-0000c630: 6060 7369 7860 6020 7061 636b 6167 652e  ``six`` package.
-0000c640: 2028 2336 3338 290a 2a20 5573 6520 7069   (#638).* Use pi
-0000c650: 636b 6c65 2070 726f 746f 636f 6c20 3320  ckle protocol 3 
-0000c660: 696e 7374 6561 6420 6f66 2070 6963 6b6c  instead of pickl
-0000c670: 6520 7072 6f74 6f63 6f6c 2031 2077 6865  e protocol 1 whe
-0000c680: 6e20 7772 6974 696e 6720 7069 636b 6c65  n writing pickle
-0000c690: 640a 2020 6f62 6a65 6374 2073 7461 7465  d.  object state
-0000c6a0: 2074 6f20 6120 6669 6c65 2069 6e20 6060   to a file in ``
-0000c6b0: 636f 6e66 6967 7572 655f 7472 6169 7473  configure_traits
-0000c6c0: 6060 2e20 2823 3739 3629 0a2a 2049 6e20  ``. (#796).* In 
-0000c6d0: 6060 7472 6169 7473 2e74 6573 7469 6e67  ``traits.testing
-0000c6e0: 2e6f 7074 696f 6e61 6c5f 6465 7065 6e64  .optional_depend
-0000c6f0: 656e 6369 6573 6060 2c20 6d61 6b65 2073  encies``, make s
-0000c700: 7572 6520 6060 7472 6169 7473 7569 2e61  ure ``traitsui.a
-0000c710: 7069 6060 2069 730a 2020 6176 6169 6c61  pi`` is.  availa
-0000c720: 626c 6520 7768 656e 6576 6572 2060 6074  ble whenever ``t
-0000c730: 7261 6974 7375 6960 6020 6973 2e20 2823  raitsui`` is. (#
-0000c740: 3631 3629 0a2a 2060 6054 7261 6974 496e  616).* ``TraitIn
-0000c750: 7374 616e 6365 6060 206e 6f77 2069 6e68  stance`` now inh
-0000c760: 6572 6974 7320 6469 7265 6374 6c79 2066  erits directly f
-0000c770: 726f 6d20 6060 5472 6169 7448 616e 646c  rom ``TraitHandl
-0000c780: 6572 6060 2069 6e73 7465 6164 206f 660a  er`` instead of.
-0000c790: 2020 2874 6865 206e 6f77 2072 656d 6f76    (the now remov
-0000c7a0: 6564 2920 6060 5468 6973 436c 6173 7360  ed) ``ThisClass`
-0000c7b0: 602e 2028 2337 3631 290a 0a46 6978 6573  `. (#761)..Fixes
-0000c7c0: 0a7e 7e7e 7e7e 0a0a 2a20 4669 7820 6120  .~~~~~..* Fix a 
-0000c7d0: 7573 6520 6f66 2074 6865 2075 6e73 7570  use of the unsup
-0000c7e0: 706f 7274 6564 2060 6056 616c 6964 6174  ported ``Validat
-0000c7f0: 6554 7261 6974 2e69 6e74 5f72 616e 6765  eTrait.int_range
-0000c800: 6060 2e20 2823 3830 3529 0a2a 2052 656d  ``. (#805).* Rem
-0000c810: 6f76 6520 756e 6e65 6365 7373 6172 7920  ove unnecessary 
-0000c820: 6060 636f 7079 6060 206d 6574 686f 6420  ``copy`` method 
-0000c830: 6f76 6572 7269 6465 2066 726f 6d20 6060  override from ``
-0000c840: 5472 6169 7453 6574 4f62 6a65 6374 6060  TraitSetObject``
-0000c850: 2e20 2823 3735 3929 0a2a 2046 6978 2060  . (#759).* Fix `
-0000c860: 6054 7261 6974 4c69 7374 4f62 6a65 6374  `TraitListObject
-0000c870: 2e63 6c65 6172 6060 2074 6f20 6973 7375  .clear`` to issu
-0000c880: 6520 7468 6520 6170 7072 6f70 7269 6174  e the appropriat
-0000c890: 6520 6974 656d 7320 6576 656e 742e 2028  e items event. (
-0000c8a0: 2337 3332 290a 2a20 4669 7820 636f 6e66  #732).* Fix conf
-0000c8b0: 7573 696e 6720 6572 726f 7220 6d65 7373  using error mess
-0000c8c0: 6167 6520 7768 656e 2060 605b 4e6f 6e65  age when ``[None
-0000c8d0: 5d60 6020 7061 7373 6564 2069 6e74 6f0a  ]`` passed into.
-0000c8e0: 2020 6060 4c69 7374 2854 6869 7328 616c    ``List(This(al
-0000c8f0: 6c6f 775f 6e6f 6e65 3d46 616c 7365 2929  low_none=False))
-0000c900: 6060 2e20 2823 3733 3429 0a2a 2046 6978  ``. (#734).* Fix
-0000c910: 206e 616d 652d 6d61 6e67 6c69 6e67 206f   name-mangling o
-0000c920: 6620 646f 7562 6c65 2d75 6e64 6572 7363  f double-undersc
-0000c930: 6f72 6520 7072 6976 6174 6520 6d65 7468  ore private meth
-0000c940: 6f64 7320 696e 2063 6c61 7373 6573 2077  ods in classes w
-0000c950: 686f 7365 0a20 206e 616d 6520 6265 6769  hose.  name begi
-0000c960: 6e73 2077 6974 6820 616e 2075 6e64 6572  ns with an under
-0000c970: 7363 6f72 652e 2028 2337 3234 290a 2a20  score. (#724).* 
-0000c980: 4669 7820 6060 6279 7465 735f 6564 6974  Fix ``bytes_edit
-0000c990: 6f72 6060 2061 6e64 2060 6070 6173 7377  or`` and ``passw
-0000c9a0: 6f72 645f 6564 6974 6f72 6060 2062 7567  ord_editor`` bug
-0000c9b0: 732c 2061 6e64 2061 6464 2074 6573 7473  s, and add tests
-0000c9c0: 2066 6f72 0a20 2061 6c6c 2065 6469 746f   for.  all edito
-0000c9d0: 7220 6661 6374 6f72 6965 732e 2028 2336  r factories. (#6
-0000c9e0: 3630 290a 2a20 4669 7820 636f 6572 6369  60).* Fix coerci
-0000c9f0: 6f6e 2066 6173 7420 7661 6c69 6461 7469  on fast validati
-0000ca00: 6f6e 2074 7970 6520 746f 2064 6f20 616e  on type to do an
-0000ca10: 2065 7861 6374 2074 7970 6520 6368 6563   exact type chec
-0000ca20: 6b20 696e 7374 6561 6420 6f66 0a20 2061  k instead of.  a
-0000ca30: 6e20 696e 7374 616e 6365 2063 6865 636b  n instance check
-0000ca40: 2e20 5468 6973 2065 6e73 7572 6573 2074  . This ensures t
-0000ca50: 6861 7420 696e 7374 616e 6365 7320 6f66  hat instances of
-0000ca60: 2073 7562 636c 6173 7365 7320 6f66 2074   subclasses of t
-0000ca70: 6865 0a20 2074 6172 6765 7420 7479 7065  he.  target type
-0000ca80: 2061 7265 2070 726f 7065 726c 7920 636f   are properly co
-0000ca90: 6e76 6572 7465 6420 746f 2074 6865 2074  nverted to the t
-0000caa0: 6172 6765 7420 7479 7065 2e20 466f 7220  arget type. For 
-0000cab0: 6578 616d 706c 652c 0a20 2069 6620 6060  example,.  if ``
-0000cac0: 5472 7565 6060 2069 7320 6173 7369 676e  True`` is assign
-0000cad0: 6564 2074 6f20 6120 7472 6169 7420 6f66  ed to a trait of
-0000cae0: 2074 7970 6520 6060 4349 6e74 6060 2c20   type ``CInt``, 
-0000caf0: 7468 6520 7265 7375 6c74 696e 670a 2020  the resulting.  
-0000cb00: 7661 6c75 6520 6973 206e 6f77 2060 6031  value is now ``1
-0000cb10: 6060 2e20 5072 6576 696f 7573 6c79 2c20  ``. Previously, 
-0000cb20: 6974 2077 6173 2060 6054 7275 6560 602e  it was ``True``.
-0000cb30: 2028 2336 3437 290a 2a20 4669 7820 6060   (#647).* Fix ``
-0000cb40: 4261 7365 5261 6e67 6560 6020 746f 2061  BaseRange`` to a
-0000cb50: 6363 6570 7420 7468 6520 7361 6d65 2076  ccept the same v
-0000cb60: 616c 7565 7320 6173 2060 6052 616e 6765  alues as ``Range
-0000cb70: 6060 2e20 2823 3538 3329 0a2a 2046 6978  ``. (#583).* Fix
-0000cb80: 2069 6e74 6567 6572 2060 6052 616e 6765   integer ``Range
-0000cb90: 6060 2074 6f20 6163 6365 7074 2069 6e74  `` to accept int
-0000cba0: 6567 6572 2d6c 696b 6520 6f62 6a65 6374  eger-like object
-0000cbb0: 732e 2028 2335 3832 290a 2a20 4669 7820  s. (#582).* Fix 
-0000cbc0: 666c 6f61 7469 6e67 2d70 6f69 6e74 2060  floating-point `
-0000cbd0: 6052 616e 6765 6060 2074 6f20 6163 6365  `Range`` to acce
-0000cbe0: 7074 2066 6c6f 6174 2d6c 696b 6520 7661  pt float-like va
-0000cbf0: 6c75 6573 2e20 2823 3537 3929 0a2a 2046  lues. (#579).* F
-0000cc00: 6978 2061 206d 6973 7369 6e67 2069 6d70  ix a missing imp
-0000cc10: 6f72 7420 696e 2074 6865 2061 6461 7074  ort in the adapt
-0000cc20: 6174 696f 6e20 6265 6e63 686d 6172 6b20  ation benchmark 
-0000cc30: 7363 7269 7074 2e20 2823 3537 3529 0a2a  script. (#575).*
-0000cc40: 2046 6978 2069 7373 7565 7320 7769 7468   Fix issues with
-0000cc50: 2074 6865 2060 6066 696c 656e 616d 6560   the ``filename`
-0000cc60: 6020 6172 6775 6d65 6e74 2074 6f20 6060  ` argument to ``
-0000cc70: 636f 6e66 6967 7572 655f 7472 6169 7473  configure_traits
-0000cc80: 6060 2e20 2823 3537 3229 0a2a 2046 6978  ``. (#572).* Fix
-0000cc90: 2061 2070 6f73 7369 626c 6520 7365 6766   a possible segf
-0000cca0: 6175 6c74 2066 726f 6d20 6361 7265 6c65  ault from carele
-0000ccb0: 7373 2066 6965 6c64 2072 652d 6173 7369  ss field re-assi
-0000ccc0: 676e 6d65 6e74 7320 696e 0a20 2060 6063  gnments in.  ``c
-0000ccd0: 7472 6169 7473 2e63 6060 2e20 2823 3834  traits.c``. (#84
-0000cce0: 3429 0a0a 4465 7072 6563 6174 696f 6e73  4)..Deprecations
-0000ccf0: 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a  .~~~~~~~~~~~~..*
-0000cd00: 2054 6865 2060 604e 4f5f 434f 4d50 4152   The ``NO_COMPAR
-0000cd10: 4560 602c 2060 604f 424a 4543 545f 4944  E``, ``OBJECT_ID
-0000cd20: 454e 5449 5459 5f43 4f4d 5041 5245 6060  ENTITY_COMPARE``
-0000cd30: 2061 6e64 2060 6052 4943 485f 434f 4d50   and ``RICH_COMP
-0000cd40: 4152 4560 600a 2020 636f 6e73 7461 6e74  ARE``.  constant
-0000cd50: 7320 6172 6520 6465 7072 6563 6174 6564  s are deprecated
-0000cd60: 2e20 5573 6520 7468 6520 636f 7272 6573  . Use the corres
-0000cd70: 706f 6e64 696e 6720 6d65 6d62 6572 7320  ponding members 
-0000cd80: 6f66 2074 6865 0a20 2060 6043 6f6d 7061  of the.  ``Compa
-0000cd90: 7269 736f 6e4d 6f64 6560 6020 656e 756d  risonMode`` enum
-0000cda0: 6572 6174 696f 6e20 696e 7374 6561 642e  eration instead.
-0000cdb0: 2028 2337 3139 290a 2a20 5468 6520 6060   (#719).* The ``
-0000cdc0: 556e 6963 6f64 6560 602c 2060 6043 556e  Unicode``, ``CUn
-0000cdd0: 6963 6f64 6560 602c 2060 6042 6173 6555  icode``, ``BaseU
-0000cde0: 6e69 636f 6465 6060 2061 6e64 2060 6042  nicode`` and ``B
-0000cdf0: 6173 6543 556e 6963 6f64 6560 6020 7472  aseCUnicode`` tr
-0000ce00: 6169 740a 2020 7479 7065 7320 6172 6520  ait.  types are 
-0000ce10: 6465 7072 6563 6174 6564 2e20 5573 6520  deprecated. Use 
-0000ce20: 6060 5374 7260 602c 2060 6043 5374 7260  ``Str``, ``CStr`
-0000ce30: 602c 2060 6042 6173 6553 7472 6060 2061  `, ``BaseStr`` a
-0000ce40: 6e64 2060 6042 6173 6543 5374 7260 600a  nd ``BaseCStr``.
-0000ce50: 2020 696e 7374 6561 642e 2028 2336 3438    instead. (#648
-0000ce60: 290a 2a20 5468 6520 6060 4c6f 6e67 6060  ).* The ``Long``
-0000ce70: 2c20 6060 434c 6f6e 6760 602c 2060 6042  , ``CLong``, ``B
-0000ce80: 6173 654c 6f6e 6760 6020 616e 6420 6060  aseLong`` and ``
-0000ce90: 4261 7365 434c 6f6e 6760 6020 7472 6169  BaseCLong`` trai
-0000cea0: 7420 7479 7065 7320 6172 650a 2020 6465  t types are.  de
-0000ceb0: 7072 6563 6174 6564 2e20 5573 6520 6060  precated. Use ``
-0000cec0: 496e 7460 602c 2060 6043 496e 7460 602c  Int``, ``CInt``,
-0000ced0: 2060 6042 6173 6549 6e74 6060 2061 6e64   ``BaseInt`` and
-0000cee0: 2060 6042 6173 6543 496e 7460 6020 696e   ``BaseCInt`` in
-0000cef0: 7374 6561 642e 0a20 2028 2336 3435 2c20  stead..  (#645, 
-0000cf00: 2335 3733 290a 2a20 5468 6520 6060 4164  #573).* The ``Ad
-0000cf10: 6170 7465 6454 6f60 6020 7472 6169 7420  aptedTo`` trait 
-0000cf20: 7479 7065 2069 7320 6465 7072 6563 6174  type is deprecat
-0000cf30: 6564 2e20 5573 6520 6060 5375 7070 6f72  ed. Use ``Suppor
-0000cf40: 7473 6060 2069 6e73 7465 6164 2e20 2823  ts`` instead. (#
-0000cf50: 3736 3029 0a2a 2054 6865 2066 6f6c 6c6f  760).* The follo
-0000cf60: 7769 6e67 2074 7261 6974 2074 7970 6520  wing trait type 
-0000cf70: 616c 6961 7365 7320 6172 6520 6465 7072  aliases are depr
-0000cf80: 6563 6174 6564 2e20 5365 6520 7468 6520  ecated. See the 
-0000cf90: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-0000cfa0: 720a 2020 7265 636f 6d6d 656e 6465 6420  r.  recommended 
-0000cfb0: 7265 706c 6163 6d65 6e74 732e 2060 6066  replacments. ``f
-0000cfc0: 616c 7365 6060 2c20 6060 7472 7565 6060  alse``, ``true``
-0000cfd0: 2c20 6060 756e 6465 6669 6e65 6460 602c  , ``undefined``,
-0000cfe0: 2060 604c 6973 7449 6e74 6060 2c0a 2020   ``ListInt``,.  
-0000cff0: 6060 4c69 7374 466c 6f61 7460 602c 2060  ``ListFloat``, `
-0000d000: 604c 6973 7453 7472 6060 2c20 6060 4c69  `ListStr``, ``Li
-0000d010: 7374 556e 6963 6f64 6560 602c 2060 604c  stUnicode``, ``L
-0000d020: 6973 7443 6f6d 706c 6578 6060 2c20 6060  istComplex``, ``
-0000d030: 4c69 7374 426f 6f6c 6060 2c0a 2020 6060  ListBool``,.  ``
-0000d040: 4c69 7374 4675 6e63 7469 6f6e 6060 2c20  ListFunction``, 
-0000d050: 6060 4c69 7374 4d65 7468 6f64 6060 2c20  ``ListMethod``, 
-0000d060: 6060 4c69 7374 5468 6973 6060 2c20 6060  ``ListThis``, ``
-0000d070: 4469 6374 5374 7241 6e79 6060 2c0a 2020  DictStrAny``,.  
-0000d080: 6060 4469 6374 5374 7253 7472 6060 2c20  ``DictStrStr``, 
-0000d090: 6060 4469 6374 5374 7249 6e74 6060 2c20  ``DictStrInt``, 
-0000d0a0: 6060 4469 6374 5374 7246 6c6f 6174 6060  ``DictStrFloat``
-0000d0b0: 2c20 6060 4469 6374 5374 7242 6f6f 6c60  , ``DictStrBool`
-0000d0c0: 602c 0a20 2060 6044 6963 7453 7472 4c69  `,.  ``DictStrLi
-0000d0d0: 7374 6060 2e20 2823 3632 3729 0a2a 2055  st``. (#627).* U
-0000d0e0: 7365 206f 6620 7468 6520 6060 6669 6c65  se of the ``file
-0000d0f0: 6e61 6d65 6060 2061 7267 756d 656e 7420  name`` argument 
-0000d100: 746f 2060 6063 6f6e 6669 6775 7265 5f74  to ``configure_t
-0000d110: 7261 6974 7360 6020 2866 6f72 2073 746f  raits`` (for sto
-0000d120: 7269 6e67 0a20 2073 7461 7465 2074 6f20  ring.  state to 
-0000d130: 6f72 2072 6573 746f 7269 6e67 2073 7461  or restoring sta
-0000d140: 7465 2066 726f 6d20 7069 636b 6c65 2066  te from pickle f
-0000d150: 696c 6573 2920 6973 2064 6570 7265 6361  iles) is depreca
-0000d160: 7465 642e 2028 2337 3932 290a 2a20 5468  ted. (#792).* Th
-0000d170: 6520 6060 5472 6169 7454 7570 6c65 6060  e ``TraitTuple``
-0000d180: 2c20 6060 5472 6169 744c 6973 7460 6020  , ``TraitList`` 
-0000d190: 616e 6420 6060 5472 6169 7444 6963 7460  and ``TraitDict`
-0000d1a0: 6020 7472 6169 7420 6861 6e64 6c65 7273  ` trait handlers
-0000d1b0: 0a20 2061 7265 2064 6570 7265 6361 7465  .  are deprecate
-0000d1c0: 642e 2055 7365 2074 6865 2060 6054 7570  d. Use the ``Tup
-0000d1d0: 6c65 6060 2c20 6060 4c69 7374 6060 2061  le``, ``List`` a
-0000d1e0: 6e64 2060 6044 6963 7460 6020 7472 6169  nd ``Dict`` trai
-0000d1f0: 7420 7479 7065 7320 696e 7374 6561 642e  t types instead.
-0000d200: 0a20 2028 2337 3730 290a 2a20 5573 6520  .  (#770).* Use 
-0000d210: 6f66 2060 6043 5472 6169 742e 6465 6661  of ``CTrait.defa
-0000d220: 756c 745f 7661 6c75 6560 6020 666f 7220  ult_value`` for 
-0000d230: 7365 7474 696e 6720 6465 6661 756c 7420  setting default 
-0000d240: 7661 6c75 6520 696e 666f 726d 6174 696f  value informatio
-0000d250: 6e20 6973 0a20 2064 6570 7265 6361 7465  n is.  deprecate
-0000d260: 642e 2055 7365 2060 6043 5472 6169 742e  d. Use ``CTrait.
-0000d270: 7365 745f 6465 6661 756c 745f 7661 6c75  set_default_valu
-0000d280: 6560 6020 696e 7374 6561 642e 2028 2336  e`` instead. (#6
-0000d290: 3230 290a 2a20 5573 6520 6f66 2074 6865  20).* Use of the
-0000d2a0: 2060 6072 6963 685f 636f 6d70 6172 6560   ``rich_compare`
-0000d2b0: 6020 7472 6169 7420 6d65 7461 6461 7461  ` trait metadata
-0000d2c0: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-0000d2d0: 5573 6520 7468 650a 2020 6060 636f 6d70  Use the.  ``comp
-0000d2e0: 6172 6973 6f6e 5f6d 6f64 6560 6020 6d65  arison_mode`` me
-0000d2f0: 7461 6461 7461 2069 6e73 7465 6164 2e20  tadata instead. 
-0000d300: 2823 3539 3829 0a0a 5265 6d6f 7661 6c73  (#598)..Removals
-0000d310: 0a7e 7e7e 7e7e 7e7e 7e0a 0a2a 2050 7974  .~~~~~~~~..* Pyt
-0000d320: 686f 6e20 3220 636f 6d70 6174 6962 696c  hon 2 compatibil
-0000d330: 6974 7920 7375 7070 6f72 7420 636f 6465  ity support code
-0000d340: 2068 6173 2062 6565 6e20 7265 6d6f 7665   has been remove
-0000d350: 642e 2028 2336 3338 2c20 2336 3434 290a  d. (#638, #644).
-0000d360: 2a20 5472 6169 7473 2063 6174 6567 6f72  * Traits categor
-0000d370: 6965 7320 6861 7665 2062 6565 6e20 7265  ies have been re
-0000d380: 6d6f 7665 642e 2028 2335 3638 290a 2a20  moved. (#568).* 
-0000d390: 5468 6520 666f 6c6c 6f77 696e 6720 7472  The following tr
-0000d3a0: 6169 7420 6861 6e64 6c65 7273 2068 6176  ait handlers hav
-0000d3b0: 6520 6265 656e 2072 656d 6f76 6564 3a20  e been removed: 
-0000d3c0: 6060 5468 6973 436c 6173 7360 602c 0a20  ``ThisClass``,. 
-0000d3d0: 2060 6054 7261 6974 436c 6173 7360 602c   ``TraitClass``,
-0000d3e0: 2060 6054 7261 6974 4578 7072 6573 7369   ``TraitExpressi
-0000d3f0: 6f6e 6060 2c20 6060 5472 6169 7443 616c  on``, ``TraitCal
-0000d400: 6c61 626c 6560 602c 2060 6054 7261 6974  lable``, ``Trait
-0000d410: 5374 7269 6e67 6060 2c0a 2020 6060 5472  String``,.  ``Tr
-0000d420: 6169 7452 616e 6765 6060 2c20 6060 5472  aitRange``, ``Tr
-0000d430: 6169 7457 6561 6b52 6566 6060 2e20 2823  aitWeakRef``. (#
-0000d440: 3738 322c 2023 3731 312c 2023 3639 392c  782, #711, #699,
-0000d450: 2023 3639 382c 2023 3632 352c 2023 3539   #698, #625, #59
-0000d460: 332c 2023 3538 372c 0a20 2023 3634 3029  3, #587,.  #640)
-0000d470: 0a2a 2060 6043 5472 6169 742e 7269 6368  .* ``CTrait.rich
-0000d480: 5f63 6f6d 7061 7265 6060 2068 6173 2062  _compare`` has b
-0000d490: 6565 6e20 7265 6d6f 7665 642e 2028 2335  een removed. (#5
-0000d4a0: 3938 290a 2a20 5468 6520 6060 6354 7261  98).* The ``cTra
-0000d4b0: 6974 2e63 6173 7460 6020 6d65 7468 6f64  it.cast`` method
-0000d4c0: 2068 6173 2062 6565 6e20 7265 6d6f 7665   has been remove
-0000d4d0: 642e 2028 2336 3633 290a 2a20 5468 6520  d. (#663).* The 
-0000d4e0: 6d61 6769 6361 6c20 6060 5472 6169 7456  magical ``TraitV
-0000d4f0: 616c 7565 6060 2061 6e64 2061 7373 6f63  alue`` and assoc
-0000d500: 6961 7465 6420 6d61 6368 696e 6572 7920  iated machinery 
-0000d510: 6861 7665 2062 6565 6e20 7265 6d6f 7665  have been remove
-0000d520: 642e 2028 2336 3538 290a 2a20 5468 6520  d. (#658).* The 
-0000d530: 6060 4765 6e65 7269 6360 6020 7472 6169  ``Generic`` trai
-0000d540: 7420 7479 7065 2068 6173 2062 6565 6e20  t type has been 
-0000d550: 7265 6d6f 7665 642e 2028 2336 3537 290a  removed. (#657).
-0000d560: 2a20 5468 6520 6060 5553 7472 6060 2074  * The ``UStr`` t
-0000d570: 7261 6974 2074 7970 6520 616e 6420 6060  rait type and ``
-0000d580: 4861 7355 6e69 7175 6553 7472 696e 6773  HasUniqueStrings
-0000d590: 6060 2063 6c61 7373 2068 6176 6520 6265  `` class have be
-0000d5a0: 656e 2072 656d 6f76 6564 2e0a 2020 2823  en removed..  (#
-0000d5b0: 3635 3429 0a2a 2054 6865 2060 6073 7472  654).* The ``str
-0000d5c0: 5f66 696e 6460 6020 616e 6420 6060 7374  _find`` and ``st
-0000d5d0: 725f 7266 696e 6460 6020 6865 6c70 6572  r_rfind`` helper
-0000d5e0: 2066 756e 6374 696f 6e73 2068 6176 6520   functions have 
-0000d5f0: 6265 656e 2072 656d 6f76 6564 2e20 2823  been removed. (#
-0000d600: 3633 3329 0a2a 2054 6865 2067 6c6f 6261  633).* The globa
-0000d610: 6c20 6060 5f74 7261 6974 5f6e 6f74 6966  l ``_trait_notif
-0000d620: 6963 6174 696f 6e5f 6861 6e64 6c65 7260  ication_handler`
-0000d630: 6020 6861 7320 6265 656e 2072 656d 6f76  ` has been remov
-0000d640: 6564 2e20 2823 3631 3929 0a2a 2060 6042  ed. (#619).* ``B
-0000d650: 6173 6554 7261 6974 4861 6e64 6c65 722e  aseTraitHandler.
-0000d660: 7265 7072 6060 2068 6173 2062 6565 6e20  repr`` has been 
-0000d670: 7265 6d6f 7665 642e 2028 2335 3939 290a  removed. (#599).
-0000d680: 2a20 6060 4861 7354 7261 6974 732e 7472  * ``HasTraits.tr
-0000d690: 6169 745f 6d6f 6e69 746f 7260 6020 7761  ait_monitor`` wa
-0000d6a0: 7320 756e 646f 6375 6d65 6e74 6564 2c20  s undocumented, 
-0000d6b0: 756e 7465 7374 6564 2c20 616e 6420 6272  untested, and br
-0000d6c0: 6f6b 656e 2c20 616e 640a 2020 6861 7320  oken, and.  has 
-0000d6d0: 6265 656e 2072 656d 6f76 6564 2e20 2823  been removed. (#
-0000d6e0: 3537 3029 0a2a 2054 6865 2060 6054 7261  570).* The ``Tra
-0000d6f0: 6974 496e 7374 616e 6365 6060 2074 7261  itInstance`` tra
-0000d700: 6974 2068 616e 646c 6572 2028 6e6f 7420  it handler (not 
-0000d710: 746f 2062 6520 636f 6e66 7573 6564 0a20  to be confused. 
-0000d720: 2077 6974 6820 7468 6520 6060 496e 7374   with the ``Inst
-0000d730: 616e 6365 6060 2074 7261 6974 2074 7970  ance`` trait typ
-0000d740: 6529 206e 6f20 6c6f 6e67 6572 2073 7570  e) no longer sup
-0000d750: 706f 7274 7320 6164 6170 7461 7469 6f6e  ports adaptation
-0000d760: 2e20 2823 3634 3129 0a2a 2054 6865 2060  . (#641).* The `
-0000d770: 6044 796e 616d 6963 5669 6577 6060 2061  `DynamicView`` a
-0000d780: 6e64 2060 6048 6173 4479 6e61 6d69 6356  nd ``HasDynamicV
-0000d790: 6965 7773 6060 2063 6c61 7373 6573 2068  iews`` classes h
-0000d7a0: 6176 6520 6265 656e 2072 656d 6f76 6564  ave been removed
-0000d7b0: 0a20 2066 726f 6d20 5472 6169 7473 2061  .  from Traits a
-0000d7c0: 6e64 206d 6f76 6564 2074 6f20 5472 6169  nd moved to Trai
-0000d7d0: 7473 5549 2069 6e73 7465 6164 2e20 2823  tsUI instead. (#
-0000d7e0: 3630 3929 0a2a 2060 6044 6963 7453 7472  609).* ``DictStr
-0000d7f0: 4c6f 6e67 6060 2068 6173 2062 6565 6e20  Long`` has been 
-0000d800: 7265 6d6f 7665 642e 2028 2335 3733 290a  removed. (#573).
-0000d810: 0a54 6573 7420 7375 6974 650a 7e7e 7e7e  .Test suite.~~~~
-0000d820: 7e7e 7e7e 7e7e 0a0a 2a20 4669 7820 7661  ~~~~~~..* Fix va
-0000d830: 7269 6f75 7320 7465 7374 7320 746f 2062  rious tests to b
-0000d840: 6520 7265 7065 6174 6162 6c65 2e20 2823  e repeatable. (#
-0000d850: 3830 322c 2023 3732 3929 0a2a 2046 6978  802, #729).* Fix
-0000d860: 2064 6570 7265 6361 7469 6f6e 2077 6172   deprecation war
-0000d870: 6e69 6e67 7320 696e 2074 6865 2074 6573  nings in the tes
-0000d880: 7420 7375 6974 6520 6f75 7470 7574 2e20  t suite output. 
-0000d890: 2823 3832 302c 2023 3830 342c 2023 3731  (#820, #804, #71
-0000d8a0: 3629 0a2a 2041 6464 206d 6163 6869 6e65  6).* Add machine
-0000d8b0: 7279 2066 6f72 2074 6573 7469 6e67 2075  ry for testing u
-0000d8c0: 6e70 6963 6b6c 696e 6720 6f66 2068 6973  npickling of his
-0000d8d0: 746f 7269 6361 6c20 7069 636b 6c65 732e  torical pickles.
-0000d8e0: 2028 2337 3837 290a 2a20 5265 6d6f 7665   (#787).* Remove
-0000d8f0: 2070 7269 6e74 2073 7461 7465 6d65 6e74   print statement
-0000d900: 7320 6672 6f6d 2074 6573 7420 7375 6974  s from test suit
-0000d910: 652e 2028 2337 3532 2c20 2337 3638 290a  e. (#752, #768).
-0000d920: 2a20 4669 7820 6120 7465 7374 2074 6f20  * Fix a test to 
-0000d930: 636c 6561 6e20 7570 2074 6865 2074 6872  clean up the thr
-0000d940: 6561 6473 2069 7420 6372 6561 7465 732e  eads it creates.
-0000d950: 2028 2337 3331 290a 2a20 4164 6420 7465   (#731).* Add te
-0000d960: 7374 7320 666f 7220 6578 7465 6e64 6564  sts for extended
-0000d970: 2074 7261 6974 2063 6861 6e67 6520 6973   trait change is
-0000d980: 7375 6573 2023 3533 3720 616e 6420 2335  sues #537 and #5
-0000d990: 3338 2028 2335 3433 290a 2a20 4f74 6865  38 (#543).* Othe
-0000d9a0: 7220 6d69 6e6f 7220 7465 7374 2066 6978  r minor test fix
-0000d9b0: 6573 2e20 2823 3730 302c 2023 3832 3129  es. (#700, #821)
-0000d9c0: 0a0a 446f 6375 6d65 6e74 6174 696f 6e0a  ..Documentation.
-0000d9d0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a  ~~~~~~~~~~~~~..*
-0000d9e0: 2049 6d70 726f 7665 2064 6f63 756d 656e   Improve documen
-0000d9f0: 7461 7469 6f6e 206f 6620 7472 6169 7420  tation of trait 
-0000da00: 636f 6e74 6169 6e65 7220 6f62 6a65 6374  container object
-0000da10: 732e 2028 2338 3130 290a 2a20 496d 7072  s. (#810).* Impr
-0000da20: 6f76 6520 646f 6375 6d65 6e74 6174 696f  ove documentatio
-0000da30: 6e20 666f 7220 7468 6520 6060 7472 6169  n for the ``trai
-0000da40: 7473 2e63 7472 6169 7473 6060 206d 6f64  ts.ctraits`` mod
-0000da50: 756c 652e 2028 2338 3236 2c20 2338 3234  ule. (#826, #824
-0000da60: 2c0a 2020 2336 3539 2c20 2336 3533 2c20  ,.  #659, #653, 
-0000da70: 2338 3239 2c20 2338 3336 290a 2a20 4669  #829, #836).* Fi
-0000da80: 7820 6261 646c 7920 666f 726d 6174 7465  x badly formatte
-0000da90: 6420 6060 5472 6169 7448 616e 646c 6572  d ``TraitHandler
-0000daa0: 6060 2064 6f63 756d 656e 7461 7469 6f6e  `` documentation
-0000dab0: 2e20 2823 3831 3729 0a2a 2046 6978 2061  . (#817).* Fix a
-0000dac0: 6e64 2069 6d70 726f 7665 2062 6164 6c79  nd improve badly
-0000dad0: 2066 6f72 6d61 7474 6564 2074 7261 6974   formatted trait
-0000dae0: 2074 7970 6573 2064 6f63 756d 656e 7461   types documenta
-0000daf0: 7469 6f6e 2e20 2823 3834 3329 0a2a 2046  tion. (#843).* F
-0000db00: 6978 2062 726f 6b65 6e20 6d6f 6475 6c65  ix broken module
-0000db10: 206c 696e 6b73 2069 6e20 7365 6374 696f   links in sectio
-0000db20: 6e20 7469 746c 6573 2069 6e20 4150 4920  n titles in API 
-0000db30: 646f 6375 6d65 6e74 6174 696f 6e2e 2028  documentation. (
-0000db40: 2338 3233 290a 2a20 4164 6469 7469 6f6e  #823).* Addition
-0000db50: 616c 2063 6c61 7373 2064 6f63 7374 7269  al class docstri
-0000db60: 6e67 2066 6978 6573 2e20 2823 3835 3429  ng fixes. (#854)
-0000db70: 0a2a 2041 6464 2063 6861 6e67 656c 6f67  .* Add changelog
-0000db80: 2074 6f20 6275 696c 7420 646f 6375 6d65   to built docume
-0000db90: 6e74 6174 696f 6e2c 2061 6e64 2061 6273  ntation, and abs
-0000dba0: 6f72 6220 6f6c 6420 6368 616e 6765 6c6f  orb old changelo
-0000dbb0: 6720 696e 746f 0a20 2074 6865 206e 6577  g into.  the new
-0000dbc0: 206f 6e65 2e20 2823 3830 302c 2023 3739   one. (#800, #79
-0000dbd0: 3929 0a2a 2052 656d 6f76 6520 6465 7072  9).* Remove depr
-0000dbe0: 6563 6174 6564 2074 7261 6974 7320 6672  ecated traits fr
-0000dbf0: 6f6d 2074 6865 2075 7365 7220 6d61 6e75  om the user manu
-0000dc00: 616c 2e20 2823 3635 3629 0a2a 2046 6978  al. (#656).* Fix
-0000dc10: 2076 6172 696f 7573 2053 7068 696e 7820   various Sphinx 
-0000dc20: 7761 726e 696e 6773 2028 2337 3137 290a  warnings (#717).
-0000dc30: 2a20 5573 6520 5356 4720 6261 6467 6573  * Use SVG badges
-0000dc40: 2069 6e20 5245 4144 4d45 2028 2335 3637   in README (#567
-0000dc50: 290a 0a42 7569 6c64 2061 6e64 2063 6f6e  )..Build and con
-0000dc60: 7469 6e75 6f75 7320 696e 7465 6772 6174  tinuous integrat
-0000dc70: 696f 6e0a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ion.~~~~~~~~~~~~
-0000dc80: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-0000dc90: 7e7e 7e7e 0a0a 2a20 456e 6162 6c65 2043  ~~~~..* Enable C
-0000dca0: 2061 7373 6572 7473 2069 6e20 5472 6176   asserts in Trav
-0000dcb0: 6973 2043 4920 7275 6e73 2e20 2823 3739  is CI runs. (#79
-0000dcc0: 3129 0a2a 2041 626f 7274 2043 4920 6f6e  1).* Abort CI on
-0000dcd0: 2063 6f6d 7069 6c65 7220 7761 726e 696e   compiler warnin
-0000dce0: 6773 2069 6e20 5472 6176 6973 2043 4920  gs in Travis CI 
-0000dcf0: 7275 6e73 2e20 2823 3736 3929 0a2a 2052  runs. (#769).* R
-0000dd00: 756e 2061 2060 6066 6c61 6b65 3860 6020  un a ``flake8`` 
-0000dd10: 6368 6563 6b20 696e 2062 6f74 6820 5472  check in both Tr
-0000dd20: 6176 6973 2043 4920 616e 6420 4170 7076  avis CI and Appv
-0000dd30: 6579 6f72 2072 756e 732e 2028 2337 3533  eyor runs. (#753
-0000dd40: 2c20 2337 3632 290a 2a20 4368 6563 6b69  , #762).* Checki
-0000dd50: 6e67 2063 6f70 7972 6967 6874 2073 7461  ng copyright sta
-0000dd60: 7465 6d65 6e74 7320 696e 2050 7974 686f  tements in Pytho
-0000dd70: 6e20 6669 6c65 7320 6173 2070 6172 7420  n files as part 
-0000dd80: 6f66 2043 4920 7275 6e73 2e20 2823 3734  of CI runs. (#74
-0000dd90: 3929 0a2a 2054 7572 6e20 7761 726e 696e  9).* Turn warnin
-0000dda0: 6773 2069 6e74 6f20 6572 726f 7273 2077  gs into errors w
-0000ddb0: 6865 6e20 6275 696c 6469 6e67 2064 6f63  hen building doc
-0000ddc0: 756d 656e 7461 7469 6f6e 2069 6e20 4349  umentation in CI
-0000ddd0: 2e20 2823 3734 3429 0a2a 2041 6464 2060  . (#744).* Add `
-0000dde0: 6067 6e75 7265 6164 6c69 6e65 6060 2061  `gnureadline`` a
-0000ddf0: 7320 6120 6465 7665 6c6f 706d 656e 7420  s a development 
-0000de00: 6465 7065 6e64 656e 6379 206f 6e20 6d61  dependency on ma
-0000de10: 634f 5320 616e 6420 4c69 6e75 782e 2028  cOS and Linux. (
-0000de20: 2336 3037 290a 2a20 4164 6420 616e 2060  #607).* Add an `
-0000de30: 6065 7473 746f 6f6c 2e70 7960 6020 6f70  `etstool.py`` op
-0000de40: 7469 6f6e 2074 6f20 7275 6e20 7465 7374  tion to run test
-0000de50: 7320 7175 6965 746c 792e 2028 2336 3036  s quietly. (#606
-0000de60: 290a 2a20 456e 6162 6c65 2074 6865 2063  ).* Enable the c
-0000de70: 6f76 6572 6167 6520 6578 7465 6e73 696f  overage extensio
-0000de80: 6e20 666f 7220 7468 6520 646f 6375 6d65  n for the docume
-0000de90: 6e74 6174 696f 6e20 6275 696c 642e 2028  ntation build. (
-0000dea0: 2338 3037 290a 2a20 5265 6d6f 7665 206d  #807).* Remove m
-0000deb0: 6f63 6b69 6e67 2069 6e20 646f 6375 6d65  ocking in docume
-0000dec0: 6e74 6174 696f 6e20 636f 6e66 6967 7572  ntation configur
-0000ded0: 6174 696f 6e2c 2061 6e64 2066 6978 2061  ation, and fix a
-0000dee0: 2064 6570 7265 6361 7465 640a 2020 636f   deprecated.  co
-0000def0: 6e66 6967 7572 6174 696f 6e20 6f70 7469  nfiguration opti
-0000df00: 6f6e 2e20 2823 3639 3629 0a0a 4d61 696e  on. (#696)..Main
-0000df10: 7465 6e61 6e63 6520 616e 6420 636f 6465  tenance and code
-0000df20: 206f 7267 616e 697a 6174 696f 6e0a 7e7e   organization.~~
-0000df30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-0000df40: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
-0000df50: 0a54 6869 7320 7265 6c65 6173 6520 696e  .This release in
-0000df60: 636c 7564 6573 2061 206c 6f74 206f 6620  cludes a lot of 
-0000df70: 7265 6661 6374 6f72 696e 6720 616e 6420  refactoring and 
-0000df80: 6d61 6e79 206d 696e 6f72 2069 6d70 726f  many minor impro
-0000df90: 7665 6d65 6e74 730a 7468 6174 2077 696c  vements.that wil
-0000dfa0: 6c20 7072 696d 6172 696c 7920 6265 6e65  l primarily bene
-0000dfb0: 6669 7420 7468 6f73 6520 776f 726b 696e  fit those workin
-0000dfc0: 6720 7769 7468 2074 6865 2054 7261 6974  g with the Trait
-0000dfd0: 7320 636f 6465 6261 7365 2e20 5468 6573  s codebase. Thes
-0000dfe0: 650a 6368 616e 6765 7320 7368 6f75 6c64  e.changes should
-0000dff0: 206e 6f74 2061 6666 6563 7420 7573 6572   not affect user
-0000e000: 2d76 6973 6962 6c65 2066 756e 6374 696f  -visible functio
-0000e010: 6e61 6c69 7479 2e20 4865 7265 2773 2061  nality. Here's a
-0000e020: 2073 756d 6d61 7279 0a6f 6620 7468 6520   summary.of the 
-0000e030: 6d6f 7265 2073 6967 6e69 6669 6361 6e74  more significant
-0000e040: 2063 6861 6e67 6573 2e0a 0a2a 2041 206d   changes...* A m
-0000e050: 616a 6f72 2072 6566 6163 746f 7220 6861  ajor refactor ha
-0000e060: 7320 7265 6d6f 7665 6420 6d6f 7374 206f  s removed most o
-0000e070: 6620 7468 6520 6369 7263 756c 6172 2064  f the circular d
-0000e080: 6570 656e 6465 6e63 6965 7320 6265 7477  ependencies betw
-0000e090: 6565 6e0a 2020 6d6f 6475 6c65 732e 2028  een.  modules. (
-0000e0a0: 2337 3330 290a 2a20 5468 6520 636f 6465  #730).* The code
-0000e0b0: 6261 7365 2069 7320 6e6f 7720 6d6f 7374  base is now most
-0000e0c0: 6c79 2060 6066 6c61 6b65 3860 6020 636c  ly ``flake8`` cl
-0000e0d0: 6561 6e2e 2028 2337 3836 2c20 2337 3533  ean. (#786, #753
-0000e0e0: 2c20 2337 3437 2c20 2337 3438 2c20 2337  , #747, #748, #7
-0000e0f0: 3436 2c0a 2020 2335 3935 290a 2a20 436f  46,.  #595).* Co
-0000e100: 7079 7269 6768 7420 6865 6164 6572 7320  pyright headers 
-0000e110: 6861 7665 2062 6565 6e20 6d61 6465 2063  have been made c
-0000e120: 6f6e 7369 7374 656e 7420 666f 7220 616c  onsistent for al
-0000e130: 6c20 5079 7468 6f6e 2066 696c 6573 2e20  l Python files. 
-0000e140: 2823 3735 3429 0a2a 2060 6063 7472 6169  (#754).* ``ctrai
-0000e150: 7473 2e63 6060 2068 6173 2062 6565 6e20  ts.c`` has been 
-0000e160: 7275 6e20 7468 726f 7567 6820 6060 636c  run through ``cl
-0000e170: 616e 672d 7469 6479 6060 2061 6e64 2060  ang-tidy`` and `
-0000e180: 6063 6c61 6e67 2d66 6f72 6d61 7460 6020  `clang-format`` 
-0000e190: 696e 0a20 206f 7264 6572 2074 6f20 6272  in.  order to br
-0000e1a0: 696e 6720 6974 2063 6c6f 7365 7220 746f  ing it closer to
-0000e1b0: 2050 4550 2037 2073 7479 6c65 2e20 2823   PEP 7 style. (#
-0000e1c0: 3731 3529 0a2a 2045 6469 746f 7220 6661  715).* Editor fa
-0000e1d0: 6374 6f72 6965 7320 6861 7665 2062 6565  ctories have bee
-0000e1e0: 6e20 6d6f 7665 6420 696e 746f 2061 206e  n moved into a n
-0000e1f0: 6577 2060 6074 7261 6974 732e 6564 6974  ew ``traits.edit
-0000e200: 6f72 5f66 6163 746f 7269 6573 6060 0a20  or_factories``. 
-0000e210: 206d 6f64 756c 652c 2074 6f20 6865 6c70   module, to help
-0000e220: 2063 6f6d 7061 7274 6d65 6e74 616c 697a   compartmentaliz
-0000e230: 6520 636f 6465 2064 6570 656e 6465 6e63  e code dependenc
-0000e240: 6965 7320 6f6e 2054 7261 6974 7355 492e  ies on TraitsUI.
-0000e250: 2028 2336 3631 290a 2a20 5472 6169 7420   (#661).* Trait 
-0000e260: 636f 6e74 6169 6e65 7220 6f62 6a65 6374  container object
-0000e270: 2063 6c61 7373 6573 2028 6060 5472 6169   classes (``Trai
-0000e280: 7444 6963 744f 626a 6563 7460 602c 2060  tDictObject``, `
-0000e290: 6054 7261 6974 4c69 7374 4f62 6a65 6374  `TraitListObject
-0000e2a0: 6060 2c0a 2020 6060 5472 6169 7453 6574  ``,.  ``TraitSet
-0000e2b0: 4f62 6a65 6374 6060 2920 6861 7665 2065  Object``) have e
-0000e2c0: 6163 6820 6265 656e 206d 6f76 6564 2069  ach been moved i
-0000e2d0: 6e74 6f20 7468 6569 7220 6f77 6e20 6d6f  nto their own mo
-0000e2e0: 6475 6c65 2c20 616c 6f6e 670a 2020 7769  dule, along.  wi
-0000e2f0: 7468 2074 6865 6972 2061 7373 6f63 6961  th their associa
-0000e300: 7465 6420 6576 656e 7420 7479 7065 2e20  ted event type. 
-0000e310: 2823 3637 3729 0a2a 204d 6973 6365 6c6c  (#677).* Miscell
-0000e320: 616e 656f 7573 206f 7468 6572 206d 696e  aneous other min
-0000e330: 6f72 2066 6978 6573 2c20 7265 6661 6374  or fixes, refact
-0000e340: 6f72 696e 6773 2061 6e64 2063 6c65 616e  orings and clean
-0000e350: 7570 732e 0a20 2028 2337 3835 2c20 2337  ups..  (#785, #7
-0000e360: 3737 2c20 2337 3530 2c20 2337 3236 2c20  77, #750, #726, 
-0000e370: 2337 3134 2c20 2337 3132 2c20 2337 3038  #714, #712, #708
-0000e380: 2c20 2337 3031 2c20 2336 3832 2c20 2336  , #701, #682, #6
-0000e390: 3635 2c20 2336 3531 2c0a 2020 2336 3532  65, #651,.  #652
-0000e3a0: 2c20 2336 3339 2c20 2336 3336 2c20 2336  , #639, #636, #6
-0000e3b0: 3334 2c20 2336 3236 2c20 2336 3332 2c20  34, #626, #632, 
-0000e3c0: 2336 3131 2c20 2336 3133 2c20 2336 3132  #611, #613, #612
-0000e3d0: 2c20 2336 3035 2c20 2336 3033 2c0a 2020  , #605, #603,.  
-0000e3e0: 2336 3030 2c20 2335 3937 2c20 2335 3836  #600, #597, #586
-0000e3f0: 2c20 2335 3835 2c20 2335 3834 2c20 2335  , #585, #584, #5
-0000e400: 3830 2c20 2335 3737 2c20 2335 3738 2c20  80, #577, #578, 
-0000e410: 2335 3634 2c20 2338 3036 290a 0a0a 5265  #564, #806)...Re
-0000e420: 6c65 6173 6520 352e 322e 300a 2d2d 2d2d  lease 5.2.0.----
-0000e430: 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561  ---------..Relea
-0000e440: 7365 643a 2032 3031 392d 3131 2d31 380a  sed: 2019-11-18.
-0000e450: 0a45 6e68 616e 6365 6d65 6e74 730a 0a2a  .Enhancements..*
-0000e460: 2053 7570 706f 7274 2069 6e73 7461 6c6c   Support install
-0000e470: 6174 696f 6e20 6672 6f6d 2073 6f75 7263  ation from sourc
-0000e480: 6520 6172 6368 6976 6573 2e20 2823 3532  e archives. (#52
-0000e490: 3829 0a0a 4669 7865 730a 0a2a 2045 6e73  8)..Fixes..* Ens
-0000e4a0: 7572 6520 6060 5472 6169 744c 6973 7445  ure ``TraitListE
-0000e4b0: 7665 6e74 2e69 6e64 6578 6060 2069 7320  vent.index`` is 
-0000e4c0: 616c 7761 7973 2061 6e20 696e 7465 6765  always an intege
-0000e4d0: 722e 2028 2335 3438 290a 2a20 5570 6461  r. (#548).* Upda
-0000e4e0: 7465 2074 6865 2064 6570 7265 6361 7465  te the deprecate
-0000e4f0: 6420 6060 636f 6c6c 6563 7469 6f6e 732e  d ``collections.
-0000e500: 4d75 7461 626c 654d 6170 7069 6e67 6060  MutableMapping``
-0000e510: 2069 6d70 6f72 742e 2028 2335 3330 290a   import. (#530).
-0000e520: 2a20 4669 7820 696e 6164 7665 7274 656e  * Fix inadverten
-0000e530: 7420 6d6f 6469 6669 6361 7469 6f6e 206f  t modification o
-0000e540: 6620 7468 6520 6060 4361 7465 676f 7279  f the ``Category
-0000e550: 6060 2062 6173 6520 636c 6173 732e 2028  `` base class. (
-0000e560: 2335 3039 290a 2a20 5265 776f 726b 2076  #509).* Rework v
-0000e570: 6572 7369 6f6e 2068 616e 646c 696e 6720  ersion handling 
-0000e580: 696e 2060 6073 6574 7570 2e70 7960 602e  in ``setup.py``.
-0000e590: 2028 2335 3135 290a 2a20 446f 6e27 7420   (#515).* Don't 
-0000e5a0: 6175 746f 6765 6e65 7261 7465 2064 6f63  autogenerate doc
-0000e5b0: 756d 656e 7461 7469 6f6e 2066 6f72 2060  umentation for `
-0000e5c0: 6056 6965 7745 6c65 6d65 6e74 6060 2e20  `ViewElement``. 
-0000e5d0: 2823 3535 3929 0a2a 2045 6e73 7572 6520  (#559).* Ensure 
-0000e5e0: 7468 6174 2061 6c6c 2074 6573 7473 2061  that all tests a
-0000e5f0: 7265 2060 6075 6e69 7474 6573 7460 6020  re ``unittest`` 
-0000e600: 636f 6d70 6174 6962 6c65 2e20 2823 3535  compatible. (#55
-0000e610: 3129 0a0a 4368 616e 6765 730a 0a2a 2052  1)..Changes..* R
-0000e620: 6570 6c61 6365 206f 6363 7572 656e 6365  eplace occurence
-0000e630: 7320 6f66 2064 6570 7265 6361 7465 6420  s of deprecated 
-0000e640: 6060 4164 6170 7473 546f 6060 2077 6974  ``AdaptsTo`` wit
-0000e650: 6820 6060 5375 7070 6f72 7473 6060 2e20  h ``Supports``. 
-0000e660: 2823 3533 3229 0a2a 2052 656d 6f76 6520  (#532).* Remove 
-0000e670: 6060 436c 6173 7360 6020 7472 6169 742e  ``Class`` trait.
-0000e680: 2028 2335 3230 290a 2a20 4465 7072 6563   (#520).* Deprec
-0000e690: 6174 6520 6060 4361 7465 676f 7279 6060  ate ``Category``
-0000e6a0: 2074 7261 6974 2e20 2823 3531 3029 0a2a   trait. (#510).*
-0000e6b0: 2046 6978 2074 7970 6f73 2069 6e20 646f   Fix typos in do
-0000e6c0: 6373 7472 696e 6773 2e20 2823 3530 3229  cstrings. (#502)
-0000e6d0: 0a2a 2055 7365 2064 6563 6f72 6174 6f72  .* Use decorator
-0000e6e0: 2066 6f72 6d20 6f66 2060 6063 6c61 7373   form of ``class
-0000e6f0: 6d65 7468 6f64 6060 2e20 2823 3530 3029  method``. (#500)
-0000e700: 0a2a 2052 656d 6f76 6520 7265 6465 6669  .* Remove redefi
-0000e710: 6e69 7469 6f6e 206f 6620 6060 4e75 6c6c  nition of ``Null
-0000e720: 4861 6e64 6c65 7260 602e 2028 2335 3138  Handler``. (#518
-0000e730: 290a 2a20 4164 6420 616e 2069 6d70 6f72  ).* Add an impor
-0000e740: 7420 6368 6563 6b20 6865 6c70 6572 2e20  t check helper. 
-0000e750: 2823 3532 3129 0a2a 2043 6c65 616e 2075  (#521).* Clean u
-0000e760: 7020 4379 7468 6f6e 2074 6573 7473 2e20  p Cython tests. 
-0000e770: 2823 3535 3529 0a2a 2043 6c65 616e 2075  (#555).* Clean u
-0000e780: 7020 7465 7374 206f 7574 7075 742e 2028  p test output. (
-0000e790: 2335 3533 290a 0a4d 6973 6365 6c6c 616e  #553)..Miscellan
-0000e7a0: 656f 7573 0a0a 2a20 5570 6461 7465 2045  eous..* Update E
-0000e7b0: 444d 2076 6572 7369 6f6e 206f 6e20 4349  DM version on CI
-0000e7c0: 2074 6f20 7665 7273 696f 6e20 322e 302e   to version 2.0.
-0000e7d0: 302e 2028 2335 3630 290a 2a20 446f 6e27  0. (#560).* Don'
-0000e7e0: 7420 6669 6e69 7368 2066 6173 7420 6f6e  t finish fast on
-0000e7f0: 2043 492e 2028 2335 3536 290a 2a20 5573   CI. (#556).* Us
-0000e800: 6520 6060 756e 6974 7465 7374 6060 2074  e ``unittest`` t
-0000e810: 6f20 7275 6e20 7465 7374 7320 696e 2043  o run tests in C
-0000e820: 492e 2028 2335 3532 290a 2a20 4c6f 772d  I. (#552).* Low-
-0000e830: 6c65 7665 6c20 6669 7865 7320 616e 6420  level fixes and 
-0000e840: 7374 796c 6520 636c 6561 6e75 7020 696e  style cleanup in
-0000e850: 2060 6065 7473 746f 6f6c 2e70 7960 602e   ``etstool.py``.
-0000e860: 2028 2335 3530 290a 2a20 4164 6420 6060   (#550).* Add ``
-0000e870: 2d2d 6564 6974 6162 6c65 6060 206f 7074  --editable`` opt
-0000e880: 696f 6e20 666f 7220 6060 696e 7374 616c  ion for ``instal
-0000e890: 6c60 602c 2060 6075 7064 6174 6560 6020  l``, ``update`` 
-0000e8a0: 4349 2063 6f6d 6d61 6e64 732e 2028 2335  CI commands. (#5
-0000e8b0: 3436 290a 2a20 4d61 6b65 2067 6974 2063  46).* Make git c
-0000e8c0: 6f6d 6d69 7420 6861 7368 2061 7661 696c  ommit hash avail
-0000e8d0: 6162 6c65 2074 6f20 6172 6368 6976 6573  able to archives
-0000e8e0: 2e20 2823 3532 3629 0a2a 2046 6978 2075  . (#526).* Fix u
-0000e8f0: 7365 206f 6620 6e6f 6e2d 6564 6d20 656e  se of non-edm en
-0000e900: 7673 2061 7320 626f 6f74 7374 7261 7020  vs as bootstrap 
-0000e910: 656e 7673 206f 6e20 5769 6e64 6f77 732e  envs on Windows.
-0000e920: 2028 2335 3132 290a 2a20 5265 6d6f 7665   (#512).* Remove
-0000e930: 2065 646d 2069 6e73 7461 6c6c 6564 2070   edm installed p
-0000e940: 6163 6b61 6765 2062 6566 6f72 6520 696e  ackage before in
-0000e950: 7374 616c 6c69 6e67 2066 726f 6d20 736f  stalling from so
-0000e960: 7572 6365 2e20 2823 3531 3629 0a2a 2041  urce. (#516).* A
-0000e970: 6464 2068 656c 7020 7465 7874 2074 6f20  dd help text to 
-0000e980: 636c 6963 6b20 6f70 7469 6f6e 732e 2028  click options. (
-0000e990: 2335 3134 290a 2a20 5661 7269 6f75 7320  #514).* Various 
-0000e9a0: 636c 6561 6e75 7073 2c20 6669 7865 7320  cleanups, fixes 
-0000e9b0: 616e 6420 656e 6861 6e63 656d 656e 7473  and enhancements
-0000e9c0: 2069 6e20 6060 6574 7374 6f6f 6c2e 7079   in ``etstool.py
-0000e9d0: 6060 2e20 2823 3531 3129 0a0a 0a52 656c  ``. (#511)...Rel
-0000e9e0: 6561 7365 2035 2e31 2e32 0a2d 2d2d 2d2d  ease 5.1.2.-----
-0000e9f0: 2d2d 2d2d 2d2d 2d2d 0a0a 5265 6c65 6173  --------..Releas
-0000ea00: 6564 3a20 3230 3139 2d30 372d 3038 0a0a  ed: 2019-07-08..
-0000ea10: 4669 7865 730a 0a2a 2054 7261 6974 7320  Fixes..* Traits 
-0000ea20: 646f 6375 6d65 6e74 6572 206e 6f20 6c6f  documenter no lo
-0000ea30: 6e67 6572 2067 656e 6572 6174 6573 2062  nger generates b
-0000ea40: 6164 2072 6553 5420 666f 7220 7472 6169  ad reST for trai
-0000ea50: 7473 2077 686f 7365 2064 6566 696e 6974  ts whose definit
-0000ea60: 696f 6e0a 2020 7370 616e 7320 6d75 6c74  ion.  spans mult
-0000ea70: 6970 6c65 2073 6f75 7263 6520 6c69 6e65  iple source line
-0000ea80: 732e 2028 2334 3934 290a 0a0a 5265 6c65  s. (#494)...Rele
-0000ea90: 6173 6520 352e 312e 310a 2d2d 2d2d 2d2d  ase 5.1.1.------
-0000eaa0: 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561 7365  -------..Release
-0000eab0: 643a 2032 3031 392d 3034 2d31 380a 0a46  d: 2019-04-18..F
-0000eac0: 6978 6573 0a0a 2a20 5265 7665 7274 2061  ixes..* Revert a
-0000ead0: 2063 6861 6e67 6520 2823 3434 3929 2077   change (#449) w
-0000eae0: 6869 6368 2061 6363 6964 656e 7461 6c6c  hich accidentall
-0000eaf0: 7920 6272 6f6b 6520 6578 7465 726e 616c  y broke external
-0000eb00: 2075 7365 7320 6f66 0a20 2060 605f 7079   uses of.  ``_py
-0000eb10: 3274 6f33 2e73 7472 5f66 696e 6460 6020  2to3.str_find`` 
-0000eb20: 616e 6420 6060 5f70 7932 746f 332e 7374  and ``_py2to3.st
-0000eb30: 725f 7266 696e 6460 602e 2028 2334 3732  r_rfind``. (#472
-0000eb40: 290a 0a52 656c 6561 7365 2035 2e31 2e30  )..Release 5.1.0
-0000eb50: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
-0000eb60: 5265 6c65 6173 6564 3a20 3230 3139 2d30  Released: 2019-0
-0000eb70: 342d 3135 0a0a 456e 6861 6e63 656d 656e  4-15..Enhancemen
-0000eb80: 7473 0a0a 2a20 4d61 6b65 2055 5549 4420  ts..* Make UUID 
-0000eb90: 7472 6169 7420 696e 6974 6961 6c69 7a61  trait initializa
-0000eba0: 626c 652e 2028 2334 3539 290a 2a20 4368  ble. (#459).* Ch
-0000ebb0: 616e 6765 2064 6566 6175 6c74 2060 6046  ange default ``F
-0000ebc0: 696c 6545 6469 746f 7260 6020 6265 6861  ileEditor`` beha
-0000ebd0: 7669 6f72 2066 6f72 2061 2060 6046 696c  vior for a ``Fil
-0000ebe0: 6560 6020 7472 6169 7420 6261 7365 6420  e`` trait based 
-0000ebf0: 6f6e 0a20 2077 6865 7468 6572 2060 6065  on.  whether ``e
-0000ec00: 7869 7374 733d 5472 7565 6060 2069 7320  xists=True`` is 
-0000ec10: 7370 6563 6966 6965 6420 666f 7220 7468  specified for th
-0000ec20: 6174 2074 7261 6974 2e20 2823 3435 312c  at trait. (#451,
-0000ec30: 2023 3436 3729 0a0a 4368 616e 6765 730a   #467)..Changes.
-0000ec40: 0a2a 2054 6865 2063 6861 6e67 6573 206d  .* The changes m
-0000ec50: 6164 6520 696e 2023 3337 3320 746f 206d  ade in #373 to m
-0000ec60: 616b 6520 6479 6e61 6d69 6361 6c6c 792d  ake dynamically-
-0000ec70: 6164 6465 6420 7472 6169 7473 2070 6963  added traits pic
-0000ec80: 6b6c 6561 626c 6520 6861 7665 0a20 2062  kleable have.  b
-0000ec90: 6565 6e20 7265 7665 7274 6564 2e20 2823  een reverted. (#
-0000eca0: 3436 3229 0a2a 2060 6074 7261 6974 732e  462).* ``traits.
-0000ecb0: 6170 692e 7079 7468 6f6e 5f76 6572 7369  api.python_versi
-0000ecc0: 6f6e 6060 2068 6173 2062 6565 6e20 7265  on`` has been re
-0000ecd0: 6d6f 7665 642e 2049 6e74 6572 6e61 6c73  moved. Internals
-0000ece0: 2068 6176 6520 6265 656e 0a20 2072 6566   have been.  ref
-0000ecf0: 6163 746f 7265 6420 746f 2075 7365 2060  actored to use `
-0000ed00: 6073 6978 2e50 5932 6060 2069 6e20 7072  `six.PY2`` in pr
-0000ed10: 6566 6572 656e 6365 2074 6f20 6060 7379  eference to ``sy
-0000ed20: 732e 7665 7273 696f 6e5f 696e 666f 6060  s.version_info``
-0000ed30: 2e0a 2020 2823 3434 3929 0a2a 2044 6f6e  ..  (#449).* Don
-0000ed40: 2774 2064 6570 656e 6420 6f6e 2074 6865  't depend on the
-0000ed50: 2033 7264 2070 6172 7479 2060 606d 6f63   3rd party ``moc
-0000ed60: 6b60 6020 6c69 6272 6172 7920 6f6e 2050  k`` library on P
-0000ed70: 7974 686f 6e20 333b 2075 7365 0a20 2060  ython 3; use.  `
-0000ed80: 6075 6e69 7474 6573 742e 6d6f 636b 6060  `unittest.mock``
-0000ed90: 2069 6e73 7465 6164 2e20 2823 3434 3629   instead. (#446)
-0000eda0: 0a0a 4669 7865 730a 0a2a 2046 6978 2061  ..Fixes..* Fix a
-0000edb0: 2066 7261 6769 6c65 204e 756d 5079 2d72   fragile NumPy-r
-0000edc0: 656c 6174 6564 2074 6573 7420 7468 6174  elated test that
-0000edd0: 2066 6169 6c65 6420 2860 6052 756e 7469   failed (``Runti
-0000ede0: 6d65 4572 726f 723a 2065 6d70 7479 5f6c  meError: empty_l
-0000edf0: 696b 650a 2020 6d65 7468 6f64 2061 6c72  ike.  method alr
-0000ee00: 6561 6479 2068 6173 2061 2064 6f63 7374  eady has a docst
-0000ee10: 7269 6e67 6060 2920 7769 7468 2074 6865  ring``) with the
-0000ee20: 206e 6577 6573 7420 7665 7273 696f 6e20   newest version 
-0000ee30: 6f66 204e 756d 5079 2e0a 2020 2823 3434  of NumPy..  (#44
-0000ee40: 3329 0a0a 4d69 7363 656c 6c61 6e65 6f75  3)..Miscellaneou
-0000ee50: 730a 0a2a 2060 6074 7261 6974 732e 5f76  s..* ``traits._v
-0000ee60: 6572 7369 6f6e 2e67 6974 5f72 6576 6973  ersion.git_revis
-0000ee70: 696f 6e60 6020 6e6f 7720 6769 7665 7320  ion`` now gives 
-0000ee80: 7468 6520 6675 6c6c 2063 6f6d 6d69 7420  the full commit 
-0000ee90: 6861 7368 2028 666f 7220 6c6f 6361 6c0a  hash (for local.
-0000eea0: 2020 6275 696c 6473 2920 696e 7374 6561    builds) instea
-0000eeb0: 6420 6f66 2061 6e20 6162 6272 6576 6961  d of an abbrevia
-0000eec0: 7465 6420 3720 6865 782d 6469 6769 7420  ted 7 hex-digit 
-0000eed0: 7665 7273 696f 6e2e 2028 2334 3533 290a  version. (#453).
-0000eee0: 2a20 4669 7820 636f 7079 7269 6768 7420  * Fix copyright 
-0000eef0: 7965 6172 7320 696e 2064 6f63 756d 656e  years in documen
-0000ef00: 7461 7469 6f6e 2062 7569 6c64 2e20 2823  tation build. (#
-0000ef10: 3434 3529 0a2a 2052 656e 616d 6520 6060  445).* Rename ``
-0000ef20: 5245 4144 4d45 2e74 7874 6060 2074 6f20  README.txt`` to 
-0000ef30: 6060 5245 4144 4d45 2e72 7374 6060 2c20  ``README.rst``, 
-0000ef40: 736f 2074 6861 7420 4769 7448 7562 2072  so that GitHub r
-0000ef50: 656e 6465 7273 2069 7420 6e69 6365 6c79  enders it nicely
-0000ef60: 2e0a 2a20 436f 6465 2063 6c65 616e 7570  ..* Code cleanup
-0000ef70: 733a 2072 656d 6f76 6520 2245 4f46 2220  s: remove "EOF" 
-0000ef80: 6d61 726b 6572 7320 6672 6f6d 2063 6f64  markers from cod
-0000ef90: 652e 2052 656d 6f76 6520 6060 5f5f 6d61  e. Remove ``__ma
-0000efa0: 696e 5f5f 6060 2062 6c6f 636b 730a 2020  in__`` blocks.  
-0000efb0: 666f 7220 756e 6974 2074 6573 7473 2e20  for unit tests. 
-0000efc0: 5265 6d6f 7665 2069 6d70 6f72 7473 206f  Remove imports o
-0000efd0: 6620 6060 756e 6974 7465 7374 6060 2066  f ``unittest`` f
-0000efe0: 726f 6d20 6060 756e 6974 7465 7374 5f74  rom ``unittest_t
-0000eff0: 6f6f 6c73 6060 2e0a 2020 2823 3434 382c  ools``..  (#448,
-0000f000: 2023 3434 3629 0a2a 2055 7064 6174 6520   #446).* Update 
-0000f010: 5472 6176 6973 2043 4920 616e 6420 4170  Travis CI and Ap
-0000f020: 7076 6579 6f72 2063 6f6e 6669 6775 7261  pveyor configura
-0000f030: 7469 6f6e 7320 746f 2072 756e 2074 6573  tions to run tes
-0000f040: 7473 2061 6761 696e 7374 0a20 2061 6c6c  ts against.  all
-0000f050: 2050 5220 6272 616e 6368 6573 2c20 6e6f   PR branches, no
-0000f060: 7420 6a75 7374 2050 5273 2061 6761 696e  t just PRs again
-0000f070: 7374 206d 6173 7465 722e 2028 2334 3636  st master. (#466
-0000f080: 290a 0a0a 5265 6c65 6173 6520 352e 302e  )...Release 5.0.
-0000f090: 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  0.-------------.
-0000f0a0: 0a52 656c 6561 7365 6420 3a20 3330 204a  .Released : 30 J
-0000f0b0: 616e 7561 7279 2032 3031 390a 0a54 6869  anuary 2019..Thi
-0000f0c0: 7320 6d61 6a6f 7220 7265 6c65 6173 6520  s major release 
-0000f0d0: 6163 6375 6d75 6c61 7465 7320 6d6f 7265  accumulates more
-0000f0e0: 2074 6861 6e20 616e 2079 6561 7227 7320   than an year's 
-0000f0f0: 776f 7274 6820 6f66 2069 6d70 726f 7665  worth of improve
-0000f100: 6d65 6e74 732c 0a63 6861 6e67 6573 2061  ments,.changes a
-0000f110: 6e64 2062 7567 2066 6978 6573 2074 6f20  nd bug fixes to 
-0000f120: 7468 6520 636f 6465 2062 6173 652e 0a0a  the code base...
-0000f130: 4120 6665 7720 6869 6768 6c69 6768 7473  A few highlights
-0000f140: 206f 6620 7468 6973 2072 656c 6561 7365   of this release
-0000f150: 2061 7265 203a 0a0a 2a20 5265 6d6f 7661   are :..* Remova
-0000f160: 6c20 6f66 2032 746f 3320 6669 7865 7273  l of 2to3 fixers
-0000f170: 2061 6e64 2074 6865 2075 7365 206f 6620   and the use of 
-0000f180: 7369 7820 746f 2070 726f 7669 6465 2050  six to provide P
-0000f190: 7974 686f 6e20 322f 3320 636f 6d70 6174  ython 2/3 compat
-0000f1a0: 6962 696c 6974 790a 2a20 5265 6d6f 7661  ibility.* Remova
-0000f1b0: 6c20 6f66 2064 6570 7265 6361 7465 6420  l of deprecated 
-0000f1c0: 6060 7472 6169 7473 2e70 726f 746f 636f  ``traits.protoco
-0000f1d0: 6c73 6060 2073 7562 6d6f 6475 6c65 2061  ls`` submodule a
-0000f1e0: 6e64 2072 656c 6174 6564 2075 7469 6c73  nd related utils
-0000f1f0: 2e0a 2a20 4e65 7720 6060 4861 7352 6571  ..* New ``HasReq
-0000f200: 7569 7265 6454 7261 6974 7360 6020 636c  uiredTraits`` cl
-0000f210: 6173 730a 2a20 4265 7474 6572 2049 5079  ass.* Better IPy
-0000f220: 7468 6f6e 2074 6162 2063 6f6d 706c 6574  thon tab complet
-0000f230: 696f 6e20 666f 7220 6060 4861 7354 7261  ion for ``HasTra
-0000f240: 6974 7360 6020 7375 6263 6c61 7373 6573  its`` subclasses
-0000f250: 0a0a 4368 616e 6765 7320 7375 6d6d 6172  ..Changes summar
-0000f260: 7920 7369 6e63 6520 342e 362e 300a 7e7e  y since 4.6.0.~~
-0000f270: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-0000f280: 7e7e 7e7e 7e7e 7e7e 7e0a 0a45 6e68 616e  ~~~~~~~~~..Enhan
-0000f290: 6365 6d65 6e74 730a 0a2a 2043 4920 666f  cements..* CI fo
-0000f2a0: 7220 646f 6375 6d65 6e74 6174 696f 6e20  r documentation 
-0000f2b0: 2823 3433 3129 0a2a 2052 656d 6f76 6520  (#431).* Remove 
-0000f2c0: 3274 6f33 2066 6978 6572 7320 2823 3433  2to3 fixers (#43
-0000f2d0: 3029 0a2a 2045 6e74 686f 7567 6874 2053  0).* Enthought S
-0000f2e0: 7068 696e 7820 5468 656d 6520 666f 7220  phinx Theme for 
-0000f2f0: 646f 6373 2028 2334 3237 290a 2a20 4e65  docs (#427).* Ne
-0000f300: 7720 6060 4861 7352 6571 7569 7265 6454  w ``HasRequiredT
-0000f310: 7261 6974 7360 6020 636c 6173 7320 2823  raits`` class (#
-0000f320: 3431 3929 0a2a 2046 7265 6520 6060 4861  419).* Free ``Ha
-0000f330: 7354 7261 6974 7360 6020 7375 6263 6c61  sTraits`` subcla
-0000f340: 7373 6573 2066 726f 6d20 6861 7368 696e  sses from hashin
-0000f350: 672f 636f 6d70 6172 696e 6720 6279 2069  g/comparing by i
-0000f360: 6465 6e74 6974 7920 2823 3431 3029 0a2a  dentity (#410).*
-0000f370: 2055 6e69 6679 2061 6e64 2066 6978 2064   Unify and fix d
-0000f380: 6566 6175 6c74 206c 6973 7420 6564 6974  efault list edit
-0000f390: 6f72 7320 2823 3339 3629 0a2a 2041 6464  ors (#396).* Add
-0000f3a0: 2060 605f 5f64 6972 5f5f 6060 206d 6574   ``__dir__`` met
-0000f3b0: 686f 6420 746f 2060 6048 6173 5472 6169  hod to ``HasTrai
-0000f3c0: 7473 6060 2066 6f72 2049 5079 7468 6f6e  ts`` for IPython
-0000f3d0: 2074 6162 2063 6f6d 706c 6574 696f 6e20   tab completion 
-0000f3e0: 2823 3338 3229 0a2a 2050 7974 686f 6e20  (#382).* Python 
-0000f3f0: 3320 636f 6d70 6174 6962 696c 6974 7920  3 compatibility 
-0000f400: 6669 7865 7320 2823 3337 3429 0a2a 204e  fixes (#374).* N
-0000f410: 6577 2063 6f6e 7465 7874 206d 616e 6167  ew context manag
-0000f420: 6572 2066 6f72 2073 6574 7469 6e67 2074  er for setting t
-0000f430: 7261 6974 2d63 6861 6e67 652d 6576 656e  rait-change-even
-0000f440: 7420 7472 6163 6572 2028 2333 3635 290a  t tracer (#365).
-0000f450: 2a20 4465 6661 756c 7420 7472 6169 7420  * Default trait 
-0000f460: 7479 7065 2063 6f6e 7374 616e 7473 2028  type constants (
-0000f470: 2333 3534 290a 0a43 6861 6e67 6573 0a0a  #354)..Changes..
-0000f480: 2a20 5265 6d6f 7665 2064 6570 7265 6361  * Remove depreca
-0000f490: 7465 6420 6060 7472 6169 7473 2e70 726f  ted ``traits.pro
-0000f4a0: 746f 636f 6c73 6060 2073 7562 6d6f 6475  tocols`` submodu
-0000f4b0: 6c65 2061 6e64 2072 656c 6174 6564 2075  le and related u
-0000f4c0: 7469 6c73 2028 2334 3335 290a 2a20 4669  tils (#435).* Fi
-0000f4d0: 7820 696e 7661 6c69 6420 7374 7269 6e67  x invalid string
-0000f4e0: 2065 7363 6170 6573 2028 2334 3239 290a   escapes (#429).
-0000f4f0: 2a20 4170 706c 7920 7468 6520 2262 6c61  * Apply the "bla
-0000f500: 636b 2220 636f 6465 2072 6566 6f72 6d61  ck" code reforma
-0000f510: 7474 696e 6720 7574 696c 6974 7920 6f6e  tting utility on
-0000f520: 2074 6865 2054 7261 6974 7320 636f 6465   the Traits code
-0000f530: 6261 7365 2028 2334 3332 290a 2a20 5570  base (#432).* Up
-0000f540: 6461 7465 2043 4920 746f 2075 7365 2065  date CI to use e
-0000f550: 646d 2061 6e64 2065 7473 746f 6f6c 206d  dm and etstool m
-0000f560: 6f64 756c 6520 2823 3432 3029 0a2a 2043  odule (#420).* C
-0000f570: 6c65 616e 2075 7020 6060 466c 6f61 7460  lean up ``Float`
-0000f580: 6020 616e 6420 6060 4261 7365 466c 6f61  ` and ``BaseFloa
-0000f590: 7460 6020 7661 6c69 6461 7469 6f6e 2028  t`` validation (
-0000f5a0: 2333 3933 290a 2a20 4d65 7267 6520 6d61  #393).* Merge ma
-0000f5b0: 7374 6572 2069 6e74 6f20 4379 7468 6f6e  ster into Cython
-0000f5c0: 2070 6f72 7420 2823 3337 3029 0a2a 2044   port (#370).* D
-0000f5d0: 6f63 7320 616e 6420 6d69 6e6f 7220 7265  ocs and minor re
-0000f5e0: 6661 6374 6f72 696e 6720 6f66 2060 604d  factoring of ``M
-0000f5f0: 6574 6148 6173 5472 6169 7473 6060 2063  etaHasTraits`` c
-0000f600: 6c61 7373 2028 2333 3636 290a 2a20 5265  lass (#366).* Re
-0000f610: 6d6f 7665 2072 6964 6963 756c 6f75 7320  move ridiculous 
-0000f620: 7072 656d 6174 7572 6520 6f70 7469 6d69  premature optimi
-0000f630: 7a61 7469 6f6e 2028 2333 3632 290a 2a20  zation (#362).* 
-0000f640: 4164 6420 7375 7070 6f72 7420 666f 7220  Add support for 
-0000f650: 5079 496e 7374 616c 6c65 7220 6170 7020  PyInstaller app 
-0000f660: 6275 6e64 6c65 7220 2823 3336 3129 0a2a  bundler (#361).*
-0000f670: 2041 6464 2064 6573 6372 6970 7469 6f6e   Add description
-0000f680: 2061 6e64 2065 7861 6d70 6c65 2066 6f72   and example for
-0000f690: 2060 6045 6974 6865 7260 6020 7472 6169   ``Either`` trai
-0000f6a0: 7420 7479 7065 2028 2333 3630 290a 2a20  t type (#360).* 
-0000f6b0: 4472 6f70 2073 7570 706f 7274 2066 6f72  Drop support for
-0000f6c0: 2050 7974 686f 6e20 322e 3620 616e 6420   Python 2.6 and 
-0000f6d0: 5079 7468 6f6e 203c 2033 2e34 2028 2333  Python < 3.4 (#3
-0000f6e0: 3435 290a 2a20 4164 6420 6d61 6b65 2074  45).* Add make t
-0000f6f0: 6172 6765 7420 666f 7220 646f 6373 6574  arget for docset
-0000f700: 2074 6f20 6265 2075 7365 6420 7769 7468   to be used with
-0000f710: 2044 6173 682f 5a65 616c 2028 2331 3830   Dash/Zeal (#180
-0000f720: 290a 0a46 6978 6573 0a0a 2a20 4669 7820  )..Fixes..* Fix 
-0000f730: 6f64 6420 6572 726f 7220 6d65 7373 6167  odd error messag
-0000f740: 6520 616e 6420 7772 6f6e 6720 6578 6365  e and wrong exce
-0000f750: 7074 696f 6e20 7479 7065 2028 2334 3236  ption type (#426
-0000f760: 290a 2a20 4669 7820 436f 6c6f 7220 616e  ).* Fix Color an
-0000f770: 6420 5247 4243 6f6c 6f72 2064 6f63 2073  d RGBColor doc s
-0000f780: 7472 696e 6773 2028 2334 3137 290a 2a20  trings (#417).* 
-0000f790: 4669 7820 7573 6520 6f66 2064 6570 7265  Fix use of depre
-0000f7a0: 6361 7265 6420 6060 696e 7370 6563 742e  cared ``inspect.
-0000f7b0: 6765 7461 7267 7370 6563 6060 2066 756e  getargspec`` fun
-0000f7c0: 6374 696f 6e20 2823 3430 3829 0a2a 2046  ction (#408).* F
-0000f7d0: 6978 2065 7874 656e 6465 6420 6e61 6d65  ix extended name
-0000f7e0: 7320 696e 2060 606f 6e5f 7472 6169 745f  s in ``on_trait_
-0000f7f0: 6368 616e 6765 6060 206c 6973 7473 2028  change`` lists (
-0000f800: 2334 3034 290a 2a20 5375 7070 6f72 7420  #404).* Support 
-0000f810: 556e 6963 6f64 6520 6f6e 2074 7261 6974  Unicode on trait
-0000f820: 2064 6f63 756d 656e 7465 7220 6f6e 2050   documenter on P
-0000f830: 7974 686f 6e20 322e 3720 2823 3338 3629  ython 2.7 (#386)
-0000f840: 0a2a 2043 6c65 6172 2065 7863 6570 7469  .* Clear excepti
-0000f850: 6f6e 2066 726f 6d20 4e75 6d70 7920 7072  on from Numpy pr
-0000f860: 6f70 6572 6c79 2028 2333 3737 290a 2a20  operly (#377).* 
-0000f870: 4669 7820 7069 636b 6c69 6e67 2061 6e64  Fix pickling and
-0000f880: 2064 6565 7063 6f70 7969 6e67 2062 7567   deepcopying bug
-0000f890: 2077 6974 6820 6479 6e61 6d69 6361 6c6c   with dynamicall
-0000f8a0: 7920 6164 6465 6420 7472 6169 7473 2028  y added traits (
-0000f8b0: 2333 3733 290a 2a20 5365 7420 6060 6175  #373).* Set ``au
-0000f8c0: 746f 5f73 6574 2f65 6e74 6572 5f73 6574  to_set/enter_set
-0000f8d0: 6060 2064 6566 6175 6c74 206f 6e63 6520  `` default once 
-0000f8e0: 2823 3337 3129 0a2a 2046 6978 2076 616c  (#371).* Fix val
-0000f8f0: 6964 6174 696f 6e20 6f66 2060 6054 6869  idation of ``Thi
-0000f900: 7360 6020 7472 6169 7420 2823 3335 3329  s`` trait (#353)
-0000f910: 0a2a 204d 616b 6520 6060 6354 7261 6974  .* Make ``cTrait
-0000f920: 2e64 6566 6175 6c74 5f76 616c 7565 5f66  .default_value_f
-0000f930: 6f72 6060 2072 6169 7365 2061 2060 6056  or`` raise a ``V
-0000f940: 616c 7565 4572 726f 7260 6020 696e 7374  alueError`` inst
-0000f950: 6561 6420 6f66 0a20 2073 6567 2066 6175  ead of.  seg fau
-0000f960: 6c74 696e 6720 7768 656e 2061 736b 6564  lting when asked
-0000f970: 2066 6f72 2074 6865 2064 6566 6175 6c74   for the default
-0000f980: 2076 616c 7565 206f 6620 6120 7472 6169   value of a trai
-0000f990: 7420 7468 6174 2064 6f65 736e 2774 0a20  t that doesn't. 
-0000f9a0: 2068 6176 6520 6f6e 652e 2028 2333 3530   have one. (#350
-0000f9b0: 290a 2a20 4669 7820 6d69 7375 7365 206f  ).* Fix misuse o
-0000f9c0: 6620 6060 756e 6974 7465 7374 2e65 7870  f ``unittest.exp
-0000f9d0: 6563 7465 6446 6169 6c75 7265 6060 2064  ectedFailure`` d
-0000f9e0: 6563 6f72 6174 6f72 2028 2333 3436 290a  ecorator (#346).
-0000f9f0: 2a20 4669 7820 6973 7375 6520 7769 7468  * Fix issue with
-0000fa00: 206f 7665 7272 6964 6465 6e20 6060 4861   overridden ``Ha
-0000fa10: 7354 7261 6974 732e 7472 6169 7460 6020  sTraits.trait`` 
-0000fa20: 6675 6e63 7469 6f6e 2028 2333 3433 290a  function (#343).
-0000fa30: 0a0a 5265 6c65 6173 6520 342e 362e 300a  ..Release 4.6.0.
-0000fa40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54  -------------..T
-0000fa50: 6869 7320 6973 2061 6e20 696e 6372 656d  his is an increm
-0000fa60: 656e 7461 6c20 7265 6c65 6173 6520 6f76  ental release ov
-0000fa70: 6572 2034 2e35 2c20 6163 6375 6d75 6c61  er 4.5, accumula
-0000fa80: 7469 6e67 206f 7665 7220 6120 7965 6172  ting over a year
-0000fa90: 2773 2077 6f72 7468 206f 660a 6275 6766  's worth of.bugf
-0000faa0: 6978 6573 2061 6e64 2073 6d61 6c6c 2069  ixes and small i
-0000fab0: 6d70 726f 7665 6d65 6e74 7320 746f 2074  mprovements to t
-0000fac0: 6865 2063 6f64 652e 0a0a 4869 6768 6c69  he code...Highli
-0000fad0: 6768 7473 206f 6620 7468 6973 2072 656c  ghts of this rel
-0000fae0: 6561 7365 2069 6e63 6c75 6465 3a0a 0a2a  ease include:..*
-0000faf0: 2073 7570 706f 7274 2066 6f72 2050 7974   support for Pyt
-0000fb00: 686f 6e20 332e 3420 616e 6420 332e 352e  hon 3.4 and 3.5.
-0000fb10: 0a2a 206e 6577 2042 7974 6573 2061 6e64  .* new Bytes and
-0000fb20: 2056 616c 6964 6174 6564 5475 706c 6520   ValidatedTuple 
-0000fb30: 7472 6169 7473 2e0a 2a20 6120 6e65 7720  traits..* a new 
-0000fb40: 4172 7261 794f 724e 6f6e 6520 7472 6169  ArrayOrNone trai
-0000fb50: 7420 7768 6963 6820 636f 7272 6563 746c  t which correctl
-0000fb60: 7920 6861 6e64 6c65 7320 4e6f 6e65 2063  y handles None c
-0000fb70: 6f6d 7061 7269 736f 6e73 2077 6974 6820  omparisons with 
-0000fb80: 4e75 6d70 790a 2020 6172 7261 7973 2e0a  Numpy.  arrays..
-0000fb90: 2a20 636c 6561 6e2d 7570 206f 6620 7468  * clean-up of th
-0000fba0: 6520 4554 5343 6f6e 6669 6720 636f 6465  e ETSConfig code
-0000fbb0: 2066 6f72 2054 7261 6974 7355 4920 746f   for TraitsUI to
-0000fbc0: 6f6c 6b69 7420 7365 6c65 6374 696f 6e2e  olkit selection.
-0000fbd0: 0a2a 2062 6574 7465 7220 636f 6d70 6174  .* better compat
-0000fbe0: 6962 696c 6974 7920 7769 7468 204e 756d  ibility with Num
-0000fbf0: 5079 2073 6361 6c61 7220 7479 7065 732e  Py scalar types.
-0000fc00: 0a2a 206d 616e 7920 6f74 6865 7220 6275  .* many other bu
-0000fc10: 6766 6978 6573 2061 6e64 2069 6d70 726f  gfixes and impro
-0000fc20: 7665 6d65 6e74 732e 0a0a 4368 616e 6765  vements...Change
-0000fc30: 2073 756d 6d61 7279 2073 696e 6365 2034   summary since 4
-0000fc40: 2e35 2e30 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  .5.0.~~~~~~~~~~~
-0000fc50: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
-0000fc60: 0a45 6e68 616e 6365 6d65 6e74 730a 0a2a  .Enhancements..*
-0000fc70: 2041 6464 6564 2061 2060 6042 7974 6573   Added a ``Bytes
-0000fc80: 6060 2054 7261 6974 2061 6e64 2072 656c  `` Trait and rel
-0000fc90: 6174 6564 2074 7261 6974 7320 2823 3332  ated traits (#32
-0000fca0: 3929 0a2a 2041 6464 6564 2073 7570 706f  9).* Added suppo
-0000fcb0: 7274 2066 6f72 2066 696e 6469 6e67 2072  rt for finding r
-0000fcc0: 6573 6f75 7263 6573 2066 726f 6d20 7a69  esources from zi
-0000fcd0: 7070 6564 2050 7974 686f 6e20 736f 7572  pped Python sour
-0000fce0: 6365 2063 6f64 6520 2823 3331 3629 0a2a  ce code (#316).*
-0000fcf0: 2041 6464 6564 2069 6e2d 706c 6163 6520   Added in-place 
-0000fd00: 7365 7420 6172 6974 686d 6574 6963 206f  set arithmetic o
-0000fd10: 7065 7261 7469 6f6e 7320 666f 7220 6060  perations for ``
-0000fd20: 5472 6169 7453 6574 4f62 6a65 6374 6060  TraitSetObject``
-0000fd30: 7320 616e 6420 6163 6365 7074 0a20 206d  s and accept.  m
-0000fd40: 6174 6368 2062 6568 6176 696f 7572 206f  atch behaviour o
-0000fd50: 6620 6060 5472 6169 7453 6574 4f62 6a65  f ``TraitSetObje
-0000fd60: 6374 6060 2077 6974 6820 7265 6775 6c61  ct`` with regula
-0000fd70: 7220 5079 7468 6f6e 2073 6574 7320 7768  r Python sets wh
-0000fd80: 656e 0a20 2070 6572 666f 726d 696e 6720  en.  performing 
-0000fd90: 6f70 6572 6174 696f 6e73 2077 6974 6820  operations with 
-0000fda0: 6e6f 6e2d 7365 7420 7479 7065 7320 2865  non-set types (e
-0000fdb0: 672e 206c 6973 7473 2c20 6469 6374 696f  g. lists, dictio
-0000fdc0: 6e61 7269 6573 2920 2823 3238 3929 0a2a  naries) (#289).*
-0000fdd0: 2041 6464 6564 2061 2063 6f6e 7465 7874   Added a context
-0000fde0: 206d 616e 6167 6572 2074 6f20 616c 6c6f   manager to allo
-0000fdf0: 7720 7072 6f76 6973 696f 6e61 6c20 7365  w provisional se
-0000fe00: 6c65 6374 696f 6e20 6f66 2061 2074 6f6f  lection of a too
-0000fe10: 6c6b 6974 2074 6f0a 2020 6060 4554 5343  lkit to.  ``ETSC
-0000fe20: 6f6e 6669 6760 6020 2874 6869 7320 6765  onfig`` (this ge
-0000fe30: 6e65 7261 6c6c 7920 696d 7072 6f76 6573  nerally improves
-0000fe40: 2072 656c 6961 6269 6c69 7479 206f 6620   reliability of 
-0000fe50: 746f 6f6c 6b69 7420 7365 6c65 6374 696f  toolkit selectio
-0000fe60: 6e0a 2020 666f 7220 5079 6661 6365 2061  n.  for Pyface a
-0000fe70: 6e64 2054 7261 6974 7355 4929 2e20 2823  nd TraitsUI). (#
-0000fe80: 3237 3629 0a2a 2041 6464 6564 2054 7261  276).* Added Tra
-0000fe90: 6974 2063 6861 6e67 6520 7265 636f 7264  it change record
-0000fea0: 6572 2074 6f20 6169 6420 696e 2064 6562  er to aid in deb
-0000feb0: 7567 6769 6e67 2065 7665 6e74 2d64 7269  ugging event-dri
-0000fec0: 7665 6e20 636f 6465 2e20 2823 3133 3929  ven code. (#139)
-0000fed0: 0a2a 2060 605f 5f69 6164 645f 5f60 6020  .* ``__iadd__`` 
-0000fee0: 616e 6420 6060 5f5f 696d 756c 5f5f 6060  and ``__imul__``
-0000fef0: 2069 6d70 6c65 6d65 6e74 6564 206f 6e20   implemented on 
-0000ff00: 5472 6169 744c 6973 744f 626a 6563 7473  TraitListObjects
-0000ff10: 2e20 2823 3136 3529 0a2a 2041 6464 6564  . (#165).* Added
-0000ff20: 206e 6577 2060 6041 7272 6179 4f72 4e6f   new ``ArrayOrNo
-0000ff30: 6e65 6060 2074 7261 6974 2074 7970 6520  ne`` trait type 
-0000ff40: 746f 2072 6570 6c61 6365 2074 6865 0a20  to replace the. 
-0000ff50: 2060 6045 6974 6865 7228 4e6f 6e65 2c20   ``Either(None, 
-0000ff60: 4172 7261 7929 6060 2069 6469 6f6d 2e20  Array)`` idiom. 
-0000ff70: 2054 6865 206f 6c64 2069 6469 6f6d 2072   The old idiom r
-0000ff80: 6573 756c 7473 2069 6e20 7761 726e 696e  esults in warnin
-0000ff90: 6773 0a20 206f 6e20 4e75 6d50 7920 3e3d  gs.  on NumPy >=
-0000ffa0: 2031 2e39 2e20 2823 3231 3929 0a2a 2041   1.9. (#219).* A
-0000ffb0: 6464 6564 2061 206e 6577 2060 6056 616c  dded a new ``Val
-0000ffc0: 6964 6174 6564 5475 706c 6560 6020 7472  idatedTuple`` tr
-0000ffd0: 6169 7420 7468 6174 2073 7570 706f 7274  ait that support
-0000ffe0: 7320 6375 7374 6f6d 2076 616c 6964 6174  s custom validat
-0000fff0: 696f 6e2e 2028 2332 3035 290a 0a43 6861  ion. (#205)..Cha
-00010000: 6e67 6573 0a0a 2a20 5265 6d6f 7665 6420  nges..* Removed 
-00010010: 7265 6475 6e64 616e 742c 2069 6e74 6572  redundant, inter
-00010020: 6e61 6c20 6060 4554 5343 6f6e 6669 6760  nal ``ETSConfig`
-00010030: 6020 6672 6f6d 2054 7261 6974 7320 636f  ` from Traits co
-00010040: 6465 6261 7365 2e20 2823 3332 3729 0a2a  debase. (#327).*
-00010050: 2042 6574 7465 7220 6572 726f 7220 7265   Better error re
-00010060: 706f 7274 696e 6720 666f 7220 6661 696c  porting for fail
-00010070: 6564 2061 7474 7269 6275 7465 2061 6363  ed attribute acc
-00010080: 6573 732e 2028 2332 3433 290a 2a20 5265  ess. (#243).* Re
-00010090: 6d6f 7665 6420 6275 6767 7920 6060 2d74  moved buggy ``-t
-000100a0: 6f6f 6c6b 6974 6060 2063 6f6d 6d61 6e64  oolkit`` command
-000100b0: 6c69 6e65 206f 7074 696f 6e20 6060 4554  line option ``ET
-000100c0: 5343 6f6e 6669 6760 602e 2028 2333 3236  SConfig``. (#326
-000100d0: 290a 2a20 5265 6d6f 7665 6420 6275 6767  ).* Removed bugg
-000100e0: 7920 6060 2a6e 616d 6573 6060 2070 6f73  y ``*names`` pos
-000100f0: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
-00010100: 7320 6672 6f6d 2060 606f 6e5f 7472 6169  s from ``on_trai
-00010110: 745f 6368 616e 6765 6060 0a20 2064 6563  t_change``.  dec
-00010120: 6f72 6174 6f72 2069 6e20 696d 7072 6f76  orator in improv
-00010130: 6564 2061 7267 756d 656e 7420 7061 7373  ed argument pass
-00010140: 696e 6720 2823 3230 3729 2e0a 2a20 416c  ing (#207)..* Al
-00010150: 6c6f 7720 6060 466c 6f61 7460 6020 616e  low ``Float`` an
-00010160: 6420 6060 4261 7365 466c 6f61 7460 6020  d ``BaseFloat`` 
-00010170: 7472 6169 7473 2074 6f20 6163 6365 7074  traits to accept
-00010180: 2050 7974 686f 6e20 6c6f 6e67 732e 2028   Python longs. (
-00010190: 2332 3732 290a 2a20 436c 6561 6e2d 7570  #272).* Clean-up
-000101a0: 2061 6e64 2066 6978 6573 2074 6f20 6578   and fixes to ex
-000101b0: 616d 706c 6520 636f 6465 2e20 2823 3132  ample code. (#12
-000101c0: 3629 0a2a 2052 656d 6f76 6520 6f75 7464  6).* Remove outd
-000101d0: 6174 6564 2060 6049 6d70 6f72 7453 7079  ated ``ImportSpy
-000101e0: 6060 2061 6e64 2060 6049 6d70 6f72 744d  `` and ``ImportM
-000101f0: 616e 6167 6572 6060 2075 7469 6c69 7469  anager`` utiliti
-00010200: 6573 2e20 2823 3138 3829 0a2a 2054 6865  es. (#188).* The
-00010210: 2060 6064 6570 7265 6361 7465 6460 6020   ``deprecated`` 
-00010220: 6465 636f 7261 746f 7220 6e6f 7720 6973  decorator now is
-00010230: 7375 6573 2061 2044 6570 7265 6361 7469  sues a Deprecati
-00010240: 6f6e 5761 726e 696e 6720 2875 7369 6e67  onWarning (using
-00010250: 0a20 2074 6865 2050 7974 686f 6e20 6060  .  the Python ``
-00010260: 7761 726e 696e 6773 6060 206d 6f64 756c  warnings`` modul
-00010270: 6529 2072 6174 6865 7220 7468 616e 206c  e) rather than l
-00010280: 6f67 6769 6e67 2061 2077 6172 6e69 6e67  ogging a warning
-00010290: 2076 6961 0a20 2074 6865 2060 606c 6f67   via.  the ``log
-000102a0: 6769 6e67 6060 206d 6163 6869 6e65 7279  ging`` machinery
-000102b0: 2e20 2049 7420 6e6f 206c 6f6e 6765 7220  .  It no longer 
-000102c0: 7472 6965 7320 746f 2072 656d 656d 6265  tries to remembe
-000102d0: 7220 7768 656e 0a20 2061 2077 6172 6e69  r when.  a warni
-000102e0: 6e67 2068 6173 2062 6565 6e20 7072 6576  ng has been prev
-000102f0: 696f 7573 6c79 2069 7373 7565 642e 2028  iously issued. (
-00010300: 2332 3230 290a 2a20 4465 7072 6563 6174  #220).* Deprecat
-00010310: 6564 2060 6048 6173 5472 6169 7473 2e67  ed ``HasTraits.g
-00010320: 6574 2829 6060 2061 6e64 2060 6048 6173  et()`` and ``Has
-00010330: 5472 6169 7473 2e73 6574 2829 6060 2028  Traits.set()`` (
-00010340: 2331 3930 292e 0a2a 2054 6865 2064 6566  #190)..* The def
-00010350: 6175 6c74 2060 6056 6965 7760 6020 7368  ault ``View`` sh
-00010360: 6f77 7320 616c 6c20 286e 6f6e 2d65 7665  ows all (non-eve
-00010370: 6e74 2920 7472 6169 7473 2077 686f 7365  nt) traits whose
-00010380: 2060 6076 6973 6962 6c65 6060 2070 726f   ``visible`` pro
-00010390: 7065 7274 790a 2020 6973 206e 6f74 2060  perty.  is not `
-000103a0: 6046 616c 7365 6060 2e20 5072 6976 6174  `False``. Privat
-000103b0: 6520 7472 6169 7473 2061 7265 2073 6574  e traits are set
-000103c0: 2060 6076 6973 6962 6c65 3d46 616c 7365   ``visible=False
-000103d0: 6060 2062 7920 6465 6661 756c 742e 2028  `` by default. (
-000103e0: 2332 3334 290a 0a46 6978 6573 0a0a 2a20  #234)..Fixes..* 
-000103f0: 4669 7820 426f 6f6c 2074 7261 6974 7320  Fix Bool traits 
-00010400: 736f 2074 6861 7420 7661 6c75 6520 7374  so that value st
-00010410: 6f72 6564 2069 7320 616c 7761 7973 2061  ored is always a
-00010420: 2050 7974 686f 6e20 6060 626f 6f6c 6060   Python ``bool``
-00010430: 2028 616e 6420 696e 0a20 2070 6172 7469   (and in.  parti
-00010440: 6375 6c61 722c 206e 6f74 2061 204e 756d  cular, not a Num
-00010450: 5079 2060 606e 702e 626f 6f6c 5f60 6029  Py ``np.bool_``)
-00010460: 2e20 2823 3331 3829 0a2a 2046 6978 2042  . (#318).* Fix B
-00010470: 6f6f 6c20 7472 6169 7473 2073 6f20 7468  ool traits so th
-00010480: 6174 2072 6567 756c 6172 2076 616c 6964  at regular valid
-00010490: 6174 6f72 2061 6363 6570 7473 204e 756d  ator accepts Num
-000104a0: 7050 7927 7320 6060 6e70 2e62 6f6f 6c5f  pPy's ``np.bool_
-000104b0: 6060 0a20 2062 6f6f 6c65 616e 2076 616c  ``.  boolean val
-000104c0: 7565 7320 2862 7269 6e67 696e 6720 6974  ues (bringing it
-000104d0: 2069 6e20 6167 7265 656d 656e 7420 7769   in agreement wi
-000104e0: 7468 2074 6865 2066 6173 7420 7661 6c69  th the fast vali
-000104f0: 6461 746f 7229 2e20 2823 3330 3229 0a2a  dator). (#302).*
-00010500: 2046 6978 2075 7365 206f 6620 6060 6e65   Fix use of ``ne
-00010510: 7874 6060 2069 6e20 6060 5472 6169 7444  xt`` in ``TraitD
-00010520: 6f63 756d 656e 7465 7260 6020 666f 7220  ocumenter`` for 
-00010530: 5079 7468 6f6e 2033 2063 6f6d 7061 7469  Python 3 compati
-00010540: 6269 6c69 7479 2e20 2823 3239 3329 0a2a  bility. (#293).*
-00010550: 2046 6978 206f 6666 2d62 792d 6f6e 6520   Fix off-by-one 
-00010560: 6572 726f 7220 7768 656e 2060 6054 7261  error when ``Tra
-00010570: 6974 4c69 7374 4f62 6a65 6374 6060 2069  itListObject`` i
-00010580: 7320 7365 7474 696e 6720 6f72 2064 656c  s setting or del
-00010590: 6574 696e 6720 736c 6963 6573 2e0a 2020  eting slices..  
-000105a0: 2823 3238 3329 0a2a 2046 6978 2072 6566  (#283).* Fix ref
-000105b0: 6572 656e 6365 2063 7963 6c65 7320 6361  erence cycles ca
-000105c0: 7573 6564 2062 7920 6060 7379 6e63 5f74  used by ``sync_t
-000105d0: 7261 6974 7360 602e 2028 2331 3335 290a  raits``. (#135).
-000105e0: 2a20 4669 7820 736f 2074 6861 7420 6060  * Fix so that ``
-000105f0: 7379 732e 6578 635f 696e 666f 2829 6060  sys.exc_info()``
-00010600: 2077 6f72 6b73 2061 7320 6578 7065 6374   works as expect
-00010610: 6564 2069 6e20 6578 6365 7074 696f 6e20  ed in exception 
-00010620: 6861 6e64 6c65 7273 2069 6e0a 2020 5079  handlers in.  Py
-00010630: 7468 6f6e 2033 2028 2332 3636 290a 2a20  thon 3 (#266).* 
-00010640: 4669 7820 6060 5374 7269 6e67 6060 2074  Fix ``String`` t
-00010650: 7261 6974 2074 6f20 6163 6365 7074 2060  rait to accept `
-00010660: 6073 7472 6060 2073 7562 636c 6173 7365  `str`` subclasse
-00010670: 7320 286c 696b 6520 6060 6e75 6d70 792e  s (like ``numpy.
-00010680: 7374 725f 6060 292e 0a20 2028 2332 3637  str_``)..  (#267
-00010690: 290a 2a20 4669 7865 6420 696e 636f 7272  ).* Fixed incorr
-000106a0: 6563 7420 696e 206c 6973 7420 6576 656e  ect in list even
-000106b0: 7473 2066 6f72 2060 6069 6e73 6572 7460  ts for ``insert`
-000106c0: 6020 6f70 6572 6174 696f 6e73 2077 6974  ` operations wit
-000106d0: 6820 616e 2069 6e64 6578 0a20 206f 7574  h an index.  out
-000106e0: 7369 6465 2074 6865 2072 616e 6765 205b  side the range [
-000106f0: 6060 2d6c 656e 2874 6172 6765 745f 6c69  ``-len(target_li
-00010700: 7374 2960 602c 2060 606c 656e 2874 6172  st)``, ``len(tar
-00010710: 6765 745f 6c69 7374 2960 605d 2e20 2823  get_list)``]. (#
-00010720: 3136 3529 0a2a 2046 6978 2069 6e63 6f72  165).* Fix incor
-00010730: 7265 6374 2062 6568 6176 696f 7572 206f  rect behaviour o
-00010740: 6620 6060 6368 6563 6b5f 696d 706c 656d  f ``check_implem
-00010750: 656e 7473 6060 2066 6f72 206f 7665 7272  ents`` for overr
-00010760: 6964 6465 6e20 6d65 7468 6f64 732e 0a20  idden methods.. 
-00010770: 2028 2331 3932 290a 2a20 4669 7820 6572   (#192).* Fix er
-00010780: 726f 7220 7768 656e 2074 7279 696e 6720  ror when trying 
-00010790: 746f 206c 6973 7465 6e20 746f 2074 7261  to listen to tra
-000107a0: 6974 7320 7573 696e 6720 6c69 7374 2062  its using list b
-000107b0: 7261 636b 6574 206e 6f74 6174 696f 6e2e  racket notation.
-000107c0: 2028 2331 3935 290a 2a20 4669 7820 7265   (#195).* Fix re
-000107d0: 6665 7265 6e63 6520 6c65 616b 2069 6e20  ference leak in 
-000107e0: 6060 4348 6173 5472 6169 7473 2e5f 6e6f  ``CHasTraits._no
-000107f0: 7469 6669 6572 7360 602e 2028 2332 3438  tifiers``. (#248
-00010800: 290a 2a20 4669 7820 7265 6665 7265 6e63  ).* Fix referenc
-00010810: 6520 6c65 616b 2066 726f 6d20 7573 6520  e leak from use 
-00010820: 6f66 2060 6044 656c 6567 6174 6573 546f  of ``DelegatesTo
-00010830: 6060 2e20 2823 3236 3029 0a2a 2049 6e73  ``. (#260).* Ins
-00010840: 7461 6e63 6520 7472 6169 7473 2077 6572  tance traits wer
-00010850: 656e 2774 2069 6e63 6c75 6465 6420 696e  en't included in
-00010860: 2074 6865 2072 6573 756c 7420 6f66 2060   the result of `
-00010870: 6074 7261 6974 7328 2960 602e 2028 2332  `traits()``. (#2
-00010880: 3334 290a 0a0a 5265 6c65 6173 6520 342e  34)...Release 4.
-00010890: 352e 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  5.0.------------
-000108a0: 2d0a 0a54 7261 6974 7320 6973 206e 6f77  -..Traits is now
-000108b0: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-000108c0: 2050 7974 686f 6e20 3321 2054 6865 206c   Python 3! The l
-000108d0: 6962 7261 7279 206e 6f77 2073 7570 706f  ibrary now suppo
-000108e0: 7274 730a 5079 7468 6f6e 2033 2e32 2061  rts.Python 3.2 a
-000108f0: 6e64 2033 2e33 2e0a 0a54 6865 2072 656c  nd 3.3...The rel
-00010900: 6561 7365 2061 6c73 6f20 696e 636c 7564  ease also includ
-00010910: 6573 2069 6e63 7265 6173 6564 2063 6f64  es increased cod
-00010920: 6520 636f 7665 7261 6765 2061 6e64 2061  e coverage and a
-00010930: 7574 6f6d 6174 6963 0a63 6f76 6572 6167  utomatic.coverag
-00010940: 6520 7265 706f 7274 2074 6872 6f75 6768  e report through
-00010950: 2063 6f76 6572 616c 6c73 2e69 6f2e 0a0a   coveralls.io...
-00010960: 0a43 6861 6e67 6520 7375 6d6d 6172 7920  .Change summary 
-00010970: 7369 6e63 6520 342e 342e 300a 7e7e 7e7e  since 4.4.0.~~~~
-00010980: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00010990: 7e7e 7e7e 7e7e 0a0a 456e 6861 6e63 656d  ~~~~~~..Enhancem
-000109a0: 656e 7473 0a0a 2a20 5465 7374 2066 696c  ents..* Test fil
-000109b0: 6573 2063 6c65 616e 7570 7320 2823 3130  es cleanups (#10
-000109c0: 382c 2023 3131 312c 2023 3132 3129 0a2a  8, #111, #121).*
-000109d0: 2041 6464 2061 7574 6f6d 6174 6963 2063   Add automatic c
-000109e0: 6f76 6572 6167 6520 7265 706f 7274 7320  overage reports 
-000109f0: 2823 3131 302c 2023 3132 3229 0a2a 2052  (#110, #122).* R
-00010a00: 656d 6f76 6564 206f 6273 6f6c 6574 6520  emoved obsolete 
-00010a10: 636f 6465 2028 2331 3039 2c20 2331 3132  code (#109, #112
-00010a20: 2c20 2331 3133 290a 2a20 496e 6372 6561  , #113).* Increa
-00010a30: 7365 6420 7465 7374 2063 6f76 6572 6167  sed test coverag
-00010a40: 6520 2823 3131 342c 2023 3131 3829 0a2a  e (#114, #118).*
-00010a50: 2050 7974 686f 6e20 3320 7375 7070 6f72   Python 3 suppor
-00010a60: 7420 2823 3131 3529 2e20 2054 6861 6e6b  t (#115).  Thank
-00010a70: 7320 5976 6573 2044 656c 6c65 792e 0a2a  s Yves Delley..*
-00010a80: 2041 6c6c 6f77 2073 6574 7469 6e67 2061   Allow setting a
-00010a90: 6e64 2072 6573 6574 7469 6e67 2074 6865  nd resetting the
-00010aa0: 2067 6c6f 6261 6c20 6164 6170 7461 7469   global adaptati
-00010ab0: 6f6e 206d 616e 6167 6572 2028 2331 3435  on manager (#145
-00010ac0: 290a 2a20 5661 7269 6f75 7320 646f 6375  ).* Various docu
-00010ad0: 6d65 6e74 6174 696f 6e20 696d 7072 6f76  mentation improv
-00010ae0: 656d 656e 7473 2028 2331 3332 2c20 2331  ements (#132, #1
-00010af0: 3333 2c20 2331 3438 2c20 2331 3534 292e  33, #148, #154).
-00010b00: 0a0a 4368 616e 6765 730a 0a2a 2054 6865  ..Changes..* The
-00010b10: 2049 6e74 2074 7261 6974 2074 7970 6520   Int trait type 
-00010b20: 6e6f 7720 6163 6365 7074 7320 5079 7468  now accepts Pyth
-00010b30: 6f6e 2069 6e74 7320 2a61 6e64 2a20 5079  on ints *and* Py
-00010b40: 7468 6f6e 206c 6f6e 6773 2c20 6173 2077  thon longs, as w
-00010b50: 656c 6c20 6173 0a20 2069 6e73 7461 6e63  ell as.  instanc
-00010b60: 6573 206f 6620 616e 7920 5079 7468 6f6e  es of any Python
-00010b70: 2074 7970 6520 7468 6174 2069 6d70 6c65   type that imple
-00010b80: 6d65 6e74 7320 7468 6520 6060 5f5f 696e  ments the ``__in
-00010b90: 6465 785f 5f60 6020 6d65 7468 6f64 2e0a  dex__`` method..
-00010ba0: 2020 5072 6576 696f 7573 6c79 2c20 6c6f    Previously, lo
-00010bb0: 6e67 2069 6e73 7461 6e63 6573 2077 6572  ng instances wer
-00010bc0: 6520 6e6f 7420 6163 6365 7074 6564 2e20  e not accepted. 
-00010bd0: 2823 3130 342c 2023 3132 3329 2e0a 0a46  (#104, #123)...F
-00010be0: 6978 6573 0a0a 2a20 4669 7820 6372 6173  ixes..* Fix cras
-00010bf0: 6820 7768 656e 2074 7279 696e 6720 746f  h when trying to
-00010c00: 2076 616c 6964 6174 6520 6120 7072 6f70   validate a prop
-00010c10: 6572 7479 2074 6861 7420 6861 7320 6265  erty that has be
-00010c20: 656e 2064 656c 6574 6564 2e20 2823 3133  en deleted. (#13
-00010c30: 3829 0a2a 2046 6978 2063 6c65 6172 696e  8).* Fix clearin
-00010c40: 6720 6578 6365 7074 696f 6e20 7768 656e  g exception when
-00010c50: 2072 6169 7369 6e67 2061 2054 7261 6974   raising a Trait
-00010c60: 4572 726f 7220 2823 3131 3929 0a2a 2046  Error (#119).* F
-00010c70: 6978 2061 7574 6f6d 6174 6963 2061 6461  ix automatic ada
-00010c80: 7074 6174 696f 6e20 7768 656e 2061 7373  ptation when ass
-00010c90: 6967 6e69 6e67 2074 6f20 4c69 7374 2074  igning to List t
-00010ca0: 7261 6974 2028 2331 3437 290a 2a20 4669  rait (#147).* Fi
-00010cb0: 7820 736f 6d65 2063 7472 6169 7473 2072  x some ctraits r
-00010cc0: 6566 636f 756e 7469 6e67 2061 6e64 2065  efcounting and e
-00010cd0: 7863 6570 7469 6f6e 2063 6c65 6172 696e  xception clearin
-00010ce0: 6720 6275 6773 2028 2334 3829 2e20 2054  g bugs (#48).  T
-00010cf0: 6861 6e6b 7320 5976 6573 0a20 2044 656c  hanks Yves.  Del
-00010d00: 6c65 792e 0a0a 0a52 656c 6561 7365 2034  ley....Release 4
-00010d10: 2e34 2e30 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .4.0.-----------
-00010d20: 2d2d 0a0a 5468 6520 6d61 6a6f 7220 6e65  --..The major ne
-00010d30: 7720 6665 6174 7572 6520 696e 2074 6869  w feature in thi
-00010d40: 7320 7265 6c65 6173 6520 6973 2061 206e  s release is a n
-00010d50: 6577 2061 6461 7074 6174 696f 6e20 6d65  ew adaptation me
-00010d60: 6368 616e 6973 6d20 696e 2074 6865 0a60  chanism in the.`
-00010d70: 6074 7261 6974 732e 6164 6170 7461 7469  `traits.adaptati
-00010d80: 6f6e 6060 2070 6163 6b61 6765 2e20 2054  on`` package.  T
-00010d90: 6865 206e 6577 206d 6563 6861 6e69 736d  he new mechanism
-00010da0: 2069 7320 696e 7465 6e64 6564 2074 6f20   is intended to 
-00010db0: 7265 706c 6163 6520 7468 650a 6f6c 6465  replace the.olde
-00010dc0: 7220 7472 6169 7473 2e70 726f 746f 636f  r traits.protoco
-00010dd0: 6c73 2070 6163 6b61 6765 2e20 2043 6f64  ls package.  Cod
-00010de0: 6520 7772 6974 7465 6e20 6167 6169 6e73  e written agains
-00010df0: 7420 6060 7472 6169 7473 2e70 726f 746f  t ``traits.proto
-00010e00: 636f 6c73 6060 2077 696c 6c0a 636f 6e74  cols`` will.cont
-00010e10: 696e 7565 2074 6f20 776f 726b 2c20 616c  inue to work, al
-00010e20: 7468 6f75 6768 2074 6865 2060 6074 7261  though the ``tra
-00010e30: 6974 732e 7072 6f74 6f63 6f6c 7360 6020  its.protocols`` 
-00010e40: 4150 4920 6861 7320 6265 656e 2064 6570  API has been dep
-00010e50: 7265 6361 7465 642c 0a61 6e64 2061 2077  recated,.and a w
-00010e60: 6172 6e69 6e67 2077 696c 6c20 6265 206c  arning will be l
-00010e70: 6f67 6765 6420 6f6e 2066 6972 7374 2075  ogged on first u
-00010e80: 7365 206f 6620 6060 7472 6169 7473 2e70  se of ``traits.p
-00010e90: 726f 746f 636f 6c73 6060 2e20 2053 6565  rotocols``.  See
-00010ea0: 2074 6865 0a27 4164 7661 6e63 6564 2054   the.'Advanced T
-00010eb0: 6f70 6963 7327 2073 6563 7469 6f6e 206f  opics' section o
-00010ec0: 6620 7468 6520 7573 6572 206d 616e 7561  f the user manua
-00010ed0: 6c20 666f 7220 6d6f 7265 2064 6574 6169  l for more detai
-00010ee0: 6c73 2e0a 0a54 6865 2072 656c 6561 7365  ls...The release
-00010ef0: 2061 6c73 6f20 696e 636c 7564 6573 2069   also includes i
-00010f00: 6d70 726f 7665 6420 7375 7070 6f72 7420  mproved support 
-00010f10: 666f 7220 7573 696e 6720 4379 7468 6f6e  for using Cython
-00010f20: 2077 6974 6820 6060 4861 7354 7261 6974   with ``HasTrait
-00010f30: 7360 600a 636c 6173 7365 732c 2073 6f6d  s``.classes, som
-00010f40: 6520 6e65 7720 6865 6c70 6572 2075 7469  e new helper uti
-00010f50: 6c69 7469 6573 2066 6f72 2077 7269 7469  lities for writi
-00010f60: 6e67 2075 6e69 7420 7465 7374 7320 666f  ng unit tests fo
-00010f70: 7220 5472 6169 7473 2065 7665 6e74 732c  r Traits events,
-00010f80: 0a61 6e64 2061 2076 6172 6965 7479 206f  .and a variety o
-00010f90: 6620 6275 6720 6669 7865 732c 2073 7461  f bug fixes, sta
-00010fa0: 6269 6c69 7479 2065 6e68 616e 6365 6d65  bility enhanceme
-00010fb0: 6e74 732c 2061 6e64 2069 6e74 6572 6e61  nts, and interna
-00010fc0: 6c20 636f 6465 0a69 6d70 726f 7665 6d65  l code.improveme
-00010fd0: 6e74 732e 0a0a 0a43 6861 6e67 6520 7375  nts....Change su
-00010fe0: 6d6d 6172 7920 7369 6e63 6520 342e 332e  mmary since 4.3.
-00010ff0: 300a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  0.~~~~~~~~~~~~~~
-00011000: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4e65  ~~~~~~~~~~~~..Ne
-00011010: 7720 6665 6174 7572 6573 0a0a 2a20 5468  w features..* Th
-00011020: 6520 6164 6170 7461 7469 6f6e 206d 6563  e adaptation mec
-00011030: 6861 6e69 736d 2069 6e20 5472 6169 7473  hanism in Traits
-00011040: 2c20 666f 726d 6572 6c79 2062 6173 6564  , formerly based
-00011050: 206f 6e20 7468 6520 2774 7261 6974 732e   on the 'traits.
-00011060: 7072 6f74 6f63 6f6c 7327 0a20 2070 6163  protocols'.  pac
-00011070: 6b61 6765 2c20 6861 7320 6265 656e 2072  kage, has been r
-00011080: 6570 6c61 6365 6420 7769 7468 2074 6865  eplaced with the
-00011090: 206d 6f72 6520 726f 6275 7374 2027 7472   more robust 'tr
-000110a0: 6169 7473 2e61 6461 7074 6174 696f 6e27  aits.adaptation'
-000110b0: 0a20 2070 6163 6b61 6765 2e20 2823 3531  .  package. (#51
-000110c0: 290a 2a20 4164 6465 6420 7574 696c 6974  ).* Added utilit
-000110d0: 7920 6675 6e63 7469 6f6e 2066 6f72 2069  y function for i
-000110e0: 6d70 6f72 7469 6e67 2073 796d 626f 6c73  mporting symbols
-000110f0: 2028 6e61 6d65 2c20 636c 6173 7365 732c   (name, classes,
-00011100: 2066 756e 6374 696f 6e73 290a 2020 6279   functions).  by
-00011110: 206e 616d 653a 2027 7472 6169 7473 2e75   name: 'traits.u
-00011120: 7469 6c2e 6170 692e 696d 706f 7274 5f73  til.api.import_s
-00011130: 796d 626f 6c27 2e20 2823 3531 290a 2a20  ymbol'. (#51).* 
-00011140: 5573 6572 7320 6361 6e20 7365 7420 6120  Users can set a 
-00011150: 676c 6f62 616c 2074 7261 6365 722c 2077  global tracer, w
-00011160: 6869 6368 2072 6563 6569 7665 7320 616c  hich receives al
-00011170: 6c20 7472 6169 7473 2063 6861 6e67 6520  l traits change 
-00011180: 6576 656e 7473 3a0a 2020 6060 7472 6169  events:.  ``trai
-00011190: 7473 2e74 7261 6974 5f6e 6f74 6966 6965  ts.trait_notifie
-000111a0: 7273 2e73 6574 5f63 6861 6e67 655f 6576  rs.set_change_ev
-000111b0: 656e 745f 7472 6163 6572 7360 602e 2028  ent_tracers``. (
-000111c0: 2337 3929 0a0a 456e 6861 6e63 656d 656e  #79)..Enhancemen
-000111d0: 7473 0a0a 2a20 5570 6461 7465 2062 656e  ts..* Update ben
-000111e0: 6368 6d61 726b 2073 6372 6970 742e 2028  chmark script. (
-000111f0: 2335 3429 0a2a 2074 7261 6974 732e 7574  #54).* traits.ut
-00011200: 696c 2e64 6570 7265 6361 7465 643a 2075  il.deprecated: u
-00011210: 7365 206d 6f64 756c 6520 6c6f 6767 6572  se module logger
-00011220: 2069 6e73 7465 6164 206f 6620 726f 6f74   instead of root
-00011230: 206c 6f67 6765 722e 2028 2335 3929 0a2a   logger. (#59).*
-00011240: 2050 726f 7669 6465 2061 6e20 696e 666f   Provide an info
-00011250: 726d 6174 6976 6520 6d65 7373 6167 6520  rmative message 
-00011260: 696e 2041 6461 7074 6174 696f 6e45 7272  in AdaptationErr
-00011270: 6f72 2e20 2823 3632 290a 2a20 416c 6c6f  or. (#62).* Allo
-00011280: 7720 4861 7354 7261 6974 7320 636c 6173  w HasTraits clas
-00011290: 7365 7320 746f 2062 6520 6379 7468 6f6e  ses to be cython
-000112a0: 697a 6564 2e20 2823 3733 290a 2a20 496d  ized. (#73).* Im
-000112b0: 7072 6f76 6520 7465 7374 7320 666f 7220  prove tests for 
-000112c0: 6379 7468 6f6e 697a 6174 696f 6e20 7375  cythonization su
-000112d0: 7070 6f72 742e 2028 2337 3529 0a2a 2045  pport. (#75).* E
-000112e0: 7874 656e 6469 6e67 2076 6172 696f 7573  xtending various
-000112f0: 2074 7261 6974 2074 6573 7469 6e67 2068   trait testing h
-00011300: 656c 7065 7273 2028 2335 3329 0a0a 5265  elpers (#53)..Re
-00011310: 6661 6374 6f72 696e 670a 0a2a 2054 6865  factoring..* The
-00011320: 2054 7261 6974 7320 6e6f 7469 6669 6361   Traits notifica
-00011330: 7469 6f6e 2063 6f64 6520 6861 7320 6265  tion code has be
-00011340: 656e 2072 6577 6f72 6b65 6420 746f 2072  en reworked to r
-00011350: 656d 6f76 6520 636f 6465 2064 7570 6c69  emove code dupli
-00011360: 6361 7469 6f6e 2c0a 2020 616e 6420 7465  cation,.  and te
-00011370: 7374 2063 6f76 6572 6167 6520 6f66 2074  st coverage of t
-00011380: 6861 7420 636f 6465 2068 6173 2062 6565  hat code has bee
-00011390: 6e20 7369 676e 6966 6963 616e 746c 7920  n significantly 
-000113a0: 696d 7072 6f76 6564 2e20 2823 3739 290a  improved. (#79).
-000113b0: 0a46 6978 6573 0a0a 2a20 4669 7820 7261  .Fixes..* Fix ra
-000113c0: 6365 2063 6f6e 6469 7469 6f6e 2077 6865  ce condition whe
-000113d0: 6e20 7265 6d6f 7669 6e67 2061 2074 7261  n removing a tra
-000113e0: 6974 7320 6c69 7374 656e 6572 2e20 2823  its listener. (#
-000113f0: 3537 290a 2a20 4669 7820 7567 6c79 2069  57).* Fix ugly i
-00011400: 6e74 6572 6163 7469 6f6e 2062 6574 7765  nteraction betwe
-00011410: 656e 2044 656c 6567 6174 6573 546f 2063  en DelegatesTo c
-00011420: 6861 6e67 6520 6861 6e64 6c65 7273 2c20  hange handlers, 
-00011430: 6479 6e61 6d69 6320 6368 616e 6765 0a20  dynamic change. 
-00011440: 2068 616e 646c 6572 7320 616e 6420 7477   handlers and tw
-00011450: 6f20 6c65 7665 6c73 206f 6620 6479 6e61  o levels of dyna
-00011460: 6d69 6320 696e 6974 6961 6c69 7a61 7469  mic initializati
-00011470: 6f6e 2e20 2823 3633 290a 2a20 5573 6520  on. (#63).* Use 
-00011480: 6120 4e75 6c6c 4861 6e64 6c65 7220 666f  a NullHandler fo
-00011490: 7220 616c 6c20 2774 7261 6974 7327 206c  r all 'traits' l
-000114a0: 6f67 6765 7273 2e20 2823 3634 290a 2a20  oggers. (#64).* 
-000114b0: 4669 7820 7261 6365 2063 6f6e 6469 7469  Fix race conditi
-000114c0: 6f6e 2069 6e20 5472 6169 7443 6861 6e67  on in TraitChang
-000114d0: 654e 6f74 6966 7957 7261 7070 6572 2e6c  eNotifyWrapper.l
-000114e0: 6973 7465 6e65 725f 6465 6c65 7465 6420  istener_deleted 
-000114f0: 2823 3636 290a 2a20 4669 7820 6c65 616b  (#66).* Fix leak
-00011500: 696e 6720 6e6f 7469 6669 6572 732e 2028  ing notifiers. (
-00011510: 2336 3829 0a2a 2046 6978 2066 6169 6c69  #68).* Fix faili
-00011520: 6e67 2073 7065 6369 616c 2069 6e73 7461  ng special insta
-00011530: 6e63 6520 7472 6169 7420 6576 656e 7473  nce trait events
-00011540: 2e20 2823 3738 290a 2a20 4669 7820 6869  . (#78).* Fix hi
-00011550: 6469 6e67 204b 6579 4572 726f 7220 6578  ding KeyError ex
-00011560: 6365 7074 696f 6e20 696e 7369 6465 2074  ception inside t
-00011570: 7261 6974 2064 6566 6175 6c74 2069 6e69  rait default ini
-00011580: 7469 616c 697a 6520 6d65 7468 6f64 2e0a  tialize method..
-00011590: 2020 2823 3831 290a 2a20 4669 7820 4164    (#81).* Fix Ad
-000115a0: 6170 7465 7220 6f62 6a65 6374 2069 6e69  apter object ini
-000115b0: 7469 616c 697a 6174 696f 6e2e 2028 2339  tialization. (#9
-000115c0: 3329 0a2a 2046 6978 2063 7963 6c69 6320  3).* Fix cyclic 
-000115d0: 6761 7262 6167 6520 6172 6973 696e 6720  garbage arising 
-000115e0: 6672 6f6d 2075 7365 206f 6620 7468 6520  from use of the 
-000115f0: 5765 616b 5265 6620 7472 6169 7420 7479  WeakRef trait ty
-00011600: 7065 2e20 2823 3935 290a 2a20 6060 5472  pe. (#95).* ``Tr
-00011610: 6169 7453 6574 4f62 6a65 6374 2e63 6f70  aitSetObject.cop
-00011620: 7960 6020 6e6f 7720 7265 7475 726e 7320  y`` now returns 
-00011630: 6120 706c 6169 6e20 7261 7468 6572 2074  a plain rather t
-00011640: 6861 6e20 616e 0a20 2075 6e69 6e69 7469  han an.  uniniti
-00011650: 616c 697a 6564 2060 6054 7261 6974 5365  alized ``TraitSe
-00011660: 744f 626a 6563 7460 6020 696e 7374 616e  tObject`` instan
-00011670: 6365 2e20 2823 3937 290a 2a20 4669 7820  ce. (#97).* Fix 
-00011680: 6379 636c 6963 2067 6172 6261 6765 2061  cyclic garbage a
-00011690: 7269 7369 6e67 2066 726f 6d20 6479 6e61  rising from dyna
-000116a0: 6d69 6320 7472 6169 7420 6368 616e 6765  mic trait change
-000116b0: 2068 616e 646c 6572 732e 2028 2331 3031   handlers. (#101
-000116c0: 290a 0a0a 5265 6c65 6173 6573 2034 2e33  )...Releases 4.3
-000116d0: 2e30 202d 2033 2e36 2e30 0a2d 2d2d 2d2d  .0 - 3.6.0.-----
-000116e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000116f0: 2d0a 0a43 6861 6e67 656c 6f67 7320 756e  -..Changelogs un
-00011700: 6176 6169 6c61 626c 652e 0a0a 0a52 656c  available....Rel
-00011710: 6561 7365 2033 2e35 2e30 0a2d 2d2d 2d2d  ease 3.5.0.-----
-00011720: 2d2d 2d2d 2d2d 2d2d 0a0a 5265 6c65 6173  --------..Releas
-00011730: 6564 3a20 3230 3130 2d31 302d 3135 0a0a  ed: 2010-10-15..
-00011740: 456e 6861 6e63 656d 656e 7473 0a0a 2a20  Enhancements..* 
-00011750: 6164 6469 6e67 2073 7570 706f 7274 2066  adding support f
-00011760: 6f72 2064 726f 702d 646f 776e 206d 656e  or drop-down men
-00011770: 7520 696e 2042 7574 746f 6e20 7472 6169  u in Button trai
-00011780: 7473 2c20 6275 7420 6f6e 6c79 2066 6f72  ts, but only for
-00011790: 2071 7420 6261 636b 656e 640a 2a20 6164   qt backend.* ad
-000117a0: 6469 6e67 2027 7368 6f77 5f6e 6f74 6562  ding 'show_noteb
-000117b0: 6f6f 6b5f 6d65 6e75 2720 6f70 7469 6f6e  ook_menu' option
-000117c0: 2074 6f20 4c69 7374 4564 6974 6f72 2073   to ListEditor s
-000117d0: 6f20 7468 6174 2074 6865 2075 7365 7220  o that the user 
-000117e0: 6361 6e0a 2020 7269 6768 742d 636c 6963  can.  right-clic
-000117f0: 6b20 616e 6420 7368 6f77 206f 7220 6869  k and show or hi
-00011800: 6465 2074 6865 2063 6f6e 7465 7874 206d  de the context m
-00011810: 656e 7520 2851 7429 0a2a 2061 6464 6564  enu (Qt).* added
-00011820: 2073 656c 6563 7469 6f6e 2072 616e 6765   selection range
-00011830: 2074 7261 6974 7320 746f 206d 616b 6520   traits to make 
-00011840: 6974 2070 6f73 7369 626c 6520 666f 7220  it possible for 
-00011850: 7573 6572 7320 746f 2072 6570 6c61 6365  users to replace
-00011860: 0a20 2073 656c 6563 7465 6420 7465 7874  .  selected text
-00011870: 0a0a 4669 7865 730a 0a2a 2066 6978 6564  ..Fixes..* fixed
-00011880: 206e 756c 6c20 636f 6c6f 7220 6564 6974   null color edit
-00011890: 6f72 2074 6f20 776f 726b 2077 6974 6820  or to work with 
-000118a0: 7475 706c 6573 0a2a 2062 7567 2077 6865  tuples.* bug whe
-000118b0: 6e20 6f70 656e 696e 6720 6120 7669 6577  n opening a view
-000118c0: 2077 6974 6820 7468 6520 546f 6f6c 6261   with the Toolba
-000118d0: 7242 7574 746f 6e0a 0a0a 5265 6c65 6173  rButton...Releas
-000118e0: 6520 332e 342e 300a 2d2d 2d2d 2d2d 2d2d  e 3.4.0.--------
-000118f0: 2d2d 2d2d 2d0a 0a52 656c 6561 7365 643a  -----..Released:
-00011900: 2032 3031 302d 3035 2d32 360a 0a45 6e68   2010-05-26..Enh
-00011910: 616e 6365 6d65 6e74 730a 0a2a 2061 6464  ancements..* add
-00011920: 696e 6720 6e65 7720 6578 616d 706c 6520  ing new example 
-00011930: 746f 206d 616b 6520 7465 7374 696e 6720  to make testing 
-00011940: 7267 6220 636f 6c6f 7220 6564 6974 6f72  rgb color editor
-00011950: 2065 6173 6965 720a 0a46 6978 6573 0a0a   easier..Fixes..
-00011960: 2a20 6669 7865 6420 4e75 6d65 7269 6343  * fixed NumericC
-00011970: 6f6c 756d 6e20 746f 206e 6f74 2065 7870  olumn to not exp
-00011980: 6563 7420 6f62 6a65 6374 2074 6f20 6861  ect object to ha
-00011990: 7665 206d 6f64 656c 5f73 656c 6563 7469  ve model_selecti
-000119a0: 6f6e 2061 7474 7269 6275 7465 2c0a 2020  on attribute,.  
-000119b0: 616e 6420 7265 6d6f 7665 6420 6d6f 7265  and removed more
-000119c0: 2064 6561 6420 7468 656d 696e 6720 636f   dead theming co
-000119d0: 6465 0a2a 2066 6978 6564 2041 5049 2062  de.* fixed API b
-000119e0: 7567 7320 7769 7468 2074 6865 204e 756d  ugs with the Num
-000119f0: 6572 6963 436f 6c75 6d6e 2077 6865 7265  ericColumn where
-00011a00: 2069 7473 2066 756e 6374 696f 6e20 7369   its function si
-00011a10: 676e 6174 7572 6573 0a20 2064 6966 6665  gnatures.  diffe
-00011a20: 7265 6420 6672 6f6d 2069 7473 2062 6173  red from its bas
-00011a30: 6520 636c 6173 732c 2062 7574 2074 6865  e class, but the
-00011a40: 2063 616c 6c69 6e67 2063 6f64 6520 6578   calling code ex
-00011a50: 7065 6374 6564 2074 6865 6d20 746f 2061  pected them to a
-00011a60: 6c6c 0a20 2062 6520 7468 6520 7361 6d65  ll.  be the same
-00011a70: 0a2a 2066 6978 6564 2062 7567 2077 6869  .* fixed bug whi
-00011a80: 6368 2077 6173 2072 656c 6174 6564 2074  ch was related t
-00011a90: 6f20 7479 7065 206e 616d 6520 6572 726f  o type name erro
-00011aa0: 7273 2063 6175 7365 6420 7768 656e 2072  rs caused when r
-00011ab0: 756e 6e69 6e67 2053 7068 696e 780a 2a20  unning Sphinx.* 
-00011ac0: 7768 656e 2075 7369 6e67 2046 696c 6528  when using File(
-00011ad0: 6578 6973 7473 3d54 7275 6529 2c20 6265  exists=True), be
-00011ae0: 2073 7572 6520 746f 2076 616c 6964 6174   sure to validat
-00011af0: 6520 7468 6520 7479 7065 206f 6620 7468  e the type of th
-00011b00: 6520 7661 6c75 650a 2020 6669 7273 7420  e value.  first 
-00011b10: 6265 666f 7265 2075 7369 6e67 206f 732e  before using os.
-00011b20: 7061 7468 2e69 7366 696c 6528 290a 0a0a  path.isfile()...
-00011b30: 5265 6c65 6173 6520 332e 332e 300a 2d2d  Release 3.3.0.--
-00011b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 656c  -----------..Rel
-00011b50: 6561 7365 643a 2032 3031 302d 3032 2d32  eased: 2010-02-2
-00011b60: 340a 0a45 6e68 616e 6365 6d65 6e74 730a  4..Enhancements.
-00011b70: 0a54 6865 206d 616a 6f72 2065 6e68 616e  .The major enhan
-00011b80: 6365 6d65 6e74 2074 6869 7320 7265 6c65  cement this rele
-00011b90: 6173 6520 6973 2074 6861 7420 7468 6520  ase is that the 
-00011ba0: 656e 7469 7265 2054 7261 6974 7320 7061  entire Traits pa
-00011bb0: 636b 6167 6520 6861 7320 6265 656e 0a63  ckage has been.c
-00011bc0: 6861 6e67 6564 2074 6f20 7573 6520 7265  hanged to use re
-00011bd0: 6c61 7469 7665 2069 6d70 6f72 7473 2073  lative imports s
-00011be0: 6f20 7468 6174 2069 7420 6361 6e20 6265  o that it can be
-00011bf0: 2069 6e73 7461 6c6c 6564 2061 7320 6120   installed as a 
-00011c00: 7375 622d 7061 636b 6167 650a 696e 7369  sub-package.insi
-00011c10: 6465 2061 6e6f 7468 6572 206c 6172 6765  de another large
-00011c20: 7220 6c69 6272 6172 7920 6f72 2070 6163  r library or pac
-00011c30: 6b61 6765 2e20 2054 6869 7320 7761 7320  kage.  This was 
-00011c40: 6e6f 7420 7072 6576 696f 7573 6c79 2070  not previously p
-00011c50: 6f73 7369 626c 652c 0a73 696e 6365 2074  ossible,.since t
-00011c60: 6865 2076 6172 696f 7573 206d 6f64 756c  he various modul
-00011c70: 6573 2069 6e73 6964 6520 5472 6169 7473  es inside Traits
-00011c80: 2077 6f75 6c64 2069 6d70 6f72 7420 6561   would import ea
-00011c90: 6368 206f 7468 6572 2064 6972 6563 746c  ch other directl
-00011ca0: 790a 7468 726f 7567 6820 2274 7261 6974  y.through "trait
-00011cb0: 732e 5b6d 6f64 756c 655d 222e 2020 4d61  s.[module]".  Ma
-00011cc0: 6e79 2074 6861 6e6b 7320 746f 2044 6172  ny thanks to Dar
-00011cd0: 7265 6e20 4461 6c65 2066 6f72 2074 6865  ren Dale for the
-00011ce0: 0a70 6174 6368 2e0a 0a46 6978 6573 0a0a  .patch...Fixes..
-00011cf0: 5468 6572 6520 6861 7665 2062 6565 6e20  There have been 
-00011d00: 6e75 6d65 726f 7573 206d 696e 6f72 2062  numerous minor b
-00011d10: 7567 6669 7865 7320 7369 6e63 6520 7468  ugfixes since th
-00011d20: 6520 6c61 7374 2072 656c 6561 7365 2e20  e last release. 
-00011d30: 2054 6865 206d 6f73 7420 6e6f 7461 626c   The most notabl
-00011d40: 650a 6f6e 6573 2061 7265 3a0a 0a2a 204d  e.ones are:..* M
-00011d50: 616e 7920 6669 7865 7320 696e 766f 6c76  any fixes involv
-00011d60: 6520 6d61 6b69 6e67 2054 7261 6974 7320  e making Traits 
-00011d70: 5549 206d 6f72 6520 726f 6275 7374 2069  UI more robust i
-00011d80: 6620 7778 5079 7468 6f6e 2069 7320 6e6f  f wxPython is no
-00011d90: 7420 696e 7374 616c 6c65 640a 2020 6f6e  t installed.  on
-00011da0: 2061 2073 7973 7465 6d2e 2020 496e 2074   a system.  In t
-00011db0: 6865 2070 6173 742c 2077 6520 6861 7665  he past, we have
-00011dc0: 2062 6565 6e20 6162 6c65 2074 6f20 7573   been able to us
-00011dd0: 6520 5174 2069 6620 6974 2077 6173 2061  e Qt if it was a
-00011de0: 6c73 6f0a 2020 696e 7374 616c 6c65 642c  lso.  installed,
-00011df0: 2062 7574 2072 656d 6f76 696e 6720 5778   but removing Wx
-00011e00: 2077 6f75 6c64 206c 6561 6420 746f 2061   would lead to a
-00011e10: 2076 6172 6965 7479 206f 6620 6c69 7474   variety of litt
-00011e20: 6c65 2062 7567 7320 696e 2076 6172 696f  le bugs in vario
-00011e30: 7573 0a20 2070 6c61 6365 732e 2020 5765  us.  places.  We
-00011e40: 2776 6520 7371 7561 7368 6564 2061 206e  've squashed a n
-00011e50: 756d 6265 7220 6f66 2074 6865 7365 2e20  umber of these. 
-00011e60: 2057 6527 7665 2061 6c73 6f20 6164 6465   We've also adde
-00011e70: 6420 6265 7474 6572 2063 6865 636b 730a  d better checks.
-00011e80: 2020 746f 206d 616b 6520 7375 7265 2077    to make sure w
-00011e90: 6527 7265 2073 656c 6563 7469 6e67 2074  e're selecting t
-00011ea0: 6865 2072 6967 6874 2074 6f6f 6c6b 6974  he right toolkit
-00011eb0: 2061 7420 696d 706f 7274 2061 6e64 2061   at import and a
-00011ec0: 7420 7275 6e74 696d 652e 0a2a 2041 206e  t runtime..* A n
-00011ed0: 6173 7479 2063 7963 6c69 6320 7265 6665  asty cyclic refe
-00011ee0: 7265 6e63 6520 7761 7320 6469 7363 6f76  rence was discov
-00011ef0: 6572 6564 2061 6e64 2065 6c69 6d69 6e61  ered and elimina
-00011f00: 7465 6420 696e 2044 656c 6567 6174 6573  ted in Delegates
-00011f10: 546f 2074 7261 6974 732e 0a2a 2054 6865  To traits..* The
-00011f20: 2055 6e64 6566 696e 6564 2061 6e64 2055   Undefined and U
-00011f30: 6e69 6e69 7469 616c 697a 6564 2054 7261  ninitialized Tra
-00011f40: 6974 7320 7765 7265 206d 6164 6520 696e  its were made in
-00011f50: 746f 2074 7275 6520 7369 6e67 6c65 746f  to true singleto
-00011f60: 6e73 2e0a 2a20 4d75 6368 206f 6620 7468  ns..* Much of th
-00011f70: 6520 696e 636f 6e73 6973 7465 6e74 2066  e inconsistent f
-00011f80: 6f72 6d61 7474 696e 6720 6163 726f 7373  ormatting across
-00011f90: 2074 6865 2065 6e74 6972 6520 5472 6169   the entire Trai
-00011fa0: 7473 2073 6f75 7263 6520 6861 730a 2020  ts source has.  
-00011fb0: 6265 656e 2065 6c69 6d69 6e61 7465 6420  been eliminated 
-00011fc0: 616e 6420 6e6f 726d 616c 697a 6564 2028  and normalized (
-00011fd0: 7461 6273 2f73 7061 6365 732c 206c 696e  tabs/spaces, lin
-00011fe0: 6520 656e 6469 6e67 7329 2e0a 0a0a 5265  e endings)....Re
-00011ff0: 6c65 6173 6520 332e 322e 300a 2d2d 2d2d  lease 3.2.0.----
-00012000: 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561  ---------..Relea
-00012010: 7365 643a 2032 3030 392d 3037 2d31 350a  sed: 2009-07-15.
-00012020: 0a45 6e68 616e 6365 6d65 6e74 730a 0a2a  .Enhancements..*
-00012030: 2049 6d70 6c65 6d65 6e74 6564 2065 6469   Implemented edi
-00012040: 7461 626c 655f 6c61 6265 6c73 2061 7474  table_labels att
-00012050: 7269 6275 7465 2069 6e20 7468 6520 5461  ribute in the Ta
-00012060: 6275 6c61 7245 6469 746f 7220 666f 7220  bularEditor for 
-00012070: 656e 6162 6c69 6e67 2065 6469 7469 6e67  enabling editing
-00012080: 206f 6620 7468 6520 6c61 6265 6c73 2028   of the labels (
-00012090: 692e 652e 2074 6865 2066 6972 7374 2063  i.e. the first c
-000120a0: 6f6c 756d 6e29 0a2a 2053 6176 696e 672f  olumn).* Saving/
-000120b0: 7265 7374 6f72 696e 6720 7769 6e64 6f77  restoring window
-000120c0: 2070 6f73 6974 696f 6e73 2077 6f72 6b73   positions works
-000120d0: 2077 6974 6820 6d75 6c74 6970 6c65 2064   with multiple d
-000120e0: 6973 706c 6179 7320 6f66 2064 6966 6665  isplays of diffe
-000120f0: 7265 6e74 2073 697a 6573 0a2a 204e 6577  rent sizes.* New
-00012100: 2050 726f 6772 6573 7345 6469 746f 720a   ProgressEditor.
-00012110: 2a20 4368 616e 6765 6420 6465 6661 756c  * Changed defaul
-00012120: 7420 636f 6c6f 7273 2066 6f72 2054 6162  t colors for Tab
-00012130: 6c65 4564 6974 6f72 0a2a 2041 6464 6564  leEditor.* Added
-00012140: 2073 7570 706f 7274 2066 6f72 2048 544d   support for HTM
-00012150: 4c45 6469 746f 7220 666f 7220 5154 2062  LEditor for QT b
-00012160: 6163 6b65 6e64 2075 7369 6e67 2051 7457  ackend using QtW
-00012170: 6562 4b69 740a 2a20 496d 7072 6f76 6564  ebKit.* Improved
-00012180: 2073 7570 706f 7274 2066 6f72 206f 7065   support for ope
-00012190: 6e69 6e67 206c 696e 6b73 2069 6e20 6578  ning links in ex
-000121a0: 7465 726e 616c 2062 726f 7773 6572 2066  ternal browser f
-000121b0: 726f 6d20 4854 4d4c 4564 6974 6f72 0a2a  rom HTMLEditor.*
-000121c0: 2041 6464 6564 2073 7570 706f 7274 2066   Added support f
-000121d0: 6f72 2054 6162 756c 6172 4564 6974 6f72  or TabularEditor
-000121e0: 2066 6f72 2051 5420 6261 636b 656e 640a   for QT backend.
-000121f0: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
-00012200: 666f 7220 6d61 726b 696e 6720 7570 2074  for marking up t
-00012210: 6865 2043 6f64 6545 6469 746f 722c 2069  he CodeEditor, i
-00012220: 6e63 6c75 6469 6e67 2061 6464 696e 6720  ncluding adding 
-00012230: 7371 7569 6767 6c65 7320 616e 6420 6469  squiggles and di
-00012240: 6d6d 696e 6720 6c69 6e65 730a 2a20 4164  mming lines.* Ad
-00012250: 6465 6420 5365 6172 6368 4564 6974 6f72  ded SearchEditor
-00012260: 0a2a 2049 6d70 726f 7665 6420 756e 6963  .* Improved unic
-00012270: 6f64 6520 7375 7070 6f72 740a 2a20 4368  ode support.* Ch
-00012280: 616e 6765 6420 6265 6861 7669 6f72 206f  anged behavior o
-00012290: 6620 5261 6e67 6545 6469 746f 7220 7465  f RangeEditor te
-000122a0: 7874 2062 6f78 2074 6f20 6e6f 7420 6175  xt box to not au
-000122b0: 746f 2d73 6574 0a2a 2041 6464 6564 2073  to-set.* Added s
-000122c0: 7570 706f 7274 2069 6e20 5261 6e67 6545  upport in RangeE
-000122d0: 6469 746f 7220 666f 7220 7370 6563 6966  ditor for specif
-000122e0: 7969 6e67 2074 6865 206d 6574 686f 6420  ying the method 
-000122f0: 746f 2065 7661 6c75 6174 6520 6e65 7720  to evaluate new 
-00012300: 7661 6c75 6573 2e0a 2a20 4164 6420 4465  values..* Add De
-00012310: 6661 756c 744f 7665 7272 6964 6520 6564  faultOverride ed
-00012320: 6974 6f72 2066 6163 746f 7279 2063 6f75  itor factory cou
-00012330: 7274 6573 7920 5374 c3a9 6661 6e20 7661  rtesy St..fan va
-00012340: 6e20 6465 7220 5761 6c74 0a2a 2052 656d  n der Walt.* Rem
-00012350: 6f76 6564 2073 7973 2e65 7869 7428 2920  oved sys.exit() 
-00012360: 6361 6c6c 2066 726f 6d20 5361 7665 4861  call from SaveHa
-00012370: 6e64 6c65 722e 6578 6974 2829 0a         ndler.exit().
+00000070: 6861 7420 6669 7865 7320 6661 696c 696e  hat fixes failin
+00000080: 6720 736f 6d65 2074 6573 7420 6661 696c  g some test fail
+00000090: 7572 6573 2077 6974 6820 7468 650a 6d6f  ures with the.mo
+000000a0: 7374 2072 6563 656e 7420 5472 6169 7473  st recent Traits
+000000b0: 5549 2076 6572 7369 6f6e 732e 0a0a 4669  UI versions...Fi
+000000c0: 7865 730a 7e7e 7e7e 7e0a 2a20 5265 706c  xes.~~~~~.* Repl
+000000d0: 6163 6520 6120 6465 7072 6563 6174 6564  ace a deprecated
+000000e0: 2076 6572 7369 6f6e 2063 6865 636b 2066   version check f
+000000f0: 6f72 2054 7261 6974 7355 492e 2028 2331  or TraitsUI. (#1
+00000100: 3734 3629 0a2a 2046 6978 2061 2074 6573  746).* Fix a tes
+00000110: 7420 7468 6174 2066 6169 6c73 206f 6e20  t that fails on 
+00000120: 7761 726e 696e 6773 206f 7468 6572 2074  warnings other t
+00000130: 6861 6e20 7468 6f73 6520 6469 7265 6374  han those direct
+00000140: 6c79 2072 656c 6174 6564 2074 6f0a 2020  ly related to.  
+00000150: 7468 6520 7465 7374 2070 7572 706f 7365  the test purpose
+00000160: 2e20 2823 3137 3439 290a 0a0a 5265 6c65  . (#1749)...Rele
+00000170: 6173 6520 362e 342e 310a 2d2d 2d2d 2d2d  ase 6.4.1.------
+00000180: 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561 7365  -------..Release
+00000190: 643a 2032 3032 322d 3038 2d31 320a 0a54  d: 2022-08-12..T
+000001a0: 6869 7320 6973 2061 2062 7567 6669 7820  his is a bugfix 
+000001b0: 7265 6c65 6173 6520 7468 6174 2066 6978  release that fix
+000001c0: 6573 2077 6865 656c 2062 7569 6c64 7320  es wheel builds 
+000001d0: 6f6e 2050 7974 686f 6e20 332e 3131 2061  on Python 3.11 a
+000001e0: 6e64 0a66 6978 6573 2073 6f6d 6520 6469  nd.fixes some di
+000001f0: 7374 7269 6275 7469 6f6e 2061 6e64 2074  stribution and t
+00000200: 6573 7469 6e67 2069 7373 7565 7320 7769  esting issues wi
+00000210: 7468 2074 7970 696e 6720 7374 7562 732e  th typing stubs.
+00000220: 0a0a 4669 7865 730a 7e7e 7e7e 7e0a 2a20  ..Fixes.~~~~~.* 
+00000230: 5570 6461 7465 2060 6063 6962 7569 6c64  Update ``cibuild
+00000240: 7768 6565 6c60 6020 746f 2074 6865 206c  wheel`` to the l
+00000250: 6174 6573 7420 7665 7273 696f 6e20 736f  atest version so
+00000260: 2074 6861 7420 7765 2067 6574 2077 6865   that we get whe
+00000270: 656c 7320 666f 720a 2020 5079 7468 6f6e  els for.  Python
+00000280: 2033 2e31 312e 2028 2331 3731 3129 0a2a   3.11. (#1711).*
+00000290: 2052 656e 616d 6520 6060 7265 7175 6972   Rename ``requir
+000002a0: 6573 5f6e 756d 7079 5f74 6573 7469 6e67  es_numpy_testing
+000002b0: 6060 2064 6563 6f72 6174 6f72 2074 6f20  `` decorator to 
+000002c0: 6060 7265 7175 6972 6573 5f6e 756d 7079  ``requires_numpy
+000002d0: 5f74 7970 696e 6760 602c 0a20 2061 6e64  _typing``,.  and
+000002e0: 2068 6176 6520 6974 2063 6865 636b 2066   have it check f
+000002f0: 6f72 2060 606e 756d 7079 2e74 7970 696e  or ``numpy.typin
+00000300: 6760 602c 206e 6f74 2060 606e 756d 7079  g``, not ``numpy
+00000310: 2e74 6573 7469 6e67 6060 2e20 2823 3137  .testing``. (#17
+00000320: 3130 290a 2a20 4669 7820 6d69 7373 696e  10).* Fix missin
+00000330: 6720 6060 6e75 6d70 795f 6578 616d 706c  g ``numpy_exampl
+00000340: 6573 6060 2064 6972 6563 746f 7279 2069  es`` directory i
+00000350: 6e20 7472 6169 7473 2d73 7475 6273 2070  n traits-stubs p
+00000360: 6163 6b61 6765 2064 6174 612e 0a20 2028  ackage data..  (
+00000370: 2331 3730 3929 0a0a 0a52 656c 6561 7365  #1709)...Release
+00000380: 2036 2e34 2e30 0a2d 2d2d 2d2d 2d2d 2d2d   6.4.0.---------
+00000390: 2d2d 2d2d 0a0a 5265 6c65 6173 6564 3a20  ----..Released: 
+000003a0: 3230 3232 2d30 382d 3132 0a0a 5472 6169  2022-08-12..Trai
+000003b0: 7473 2036 2e34 2069 7320 6120 6d69 6e6f  ts 6.4 is a mino
+000003c0: 7220 6665 6174 7572 6520 7265 6c65 6173  r feature releas
+000003d0: 6520 6f66 2054 7261 6974 732c 2077 6869  e of Traits, whi
+000003e0: 6368 2066 6f63 7573 6573 206d 6169 6e6c  ch focuses mainl
+000003f0: 7920 6f6e 2074 7970 696e 670a 7374 7562  y on typing.stub
+00000400: 2061 6e64 2064 6f63 756d 656e 7461 7469   and documentati
+00000410: 6f6e 2075 7064 6174 6573 2e0a 0a4d 6967  on updates...Mig
+00000420: 7261 7469 6e67 2066 726f 6d20 5472 6169  rating from Trai
+00000430: 7473 2036 2e33 0a7e 7e7e 7e7e 7e7e 7e7e  ts 6.3.~~~~~~~~~
+00000440: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00000450: 0a0a 5472 6169 7473 2036 2e34 2073 686f  ..Traits 6.4 sho
+00000460: 756c 6420 6265 206c 6172 6765 6c79 2062  uld be largely b
+00000470: 6163 6b77 6172 6473 2063 6f6d 7061 7469  ackwards compati
+00000480: 626c 6520 7769 7468 2054 7261 6974 7320  ble with Traits 
+00000490: 362e 332c 2062 7574 2074 6865 7265 0a61  6.3, but there.a
+000004a0: 7265 2061 2063 6f75 706c 6520 6f66 2074  re a couple of t
+000004b0: 6869 6e67 7320 746f 2077 6174 6368 206f  hings to watch o
+000004c0: 7574 2066 6f72 2e0a 0a2a 2052 656d 696e  ut for...* Remin
+000004d0: 6465 723a 2077 6869 6c65 2074 6865 2060  der: while the `
+000004e0: 6045 6974 6865 7260 6020 616e 6420 6060  `Either`` and ``
+000004f0: 5472 6169 7460 6020 7472 6169 7420 7479  Trait`` trait ty
+00000500: 7065 7320 6172 6520 6e6f 7420 7965 7420  pes are not yet 
+00000510: 666f 726d 616c 6c79 0a20 2064 6570 7265  formally.  depre
+00000520: 6361 7465 642c 2074 6865 2069 6e74 656e  cated, the inten
+00000530: 7469 6f6e 2069 7320 746f 2065 7665 6e74  tion is to event
+00000540: 7561 6c6c 7920 6465 7072 6563 6174 6520  ually deprecate 
+00000550: 616e 6420 7265 6d6f 7665 2074 6865 6d2e  and remove them.
+00000560: 0a20 2050 726f 6a65 6374 7320 6172 6520  .  Projects are 
+00000570: 656e 636f 7572 6167 6564 2074 6f20 7570  encouraged to up
+00000580: 6461 7465 2074 6865 6972 2063 6f64 6520  date their code 
+00000590: 746f 2075 7365 2060 6055 6e69 6f6e 6060  to use ``Union``
+000005a0: 2069 6e73 7465 6164 2e0a 2a20 5369 6d69   instead..* Simi
+000005b0: 6c61 726c 792c 2061 6e79 2075 7365 7320  larly, any uses 
+000005c0: 6f66 2074 6865 2060 6055 6e69 636f 6465  of the ``Unicode
+000005d0: 6060 2074 7261 6974 2074 7970 6520 696e  `` trait type in
+000005e0: 2079 6f75 7220 7072 6f6a 6563 7420 7368   your project sh
+000005f0: 6f75 6c64 0a20 2062 6520 7265 706c 6163  ould.  be replac
+00000600: 6564 2077 6974 6820 6060 5374 7260 602e  ed with ``Str``.
+00000610: 0a2a 2056 616c 6964 6174 696f 6e20 6f66  .* Validation of
+00000620: 2069 7465 6d73 2077 6974 6869 6e20 6120   items within a 
+00000630: 636f 6e74 6169 6e65 7220 2865 2e67 2e2c  container (e.g.,
+00000640: 2060 6066 6f6f 7320 3d20 4c69 7374 284d   ``foos = List(M
+00000650: 7954 7261 6974 5479 7065 2960 6029 0a20  yTraitType)``). 
+00000660: 206e 6f77 2061 6c77 6179 7320 6d61 7463   now always matc
+00000670: 6865 7320 7468 6520 7661 6c69 6461 7469  hes the validati
+00000680: 6f6e 2075 7365 6420 666f 7220 7468 6520  on used for the 
+00000690: 6974 656d 2074 7261 6974 2061 7420 746f  item trait at to
+000006a0: 7020 6c65 7665 6c20 2865 2e67 2e2c 0a20  p level (e.g.,. 
+000006b0: 2060 6066 6f6f 203d 204d 7954 7261 6974   ``foo = MyTrait
+000006c0: 5479 7065 6060 292e 2050 7265 7669 6f75  Type``). Previou
+000006d0: 736c 792c 2074 6865 2076 616c 6964 6174  sly, the validat
+000006e0: 696f 6e20 6d65 7468 6f64 7320 7573 6564  ion methods used
+000006f0: 2063 6f75 6c64 2064 6966 6665 722c 0a20   could differ,. 
+00000700: 2074 6861 6e6b 7320 746f 2061 2062 7567   thanks to a bug
+00000710: 2069 6e20 7468 6520 636f 6e74 6169 6e65   in the containe
+00000720: 7220 696d 706c 656d 656e 7461 7469 6f6e  r implementation
+00000730: 732e 2046 6f72 206d 6f73 7420 7472 6169  s. For most trai
+00000740: 7420 7479 7065 7320 7468 6973 0a20 2077  t types this.  w
+00000750: 696c 6c20 6d61 6b65 206e 6f20 6469 6666  ill make no diff
+00000760: 6572 656e 6365 2c20 6275 7420 666f 7220  erence, but for 
+00000770: 7468 6520 6060 5475 706c 6560 6020 7472  the ``Tuple`` tr
+00000780: 6169 7420 7479 7065 2074 6869 7320 6368  ait type this ch
+00000790: 616e 6765 2068 6173 2074 6865 0a20 2063  ange has the.  c
+000007a0: 6f6e 7365 7175 656e 6365 2074 6861 7420  onsequence that 
+000007b0: 6c69 7374 7320 7769 6c6c 206e 6f20 6c6f  lists will no lo
+000007c0: 6e67 6572 2062 6520 6163 6365 7074 6564  nger be accepted
+000007d0: 2061 7320 7661 6c69 6420 666f 7220 6060   as valid for ``
+000007e0: 5475 706c 6560 600a 2020 7472 6169 7473  Tuple``.  traits
+000007f0: 2069 6e73 6964 6520 6c69 7374 2069 7465   inside list ite
+00000800: 6d73 2e20 5365 6520 6973 7375 6520 2331  ms. See issue #1
+00000810: 3631 3920 616e 6420 5052 2023 3136 3235  619 and PR #1625
+00000820: 2066 6f72 206d 6f72 6520 696e 666f 726d   for more inform
+00000830: 6174 696f 6e2e 0a2a 2052 656c 6174 6564  ation..* Related
+00000840: 2074 6f20 7468 6520 6162 6f76 653a 2061   to the above: a
+00000850: 2074 6f70 2d6c 6576 656c 2060 6054 7570   top-level ``Tup
+00000860: 6c65 2829 6060 2074 7261 6974 2064 6563  le()`` trait dec
+00000870: 6c61 7261 7469 6f6e 2063 7572 7265 6e74  laration current
+00000880: 6c79 0a20 2061 6363 6570 7473 2050 7974  ly.  accepts Pyt
+00000890: 686f 6e20 6060 6c69 7374 6060 206f 626a  hon ``list`` obj
+000008a0: 6563 7473 2c20 7768 696c 6520 6120 6060  ects, while a ``
+000008b0: 5475 706c 6560 6020 6465 636c 6172 6174  Tuple`` declarat
+000008c0: 696f 6e20 7769 7468 2065 7870 6c69 6369  ion with explici
+000008d0: 740a 2020 6974 656d 2074 7970 6573 2028  t.  item types (
+000008e0: 666f 7220 6578 616d 706c 6520 6060 5475  for example ``Tu
+000008f0: 706c 6528 496e 7428 292c 2049 6e74 2829  ple(Int(), Int()
+00000900: 2960 6029 2064 6f65 7320 6e6f 742e 2054  )``) does not. T
+00000910: 6865 2073 7570 706f 7274 2066 6f72 0a20  he support for. 
+00000920: 2060 606c 6973 7460 6020 6f62 6a65 6374   ``list`` object
+00000930: 7320 696e 2070 6c61 696e 2060 6054 7570  s in plain ``Tup
+00000940: 6c65 2829 6060 2069 7320 6465 7072 6563  le()`` is deprec
+00000950: 6174 6564 2c20 616e 6420 7769 6c6c 2062  ated, and will b
+00000960: 6520 7265 6d6f 7665 6420 696e 2061 0a20  e removed in a. 
+00000970: 2066 7574 7572 6520 7665 7273 696f 6e20   future version 
+00000980: 6f66 2054 7261 6974 732e 2053 6565 2050  of Traits. See P
+00000990: 5220 2331 3632 3720 666f 7220 6d6f 7265  R #1627 for more
+000009a0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 0a44   information...D
+000009b0: 6574 6169 6c65 6420 5052 2d62 792d 5052  etailed PR-by-PR
+000009c0: 2063 6861 6e67 6573 0a7e 7e7e 7e7e 7e7e   changes.~~~~~~~
+000009d0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+000009e0: 7e7e 0a0a 5468 6520 666f 6c6c 6f77 696e  ~~..The followin
+000009f0: 6720 7065 6f70 6c65 2063 6f6e 7472 6962  g people contrib
+00000a00: 7574 6564 2063 6f64 6520 6368 616e 6765  uted code change
+00000a10: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00000a20: 7365 3a0a 0a2a 2043 6169 6f20 4167 6961  se:..* Caio Agia
+00000a30: 6e69 0a2a 2053 7465 7665 2041 6c6c 656e  ni.* Steve Allen
+00000a40: 0a2a 204d 6172 6b20 4469 636b 696e 736f  .* Mark Dickinso
+00000a50: 6e0a 2a20 5361 6920 5261 6875 6c20 506f  n.* Sai Rahul Po
+00000a60: 7275 7269 0a2a 2043 6f72 7261 6e20 5765  ruri.* Corran We
+00000a70: 6273 7465 720a 0a46 6561 7475 7265 730a  bster..Features.
+00000a80: 7e7e 7e7e 7e7e 7e7e 0a2a 2060 6045 5453  ~~~~~~~~.* ``ETS
+00000a90: 436f 6e66 6967 6060 2061 7474 7269 6275  Config`` attribu
+00000aa0: 7465 7320 6e6f 7720 7375 7070 6f72 7420  tes now support 
+00000ab0: 6465 6c65 7469 6f6e 2e20 5468 6973 206d  deletion. This m
+00000ac0: 616b 6573 2069 7420 6561 7369 6572 2074  akes it easier t
+00000ad0: 6f20 6d61 6b65 0a20 2074 656d 706f 7261  o make.  tempora
+00000ae0: 7279 2063 6861 6e67 6573 2074 6f20 6060  ry changes to ``
+00000af0: 4554 5343 6f6e 6669 6760 6020 6174 7472  ETSConfig`` attr
+00000b00: 6962 7574 6573 2064 7572 696e 6720 756e  ibutes during un
+00000b10: 6974 2074 6573 7469 6e67 2e20 2823 3136  it testing. (#16
+00000b20: 3730 2c0a 2020 2331 3638 3629 0a2a 2060  70,.  #1686).* `
+00000b30: 6043 6f6d 706c 6578 6060 2074 7261 6974  `Complex`` trait
+00000b40: 2074 7970 6520 7661 6c69 6461 7469 6f6e   type validation
+00000b50: 2069 7320 6e6f 7720 6d6f 7265 206c 656e   is now more len
+00000b60: 6965 6e74 3a20 616e 7920 7479 7065 2074  ient: any type t
+00000b70: 6861 740a 2020 696d 706c 656d 656e 7473  hat.  implements
+00000b80: 2060 605f 5f63 6f6d 706c 6578 5f5f 6060   ``__complex__``
+00000b90: 2077 696c 6c20 6265 2061 6363 6570 7465   will be accepte
+00000ba0: 642e 2028 2331 3539 3429 0a2a 2060 6042  d. (#1594).* ``B
+00000bb0: 6173 6546 6c6f 6174 6060 2076 616c 6964  aseFloat`` valid
+00000bc0: 6174 696f 6e20 6973 206e 6f77 206d 6f72  ation is now mor
+00000bd0: 6520 6c65 6e69 656e 742c 2061 6e64 206d  e lenient, and m
+00000be0: 6174 6368 6573 2060 6046 6c6f 6174 6060  atches ``Float``
+00000bf0: 0a20 2076 616c 6964 6174 696f 6e3a 2060  .  validation: `
+00000c00: 6042 6173 6546 6c6f 6174 6060 206e 6f77  `BaseFloat`` now
+00000c10: 2061 6c73 6f20 6163 6365 7074 7320 6f62   also accepts ob
+00000c20: 6a65 6374 7320 7768 6f73 6520 7479 7065  jects whose type
+00000c30: 2068 6173 2061 6e0a 2020 6060 5f5f 696e   has an.  ``__in
+00000c40: 6465 785f 5f60 6020 6d65 7468 6f64 2e20  dex__`` method. 
+00000c50: 2823 3135 3935 290a 0a43 6861 6e67 6573  (#1595)..Changes
+00000c60: 0a7e 7e7e 7e7e 7e7e 0a2a 2041 6e20 6060  .~~~~~~~.* An ``
+00000c70: 656e 756d 6572 6174 6560 6020 616c 6961  enumerate`` alia
+00000c80: 7320 6861 7320 6265 656e 2072 656d 6f76  s has been remov
+00000c90: 6564 2066 726f 6d20 6060 7472 6169 7473  ed from ``traits
+00000ca0: 2e74 7261 6974 5f62 6173 6560 602e 2049  .trait_base``. I
+00000cb0: 6e20 7468 650a 2020 756e 6c69 6b65 6c79  n the.  unlikely
+00000cc0: 2065 7665 6e74 206f 6620 636f 6465 2074   event of code t
+00000cd0: 6861 7420 696d 706f 7274 7320 6060 656e  hat imports ``en
+00000ce0: 756d 6572 6174 6560 6020 6672 6f6d 2060  umerate`` from `
+00000cf0: 6074 7261 6974 732e 7472 6169 745f 6261  `traits.trait_ba
+00000d00: 7365 6060 2c0a 2020 7573 6520 7468 6520  se``,.  use the 
+00000d10: 6275 696c 742d 696e 2060 6065 6e75 6d65  built-in ``enume
+00000d20: 7261 7465 6060 2069 6e73 7465 6164 2e20  rate`` instead. 
+00000d30: 2823 3136 3831 290a 2a20 4661 7374 2076  (#1681).* Fast v
+00000d40: 616c 6964 6174 696f 6e20 7475 706c 6573  alidation tuples
+00000d50: 2060 6069 6e74 5f66 6173 745f 7661 6c69   ``int_fast_vali
+00000d60: 6461 7465 6060 2c20 6060 666c 6f61 745f  date``, ``float_
+00000d70: 6661 7374 5f76 616c 6964 6174 6560 6020  fast_validate`` 
+00000d80: 616e 640a 2020 6060 636f 6d70 6c65 785f  and.  ``complex_
+00000d90: 6661 7374 5f76 616c 6964 6174 6560 6020  fast_validate`` 
+00000da0: 6861 7665 2062 6565 6e20 7265 6d6f 7665  have been remove
+00000db0: 6420 6672 6f6d 2074 6865 2060 6074 7261  d from the ``tra
+00000dc0: 6974 732e 7472 6169 745f 7479 7065 7360  its.trait_types`
+00000dd0: 600a 2020 6d6f 6475 6c65 2e20 2823 3136  `.  module. (#16
+00000de0: 3031 290a 0a46 6978 6573 0a7e 7e7e 7e7e  01)..Fixes.~~~~~
+00000df0: 0a2a 2060 6054 7261 6974 4c69 7374 4f62  .* ``TraitListOb
+00000e00: 6a65 6374 6060 2c20 6060 5472 6169 7444  ject``, ``TraitD
+00000e10: 6963 7460 6020 6f62 6a65 6374 2061 6e64  ict`` object and
+00000e20: 2060 6054 7261 6974 5365 744f 626a 6563   ``TraitSetObjec
+00000e30: 7460 6020 6e6f 7720 7573 6520 7468 650a  t`` now use the.
+00000e40: 2020 6060 7661 6c69 6461 7465 6060 206d    ``validate`` m
+00000e50: 6574 686f 6420 6f66 2074 6865 2061 7070  ethod of the app
+00000e60: 726f 7072 6961 7465 2060 6043 5472 6169  ropriate ``CTrai
+00000e70: 7460 6020 696e 7374 616e 6365 7320 746f  t`` instances to
+00000e80: 2076 616c 6964 6174 650a 2020 6974 656d   validate.  item
+00000e90: 732c 206b 6579 7320 616e 6420 7661 6c75  s, keys and valu
+00000ea0: 6573 2e20 5072 6576 696f 7573 6c79 2074  es. Previously t
+00000eb0: 6865 2068 616e 646c 6572 2773 2060 6076  he handler's ``v
+00000ec0: 616c 6964 6174 6560 6020 6d65 7468 6f64  alidate`` method
+00000ed0: 2077 6173 0a20 2075 7365 643b 2074 6869   was.  used; thi
+00000ee0: 7320 6761 7665 2062 7567 6779 2062 6568  s gave buggy beh
+00000ef0: 6176 696f 7572 2069 6e20 6361 7365 7320  aviour in cases 
+00000f00: 7768 6572 6520 7468 6520 6861 6e64 6c65  where the handle
+00000f10: 7227 7320 6060 7661 6c69 6461 7465 6060  r's ``validate``
+00000f20: 0a20 206d 6574 686f 6420 6469 6666 6572  .  method differ
+00000f30: 6564 2066 726f 6d20 7468 6520 6163 7475  ed from the actu
+00000f40: 616c 2076 616c 6964 6174 696f 6e20 696e  al validation in
+00000f50: 2075 7365 2e20 2823 3136 3235 290a 2a20   use. (#1625).* 
+00000f60: 4669 7820 7370 6563 6966 6963 6174 696f  Fix specificatio
+00000f70: 6e20 6f66 2060 6064 6566 6175 6c74 5f76  n of ``default_v
+00000f80: 616c 7565 6060 2074 6861 7420 696e 636f  alue`` that inco
+00000f90: 7272 6563 746c 7920 6469 7372 6567 6172  rrectly disregar
+00000fa0: 6465 640a 2020 6060 6465 6661 756c 745f  ded.  ``default_
+00000fb0: 7661 6c75 655f 7479 7065 6060 2e20 2823  value_type``. (#
+00000fc0: 3136 3331 290a 2a20 4669 7820 696e 636f  1631).* Fix inco
+00000fd0: 7272 6563 7420 7265 7375 6c74 7320 6672  rrect results fr
+00000fe0: 6f6d 2020 6060 636c 6f6e 655f 7472 6169  om  ``clone_trai
+00000ff0: 7473 6060 2061 7070 6c69 6564 2074 6f20  ts`` applied to 
+00001000: 6060 4c69 7374 6060 2c20 6060 4469 6374  ``List``, ``Dict
+00001010: 6060 0a20 2061 6e64 2060 6053 6574 6060  ``.  and ``Set``
+00001020: 2074 7261 6974 732e 2028 2331 3632 3429   traits. (#1624)
+00001030: 0a2a 2054 6865 2060 6066 696e 645f 7265  .* The ``find_re
+00001040: 736f 7572 6365 6060 2061 6e64 2060 6073  source`` and ``s
+00001050: 746f 7265 5f72 6573 6f75 7263 6560 6020  tore_resource`` 
+00001060: 7465 7374 7320 6172 6520 6e6f 7720 736b  tests are now sk
+00001070: 6970 7065 640a 2020 6966 2074 6865 2060  ipped.  if the `
+00001080: 6070 6b67 5f72 6573 6f75 7263 6573 6060  `pkg_resources``
+00001090: 206d 6f64 756c 6520 6973 206e 6f74 2070   module is not p
+000010a0: 7265 7365 6e74 2069 6e20 7468 6520 656e  resent in the en
+000010b0: 7669 726f 6e6d 656e 742e 2028 2331 3637  vironment. (#167
+000010c0: 3929 0a2a 2041 6e20 6060 4554 5343 6f6e  9).* An ``ETSCon
+000010d0: 6669 6760 6020 7465 7374 2068 6173 2062  fig`` test has b
+000010e0: 6565 6e20 7265 6e61 6d65 6420 736f 2074  een renamed so t
+000010f0: 6861 7420 6974 2773 2070 726f 7065 726c  hat it's properl
+00001100: 7920 7069 636b 6564 2075 700a 2020 6279  y picked up.  by
+00001110: 2074 6865 2074 6573 7420 7275 6e6e 6572   the test runner
+00001120: 2e20 2823 3136 3731 290a 2a20 4669 7820  . (#1671).* Fix 
+00001130: 736f 6d65 2060 6045 5453 436f 6e66 6967  some ``ETSConfig
+00001140: 6060 2074 6573 7473 2074 6861 7420 6173  `` tests that as
+00001150: 7375 6d65 2075 6e69 7474 6573 7420 6173  sume unittest as
+00001160: 2074 6865 2074 6573 7420 7275 6e6e 6572   the test runner
+00001170: 2e20 2823 3136 3833 290a 2a20 5265 6e61  . (#1683).* Rena
+00001180: 6d65 2076 6172 696f 7573 2074 6573 742d  me various test-
+00001190: 7265 6c61 7465 6420 636c 6173 7365 7320  related classes 
+000011a0: 746f 2061 766f 6964 2070 7974 6573 7420  to avoid pytest 
+000011b0: 7472 7969 6e67 2074 6f20 6861 7276 6573  trying to harves
+000011c0: 7420 7465 7374 0a20 206d 6574 686f 6473  t test.  methods
+000011d0: 2066 726f 6d20 7468 656d 2e20 2823 3136   from them. (#16
+000011e0: 3834 290a 2a20 4f76 6572 7269 6469 6e67  84).* Overriding
+000011f0: 2061 2064 6566 6175 6c74 2066 6f72 2061   a default for a
+00001200: 2060 604c 6973 7460 6020 6f72 206f 7468   ``List`` or oth
+00001210: 6572 2063 6f6c 6c65 6374 696f 6e20 7472  er collection tr
+00001220: 6169 7420 696e 2061 2073 7562 636c 6173  ait in a subclas
+00001230: 730a 2020 6e6f 7720 776f 726b 7320 6173  s.  now works as
+00001240: 2065 7870 6563 7465 642e 2050 7265 7669   expected. Previ
+00001250: 6f75 736c 792c 2074 6865 2062 6568 6176  ously, the behav
+00001260: 696f 7572 2077 6173 2075 6e75 7361 626c  iour was unusabl
+00001270: 7920 6275 6767 792e 2028 2331 3634 3529  y buggy. (#1645)
+00001280: 0a0a 4465 7072 6563 6174 696f 6e73 0a7e  ..Deprecations.~
+00001290: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 2a20 6060  ~~~~~~~~~~~.* ``
+000012a0: 5475 706c 6560 6020 7472 6169 7473 2063  Tuple`` traits c
+000012b0: 7572 7265 6e74 6c79 2061 6363 6570 7420  urrently accept 
+000012c0: 5079 7468 6f6e 2060 606c 6973 7460 6020  Python ``list`` 
+000012d0: 6f62 6a65 6374 7320 696e 2073 6f6d 6520  objects in some 
+000012e0: 2862 7574 0a20 206e 6f74 2061 6c6c 2920  (but.  not all) 
+000012f0: 6369 7263 756d 7374 616e 6365 732e 2054  circumstances. T
+00001300: 6861 7420 6665 6174 7572 6520 6973 2064  hat feature is d
+00001310: 6570 7265 6361 7465 642c 2061 6e64 2077  eprecated, and w
+00001320: 696c 6c20 6265 2072 656d 6f76 6564 0a20  ill be removed. 
+00001330: 2069 6e20 6120 6675 7475 7265 2076 6572   in a future ver
+00001340: 7369 6f6e 206f 6620 5472 6169 7473 2e20  sion of Traits. 
+00001350: 2823 3136 3237 290a 0a54 7970 6520 7374  (#1627)..Type st
+00001360: 7562 730a 7e7e 7e7e 7e7e 7e7e 7e7e 0a2a  ubs.~~~~~~~~~~.*
+00001370: 2041 6464 2073 7475 6273 2066 6f72 2060   Add stubs for `
+00001380: 6041 7272 6179 6060 2c20 6060 4172 7261  `Array``, ``Arra
+00001390: 794f 724e 6f6e 6560 602c 2061 6e64 2060  yOrNone``, and `
+000013a0: 6043 4172 7261 7960 602e 2028 2331 3638  `CArray``. (#168
+000013b0: 3229 0a2a 2046 6978 2076 6172 696f 7573  2).* Fix various
+000013c0: 2073 7475 6273 2066 6f72 2060 6074 7261   stubs for ``tra
+000013d0: 6974 732e 7472 6169 745f 7479 7065 7360  its.trait_types`
+000013e0: 603b 2061 6464 2073 7475 6273 2066 6f72  `; add stubs for
+000013f0: 0a20 2060 6074 7261 6974 732e 6374 7261  .  ``traits.ctra
+00001400: 6974 7360 602e 2028 2331 3636 3129 0a2a  its``. (#1661).*
+00001410: 2046 6978 2074 6861 7420 6060 5472 6169   Fix that ``Trai
+00001420: 7445 7272 6f72 6060 2073 7475 6273 2077  tError`` stubs w
+00001430: 6572 656e 2774 2065 7870 6f73 6564 2061  eren't exposed a
+00001440: 7420 6060 7472 6169 7473 2e61 7069 6060  t ``traits.api``
+00001450: 206c 6576 656c 2e0a 2020 2823 3136 3538   level..  (#1658
+00001460: 290a 2a20 4d61 6b65 2060 6049 6e74 6060  ).* Make ``Int``
+00001470: 2061 6e64 2060 6046 6c6f 6174 6060 2074   and ``Float`` t
+00001480: 7970 6520 7374 7562 7320 6d6f 7265 2061  ype stubs more a
+00001490: 6363 7572 6174 652e 2028 2331 3635 3629  ccurate. (#1656)
+000014a0: 0a2a 2046 6978 2069 6e63 6f72 7265 6374  .* Fix incorrect
+000014b0: 2074 7970 6520 7374 7562 7320 666f 7220   type stubs for 
+000014c0: 7468 6520 6060 4469 6374 6060 2074 7261  the ``Dict`` tra
+000014d0: 6974 2074 7970 652e 2028 2331 3635 3529  it type. (#1655)
+000014e0: 0a0a 446f 6375 6d65 6e74 6174 696f 6e0a  ..Documentation.
+000014f0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 2a20  ~~~~~~~~~~~~~.* 
+00001500: 4d61 6b65 2060 6045 5453 436f 6e66 6967  Make ``ETSConfig
+00001510: 6060 2063 6c61 7373 2064 6f63 756d 656e  `` class documen
+00001520: 7461 7469 6f6e 2076 6973 6962 6c65 2069  tation visible i
+00001530: 6e20 7468 6520 4150 4920 646f 6373 2e20  n the API docs. 
+00001540: 2823 3136 3838 290a 2a20 4164 6420 636f  (#1688).* Add co
+00001550: 7079 2062 7574 746f 6e73 2074 6f20 636f  py buttons to co
+00001560: 6465 2073 616d 706c 6573 2069 6e20 646f  de samples in do
+00001570: 6375 6d65 6e74 6174 696f 6e2e 2028 2331  cumentation. (#1
+00001580: 3635 312c 2023 3136 3533 290a 2a20 446f  651, #1653).* Do
+00001590: 6375 6d65 6e74 2060 6044 6174 6560 602c  cument ``Date``,
+000015a0: 2060 6044 6174 6574 696d 6560 6020 616e   ``Datetime`` an
+000015b0: 6420 6060 5469 6d65 6060 2074 7261 6974  d ``Time`` trait
+000015c0: 2074 7970 6573 2e20 2823 3136 3431 290a   types. (#1641).
+000015d0: 2a20 4669 7820 736f 6d65 206d 6973 7369  * Fix some missi
+000015e0: 6e67 206d 656e 7469 6f6e 7320 6f66 2060  ng mentions of `
+000015f0: 6053 6574 6060 2069 6e20 6e6f 7469 6669  `Set`` in notifi
+00001600: 6361 7469 6f6e 2064 6f63 732e 2028 2331  cation docs. (#1
+00001610: 3631 3829 0a2a 2044 6f63 756d 656e 7420  618).* Document 
+00001620: 7468 6520 6060 2773 6f6d 655f 7472 6169  the ``'some_trai
+00001630: 742e 2d27 6060 2070 6174 7465 726e 2066  t.-'`` pattern f
+00001640: 6f72 2060 606f 6e5f 7472 6169 745f 6368  or ``on_trait_ch
+00001650: 616e 6765 6060 2e20 2823 3135 3932 290a  ange``. (#1592).
+00001660: 2a20 446f 6375 6d65 6e74 2074 6861 7420  * Document that 
+00001670: 6060 4569 7468 6572 6060 2073 686f 756c  ``Either`` shoul
+00001680: 6420 6e6f 7420 6265 2075 7365 6420 696e  d not be used in
+00001690: 206e 6577 2063 6f64 652e 2028 2331 3639   new code. (#169
+000016a0: 3929 0a2a 2044 6f63 756d 656e 7420 7468  9).* Document th
+000016b0: 6174 2060 6054 7261 6974 5072 6566 6978  at ``TraitPrefix
+000016c0: 4d61 7060 6020 616e 6420 6060 5472 6169  Map`` and ``Trai
+000016d0: 7450 7265 6669 784c 6973 7460 6020 6172  tPrefixList`` ar
+000016e0: 6520 6465 7072 6563 6174 6564 2e0a 2020  e deprecated..  
+000016f0: 2823 3137 3032 290a 2a20 446f 6375 6d65  (#1702).* Docume
+00001700: 6e74 2074 6861 7420 7468 6520 5472 6169  nt that the Trai
+00001710: 7420 6661 6374 6f72 7920 6675 6e63 7469  t factory functi
+00001720: 6f6e 2073 686f 756c 6420 6e6f 7420 6265  on should not be
+00001730: 2075 7365 6420 696e 206e 6577 2063 6f64   used in new cod
+00001740: 652e 0a20 2028 2331 3730 3029 0a2a 204d  e..  (#1700).* M
+00001750: 6973 6365 6c6c 616e 656f 7573 206d 696e  iscellaneous min
+00001760: 6f72 2066 6978 6573 2e20 2823 3135 3833  or fixes. (#1583
+00001770: 2c20 2331 3631 312c 2023 3136 3532 2c20  , #1611, #1652, 
+00001780: 2331 3638 3029 0a0a 4275 696c 6420 616e  #1680)..Build an
+00001790: 6420 636f 6e74 696e 756f 7573 2069 6e74  d continuous int
+000017a0: 6567 7261 7469 6f6e 0a7e 7e7e 7e7e 7e7e  egration.~~~~~~~
+000017b0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+000017c0: 7e7e 7e7e 7e7e 7e7e 7e0a 2a20 446f 6e27  ~~~~~~~~~.* Don'
+000017d0: 7420 636f 6c6c 6563 7420 7472 6169 7473  t collect traits
+000017e0: 2d73 7475 6273 2074 6573 7473 2075 6e64  -stubs tests und
+000017f0: 6572 2070 7974 6573 742e 2041 7320 6120  er pytest. As a 
+00001800: 7265 7375 6c74 206f 6620 7468 6973 0a20  result of this. 
+00001810: 2061 6e64 206f 7468 6572 2066 6978 6573   and other fixes
+00001820: 2c20 7468 6520 7465 7374 2073 7569 7465  , the test suite
+00001830: 206e 6f77 2070 6173 7365 7320 756e 6465   now passes unde
+00001840: 7220 7079 7465 7374 2e20 2823 3136 3930  r pytest. (#1690
+00001850: 290a 2a20 5570 6461 7465 2060 6065 7473  ).* Update ``ets
+00001860: 746f 6f6c 2e70 7960 6020 666f 7220 5079  tool.py`` for Py
+00001870: 7468 6f6e 2033 2e38 2073 7570 706f 7274  thon 3.8 support
+00001880: 2e20 5079 7468 6f6e 2033 2e38 2069 7320  . Python 3.8 is 
+00001890: 6e6f 7720 7468 650a 2020 6465 6661 756c  now the.  defaul
+000018a0: 7420 5079 7468 6f6e 2076 6572 7369 6f6e  t Python version
+000018b0: 2066 6f72 2062 7569 6c64 732e 2028 2331   for builds. (#1
+000018c0: 3639 3429 0a2a 2055 7365 2050 7953 6964  694).* Use PySid
+000018d0: 6536 2066 6f72 2050 7974 686f 6e20 3e3d  e6 for Python >=
+000018e0: 2033 2e38 2069 6e73 7465 6164 206f 6620   3.8 instead of 
+000018f0: 5079 5369 6465 3220 696e 2043 4920 7465  PySide2 in CI te
+00001900: 7374 696e 672e 2028 2331 3638 3529 0a2a  sting. (#1685).*
+00001910: 2041 6464 2060 6070 7970 726f 6a65 6374   Add ``pyproject
+00001920: 2e74 6f6d 6c60 6020 6669 6c65 7320 666f  .toml`` files fo
+00001930: 7220 626f 7468 2054 7261 6974 7320 616e  r both Traits an
+00001940: 6420 7472 6169 7473 2d73 7475 6273 2e20  d traits-stubs. 
+00001950: 2823 3136 3839 2c20 2331 3637 3629 0a2a  (#1689, #1676).*
+00001960: 2041 6464 2050 7974 686f 6e20 332e 3131   Add Python 3.11
+00001970: 2074 6f20 736f 6d65 2077 6f72 6b66 6c6f   to some workflo
+00001980: 7720 7275 6e73 2e20 2823 3136 3030 2c20  w runs. (#1600, 
+00001990: 2331 3636 302c 2023 3136 3734 290a 2a20  #1660, #1674).* 
+000019a0: 4164 6420 5079 7468 6f6e 2033 2e31 3020  Add Python 3.10 
+000019b0: 746f 2069 6e73 7461 6c6c 2d66 726f 6d2d  to install-from-
+000019c0: 5079 5049 2077 6f72 6b66 6c6f 772e 2028  PyPI workflow. (
+000019d0: 2331 3537 3629 0a2a 2041 6c6c 6f77 2072  #1576).* Allow r
+000019e0: 756e 6e69 6e67 2074 6865 206d 6169 6e20  unning the main 
+000019f0: 7465 7374 2077 6f72 6b66 6c6f 7720 6d61  test workflow ma
+00001a00: 6e75 616c 6c79 2e20 2823 3136 3037 290a  nually. (#1607).
+00001a10: 2a20 5377 6974 6368 2053 6c61 636b 2063  * Switch Slack c
+00001a20: 6861 6e6e 656c 2075 7365 6420 746f 2072  hannel used to r
+00001a30: 6570 6f72 7420 4769 7448 7562 2041 6374  eport GitHub Act
+00001a40: 696f 6e73 2066 6169 6c75 7265 732e 2028  ions failures. (
+00001a50: 2331 3635 3029 0a2a 2045 7863 6c75 6465  #1650).* Exclude
+00001a60: 2060 6062 7569 6c64 6060 2064 6972 6563   ``build`` direc
+00001a70: 746f 7279 2069 6e20 666c 616b 6538 2063  tory in flake8 c
+00001a80: 6f6e 6669 6775 7261 7469 6f6e 2e20 2823  onfiguration. (#
+00001a90: 3136 3335 290a 2a20 5265 2d69 6e63 6c75  1635).* Re-inclu
+00001aa0: 6465 204e 756d 5079 2061 7320 6120 7465  de NumPy as a te
+00001ab0: 7374 2064 6570 656e 6465 6e63 7920 6f6e  st dependency on
+00001ac0: 2050 7974 686f 6e20 332e 3130 2e20 2823   Python 3.10. (#
+00001ad0: 3135 3933 290a 0a4d 6169 6e74 656e 616e  1593)..Maintenan
+00001ae0: 6365 2061 6e64 2072 6566 6163 746f 7269  ce and refactori
+00001af0: 6e67 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ng.~~~~~~~~~~~~~
+00001b00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a2a  ~~~~~~~~~~~~~~.*
+00001b10: 2060 602e 6769 7469 676e 6f72 6560 6020   ``.gitignore`` 
+00001b20: 636c 6561 6e75 7020 616e 6420 7570 6461  cleanup and upda
+00001b30: 7465 732e 2028 2331 3637 382c 2023 3136  tes. (#1678, #16
+00001b40: 3837 290a 2a20 5265 7475 726e 2060 6050  87).* Return ``P
+00001b50: 7945 7272 5f46 6f72 6d61 7460 6020 6361  yErr_Format`` ca
+00001b60: 6c6c 7320 696e 2060 6074 7261 6974 732f  lls in ``traits/
+00001b70: 6374 7261 6974 732e 6360 602e 2028 2331  ctraits.c``. (#1
+00001b80: 3634 3029 0a2a 2055 7064 6174 6520 636f  640).* Update co
+00001b90: 7079 7269 6768 7420 6865 6164 6572 2065  pyright header e
+00001ba0: 6e64 2079 6561 7220 746f 2032 3032 322e  nd year to 2022.
+00001bb0: 2028 2331 3631 3229 0a2a 2054 6865 2060   (#1612).* The `
+00001bc0: 6063 692d 7372 632d 7265 7175 6972 656d  `ci-src-requirem
+00001bd0: 656e 7473 2e74 7874 6060 2066 696c 6520  ents.txt`` file 
+00001be0: 6973 6e27 7420 7573 6564 3b20 7265 6d6f  isn't used; remo
+00001bf0: 7665 2069 742e 2028 2331 3630 3229 0a0a  ve it. (#1602)..
+00001c00: 0a52 656c 6561 7365 2036 2e33 2e32 0a2d  .Release 6.3.2.-
+00001c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5265  ------------..Re
+00001c20: 6c65 6173 6564 3a20 3230 3231 2d31 312d  leased: 2021-11-
+00001c30: 3130 0a0a 5472 6169 7473 2036 2e33 2e32  10..Traits 6.3.2
+00001c40: 2069 7320 6120 6275 6766 6978 2072 656c   is a bugfix rel
+00001c50: 6561 7365 2c20 6669 7869 6e67 2061 6e20  ease, fixing an 
+00001c60: 6973 7375 6520 7769 7468 2064 7570 6c69  issue with dupli
+00001c70: 6361 7465 0a6e 6f74 6966 6963 6174 696f  cate.notificatio
+00001c80: 6e73 2066 726f 6d20 6060 5072 6f70 6572  ns from ``Proper
+00001c90: 7479 6060 2074 7261 6974 7320 7573 696e  ty`` traits usin
+00001ca0: 6720 7468 6520 6060 6f62 7365 7276 6560  g the ``observe`
+00001cb0: 6020 6672 616d 6577 6f72 6b2e 0a0a 0a46  ` framework....F
+00001cc0: 6978 6573 0a7e 7e7e 7e7e 0a0a 2a20 4669  ixes.~~~~~..* Fi
+00001cd0: 7820 7468 6174 2060 6050 726f 7065 7274  x that ``Propert
+00001ce0: 7960 6020 7472 6169 7473 2075 7369 6e67  y`` traits using
+00001cf0: 2060 606f 6273 6572 7665 6060 206d 6574   ``observe`` met
+00001d00: 6164 6174 6120 636f 756c 6420 6265 2066  adata could be f
+00001d10: 6972 6564 0a20 2074 7769 6365 2069 6e20  ired.  twice in 
+00001d20: 7375 6263 6c61 7373 6573 2e20 2823 3135  subclasses. (#15
+00001d30: 3837 290a 0a0a 5265 6c65 6173 6520 362e  87)...Release 6.
+00001d40: 332e 310a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  3.1.------------
+00001d50: 2d0a 0a52 656c 6561 7365 643a 2032 3032  -..Released: 202
+00001d60: 312d 3130 2d31 320a 0a54 7261 6974 7320  1-10-12..Traits 
+00001d70: 362e 332e 3120 6973 2061 2062 7567 6669  6.3.1 is a bugfi
+00001d80: 7820 7265 6c65 6173 652c 2066 6978 696e  x release, fixin
+00001d90: 6720 616e 2069 6e63 6f6d 7061 7469 6269  g an incompatibi
+00001da0: 6c69 7479 2062 6574 7765 656e 0a54 7261  lity between.Tra
+00001db0: 6974 7320 362e 332e 3020 616e 6420 4d61  its 6.3.0 and Ma
+00001dc0: 7961 7669 203c 3d20 342e 372e 332e 0a0a  yavi <= 4.7.3...
+00001dd0: 4669 7865 730a 7e7e 7e7e 7e0a 0a2a 204d  Fixes.~~~~~..* M
+00001de0: 616b 6520 6060 5072 6566 6978 4d61 702e  ake ``PrefixMap.
+00001df0: 5f6d 6170 6060 2061 7661 696c 6162 6c65  _map`` available
+00001e00: 2061 6761 696e 2c20 666f 7220 636f 6d70   again, for comp
+00001e10: 6174 6962 696c 6974 7920 7769 7468 204d  atibility with M
+00001e20: 6179 6176 692e 0a20 2028 2331 3537 3829  ayavi..  (#1578)
+00001e30: 0a0a 0a52 656c 6561 7365 2036 2e33 2e30  ...Release 6.3.0
+00001e40: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
+00001e50: 5265 6c65 6173 6564 3a20 3230 3231 2d31  Released: 2021-1
+00001e60: 302d 3038 0a0a 5472 6169 7473 2036 2e33  0-08..Traits 6.3
+00001e70: 2069 7320 7468 6520 6c61 7465 7374 2066   is the latest f
+00001e80: 6561 7475 7265 2072 656c 6561 7365 2069  eature release i
+00001e90: 6e20 7468 6520 5472 6169 7473 2036 2073  n the Traits 6 s
+00001ea0: 6572 6965 732c 2077 6974 6820 7365 7665  eries, with seve
+00001eb0: 7261 6c0a 696d 7072 6f76 656d 656e 7473  ral.improvements
+00001ec0: 2061 6e64 2066 6978 6573 206f 7665 7220   and fixes over 
+00001ed0: 5472 6169 7473 2036 2e32 2e0a 0a0a 4869  Traits 6.2....Hi
+00001ee0: 6768 6c69 6768 7473 206f 6620 7468 6973  ghlights of this
+00001ef0: 2072 656c 6561 7365 0a7e 7e7e 7e7e 7e7e   release.~~~~~~~
+00001f00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00001f10: 7e7e 7e0a 0a2a 2054 6865 7265 2068 6176  ~~~..* There hav
+00001f20: 6520 6265 656e 2076 6172 696f 7573 206d  e been various m
+00001f30: 696e 6f72 2070 6572 666f 726d 616e 6365  inor performance
+00001f40: 2069 6d70 726f 7665 6d65 6e74 7320 746f   improvements to
+00001f50: 2074 6865 2063 6f72 650a 2020 6060 6f6e   the core.  ``on
+00001f60: 5f74 7261 6974 5f63 6861 6e67 6560 6020  _trait_change`` 
+00001f70: 616e 6420 6060 6f62 7365 7276 6560 6020  and ``observe`` 
+00001f80: 6d61 6368 696e 6572 792e 2054 6865 7365  machinery. These
+00001f90: 206d 6179 2069 6d70 726f 7665 0a20 2073   may improve.  s
+00001fa0: 7461 7274 7570 2074 696d 6520 666f 7220  tartup time for 
+00001fb0: 736f 6d65 2054 7261 6974 732d 7573 696e  some Traits-usin
+00001fc0: 6720 6170 706c 6963 6174 696f 6e73 2e0a  g applications..
+00001fd0: 2a20 5468 6520 6060 6f62 7365 7276 6560  * The ``observe`
+00001fe0: 6020 6d69 6e69 2d6c 616e 6775 6167 6520  ` mini-language 
+00001ff0: 6e6f 7720 6861 7320 696e 2d6c 616e 6775  now has in-langu
+00002000: 6167 6520 7375 7070 6f72 7420 666f 7220  age support for 
+00002010: 6c69 7374 656e 696e 670a 2020 746f 2061  listening.  to a
+00002020: 6c6c 2074 7261 6974 732c 2075 7369 6e67  ll traits, using
+00002030: 2074 6865 2060 602a 6060 2063 6861 7261   the ``*`` chara
+00002040: 6374 6572 2e0a 2a20 5375 7070 6f72 7420  cter..* Support 
+00002050: 666f 7220 5079 7468 6f6e 2033 2e31 3020  for Python 3.10 
+00002060: 6861 7320 6265 656e 2061 6464 6564 2e0a  has been added..
+00002070: 0a0a 4d69 6772 6174 696f 6e20 6775 6964  ..Migration guid
+00002080: 650a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  e.~~~~~~~~~~~~~~
+00002090: 7e0a 0a54 7261 6974 7320 362e 3320 6973  ~..Traits 6.3 is
+000020a0: 2069 6e74 656e 6465 6420 746f 2062 6520   intended to be 
+000020b0: 6675 6c6c 7920 6261 636b 7761 7264 7320  fully backwards 
+000020c0: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+000020d0: 5472 6169 7473 2036 2e32 2c20 616e 640a  Traits 6.2, and.
+000020e0: 6d6f 7374 2070 726f 6a65 6374 7320 7368  most projects sh
+000020f0: 6f75 6c64 2068 6176 6520 6e6f 2064 6966  ould have no dif
+00002100: 6669 6375 6c74 6965 7320 7570 6772 6164  ficulties upgrad
+00002110: 696e 672e 2048 6f77 6576 6572 2c20 796f  ing. However, yo
+00002120: 7520 6d61 7920 7365 650a 736f 6d65 206e  u may see.some n
+00002130: 6577 2064 6570 7265 6361 7469 6f6e 2077  ew deprecation w
+00002140: 6172 6e69 6e67 7320 666f 7220 6578 6973  arnings for exis
+00002150: 7469 6e67 2063 6f64 652c 2077 6172 6e69  ting code, warni
+00002160: 6e67 2061 626f 7574 2062 6568 6176 696f  ng about behavio
+00002170: 7572 0a74 6861 7420 7769 6c6c 2062 6520  ur.that will be 
+00002180: 6368 616e 6765 6420 696e 2054 7261 6974  changed in Trait
+00002190: 7320 372e 302e 2054 6865 7265 2061 7265  s 7.0. There are
+000021a0: 2074 776f 2070 6172 7469 6375 6c61 7220   two particular 
+000021b0: 7365 7473 206f 6620 6368 616e 6765 730a  sets of changes.
+000021c0: 746f 206c 6f6f 6b20 6f75 7420 666f 723a  to look out for:
+000021d0: 0a0a 2a20 5374 6172 7469 6e67 2077 6974  ..* Starting wit
+000021e0: 6820 5472 6169 7473 2037 2e30 2c20 7468  h Traits 7.0, th
+000021f0: 6520 6060 416e 7960 6020 7472 6169 7420  e ``Any`` trait 
+00002200: 7479 7065 2077 696c 6c20 7472 6561 7420  type will treat 
+00002210: 6120 6465 6661 756c 740a 2020 7661 6c75  a default.  valu
+00002220: 6520 6f66 2074 7970 6520 6060 6c69 7374  e of type ``list
+00002230: 6060 206f 7220 6060 6469 6374 6060 2064  `` or ``dict`` d
+00002240: 6966 6665 7265 6e74 6c79 2e20 4375 7272  ifferently. Curr
+00002250: 656e 746c 792c 2069 6e73 7461 6e63 6573  ently, instances
+00002260: 206f 660a 2020 6060 6c69 7374 6060 2061   of.  ``list`` a
+00002270: 6e64 2060 6064 6963 7460 6020 6172 6520  nd ``dict`` are 
+00002280: 7370 6563 6961 6c2d 6361 7365 642c 2061  special-cased, a
+00002290: 6e64 2061 2070 6572 2d69 6e73 7461 6e63  nd a per-instanc
+000022a0: 6520 636f 7079 206f 6620 7468 650a 2020  e copy of the.  
+000022b0: 6465 6661 756c 7420 6973 2070 726f 7669  default is provi
+000022c0: 6465 6420 746f 2065 6163 6820 6060 4861  ded to each ``Ha
+000022d0: 7354 7261 6974 7360 6020 696e 7374 616e  sTraits`` instan
+000022e0: 6365 2e20 496e 2054 7261 6974 7320 372e  ce. In Traits 7.
+000022f0: 302c 2074 6869 730a 2020 7370 6563 6961  0, this.  specia
+00002300: 6c2d 6361 7369 6e67 2077 696c 6c20 6265  l-casing will be
+00002310: 2072 656d 6f76 6564 2c20 616e 6420 7468   removed, and th
+00002320: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+00002330: 7769 6c6c 2062 6520 7368 6172 6564 2062  will be shared b
+00002340: 6574 7765 656e 0a20 2061 6c6c 2069 6e73  etween.  all ins
+00002350: 7461 6e63 6573 2e20 466f 7220 7468 6520  tances. For the 
+00002360: 362e 3320 7265 6c65 6173 6520 6f66 2054  6.3 release of T
+00002370: 7261 6974 732c 2061 2064 6570 7265 6361  raits, a depreca
+00002380: 7469 6f6e 2077 6172 6e69 6e67 2069 7320  tion warning is 
+00002390: 6973 7375 6564 0a20 2077 6865 6e65 7665  issued.  wheneve
+000023a0: 7220 6120 7472 6169 7420 6465 6669 6e69  r a trait defini
+000023b0: 7469 6f6e 206f 6620 7468 6520 666f 726d  tion of the form
+000023c0: 2060 6041 6e79 285b 312c 2032 2c20 335d   ``Any([1, 2, 3]
+000023d0: 2960 6020 6f72 2060 6041 6e79 287b 7d29  )`` or ``Any({})
+000023e0: 6060 0a20 2069 7320 656e 636f 756e 7465  ``.  is encounte
+000023f0: 7265 642e 2055 7365 7273 2063 616e 2072  red. Users can r
+00002400: 6574 6169 6e20 7468 6520 6578 6973 7469  etain the existi
+00002410: 6e67 2062 6568 6176 696f 7572 2061 6e64  ng behaviour and
+00002420: 2073 7570 7072 6573 7320 7468 650a 2020   suppress the.  
+00002430: 7761 726e 696e 6720 6279 2063 6861 6e67  warning by chang
+00002440: 696e 6720 7468 6569 7220 636f 6465 2074  ing their code t
+00002450: 6f20 7573 6520 7468 6520 6e65 7720 6060  o use the new ``
+00002460: 6661 6374 6f72 7960 6020 6172 6775 6d65  factory`` argume
+00002470: 6e74 2074 6f20 7468 650a 2020 6060 416e  nt to the.  ``An
+00002480: 7960 6020 7472 6169 7420 7479 7065 2c20  y`` trait type, 
+00002490: 666f 7220 6578 616d 706c 6520 7265 706c  for example repl
+000024a0: 6163 696e 6720 6120 7472 6169 7420 6465  acing a trait de
+000024b0: 636c 6172 6174 696f 6e20 6060 666f 6f20  claration ``foo 
+000024c0: 3d0a 2020 416e 7928 7b7d 2960 6020 7769  =.  Any({})`` wi
+000024d0: 7468 2060 6066 6f6f 203d 2041 6e79 2866  th ``foo = Any(f
+000024e0: 6163 746f 7279 3d64 6963 7429 6060 2c20  actory=dict)``, 
+000024f0: 616e 6420 6120 7472 6169 7420 6465 636c  and a trait decl
+00002500: 6172 6174 696f 6e20 6060 666f 6f20 3d0a  aration ``foo =.
+00002510: 2020 416e 7928 5b31 2c20 322c 2033 5d29    Any([1, 2, 3])
+00002520: 6060 2077 6974 6820 6060 666f 6f20 3d20  `` with ``foo = 
+00002530: 416e 7928 6661 6374 6f72 793d 6c69 7374  Any(factory=list
+00002540: 2c20 6172 6773 3d28 5b31 2c20 322c 2033  , args=([1, 2, 3
+00002550: 5d2c 2929 6060 2e0a 0a2a 2053 7461 7274  ],))``...* Start
+00002560: 696e 6720 7769 7468 2054 7261 6974 7320  ing with Traits 
+00002570: 372e 302c 2074 6865 2060 6044 6174 6560  7.0, the ``Date`
+00002580: 6020 7472 6169 7420 7479 7065 2077 696c  ` trait type wil
+00002590: 6c20 6e6f 206c 6f6e 6765 7220 6163 6365  l no longer acce
+000025a0: 7074 0a20 2060 6064 6174 6574 696d 6560  pt.  ``datetime`
+000025b0: 6020 696e 7374 616e 6365 7320 6279 2064  ` instances by d
+000025c0: 6566 6175 6c74 2e20 5472 6169 7473 2036  efault. Traits 6
+000025d0: 2e33 2077 696c 6c20 6973 7375 6520 6120  .3 will issue a 
+000025e0: 6465 7072 6563 6174 696f 6e0a 2020 7761  deprecation.  wa
+000025f0: 726e 696e 6720 7768 656e 6576 6572 2061  rning whenever a
+00002600: 2060 6064 6174 6574 696d 6560 6020 696e   ``datetime`` in
+00002610: 7374 616e 6365 2069 7320 6173 7369 676e  stance is assign
+00002620: 6564 2061 7320 6120 7661 6c75 6520 666f  ed as a value fo
+00002630: 720a 2020 6120 6060 4461 7465 6060 2074  r.  a ``Date`` t
+00002640: 7261 6974 2e20 5468 6520 6578 6973 7469  rait. The existi
+00002650: 6e67 2062 6568 6176 696f 7572 2063 616e  ng behaviour can
+00002660: 2062 6520 7072 6573 6572 7665 6420 616e   be preserved an
+00002670: 6420 7468 6520 7761 726e 696e 670a 2020  d the warning.  
+00002680: 7369 6c65 6e63 6564 2062 7920 7573 696e  silenced by usin
+00002690: 6720 6060 4461 7465 2861 6c6c 6f77 5f64  g ``Date(allow_d
+000026a0: 6174 6574 696d 653d 5472 7565 2960 603b  atetime=True)``;
+000026b0: 2061 6c74 6572 6e61 7469 7665 6c79 2c20   alternatively, 
+000026c0: 796f 7520 6361 6e0a 2020 7573 6520 6060  you can.  use ``
+000026d0: 4461 7465 2861 6c6c 6f77 5f64 6174 6574  Date(allow_datet
+000026e0: 696d 653d 4661 6c73 6529 6060 2074 6f20  ime=False)`` to 
+000026f0: 6164 6f70 7420 7468 6520 5472 6169 7473  adopt the Traits
+00002700: 2037 2e30 2062 6568 6176 696f 7572 0a20   7.0 behaviour. 
+00002710: 2072 6967 6874 206e 6f77 2e0a 0a0a 4465   right now....De
+00002720: 7461 696c 6564 2050 522d 6279 2d50 5220  tailed PR-by-PR 
+00002730: 6368 616e 6765 730a 7e7e 7e7e 7e7e 7e7e  changes.~~~~~~~~
+00002740: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00002750: 7e0a 0a4f 7665 7220 3830 2070 756c 6c20  ~..Over 80 pull 
+00002760: 7265 7175 6573 7473 2077 656e 7420 696e  requests went in
+00002770: 746f 2074 6869 7320 7265 6c65 6173 652e  to this release.
+00002780: 2054 6865 2066 6f6c 6c6f 7769 6e67 2070   The following p
+00002790: 656f 706c 6520 636f 6e74 7269 6275 7465  eople contribute
+000027a0: 640a 746f 2074 6865 2072 656c 6561 7365  d.to the release
+000027b0: 3a0a 0a2a 2030 7866 6c6f 7475 730a 2a20  :..* 0xflotus.* 
+000027c0: 4161 726f 6e20 4179 7265 730a 2a20 4b69  Aaron Ayres.* Ki
+000027d0: 7420 4368 6f69 0a2a 204d 6172 6b20 4469  t Choi.* Mark Di
+000027e0: 636b 696e 736f 6e0a 2a20 4368 6967 6f7a  ckinson.* Chigoz
+000027f0: 6965 204e 7269 0a2a 2050 6f72 7572 6920  ie Nri.* Poruri 
+00002800: 5361 6920 5261 6875 6c0a 2a20 436f 7272  Sai Rahul.* Corr
+00002810: 616e 2057 6562 7374 6572 0a2a 204a 6f68  an Webster.* Joh
+00002820: 6e20 5769 6767 696e 730a 2a20 5065 7465  n Wiggins.* Pete
+00002830: 7220 5a61 6865 6d73 7a6b 790a 0a54 6861  r Zahemszky..Tha
+00002840: 6e6b 2079 6f75 2074 6f20 616c 6c20 7768  nk you to all wh
+00002850: 6f20 636f 6e74 7269 6275 7465 6421 0a0a  o contributed!..
+00002860: 0a46 6561 7475 7265 730a 7e7e 7e7e 7e7e  .Features.~~~~~~
+00002870: 7e7e 0a0a 2a20 5468 6520 6060 6f62 7365  ~~..* The ``obse
+00002880: 7276 6560 6020 6d69 6e69 2d6c 616e 6775  rve`` mini-langu
+00002890: 6167 6520 6e6f 7720 7375 7070 6f72 7473  age now supports
+000028a0: 2075 7365 206f 6620 6060 222a 2260 6020   use of ``"*"`` 
+000028b0: 666f 7220 6c69 7374 656e 696e 6720 746f  for listening to
+000028c0: 0a20 2061 6c6c 2074 7261 6974 7320 6f6e  .  all traits on
+000028d0: 2061 2060 6048 6173 5472 6169 7473 6060   a ``HasTraits``
+000028e0: 206f 626a 6563 742e 2043 7572 7265 6e74   object. Current
+000028f0: 6c79 2074 6869 7320 7375 7070 6f72 7420  ly this support 
+00002900: 6973 206c 696d 6974 6564 2074 6f0a 2020  is limited to.  
+00002910: 6361 7365 7320 7768 6572 6520 7468 6520  cases where the 
+00002920: 6060 222a 2260 6020 6170 7065 6172 7320  ``"*"`` appears 
+00002930: 696e 2061 2074 6572 6d69 6e61 6c20 706f  in a terminal po
+00002940: 7369 7469 6f6e 2e20 466f 7220 6578 616d  sition. For exam
+00002950: 706c 652c 0a20 2060 606f 6273 6572 7665  ple,.  ``observe
+00002960: 2822 666f 6f3a 2a22 2960 6020 6973 2073  ("foo:*")`` is s
+00002970: 7570 706f 7274 6564 2c20 6275 7420 6060  upported, but ``
+00002980: 6f62 7365 7276 6528 222a 3a66 6f6f 2229  observe("*:foo")
+00002990: 6060 2069 7320 6e6f 742e 0a20 2028 2331  `` is not..  (#1
+000029a0: 3439 362c 2023 3135 3235 290a 2a20 5468  496, #1525).* Th
+000029b0: 6520 6060 416e 7960 6020 7472 6169 7420  e ``Any`` trait 
+000029c0: 7479 7065 206e 6f77 2073 7570 706f 7274  type now support
+000029d0: 7320 6120 6060 6661 6374 6f72 7960 6020  s a ``factory`` 
+000029e0: 6172 6775 6d65 6e74 2028 7769 7468 2061  argument (with a
+000029f0: 6363 6f6d 7061 6e79 696e 670a 2020 6060  ccompanying.  ``
+00002a00: 6172 6773 6060 2061 6e64 2060 606b 7760  args`` and ``kw`
+00002a10: 6020 6172 6775 6d65 6e74 7329 2e20 5468  ` arguments). Th
+00002a20: 6973 2063 616e 2062 6520 7573 6564 2074  is can be used t
+00002a30: 6f20 7370 6563 6966 7920 6120 7065 722d  o specify a per-
+00002a40: 696e 7374 616e 6365 0a20 2064 6566 6175  instance.  defau
+00002a50: 6c74 2c20 666f 7220 6578 616d 706c 6520  lt, for example 
+00002a60: 7769 7468 2060 6041 6e79 2866 6163 746f  with ``Any(facto
+00002a70: 7279 3d64 6963 7429 6060 2e20 2823 3135  ry=dict)``. (#15
+00002a80: 3537 2c20 2331 3535 3829 0a2a 2054 6865  57, #1558).* The
+00002a90: 2060 6044 6566 6175 6c74 5661 6c75 6560   ``DefaultValue`
+00002aa0: 6020 656e 756d 6572 6174 696f 6e20 6861  ` enumeration ha
+00002ab0: 7320 6120 6e65 7720 6d65 6d62 6572 2060  s a new member `
+00002ac0: 6044 6566 6175 6c74 5661 6c75 652e 6469  `DefaultValue.di
+00002ad0: 7361 6c6c 6f77 6060 0a20 2069 6e74 656e  sallow``.  inten
+00002ae0: 6465 6420 746f 2062 6520 7573 6564 2066  ded to be used f
+00002af0: 6f72 2074 7261 6974 2074 7970 6573 2074  or trait types t
+00002b00: 6861 7420 646f 6e27 7420 6861 7665 2061  hat don't have a
+00002b10: 206d 6561 6e69 6e67 6675 6c20 6465 6661   meaningful defa
+00002b20: 756c 742e 2046 6f72 0a20 2074 7261 6974  ult. For.  trait
+00002b30: 7320 7573 696e 6720 7468 6973 2064 6566  s using this def
+00002b40: 6175 6c74 2076 616c 7565 2074 7970 652c  ault value type,
+00002b50: 2061 6e20 6174 7465 6d70 7420 746f 2072   an attempt to r
+00002b60: 6574 7269 6576 6520 7468 650a 2020 636f  etrieve the.  co
+00002b70: 7272 6573 706f 6e64 696e 6720 6465 6661  rresponding defa
+00002b80: 756c 7420 7573 696e 6720 6060 6465 6661  ult using ``defa
+00002b90: 756c 745f 7661 6c75 655f 666f 7260 6020  ult_value_for`` 
+00002ba0: 7769 6c6c 2072 6169 7365 2060 6056 616c  will raise ``Val
+00002bb0: 7565 4572 726f 7260 602e 0a20 2028 2331  ueError``..  (#1
+00002bc0: 3534 3629 0a2a 2057 6865 6e20 6120 6d65  546).* When a me
+00002bd0: 7468 6f64 2069 7320 6465 636f 7261 7465  thod is decorate
+00002be0: 6420 7769 7468 2061 6e20 6060 6f62 7365  d with an ``obse
+00002bf0: 7276 6560 6020 6465 636f 7261 746f 722c  rve`` decorator,
+00002c00: 2074 6865 206d 6574 686f 640a 2020 7369   the method.  si
+00002c10: 676e 6174 7572 6520 6973 206e 6f77 2063  gnature is now c
+00002c20: 6865 636b 6564 2c20 616e 6420 6120 7761  hecked, and a wa
+00002c30: 726e 696e 6720 6973 7375 6564 2069 6620  rning issued if 
+00002c40: 6974 2064 6f65 736e 2774 206d 6174 6368  it doesn't match
+00002c50: 2074 6865 0a20 2065 7870 6563 7465 6420   the.  expected 
+00002c60: 7369 676e 6174 7572 652e 2054 6869 7320  signature. This 
+00002c70: 7368 6f75 6c64 2063 6174 6368 2074 6865  should catch the
+00002c80: 2063 6f6d 6d6f 6e20 6572 726f 7220 6f66   common error of
+00002c90: 2066 6f72 6765 7474 696e 6720 746f 0a20   forgetting to. 
+00002ca0: 2070 726f 7669 6465 2074 6865 2060 6065   provide the ``e
+00002cb0: 7665 6e74 6060 2070 6172 616d 6574 6572  vent`` parameter
+00002cc0: 2e20 2823 3135 3239 290a 2a20 496e 2060  . (#1529).* In `
+00002cd0: 6045 5453 546f 6f6c 6b69 7460 602c 2074  `ETSToolkit``, t
+00002ce0: 6865 2060 6022 7174 2260 6020 746f 6f6c  he ``"qt"`` tool
+00002cf0: 6b69 7420 6e61 6d65 2069 7320 6e6f 7720  kit name is now 
+00002d00: 7375 7070 6f72 7465 6420 6173 2061 2073  supported as a s
+00002d10: 796e 6f6e 796d 0a20 2066 6f72 2060 6022  ynonym.  for ``"
+00002d20: 7174 3422 6060 2e20 2823 3134 3336 290a  qt4"``. (#1436).
+00002d30: 2a20 5468 6520 6060 4461 7465 6060 2c20  * The ``Date``, 
+00002d40: 6060 4461 7465 7469 6d65 6060 2061 6e64  ``Datetime`` and
+00002d50: 2060 6054 696d 6560 6020 7472 6169 7420   ``Time`` trait 
+00002d60: 7479 7065 7320 6861 7665 2061 206e 6577  types have a new
+00002d70: 2061 7267 756d 656e 740a 2020 6060 616c   argument.  ``al
+00002d80: 6c6f 775f 6e6f 6e65 6060 2e20 496e 2074  low_none``. In t
+00002d90: 6865 2066 7574 7572 652c 2074 6865 7365  he future, these
+00002da0: 2074 7261 6974 2074 7970 6573 2077 696c   trait types wil
+00002db0: 6c20 6e6f 7420 6163 6365 7074 2060 604e  l not accept ``N
+00002dc0: 6f6e 6560 600a 2020 756e 6c65 7373 2060  one``.  unless `
+00002dd0: 6061 6c6c 6f77 5f6e 6f6e 653d 5472 7565  `allow_none=True
+00002de0: 6060 2069 7320 7370 6563 6966 6965 642e  `` is specified.
+00002df0: 2028 2331 3433 3229 0a2a 2054 6865 2060   (#1432).* The `
+00002e00: 6044 6174 6560 6020 7472 6169 7420 7479  `Date`` trait ty
+00002e10: 7065 2068 6173 2061 206e 6577 2061 7267  pe has a new arg
+00002e20: 756d 656e 7420 6060 616c 6c6f 775f 6461  ument ``allow_da
+00002e30: 7465 7469 6d65 6060 2e20 496e 2074 6865  tetime``. In the
+00002e40: 2066 7574 7572 652c 0a20 2060 6064 6174   future,.  ``dat
+00002e50: 6574 696d 6560 6020 696e 7374 616e 6365  etime`` instance
+00002e60: 7320 7769 6c6c 206e 6f74 2062 6520 7661  s will not be va
+00002e70: 6c69 6420 7661 6c75 6573 2066 6f72 2061  lid values for a
+00002e80: 2060 6044 6174 6560 6020 7472 6169 7420   ``Date`` trait 
+00002e90: 756e 6c65 7373 0a20 2060 6061 6c6c 6f77  unless.  ``allow
+00002ea0: 5f64 6174 6574 696d 653d 5472 7565 6060  _datetime=True``
+00002eb0: 2069 7320 7370 6563 6966 6965 642e 2028   is specified. (
+00002ec0: 2331 3432 3929 0a0a 0a50 6572 666f 726d  #1429)...Perform
+00002ed0: 616e 6365 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  ance.~~~~~~~~~~~
+00002ee0: 0a0a 2a20 5468 6520 6060 4f62 7365 7276  ..* The ``Observ
+00002ef0: 6572 4772 6170 6860 6020 696e 7374 616e  erGraph`` instan
+00002f00: 6365 7320 7468 6174 2072 6573 756c 7420  ces that result 
+00002f10: 6672 6f6d 2063 6f6d 7069 6c69 6e67 0a20  from compiling. 
+00002f20: 2060 604f 6273 6572 7665 7245 7870 7265   ``ObserverExpre
+00002f30: 7373 696f 6e60 6020 6f62 6a65 6374 7320  ssion`` objects 
+00002f40: 616e 6420 6f62 7365 7276 6520 6d69 6e69  and observe mini
+00002f50: 2d6c 616e 6775 6167 6520 7374 7269 6e67  -language string
+00002f60: 7320 6172 6520 6e6f 770a 2020 6361 6368  s are now.  cach
+00002f70: 6564 2e20 5468 6973 2073 686f 756c 6420  ed. This should 
+00002f80: 7370 6565 6420 7570 2063 7265 6174 696f  speed up creatio
+00002f90: 6e20 616e 6420 696e 7374 616e 7469 6174  n and instantiat
+00002fa0: 696f 6e20 6f66 2060 6048 6173 5472 6169  ion of ``HasTrai
+00002fb0: 7473 6060 0a20 2073 7562 636c 6173 7365  ts``.  subclasse
+00002fc0: 7320 7468 6174 2069 6e76 6f6c 7665 206c  s that involve l
+00002fd0: 6973 7465 6e69 6e67 2066 6f72 2074 6865  istening for the
+00002fe0: 2073 616d 6520 7061 7474 6572 6e20 696e   same pattern in
+00002ff0: 206d 756c 7469 706c 6520 706c 6163 6573   multiple places
+00003000: 2e0a 2020 2823 3135 3136 2c20 2331 3532  ..  (#1516, #152
+00003010: 3829 0a2a 2054 6865 2065 7175 616c 6974  8).* The equalit
+00003020: 7920 6465 6669 6e69 7469 6f6e 206f 6e20  y definition on 
+00003030: 6060 4f62 7365 7276 6572 4578 7072 6573  ``ObserverExpres
+00003040: 7369 6f6e 6060 2068 6173 2062 6565 6e20  sion`` has been 
+00003050: 7369 6d70 6c69 6669 6564 2e0a 2020 2823  simplified..  (#
+00003060: 3135 3137 290a 2a20 5468 6520 6060 4f62  1517).* The ``Ob
+00003070: 7365 7276 6572 4578 7072 6573 7369 6f6e  serverExpression
+00003080: 6060 2c20 6060 4f62 7365 7276 6572 4772  ``, ``ObserverGr
+00003090: 6170 6860 6020 616e 6420 7265 6c61 7465  aph`` and relate
+000030a0: 640a 2020 636c 6173 7365 7320 6e6f 7720  d.  classes now 
+000030b0: 7573 6520 6060 5f5f 736c 6f74 735f 5f60  use ``__slots__`
+000030c0: 6020 746f 2069 6d70 726f 7665 2073 7065  ` to improve spe
+000030d0: 6564 2061 6e64 206d 656d 6f72 7920 7573  ed and memory us
+000030e0: 652e 2028 2331 3531 332c 2023 3135 3135  e. (#1513, #1515
+000030f0: 290a 2a20 5468 6520 6060 6f6e 5f74 7261  ).* The ``on_tra
+00003100: 6974 5f63 6861 6e67 6560 6020 6d65 7468  it_change`` meth
+00003110: 6f64 2068 6173 2062 6565 6e20 7370 6564  od has been sped
+00003120: 2075 7020 6279 2061 6c6d 6f73 7420 6120   up by almost a 
+00003130: 6661 6374 6f72 206f 6620 7477 6f2c 0a20  factor of two,. 
+00003140: 2062 7920 7265 6d6f 7669 6e67 2075 6e6e   by removing unn
+00003150: 6563 6573 7361 7279 2069 6e74 6572 6e61  ecessary interna
+00003160: 6c20 7573 6167 6520 6f66 2054 7261 6974  l usage of Trait
+00003170: 7320 696e 2074 6865 2070 6172 7369 6e67  s in the parsing
+00003180: 2061 6e64 206c 6973 7465 6e65 720a 2020   and listener.  
+00003190: 6675 6e63 7469 6f6e 616c 6974 792e 2028  functionality. (
+000031a0: 2331 3439 302c 2023 3134 3931 2c20 2331  #1490, #1491, #1
+000031b0: 3439 322c 2023 3134 3933 290a 0a0a 4368  492, #1493)...Ch
+000031c0: 616e 6765 730a 7e7e 7e7e 7e7e 7e0a 0a2a  anges.~~~~~~~..*
+000031d0: 2041 6e20 696e 7661 6c69 6420 7374 6174   An invalid stat
+000031e0: 6963 2064 6566 6175 6c74 2076 616c 7565  ic default value
+000031f0: 2069 6e20 6120 6060 5072 6566 6978 4c69   in a ``PrefixLi
+00003200: 7374 6060 206f 7220 6060 5072 6566 6978  st`` or ``Prefix
+00003210: 4d61 7060 6020 7472 6169 740a 2020 6465  Map`` trait.  de
+00003220: 636c 6172 6174 696f 6e20 6e6f 7720 7261  claration now ra
+00003230: 6973 6573 2060 6056 616c 7565 4572 726f  ises ``ValueErro
+00003240: 7260 6020 7261 7468 6572 2074 6861 6e20  r`` rather than 
+00003250: 6060 5472 6169 7445 7272 6f72 6060 2e20  ``TraitError``. 
+00003260: 2823 3135 3634 290a 2a20 6060 5072 6566  (#1564).* ``Pref
+00003270: 6978 4c69 7374 6060 2061 6e64 2060 6050  ixList`` and ``P
+00003280: 7265 6669 784d 6170 6060 206e 6f20 6c6f  refixMap`` no lo
+00003290: 6e67 6572 2063 6163 6865 2063 6f6d 706c  nger cache compl
+000032a0: 6574 696f 6e73 2e20 2823 3135 3634 290a  etions. (#1564).
+000032b0: 2a20 4120 6661 696c 7572 6520 746f 2070  * A failure to p
+000032c0: 6172 7365 2061 6e20 6060 6f62 7365 7276  arse an ``observ
+000032d0: 6560 6020 6d69 6e69 2d6c 616e 6775 6167  e`` mini-languag
+000032e0: 6520 7374 7269 6e67 206e 6f77 2072 6169  e string now rai
+000032f0: 7365 730a 2020 6060 5661 6c75 6545 7272  ses.  ``ValueErr
+00003300: 6f72 6060 2072 6174 6865 7220 7468 616e  or`` rather than
+00003310: 2060 604c 6172 6b45 7272 6f72 6060 2e20   ``LarkError``. 
+00003320: 2823 3135 3037 290a 2a20 5468 6520 6060  (#1507).* The ``
+00003330: 4e6f 7469 6669 6572 4e6f 7446 6f75 6e64  NotifierNotFound
+00003340: 6060 2065 7863 6570 7469 6f6e 2069 7320  `` exception is 
+00003350: 6e6f 7720 7075 626c 6973 6865 6420 696e  now published in
+00003360: 0a20 2060 6074 7261 6974 732e 6f62 7365  .  ``traits.obse
+00003370: 7276 6174 696f 6e2e 6170 6960 602e 2028  rvation.api``. (
+00003380: 2331 3439 3829 0a2a 2041 6e20 6174 7465  #1498).* An atte
+00003390: 6d70 7420 746f 2061 6363 6573 7320 6120  mpt to access a 
+000033a0: 6e6f 6e65 7869 7374 656e 7420 2264 756e  nonexistent "dun
+000033b0: 6465 7222 2061 7474 7269 6275 7465 2028  der" attribute (
+000033c0: 616e 2061 7474 7269 6275 7465 2077 686f  an attribute who
+000033d0: 7365 0a20 206e 616d 6520 7374 6172 7473  se.  name starts
+000033e0: 2061 6e64 2065 6e64 7320 7769 7468 2022   and ends with "
+000033f0: 5f5f 2229 206f 6e20 6120 6060 4354 7261  __") on a ``CTra
+00003400: 6974 6060 2069 6e73 7461 6e63 6520 7769  it`` instance wi
+00003410: 6c6c 206e 6f77 2072 6169 7365 0a20 2060  ll now raise.  `
+00003420: 6041 7474 7269 6275 7465 4572 726f 7260  `AttributeError`
+00003430: 602e 2050 7265 7669 6f75 736c 792c 2069  `. Previously, i
+00003440: 7420 776f 756c 6420 7265 7475 726e 2060  t would return `
+00003450: 604e 6f6e 6560 602e 2028 2331 3436 392c  `None``. (#1469,
+00003460: 2023 3134 3734 2c0a 2020 2331 3437 3729   #1474,.  #1477)
+00003470: 0a0a 0a44 6570 7265 6361 7469 6f6e 730a  ...Deprecations.
+00003480: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20  ~~~~~~~~~~~~..* 
+00003490: 5468 6520 6060 416e 7960 6020 7472 6169  The ``Any`` trai
+000034a0: 7420 7479 7065 2063 7572 7265 6e74 6c79  t type currently
+000034b0: 2069 6d70 6c69 6369 746c 7920 6d61 6b65   implicitly make
+000034c0: 7320 6120 7065 722d 6060 4861 7354 7261  s a per-``HasTra
+000034d0: 6974 7360 602d 696e 7374 616e 6365 0a20  its``-instance. 
+000034e0: 2063 6f70 7920 6f66 2074 6865 2064 6566   copy of the def
+000034f0: 6175 6c74 2076 616c 7565 2069 6620 7468  ault value if th
+00003500: 6174 2076 616c 7565 2069 7320 616e 2069  at value is an i
+00003510: 6e73 7461 6e63 6520 6f66 2065 6974 6865  nstance of eithe
+00003520: 7220 6060 6c69 7374 6060 206f 720a 2020  r ``list`` or.  
+00003530: 6060 6469 6374 6060 2e20 5468 6973 2062  ``dict``. This b
+00003540: 6568 6176 696f 7572 2069 7320 6465 7072  ehaviour is depr
+00003550: 6563 6174 6564 2c20 616e 6420 7769 6c6c  ecated, and will
+00003560: 2062 6520 7265 6d6f 7665 6420 696e 2054   be removed in T
+00003570: 7261 6974 7320 372e 302e 0a20 2046 6f72  raits 7.0..  For
+00003580: 2061 2070 6572 2d69 6e73 7461 6e63 6520   a per-instance 
+00003590: 6465 6661 756c 742c 2075 7365 2074 6865  default, use the
+000035a0: 206e 6577 2060 6066 6163 746f 7279 6060   new ``factory``
+000035b0: 2061 7267 756d 656e 7420 746f 2060 6041   argument to ``A
+000035c0: 6e79 6060 0a20 2069 6e73 7465 6164 2e20  ny``.  instead. 
+000035d0: 2823 3135 3438 2c20 2331 3533 3229 0a2a  (#1548, #1532).*
+000035e0: 2054 6865 2060 6044 6174 6560 602c 2060   The ``Date``, `
+000035f0: 6044 6174 6574 696d 6560 6020 616e 6420  `Datetime`` and 
+00003600: 6060 5469 6d65 6060 2074 7261 6974 2074  ``Time`` trait t
+00003610: 7970 6573 2077 696c 6c20 6e6f 206c 6f6e  ypes will no lon
+00003620: 6765 7220 6163 6365 7074 0a20 2060 604e  ger accept.  ``N
+00003630: 6f6e 6560 6020 6173 2061 2076 616c 6964  one`` as a valid
+00003640: 2074 7261 6974 2076 616c 7565 2069 6e20   trait value in 
+00003650: 7468 6520 6675 7475 7265 2e20 546f 206b  the future. To k
+00003660: 6565 7020 7468 6520 6578 6973 7469 6e67  eep the existing
+00003670: 0a20 2062 6568 6176 696f 7572 2c20 7573  .  behaviour, us
+00003680: 6520 7468 6520 6e65 7720 6060 616c 6c6f  e the new ``allo
+00003690: 775f 6e6f 6e65 6060 206b 6579 776f 7264  w_none`` keyword
+000036a0: 2061 7267 756d 656e 7420 746f 2074 6865   argument to the
+000036b0: 7365 2074 7261 6974 2074 7970 6573 2e0a  se trait types..
+000036c0: 2020 2823 3134 3434 290a 2a20 5468 6520    (#1444).* The 
+000036d0: 6060 4461 7465 6060 2074 7261 6974 2074  ``Date`` trait t
+000036e0: 7970 6520 7769 6c6c 206e 6f20 6c6f 6e67  ype will no long
+000036f0: 6572 2061 6363 6570 7420 6060 6461 7465  er accept ``date
+00003700: 7469 6d65 6060 2069 6e73 7461 6e63 6573  time`` instances
+00003710: 2062 790a 2020 6465 6661 756c 7420 696e   by.  default in
+00003720: 2074 6865 2066 7574 7572 652e 2054 6f20   the future. To 
+00003730: 6b65 6570 2074 6865 2065 7869 7374 696e  keep the existin
+00003740: 6720 6265 6861 7669 6f75 722c 2075 7365  g behaviour, use
+00003750: 2074 6865 206e 6577 0a20 2060 6061 6c6c   the new.  ``all
+00003760: 6f77 5f64 6174 6574 696d 6560 6020 6b65  ow_datetime`` ke
+00003770: 7977 6f72 6420 6172 6775 6d65 6e74 2e20  yword argument. 
+00003780: 2823 3134 3431 290a 2a20 5468 6520 6060  (#1441).* The ``
+00003790: 5379 6d62 6f6c 6060 2074 7261 6974 2074  Symbol`` trait t
+000037a0: 7970 6520 6973 2064 6570 7265 6361 7465  ype is deprecate
+000037b0: 642e 2046 6f72 2072 6573 6f6c 7574 696f  d. For resolutio
+000037c0: 6e20 6f66 2061 2073 7472 696e 670a 2020  n of a string.  
+000037d0: 7265 7072 6573 656e 7469 6e67 2061 2070  representing a p
+000037e0: 6163 6b61 6765 2f6d 6f64 756c 652f 6f62  ackage/module/ob
+000037f0: 6a65 6374 2063 6f6d 6269 6e61 7469 6f6e  ject combination
+00003800: 2c20 7573 6520 6060 696d 706f 7274 5f73  , use ``import_s
+00003810: 796d 626f 6c60 600a 2020 696e 7374 6561  ymbol``.  instea
+00003820: 642e 2028 2331 3534 3229 0a2a 2054 6865  d. (#1542).* The
+00003830: 2060 604d 6574 6148 6173 5472 6169 7473   ``MetaHasTraits
+00003840: 2e61 6464 5f6c 6973 7465 6e65 7260 6020  .add_listener`` 
+00003850: 616e 6420 6060 4d65 7461 4861 7354 7261  and ``MetaHasTra
+00003860: 6974 732e 7265 6d6f 7665 5f6c 6973 7465  its.remove_liste
+00003870: 6e65 7260 600a 2020 6d65 7468 6f64 7320  ner``.  methods 
+00003880: 6172 6520 6465 7072 6563 6174 6564 2e20  are deprecated. 
+00003890: 2823 3135 3530 290a 2a20 5468 6520 6060  (#1550).* The ``
+000038a0: 636c 6561 6e5f 6669 6c65 6e61 6d65 6060  clean_filename``
+000038b0: 2061 6e64 2060 6063 6c65 616e 5f74 696d   and ``clean_tim
+000038c0: 6573 7461 6d70 6060 2075 7469 6c69 7469  estamp`` utiliti
+000038d0: 6573 2061 7265 2064 6570 7265 6361 7465  es are deprecate
+000038e0: 642e 2049 660a 2020 796f 7520 6e65 6564  d. If.  you need
+000038f0: 2074 6865 7365 2075 7469 6c69 7469 6573   these utilities
+00003900: 2069 6e20 796f 7572 206f 776e 2070 726f   in your own pro
+00003910: 6a65 6374 2c20 796f 7527 7265 2061 6476  ject, you're adv
+00003920: 6973 6564 2074 6f20 636f 7079 2074 6865  ised to copy the
+00003930: 0a20 2063 6f64 6520 6469 7265 6374 6c79  .  code directly
+00003940: 2069 6e74 6f20 796f 7572 2070 726f 6a65   into your proje
+00003950: 6374 2e20 2823 3135 3237 290a 2a20 5468  ct. (#1527).* Th
+00003960: 6520 6060 6669 6e64 5f72 6573 6f75 7263  e ``find_resourc
+00003970: 6560 6020 616e 6420 6060 7374 6f72 655f  e`` and ``store_
+00003980: 7265 736f 7572 6365 6060 2066 756e 6374  resource`` funct
+00003990: 696f 6e73 2061 7265 2064 6570 7265 6361  ions are depreca
+000039a0: 7465 642e 204e 6577 0a20 2063 6f64 6520  ted. New.  code 
+000039b0: 7368 6f75 6c64 2075 7365 2060 6069 6d70  should use ``imp
+000039c0: 6f72 746c 6962 2e72 6573 6f75 7263 6573  ortlib.resources
+000039d0: 6060 206f 7220 6060 696d 706f 7274 6c69  `` or ``importli
+000039e0: 625f 7265 736f 7572 6365 7360 6020 696e  b_resources`` in
+000039f0: 7374 6561 640a 2020 6f66 2065 6974 6865  stead.  of eithe
+00003a00: 7220 6f66 2074 6865 7365 2066 756e 6374  r of these funct
+00003a10: 696f 6e73 2e20 2823 3135 3031 290a 0a0a  ions. (#1501)...
+00003a20: 4669 7865 730a 7e7e 7e7e 7e0a 0a2a 2049  Fixes.~~~~~..* I
+00003a30: 6e76 616c 6964 2061 7373 6967 6e6d 656e  nvalid assignmen
+00003a40: 7473 2074 6f20 6060 5072 6566 6978 4c69  ts to ``PrefixLi
+00003a50: 7374 6060 2061 6e64 2060 6050 7265 6669  st`` and ``Prefi
+00003a60: 784d 6170 6060 2074 7261 6974 7320 7072  xMap`` traits pr
+00003a70: 6f64 7563 6564 0a20 2061 6e20 756e 6e65  oduced.  an unne
+00003a80: 6365 7373 6172 696c 7920 6e65 7374 6564  cessarily nested
+00003a90: 2065 7863 6570 7469 6f6e 2e20 5468 6973   exception. This
+00003aa0: 2068 6173 2062 6565 6e20 6669 7865 642e   has been fixed.
+00003ab0: 2028 2331 3536 3429 0a2a 2041 6e20 6060   (#1564).* An ``
+00003ac0: 6f62 7365 7276 6560 602d 6465 636f 7261  observe``-decora
+00003ad0: 7465 6420 6c69 7374 656e 6572 206d 6574  ted listener met
+00003ae0: 686f 6420 7768 6f73 6520 6e61 6d65 2068  hod whose name h
+00003af0: 6173 2074 6865 2073 7065 6369 616c 2066  as the special f
+00003b00: 6f72 6d0a 2020 6060 225f 7472 6169 746e  orm.  ``"_traitn
+00003b10: 616d 655f 6368 616e 6765 6422 6060 2077  ame_changed"`` w
+00003b20: 696c 6c20 6e6f 206c 6f6e 6765 7220 6265  ill no longer be
+00003b30: 2074 7269 6767 6572 6564 2062 6f74 6820   triggered both 
+00003b40: 6173 2061 7320 7265 7375 6c74 0a20 206f  as as result.  o
+00003b50: 6620 7468 6520 6060 6f62 7365 7276 6560  f the ``observe`
+00003b60: 6020 6465 636f 7261 746f 7220 2a61 6e64  ` decorator *and
+00003b70: 2a20 7468 6520 7370 6563 6961 6c20 6e61  * the special na
+00003b80: 6d69 6e67 3a20 6974 2077 696c 6c20 6f6e  ming: it will on
+00003b90: 6c79 2062 650a 2020 7472 6967 6765 7265  ly be.  triggere
+00003ba0: 6420 7669 6120 7468 6520 6060 6f62 7365  d via the ``obse
+00003bb0: 7276 6560 6020 6465 636f 7261 746f 722e  rve`` decorator.
+00003bc0: 2028 2331 3536 3029 0a2a 2054 6865 2060   (#1560).* The `
+00003bd0: 6064 656c 6567 6174 6560 6020 7061 7261  `delegate`` para
+00003be0: 6d65 7465 7220 7761 7320 6d69 7374 7970  meter was mistyp
+00003bf0: 6564 2069 6e20 7468 6520 7479 7069 6e67  ed in the typing
+00003c00: 2073 7475 6273 2066 6f72 2074 6865 0a20   stubs for the. 
+00003c10: 2060 6044 656c 6567 6174 6560 6020 7472   ``Delegate`` tr
+00003c20: 6169 7420 7479 7065 2e20 5468 6973 2068  ait type. This h
+00003c30: 6173 2062 6565 6e20 6669 7865 642e 2028  as been fixed. (
+00003c40: 2331 3535 3629 0a2a 2054 6865 2060 6046  #1556).* The ``F
+00003c50: 756e 6374 696f 6e60 6020 616e 6420 6060  unction`` and ``
+00003c60: 4d65 7468 6f64 6060 2074 7261 6974 2074  Method`` trait t
+00003c70: 7970 6573 2077 696c 6c20 6e6f 206c 6f6e  ypes will no lon
+00003c80: 6765 7220 6661 696c 2077 6865 6e0a 2020  ger fail when.  
+00003c90: 6172 6775 6d65 6e74 7320 6172 6520 7061  arguments are pa
+00003ca0: 7373 6564 2e20 4e6f 7465 2074 6861 7420  ssed. Note that 
+00003cb0: 7468 6573 6520 7472 6169 7420 7479 7065  these trait type
+00003cc0: 7320 6172 6520 616c 7265 6164 7920 6465  s are already de
+00003cd0: 7072 6563 6174 6564 2c20 616e 640a 2020  precated, and.  
+00003ce0: 7368 6f75 6c64 206e 6f74 2062 6520 7573  should not be us
+00003cf0: 6564 2069 6e20 6e65 7720 636f 6465 2e20  ed in new code. 
+00003d00: 2823 3135 3433 290a 2a20 496e 6e65 7220  (#1543).* Inner 
+00003d10: 7472 6169 7473 206f 6620 6120 6060 556e  traits of a ``Un
+00003d20: 696f 6e60 6020 7472 6169 7420 6172 6520  ion`` trait are 
+00003d30: 6e6f 7720 7661 6c69 6461 7465 6420 7072  now validated pr
+00003d40: 6f70 6572 6c79 2e20 5072 6576 696f 7573  operly. Previous
+00003d50: 6c79 2c20 696e 0a20 2074 7261 6974 2064  ly, in.  trait d
+00003d60: 6563 6c61 7261 7469 6f6e 7320 6c69 6b65  eclarations like
+00003d70: 2060 6066 6f6f 203d 2055 6e69 6f6e 284c   ``foo = Union(L
+00003d80: 6973 7428 496e 7429 2c20 5374 7229 6060  ist(Int), Str)``
+00003d90: 2c20 7468 6520 6c69 7374 2065 6e74 7269  , the list entri
+00003da0: 6573 0a20 2077 6f75 6c64 206e 6f74 2062  es.  would not b
+00003db0: 6520 7661 6c69 6461 7465 642e 2028 2331  e validated. (#1
+00003dc0: 3532 322c 2023 3135 3334 290a 2a20 5472  522, #1534).* Tr
+00003dd0: 6169 7473 2077 6974 6820 6120 6479 6e61  aits with a dyna
+00003de0: 6d69 6320 6465 6661 756c 7420 7468 6174  mic default that
+00003df0: 2061 7070 6561 7220 6173 2069 6e6e 6572   appear as inner
+00003e00: 2074 7261 6974 7320 6f66 2061 2060 6054   traits of a ``T
+00003e10: 7570 6c65 6060 0a20 2074 7261 6974 2061  uple``.  trait a
+00003e20: 7265 206e 6f77 2076 616c 6964 6174 6564  re now validated
+00003e30: 2070 726f 7065 726c 792e 2028 2331 3532   properly. (#152
+00003e40: 3129 0a2a 2041 2070 6f74 656e 7469 616c  1).* A potential
+00003e50: 2072 6163 6520 636f 6e64 6974 696f 6e20   race condition 
+00003e60: 696e 2060 604c 6973 7465 6e65 7248 616e  in ``ListenerHan
+00003e70: 646c 6572 6060 2068 6173 2062 6565 6e20  dler`` has been 
+00003e80: 6669 7865 642e 2054 6865 0a20 2072 6163  fixed. The.  rac
+00003e90: 6520 636f 6e64 6974 696f 6e20 6973 2068  e condition is h
+00003ea0: 6172 6420 746f 2065 7865 7263 6973 6520  ard to exercise 
+00003eb0: 616e 6420 6861 7320 6e6f 7420 6265 656e  and has not been
+00003ec0: 2077 6974 6e65 7373 6564 2069 6e20 7468   witnessed in th
+00003ed0: 6520 7769 6c64 2e0a 2020 2823 3134 3935  e wild..  (#1495
+00003ee0: 290a 2a20 5573 6520 6f66 2060 6061 6464  ).* Use of ``add
+00003ef0: 5f63 6c61 7373 5f74 7261 6974 6060 2074  _class_trait`` t
+00003f00: 6f20 6164 6420 6120 6060 4c69 7374 6060  o add a ``List``
+00003f10: 2074 7261 6974 2077 6173 2062 726f 6b65   trait was broke
+00003f20: 6e20 696e 2074 6865 2070 7265 7365 6e63  n in the presenc
+00003f30: 650a 2020 6f66 2073 7562 636c 6173 7365  e.  of subclasse
+00003f40: 732e 2054 6869 7320 6861 7320 6265 656e  s. This has been
+00003f50: 2066 6978 6564 2e20 2823 3134 3631 290a   fixed. (#1461).
+00003f60: 2a20 4120 7573 6520 6f66 2074 6865 2028  * A use of the (
+00003f70: 6465 7072 6563 6174 6564 2920 6060 6469  deprecated) ``di
+00003f80: 7374 7574 696c 7360 6020 6c69 6272 6172  stutils`` librar
+00003f90: 7920 6861 7320 6265 656e 2072 6570 6c61  y has been repla
+00003fa0: 6365 6420 7769 7468 0a20 2060 6073 7973  ced with.  ``sys
+00003fb0: 636f 6e66 6967 6060 2e20 2823 3134 3532  config``. (#1452
+00003fc0: 290a 2a20 4479 6e61 6d69 6320 6465 6661  ).* Dynamic defa
+00003fd0: 756c 7420 6861 6e64 696e 6720 6861 7320  ult handing has 
+00003fe0: 6265 656e 2066 6978 6564 2069 6e20 7468  been fixed in th
+00003ff0: 6520 6060 5f69 6e73 7461 6e63 655f 6861  e ``_instance_ha
+00004000: 6e64 6c65 725f 6661 6374 6f72 7960 600a  ndler_factory``.
+00004010: 2020 7573 6564 2062 7920 7468 6520 5472    used by the Tr
+00004020: 6169 7473 5549 2060 6054 6162 6c65 4564  aitsUI ``TableEd
+00004030: 6974 6f72 6060 2e20 2823 3134 3436 2c20  itor``. (#1446, 
+00004040: 2331 3435 3029 0a2a 2054 6865 2074 7261  #1450).* The tra
+00004050: 6974 2064 6573 6372 6970 7469 6f6e 7320  it descriptions 
+00004060: 2874 6865 2022 696e 666f 2220 7465 7874  (the "info" text
+00004070: 2920 666f 7220 7468 6520 6060 4669 6c65  ) for the ``File
+00004080: 6060 2061 6e64 2060 6044 6972 6563 746f  `` and ``Directo
+00004090: 7279 6060 0a20 2074 7261 6974 7320 6861  ry``.  traits ha
+000040a0: 7665 2062 6565 6e20 6669 7865 6420 746f  ve been fixed to
+000040b0: 2061 766f 6964 2067 6976 696e 6720 6120   avoid giving a 
+000040c0: 6d69 736c 6561 6469 6e67 2065 7272 6f72  misleading error
+000040d0: 206d 6573 7361 6765 2077 6865 6e0a 2020   message when.  
+000040e0: 6060 6578 6973 7473 3d54 7275 6560 602e  ``exists=True``.
+000040f0: 2028 2331 3434 3029 0a2a 2043 6c6f 6e65   (#1440).* Clone
+00004100: 7320 6f66 2060 6042 6173 6549 6e73 7461  s of ``BaseInsta
+00004110: 6e63 6560 6020 7472 6169 7473 2064 6964  nce`` traits did
+00004120: 6e27 7420 636f 7272 6563 746c 7920 7265  n't correctly re
+00004130: 7370 6563 7420 7468 6520 6060 616c 6c6f  spect the ``allo
+00004140: 775f 6e6f 6e65 6060 0a20 2070 6172 616d  w_none``.  param
+00004150: 6574 6572 2e20 5468 6973 2069 7320 6e6f  eter. This is no
+00004160: 7720 6669 7865 642e 2028 2331 3433 3329  w fixed. (#1433)
+00004170: 0a2a 2041 6e20 6f75 7464 6174 6564 2072  .* An outdated r
+00004180: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
+00004190: 2270 7967 6c65 7422 204b 6976 6120 6261  "pyglet" Kiva ba
+000041a0: 636b 656e 6420 6861 7320 6265 656e 2072  ckend has been r
+000041b0: 656d 6f76 6564 2e20 2823 3134 3331 290a  emoved. (#1431).
+000041c0: 0a0a 446f 6375 6d65 6e74 6174 696f 6e0a  ..Documentation.
+000041d0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a  ~~~~~~~~~~~~~..*
+000041e0: 2042 7269 6566 2069 6e73 7461 6c6c 6174   Brief installat
+000041f0: 696f 6e20 646f 6373 2068 6176 6520 6265  ion docs have be
+00004200: 656e 2061 6464 6564 2e20 2823 3135 3539  en added. (#1559
+00004210: 290a 2a20 4f63 6375 7272 656e 6365 7320  ).* Occurrences 
+00004220: 6f66 2060 6041 6e79 2873 6f6d 655f 6c69  of ``Any(some_li
+00004230: 7374 2960 6020 696e 2064 6f63 7320 6861  st)`` in docs ha
+00004240: 7665 2062 6565 6e20 7265 706c 6163 6564  ve been replaced
+00004250: 2e20 2823 3135 3437 290a 2a20 5468 6520  . (#1547).* The 
+00004260: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
+00004270: 7220 6060 7379 6e63 5f74 7261 6974 6060  r ``sync_trait``
+00004280: 2068 6173 2062 6565 6e20 7570 6461 7465   has been update
+00004290: 6420 746f 206e 6f74 6520 7468 6174 2069  d to note that i
+000042a0: 7420 6f6e 6c79 0a20 2073 796e 6368 726f  t only.  synchro
+000042b0: 6e69 7365 7320 6974 656d 7320 666f 7220  nises items for 
+000042c0: 6060 4c69 7374 6060 2074 7261 6974 732c  ``List`` traits,
+000042d0: 206e 6f74 2066 6f72 2060 6044 6963 7460   not for ``Dict`
+000042e0: 6020 616e 6420 6060 5365 7460 6020 7472  ` and ``Set`` tr
+000042f0: 6169 7473 2e0a 2020 2823 3135 3139 290a  aits..  (#1519).
+00004300: 2a20 4120 636f 6e66 6967 7572 6174 696f  * A configuratio
+00004310: 6e20 6669 6c65 2066 6f72 2052 6561 6420  n file for Read 
+00004320: 7468 6520 446f 6373 2068 6173 2062 6565  the Docs has bee
+00004330: 6e20 6164 6465 642e 2028 2331 3437 3829  n added. (#1478)
+00004340: 0a2a 2041 2060 6044 6570 7265 6361 7469  .* A ``Deprecati
+00004350: 6f6e 5761 726e 696e 6760 6020 6172 6973  onWarning`` aris
+00004360: 696e 6720 6672 6f6d 2061 6e20 756e 6e65  ing from an unne
+00004370: 6365 7373 6172 7920 6f76 6572 7269 6465  cessary override
+00004380: 206f 6620 7468 650a 2020 6060 6164 645f   of the.  ``add_
+00004390: 636f 6e74 656e 7460 6020 6d65 7468 6f64  content`` method
+000043a0: 2069 6e20 7468 6520 6060 5472 6169 7444   in the ``TraitD
+000043b0: 6f63 756d 656e 7465 7260 6020 6861 7320  ocumenter`` has 
+000043c0: 6265 656e 2066 6978 6564 2e20 2823 3134  been fixed. (#14
+000043d0: 3735 290a 2a20 5468 6520 5370 6869 6e78  75).* The Sphinx
+000043e0: 2076 6572 7369 6f6e 2077 6173 2074 656d   version was tem
+000043f0: 706f 7261 7269 6c79 2070 696e 6e65 6420  porarily pinned 
+00004400: 746f 2061 766f 6964 2062 7569 6c64 2066  to avoid build f
+00004410: 6169 6c75 7265 7320 6172 6973 696e 670a  ailures arising.
+00004420: 2020 6672 6f6d 2062 7567 7320 696e 2053    from bugs in S
+00004430: 7068 696e 7820 342e 302e 312e 2054 6861  phinx 4.0.1. Tha
+00004440: 7420 7069 6e20 6861 7320 7369 6e63 6520  t pin has since 
+00004450: 6265 656e 2072 6576 6572 7465 642e 0a20  been reverted.. 
+00004460: 2028 2331 3437 312c 2023 3134 3632 290a   (#1471, #1462).
+00004470: 2a20 5661 7269 6f75 7320 646f 6373 7472  * Various docstr
+00004480: 696e 6720 6669 7865 7320 6861 7665 2062  ing fixes have b
+00004490: 6565 6e20 6170 706c 6965 642e 2028 2331  een applied. (#1
+000044a0: 3436 382c 2023 3134 3635 290a 2a20 5661  468, #1465).* Va
+000044b0: 7269 6f75 7320 7479 706f 2066 6978 6573  rious typo fixes
+000044c0: 2068 6176 6520 6265 656e 2061 7070 6c69   have been appli
+000044d0: 6564 2e20 2823 3134 3538 2c20 2331 3434  ed. (#1458, #144
+000044e0: 3229 0a2a 2052 6566 6572 656e 6365 7320  2).* References 
+000044f0: 746f 2060 6048 6173 5472 6169 7473 2e73  to ``HasTraits.s
+00004500: 6574 6060 2068 6176 6520 6265 656e 2072  et`` have been r
+00004510: 6570 6c61 6365 6420 7769 7468 0a20 2060  eplaced with.  `
+00004520: 6048 6173 5472 6169 7473 2e74 7261 6974  `HasTraits.trait
+00004530: 5f73 6574 6060 2e20 2823 3134 3531 290a  _set``. (#1451).
+00004540: 2a20 536f 6d65 2069 7373 7565 7320 7769  * Some issues wi
+00004550: 7468 2074 6865 2074 7574 6f72 6961 6c20  th the tutorial 
+00004560: 4353 5320 7573 6564 2069 6e20 7468 6520  CSS used in the 
+00004570: 4554 5320 6465 6d6f 2061 7070 6c69 6361  ETS demo applica
+00004580: 7469 6f6e 2068 6176 6520 6265 656e 0a20  tion have been. 
+00004590: 2066 6978 6564 3b20 7468 6520 636f 6c6f   fixed; the colo
+000045a0: 7572 2073 6368 656d 6520 6861 7320 6265  ur scheme has be
+000045b0: 656e 2063 6861 6e67 6564 2074 6f20 456e  en changed to En
+000045c0: 7468 6f75 6768 7420 636f 6c6f 7572 732e  thought colours.
+000045d0: 2028 2331 3432 312c 0a20 2023 3134 3139   (#1421,.  #1419
+000045e0: 290a 0a0a 436c 6561 6e75 7020 616e 6420  )...Cleanup and 
+000045f0: 7265 6661 6374 6f72 696e 670a 7e7e 7e7e  refactoring.~~~~
+00004600: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00004610: 7e7e 7e0a 0a2a 2041 6c6c 2062 7569 6c74  ~~~..* All built
+00004620: 2d69 6e20 5472 6169 7454 7970 6520 7375  -in TraitType su
+00004630: 6263 6c61 7373 6573 206e 6f77 2070 726f  bclasses now pro
+00004640: 7669 6465 2074 6865 2064 6566 6175 6c74  vide the default
+00004650: 2076 616c 7565 2074 7970 6520 6469 7265   value type dire
+00004660: 6374 6c79 0a20 2072 6174 6865 7220 7468  ctly.  rather th
+00004670: 616e 2069 6e66 6572 7269 6e67 2069 742e  an inferring it.
+00004680: 2028 2331 3535 352c 2023 3135 3336 2c20   (#1555, #1536, 
+00004690: 2331 3533 312c 2023 3135 3339 2c20 2331  #1531, #1539, #1
+000046a0: 3533 322c 2023 3135 3430 290a 2a20 5468  532, #1540).* Th
+000046b0: 6520 6060 7472 6169 745f 6164 6465 6460  e ``trait_added`
+000046c0: 6020 616e 6420 6060 7472 6169 745f 6d6f  ` and ``trait_mo
+000046d0: 6469 6669 6564 6060 2074 7261 6974 7320  dified`` traits 
+000046e0: 6f6e 2060 6048 6173 5472 6169 7473 6060  on ``HasTraits``
+000046f0: 206e 6f77 0a20 2068 6176 6520 7072 6f70   now.  have prop
+00004700: 6572 2074 7261 6974 2074 7970 6520 6465  er trait type de
+00004710: 636c 6172 6174 696f 6e73 2e20 2823 3135  clarations. (#15
+00004720: 3532 290a 2a20 5265 6475 6e64 616e 7420  52).* Redundant 
+00004730: 6060 756e 6974 7465 7374 2e6d 6169 6e20  ``unittest.main 
+00004740: 626c 6f63 6b73 6060 2068 6176 6520 6265  blocks`` have be
+00004750: 656e 2072 656d 6f76 6564 2e20 2823 3135  en removed. (#15
+00004760: 3435 290a 2a20 5374 796c 6520 6669 7865  45).* Style fixe
+00004770: 7320 6861 7665 2062 6565 6e20 6170 706c  s have been appl
+00004780: 6965 6420 746f 2060 6074 7261 6974 5f74  ied to ``trait_t
+00004790: 7970 6573 2e70 7969 6060 2e20 2823 3135  ypes.pyi``. (#15
+000047a0: 3233 290a 2a20 6060 4f62 7365 7276 6572  23).* ``Observer
+000047b0: 4578 7072 6573 7369 6f6e 6060 2061 6e64  Expression`` and
+000047c0: 206f 7468 6572 206b 6579 206f 6273 6572   other key obser
+000047d0: 7661 7469 6f6e 2063 6c61 7373 6573 206e  vation classes n
+000047e0: 6f77 2068 6176 6520 6d6f 7265 0a20 2064  ow have more.  d
+000047f0: 6562 7567 2d66 7269 656e 646c 7920 6060  ebug-friendly ``
+00004800: 7265 7072 6060 2069 6d70 6c65 6d65 6e74  repr`` implement
+00004810: 6174 696f 6e73 2e20 2823 3135 3134 290a  ations. (#1514).
+00004820: 2a20 5468 6520 6060 6f62 7365 7276 6572  * The ``observer
+00004830: 6060 2070 6172 7369 6e67 2069 6e74 6572  `` parsing inter
+00004840: 6e61 6c73 2068 6176 6520 6265 656e 2072  nals have been r
+00004850: 6577 6f72 6b65 6420 746f 206d 616b 650a  eworked to make.
+00004860: 2020 6060 4f62 7365 7276 6572 4772 6170    ``ObserverGrap
+00004870: 6860 6020 7468 6520 6b65 7920 2263 6f6d  h`` the key "com
+00004880: 7069 6c65 6422 206f 626a 6563 7420 7468  piled" object th
+00004890: 6174 2074 6865 2072 6573 7420 6f66 2054  at the rest of T
+000048a0: 7261 6974 7320 6361 7265 730a 2020 6162  raits cares.  ab
+000048b0: 6f75 742c 2072 6174 6865 7220 7468 616e  out, rather than
+000048c0: 2060 604f 6273 6572 7665 7245 7870 7265   ``ObserverExpre
+000048d0: 7373 696f 6e60 602e 2028 2331 3531 3229  ssion``. (#1512)
+000048e0: 0a2a 2054 6865 2067 7261 6d6d 6172 2061  .* The grammar a
+000048f0: 6e64 2070 6172 7365 7220 666f 7220 7468  nd parser for th
+00004900: 6520 6f62 7365 7276 6520 6d69 6e69 2d6c  e observe mini-l
+00004910: 616e 6775 6167 6520 6861 7665 2062 6565  anguage have bee
+00004920: 6e20 7369 6d70 6c69 6669 6564 2e0a 2020  n simplified..  
+00004930: 2823 3135 3036 290a 2a20 436f 6e66 7573  (#1506).* Confus
+00004940: 696f 6e20 6265 7477 6565 6e20 2261 6e79  ion between "any
+00004950: 5f74 7261 6974 2220 616e 6420 2261 6e79  _trait" and "any
+00004960: 7472 6169 7422 2069 6e20 6e6f 6e2d 7573  trait" in non-us
+00004970: 6572 2d66 6163 696e 670a 2020 6675 6e63  er-facing.  func
+00004980: 7469 6f6e 7320 616e 6420 636c 6173 7365  tions and classe
+00004990: 7320 6861 7320 6265 656e 2063 6c65 616e  s has been clean
+000049a0: 6564 2075 702e 2028 2331 3439 3729 0a2a  ed up. (#1497).*
+000049b0: 2055 6e6e 6563 6573 7361 7279 2060 606e   Unnecessary ``n
+000049c0: 6f71 6160 6020 6d61 726b 6572 7320 6861  oqa`` markers ha
+000049d0: 7665 2062 6565 6e20 7265 6d6f 7665 642e  ve been removed.
+000049e0: 2028 2331 3439 3929 0a2a 2041 2075 7365   (#1499).* A use
+000049f0: 206f 6620 7468 6520 6060 7072 6f70 6572   of the ``proper
+00004a00: 7479 6060 2063 616c 6c61 626c 6520 6861  ty`` callable ha
+00004a10: 7320 6265 656e 2072 6570 6c61 6365 6420  s been replaced 
+00004a20: 7769 7468 2061 2060 6070 726f 7065 7274  with a ``propert
+00004a30: 7960 600a 2020 6465 636f 7261 746f 722e  y``.  decorator.
+00004a40: 2028 2331 3437 3029 0a2a 2041 2062 6164   (#1470).* A bad
+00004a50: 206f 6273 6572 7665 2d64 6563 6f72 6174   observe-decorat
+00004a60: 6564 206c 6973 7465 6e65 7220 7369 676e  ed listener sign
+00004a70: 6174 7572 6520 696e 2061 2074 6573 7420  ature in a test 
+00004a80: 6861 7320 6265 656e 2066 6978 6564 2e20  has been fixed. 
+00004a90: 2823 3135 3330 290a 0a0a 4275 696c 6420  (#1530)...Build 
+00004aa0: 616e 6420 6465 7665 6c6f 706d 656e 7420  and development 
+00004ab0: 776f 726b 666c 6f77 0a7e 7e7e 7e7e 7e7e  workflow.~~~~~~~
+00004ac0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00004ad0: 7e7e 7e7e 7e7e 7e0a 0a2a 2050 7974 686f  ~~~~~~~..* Pytho
+00004ae0: 6e20 332e 3130 2069 7320 7375 7070 6f72  n 3.10 is suppor
+00004af0: 7465 6420 616e 6420 7465 7374 6564 2c20  ted and tested, 
+00004b00: 616e 6420 7768 6565 6c73 2061 7265 2062  and wheels are b
+00004b10: 7569 6c74 2066 6f72 2050 7974 686f 6e20  uilt for Python 
+00004b20: 332e 3130 2e0a 2020 2823 3134 3235 2c20  3.10..  (#1425, 
+00004b30: 2331 3536 372c 2023 3135 3639 2c20 2331  #1567, #1569, #1
+00004b40: 3537 3129 0a2a 2057 6865 656c 7320 6172  571).* Wheels ar
+00004b50: 6520 6e6f 7720 6275 696c 7420 666f 7220  e now built for 
+00004b60: 4c69 6e75 782f 6161 7263 6836 342e 2028  Linux/aarch64. (
+00004b70: 2331 3536 3729 0a2a 2055 6e69 7665 7273  #1567).* Univers
+00004b80: 616c 2077 6865 656c 7320 6172 6520 6e6f  al wheels are no
+00004b90: 7720 6275 696c 7420 666f 7220 6d61 634f  w built for macO
+00004ba0: 532c 2074 6f20 7375 7070 6f72 7420 4170  S, to support Ap
+00004bb0: 706c 6520 5369 6c69 636f 6e2e 2028 2331  ple Silicon. (#1
+00004bc0: 3536 3729 0a2a 2043 726f 6e20 6a6f 6273  567).* Cron jobs
+00004bd0: 206e 6f77 2073 656e 6420 6661 696c 7572   now send failur
+00004be0: 652f 7375 6363 6573 7320 536c 6163 6b20  e/success Slack 
+00004bf0: 6e6f 7469 6669 6361 7469 6f6e 7320 746f  notifications to
+00004c00: 2045 6e74 686f 7567 6874 2773 0a20 2069   Enthought's.  i
+00004c10: 6e74 6572 6e61 6c20 6368 616e 6e65 6c2e  nternal channel.
+00004c20: 2028 2331 3438 3129 0a2a 2041 6c6c 2063   (#1481).* All c
+00004c30: 726f 6e20 6a6f 6273 206e 6f77 2069 6e63  ron jobs now inc
+00004c40: 6c75 6465 2061 2060 6077 6f72 6b66 6c6f  lude a ``workflo
+00004c50: 775f 6469 7370 6174 6368 6060 2074 7269  w_dispatch`` tri
+00004c60: 6767 6572 2e20 2823 3134 3830 290a 2a20  gger. (#1480).* 
+00004c70: 5468 6520 6d61 696e 2064 6576 656c 6f70  The main develop
+00004c80: 6d65 6e74 2062 7261 6e63 6820 6973 206e  ment branch is n
+00004c90: 6f77 2063 616c 6c65 6420 226d 6169 6e22  ow called "main"
+00004ca0: 2072 6174 6865 7220 7468 616e 2022 6d61   rather than "ma
+00004cb0: 7374 6572 222e 0a20 2028 2331 3436 3729  ster"..  (#1467)
+00004cc0: 0a2a 2041 7574 6f6d 6174 6564 2074 6573  .* Automated tes
+00004cd0: 7473 2068 6176 6520 6265 656e 2061 6464  ts have been add
+00004ce0: 6564 2066 6f72 2050 7950 4920 7768 6565  ed for PyPI whee
+00004cf0: 6c73 2e20 2823 3134 3137 290a 0a0a 5265  ls. (#1417)...Re
+00004d00: 6c65 6173 6520 362e 322e 300a 2d2d 2d2d  lease 6.2.0.----
+00004d10: 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561  ---------..Relea
+00004d20: 7365 643a 2032 3032 312d 3031 2d32 310a  sed: 2021-01-21.
+00004d30: 0a54 6865 2054 7261 6974 7320 6c69 6272  .The Traits libr
+00004d40: 6172 7920 6973 2061 2066 6f75 6e64 6174  ary is a foundat
+00004d50: 696f 6e61 6c20 636f 6d70 6f6e 656e 7420  ional component 
+00004d60: 6f66 2074 6865 2045 6e74 686f 7567 6874  of the Enthought
+00004d70: 2054 6f6f 6c20 5375 6974 652e 2049 740a   Tool Suite. It.
+00004d80: 7072 6f76 6964 6573 206f 6273 6572 7661  provides observa
+00004d90: 626c 652c 2074 7970 6564 2061 7474 7269  ble, typed attri
+00004da0: 6275 7465 7320 666f 7220 5079 7468 6f6e  butes for Python
+00004db0: 2063 6c61 7373 6573 2c20 6d61 6b69 6e67   classes, making
+00004dc0: 2074 686f 7365 2063 6c61 7373 6573 0a73   those classes.s
+00004dd0: 7569 7461 626c 6520 666f 7220 6576 656e  uitable for even
+00004de0: 742d 6472 6976 656e 2064 6174 6166 6c6f  t-driven dataflo
+00004df0: 7720 7072 6f67 7261 6d6d 696e 6720 616e  w programming an
+00004e00: 6420 666f 7220 696d 6d65 6469 6174 6520  d for immediate 
+00004e10: 7573 6520 6173 206d 6f64 656c 730a 666f  use as models.fo
+00004e20: 7220 6772 6170 6869 6361 6c20 7573 6572  r graphical user
+00004e30: 2069 6e74 6572 6661 6365 732c 206c 696b   interfaces, lik
+00004e40: 6520 7468 6f73 6520 7072 6f76 6964 6564  e those provided
+00004e50: 2062 7920 7468 6520 5472 6169 7473 5549   by the TraitsUI
+00004e60: 206c 6962 7261 7279 2e0a 0a54 7261 6974   library...Trait
+00004e70: 7320 362e 3220 6973 2074 6865 206c 6174  s 6.2 is the lat
+00004e80: 6573 7420 6665 6174 7572 6520 7265 6c65  est feature rele
+00004e90: 6173 6520 696e 2074 6865 2054 7261 6974  ase in the Trait
+00004ea0: 7320 3620 7365 7269 6573 2c20 7769 7468  s 6 series, with
+00004eb0: 2073 6576 6572 616c 0a69 6d70 726f 7665   several.improve
+00004ec0: 6d65 6e74 7320 616e 6420 6669 7865 7320  ments and fixes 
+00004ed0: 6f76 6572 2054 7261 6974 7320 362e 312e  over Traits 6.1.
+00004ee0: 0a0a 4869 6768 6c69 6768 7473 206f 6620  ..Highlights of 
+00004ef0: 7468 6973 2072 656c 6561 7365 0a7e 7e7e  this release.~~~
+00004f00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00004f10: 7e7e 7e7e 7e7e 7e0a 0a2a 2054 6865 2054  ~~~~~~~..* The T
+00004f20: 7261 6974 7320 6578 616d 706c 6573 2061  raits examples a
+00004f30: 7265 206e 6f77 2064 6973 7472 6962 7574  re now distribut
+00004f40: 6564 2061 7320 7061 7274 206f 6620 7468  ed as part of th
+00004f50: 6520 5472 6169 7473 2065 6767 2c20 616e  e Traits egg, an
+00004f60: 640a 2020 6172 6520 636f 6e74 7269 6275  d.  are contribu
+00004f70: 7465 6420 746f 2074 6865 2060 6065 7473  ted to the ``ets
+00004f80: 6465 6d6f 6060 2061 7070 6c69 6361 7469  demo`` applicati
+00004f90: 6f6e 2e20 2854 6865 206c 6174 7465 7220  on. (The latter 
+00004fa0: 6361 6e20 6265 0a20 2069 6e73 7461 6c6c  can be.  install
+00004fb0: 6564 2066 726f 6d20 5079 5049 2077 6974  ed from PyPI wit
+00004fc0: 6820 6060 7069 7020 696e 7374 616c 6c20  h ``pip install 
+00004fd0: 6574 7364 656d 6f60 602e 290a 2a20 5065  etsdemo``.).* Pe
+00004fe0: 7266 6f72 6d61 6e63 6520 6f66 2074 6865  rformance of the
+00004ff0: 2060 606f 6273 6572 7665 6060 2066 7261   ``observe`` fra
+00005000: 6d65 776f 726b 2068 6173 2062 6565 6e20  mework has been 
+00005010: 7369 676e 6966 6963 616e 746c 7920 696d  significantly im
+00005020: 7072 6f76 6564 2e0a 2a20 4974 2773 206e  proved..* It's n
+00005030: 6f20 6c6f 6e67 6572 206e 6563 6573 7361  o longer necessa
+00005040: 7279 2074 6f20 7370 6563 6966 7920 6120  ry to specify a 
+00005050: 7472 6169 7420 636f 6d70 6172 6973 6f6e  trait comparison
+00005060: 206d 6f64 6520 6f66 0a20 2060 6043 6f6d   mode of.  ``Com
+00005070: 7061 7269 736f 6e4d 6f64 652e 6964 656e  parisonMode.iden
+00005080: 7469 7479 6060 2077 6865 6e20 7573 696e  tity`` when usin
+00005090: 6720 6060 6f62 7365 7276 6560 6020 746f  g ``observe`` to
+000050a0: 206f 6273 6572 7665 2069 7465 6d73 0a20   observe items. 
+000050b0: 2069 6e20 6120 6060 4c69 7374 6060 2c20   in a ``List``, 
+000050c0: 6060 4469 6374 6060 206f 7220 6060 5365  ``Dict`` or ``Se
+000050d0: 7460 602e 0a2a 2053 7570 706f 7274 2066  t``..* Support f
+000050e0: 6f72 2050 7974 686f 6e20 332e 3520 6861  or Python 3.5 ha
+000050f0: 7320 6265 656e 2064 726f 7070 6564 2e0a  s been dropped..
+00005100: 2a20 5768 656e 2069 6d70 6f72 7469 6e67  * When importing
+00005110: 2066 726f 6d20 5472 6169 7473 2c20 796f   from Traits, yo
+00005120: 7520 7368 6f75 6c64 2061 6c77 6179 7320  u should always 
+00005130: 696d 706f 7274 2066 726f 6d20 6f6e 6520  import from one 
+00005140: 6f66 2074 6865 2060 6061 7069 6060 0a20  of the ``api``. 
+00005150: 206d 6f64 756c 6573 2028 666f 7220 6578   modules (for ex
+00005160: 616d 706c 652c 2060 6074 7261 6974 732e  ample, ``traits.
+00005170: 6170 6960 602c 2060 6074 7261 6974 732e  api``, ``traits.
+00005180: 6164 6170 7461 7469 6f6e 2e61 7069 6060  adaptation.api``
+00005190: 2c20 6574 632e 2920 5468 6973 0a20 2072  , etc.) This.  r
+000051a0: 6563 6f6d 6d65 6e64 6174 696f 6e20 6861  ecommendation ha
+000051b0: 7320 6e6f 7720 6265 656e 206d 6164 6520  s now been made 
+000051c0: 6578 706c 6963 6974 2069 6e20 7468 6520  explicit in the 
+000051d0: 646f 6375 6d65 6e74 6174 696f 6e2e 2049  documentation. I
+000051e0: 6620 796f 7520 6669 6e64 0a20 2073 6f6d  f you find.  som
+000051f0: 6574 6869 6e67 2079 6f75 206e 6565 6420  ething you need 
+00005200: 7468 6174 2773 206e 6f74 2061 7661 696c  that's not avail
+00005210: 6162 6c65 2066 726f 6d20 6f6e 6520 6f66  able from one of
+00005220: 2074 6865 2060 6061 7069 6060 206d 6f64   the ``api`` mod
+00005230: 756c 6573 2c0a 2020 706c 6561 7365 206c  ules,.  please l
+00005240: 6574 2074 6865 2054 7261 6974 7320 6465  et the Traits de
+00005250: 7665 6c6f 7065 7273 206b 6e6f 772e 0a0a  velopers know...
+00005260: 0a44 6574 6169 6c65 6420 5052 2d62 792d  .Detailed PR-by-
+00005270: 5052 2063 6861 6e67 6573 0a7e 7e7e 7e7e  PR changes.~~~~~
+00005280: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00005290: 7e7e 7e7e 0a0a 4d6f 7265 2074 6861 6e20  ~~~~..More than 
+000052a0: 3630 2050 5273 2077 656e 7420 696e 746f  60 PRs went into
+000052b0: 2074 6869 7320 7265 6c65 6173 652e 2054   this release. T
+000052c0: 6865 2066 6f6c 6c6f 7769 6e67 2070 656f  he following peo
+000052d0: 706c 6520 636f 6e74 7269 6275 7465 6420  ple contributed 
+000052e0: 746f 0a74 6869 7320 7265 6c65 6173 653a  to.this release:
+000052f0: 0a0a 2a20 4161 726f 6e20 4179 7265 730a  ..* Aaron Ayres.
+00005300: 2a20 416c 6578 616e 6472 6520 4368 6162  * Alexandre Chab
+00005310: 6f74 2d4c 6563 6c65 7263 0a2a 204b 6974  ot-Leclerc.* Kit
+00005320: 2043 686f 690a 2a20 4d61 726b 2044 6963   Choi.* Mark Dic
+00005330: 6b69 6e73 6f6e 0a2a 204b 6576 696e 2044  kinson.* Kevin D
+00005340: 7566 660a 2a20 476c 656e 2047 7261 6e7a  uff.* Glen Granz
+00005350: 6f77 0a2a 204d 6174 7420 4861 6e63 6f63  ow.* Matt Hancoc
+00005360: 6b0a 2a20 5261 6875 6c20 506f 7275 7269  k.* Rahul Poruri
+00005370: 0a2a 2045 7269 6320 5072 6573 7461 740a  .* Eric Prestat.
+00005380: 2a20 4b75 7961 2054 616b 616d 690a 2a20  * Kuya Takami.* 
+00005390: 4875 676f 2076 616e 204b 656d 656e 6164  Hugo van Kemenad
+000053a0: 650a 2a20 4164 6974 7961 2056 6174 730a  e.* Aditya Vats.
+000053b0: 2a20 436f 7272 616e 2057 6562 7374 6572  * Corran Webster
+000053c0: 0a0a 0a46 6561 7475 7265 730a 7e7e 7e7e  ...Features.~~~~
+000053d0: 7e7e 7e7e 0a0a 2a20 5468 6520 6060 5072  ~~~~..* The ``Pr
+000053e0: 6f70 6572 7479 6060 2074 7261 6974 2074  operty`` trait t
+000053f0: 7970 6520 6e6f 7720 7375 7070 6f72 7473  ype now supports
+00005400: 2074 6865 2060 606f 6273 6572 7665 6060   the ``observe``
+00005410: 206b 6579 776f 7264 2e20 2823 3131 3735   keyword. (#1175
+00005420: 2c0a 2020 2331 3430 3029 0a2a 2041 6464  ,.  #1400).* Add
+00005430: 2060 607c 3d60 6020 7375 7070 6f72 7420   ``|=`` support 
+00005440: 746f 2054 7261 6974 4469 6374 2066 6f72  to TraitDict for
+00005450: 2050 7974 686f 6e20 332e 3920 616e 6420   Python 3.9 and 
+00005460: 6c61 7465 722e 2028 2331 3330 3629 0a2a  later. (#1306).*
+00005470: 2041 6464 2063 6173 7469 6e67 206b 6579   Add casting key
+00005480: 776f 7264 2074 6f20 6e75 6d65 7269 6320  word to numeric 
+00005490: 6172 7261 7920 7479 7065 732e 2028 2335  array types. (#5
+000054a0: 3437 290a 2a20 5468 6520 5472 6169 7473  47).* The Traits
+000054b0: 2065 7861 6d70 6c65 7320 6172 6520 6e6f   examples are no
+000054c0: 7720 7061 7274 206f 6620 7468 6520 5472  w part of the Tr
+000054d0: 6169 7473 2070 6163 6b61 6765 2c20 616e  aits package, an
+000054e0: 6420 736f 2061 7265 0a20 2063 6f6e 7472  d so are.  contr
+000054f0: 6962 7574 6564 2074 6f20 6060 6574 7364  ibuted to ``etsd
+00005500: 656d 6f60 602e 2028 2331 3237 3529 0a2a  emo``. (#1275).*
+00005510: 2054 6865 2054 7261 6974 7320 6578 616d   The Traits exam
+00005520: 706c 6573 2070 6163 6b61 6765 206e 6f77  ples package now
+00005530: 2069 6e63 6c75 6465 7320 6120 6265 6769   includes a begi
+00005540: 6e6e 6572 2773 2074 7574 6f72 6961 6c2e  nner's tutorial.
+00005550: 2028 2331 3036 3129 0a0a 0a50 6572 666f   (#1061)...Perfo
+00005560: 726d 616e 6365 0a7e 7e7e 7e7e 7e7e 7e7e  rmance.~~~~~~~~~
+00005570: 7e7e 0a0a 2a20 5061 7273 696e 6720 6f66  ~~..* Parsing of
+00005580: 2074 6865 2060 606f 6273 6572 7665 6060   the ``observe``
+00005590: 2073 7472 696e 6720 7761 7320 7072 6576   string was prev
+000055a0: 696f 7573 6c79 2061 2070 6572 666f 726d  iously a perform
+000055b0: 616e 6365 2062 6f74 746c 656e 6563 6b2e  ance bottleneck.
+000055c0: 0a20 2054 6869 7320 6861 7320 6265 656e  .  This has been
+000055d0: 2066 6978 6564 2c20 6279 2072 656d 6f76   fixed, by remov
+000055e0: 696e 6720 736f 6d65 2072 6564 756e 6461  ing some redunda
+000055f0: 6e74 2070 6172 7369 6e67 2063 616c 6c73  nt parsing calls
+00005600: 2061 6e64 2062 7920 6361 6368 696e 670a   and by caching.
+00005610: 2020 7061 7273 696e 6720 7265 7375 6c74    parsing result
+00005620: 732e 2028 2331 3334 332c 2023 3133 3434  s. (#1343, #1344
+00005630: 2c20 2331 3334 3529 0a0a 0a43 6861 6e67  , #1345)...Chang
+00005640: 6573 0a7e 7e7e 7e7e 7e7e 0a0a 2a20 5468  es.~~~~~~~..* Th
+00005650: 6520 6060 4e6f 4465 6661 756c 7453 7065  e ``NoDefaultSpe
+00005660: 6369 6669 6564 6060 2063 6f6e 7374 616e  cified`` constan
+00005670: 7420 2875 7365 6420 6173 2061 2064 6566  t (used as a def
+00005680: 6175 6c74 2076 616c 7565 2066 6f72 0a20  ault value for. 
+00005690: 2074 6865 2060 6054 7261 6974 5479 7065   the ``TraitType
+000056a0: 6060 2060 6064 6566 6175 6c74 5f76 616c  `` ``default_val
+000056b0: 7565 6060 2061 7267 756d 656e 7429 2069  ue`` argument) i
+000056c0: 7320 6e6f 7720 7075 626c 6963 2c20 6d61  s now public, ma
+000056d0: 6465 0a20 2061 7661 696c 6162 6c65 2066  de.  available f
+000056e0: 726f 6d20 6060 7472 6169 7473 2e61 7069  rom ``traits.api
+000056f0: 6060 2e20 2823 3133 3834 2c20 2331 3338  ``. (#1384, #138
+00005700: 302c 2023 3133 3738 290a 2a20 5468 6520  0, #1378).* The 
+00005710: 6465 7072 6563 6174 696f 6e20 6f66 2074  deprecation of t
+00005720: 6865 2060 6054 7261 6974 4d61 7060 6020  he ``TraitMap`` 
+00005730: 7472 6169 7420 7479 7065 2068 6173 2062  trait type has b
+00005740: 6565 6e20 7265 7665 7273 6564 2c20 6265  een reversed, be
+00005750: 6361 7573 650a 2020 7468 6572 6520 6172  cause.  there ar
+00005760: 6520 6578 6973 7469 6e67 2075 7365 7320  e existing uses 
+00005770: 6f66 2060 6054 7261 6974 4d61 7060 6020  of ``TraitMap`` 
+00005780: 7468 6174 2061 7265 2068 6172 6420 746f  that are hard to
+00005790: 2072 6570 6c61 6365 2e0a 2020 4e65 7665   replace..  Neve
+000057a0: 7274 6865 6c65 7373 2c20 6974 2069 7320  rtheless, it is 
+000057b0: 7374 696c 6c20 6e6f 7420 7265 636f 6d6d  still not recomm
+000057c0: 656e 6465 6420 746f 2075 7365 2060 6054  ended to use ``T
+000057d0: 7261 6974 4d61 7060 6020 696e 206e 6577  raitMap`` in new
+000057e0: 2063 6f64 652e 0a20 2055 7365 2060 604d   code..  Use ``M
+000057f0: 6170 6060 2069 6e73 7465 6164 2e20 2823  ap`` instead. (#
+00005800: 3133 3635 290a 2a20 416e 2061 7474 656d  1365).* An attem
+00005810: 7074 2074 6f20 7573 6520 6060 5072 6566  pt to use ``Pref
+00005820: 6978 4c69 7374 6060 2077 6974 6820 616e  ixList`` with an
+00005830: 2065 6d70 7479 206c 6973 742c 206f 7220   empty list, or 
+00005840: 6060 5072 6566 6978 4d61 7060 6020 6f72  ``PrefixMap`` or
+00005850: 0a20 2060 604d 6170 6060 2077 6974 6820  .  ``Map`` with 
+00005860: 616e 2065 6d70 7479 2064 6963 7469 6f6e  an empty diction
+00005870: 6172 792c 206e 6f77 2072 6169 7365 7320  ary, now raises 
+00005880: 6060 5661 6c75 6545 7272 6f72 6060 2e20  ``ValueError``. 
+00005890: 4173 2061 2072 6573 756c 742c 0a20 2074  As a result,.  t
+000058a0: 6865 2064 6566 6175 6c74 2064 6566 6175  he default defau
+000058b0: 6c74 2076 616c 7565 2028 7768 6963 6820  lt value (which 
+000058c0: 7573 6564 2074 6f20 6265 2060 604e 6f6e  used to be ``Non
+000058d0: 6560 6029 2069 7320 616c 7761 7973 2076  e``) is always v
+000058e0: 616c 6964 2e0a 2020 2823 3133 3531 290a  alid..  (#1351).
+000058f0: 2a20 6060 5472 6169 744c 6973 7445 7665  * ``TraitListEve
+00005900: 6e74 6060 2061 7267 756d 656e 7473 2061  nt`` arguments a
+00005910: 7265 206e 6f77 206b 6579 776f 7264 206f  re now keyword o
+00005920: 6e6c 792e 2028 2331 3334 3629 0a2a 2049  nly. (#1346).* I
+00005930: 7427 7320 6e6f 206c 6f6e 6765 7220 6e65  t's no longer ne
+00005940: 6365 7373 6172 7920 746f 2073 7065 6369  cessary to speci
+00005950: 6679 2061 2074 7261 6974 2063 6f6d 7061  fy a trait compa
+00005960: 7269 736f 6e20 6d6f 6465 206f 660a 2020  rison mode of.  
+00005970: 6060 436f 6d70 6172 6973 6f6e 4d6f 6465  ``ComparisonMode
+00005980: 2e69 6465 6e74 6974 7960 6020 7768 656e  .identity`` when
+00005990: 2075 7369 6e67 2060 606f 6273 6572 7665   using ``observe
+000059a0: 6060 2074 6f20 6f62 7365 7276 6520 6974  `` to observe it
+000059b0: 656d 730a 2020 696e 2061 2060 604c 6973  ems.  in a ``Lis
+000059c0: 7460 602c 2060 6044 6963 7460 6020 6f72  t``, ``Dict`` or
+000059d0: 2060 6053 6574 6060 2e20 2823 3131 3635   ``Set``. (#1165
+000059e0: 2c20 2331 3332 382c 2023 3132 3430 290a  , #1328, #1240).
+000059f0: 0a0a 4465 7072 6563 6174 696f 6e73 0a7e  ..Deprecations.~
+00005a00: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a 2054  ~~~~~~~~~~~..* T
+00005a10: 6865 2060 6046 756e 6374 696f 6e60 6020  he ``Function`` 
+00005a20: 616e 6420 6060 4d65 7468 6f64 6060 2074  and ``Method`` t
+00005a30: 7261 6974 2074 7970 6573 2061 7265 2064  rait types are d
+00005a40: 6570 7265 6361 7465 642e 2055 7365 0a20  eprecated. Use. 
+00005a50: 2060 6043 616c 6c61 626c 6560 6020 6f72   ``Callable`` or
+00005a60: 2060 6049 6e73 7461 6e63 6560 6020 696e   ``Instance`` in
+00005a70: 7374 6561 642e 2028 2331 3339 392c 2023  stead. (#1399, #
+00005a80: 3133 3937 290a 2a20 5468 6520 6060 6564  1397).* The ``ed
+00005a90: 6974 6060 2070 6172 616d 6574 6572 2074  it`` parameter t
+00005aa0: 6f20 6060 636f 6e66 6967 7572 655f 7472  o ``configure_tr
+00005ab0: 6169 7473 6060 2068 6173 2062 6565 6e20  aits`` has been 
+00005ac0: 6465 7072 6563 6174 6564 2e20 2823 3133  deprecated. (#13
+00005ad0: 3131 290a 2a20 5468 6520 6060 556e 6974  11).* The ``Unit
+00005ae0: 7465 7374 546f 6f6c 732e 5f63 6174 6368  testTools._catch
+00005af0: 5f77 6172 6e69 6e67 7360 6020 6675 6e63  _warnings`` func
+00005b00: 7469 6f6e 2068 6173 2062 6565 6e20 6465  tion has been de
+00005b10: 7072 6563 6174 6564 2e20 2823 3133 3130  precated. (#1310
+00005b20: 290a 2a20 5468 6520 7573 6520 6f66 2074  ).* The use of t
+00005b30: 6865 2060 6043 4845 434b 5f49 4e54 4552  he ``CHECK_INTER
+00005b40: 4641 4345 5360 6020 676c 6f62 616c 2076  FACES`` global v
+00005b50: 6172 6961 626c 6520 666f 7220 6175 746f  ariable for auto
+00005b60: 6d61 7465 640a 2020 696e 7465 7266 6163  mated.  interfac
+00005b70: 6520 6368 6563 6b69 6e67 2068 6173 2062  e checking has b
+00005b80: 6565 6e20 6465 7072 6563 6174 6564 2e20  een deprecated. 
+00005b90: 2823 3132 3331 290a 0a0a 4669 7865 730a  (#1231)...Fixes.
+00005ba0: 7e7e 7e7e 7e0a 0a2a 204e 6f6e 2d60 6054  ~~~~~..* Non-``T
+00005bb0: 7261 6974 4572 726f 7260 6020 6578 6365  raitError`` exce
+00005bc0: 7074 696f 6e73 2072 6169 7365 6420 6475  ptions raised du
+00005bd0: 7269 6e67 2060 6054 7570 6c65 6060 2076  ring ``Tuple`` v
+00005be0: 616c 6964 6174 696f 6e20 6172 6520 6e6f  alidation are no
+00005bf0: 770a 2020 7072 6f70 6167 6174 6564 2e20  w.  propagated. 
+00005c00: 5072 6576 696f 7573 6c79 2074 6865 7920  Previously they 
+00005c10: 7765 7265 2063 6f6e 7665 7274 6564 2069  were converted i
+00005c20: 6e74 6f20 6060 5472 6169 7445 7272 6f72  nto ``TraitError
+00005c30: 6060 2e20 2823 3133 3933 290a 2a20 4479  ``. (#1393).* Dy
+00005c40: 6e61 6d69 6320 6060 5261 6e67 6560 6020  namic ``Range`` 
+00005c50: 616e 6420 6060 456e 756d 6060 2074 7261  and ``Enum`` tra
+00005c60: 6974 7320 6172 6520 6e6f 7720 7072 6f70  its are now prop
+00005c70: 6572 6c79 2076 616c 6964 6174 6564 0a20  erly validated. 
+00005c80: 2077 6865 6e20 696e 7369 6465 2061 2063   when inside a c
+00005c90: 6f6e 7461 696e 6572 2028 666f 7220 6578  ontainer (for ex
+00005ca0: 616d 706c 6520 6060 5475 706c 6560 6020  ample ``Tuple`` 
+00005cb0: 6f72 2060 604c 6973 7460 6029 2e20 5072  or ``List``). Pr
+00005cc0: 6576 696f 7573 6c79 0a20 206e 6f20 7661  eviously.  no va
+00005cd0: 6c69 6461 7469 6f6e 2077 6173 2070 6572  lidation was per
+00005ce0: 666f 726d 6564 2e20 2823 3133 3838 2c20  formed. (#1388, 
+00005cf0: 2331 3339 3229 0a2a 2052 656d 6f76 6520  #1392).* Remove 
+00005d00: 7468 6520 756e 7573 6564 206d 6f64 756c  the unused modul
+00005d10: 652d 6c65 7665 6c20 636f 6e73 7461 6e74  e-level constant
+00005d20: 2060 6074 7261 6974 732e 6861 735f 7472   ``traits.has_tr
+00005d30: 6169 7473 2e45 6d70 7479 4c69 7374 6060  aits.EmptyList``
+00005d40: 2e0a 2020 2823 3133 3636 290a 2a20 446f  ..  (#1366).* Do
+00005d50: 6e27 7420 6861 7264 2d63 6f64 6520 636c  n't hard-code cl
+00005d60: 6173 7320 6e61 6d65 7320 696e 2060 605f  ass names in ``_
+00005d70: 5f72 6570 725f 5f60 6020 696d 706c 656d  _repr__`` implem
+00005d80: 656e 7461 7469 6f6e 7320 6f66 0a20 2060  entations of.  `
+00005d90: 6054 7261 6974 4c69 7374 4576 656e 7460  `TraitListEvent`
+00005da0: 602c 2060 6054 7261 6974 5365 7445 7665  `, ``TraitSetEve
+00005db0: 6e74 6060 2061 6e64 2060 6054 7261 6974  nt`` and ``Trait
+00005dc0: 4469 6374 4576 656e 7460 602e 2028 2331  DictEvent``. (#1
+00005dd0: 3333 3529 0a2a 2044 6f6e 2774 206e 6f74  335).* Don't not
+00005de0: 6966 7920 6f6e 2065 6d70 7479 2060 6075  ify on empty ``u
+00005df0: 7064 6174 6560 605c 2073 206f 6620 6060  pdate``\ s of ``
+00005e00: 4469 6374 6060 2074 7261 6974 732e 2028  Dict`` traits. (
+00005e10: 2331 3330 3829 0a2a 2046 6978 2065 7863  #1308).* Fix exc
+00005e20: 6570 7469 6f6e 2072 6169 7365 6420 7768  eption raised wh
+00005e30: 656e 2061 7373 6967 6e69 6e67 2061 204e  en assigning a N
+00005e40: 756d 5079 2061 7272 6179 2074 6f20 6120  umPy array to a 
+00005e50: 6060 4c69 7374 6060 0a20 2074 7261 6974  ``List``.  trait
+00005e60: 2e20 2823 3132 3738 290a 2a20 4669 7820  . (#1278).* Fix 
+00005e70: 7573 6573 206f 6620 6465 7072 6563 6174  uses of deprecat
+00005e80: 6564 2060 606c 6f67 6765 722e 7761 726e  ed ``logger.warn
+00005e90: 6060 2066 756e 6374 696f 6e2e 2028 2331  `` function. (#1
+00005ea0: 3238 3329 0a2a 2046 6978 2061 2062 6164  283).* Fix a bad
+00005eb0: 2060 6049 6e73 7461 6e63 6560 6020 7472   ``Instance`` tr
+00005ec0: 6169 7420 6465 636c 6172 6174 696f 6e20  ait declaration 
+00005ed0: 666f 7220 6120 7072 6976 6174 6520 7472  for a private tr
+00005ee0: 6169 7420 696e 0a20 2074 6865 2060 605f  ait in.  the ``_
+00005ef0: 5472 6169 7443 6861 6e67 6543 6f6c 6c65  TraitChangeColle
+00005f00: 6374 6f72 6060 2063 6c61 7373 2e20 2823  ctor`` class. (#
+00005f10: 3134 3131 290a 0a0a 446f 6375 6d65 6e74  1411)...Document
+00005f20: 6174 696f 6e0a 7e7e 7e7e 7e7e 7e7e 7e7e  ation.~~~~~~~~~~
+00005f30: 7e7e 7e0a 0a2a 2041 6464 2022 5475 746f  ~~~..* Add "Tuto
+00005f40: 7269 616c 2220 7365 6374 696f 6e20 746f  rial" section to
+00005f50: 2074 6865 206d 6169 6e20 646f 6375 6d65   the main docume
+00005f60: 6e74 6174 696f 6e2c 2062 6173 6564 206f  ntation, based o
+00005f70: 6e20 7468 650a 2020 6e65 7720 6060 7472  n the.  new ``tr
+00005f80: 6169 7473 2e65 7861 6d70 6c65 7360 6020  aits.examples`` 
+00005f90: 7475 746f 7269 616c 2063 6f6e 7465 6e74  tutorial content
+00005fa0: 2e20 2823 3133 3734 290a 2a20 436c 6172  . (#1374).* Clar
+00005fb0: 6966 7920 7468 6174 206f 6e6c 7920 7468  ify that only th
+00005fc0: 6520 6060 6170 6960 6020 6d6f 6475 6c65  e ``api`` module
+00005fd0: 7320 7368 6f75 6c64 2062 6520 7573 6564  s should be used
+00005fe0: 2066 6f72 2069 6d70 6f72 7473 2e20 2823   for imports. (#
+00005ff0: 3133 3837 290a 2a20 5570 6461 7465 2063  1387).* Update c
+00006000: 6f70 7972 6967 6874 2068 6561 6465 7220  opyright header 
+00006010: 656e 6420 7965 6172 732e 2028 2331 3337  end years. (#137
+00006020: 3629 0a2a 2055 7064 6174 6520 636f 6e74  6).* Update cont
+00006030: 656e 7473 206f 6620 6060 696d 6167 655f  ents of ``image_
+00006040: 4c49 4345 4e53 452e 7478 7460 602e 2028  LICENSE.txt``. (
+00006050: 2331 3336 3229 0a2a 2052 656d 6f76 6520  #1362).* Remove 
+00006060: 6d65 6e74 696f 6e73 206f 6620 7468 6520  mentions of the 
+00006070: 7265 6d6f 7665 6420 6675 6e63 7469 6f6e  removed function
+00006080: 7320 6060 6164 6170 7473 6060 2061 6e64  s ``adapts`` and
+00006090: 2060 6069 6d70 6c65 6d65 6e74 7360 6020   ``implements`` 
+000060a0: 6672 6f6d 0a20 2074 6865 2065 7861 6d70  from.  the examp
+000060b0: 6c65 7320 616e 6420 7475 746f 7269 616c  les and tutorial
+000060c0: 2e20 2823 3133 3637 290a 2a20 4d6f 7665  . (#1367).* Move
+000060d0: 2054 7261 6974 7320 696e 7472 6f64 7563   Traits introduc
+000060e0: 7469 6f6e 2064 6573 6372 6970 7469 6f6e  tion description
+000060f0: 2074 6f20 6060 696e 6465 782e 7273 7460   to ``index.rst`
+00006100: 602e 2028 2331 3335 3829 0a2a 2046 6978  `. (#1358).* Fix
+00006110: 2070 6174 6820 746f 2045 6e74 686f 7567   path to Enthoug
+00006120: 6874 206c 6f67 6f20 7768 656e 2062 7569  ht logo when bui
+00006130: 6c64 696e 6720 646f 6373 6574 2e20 2823  lding docset. (#
+00006140: 3132 3835 290a 2a20 4669 7820 7468 6520  1285).* Fix the 
+00006150: 6060 7472 6169 745f 646f 6375 6d65 6e74  ``trait_document
+00006160: 6572 6060 2065 7874 656e 7369 6f6e 2074  er`` extension t
+00006170: 6f20 6265 206c 6573 7320 6672 6167 696c  o be less fragil
+00006180: 652e 2028 2331 3234 3729 0a2a 2041 6464  e. (#1247).* Add
+00006190: 2075 7365 7220 6d61 6e75 616c 2064 6f63   user manual doc
+000061a0: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
+000061b0: 6865 2060 6049 6e73 7461 6e63 6560 6020  he ``Instance`` 
+000061c0: 7472 6169 7420 7479 7065 2e20 2823 3133  trait type. (#13
+000061d0: 3935 290a 2a20 446f 6375 6d65 6e74 2074  95).* Document t
+000061e0: 6861 7420 7468 6520 6060 4c69 7374 6060  hat the ``List``
+000061f0: 2c20 6060 4469 6374 6060 2061 6e64 2060  , ``Dict`` and `
+00006200: 6053 6574 6060 2074 7261 6974 2074 7970  `Set`` trait typ
+00006210: 6573 2063 6f70 7920 6f6e 0a20 2061 7373  es copy on.  ass
+00006220: 6967 6e6d 656e 742e 2028 2331 3430 3229  ignment. (#1402)
+00006230: 0a2a 2056 6172 696f 7573 206f 7468 6572  .* Various other
+00006240: 206d 696e 6f72 2069 6d70 726f 7665 6d65   minor improveme
+00006250: 6e74 732c 2074 7970 6f20 6669 7865 732c  nts, typo fixes,
+00006260: 2061 6e64 206f 7468 6572 2064 6f63 756d   and other docum
+00006270: 656e 7461 7469 6f6e 2066 6978 6573 2e0a  entation fixes..
+00006280: 2020 2823 3133 3936 2c20 2331 3338 332c    (#1396, #1383,
+00006290: 2023 3133 3831 2c20 2331 3338 342c 2023   #1381, #1384, #
+000062a0: 3132 3932 2c20 2331 3335 352c 2023 3133  1292, #1355, #13
+000062b0: 3530 2c20 2331 3331 392c 2023 3132 3932  50, #1319, #1292
+000062c0: 2c20 2331 3430 3129 0a0a 0a43 6c65 616e  , #1401)...Clean
+000062d0: 7570 2061 6e64 206f 7468 6572 206d 6169  up and other mai
+000062e0: 6e74 656e 616e 6365 0a7e 7e7e 7e7e 7e7e  ntenance.~~~~~~~
+000062f0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00006300: 7e7e 7e7e 7e7e 0a0a 2a20 5265 6d6f 7665  ~~~~~~..* Remove
+00006310: 2064 6561 6420 636f 6465 2e20 2823 3132   dead code. (#12
+00006320: 3831 290a 2a20 5570 6461 7465 2060 6073  81).* Update ``s
+00006330: 7570 6572 6060 2075 7361 6765 2074 6f20  uper`` usage to 
+00006340: 7468 6520 7573 7561 6c20 5079 7468 6f6e  the usual Python
+00006350: 2033 2061 7267 756d 656e 742d 6c65 7373   3 argument-less
+00006360: 2070 6174 7465 726e 2e20 2823 3132 3830   pattern. (#1280
+00006370: 290a 2a20 5265 6d6f 7665 2070 6572 2d69  ).* Remove per-i
+00006380: 6d70 6f72 7420 6060 2320 6e6f 7161 6060  mport ``# noqa``
+00006390: 2063 6f6d 6d65 6e74 7320 696e 2060 6061   comments in ``a
+000063a0: 7069 6060 206d 6f64 756c 6573 2069 6e20  pi`` modules in 
+000063b0: 6661 766f 7572 206f 660a 2020 7065 722d  favour of.  per-
+000063c0: 6669 6c65 2069 676e 6f72 6573 2069 6e20  file ignores in 
+000063d0: 7468 6520 6060 666c 616b 6538 6060 2063  the ``flake8`` c
+000063e0: 6f6e 6669 6775 7261 7469 6f6e 2e20 2823  onfiguration. (#
+000063f0: 3132 3639 290a 2a20 5265 6d6f 7665 206f  1269).* Remove o
+00006400: 7574 2d6f 662d 6461 7465 2061 6e64 206e  ut-of-date and n
+00006410: 6f6e 2d66 756e 6374 696f 6e61 6c20 636f  on-functional co
+00006420: 7665 7261 6765 2062 6164 6765 2066 726f  verage badge fro
+00006430: 6d20 5245 4144 4d45 2e20 2823 3132 3633  m README. (#1263
+00006440: 290a 2a20 5265 6e61 6d65 2060 605f 695f  ).* Rename ``_i_
+00006450: 6f62 7365 7276 6162 6c65 6060 206d 6f64  observable`` mod
+00006460: 756c 6520 746f 2060 6069 5f6f 6273 6572  ule to ``i_obser
+00006470: 7661 626c 6560 602e 2028 2331 3239 3629  vable``. (#1296)
+00006480: 0a2a 2052 6566 6163 746f 7220 616e 6420  .* Refactor and 
+00006490: 7369 6d70 6c69 6679 206d 6574 686f 6420  simplify method 
+000064a0: 6368 6563 6b73 2e20 2823 3131 3736 290a  checks. (#1176).
+000064b0: 2a20 4669 7820 7479 706f 2069 6e20 6f70  * Fix typo in op
+000064c0: 7469 6f6e 616c 5f64 6570 656e 6465 6e63  tional_dependenc
+000064d0: 6965 7320 636f 6d6d 656e 742e 2028 2331  ies comment. (#1
+000064e0: 3233 3529 0a2a 2055 7365 2043 6f6d 7061  235).* Use Compa
+000064f0: 7269 736f 6e4d 6f64 6520 636f 6e73 7461  risonMode consta
+00006500: 6e74 7320 696e 7374 6561 6420 6f66 206d  nts instead of m
+00006510: 6167 6963 206e 756d 6265 7273 2e20 2823  agic numbers. (#
+00006520: 3132 3239 290a 0a0a 5465 7374 2073 7569  1229)...Test sui
+00006530: 7465 0a7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a  te.~~~~~~~~~~..*
+00006540: 2050 7265 7665 6e74 2074 6573 745f 656e   Prevent test_en
+00006550: 756d 2066 6169 6c75 7265 7320 6966 2074  um failures if t
+00006560: 7261 6974 7375 6920 6f72 2047 5549 2074  raitsui or GUI t
+00006570: 6f6f 6c6b 6974 2061 7265 206e 6f74 2069  oolkit are not i
+00006580: 6e73 7461 6c6c 6564 2e0a 2020 2823 3133  nstalled..  (#13
+00006590: 3439 290a 2a20 5465 7374 7320 7468 6174  49).* Tests that
+000065a0: 2072 6571 7569 7265 2060 6070 6b67 5f72   require ``pkg_r
+000065b0: 6573 6f75 7263 6573 6060 2061 7265 2073  esources`` are s
+000065c0: 6b69 7070 6564 2069 6620 6060 7365 7475  kipped if ``setu
+000065d0: 7074 6f6f 6c73 6060 2069 7320 6e6f 740a  ptools`` is not.
+000065e0: 2020 696e 7374 616c 6c65 642e 2028 2331    installed. (#1
+000065f0: 3330 3129 0a2a 2046 6978 2061 6e20 6f72  301).* Fix an or
+00006600: 6465 722d 6465 7065 6e64 656e 6379 2062  der-dependency b
+00006610: 7567 2069 6e20 7468 6520 6060 7465 7374  ug in the ``test
+00006620: 5f73 7562 636c 6173 7365 735f 7765 616b  _subclasses_weak
+00006630: 7265 6660 6020 7265 6772 6573 7369 6f6e  ref`` regression
+00006640: 0a20 2074 6573 742e 2028 2331 3239 3029  .  test. (#1290)
+00006650: 0a2a 2046 6978 2061 2074 7970 6f20 696e  .* Fix a typo in
+00006660: 2061 2074 6573 7420 6d65 7468 6f64 206e   a test method n
+00006670: 616d 652e 2028 2331 3330 3929 0a2a 2056  ame. (#1309).* V
+00006680: 6172 696f 7573 2061 6464 6974 696f 6e61  arious additiona
+00006690: 6c20 6f72 2069 6d70 726f 7665 6420 7465  l or improved te
+000066a0: 7374 7320 666f 7220 6578 6973 7469 6e67  sts for existing
+000066b0: 2063 6f64 652e 0a20 2028 2331 3335 392c   code..  (#1359,
+000066c0: 2023 3133 3336 2c20 2331 3333 302c 2023   #1336, #1330, #
+000066d0: 3132 3438 2c20 2331 3232 352c 2023 3132  1248, #1225, #12
+000066e0: 3038 2c20 2331 3230 3929 0a0a 0a42 7569  08, #1209)...Bui
+000066f0: 6c64 2061 6e64 2064 6576 656c 6f70 6d65  ld and developme
+00006700: 6e74 2077 6f72 6b66 6c6f 7720 6368 616e  nt workflow chan
+00006710: 6765 730a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ges.~~~~~~~~~~~~
+00006720: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00006730: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20 5472  ~~~~~~~~~~..* Tr
+00006740: 6169 7473 206e 6f77 2075 7365 7320 4769  aits now uses Gi
+00006750: 7448 7562 2041 6374 696f 6e73 2066 6f72  tHub Actions for
+00006760: 2063 6f6e 7469 6e75 6f75 7320 696e 7465   continuous inte
+00006770: 6772 6174 696f 6e2e 2054 6865 2054 7261  gration. The Tra
+00006780: 7669 7320 4349 0a20 2061 6e64 2041 7070  vis CI.  and App
+00006790: 7665 796f 7220 636f 6e66 6967 7572 6174  veyor configurat
+000067a0: 696f 6e73 2068 6176 6520 6265 656e 2072  ions have been r
+000067b0: 656d 6f76 6564 2e20 2823 3132 3936 2c20  emoved. (#1296, 
+000067c0: 2331 3336 3029 0a2a 2043 4920 7275 6e73  #1360).* CI runs
+000067d0: 2061 7265 206e 6f20 6c6f 6e67 6572 2062   are no longer b
+000067e0: 6173 6564 206f 6e20 4544 4d2e 2028 2338  ased on EDM. (#8
+000067f0: 3738 290a 2a20 4e65 7720 4349 2072 756e  78).* New CI run
+00006800: 2066 6f72 2074 6865 2063 6f72 6520 7465   for the core te
+00006810: 7374 2073 7569 7465 2c20 7769 7468 6f75  st suite, withou
+00006820: 7420 616e 7920 6f70 7469 6f6e 616c 2064  t any optional d
+00006830: 6570 656e 6465 6e63 6965 732e 0a20 2028  ependencies..  (
+00006840: 2331 3331 3429 0a2a 2054 6573 7420 5079  #1314).* Test Py
+00006850: 7468 6f6e 2033 2e39 2069 6e20 7468 6520  thon 3.9 in the 
+00006860: 636f 6e74 696e 756f 7573 2069 6e74 6567  continuous integ
+00006870: 7261 7469 6f6e 2028 616e 6420 6472 6f70  ration (and drop
+00006880: 2074 6573 7473 2066 6f72 2050 7974 686f   tests for Pytho
+00006890: 6e0a 2020 332e 3520 616e 6420 6f6c 6465  n.  3.5 and olde
+000068a0: 7229 2e20 2823 3133 3236 2c20 2331 3331  r). (#1326, #131
+000068b0: 332c 202c 2023 3133 3033 290a 2a20 4d61  3, , #1303).* Ma
+000068c0: 6b65 2060 6074 7261 6974 732e 6578 616d  ke ``traits.exam
+000068d0: 706c 6573 6060 2069 6e74 6f20 6120 7061  ples`` into a pa
+000068e0: 636b 6167 652e 2028 2331 3334 3829 0a2a  ckage. (#1348).*
+000068f0: 204d 616b 6520 6578 616d 706c 6573 2064   Make examples d
+00006900: 6972 6563 746f 7269 6573 2060 6066 6c61  irectories ``fla
+00006910: 6b65 3860 602d 636c 6561 6e2e 2028 2331  ke8``-clean. (#1
+00006920: 3335 3329 0a2a 2046 6978 2065 7861 6d70  353).* Fix examp
+00006930: 6c65 7320 7061 636b 6167 696e 6720 6e69  les packaging ni
+00006940: 742e 2028 2331 3336 3329 0a2a 2053 7570  t. (#1363).* Sup
+00006950: 706f 7274 2060 602d 6860 6020 666f 7220  port ``-h`` for 
+00006960: 6765 7474 696e 6720 6865 6c70 2069 6e20  getting help in 
+00006970: 6060 6574 7374 6f6f 6c2e 7079 6060 2e20  ``etstool.py``. 
+00006980: 2823 3133 3437 290a 2a20 4164 6420 6060  (#1347).* Add ``
+00006990: 7368 656c 6c60 6020 636f 6d6d 616e 6420  shell`` command 
+000069a0: 746f 2060 6065 7473 746f 6f6c 2e70 7960  to ``etstool.py`
+000069b0: 602e 2028 2331 3239 3329 0a2a 2055 7365  `. (#1293).* Use
+000069c0: 2074 6865 2060 6066 6c61 6b65 385f 6574   the ``flake8_et
+000069d0: 7360 6020 7061 636b 6167 6520 696e 2070  s`` package in p
+000069e0: 6c61 6365 206f 6620 7468 6520 6c6f 6361  lace of the loca
+000069f0: 6c20 6060 636f 7079 7269 6768 745f 6865  l ``copyright_he
+00006a00: 6164 6572 6060 0a20 2070 6163 6b61 6765  ader``.  package
+00006a10: 2e0a 2020 5468 6520 6060 636f 7079 7269  ..  The ``copyri
+00006a20: 6768 745f 6865 6164 6572 6060 2070 6163  ght_header`` pac
+00006a30: 6b61 6765 2068 6173 2062 6565 6e20 7265  kage has been re
+00006a40: 6d6f 7665 642e 2028 2331 3334 3129 0a2a  moved. (#1341).*
+00006a50: 2041 6464 2073 6372 6970 7420 6060 6368   Add script ``ch
+00006a60: 6563 6b5f 6f62 7365 7276 655f 7469 6d69  eck_observe_timi
+00006a70: 6e67 2e70 7960 6020 746f 2062 656e 6368  ng.py`` to bench
+00006a80: 6d61 726b 2070 6572 666f 726d 616e 6365  mark performance
+00006a90: 206f 660a 2020 6060 6f62 7365 7276 6560   of.  ``observe`
+00006aa0: 6020 746f 2063 6f6d 7061 7265 2077 6974  ` to compare wit
+00006ab0: 6820 6060 6f6e 5f74 7261 6974 5f63 6861  h ``on_trait_cha
+00006ac0: 6e67 6560 602e 2028 2331 3333 3129 0a2a  nge``. (#1331).*
+00006ad0: 2043 6f72 7265 6374 2074 6865 206d 696e   Correct the min
+00006ae0: 696d 756d 2053 7068 696e 7820 7665 7273  imum Sphinx vers
+00006af0: 696f 6e20 696e 2052 4541 444d 452e 2028  ion in README. (
+00006b00: 2331 3231 362c 2023 3133 3230 290a 2a20  #1216, #1320).* 
+00006b10: 5265 7374 7269 6374 2053 7068 696e 7820  Restrict Sphinx 
+00006b20: 7665 7273 696f 6e20 746f 2061 766f 6964  version to avoid
+00006b30: 2062 7567 6779 2076 6572 7369 6f6e 732e   buggy versions.
+00006b40: 2028 2331 3237 3629 0a2a 204d 616b 6520   (#1276).* Make 
+00006b50: 6060 6d79 7079 6060 2061 6e20 6f70 7469  ``mypy`` an opti
+00006b60: 6f6e 616c 2064 6570 656e 6465 6e63 792e  onal dependency.
+00006b70: 2028 2331 3238 3929 0a2a 2053 7065 6564   (#1289).* Speed
+00006b80: 2075 7020 4349 2062 7569 6c64 7320 666f   up CI builds fo
+00006b90: 7220 5472 6176 6973 2061 6e64 2041 7070  r Travis and App
+00006ba0: 7665 796f 7220 6279 2063 6163 6869 6e67  veyor by caching
+00006bb0: 2074 6865 2060 6070 6970 6060 2064 6972   the ``pip`` dir
+00006bc0: 6563 746f 7279 0a20 2028 6e6f 7720 7265  ectory.  (now re
+00006bd0: 6475 6e64 616e 7429 2e20 2823 3132 3431  dundant). (#1241
+00006be0: 290a 2a20 4164 6420 6175 746f 6d61 7465  ).* Add automate
+00006bf0: 6420 7768 6565 6c20 616e 6420 7364 6973  d wheel and sdis
+00006c00: 7420 6275 696c 6469 6e67 2066 6f72 2054  t building for T
+00006c10: 7261 6974 7320 7265 6c65 6173 6573 2e20  raits releases. 
+00006c20: 2823 3134 3034 2c20 2331 3239 3129 0a2a  (#1404, #1291).*
+00006c30: 2041 6464 2063 726f 6e2d 6a6f 6220 776f   Add cron-job wo
+00006c40: 726b 666c 6f77 2074 6f20 7265 6775 6c61  rkflow to regula
+00006c50: 726c 7920 7465 7374 2069 6e73 7461 6c6c  rly test install
+00006c60: 206f 6620 7468 6520 6c61 7465 7374 2072   of the latest r
+00006c70: 656c 6561 7365 730a 2020 6672 6f6d 2050  eleases.  from P
+00006c80: 7950 492e 2028 2331 3430 3629 0a0a 0a52  yPI. (#1406)...R
+00006c90: 656c 6561 7365 2036 2e31 2e31 0a2d 2d2d  elease 6.1.1.---
+00006ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5265 6c65  ----------..Rele
+00006cb0: 6173 6564 3a20 3230 3230 2d30 372d 3233  ased: 2020-07-23
+00006cc0: 0a0a 5472 6169 7473 2036 2e31 2e31 2069  ..Traits 6.1.1 i
+00006cd0: 7320 6120 6275 6766 6978 2072 656c 6561  s a bugfix relea
+00006ce0: 7365 2066 6978 696e 6720 6120 6861 6e64  se fixing a hand
+00006cf0: 6675 6c20 6f66 206d 696e 6f72 2064 6f63  ful of minor doc
+00006d00: 756d 656e 7461 7469 6f6e 2061 6e64 0a74  umentation and.t
+00006d10: 6573 742d 7265 6c61 7465 6420 6973 7375  est-related issu
+00006d20: 6573 2077 6974 6820 7468 6520 5472 6169  es with the Trai
+00006d30: 7473 2036 2e31 2e30 2072 656c 6561 7365  ts 6.1.0 release
+00006d40: 2e20 5468 6572 6520 6172 6520 6e6f 2041  . There are no A
+00006d50: 5049 2d62 7265 616b 696e 670a 6368 616e  PI-breaking.chan
+00006d60: 6765 7320 696e 2074 6869 7320 7265 6c65  ges in this rele
+00006d70: 6173 652e 2049 7427 7320 7265 636f 6d6d  ase. It's recomm
+00006d80: 656e 6465 6420 7468 6174 2061 6c6c 2075  ended that all u
+00006d90: 7365 7273 206f 6620 5472 6169 7473 2036  sers of Traits 6
+00006da0: 2e31 2e30 0a75 7067 7261 6465 2074 6f20  .1.0.upgrade to 
+00006db0: 5472 6169 7473 2036 2e31 2e31 2e0a 0a46  Traits 6.1.1...F
+00006dc0: 6978 6573 0a7e 7e7e 7e7e 0a0a 2a20 446f  ixes.~~~~~..* Do
+00006dd0: 6e27 7420 6d75 7461 7465 2067 6c6f 6261  n't mutate globa
+00006de0: 6c20 7374 6174 6520 6174 2069 6d70 6f72  l state at impor
+00006df0: 7420 7469 6d65 2069 6e20 6120 7465 7374  t time in a test
+00006e00: 206d 6f64 756c 652e 2028 2331 3232 3229   module. (#1222)
+00006e10: 0a2a 2053 7461 6e64 6172 6469 7a65 2061  .* Standardize a
+00006e20: 6e64 2066 6978 2063 6f70 7972 6967 6874  nd fix copyright
+00006e30: 2079 6561 7273 2069 6e20 736f 7572 6365   years in source
+00006e40: 2066 696c 6573 2e20 2823 3132 3237 2c20   files. (#1227, 
+00006e50: 2331 3139 3829 0a2a 2046 6978 2074 7261  #1198).* Fix tra
+00006e60: 6974 2d64 6f63 756d 656e 7465 7220 6578  it-documenter ex
+00006e70: 7465 6e73 696f 6e20 7465 7374 7320 666f  tension tests fo
+00006e80: 7220 5370 6869 6e78 2033 2e31 2e20 2823  r Sphinx 3.1. (#
+00006e90: 3132 3036 290a 2a20 4669 7820 7472 6169  1206).* Fix trai
+00006ea0: 742d 646f 6375 6d65 6e74 6572 2065 7874  t-documenter ext
+00006eb0: 656e 7369 6f6e 2074 6f20 6861 6e64 6c65  ension to handle
+00006ec0: 2070 726f 7065 7274 6965 7320 636f 7272   properties corr
+00006ed0: 6563 746c 792e 2028 2331 3234 3629 0a0a  ectly. (#1246)..
+00006ee0: 446f 6375 6d65 6e74 6174 696f 6e20 6669  Documentation fi
+00006ef0: 7865 730a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  xes.~~~~~~~~~~~~
+00006f00: 7e7e 7e7e 7e7e 7e0a 0a2a 2045 7870 616e  ~~~~~~~..* Expan
+00006f10: 6420 7573 6572 206d 616e 7561 6c20 746f  d user manual to
+00006f20: 206d 656e 7469 6f6e 2064 6973 7061 7463   mention dispatc
+00006f30: 682e 2028 2331 3139 3529 0a2a 2046 6978  h. (#1195).* Fix
+00006f40: 2073 6f6d 6520 7370 656c 6c69 6e67 2061   some spelling a
+00006f50: 6e64 2067 7261 6d6d 6172 2065 7272 6f72  nd grammar error
+00006f60: 7320 696e 2074 6865 2075 7365 7220 6d61  s in the user ma
+00006f70: 6e75 616c 2e20 2823 3132 3130 290a 2a20  nual. (#1210).* 
+00006f80: 4669 7820 6465 7363 7269 7074 696f 6e20  Fix description 
+00006f90: 696e 2052 4541 444d 4520 746f 206d 6174  in README to mat
+00006fa0: 6368 2074 6865 206f 6e65 2069 6e20 7468  ch the one in th
+00006fb0: 6520 7365 7475 7020 7363 7269 7074 2e20  e setup script. 
+00006fc0: 2823 3132 3139 290a 2a20 5570 6461 7465  (#1219).* Update
+00006fd0: 2050 7950 4920 6c69 6e6b 7320 616e 6420   PyPI links and 
+00006fe0: 6361 7069 7461 6c69 7a61 7469 6f6e 2069  capitalization i
+00006ff0: 6e20 5245 4144 4d45 2e72 7374 2e20 2823  n README.rst. (#
+00007000: 3132 3530 290a 2a20 4669 7820 7573 6572  1250).* Fix user
+00007010: 206d 616e 7561 6c20 6d65 6e74 696f 6e69   manual mentioni
+00007020: 6e67 2061 206e 6f6e 6578 6973 7469 6e67  ng a nonexisting
+00007030: 2066 6561 7475 7265 2069 6e20 6d65 7461   feature in meta
+00007040: 6461 7461 2066 696c 7465 722e 2028 2331  data filter. (#1
+00007050: 3230 3729 0a2a 2046 6978 2074 7970 6f20  207).* Fix typo 
+00007060: 696e 2063 6f6d 6d65 6e74 2069 6e20 6f70  in comment in op
+00007070: 7469 6f6e 616c 5f64 6570 656e 6465 6e63  tional_dependenc
+00007080: 6965 732e 2028 2331 3233 3529 0a0a 0a52  ies. (#1235)...R
+00007090: 656c 6561 7365 2036 2e31 2e30 0a2d 2d2d  elease 6.1.0.---
+000070a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5265 6c65  ----------..Rele
+000070b0: 6173 6564 3a20 3230 3230 2d30 362d 3035  ased: 2020-06-05
+000070c0: 0a0a 5468 6520 5472 6169 7473 206c 6962  ..The Traits lib
+000070d0: 7261 7279 2069 7320 6120 666f 756e 6461  rary is a founda
+000070e0: 7469 6f6e 616c 2063 6f6d 706f 6e65 6e74  tional component
+000070f0: 206f 6620 7468 6520 456e 7468 6f75 6768   of the Enthough
+00007100: 7420 546f 6f6c 2053 7569 7465 2e20 4974  t Tool Suite. It
+00007110: 0a70 726f 7669 6465 7320 6f62 7365 7276  .provides observ
+00007120: 6162 6c65 2c20 7479 7065 6420 6174 7472  able, typed attr
+00007130: 6962 7574 6573 2066 6f72 2050 7974 686f  ibutes for Pytho
+00007140: 6e20 636c 6173 7365 732c 206d 616b 696e  n classes, makin
+00007150: 6720 7468 6f73 6520 636c 6173 7365 730a  g those classes.
+00007160: 7375 6974 6162 6c65 2066 6f72 2065 7665  suitable for eve
+00007170: 6e74 2d64 7269 7665 6e20 6461 7461 666c  nt-driven datafl
+00007180: 6f77 2070 726f 6772 616d 6d69 6e67 2061  ow programming a
+00007190: 6e64 2066 6f72 2069 6d6d 6564 6961 7465  nd for immediate
+000071a0: 2075 7365 2061 7320 6d6f 6465 6c73 0a66   use as models.f
+000071b0: 6f72 2067 7261 7068 6963 616c 2075 7365  or graphical use
+000071c0: 7220 696e 7465 7266 6163 6573 2c20 6c69  r interfaces, li
+000071d0: 6b65 2074 686f 7365 2070 726f 7669 6465  ke those provide
+000071e0: 6420 6279 2074 6865 2054 7261 6974 7355  d by the TraitsU
+000071f0: 4920 6c69 6272 6172 792e 0a0a 5472 6169  I library...Trai
+00007200: 7473 2036 2e31 2069 7320 7468 6520 6c61  ts 6.1 is the la
+00007210: 7465 7374 2066 6561 7475 7265 2072 656c  test feature rel
+00007220: 6561 7365 2069 6e20 7468 6520 5472 6169  ease in the Trai
+00007230: 7473 2036 2073 6572 6965 732c 2061 6e64  ts 6 series, and
+00007240: 2063 6f6e 7461 696e 730a 7365 7665 7261   contains.severa
+00007250: 6c20 6d61 6a6f 7220 696d 7072 6f76 656d  l major improvem
+00007260: 656e 7473 2e0a 0a48 6967 686c 6967 6874  ents...Highlight
+00007270: 7320 6f66 2074 6869 7320 7265 6c65 6173  s of this releas
+00007280: 650a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  e.~~~~~~~~~~~~~~
+00007290: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20  ~~~~~~~~~~~~..* 
+000072a0: 4120 6e65 7720 3a6d 6f64 3a60 6f62 7365  A new :mod:`obse
+000072b0: 7276 6174 696f 6e20 3c74 7261 6974 732e  rvation <traits.
+000072c0: 6f62 7365 7276 6174 696f 6e3e 6020 6672  observation>` fr
+000072d0: 616d 6577 6f72 6b20 666f 7220 6f62 7365  amework for obse
+000072e0: 7276 696e 6720 7472 6169 7465 640a 2020  rving traited.  
+000072f0: 6174 7472 6962 7574 6573 2061 6e64 206f  attributes and o
+00007300: 7468 6572 206f 6273 6572 7661 626c 6520  ther observable 
+00007310: 6f62 6a65 6374 7320 6861 7320 6265 656e  objects has been
+00007320: 2069 6e74 726f 6475 6365 642e 2054 6869   introduced. Thi
+00007330: 7320 6973 2069 6e74 656e 6465 640a 2020  s is intended.  
+00007340: 746f 2070 726f 7669 6465 2061 2066 756c  to provide a ful
+00007350: 6c20 7265 706c 6163 656d 656e 7420 666f  l replacement fo
+00007360: 7220 7468 6520 6578 6973 7469 6e67 203a  r the existing :
+00007370: 6675 6e63 3a60 6f6e 5f74 7261 6974 5f63  func:`on_trait_c
+00007380: 6861 6e67 6560 0a20 206d 6563 6861 6e69  hange`.  mechani
+00007390: 736d 2c20 616e 6420 6169 6d73 2074 6f20  sm, and aims to 
+000073a0: 6669 7820 6120 6e75 6d62 6572 206f 6620  fix a number of 
+000073b0: 6675 6e64 616d 656e 7461 6c20 666c 6177  fundamental flaw
+000073c0: 7320 616e 6420 6c69 6d69 7461 7469 6f6e  s and limitation
+000073d0: 7320 6f66 0a20 2074 6861 7420 6d65 6368  s of.  that mech
+000073e0: 616e 6973 6d2e 2053 6565 2074 6865 203a  anism. See the :
+000073f0: 7265 663a 606f 6273 6572 7665 2d6e 6f74  ref:`observe-not
+00007400: 6966 6963 6174 696f 6e60 2073 6563 7469  ification` secti
+00007410: 6f6e 206f 660a 2020 7468 6520 7573 6572  on of.  the user
+00007420: 206d 616e 7561 6c20 666f 7220 616e 2069   manual for an i
+00007430: 6e74 726f 6475 6374 696f 6e20 746f 2074  ntroduction to t
+00007440: 6869 7320 6672 616d 6577 6f72 6b2e 0a0a  his framework...
+00007450: 2a20 4e65 7720 3a63 6c61 7373 3a60 7e74  * New :class:`~t
+00007460: 7261 6974 732e 7472 6169 745f 6c69 7374  raits.trait_list
+00007470: 5f6f 626a 6563 742e 5472 6169 744c 6973  _object.TraitLis
+00007480: 7460 2c0a 2020 3a63 6c61 7373 3a60 7e74  t`,.  :class:`~t
+00007490: 7261 6974 732e 7472 6169 745f 6469 6374  raits.trait_dict
+000074a0: 5f6f 626a 6563 742e 5472 6169 7444 6963  _object.TraitDic
+000074b0: 7460 2061 6e64 0a20 203a 636c 6173 733a  t` and.  :class:
+000074c0: 607e 7472 6169 7473 2e74 7261 6974 5f73  `~traits.trait_s
+000074d0: 6574 5f6f 626a 6563 742e 5472 6169 7453  et_object.TraitS
+000074e0: 6574 6020 636c 6173 7365 7320 6861 7665  et` classes have
+000074f0: 2062 6565 6e20 6164 6465 642c 0a20 2073   been added,.  s
+00007500: 7562 636c 6173 7369 6e67 2050 7974 686f  ubclassing Pytho
+00007510: 6e27 7320 6275 696c 742d 696e 203a 636c  n's built-in :cl
+00007520: 6173 733a 6070 7974 686f 6e3a 6c69 7374  ass:`python:list
+00007530: 602c 203a 636c 6173 733a 6070 7974 686f  `, :class:`pytho
+00007540: 6e3a 6469 6374 6020 616e 640a 2020 3a63  n:dict` and.  :c
+00007550: 6c61 7373 3a60 7079 7468 6f6e 3a73 6574  lass:`python:set
+00007560: 6020 2872 6573 7065 6374 6976 656c 7929  ` (respectively)
+00007570: 2e20 496e 7374 616e 6365 7320 6f66 2074  . Instances of t
+00007580: 6865 7365 2063 6c61 7373 6573 2061 7265  hese classes are
+00007590: 206f 6273 6572 7661 626c 650a 2020 6f62   observable.  ob
+000075a0: 6a65 6374 7320 696e 2074 6865 6972 206f  jects in their o
+000075b0: 776e 2072 6967 6874 2c20 616e 6420 6974  wn right, and it
+000075c0: 2773 2070 6f73 7369 626c 6520 746f 2061  's possible to a
+000075d0: 7474 6163 6820 6f62 7365 7276 6572 7320  ttach observers 
+000075e0: 746f 2074 6865 6d0a 2020 6469 7265 6374  to them.  direct
+000075f0: 6c79 2e20 5468 6573 6520 636c 6173 7365  ly. These classe
+00007600: 7320 7765 7265 2070 7269 6d61 7269 6c79  s were primarily
+00007610: 2069 6e74 726f 6475 6365 6420 746f 2073   introduced to s
+00007620: 7570 706f 7274 2074 6865 206e 6577 0a20  upport the new. 
+00007630: 206f 6273 6572 7661 7469 6f6e 2066 7261   observation fra
+00007640: 6d65 776f 726b 2c20 616e 6420 6172 6520  mework, and are 
+00007650: 6e6f 7420 6578 7065 6374 6564 2074 6f20  not expected to 
+00007660: 6265 2075 7365 6420 6469 7265 6374 6c79  be used directly
+00007670: 2e20 5468 6520 4150 4920 666f 720a 2020  . The API for.  
+00007680: 7468 6573 6520 6f62 6a65 6374 7320 616e  these objects an
+00007690: 6420 7468 6569 7220 6e6f 7469 6669 6361  d their notifica
+000076a0: 7469 6f6e 2073 7973 7465 6d20 6973 2070  tion system is p
+000076b0: 726f 7669 7369 6f6e 616c 2c20 616e 6420  rovisional, and 
+000076c0: 6d61 7920 6368 616e 6765 2069 6e0a 2020  may change in.  
+000076d0: 6120 6675 7475 7265 2054 7261 6974 7320  a future Traits 
+000076e0: 7265 6c65 6173 652e 0a0a 2a20 4120 6e65  release...* A ne
+000076f0: 7720 3a63 6c61 7373 3a60 2e55 6e69 6f6e  w :class:`.Union
+00007700: 6020 7472 6169 7420 7479 7065 2068 6173  ` trait type has
+00007710: 2062 6565 6e20 6164 6465 642e 2054 6869   been added. Thi
+00007720: 7320 6973 2069 6e74 656e 6465 6420 6173  s is intended as
+00007730: 2061 0a20 2073 696d 706c 6572 2072 6570   a.  simpler rep
+00007740: 6c61 6365 6d65 6e74 2066 6f72 2074 6865  lacement for the
+00007750: 2065 7869 7374 696e 6720 3a63 6c61 7373   existing :class
+00007760: 3a60 2e45 6974 6865 7260 2074 7261 6974  :`.Either` trait
+00007770: 2074 7970 652c 2077 6869 6368 0a20 2077   type, which.  w
+00007780: 696c 6c20 6576 656e 7475 616c 6c79 2062  ill eventually b
+00007790: 6520 6465 7072 6563 6174 6564 2e0a 0a2a  e deprecated...*
+000077a0: 204e 6577 203a 636c 6173 733a 602e 5072   New :class:`.Pr
+000077b0: 6566 6978 4c69 7374 602c 203a 636c 6173  efixList`, :clas
+000077c0: 733a 602e 5072 6566 6978 4d61 7060 2061  s:`.PrefixMap` a
+000077d0: 6e64 203a 636c 6173 733a 602e 4d61 7060  nd :class:`.Map`
+000077e0: 2074 7261 6974 2074 7970 6573 0a20 2068   trait types.  h
+000077f0: 6176 6520 6265 656e 2061 6464 6564 2e20  ave been added. 
+00007800: 5468 6573 6520 7265 706c 6163 6520 7468  These replace th
+00007810: 6520 6578 6973 7469 6e67 203a 636c 6173  e existing :clas
+00007820: 733a 602e 5472 6169 7450 7265 6669 784c  s:`.TraitPrefixL
+00007830: 6973 7460 2c0a 2020 3a63 6c61 7373 3a60  ist`,.  :class:`
+00007840: 2e54 7261 6974 5072 6566 6978 4d61 7060  .TraitPrefixMap`
+00007850: 2061 6e64 203a 636c 6173 733a 602e 5472   and :class:`.Tr
+00007860: 6169 744d 6170 6020 7375 6263 6c61 7373  aitMap` subclass
+00007870: 6573 206f 660a 2020 3a63 6c61 7373 3a60  es of.  :class:`
+00007880: 2e54 7261 6974 4861 6e64 6c65 7260 2c20  .TraitHandler`, 
+00007890: 7768 6963 6820 6172 6520 6465 7072 6563  which are deprec
+000078a0: 6174 6564 2e0a 0a2a 2054 7970 696e 6720  ated...* Typing 
+000078b0: 7374 7562 7320 666f 7220 7468 6520 5472  stubs for the Tr
+000078c0: 6169 7473 206c 6962 7261 7279 2068 6176  aits library hav
+000078d0: 6520 6265 656e 2061 6464 6564 2069 6e20  e been added in 
+000078e0: 610a 2020 6060 7472 6169 7473 2d73 7475  a.  ``traits-stu
+000078f0: 6273 6060 2070 6163 6b61 6765 2c20 7768  bs`` package, wh
+00007900: 6963 6820 7769 6c6c 2062 6520 7265 6c65  ich will be rele
+00007910: 6173 6564 2073 6570 6172 6174 656c 7920  ased separately 
+00007920: 746f 2050 7950 492e 2054 6869 730a 2020  to PyPI. This.  
+00007930: 7368 6f75 6c64 2068 656c 7020 7375 7070  should help supp
+00007940: 6f72 7420 5472 6169 7473 2d75 7369 6e67  ort Traits-using
+00007950: 2070 726f 6a65 6374 7320 7468 6174 2077   projects that w
+00007960: 616e 7420 746f 206d 616b 6520 7573 6520  ant to make use 
+00007970: 6f66 2074 7970 650a 2020 616e 6e6f 7461  of type.  annota
+00007980: 7469 6f6e 7320 616e 6420 7479 7065 2063  tions and type c
+00007990: 6865 636b 6572 7320 6c69 6b65 2060 6d79  heckers like `my
+000079a0: 7079 203c 6874 7470 3a2f 2f6d 7970 792d  py <http://mypy-
+000079b0: 6c61 6e67 2e6f 7267 2f3e 605f 2e0a 0a0a  lang.org/>`_....
+000079c0: 4e6f 7465 7320 6f6e 2075 7067 7261 6469  Notes on upgradi
+000079d0: 6e67 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ng.~~~~~~~~~~~~~
+000079e0: 7e7e 7e7e 7e0a 0a41 7320 6661 7220 6173  ~~~~~..As far as
+000079f0: 2070 6f73 7369 626c 652c 2054 7261 6974   possible, Trait
+00007a00: 7320 362e 3120 6973 2062 6163 6b77 6172  s 6.1 is backwar
+00007a10: 6473 2063 6f6d 7061 7469 626c 6520 7769  ds compatible wi
+00007a20: 7468 2054 7261 6974 7320 362e 302e 0a48  th Traits 6.0..H
+00007a30: 6f77 6576 6572 2c20 7468 6572 6520 6172  owever, there ar
+00007a40: 6520 6120 6665 7720 7468 696e 6773 2074  e a few things t
+00007a50: 6f20 6265 2061 7761 7265 206f 6620 7768  o be aware of wh
+00007a60: 656e 2075 7067 7261 6469 6e67 2e0a 0a2a  en upgrading...*
+00007a70: 2054 7261 6974 7320 362e 3120 6973 206e   Traits 6.1 is n
+00007a80: 6f74 2063 6f6d 7061 7469 626c 6520 7769  ot compatible wi
+00007a90: 7468 2054 7261 6974 7355 4920 7665 7273  th TraitsUI vers
+00007aa0: 696f 6e73 206f 6c64 6572 2074 6861 6e20  ions older than 
+00007ab0: 5472 6169 7473 5549 2037 2e30 2e0a 2020  TraitsUI 7.0..  
+00007ac0: 4120 636f 6d62 696e 6174 696f 6e20 6f66  A combination of
+00007ad0: 2054 7261 6974 7320 362e 3120 6f72 206c   Traits 6.1 or l
+00007ae0: 6174 6572 2077 6974 6820 5472 6169 7473  ater with Traits
+00007af0: 5549 2036 2e78 206f 7220 6561 726c 6965  UI 6.x or earlie
+00007b00: 7220 7769 6c6c 2066 6169 6c0a 2020 746f  r will fail.  to
+00007b10: 2070 726f 7065 726c 7920 7265 636f 676e   properly recogn
+00007b20: 6973 6520 3a63 6c61 7373 3a60 7e74 7261  ise :class:`~tra
+00007b30: 6974 7375 692e 7669 6577 2e56 6965 7760  itsui.view.View`
+00007b40: 2063 6c61 7373 2076 6172 6961 626c 6573   class variables
+00007b50: 2061 730a 2020 5472 6169 7473 5549 2076   as.  TraitsUI v
+00007b60: 6965 7773 2c20 616e 6420 616e 2065 7272  iews, and an err
+00007b70: 6f72 2077 696c 6c20 6265 2072 6169 7365  or will be raise
+00007b80: 6420 6966 2079 6f75 2061 7474 656d 7074  d if you attempt
+00007b90: 2074 6f20 6372 6561 7465 2061 0a20 2054   to create a.  T
+00007ba0: 7261 6974 7355 4920 7669 6577 2e0a 0a2a  raitsUI view...*
+00007bb0: 2054 7261 6974 7320 6e6f 7720 646f 6573   Traits now does
+00007bc0: 206e 6f20 6c6f 6767 696e 6720 636f 6e66   no logging conf
+00007bd0: 6967 7572 6174 696f 6e20 6174 2061 6c6c  iguration at all
+00007be0: 2c20 6c65 6176 696e 6720 616c 6c20 7375  , leaving all su
+00007bf0: 6368 0a20 2063 6f6e 6669 6775 7261 7469  ch.  configurati
+00007c00: 6f6e 2074 6f20 7468 6520 6170 706c 6963  on to the applic
+00007c10: 6174 696f 6e2e 0a0a 2020 496e 206d 6f72  ation...  In mor
+00007c20: 6520 6465 7461 696c 3a20 7472 6169 7420  e detail: trait 
+00007c30: 6e6f 7469 6669 6361 7469 6f6e 2068 616e  notification han
+00007c40: 646c 6572 7320 7368 6f75 6c64 206e 6f74  dlers should not
+00007c50: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+00007c60: 7320 696e 0a20 206e 6f72 6d61 6c20 7573  s in.  normal us
+00007c70: 652c 2073 6f20 616e 2065 7863 6570 7469  e, so an excepti
+00007c80: 6f6e 2069 7320 6c6f 6767 6564 2077 6865  on is logged whe
+00007c90: 6e65 7665 7220 6120 7472 6169 7420 6e6f  never a trait no
+00007ca0: 7469 6669 6361 7469 6f6e 2068 616e 646c  tification handl
+00007cb0: 6572 0a20 2072 6169 7365 732e 2054 6869  er.  raises. Thi
+00007cc0: 7320 7061 7274 206f 6620 7468 6520 6265  s part of the be
+00007cd0: 6861 7669 6f75 7220 6861 7320 6e6f 7420  haviour has not 
+00007ce0: 6368 616e 6765 642e 2057 6861 7420 2a68  changed. What *h
+00007cf0: 6173 2a20 6368 616e 6765 6420 6973 2074  as* changed is t
+00007d00: 6865 0a20 2077 6179 2074 6861 7420 6c6f  he.  way that lo
+00007d10: 6767 6564 2065 7863 6570 7469 6f6e 2069  gged exception i
+00007d20: 7320 6861 6e64 6c65 6420 756e 6465 7220  s handled under 
+00007d30: 6465 6661 756c 7420 6578 6365 7074 696f  default exceptio
+00007d40: 6e20 6861 6e64 6c69 6e67 2e0a 0a20 2050  n handling...  P
+00007d50: 7265 7669 6f75 736c 792c 2054 7261 6974  reviously, Trait
+00007d60: 7320 6164 6465 6420 6120 3a63 6c61 7373  s added a :class
+00007d70: 3a60 7e6c 6f67 6769 6e67 2e53 7472 6561  :`~logging.Strea
+00007d80: 6d48 616e 646c 6572 6020 746f 2074 6865  mHandler` to the
+00007d90: 0a20 2074 6f70 2d6c 6576 656c 2060 6022  .  top-level ``"
+00007da0: 7472 6169 7473 2260 6020 6c6f 6767 6572  traits"`` logger
+00007db0: 2c20 736f 2074 6861 7420 7472 6169 7420  , so that trait 
+00007dc0: 6e6f 7469 6669 6361 7469 6f6e 2065 7863  notification exc
+00007dd0: 6570 7469 6f6e 7320 776f 756c 640a 2020  eptions would.  
+00007de0: 616c 7761 7973 2062 6520 7669 7369 626c  always be visibl
+00007df0: 652e 2054 7261 6974 7320 616c 736f 2061  e. Traits also a
+00007e00: 6464 6564 2061 203a 636c 6173 733a 607e  dded a :class:`~
+00007e10: 6c6f 6767 696e 672e 4e75 6c6c 4861 6e64  logging.NullHand
+00007e20: 6c65 7260 2074 6f20 7468 6174 0a20 206c  ler` to that.  l
+00007e30: 6f67 6765 722e 2042 6f74 6820 6f66 2074  ogger. Both of t
+00007e40: 686f 7365 2068 616e 646c 6572 7320 6861  hose handlers ha
+00007e50: 7665 206e 6f77 2062 6565 6e20 7265 6d6f  ve now been remo
+00007e60: 7665 642e 2057 6520 6e6f 7720 7265 6c79  ved. We now rely
+00007e70: 206f 6e0a 2020 5079 7468 6f6e 2773 2022   on.  Python's "
+00007e80: 6861 6e64 6c65 7220 6f66 206c 6173 7420  handler of last 
+00007e90: 7265 736f 7274 222c 2077 6869 6368 2077  resort", which w
+00007ea0: 696c 6c20 636f 6e74 696e 7565 2074 6f20  ill continue to 
+00007eb0: 6d61 6b65 206e 6f74 6966 6963 6174 696f  make notificatio
+00007ec0: 6e0a 2020 6578 6365 7074 696f 6e73 2074  n.  exceptions t
+00007ed0: 6f20 7468 6520 7573 6572 2076 6973 6962  o the user visib
+00007ee0: 6c65 2069 6e20 7468 6520 6162 7365 6e63  le in the absenc
+00007ef0: 6520 6f66 2061 6e79 2061 7070 6c69 6361  e of any applica
+00007f00: 7469 6f6e 2d6c 6576 656c 0a20 206c 6f67  tion-level.  log
+00007f10: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0a   configuration..
+00007f20: 0a2a 2057 6865 6e20 6c69 7374 656e 696e  .* When listenin
+00007f30: 6720 666f 7220 6368 616e 6765 7320 746f  g for changes to
+00007f40: 2074 6865 2069 7465 6d73 206f 6620 6120   the items of a 
+00007f50: 3a63 6c61 7373 3a60 2e4c 6973 7460 2074  :class:`.List` t
+00007f60: 7261 6974 2c20 616e 2069 6e64 6578 0a20  rait, an index. 
+00007f70: 206f 7220 736c 6963 6520 7365 7420 6f70   or slice set op
+00007f80: 6572 6174 696f 6e20 6e6f 206c 6f6e 6765  eration no longe
+00007f90: 7220 7065 7266 6f72 6d73 2061 6e20 6571  r performs an eq
+00007fa0: 7561 6c69 7479 2063 6865 636b 2062 6574  uality check bet
+00007fb0: 7765 656e 2074 6865 0a20 2072 6570 6c61  ween the.  repla
+00007fc0: 6365 6420 656c 656d 656e 7473 2061 6e64  ced elements and
+00007fd0: 2074 6865 2072 6570 6c61 6365 6d65 6e74   the replacement
+00007fe0: 2065 6c65 6d65 6e74 7320 7768 656e 2064   elements when d
+00007ff0: 6563 6964 696e 6720 7768 6574 6865 7220  eciding whether 
+00008000: 746f 2069 7373 7565 0a20 2061 206e 6f74  to issue.  a not
+00008010: 6966 6963 6174 696f 6e3b 2069 6e73 7465  ification; inste
+00008020: 6164 2c20 6120 6e6f 7469 6669 6361 7469  ad, a notificati
+00008030: 6f6e 2069 7320 616c 7761 7973 2069 7373  on is always iss
+00008040: 7565 6420 6966 2061 7420 6c65 6173 7420  ued if at least 
+00008050: 6f6e 650a 2020 656c 656d 656e 7420 7761  one.  element wa
+00008060: 7320 7265 706c 6163 6564 2e20 466f 7220  s replaced. For 
+00008070: 6578 616d 706c 652c 2063 6f6e 7369 6465  example, conside
+00008080: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
+00008090: 636c 6173 733a 3a0a 0a20 2020 2063 6c61  class::..    cla
+000080a0: 7373 2053 656c 6563 7469 6f6e 2848 6173  ss Selection(Has
+000080b0: 5472 6169 7473 293a 0a20 2020 2020 2020  Traits):.       
+000080c0: 2069 6e64 6963 6573 203d 204c 6973 7428   indices = List(
+000080d0: 496e 7429 0a0a 2020 2020 2020 2020 406f  Int)..        @o
+000080e0: 6e5f 7472 6169 745f 6368 616e 6765 2822  n_trait_change("
+000080f0: 696e 6469 6365 735f 6974 656d 7322 290a  indices_items").
+00008100: 2020 2020 2020 2020 6465 6620 7265 706f          def repo
+00008110: 7274 5f63 6861 6e67 6528 7365 6c66 2c20  rt_change(self, 
+00008120: 6576 656e 7429 3a0a 2020 2020 2020 2020  event):.        
+00008130: 2020 2020 7072 696e 7428 2249 6e64 6963      print("Indic
+00008140: 6573 2063 6861 6e67 6564 3a20 222c 2065  es changed: ", e
+00008150: 7665 6e74 290a 0a20 2057 6865 6e20 7265  vent)..  When re
+00008160: 706c 6163 696e 6720 7468 6520 6038 6020  placing the `8` 
+00008170: 7769 7468 2074 6865 2073 616d 6520 696e  with the same in
+00008180: 7465 6765 722c 2077 6520 6765 7420 7468  teger, we get th
+00008190: 6973 2062 6568 6176 696f 723a 3a0a 0a20  is behavior::.. 
+000081a0: 2020 203e 3e3e 2073 656c 6563 7469 6f6e     >>> selection
+000081b0: 203d 2053 656c 6563 7469 6f6e 2869 6e64   = Selection(ind
+000081c0: 6963 6573 3d5b 322c 2035 2c20 385d 290a  ices=[2, 5, 8]).
+000081d0: 2020 2020 3e3e 3e20 7365 6c65 6374 696f      >>> selectio
+000081e0: 6e2e 696e 6469 6365 735b 325d 203d 2038  n.indices[2] = 8
+000081f0: 0a20 2020 2049 6e64 6963 6573 2063 6861  .    Indices cha
+00008200: 6e67 6564 3a20 2054 7261 6974 4c69 7374  nged:  TraitList
+00008210: 4576 656e 7428 696e 6465 783d 322c 2072  Event(index=2, r
+00008220: 656d 6f76 6564 3d5b 385d 2c20 6164 6465  emoved=[8], adde
+00008230: 643d 5b38 5d29 0a0a 2020 5072 6576 696f  d=[8])..  Previo
+00008240: 7573 6c79 2c20 6e6f 206e 6f74 6966 6963  usly, no notific
+00008250: 6174 696f 6e20 776f 756c 6420 6861 7665  ation would have
+00008260: 2062 6565 6e20 6973 7375 6564 2e0a 0a2a   been issued...*
+00008270: 2054 6865 203a 6675 6e63 3a60 2e43 6f6c   The :func:`.Col
+00008280: 6f72 602c 203a 6675 6e63 3a60 2e52 4742  or`, :func:`.RGB
+00008290: 436f 6c6f 7260 2061 6e64 203a 6675 6e63  Color` and :func
+000082a0: 3a60 2e46 6f6e 7460 2074 7261 6974 2066  :`.Font` trait f
+000082b0: 6163 746f 7269 6573 0a20 2068 6176 6520  actories.  have 
+000082c0: 6d6f 7665 6420 746f 2054 7261 6974 7355  moved to TraitsU
+000082d0: 492c 2061 6e64 2073 686f 756c 6420 6265  I, and should be
+000082e0: 2069 6d70 6f72 7465 6420 6672 6f6d 2074   imported from t
+000082f0: 6865 7265 2072 6174 6865 7220 7468 616e  here rather than
+00008300: 2066 726f 6d0a 2020 5472 6169 7473 2e20   from.  Traits. 
+00008310: 466f 7220 6261 636b 7761 7264 7320 636f  For backwards co
+00008320: 6d70 6174 6962 696c 6974 792c 2074 6865  mpatibility, the
+00008330: 2066 6163 746f 7269 6573 2061 7265 2073   factories are s
+00008340: 7469 6c6c 0a20 2061 7661 696c 6162 6c65  till.  available
+00008350: 2069 6e20 5472 6169 7473 2c20 6275 7420   in Traits, but 
+00008360: 7468 6579 2061 7265 2064 6570 7265 6361  they are depreca
+00008370: 7465 6420 616e 6420 7769 6c6c 2065 7665  ted and will eve
+00008380: 6e74 7561 6c6c 790a 2020 6265 2072 656d  ntually.  be rem
+00008390: 6f76 6564 2e0a 0a2a 2041 7320 6120 7265  oved...* As a re
+000083a0: 6d69 6e64 6572 2c20 7468 6520 3a64 6174  minder, the :dat
+000083b0: 613a 602e 556e 6963 6f64 6560 2061 6e64  a:`.Unicode` and
+000083c0: 203a 6461 7461 3a60 2e4c 6f6e 6760 2074   :data:`.Long` t
+000083d0: 7261 6974 2074 7970 6573 2061 7265 0a20  rait types are. 
+000083e0: 2064 6570 7265 6361 7465 6420 7369 6e63   deprecated sinc
+000083f0: 6520 5472 6169 7473 2036 2e30 2e20 506c  e Traits 6.0. Pl
+00008400: 6561 7365 2072 6570 6c61 6365 2075 7365  ease replace use
+00008410: 7320 7769 7468 203a 636c 6173 733a 602e  s with :class:`.
+00008420: 5374 7260 2061 6e64 0a20 203a 636c 6173  Str` and.  :clas
+00008430: 733a 602e 496e 7460 2072 6573 7065 6374  s:`.Int` respect
+00008440: 6976 656c 792e 2054 6f20 6176 6f69 6420  ively. To avoid 
+00008450: 6578 6365 7373 6976 6520 6e6f 6973 6520  excessive noise 
+00008460: 696e 2054 7261 6974 732d 7573 696e 670a  in Traits-using.
+00008470: 2020 7072 6f6a 6563 7473 2c20 5472 6169    projects, Trai
+00008480: 7473 2064 6f65 7320 6e6f 7420 7965 7420  ts does not yet 
+00008490: 6973 7375 6520 6465 7072 6563 6174 696f  issue deprecatio
+000084a0: 6e20 7761 726e 696e 6773 2066 6f72 2065  n warnings for e
+000084b0: 7869 7374 696e 6720 7573 6573 206f 660a  xisting uses of.
+000084c0: 2020 3a64 6174 613a 602e 556e 6963 6f64    :data:`.Unicod
+000084d0: 6560 2061 6e64 203a 6461 7461 3a60 2e4c  e` and :data:`.L
+000084e0: 6f6e 6760 2e20 5468 6f73 6520 7761 726e  ong`. Those warn
+000084f0: 696e 6773 2077 696c 6c20 6265 2069 6e74  ings will be int
+00008500: 726f 6475 6365 6420 696e 2061 0a20 2066  roduced in a.  f
+00008510: 7574 7572 6520 5472 6169 7473 2072 656c  uture Traits rel
+00008520: 6561 7365 2c20 7072 696f 7220 746f 2074  ease, prior to t
+00008530: 6865 2072 656d 6f76 616c 206f 6620 7468  he removal of th
+00008540: 6573 6520 7472 6169 7420 7479 7065 732e  ese trait types.
+00008550: 0a0a 0a50 656e 6469 6e67 2064 6570 7265  ...Pending depre
+00008560: 6361 7469 6f6e 730a 7e7e 7e7e 7e7e 7e7e  cations.~~~~~~~~
+00008570: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 496e  ~~~~~~~~~~~~..In
+00008580: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
+00008590: 2064 6570 7265 6361 7469 6f6e 7320 6c69   deprecations li
+000085a0: 7374 6564 2069 6e20 7468 6520 6368 616e  sted in the chan
+000085b0: 6765 6c6f 6720 6265 6c6f 772c 2073 6f6d  gelog below, som
+000085c0: 6520 7061 7274 7320 6f66 0a74 6865 2054  e parts of.the T
+000085d0: 7261 6974 7320 6c69 6272 6172 7920 6172  raits library ar
+000085e0: 6520 6e6f 7420 7965 7420 666f 726d 616c  e not yet formal
+000085f0: 6c79 2064 6570 7265 6361 7465 642c 2062  ly deprecated, b
+00008600: 7574 2061 7265 206c 696b 656c 7920 746f  ut are likely to
+00008610: 2062 650a 6465 7072 6563 6174 6564 2062   be.deprecated b
+00008620: 6566 6f72 6520 5472 6169 7473 2037 2e30  efore Traits 7.0
+00008630: 2e20 5573 6572 7320 7368 6f75 6c64 2062  . Users should b
+00008640: 6520 6177 6172 6520 6f66 2074 6865 2066  e aware of the f
+00008650: 6f6c 6c6f 7769 6e67 2070 6f73 7369 626c  ollowing possibl
+00008660: 650a 6675 7475 7265 2063 6861 6e67 6573  e.future changes
+00008670: 3a0a 0a2a 2054 6865 203a 636c 6173 733a  :..* The :class:
+00008680: 602e 4569 7468 6572 6020 7472 6169 7420  `.Either` trait 
+00008690: 7479 7065 2077 696c 6c20 6576 656e 7475  type will eventu
+000086a0: 616c 6c79 2062 6520 6465 7072 6563 6174  ally be deprecat
+000086b0: 6564 2e20 5768 6572 650a 2020 706f 7373  ed. Where.  poss
+000086c0: 6962 6c65 2c20 7573 6520 3a63 6c61 7373  ible, use :class
+000086d0: 3a60 2e55 6e69 6f6e 6020 696e 7374 6561  :`.Union` instea
+000086e0: 642e 2057 6865 6e20 7265 706c 6163 696e  d. When replacin
+000086f0: 6720 7573 6573 206f 660a 2020 3a63 6c61  g uses of.  :cla
+00008700: 7373 3a60 2e45 6974 6865 7260 2077 6974  ss:`.Either` wit
+00008710: 6820 3a63 6c61 7373 3a60 2e55 6e69 6f6e  h :class:`.Union
+00008720: 602c 206e 6f74 6520 7468 6174 2074 6865  `, note that the
+00008730: 7265 2061 7265 2073 6f6d 6520 7369 676e  re are some sign
+00008740: 6966 6963 616e 740a 2020 4150 4920 616e  ificant.  API an
+00008750: 6420 6265 6861 7669 6f72 616c 2064 6966  d behavioral dif
+00008760: 6665 7265 6e63 6573 2062 6574 7765 656e  ferences between
+00008770: 2074 6865 2074 776f 2074 7261 6974 2074   the two trait t
+00008780: 7970 6573 2c20 7061 7274 6963 756c 6172  ypes, particular
+00008790: 6c79 2077 6974 680a 2020 7265 7370 6563  ly with.  respec
+000087a0: 7420 746f 2068 616e 646c 696e 6720 6f66  t to handling of
+000087b0: 2064 6566 6175 6c74 732e 2053 6565 203a   defaults. See :
+000087c0: 7265 663a 606d 6967 7261 7469 6f6e 5f65  ref:`migration_e
+000087d0: 6974 6865 725f 746f 5f75 6e69 6f6e 6020  ither_to_union` 
+000087e0: 666f 720a 2020 6d6f 7265 2064 6574 6169  for.  more detai
+000087f0: 6c73 2e0a 0a2a 2054 6865 2060 6074 7261  ls...* The ``tra
+00008800: 6974 5f6d 6f64 6966 6965 6460 6020 6576  it_modified`` ev
+00008810: 656e 7420 7472 6169 7420 7468 6174 2773  ent trait that's
+00008820: 2070 7265 7365 6e74 206f 6e20 616c 6c20   present on all 
+00008830: 3a63 6c61 7373 3a60 2e48 6173 5472 6169  :class:`.HasTrai
+00008840: 7473 600a 2020 7375 6263 6c61 7373 6573  ts`.  subclasses
+00008850: 2077 696c 6c20 6576 656e 7475 616c 6c79   will eventually
+00008860: 2062 6520 7265 6d6f 7665 642e 2055 7365   be removed. Use
+00008870: 7273 2073 686f 756c 6420 6e6f 7420 7265  rs should not re
+00008880: 6c79 206f 6e20 6974 2062 6569 6e67 0a20  ly on it being. 
+00008890: 2070 7265 7365 6e74 2069 6e20 616e 206f   present in an o
+000088a0: 626a 6563 7427 7320 6060 636c 6173 735f  bject's ``class_
+000088b0: 7472 6169 7473 6060 2064 6963 7469 6f6e  traits`` diction
+000088c0: 6172 792e 0a0a 2a20 5472 6169 7420 6e61  ary...* Trait na
+000088d0: 6d65 7320 7374 6172 7469 6e67 2077 6974  mes starting wit
+000088e0: 6820 6060 7472 6169 7460 602c 2060 6074  h ``trait``, ``t
+000088f0: 7261 6974 7360 602c 2060 605f 7472 6169  raits``, ``_trai
+00008900: 7460 6020 6f72 0a20 2060 605f 7472 6169  t`` or.  ``_trai
+00008910: 7473 6060 206d 6179 2062 6563 6f6d 6520  ts`` may become 
+00008920: 7265 7365 7276 6564 2066 6f72 2075 7365  reserved for use
+00008930: 2062 7920 4554 5320 6174 2073 6f6d 6520   by ETS at some 
+00008940: 706f 696e 7420 696e 2074 6865 2066 7574  point in the fut
+00008950: 7572 652e 0a20 2041 766f 6964 2075 7369  ure..  Avoid usi
+00008960: 6e67 2074 6865 7365 206e 616d 6573 2066  ng these names f
+00008970: 6f72 2079 6f75 7220 6f77 6e20 7472 6169  or your own trai
+00008980: 7473 2e0a 0a44 6574 6169 6c65 6420 5052  ts...Detailed PR
+00008990: 2d62 792d 5052 2063 6861 6e67 6573 0a7e  -by-PR changes.~
+000089a0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+000089b0: 7e7e 7e7e 7e7e 7e7e 0a0a 4d6f 7265 2074  ~~~~~~~~..More t
+000089c0: 6861 6e20 3136 3020 5052 7320 7765 6e74  han 160 PRs went
+000089d0: 2069 6e74 6f20 7468 6973 2072 656c 6561   into this relea
+000089e0: 7365 2e20 5468 6520 666f 6c6c 6f77 696e  se. The followin
+000089f0: 6720 7065 6f70 6c65 2063 6f6e 7472 6962  g people contrib
+00008a00: 7574 6564 0a63 6f64 6520 6368 616e 6765  uted.code change
+00008a10: 7320 666f 7220 7468 6973 2072 656c 6561  s for this relea
+00008a20: 7365 3a0a 0a2a 2049 6576 6120 4365 726e  se:..* Ieva Cern
+00008a30: 7974 650a 2a20 4b69 7420 5961 6e20 4368  yte.* Kit Yan Ch
+00008a40: 6f69 0a2a 204d 6178 696d 6520 436f 7374  oi.* Maxime Cost
+00008a50: 616c 6f6e 6761 0a2a 204d 6172 6b20 4469  alonga.* Mark Di
+00008a60: 636b 696e 736f 6e0a 2a20 4d61 7474 2048  ckinson.* Matt H
+00008a70: 616e 636f 636b 0a2a 204d 6964 6875 6e20  ancock.* Midhun 
+00008a80: 4d61 6468 7573 6f6f 6461 6e61 6e0a 2a20  Madhusoodanan.* 
+00008a90: 5368 6f65 6220 4d6f 6861 6d6d 6564 0a2a  Shoeb Mohammed.*
+00008aa0: 2046 7261 6e6b 6c69 6e20 5665 6e74 7572   Franklin Ventur
+00008ab0: 610a 2a20 436f 7272 616e 2057 6562 7374  a.* Corran Webst
+00008ac0: 6572 0a0a 4665 6174 7572 6573 0a7e 7e7e  er..Features.~~~
+00008ad0: 7e7e 7e7e 7e0a 0a2a 2041 6464 2060 606f  ~~~~~..* Add ``o
+00008ae0: 732e 5061 7468 4c69 6b65 6060 2073 7570  s.PathLike`` sup
+00008af0: 706f 7274 2066 6f72 2060 6044 6972 6563  port for ``Direc
+00008b00: 746f 7279 6060 2074 7261 6974 732e 2028  tory`` traits. (
+00008b10: 2338 3637 290a 2a20 4164 6420 6060 556e  #867).* Add ``Un
+00008b20: 696f 6e60 6020 7472 6169 7420 7479 7065  ion`` trait type
+00008b30: 2e20 2823 3737 392c 2023 3131 3033 2c20  . (#779, #1103, 
+00008b40: 2331 3130 372c 2023 3131 3136 2c20 2331  #1107, #1116, #1
+00008b50: 3131 3529 0a2a 2041 6464 2060 6050 7265  115).* Add ``Pre
+00008b60: 6669 784c 6973 7460 6020 7472 6169 7420  fixList`` trait 
+00008b70: 7479 7065 2e20 2823 3837 312c 2023 3131  type. (#871, #11
+00008b80: 3432 2c20 2331 3134 342c 2023 3131 3437  42, #1144, #1147
+00008b90: 290a 2a20 4164 6420 6060 616c 6c6f 775f  ).* Add ``allow_
+00008ba0: 6e6f 6e65 6060 2066 6c61 6720 666f 7220  none`` flag for 
+00008bb0: 6060 4361 6c6c 6162 6c65 6060 2074 7261  ``Callable`` tra
+00008bc0: 6974 2e20 2823 3838 3529 0a2a 2041 6464  it. (#885).* Add
+00008bd0: 2073 7570 706f 7274 2066 6f72 2074 7970   support for typ
+00008be0: 6520 616e 6e6f 7461 7469 6f6e 2e20 2823  e annotation. (#
+00008bf0: 3930 342c 2023 3130 3634 290a 2a20 416c  904, #1064).* Al
+00008c00: 6c6f 7720 6d75 7461 626c 6520 7661 6c75  low mutable valu
+00008c10: 6573 2069 6e20 6060 436f 6e73 7461 6e74  es in ``Constant
+00008c20: 6060 2074 7261 6974 2e20 2823 3932 3929  `` trait. (#929)
+00008c30: 0a2a 2041 6464 2060 604d 6170 6060 2061  .* Add ``Map`` a
+00008c40: 6e64 2060 6050 7265 6669 784d 6170 6060  nd ``PrefixMap``
+00008c50: 2074 7261 6974 2074 7970 6573 2e20 2823   trait types. (#
+00008c60: 3838 362c 2023 3935 332c 2023 3935 362c  886, #953, #956,
+00008c70: 2023 3937 302c 2023 3131 3339 2c0a 2020   #970, #1139,.  
+00008c80: 2331 3138 3929 0a2a 2041 6464 2060 6054  #1189).* Add ``T
+00008c90: 7261 6974 4c69 7374 6060 2061 7320 7468  raitList`` as th
+00008ca0: 6520 6261 7365 206c 6973 7420 6f62 6a65  e base list obje
+00008cb0: 6374 2074 6861 7420 6361 6e20 7065 7266  ct that can perf
+00008cc0: 6f72 6d20 7661 6c69 6461 7469 6f6e 0a20  orm validation. 
+00008cd0: 2061 6e64 2065 6d69 7420 6368 616e 6765   and emit change
+00008ce0: 206e 6f74 6966 6963 6174 696f 6e73 2e20   notifications. 
+00008cf0: 2823 3931 322c 2023 3938 312c 2023 3938  (#912, #981, #98
+00008d00: 342c 2023 3938 392c 2023 3939 392c 2023  4, #989, #999, #
+00008d10: 3130 3033 2c20 2331 3031 312c 0a20 2023  1003, #1011,.  #
+00008d20: 3130 3236 2c20 2331 3030 392c 2023 3130  1026, #1009, #10
+00008d30: 3430 2c20 2331 3137 322c 2023 3131 3733  40, #1172, #1173
+00008d40: 290a 2a20 4164 6420 6060 5472 6169 7444  ).* Add ``TraitD
+00008d50: 6963 7460 6020 6173 2074 6865 2062 6173  ict`` as the bas
+00008d60: 6520 6469 6374 206f 626a 6563 7420 7468  e dict object th
+00008d70: 6174 2063 616e 2070 6572 666f 726d 2076  at can perform v
+00008d80: 616c 6964 6174 696f 6e20 616e 640a 2020  alidation and.  
+00008d90: 656d 6974 2063 6861 6e67 6520 6e6f 7469  emit change noti
+00008da0: 6669 6361 7469 6f6e 732e 2028 2339 3133  fications. (#913
+00008db0: 290a 2a20 4164 6420 6060 5472 6169 7453  ).* Add ``TraitS
+00008dc0: 6574 6060 2061 7320 7468 6520 6261 7365  et`` as the base
+00008dd0: 2073 6574 206f 626a 6563 7420 7468 6174   set object that
+00008de0: 2063 616e 2070 6572 666f 726d 2076 616c   can perform val
+00008df0: 6964 6174 696f 6e20 616e 640a 2020 656d  idation and.  em
+00008e00: 6974 2063 6861 6e67 6520 6e6f 7469 6669  it change notifi
+00008e10: 6361 7469 6f6e 732e 2028 2339 3232 2c20  cations. (#922, 
+00008e20: 2331 3034 3329 0a2a 2049 6d70 6c65 6d65  #1043).* Impleme
+00008e30: 6e74 2060 606f 6273 6572 7665 6060 2074  nt ``observe`` t
+00008e40: 6f20 7375 7065 7273 6564 6520 6060 6f6e  o supersede ``on
+00008e50: 5f74 7261 6974 5f63 6861 6e67 6560 6020  _trait_change`` 
+00008e60: 666f 7220 6f62 7365 7276 696e 6720 7472  for observing tr
+00008e70: 6169 740a 2020 6368 616e 6765 732e 2028  ait.  changes. (
+00008e80: 2339 3736 2c20 2331 3030 302c 2023 3130  #976, #1000, #10
+00008e90: 3037 2c20 2331 3036 352c 2023 3130 3233  07, #1065, #1023
+00008ea0: 2c20 2331 3036 362c 2023 3130 3730 2c20  , #1066, #1070, 
+00008eb0: 2331 3036 392c 2023 3130 3637 2c0a 2020  #1069, #1067,.  
+00008ec0: 2331 3038 302c 2023 3130 3832 2c20 2331  #1080, #1082, #1
+00008ed0: 3037 392c 2023 3130 3731 2c20 2331 3037  079, #1071, #107
+00008ee0: 322c 2023 3130 3735 2c20 2331 3038 352c  2, #1075, #1085,
+00008ef0: 2023 3130 3839 2c20 2331 3037 382c 2023   #1089, #1078, #
+00008f00: 3130 3933 2c20 2331 3038 362c 0a20 2023  1093, #1086,.  #
+00008f10: 3130 3737 2c20 2331 3039 352c 2023 3131  1077, #1095, #11
+00008f20: 3032 2c20 2331 3130 382c 2023 3131 3130  02, #1108, #1110
+00008f30: 2c20 2331 3131 322c 2023 3131 3137 2c20  , #1112, #1117, 
+00008f40: 2331 3131 382c 2023 3131 3233 2c20 2331  #1118, #1123, #1
+00008f50: 3132 352c 2023 3131 3236 2c0a 2020 2331  125, #1126,.  #1
+00008f60: 3132 382c 2023 3131 3239 2c20 2331 3133  128, #1129, #113
+00008f70: 352c 2023 3131 3536 290a 0a43 6861 6e67  5, #1156)..Chang
+00008f80: 6573 0a7e 7e7e 7e7e 7e7e 0a0a 2a20 4755  es.~~~~~~~..* GU
+00008f90: 4920 6170 706c 6963 6174 696f 6e73 2075  I applications u
+00008fa0: 7369 6e67 2054 7261 6974 7320 362e 3120  sing Traits 6.1 
+00008fb0: 7769 6c6c 2072 6571 7569 7265 2054 7261  will require Tra
+00008fc0: 6974 7355 4920 3e3d 2037 2e30 2e20 2823  itsUI >= 7.0. (#
+00008fd0: 3131 3334 290a 2a20 6060 5472 6169 7453  1134).* ``TraitS
+00008fe0: 6574 4576 656e 7460 6020 616e 6420 6060  etEvent`` and ``
+00008ff0: 5472 6169 7444 6963 7445 7665 6e74 6060  TraitDictEvent``
+00009000: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
+00009010: 6172 6775 6d65 6e74 7320 6172 6520 6e6f  arguments are no
+00009020: 770a 2020 6b65 7977 6f72 642d 6f6e 6c79  w.  keyword-only
+00009030: 2e20 2823 3130 3336 290a 2a20 6060 5472  . (#1036).* ``Tr
+00009040: 6169 744c 6973 744f 626a 6563 7460 6020  aitListObject`` 
+00009050: 7769 6c6c 206e 6f20 6c6f 6e67 6572 2073  will no longer s
+00009060: 6b69 7020 6e6f 7469 6669 6361 7469 6f6e  kip notification
+00009070: 7320 6576 656e 2069 6620 6d75 7461 7469  s even if mutati
+00009080: 6f6e 730a 2020 7265 7375 6c74 2069 6e20  ons.  result in 
+00009090: 636f 6e74 656e 7420 7468 6174 2063 6f6d  content that com
+000090a0: 7061 7265 7320 6571 7561 6c6c 7920 746f  pares equally to
+000090b0: 2074 6865 206f 6c64 2076 616c 7565 732e   the old values.
+000090c0: 2028 2331 3032 3629 0a2a 2060 6054 7261   (#1026).* ``Tra
+000090d0: 6974 4c69 7374 4576 656e 742e 696e 6465  itListEvent.inde
+000090e0: 7860 6020 7265 706f 7274 6564 2062 7920  x`` reported by 
+000090f0: 6d75 7461 7469 6f6e 7320 746f 2061 206c  mutations to a l
+00009100: 6973 7420 6973 206e 6f77 206e 6f72 6d61  ist is now norma
+00009110: 6c69 7a65 642e 0a20 2028 2331 3030 3929  lized..  (#1009)
+00009120: 0a2a 2054 6865 2064 6566 6175 6c74 206e  .* The default n
+00009130: 6f74 6966 6963 6174 696f 6e20 6572 726f  otification erro
+00009140: 7220 6861 6e64 6c65 7220 666f 7220 5472  r handler for Tr
+00009150: 6169 7473 206e 6f20 6c6f 6e67 6572 2063  aits no longer c
+00009160: 6f6e 6669 6775 7265 730a 2020 6c6f 6767  onfigures.  logg
+00009170: 696e 672c 2061 6e64 2074 6865 2074 6f70  ing, and the top
+00009180: 2d6c 6576 656c 2060 604e 756c 6c48 616e  -level ``NullHan
+00009190: 646c 6572 6060 206c 6f67 2068 616e 646c  dler`` log handl
+000091a0: 6572 2068 6173 2062 6565 6e20 7265 6d6f  er has been remo
+000091b0: 7665 642e 0a20 2028 2331 3136 3129 0a0a  ved..  (#1161)..
+000091c0: 4669 7865 730a 7e7e 7e7e 7e0a 2a20 416c  Fixes.~~~~~.* Al
+000091d0: 6c6f 7720 6173 7369 676e 696e 6720 4e6f  low assigning No
+000091e0: 6e65 2074 6f20 6060 4354 7261 6974 2e70  ne to ``CTrait.p
+000091f0: 6f73 745f 7365 7461 7474 7260 602e 2028  ost_setattr``. (
+00009200: 2338 3333 290a 2a20 4669 7820 7265 6665  #833).* Fix refe
+00009210: 7265 6e63 6520 636f 756e 7420 6572 726f  rence count erro
+00009220: 722e 2028 2339 3037 290a 2a20 496d 7072  r. (#907).* Impr
+00009230: 6f76 6520 6060 4861 7354 7261 6974 7360  ove ``HasTraits`
+00009240: 6020 696e 7472 6f73 7065 6374 696f 6e20  ` introspection 
+00009250: 7769 7468 2060 6064 6972 2829 6060 2e20  with ``dir()``. 
+00009260: 2823 3932 3729 0a2a 2046 6978 2074 6865  (#927).* Fix the
+00009270: 2064 6174 6574 696d 652d 746f 2d73 7472   datetime-to-str
+00009280: 2063 6f6e 7665 7274 6572 7320 7573 6564   converters used
+00009290: 2069 6e20 6060 4461 7465 7469 6d65 4564   in ``DatetimeEd
+000092a0: 6974 6f72 6060 2e20 2823 3933 3729 0a2a  itor``. (#937).*
+000092b0: 2052 6169 7365 2060 6054 7261 6974 4e6f   Raise ``TraitNo
+000092c0: 7469 6669 6361 7469 6f6e 4572 726f 7260  tificationError`
+000092d0: 6020 6f6e 2074 7261 696c 696e 6720 636f  ` on trailing co
+000092e0: 6d6d 6120 696e 2060 606f 6e5f 7472 6169  mma in ``on_trai
+000092f0: 745f 6368 616e 6765 6060 2e0a 2020 2823  t_change``..  (#
+00009300: 3932 3629 0a2a 2046 6978 2065 7863 6570  926).* Fix excep
+00009310: 7469 6f6e 2073 7761 6c6c 6f77 696e 6720  tion swallowing 
+00009320: 6279 2054 7261 6974 2061 7474 7269 6275  by Trait attribu
+00009330: 7465 2061 6363 6573 732e 2028 2339 3539  te access. (#959
+00009340: 2c20 2339 3630 290a 2a20 416c 6c6f 7720  , #960).* Allow 
+00009350: 636f 6c6c 6563 7469 6f6e 7320 696e 2076  collections in v
+00009360: 616c 6964 2076 616c 7565 7320 666f 7220  alid values for 
+00009370: 6060 456e 756d 6060 2074 7261 6974 2e20  ``Enum`` trait. 
+00009380: 2823 3838 3929 0a2a 2046 6978 2060 6054  (#889).* Fix ``T
+00009390: 7261 6974 4572 726f 7260 6020 7768 656e  raitError`` when
+000093a0: 206d 7574 6174 696e 6720 6120 6c69 7374   mutating a list
+000093b0: 2f64 6963 742f 7365 7420 696e 7369 6465  /dict/set inside
+000093c0: 2061 6e6f 7468 6572 2063 6f6e 7461 696e   another contain
+000093d0: 6572 2e0a 2020 2823 3130 3138 290a 2a20  er..  (#1018).* 
+000093e0: 4669 7820 7365 7474 696e 6720 6465 6661  Fix setting defa
+000093f0: 756c 7420 7661 6c75 6573 2076 6961 2064  ult values via d
+00009400: 796e 616d 6963 2064 6566 6175 6c74 206d  ynamic default m
+00009410: 6574 686f 6473 206f 7220 6f76 6572 7269  ethods or overri
+00009420: 6469 6e67 2074 7261 6974 2069 6e0a 2020  ding trait in.  
+00009430: 7375 6263 6c61 7373 6573 2066 6f72 206d  subclasses for m
+00009440: 6170 7065 6420 7472 6169 7473 2c20 7573  apped traits, us
+00009450: 6564 2062 7920 6060 4d61 7060 602c 2060  ed by ``Map``, `
+00009460: 6045 7870 7265 7373 696f 6e60 602c 2060  `Expression``, `
+00009470: 6050 7265 6669 784d 6170 6060 2e0a 2020  `PrefixMap``..  
+00009480: 2823 3130 3931 2c20 2331 3138 3829 0a2a  (#1091, #1188).*
+00009490: 2046 6978 2073 6574 7469 6e67 2064 6566   Fix setting def
+000094a0: 6175 6c74 2076 616c 7565 7320 7669 6120  ault values via 
+000094b0: 6479 6e61 6d69 6320 6465 6661 756c 7420  dynamic default 
+000094c0: 6d65 7468 6f64 7320 6f72 206f 7665 7272  methods or overr
+000094d0: 6964 696e 6720 7472 6169 7420 696e 0a20  iding trait in. 
+000094e0: 2073 7562 636c 6173 7365 7320 666f 7220   subclasses for 
+000094f0: 6060 4578 7072 6573 7369 6f6e 6060 2061  ``Expression`` a
+00009500: 6e64 2060 6041 6461 7074 7354 6f60 602e  nd ``AdaptsTo``.
+00009510: 2028 2331 3038 382c 2023 3131 3139 2c20   (#1088, #1119, 
+00009520: 2331 3135 3229 0a0a 4465 7072 6563 6174  #1152)..Deprecat
+00009530: 696f 6e73 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  ions.~~~~~~~~~~~
+00009540: 7e0a 0a2a 2060 6074 7261 6974 732e 7465  ~..* ``traits.te
+00009550: 7374 696e 672e 6e6f 7365 5f74 6f6f 6c73  sting.nose_tools
+00009560: 6060 2069 7320 6465 7072 6563 6174 6564  `` is deprecated
+00009570: 2e20 2823 3838 3029 0a2a 2060 6053 696e  . (#880).* ``Sin
+00009580: 676c 6574 6f6e 4861 7354 7261 6974 7360  gletonHasTraits`
+00009590: 602c 2060 6053 696e 676c 6574 6f6e 4861  `, ``SingletonHa
+000095a0: 7353 7472 6963 7454 7261 6974 7360 6020  sStrictTraits`` 
+000095b0: 616e 640a 2020 6060 5369 6e67 6c65 746f  and.  ``Singleto
+000095c0: 6e48 6173 5072 6976 6174 6554 7261 6974  nHasPrivateTrait
+000095d0: 7360 6020 6172 6520 6465 7072 6563 6174  s`` are deprecat
+000095e0: 6564 2e20 2823 3838 3729 0a2a 2060 6054  ed. (#887).* ``T
+000095f0: 7261 6974 4d61 7060 6020 6973 2064 6570  raitMap`` is dep
+00009600: 7265 6361 7465 642c 2075 7365 2060 604d  recated, use ``M
+00009610: 6170 6060 2069 6e73 7465 6164 2e20 2823  ap`` instead. (#
+00009620: 3937 3429 0a2a 2060 6054 7261 6974 5072  974).* ``TraitPr
+00009630: 6566 6978 4d61 7060 6020 6973 2064 6570  efixMap`` is dep
+00009640: 7265 6361 7465 642c 2075 7365 2060 6050  recated, use ``P
+00009650: 7265 6669 784d 6170 6060 2069 6e73 7465  refixMap`` inste
+00009660: 6164 2e20 2823 3937 3429 0a2a 2060 6054  ad. (#974).* ``T
+00009670: 7261 6974 5072 6566 6978 4c69 7374 6060  raitPrefixList``
+00009680: 2069 7320 6465 7072 6563 6174 6564 2c20   is deprecated, 
+00009690: 7573 6520 6060 5072 6566 6978 4c69 7374  use ``PrefixList
+000096a0: 6060 2e20 2823 3937 3429 0a2a 2060 6043  ``. (#974).* ``C
+000096b0: 6f6c 6f72 6060 2c20 6060 5242 4743 6f6c  olor``, ``RBGCol
+000096c0: 6f72 6060 2061 6e64 2060 6046 6f6e 7460  or`` and ``Font`
+000096d0: 6020 6172 6520 6e6f 7720 6465 7072 6563  ` are now deprec
+000096e0: 6174 6564 2e20 5573 6520 7468 6520 6f6e  ated. Use the on
+000096f0: 6573 2066 726f 6d0a 2020 5472 6169 7473  es from.  Traits
+00009700: 5549 2069 6e73 7465 6164 2e20 2823 3130  UI instead. (#10
+00009710: 3232 290a 0a52 656d 6f76 616c 730a 7e7e  22)..Removals.~~
+00009720: 7e7e 7e7e 7e7e 0a0a 2a20 6060 7472 6169  ~~~~~~..* ``trai
+00009730: 7473 5f73 7570 6572 6060 2069 7320 7265  ts_super`` is re
+00009740: 6d6f 7665 642e 2028 2331 3031 3529 0a0a  moved. (#1015)..
+00009750: 446f 6375 6d65 6e74 6174 696f 6e0a 7e7e  Documentation.~~
+00009760: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a 2041  ~~~~~~~~~~~..* A
+00009770: 6464 2064 6574 6169 6c73 206f 6e20 6372  dd details on cr
+00009780: 6561 7469 6e67 2063 7573 746f 6d20 7472  eating custom tr
+00009790: 6169 7420 7072 6f70 6572 7469 6573 2e20  ait properties. 
+000097a0: 2823 3338 3729 0a2a 2043 726f 7373 2072  (#387).* Cross r
+000097b0: 6566 6572 656e 6365 2073 7065 6369 616c  eference special
+000097c0: 2068 616e 646c 6572 2073 6967 6e61 7475   handler signatu
+000097d0: 7265 7320 666f 7220 6c69 7374 656e 696e  res for listenin
+000097e0: 6720 746f 206e 6573 7465 6420 6174 7472  g to nested attr
+000097f0: 6962 7574 6573 0a20 2069 6e20 6c69 7374  ibutes.  in list
+00009800: 2061 6e64 2064 6963 742e 2028 2338 3934   and dict. (#894
+00009810: 290a 2a20 5265 706c 6163 6520 2754 7261  ).* Replace 'Tra
+00009820: 6974 7320 3527 2077 6974 6820 2754 7261  its 5' with 'Tra
+00009830: 6974 7320 3627 2069 6e20 7468 6520 646f  its 6' in the do
+00009840: 6375 6d65 6e74 6174 696f 6e2e 2028 2339  cumentation. (#9
+00009850: 3033 290a 2a20 5573 6520 6d61 6a6f 722e  03).* Use major.
+00009860: 6d69 6e6f 7220 7665 7273 696f 6e20 696e  minor version in
+00009870: 2064 6f63 756d 656e 7461 7469 6f6e 2e20   documentation. 
+00009880: 2823 3131 3234 290a 2a20 4164 6420 696e  (#1124).* Add in
+00009890: 6974 6961 6c20 646f 6375 6d65 6e74 6174  itial documentat
+000098a0: 696f 6e20 6f6e 2054 7261 6974 7320 696e  ion on Traits in
+000098b0: 7465 726e 616c 732e 2028 2339 3538 290a  ternals. (#958).
+000098c0: 2a20 4669 7820 6578 616d 706c 6520 636c  * Fix example cl
+000098d0: 6173 7320 6060 4f64 6449 6e74 6060 2e20  ass ``OddInt``. 
+000098e0: 2823 3937 3329 0a2a 2041 6464 2044 6f73  (#973).* Add Dos
+000098f0: 2061 6e64 2044 6f6e 7473 2066 6f72 2077   and Donts for w
+00009900: 7269 7469 6e67 2063 6861 6e67 6520 6861  riting change ha
+00009910: 6e64 6c65 7273 2e20 2823 3130 3137 290a  ndlers. (#1017).
+00009920: 2a20 436c 6172 6966 7920 7768 656e 2064  * Clarify when d
+00009930: 6566 6175 6c74 2069 6e69 7469 616c 697a  efault initializ
+00009940: 6572 2069 7320 6361 6c6c 6564 2061 6e64  er is called and
+00009950: 2077 6865 6e20 6861 6e64 6c65 7273 2061   when handlers a
+00009960: 7265 2072 6567 6973 7465 7265 642e 0a20  re registered.. 
+00009970: 2028 2331 3031 3929 0a2a 2046 6978 2064   (#1019).* Fix d
+00009980: 6f63 756d 656e 7461 7469 6f6e 2072 656e  ocumentation ren
+00009990: 6465 7269 6e67 2069 7373 7565 7320 616e  dering issues an
+000099a0: 6420 6672 6f6e 7420 6d61 7474 6572 2e20  d front matter. 
+000099b0: 2823 3130 3339 2c20 2331 3035 3329 0a2a  (#1039, #1053).*
+000099c0: 2043 6c61 7269 6679 2077 6865 6e20 6479   Clarify when dy
+000099d0: 6e61 6d69 6320 6465 6661 756c 7420 7661  namic default va
+000099e0: 6c75 6573 2061 7265 2063 6f6e 7369 6465  lues are conside
+000099f0: 7265 6420 746f 2068 6176 6520 6578 6973  red to have exis
+00009a00: 7465 642e 2028 2331 3036 3829 0a2a 2045  ted. (#1068).* E
+00009a10: 7870 616e 6420 7573 6572 206d 616e 7561  xpand user manua
+00009a20: 6c20 6f6e 2063 6f6e 7461 696e 6572 2074  l on container t
+00009a30: 7261 6974 7320 616e 6420 6f62 6a65 6374  raits and object
+00009a40: 732e 2028 2331 3035 3829 0a2a 2041 6464  s. (#1058).* Add
+00009a50: 2069 6e74 6572 7370 6869 6e78 2073 7570   intersphinx sup
+00009a60: 706f 7274 2074 6f20 636f 6e66 6967 7572  port to configur
+00009a70: 6174 696f 6e2e 2028 2331 3133 3629 0a2a  ation. (#1136).*
+00009a80: 2041 6464 2075 7365 7220 6d61 6e75 616c   Add user manual
+00009a90: 2073 6563 7469 6f6e 206f 6e20 7468 6520   section on the 
+00009aa0: 6e65 7720 6060 6f62 7365 7276 6560 6020  new ``observe`` 
+00009ab0: 6e6f 7469 6669 6361 7469 6f6e 2073 7973  notification sys
+00009ac0: 7465 6d2e 2028 2331 3036 302c 0a20 2023  tem. (#1060,.  #
+00009ad0: 3131 3430 2c20 2331 3134 3329 0a2a 2041  1140, #1143).* A
+00009ae0: 6464 2075 7365 7220 6d61 6e75 616c 2073  dd user manual s
+00009af0: 6563 7469 6f6e 206f 6e20 7468 6520 6060  ection on the ``
+00009b00: 556e 696f 6e60 6020 7472 6169 7420 7479  Union`` trait ty
+00009b10: 7065 2061 6e64 2068 6f77 2074 6f20 6d69  pe and how to mi
+00009b20: 6772 6174 6520 6672 6f6d 0a20 2060 6045  grate from.  ``E
+00009b30: 6974 6865 7260 6020 2823 3737 392c 2023  ither`` (#779, #
+00009b40: 3131 3533 2c20 2331 3136 3229 0a2a 204f  1153, #1162).* O
+00009b50: 7468 6572 206d 696e 6f72 2063 6c65 616e  ther minor clean
+00009b60: 7570 7320 616e 6420 6669 7865 732e 2028  ups and fixes. (
+00009b70: 2339 3439 2c20 2331 3134 312c 2023 3131  #949, #1141, #11
+00009b80: 3738 290a 0a54 6573 7420 7375 6974 650a  78)..Test suite.
+00009b90: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 2a20 416c  ~~~~~~~~~~..* Al
+00009ba0: 6c6f 7720 7465 7374 7320 746f 2062 6520  low tests to be 
+00009bb0: 736b 6970 7065 6420 6966 2054 7261 6974  skipped if Trait
+00009bc0: 7355 4920 6973 206e 6f74 2069 6e73 7461  sUI is not insta
+00009bd0: 6c6c 6564 2e20 2823 3130 3338 290a 2a20  lled. (#1038).* 
+00009be0: 4164 6420 6060 6578 7472 6173 5f72 6571  Add ``extras_req
+00009bf0: 7569 7265 6060 2065 6e74 7279 2066 6f72  uire`` entry for
+00009c00: 2074 6573 7469 6e67 2e20 2823 3837 3929   testing. (#879)
+00009c10: 0a2a 2041 6464 2074 6573 7473 2066 6f72  .* Add tests for
+00009c20: 2070 6172 7369 6e67 2060 606f 6e5f 7472   parsing ``on_tr
+00009c30: 6169 745f 6368 616e 6765 6060 206d 696e  ait_change`` min
+00009c40: 692d 6c61 6e67 7561 6765 2e20 2823 3932  i-language. (#92
+00009c50: 3129 0a2a 2046 6978 2061 206d 6973 7369  1).* Fix a missi
+00009c60: 6e67 2069 6d70 6f72 7420 746f 2061 6c6c  ng import to all
+00009c70: 6f77 2061 2074 6573 7420 6d6f 6475 6c65  ow a test module
+00009c80: 2074 6f20 6265 2072 756e 2073 7461 6e64   to be run stand
+00009c90: 616c 6f6e 652e 2028 2339 3631 290a 2a20  alone. (#961).* 
+00009ca0: 4164 6420 6120 4755 4920 7465 7374 2066  Add a GUI test f
+00009cb0: 6f72 2060 6045 6e75 6d2e 6372 6561 7465  or ``Enum.create
+00009cc0: 5f65 6469 746f 7260 602e 2028 2339 3838  _editor``. (#988
+00009cd0: 290a 2a20 4669 7820 736f 6d65 206d 6f64  ).* Fix some mod
+00009ce0: 756c 652d 6c65 7665 6c20 6060 4465 7072  ule-level ``Depr
+00009cf0: 6563 6174 696f 6e57 6172 6e69 6e67 6060  ecationWarning``
+00009d00: 206d 6573 7361 6765 732e 2028 2331 3135   messages. (#115
+00009d10: 3729 0a0a 4275 696c 6420 616e 6420 636f  7)..Build and co
+00009d20: 6e74 696e 756f 7573 2069 6e74 6567 7261  ntinuous integra
+00009d30: 7469 6f6e 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  tion.~~~~~~~~~~~
+00009d40: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00009d50: 7e7e 7e7e 7e0a 2a20 4349 206e 6f20 6c6f  ~~~~~.* CI no lo
+00009d60: 6e67 6572 2072 756e 7320 6f6e 2050 7974  nger runs on Pyt
+00009d70: 686f 6e20 332e 3520 2823 3130 3434 290a  hon 3.5 (#1044).
+00009d80: 2a20 4164 6420 636f 6e66 6967 6f62 6a20  * Add configobj 
+00009d90: 6465 7065 6e64 656e 6379 2061 6e64 2072  dependency and r
+00009da0: 656d 6f76 6520 7265 6d61 696e 696e 6720  emove remaining 
+00009db0: 332e 3520 7265 6665 7265 6e63 6573 2069  3.5 references i
+00009dc0: 6e0a 2020 6060 6574 7374 6f6f 6c2e 7079  n.  ``etstool.py
+00009dd0: 6060 2e20 2823 3130 3531 290a 2a20 436f  ``. (#1051).* Co
+00009de0: 6465 636f 7620 7265 706f 7274 7320 6172  decov reports ar
+00009df0: 6520 6e6f 206c 6f6e 6765 7220 7265 7472  e no longer retr
+00009e00: 6965 7665 6420 666f 7220 7075 6c6c 2072  ieved for pull r
+00009e10: 6571 7565 7374 732e 2028 2331 3130 3929  equests. (#1109)
+00009e20: 0a2a 2043 4920 7465 7374 7320 7265 7175  .* CI tests requ
+00009e30: 6972 696e 6720 6120 4755 4920 6172 6520  iring a GUI are 
+00009e40: 6e6f 7720 7275 6e20 6167 6169 6e73 7420  now run against 
+00009e50: 5079 5174 3520 7261 7468 6572 2074 6861  PyQt5 rather tha
+00009e60: 6e20 5079 5174 342e 0a20 2028 2331 3132  n PyQt4..  (#112
+00009e70: 3729 0a2a 2041 6464 2053 6c61 636b 206e  7).* Add Slack n
+00009e80: 6f74 6966 6963 6174 696f 6e73 2066 6f72  otifications for
+00009e90: 2043 492e 2028 2331 3037 3429 0a2a 2046   CI. (#1074).* F
+00009ea0: 6978 2061 6e64 2069 6d70 726f 7665 2076  ix and improve v
+00009eb0: 6172 696f 7573 2060 6073 6574 7570 2e70  arious ``setup.p
+00009ec0: 7960 6020 7061 636b 6167 6520 6d65 7461  y`` package meta
+00009ed0: 6461 7461 2066 6965 6c64 732e 2028 2331  data fields. (#1
+00009ee0: 3138 3529 0a0a 4d61 696e 7465 6e61 6e63  185)..Maintenanc
+00009ef0: 6520 616e 6420 636f 6465 206f 7267 616e  e and code organ
+00009f00: 697a 6174 696f 6e0a 7e7e 7e7e 7e7e 7e7e  ization.~~~~~~~~
+00009f10: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00009f20: 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a 2052 6566  ~~~~~~~~~..* Ref
+00009f30: 6163 746f 7220 4348 6173 5472 6169 7473  actor CHasTraits
+00009f40: 2060 6074 7261 6974 735f 696e 6974 6564   ``traits_inited
+00009f50: 6060 206d 6574 686f 642e 2028 2338 3432  `` method. (#842
+00009f60: 290a 2a20 4164 6420 7375 7070 6f72 7420  ).* Add support 
+00009f70: 666f 7220 7072 6572 656c 6561 7365 2073  for prerelease s
+00009f80: 6563 7469 6f6e 2069 6e20 7665 7273 696f  ection in versio
+00009f90: 6e2e 2028 2338 3634 290a 2a20 5265 6e61  n. (#864).* Rena
+00009fa0: 6d65 2063 6f6d 7061 7269 736f 6e20 6d6f  me comparison mo
+00009fb0: 6465 2069 6e74 6567 6572 2063 6f6e 7374  de integer const
+00009fc0: 616e 7473 2069 6e20 6060 6374 7261 6974  ants in ``ctrait
+00009fd0: 732e 6360 602e 2028 2338 3632 290a 2a20  s.c``. (#862).* 
+00009fe0: 466f 6c6c 6f77 2062 6573 7420 7072 6163  Follow best prac
+00009ff0: 7469 6365 7320 7768 656e 206f 7065 6e69  tices when openi
+0000a000: 6e67 2066 696c 6573 2e20 2823 3837 3229  ng files. (#872)
+0000a010: 0a2a 2049 6e69 7469 616c 697a 6520 6060  .* Initialize ``
+0000a020: 6354 7261 6974 6060 2060 6067 6574 6174  cTrait`` ``getat
+0000a030: 7472 6060 2c20 6060 7365 7461 7474 7260  tr``, ``setattr`
+0000a040: 6020 6861 6e64 6c65 7273 2069 6e20 6060  ` handlers in ``
+0000a050: 7470 5f6e 6577 6060 2e20 2823 3837 3529  tp_new``. (#875)
+0000a060: 0a2a 2043 6865 636b 2060 6074 7261 6974  .* Check ``trait
+0000a070: 5f63 6861 6e67 655f 6e6f 7469 6679 6060  _change_notify``
+0000a080: 2065 6172 6c79 2069 6e20 6060 6361 6c6c   early in ``call
+0000a090: 5f6e 6f74 6966 6965 7273 6060 2e20 2823  _notifiers``. (#
+0000a0a0: 3931 3729 0a2a 2052 6566 6163 746f 7220  917).* Refactor 
+0000a0b0: 6060 6374 7261 6974 732e 6360 6020 666f  ``ctraits.c`` fo
+0000a0c0: 7220 6361 6c6c 696e 6720 7472 6169 7420  r calling trait 
+0000a0d0: 616e 6420 6f62 6a65 6374 206e 6f74 6966  and object notif
+0000a0e0: 6965 7273 2e20 2823 3931 3829 0a2a 2060  iers. (#918).* `
+0000a0f0: 6042 6173 6545 6e75 6d60 6020 616e 6420  `BaseEnum`` and 
+0000a100: 6060 456e 756d 6060 2066 6978 6573 2061  ``Enum`` fixes a
+0000a110: 6e64 2063 6c65 616e 7570 2e20 2823 3936  nd cleanup. (#96
+0000a120: 3829 0a2a 2053 706c 6974 2060 6063 7472  8).* Split ``ctr
+0000a130: 6169 7473 6060 2070 726f 7065 7274 7920  aits`` property 
+0000a140: 6170 6920 746f 2060 605f 7365 745f 7072  api to ``_set_pr
+0000a150: 6f70 6572 7479 6060 2061 6e64 2060 605f  operty`` and ``_
+0000a160: 6765 745f 7072 6f70 6572 7479 6060 2e0a  get_property``..
+0000a170: 2020 2823 3936 3729 0a2a 2046 6978 206f    (#967).* Fix o
+0000a180: 7665 7263 6f6d 706c 6963 6174 6564 2060  vercomplicated `
+0000a190: 605f 5f64 6565 7063 6f70 795f 5f60 6020  `__deepcopy__`` 
+0000a1a0: 696d 706c 656d 656e 7461 7469 6f6e 2e20  implementation. 
+0000a1b0: 2823 3939 3229 0a2a 2041 6464 2060 605f  (#992).* Add ``_
+0000a1c0: 5f72 6570 725f 5f60 6020 696d 706c 656d  _repr__`` implem
+0000a1d0: 656e 7461 7469 6f6e 2066 6f72 2060 6054  entation for ``T
+0000a1e0: 7261 6974 4c69 7374 4576 656e 7460 602c  raitListEvent``,
+0000a1f0: 2060 6054 7261 6974 4469 6374 4576 656e   ``TraitDictEven
+0000a200: 7460 600a 2020 616e 6420 6060 5472 6169  t``.  and ``Trai
+0000a210: 7453 6574 4576 656e 7460 602e 2028 2331  tSetEvent``. (#1
+0000a220: 3030 362c 2023 3131 3438 2c20 2331 3134  006, #1148, #114
+0000a230: 3929 0a2a 2052 656d 6f76 6520 6361 6368  9).* Remove cach
+0000a240: 696e 6720 6f66 2065 6469 746f 7220 6661  ing of editor fa
+0000a250: 6374 6f72 6965 732e 2028 2331 3033 3229  ctories. (#1032)
+0000a260: 0a2a 2052 656d 6f76 6520 636f 6e64 6974  .* Remove condit
+0000a270: 696f 6e61 6c20 7472 6169 7473 7569 2069  ional traitsui i
+0000a280: 6d70 6f72 7473 2e20 2823 3130 3333 290a  mports. (#1033).
+0000a290: 2a20 5265 6d6f 7665 2063 6f64 6520 6475  * Remove code du
+0000a2a0: 706c 6963 6174 696f 6e20 696e 2060 6074  plication in ``t
+0000a2b0: 7574 6f72 2e70 7960 602e 2028 2331 3033  utor.py``. (#103
+0000a2c0: 3429 0a2a 2046 6978 2063 6f72 7265 6374  4).* Fix correct
+0000a2d0: 6e65 7373 2069 6e20 6060 456e 756d 6060  ness in ``Enum``
+0000a2e0: 2064 6566 6175 6c74 2074 7261 6974 7375   default traitsu
+0000a2f0: 6920 6564 6974 6f72 2e20 2823 3130 3132  i editor. (#1012
+0000a300: 290a 2a20 5573 6520 6060 4e55 4c4c 6060  ).* Use ``NULL``
+0000a310: 2066 6f72 207a 6572 6f2d 6172 6775 6d65   for zero-argume
+0000a320: 6e74 2060 6050 794f 626a 6563 745f 4361  nt ``PyObject_Ca
+0000a330: 6c6c 4d65 7468 6f64 6060 2066 6f72 6d61  llMethod`` forma
+0000a340: 742e 2028 2331 3130 3029 0a2a 204d 6973  t. (#1100).* Mis
+0000a350: 6365 6c6c 616e 656f 7573 206f 7468 6572  cellaneous other
+0000a360: 206d 696e 6f72 2066 6978 6573 2c20 7265   minor fixes, re
+0000a370: 6661 6374 6f72 696e 6773 2061 6e64 2063  factorings and c
+0000a380: 6c65 616e 7570 732e 2028 2338 3734 2c20  leanups. (#874, 
+0000a390: 2338 3832 2c0a 2020 2339 3135 2c20 2339  #882,.  #915, #9
+0000a3a0: 3230 2c20 2339 3233 2c20 2339 3234 2c20  20, #923, #924, 
+0000a3b0: 2339 3335 2c20 2339 3339 2c20 2339 3434  #935, #939, #944
+0000a3c0: 2c20 2339 3530 2c20 2339 3634 290a 0a0a  , #950, #964)...
+0000a3d0: 5265 6c65 6173 6520 362e 302e 300a 2d2d  Release 6.0.0.--
+0000a3e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 656c  -----------..Rel
+0000a3f0: 6561 7365 643a 2032 3032 302d 3032 2d31  eased: 2020-02-1
+0000a400: 340a 0a4e 6f20 6368 616e 6765 7320 7369  4..No changes si
+0000a410: 6e63 6520 7468 6520 362e 302e 3072 6330  nce the 6.0.0rc0
+0000a420: 2072 656c 6561 7365 2063 616e 6469 6461   release candida
+0000a430: 7465 2e0a 0a0a 5265 6c65 6173 6520 362e  te....Release 6.
+0000a440: 302e 3072 6330 0a2d 2d2d 2d2d 2d2d 2d2d  0.0rc0.---------
+0000a450: 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561 7365  -------..Release
+0000a460: 643a 2032 3032 302d 3031 2d33 300a 0a52  d: 2020-01-30..R
+0000a470: 656c 6561 7365 206e 6f74 6573 0a7e 7e7e  elease notes.~~~
+0000a480: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 5472 6169  ~~~~~~~~~~..Trai
+0000a490: 7473 2036 2e30 2069 7320 6120 6d61 6a6f  ts 6.0 is a majo
+0000a4a0: 7220 7570 6461 7465 2074 6f20 7468 6520  r update to the 
+0000a4b0: 5472 6169 7473 2070 6163 6b61 6765 2c20  Traits package, 
+0000a4c0: 7769 7468 2061 206e 756d 6265 7220 6f66  with a number of
+0000a4d0: 0a62 6163 6b77 6172 6420 696e 636f 6d70  .backward incomp
+0000a4e0: 6174 6962 6c65 2063 6861 6e67 6573 2066  atible changes f
+0000a4f0: 726f 6d20 6974 7320 7072 6564 6563 6573  rom its predeces
+0000a500: 736f 722e 204e 6f74 6162 6c65 2063 6861  sor. Notable cha
+0000a510: 6e67 6573 3a0a 0a2a 2050 7974 686f 6e20  nges:..* Python 
+0000a520: 322e 3720 6973 206e 6f20 6c6f 6e67 6572  2.7 is no longer
+0000a530: 2073 7570 706f 7274 6564 3b20 5472 6169   supported; Trai
+0000a540: 7473 2036 2e30 2072 6571 7569 7265 7320  ts 6.0 requires 
+0000a550: 5079 7468 6f6e 2033 2e35 206f 7220 6c61  Python 3.5 or la
+0000a560: 7465 722e 0a2a 2054 7261 6974 2074 7970  ter..* Trait typ
+0000a570: 6573 2072 656c 6174 6564 2074 6f20 5079  es related to Py
+0000a580: 7468 6f6e 2032 2028 666f 7220 6578 616d  thon 2 (for exam
+0000a590: 706c 6520 6060 556e 6963 6f64 6560 6020  ple ``Unicode`` 
+0000a5a0: 616e 6420 6060 4c6f 6e67 6060 2920 6861  and ``Long``) ha
+0000a5b0: 7665 0a20 2062 6565 6e20 6465 7072 6563  ve.  been deprec
+0000a5c0: 6174 6564 2069 6e20 6661 766f 7572 206f  ated in favour o
+0000a5d0: 6620 7468 6569 7220 5079 7468 6f6e 2033  f their Python 3
+0000a5e0: 2065 7175 6976 616c 656e 7473 2028 666f   equivalents (fo
+0000a5f0: 7220 6578 616d 706c 6520 6060 5374 7260  r example ``Str`
+0000a600: 600a 2020 616e 6420 6060 496e 7460 6029  `.  and ``Int``)
+0000a610: 2e0a 2a20 4d61 6e79 206c 6974 746c 652d  ..* Many little-
+0000a620: 7573 6564 2068 6973 746f 7269 6361 6c20  used historical 
+0000a630: 6665 6174 7572 6573 206f 6620 5472 6169  features of Trai
+0000a640: 7473 2068 6176 6520 6265 656e 2064 6570  ts have been dep
+0000a650: 7265 6361 7465 642c 2061 6e64 0a20 2061  recated, and.  a
+0000a660: 7265 2073 6368 6564 756c 6564 2066 6f72  re scheduled for
+0000a670: 2072 656d 6f76 616c 2069 6e20 5472 6169   removal in Trai
+0000a680: 7473 2037 2e30 2e0a 2a20 536f 6d65 2068  ts 7.0..* Some h
+0000a690: 6973 746f 7269 6361 6c20 6665 6174 7572  istorical featur
+0000a6a0: 6573 206f 6620 5472 6169 7473 2074 6861  es of Traits tha
+0000a6b0: 7420 6861 6420 6e6f 2065 7669 6465 6e63  t had no evidenc
+0000a6c0: 6520 6f66 2065 7874 6572 6e61 6c20 7573  e of external us
+0000a6d0: 6167 650a 2020 7765 7265 2072 656d 6f76  age.  were remov
+0000a6e0: 6564 2069 6e20 5472 6169 7473 2036 2e30  ed in Traits 6.0
+0000a6f0: 2e0a 2a20 496e 7472 6f73 7065 6374 696f  ..* Introspectio
+0000a700: 6e20 6f66 2060 6043 5472 6169 7460 6020  n of ``CTrait`` 
+0000a710: 616e 6420 6060 4861 7354 7261 6974 7360  and ``HasTraits`
+0000a720: 6020 6f62 6a65 6374 7320 6973 2067 7265  ` objects is gre
+0000a730: 6174 6c79 2069 6d70 726f 7665 642e 0a20  atly improved.. 
+0000a740: 2041 6c6c 206f 6620 7468 6520 696e 7465   All of the inte
+0000a750: 726e 616c 2073 7461 7465 2074 6861 7420  rnal state that 
+0000a760: 7761 7320 7072 6576 696f 7573 6c79 2068  was previously h
+0000a770: 6964 6465 6e20 7769 7468 696e 2074 6865  idden within the
+0000a780: 2043 2065 7874 656e 7369 6f6e 0a20 2069   C extension.  i
+0000a790: 7320 6e6f 7720 6163 6365 7373 6962 6c65  s now accessible
+0000a7a0: 2066 726f 6d20 5079 7468 6f6e 2e0a 2a20   from Python..* 
+0000a7b0: 5468 6520 5472 6169 7473 2063 6f64 6562  The Traits codeb
+0000a7c0: 6173 6520 6861 7320 756e 6465 7267 6f6e  ase has undergon
+0000a7d0: 6520 736f 6d65 2073 6967 6e69 6669 6361  e some significa
+0000a7e0: 6e74 2072 656f 7267 616e 697a 6174 696f  nt reorganizatio
+0000a7f0: 6e73 2c0a 2020 7265 666f 726d 6174 7469  ns,.  reformatti
+0000a800: 6e67 7320 616e 6420 7374 796c 6520 636c  ngs and style cl
+0000a810: 6561 6e75 7073 2074 6f20 6d61 6b65 2069  eanups to make i
+0000a820: 7420 6561 7369 6572 2074 6f20 776f 726b  t easier to work
+0000a830: 2077 6974 682c 2061 6e64 0a20 2074 6f20   with, and.  to 
+0000a840: 696d 7072 6f76 6520 7468 6520 7365 7061  improve the sepa
+0000a850: 7261 7469 6f6e 2062 6574 7765 656e 2054  ration between T
+0000a860: 7261 6974 7320 616e 6420 5472 6169 7473  raits and Traits
+0000a870: 5549 2e0a 2a20 5468 6973 2072 656c 6561  UI..* This relea
+0000a880: 7365 2077 6173 2066 6f63 7573 6564 206d  se was focused m
+0000a890: 6169 6e6c 7920 6f6e 2063 6c65 616e 7570  ainly on cleanup
+0000a8a0: 2061 6e64 2062 7567 6669 7869 6e67 2e20   and bugfixing. 
+0000a8b0: 4e65 7665 7274 6865 6c65 7373 2c0a 2020  Nevertheless,.  
+0000a8c0: 6974 2063 6f6e 7461 696e 7320 6120 7370  it contains a sp
+0000a8d0: 7269 6e6b 6c69 6e67 206f 6620 6e65 7720  rinkling of new 
+0000a8e0: 6665 6174 7572 6573 2e20 5468 6572 6527  features. There'
+0000a8f0: 7320 6120 6e65 7720 6060 4461 7465 7469  s a new ``Dateti
+0000a900: 6d65 6060 0a20 2074 7261 6974 2074 7970  me``.  trait typ
+0000a910: 652e 2054 6865 2060 6045 6e75 6d60 6020  e. The ``Enum`` 
+0000a920: 7472 6169 7420 7479 7065 206e 6f77 2073  trait type now s
+0000a930: 7570 706f 7274 7320 5079 7468 6f6e 2065  upports Python e
+0000a940: 6e75 6d65 7261 7469 6f6e 732e 0a20 2054  numerations..  T
+0000a950: 6865 2060 6046 696c 6560 6020 7472 6169  he ``File`` trai
+0000a960: 7420 7479 7065 2073 7570 706f 7274 7320  t type supports 
+0000a970: 7061 7468 2d6c 696b 6520 6f62 6a65 6374  path-like object
+0000a980: 732e 0a0a 4d6f 7265 2074 6861 6e20 3135  s...More than 15
+0000a990: 3020 5052 7320 7765 6e74 2069 6e74 6f20  0 PRs went into 
+0000a9a0: 7468 6973 2072 656c 6561 7365 2e20 5468  this release. Th
+0000a9b0: 6520 666f 6c6c 6f77 696e 6720 7065 6f70  e following peop
+0000a9c0: 6c65 2063 6f6e 7472 6962 7574 6564 0a63  le contributed.c
+0000a9d0: 6f64 6520 6368 616e 6765 7320 666f 7220  ode changes for 
+0000a9e0: 7468 6973 2072 656c 6561 7365 3a0a 0a2a  this release:..*
+0000a9f0: 204b 6974 2059 616e 2043 686f 690a 2a20   Kit Yan Choi.* 
+0000aa00: 4d61 726b 2044 6963 6b69 6e73 6f6e 0a2a  Mark Dickinson.*
+0000aa10: 204b 6576 696e 2044 7566 660a 2a20 526f   Kevin Duff.* Ro
+0000aa20: 6265 7274 204b 6572 6e0a 2a20 4d69 6468  bert Kern.* Midh
+0000aa30: 756e 204d 6164 6875 736f 6f64 616e 616e  un Madhusoodanan
+0000aa40: 0a2a 2053 686f 6562 204d 6f68 616d 6d65  .* Shoeb Mohamme
+0000aa50: 640a 2a20 5361 6920 5261 6875 6c20 506f  d.* Sai Rahul Po
+0000aa60: 7275 7269 0a2a 2043 6f72 7261 6e20 5765  ruri.* Corran We
+0000aa70: 6273 7465 720a 2a20 4a6f 686e 2057 6967  bster.* John Wig
+0000aa80: 6769 6e73 0a0a 506f 7274 696e 6720 6775  gins..Porting gu
+0000aa90: 6964 650a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ide.~~~~~~~~~~~~
+0000aaa0: 7e0a 0a46 6f72 2074 6865 206d 6f73 7420  ~..For the most 
+0000aab0: 7061 7274 2c20 6578 6973 7469 6e67 2063  part, existing c
+0000aac0: 6f64 6520 7468 6174 2077 6f72 6b73 2077  ode that works w
+0000aad0: 6974 6820 5472 6169 7473 2035 2e32 2e30  ith Traits 5.2.0
+0000aae0: 2073 686f 756c 640a 636f 6e74 696e 7565   should.continue
+0000aaf0: 2074 6f20 776f 726b 2077 6974 6820 5472   to work with Tr
+0000ab00: 6169 7473 2036 2e30 2e30 2077 6974 686f  aits 6.0.0 witho
+0000ab10: 7574 2063 6861 6e67 6573 2e20 486f 7765  ut changes. Howe
+0000ab20: 7665 722c 2074 6865 7265 0a61 7265 2073  ver, there.are s
+0000ab30: 6f6d 6520 706f 7465 6e74 6961 6c6c 7920  ome potentially 
+0000ab40: 6272 6561 6b69 6e67 2063 6861 6e67 6573  breaking changes
+0000ab50: 2069 6e20 5472 6169 7473 2036 2e30 2e30   in Traits 6.0.0
+0000ab60: 2c20 616e 6420 7765 2072 6563 6f6d 6d65  , and we recomme
+0000ab70: 6e64 0a61 7070 6c79 696e 6720 6361 7574  nd.applying caut
+0000ab80: 696f 6e20 7768 656e 2075 7067 7261 6469  ion when upgradi
+0000ab90: 6e67 2e0a 0a48 6572 6527 7320 6120 6775  ng...Here's a gu
+0000aba0: 6964 6520 746f 2064 6561 6c69 6e67 2077  ide to dealing w
+0000abb0: 6974 6820 736f 6d65 206f 6620 7468 6520  ith some of the 
+0000abc0: 706f 7465 6e74 6961 6c6c 7920 6272 6561  potentially brea
+0000abd0: 6b69 6e67 2063 6861 6e67 6573 2e0a 0a2a  king changes...*
+0000abe0: 2054 6865 2060 6055 6e69 636f 6465 6060   The ``Unicode``
+0000abf0: 2061 6e64 2060 6043 556e 6963 6f64 6560   and ``CUnicode`
+0000ac00: 6020 7472 6169 7420 7479 7065 7320 6172  ` trait types ar
+0000ac10: 6520 6e6f 7720 7369 6d70 6c79 2073 796e  e now simply syn
+0000ac20: 6f6e 796d 7320 666f 720a 2020 6060 5374  onyms for.  ``St
+0000ac30: 7260 6020 616e 6420 6060 4353 7472 6060  r`` and ``CStr``
+0000ac40: 2e20 6060 556e 6963 6f64 6560 6020 616e  . ``Unicode`` an
+0000ac50: 6420 6060 4355 6e69 636f 6465 6060 2061  d ``CUnicode`` a
+0000ac60: 7265 2063 6f6e 7369 6465 7265 6420 6465  re considered de
+0000ac70: 7072 6563 6174 6564 2e0a 2020 466f 7220  precated..  For 
+0000ac80: 6e6f 772c 206e 6f20 6465 7072 6563 6174  now, no deprecat
+0000ac90: 696f 6e20 7761 726e 696e 6720 6973 2069  ion warning is i
+0000aca0: 7373 7565 6420 6f6e 2075 7365 206f 6620  ssued on use of 
+0000acb0: 7468 6573 6520 6465 7072 6563 6174 6564  these deprecated
+0000acc0: 2074 7261 6974 0a20 2074 7970 6573 2c20   trait.  types, 
+0000acd0: 6275 7420 696e 2054 7261 6974 7320 362e  but in Traits 6.
+0000ace0: 312e 3020 616e 6420 6c61 7465 722c 2077  1.0 and later, w
+0000acf0: 6172 6e69 6e67 7320 6d61 7920 6265 2069  arnings may be i
+0000ad00: 7373 7565 642c 2061 6e64 2069 6e20 5472  ssued, and in Tr
+0000ad10: 6169 7473 0a20 2037 2e30 2e30 2074 6865  aits.  7.0.0 the
+0000ad20: 7365 2074 7261 6974 2074 7970 6573 206d  se trait types m
+0000ad30: 6179 2062 6520 7265 6d6f 7665 642e 2049  ay be removed. I
+0000ad40: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
+0000ad50: 7468 6174 2075 7365 7273 2075 7064 6174  that users updat
+0000ad60: 650a 2020 616c 6c20 7573 6573 206f 6620  e.  all uses of 
+0000ad70: 6060 556e 6963 6f64 6560 6020 746f 2060  ``Unicode`` to `
+0000ad80: 6053 7472 6060 2061 6e64 2060 6043 556e  `Str`` and ``CUn
+0000ad90: 6963 6f64 6560 6020 746f 2060 6043 5374  icode`` to ``CSt
+0000ada0: 7260 6020 746f 2061 766f 6964 0a20 2077  r`` to avoid.  w
+0000adb0: 6172 6e69 6e67 7320 6f72 2065 7272 6f72  arnings or error
+0000adc0: 7320 696e 2074 6865 2066 7574 7572 652e  s in the future.
+0000add0: 0a0a 2a20 5369 6d69 6c61 726c 792c 2060  ..* Similarly, `
+0000ade0: 604c 6f6e 6760 6020 616e 6420 6060 434c  `Long`` and ``CL
+0000adf0: 6f6e 6760 6020 6172 6520 6e6f 7720 7379  ong`` are now sy
+0000ae00: 6e6f 6e79 6d73 2066 6f72 2060 6049 6e74  nonyms for ``Int
+0000ae10: 6060 2061 6e64 2060 6043 496e 7460 602e  `` and ``CInt``.
+0000ae20: 0a20 2054 6865 2073 616d 6520 7265 636f  .  The same reco
+0000ae30: 6d6d 656e 6461 7469 6f6e 7320 6170 706c  mmendations appl
+0000ae40: 7920 6173 2066 6f72 2074 6865 2060 6055  y as for the ``U
+0000ae50: 6e69 636f 6465 6060 202f 2060 6053 7472  nicode`` / ``Str
+0000ae60: 6060 2074 7261 6974 2074 7970 6573 2e0a  `` trait types..
+0000ae70: 0a2a 2055 7365 7320 6f66 2060 604e 4f5f  .* Uses of ``NO_
+0000ae80: 434f 4d50 4152 4560 602c 2060 604f 424a  COMPARE``, ``OBJ
+0000ae90: 4543 545f 4944 454e 5449 5459 5f43 4f4d  ECT_IDENTITY_COM
+0000aea0: 5041 5245 6060 2061 6e64 2060 6052 4943  PARE`` and ``RIC
+0000aeb0: 485f 434f 4d50 4152 4560 600a 2020 7368  H_COMPARE``.  sh
+0000aec0: 6f75 6c64 2062 6520 7265 706c 6163 6564  ould be replaced
+0000aed0: 2077 6974 6820 7468 6520 6170 7072 6f70   with the approp
+0000aee0: 7269 6174 6520 6060 436f 6d70 6172 6973  riate ``Comparis
+0000aef0: 6f6e 4d6f 6465 6060 2065 6e75 6d65 7261  onMode`` enumera
+0000af00: 7469 6f6e 0a20 206d 656d 6265 7273 2e0a  tion.  members..
+0000af10: 0a2a 2054 6865 2076 616c 6964 6174 696f  .* The validatio
+0000af20: 6e20 666f 7220 6120 6060 496e 7374 616e  n for a ``Instan
+0000af30: 6365 2849 536f 6d65 496e 7465 7266 6163  ce(ISomeInterfac
+0000af40: 6529 6060 2074 7261 6974 2074 7970 6520  e)`` trait type 
+0000af50: 6861 7320 6368 616e 6765 642c 0a20 2077  has changed,.  w
+0000af60: 6865 7265 2060 6049 536f 6d65 496e 7465  here ``ISomeInte
+0000af70: 7266 6163 6560 6020 6973 2061 2073 7562  rface`` is a sub
+0000af80: 636c 6173 7320 6f66 2060 6049 6e74 6572  class of ``Inter
+0000af90: 6661 6365 6060 2e20 5072 6576 696f 7573  face``. Previous
+0000afa0: 6c79 2c20 616e 0a20 2061 7373 6967 6e6d  ly, an.  assignm
+0000afb0: 656e 7420 746f 2073 7563 6820 6120 7472  ent to such a tr
+0000afc0: 6169 7420 7661 6c69 6461 7465 6420 7468  ait validated th
+0000afd0: 6520 7479 7065 206f 6620 7468 6520 6173  e type of the as
+0000afe0: 7369 676e 6564 2076 616c 7565 2061 6761  signed value aga
+0000aff0: 696e 7374 0a20 2074 6865 2069 6e74 6572  inst.  the inter
+0000b000: 6661 6365 2c20 6d65 7468 6f64 2062 7920  face, method by 
+0000b010: 6d65 7468 6f64 2e20 4e6f 7720 616e 2060  method. Now an `
+0000b020: 6069 7369 6e73 7461 6e63 6560 6020 6368  `isinstance`` ch
+0000b030: 6563 6b20 6973 2070 6572 666f 726d 6564  eck is performed
+0000b040: 0a20 2061 6761 696e 7374 2074 6865 2069  .  against the i
+0000b050: 6e74 6572 6661 6365 2069 6e73 7465 6164  nterface instead
+0000b060: 2e20 4d61 6b65 2073 7572 6520 7468 6174  . Make sure that
+0000b070: 2063 6c61 7373 6573 2069 6d70 6c65 6d65   classes impleme
+0000b080: 6e74 696e 6720 6120 6769 7665 6e0a 2020  nting a given.  
+0000b090: 696e 7465 7266 6163 6520 6861 7665 2074  interface have t
+0000b0a0: 6865 2061 7070 726f 7072 6961 7465 2060  he appropriate `
+0000b0b0: 6070 726f 7669 6465 7360 6020 6465 636f  `provides`` deco
+0000b0c0: 7261 746f 722e 0a0a 2020 4f6e 6520 6e6f  rator...  One no
+0000b0d0: 7461 626c 6520 7369 6465 2d65 6666 6563  table side-effec
+0000b0e0: 7420 6f66 2074 6865 2061 626f 7665 2063  t of the above c
+0000b0f0: 6861 6e67 6520 6973 2074 6861 7420 706c  hange is that pl
+0000b100: 6169 6e20 6060 6d6f 636b 2e4d 6f63 6b60  ain ``mock.Mock`
+0000b110: 600a 2020 696e 7374 616e 6365 7320 6361  `.  instances ca
+0000b120: 6e20 6e6f 206c 6f6e 6765 7220 6265 2061  n no longer be a
+0000b130: 7373 6967 6e65 6420 746f 2060 6049 6e73  ssigned to ``Ins
+0000b140: 7461 6e63 6528 4953 6f6d 6549 6e74 6572  tance(ISomeInter
+0000b150: 6661 6365 2960 6020 7472 6169 7473 2e0a  face)`` traits..
+0000b160: 2020 546f 2067 6574 2061 726f 756e 6420    To get around 
+0000b170: 7468 6973 2c20 7573 6520 6060 7370 6563  this, use ``spec
+0000b180: 3d49 536f 6d65 496e 7465 7266 6163 6560  =ISomeInterface`
+0000b190: 6020 7768 656e 2063 7265 6174 696e 6720  ` when creating 
+0000b1a0: 796f 7572 206d 6f63 6b0a 2020 6f62 6a65  your mock.  obje
+0000b1b0: 6374 2e0a 0a20 2054 6869 7320 6368 616e  ct...  This chan
+0000b1c0: 6765 2064 6f65 7320 6e6f 7420 6166 6665  ge does not affe
+0000b1d0: 6374 2060 6049 6e73 7461 6e63 6560 6020  ct ``Instance`` 
+0000b1e0: 7472 6169 7473 2066 6f72 206e 6f6e 2d69  traits for non-i
+0000b1f0: 6e74 6572 6661 6365 2063 6c61 7373 6573  nterface classes
+0000b200: 2e0a 0a2a 2054 6865 2066 6f72 6d61 7420  ...* The format 
+0000b210: 6f66 2060 6054 7261 6974 4c69 7374 4576  of ``TraitListEv
+0000b220: 656e 7473 6060 2068 6173 2063 6861 6e67  ents`` has chang
+0000b230: 6564 3a20 666f 7220 6c69 7374 2065 7665  ed: for list eve
+0000b240: 6e74 7320 6765 6e65 7261 7465 6420 6672  nts generated fr
+0000b250: 6f6d 0a20 2061 2073 6c69 6365 2073 6574  om.  a slice set
+0000b260: 206f 7220 736c 6963 6520 6465 6c65 7465   or slice delete
+0000b270: 206f 7065 7261 7469 6f6e 2077 6865 7265   operation where
+0000b280: 2074 6861 7420 736c 6963 6520 6861 6420   that slice had 
+0000b290: 6120 7374 6570 206f 7468 6572 0a20 2074  a step other.  t
+0000b2a0: 6861 6e20 6060 3160 602c 2074 6865 2060  han ``1``, the `
+0000b2b0: 6061 6464 6564 6060 2061 6e64 2060 6072  `added`` and ``r
+0000b2c0: 656d 6f76 6564 6060 2066 6965 6c64 7320  emoved`` fields 
+0000b2d0: 6f66 2074 6865 2065 7665 6e74 2068 6164  of the event had
+0000b2e0: 2061 6e20 6578 7472 610a 2020 6c65 7665   an extra.  leve
+0000b2f0: 6c20 6f66 206c 6973 7420 7772 6170 7069  l of list wrappi
+0000b300: 6e67 2028 666f 7220 6578 616d 706c 652c  ng (for example,
+0000b310: 2060 6061 6464 6564 6060 206d 6967 6874   ``added`` might
+0000b320: 2062 6520 6060 5b5b 312c 2032 2c20 335d   be ``[[1, 2, 3]
+0000b330: 5d60 600a 2020 696e 7374 6561 6420 6f66  ]``.  instead of
+0000b340: 2060 605b 312c 2032 2c20 335d 6060 292e   ``[1, 2, 3]``).
+0000b350: 2049 6e20 5472 6169 7473 2036 2e30 2c20   In Traits 6.0, 
+0000b360: 7468 6973 2065 7874 7261 2077 7261 7070  this extra wrapp
+0000b370: 696e 6720 6861 7320 6265 656e 0a20 2072  ing has been.  r
+0000b380: 656d 6f76 6564 2e20 5468 6572 6520 6d61  emoved. There ma
+0000b390: 7920 6265 2065 7869 7374 696e 6720 636f  y be existing co
+0000b3a0: 6465 2074 6861 7420 7370 6563 6961 6c2d  de that special-
+0000b3b0: 6361 7365 6420 7468 6520 6578 7472 6120  cased the extra 
+0000b3c0: 7772 6170 7069 6e67 2e0a 0a2a 204d 616e  wrapping...* Man
+0000b3d0: 7920 636c 6173 7365 7320 616e 6420 6675  y classes and fu
+0000b3e0: 6e63 7469 6f6e 7320 6861 7665 206d 6f76  nctions have mov
+0000b3f0: 6564 2061 726f 756e 6420 7769 7468 696e  ed around within
+0000b400: 2074 6865 2054 7261 6974 7320 636f 6465   the Traits code
+0000b410: 6261 7365 2e0a 2020 4966 2079 6f75 2068  base..  If you h
+0000b420: 6176 6520 636f 6465 2074 6861 7420 696d  ave code that im
+0000b430: 706f 7274 7320 6469 7265 6374 6c79 2066  ports directly f
+0000b440: 726f 6d20 5472 6169 7473 206d 6f64 756c  rom Traits modul
+0000b450: 6573 2061 6e64 2073 7562 7061 636b 6167  es and subpackag
+0000b460: 6573 0a20 2069 6e73 7465 6164 206f 6620  es.  instead of 
+0000b470: 6672 6f6d 2060 6074 7261 6974 732e 6170  from ``traits.ap
+0000b480: 6960 6020 6f72 2074 6865 206f 7468 6572  i`` or the other
+0000b490: 2073 7562 7061 636b 6167 6520 6060 6170   subpackage ``ap
+0000b4a0: 6960 6020 6d6f 6475 6c65 732c 2073 6f6d  i`` modules, som
+0000b4b0: 650a 2020 6f66 2074 686f 7365 2069 6d70  e.  of those imp
+0000b4c0: 6f72 7473 206d 6179 2066 6169 6c2e 2054  orts may fail. T
+0000b4d0: 6f20 6176 6f69 6420 706f 7465 6e74 6961  o avoid potentia
+0000b4e0: 6c20 666f 7220 6060 496d 706f 7274 4572  l for ``ImportEr
+0000b4f0: 726f 7260 6073 2c20 796f 750a 2020 7368  ror``s, you.  sh
+0000b500: 6f75 6c64 2069 6d70 6f72 7420 6672 6f6d  ould import from
+0000b510: 2060 6074 7261 6974 732e 6170 6960 6020   ``traits.api`` 
+0000b520: 7768 656e 6576 6572 2070 6f73 7369 626c  whenever possibl
+0000b530: 652e 2049 6620 796f 7520 6669 6e64 2079  e. If you find y
+0000b540: 6f75 7273 656c 660a 2020 6e65 6564 696e  ourself.  needin
+0000b550: 6720 736f 6d65 2070 6965 6365 206f 6620  g some piece of 
+0000b560: 5472 6169 7473 2066 756e 6374 696f 6e61  Traits functiona
+0000b570: 6c69 7479 2074 6861 7420 6973 6e27 7420  lity that isn't 
+0000b580: 6578 706f 7365 6420 696e 0a20 2060 6074  exposed in.  ``t
+0000b590: 7261 6974 732e 6170 6960 602c 2061 6e64  raits.api``, and
+0000b5a0: 2079 6f75 2074 6869 6e6b 2069 7420 7368   you think it sh
+0000b5b0: 6f75 6c64 2062 652c 2070 6c65 6173 6520  ould be, please 
+0000b5c0: 6f70 656e 2061 6e20 6973 7375 6520 6f6e  open an issue on
+0000b5d0: 2074 6865 0a20 2054 7261 6974 7320 6275   the.  Traits bu
+0000b5e0: 6720 7472 6163 6b65 722e 0a0a 4665 6174  g tracker...Feat
+0000b5f0: 7572 6573 0a7e 7e7e 7e7e 7e7e 7e0a 0a2a  ures.~~~~~~~~..*
+0000b600: 2041 6464 206e 6577 2060 6044 6174 6574   Add new ``Datet
+0000b610: 696d 6560 6020 7472 6169 7420 7479 7065  ime`` trait type
+0000b620: 2e20 2823 3733 372c 2023 3831 342c 2023  . (#737, #814, #
+0000b630: 3831 332c 2023 3831 352c 2023 3834 3829  813, #815, #848)
+0000b640: 0a2a 2053 7570 706f 7274 2050 7974 686f  .* Support Pytho
+0000b650: 6e20 456e 756d 7320 6173 2076 616c 7565  n Enums as value
+0000b660: 2073 6574 7320 666f 7220 7468 6520 6060   sets for the ``
+0000b670: 456e 756d 6060 2074 7261 6974 2e20 2823  Enum`` trait. (#
+0000b680: 3638 352c 2023 3832 382c 2023 3835 3529  685, #828, #855)
+0000b690: 0a2a 2041 6464 2060 6053 7562 636c 6173  .* Add ``Subclas
+0000b6a0: 7360 6020 616c 6961 7320 666f 7220 7468  s`` alias for th
+0000b6b0: 6520 6060 5479 7065 6060 2074 7261 6974  e ``Type`` trait
+0000b6c0: 2074 7970 652e 2028 2337 3339 290a 2a20   type. (#739).* 
+0000b6d0: 4164 6420 7061 7468 2d6c 696b 6520 7375  Add path-like su
+0000b6e0: 7070 6f72 7420 666f 7220 7468 6520 6060  pport for the ``
+0000b6f0: 4669 6c65 6060 2074 7261 6974 2e20 2823  File`` trait. (#
+0000b700: 3733 3629 0a2a 2041 6464 206e 6577 2060  736).* Add new `
+0000b710: 6043 6f6d 7061 7269 736f 6e4d 6f64 6560  `ComparisonMode`
+0000b720: 6020 656e 756d 6572 6174 696f 6e20 7479  ` enumeration ty
+0000b730: 7065 2074 6f20 7265 706c 6163 6520 7468  pe to replace th
+0000b740: 6520 6f6c 640a 2020 6060 4e4f 5f43 4f4d  e old.  ``NO_COM
+0000b750: 5041 5245 6060 2c20 6060 4f42 4a45 4354  PARE``, ``OBJECT
+0000b760: 5f49 4445 4e54 4954 595f 434f 4d50 4152  _IDENTITY_COMPAR
+0000b770: 4560 6020 616e 6420 6060 5249 4348 5f43  E`` and ``RICH_C
+0000b780: 4f4d 5041 5245 6060 0a20 2063 6f6e 7374  OMPARE``.  const
+0000b790: 616e 7473 2e20 5468 6520 6f6c 6420 636f  ants. The old co
+0000b7a0: 6e73 7461 6e74 7320 6172 6520 6465 7072  nstants are depr
+0000b7b0: 6563 6174 6564 2e20 2823 3833 302c 2023  ecated. (#830, #
+0000b7c0: 3731 392c 2023 3638 3029 0a2a 2041 6464  719, #680).* Add
+0000b7d0: 2066 6173 7420 7661 6c69 6461 7469 6f6e   fast validation
+0000b7e0: 2066 6f72 2060 6043 616c 6c61 626c 6560   for ``Callable`
+0000b7f0: 6020 7472 6169 7420 7479 7065 3b20 696e  ` trait type; in
+0000b800: 7472 6f64 7563 650a 2020 6e65 7720 6060  troduce.  new ``
+0000b810: 4261 7365 4361 6c6c 6162 6c65 6060 2074  BaseCallable`` t
+0000b820: 7261 6974 2074 7970 6520 666f 7220 7375  rait type for su
+0000b830: 6263 6c61 7373 696e 6720 7075 7270 6f73  bclassing purpos
+0000b840: 6573 2e0a 2020 2823 3739 382c 2023 3739  es..  (#798, #79
+0000b850: 352c 2023 3736 3729 0a2a 2041 6464 2060  5, #767).* Add `
+0000b860: 6043 5472 6169 742e 636f 6d70 6172 6973  `CTrait.comparis
+0000b870: 6f6e 5f6d 6f64 6560 6020 7072 6f70 6572  on_mode`` proper
+0000b880: 7479 2074 6f20 616c 6c6f 7720 696e 7370  ty to allow insp
+0000b890: 6563 7469 6f6e 2061 6e64 0a20 206d 6f64  ection and.  mod
+0000b8a0: 6966 6963 6174 696f 6e20 6f66 2061 2074  ification of a t
+0000b8b0: 7261 6974 2773 2063 6f6d 7061 7269 736f  rait's compariso
+0000b8c0: 6e20 6d6f 6465 2e20 2823 3735 382c 2023  n mode. (#758, #
+0000b8d0: 3733 3529 0a2a 2041 6464 2060 6061 735f  735).* Add ``as_
+0000b8e0: 6374 7261 6974 6060 2063 6f6e 7665 7274  ctrait`` convert
+0000b8f0: 6572 2066 756e 6374 696f 6e20 746f 2060  er function to `
+0000b900: 6074 7261 6974 732e 6170 6960 602e 2054  `traits.api``. T
+0000b910: 6869 7320 6675 6e63 7469 6f6e 0a20 2063  his function.  c
+0000b920: 6f6e 7665 7274 7320 6120 7472 6169 742d  onverts a trait-
+0000b930: 6c69 6b65 206f 626a 6563 7420 6f72 2074  like object or t
+0000b940: 7970 6520 746f 2061 2060 6043 5472 6169  ype to a ``CTrai
+0000b950: 7460 602c 2072 6169 7369 6e67 2060 6054  t``, raising ``T
+0000b960: 7970 6545 7272 6f72 6060 0a20 2066 6f72  ypeError``.  for
+0000b970: 206f 626a 6563 7473 2074 6861 7420 6361   objects that ca
+0000b980: 6e27 7420 6265 2069 6e74 6572 7072 6574  n't be interpret
+0000b990: 6564 2061 7320 6120 6060 4354 7261 6974  ed as a ``CTrait
+0000b9a0: 6060 2e20 4974 2773 2069 6e74 656e 6465  ``. It's intende
+0000b9b0: 640a 2020 666f 7220 7573 6520 6279 2075  d.  for use by u
+0000b9c0: 7365 7273 2077 686f 2077 616e 7420 746f  sers who want to
+0000b9d0: 2063 7265 6174 6520 7468 6569 7220 6f77   create their ow
+0000b9e0: 6e20 7061 7261 6d65 7465 7269 7365 6420  n parameterised 
+0000b9f0: 7472 6169 740a 2020 7479 7065 732e 0a0a  trait.  types...
+0000ba00: 2020 5468 6520 6060 6173 5f63 7472 6169    The ``as_ctrai
+0000ba10: 7460 6020 6665 6174 7572 6520 636f 6d65  t`` feature come
+0000ba20: 7320 7769 7468 2c20 616e 6420 7265 6c69  s with, and reli
+0000ba30: 6573 2075 706f 6e2c 2061 206e 6577 2069  es upon, a new i
+0000ba40: 6e66 6f72 6d61 6c0a 2020 696e 7465 7266  nformal.  interf
+0000ba50: 6163 653a 206f 626a 6563 7473 2074 6861  ace: objects tha
+0000ba60: 7420 6361 6e20 6265 2063 6f6e 7665 7274  t can be convert
+0000ba70: 6564 2074 6f20 736f 6d65 7468 696e 6720  ed to something 
+0000ba80: 6f66 2074 7970 6520 6060 4354 7261 6974  of type ``CTrait
+0000ba90: 6060 2063 616e 0a20 2070 726f 7669 6465  `` can.  provide
+0000baa0: 2061 6e20 7a65 726f 2d61 7267 756d 656e   an zero-argumen
+0000bab0: 7420 6060 6173 5f63 7472 6169 7460 6020  t ``as_ctrait`` 
+0000bac0: 6d65 7468 6f64 2074 6861 7420 7265 7475  method that retu
+0000bad0: 726e 7320 6120 6e65 7720 6060 4354 7261  rns a new ``CTra
+0000bae0: 6974 6060 2e0a 2020 5479 7065 7320 6361  it``..  Types ca
+0000baf0: 6e20 7072 6f76 6964 6520 616e 2060 6069  n provide an ``i
+0000bb00: 6e73 7461 6e74 6961 7465 5f61 6e64 5f67  nstantiate_and_g
+0000bb10: 6574 5f63 7472 6169 7460 6020 6d65 7468  et_ctrait`` meth
+0000bb20: 6f64 2c20 7768 6963 6820 7768 656e 0a20  od, which when. 
+0000bb30: 2063 616c 6c65 6420 7769 7468 206e 6f20   called with no 
+0000bb40: 6172 6775 6d65 6e74 7320 7072 6f76 6964  arguments provid
+0000bb50: 6573 2061 206e 6577 2060 6043 5472 6169  es a new ``CTrai
+0000bb60: 7460 6020 666f 7220 7468 6174 2074 7970  t`` for that typ
+0000bb70: 652e 0a20 2028 2337 3833 2c20 2337 3934  e..  (#783, #794
+0000bb80: 290a 2a20 4164 6420 6120 6e65 7720 6060  ).* Add a new ``
+0000bb90: 4861 7354 7261 6974 732e 5f63 6c61 7373  HasTraits._class
+0000bba0: 5f74 7261 6974 7360 6020 6d65 7468 6f64  _traits`` method
+0000bbb0: 2066 6f72 2069 6e74 726f 7370 6563 7469   for introspecti
+0000bbc0: 6f6e 206f 6620 616e 0a20 206f 626a 6563  on of an.  objec
+0000bbd0: 7427 7320 636c 6173 7320 7472 6169 7473  t's class traits
+0000bbe0: 2e20 5468 6973 2070 6172 616c 6c65 6c73  . This parallels
+0000bbf0: 2074 6865 2065 7869 7374 696e 670a 2020   the existing.  
+0000bc00: 6060 4861 7354 7261 6974 732e 5f69 6e73  ``HasTraits._ins
+0000bc10: 7461 6e63 655f 7472 6169 7473 6060 206d  tance_traits`` m
+0000bc20: 6574 686f 642e 2054 6869 7320 6d65 7468  ethod. This meth
+0000bc30: 6f64 2069 7320 696e 7465 6e64 6564 2066  od is intended f
+0000bc40: 6f72 2075 7365 2069 6e0a 2020 6465 6275  or use in.  debu
+0000bc50: 6767 696e 672e 2049 7427 7320 6e6f 7420  gging. It's not 
+0000bc60: 7265 636f 6d6d 656e 6465 6420 666f 7220  recommended for 
+0000bc70: 7573 6572 7320 746f 206d 6f64 6966 7920  users to modify 
+0000bc80: 7468 6520 7265 7475 726e 6564 2064 6963  the returned dic
+0000bc90: 7469 6f6e 6172 792e 0a20 2028 2337 3032  tionary..  (#702
+0000bca0: 290a 2a20 4164 6420 6060 4354 7261 6974  ).* Add ``CTrait
+0000bcb0: 2e73 6574 5f64 6566 6175 6c74 5f76 616c  .set_default_val
+0000bcc0: 7565 6060 206d 6574 686f 6420 666f 7220  ue`` method for 
+0000bcd0: 7365 7474 696e 6720 696e 666f 726d 6174  setting informat
+0000bce0: 696f 6e20 6162 6f75 7420 7468 650a 2020  ion about the.  
+0000bcf0: 6465 6661 756c 7420 6f66 2061 2060 6043  default of a ``C
+0000bd00: 5472 6169 7460 602e 2054 6869 7320 7072  Trait``. This pr
+0000bd10: 6f76 6964 6573 2061 6e20 616c 7465 726e  ovides an altern
+0000bd20: 6174 6976 6520 746f 2074 6865 2070 7265  ative to the pre
+0000bd30: 7669 6f75 7320 6d65 7468 6f64 0a20 206f  vious method.  o
+0000bd40: 6620 7573 696e 6720 6060 4354 7261 6974  f using ``CTrait
+0000bd50: 2e64 6566 6175 6c74 5f76 616c 7565 6060  .default_value``
+0000bd60: 2e20 5468 6520 7573 6520 6f66 2060 6043  . The use of ``C
+0000bd70: 5472 6169 742e 6465 6661 756c 745f 7661  Trait.default_va
+0000bd80: 6c75 6560 6020 746f 2073 6574 0a20 2028  lue`` to set.  (
+0000bd90: 7261 7468 6572 2074 6861 6e20 6765 7429  rather than get)
+0000bda0: 2064 6566 6175 6c74 2069 6e66 6f72 6d61   default informa
+0000bdb0: 7469 6f6e 2069 7320 6465 7072 6563 6174  tion is deprecat
+0000bdc0: 6564 2e20 2823 3632 3029 0a2a 2041 6464  ed. (#620).* Add
+0000bdd0: 206e 6577 206d 6574 686f 6473 2060 6048   new methods ``H
+0000bde0: 6173 5472 6169 7473 2e5f 7472 6169 745f  asTraits._trait_
+0000bdf0: 6e6f 7469 6669 6361 7469 6f6e 735f 656e  notifications_en
+0000be00: 6162 6c65 6460 602c 0a20 2060 6048 6173  abled``,.  ``Has
+0000be10: 5472 6169 7473 2e5f 7472 6169 745f 6e6f  Traits._trait_no
+0000be20: 7469 6669 6361 7469 6f6e 735f 7665 746f  tifications_veto
+0000be30: 6564 6060 2074 6f20 616c 6c6f 7720 696e  ed`` to allow in
+0000be40: 7472 6f73 7065 6374 696f 6e20 6f66 2074  trospection of t
+0000be50: 6865 0a20 206e 6f74 6966 6963 6174 696f  he.  notificatio
+0000be60: 6e73 2073 7461 7465 7320 7365 7420 6279  ns states set by
+0000be70: 2074 6865 2065 7869 7374 696e 6720 6d65   the existing me
+0000be80: 7468 6f64 730a 2020 6060 4861 7354 7261  thods.  ``HasTra
+0000be90: 6974 732e 5f74 7261 6974 5f63 6861 6e67  its._trait_chang
+0000bea0: 655f 6e6f 7469 6679 6060 2061 6e64 2060  e_notify`` and `
+0000beb0: 6048 6173 5472 6169 7473 2e5f 7472 6169  `HasTraits._trai
+0000bec0: 745f 7665 746f 5f6e 6f74 6966 7960 602e  t_veto_notify``.
+0000bed0: 0a20 2028 2337 3034 290a 2a20 4164 6420  .  (#704).* Add 
+0000bee0: 6060 5472 6169 744b 696e 6460 602c 2060  ``TraitKind``, `
+0000bef0: 6056 616c 6964 6174 6554 7261 6974 6060  `ValidateTrait``
+0000bf00: 2061 6e64 2060 6044 6566 6175 6c74 5661   and ``DefaultVa
+0000bf10: 6c75 6560 6020 5079 7468 6f6e 2065 6e75  lue`` Python enu
+0000bf20: 6d65 7261 7469 6f6e 0a20 2074 7970 6573  meration.  types
+0000bf30: 2074 6f20 7265 706c 6163 6520 7072 6576   to replace prev
+0000bf40: 696f 7573 2075 7365 7320 6f66 206d 6167  ious uses of mag
+0000bf50: 6963 2069 6e74 6567 6572 7320 7769 7468  ic integers with
+0000bf60: 696e 2074 6865 2054 7261 6974 7320 636f  in the Traits co
+0000bf70: 6465 6261 7365 2e0a 2020 2823 3638 302c  debase..  (#680,
+0000bf80: 2023 3835 3729 0a2a 2054 6865 2076 6172   #857).* The var
+0000bf90: 696f 7573 2060 6043 5472 6169 7460 6020  ious ``CTrait`` 
+0000bfa0: 696e 7465 726e 616c 2066 6c61 6773 2061  internal flags a
+0000bfb0: 7265 206e 6f77 2065 7870 6f73 6564 2074  re now exposed t
+0000bfc0: 6f20 5079 7468 6f6e 2061 730a 2020 7072  o Python as.  pr
+0000bfd0: 6f70 6572 7469 6573 3a20 6060 4354 7261  operties: ``CTra
+0000bfe0: 6974 2e69 735f 7072 6f70 6572 7479 6060  it.is_property``
+0000bff0: 2028 7265 6164 2d6f 6e6c 7929 2c20 6060   (read-only), ``
+0000c000: 4354 7261 6974 2e6d 6f64 6966 795f 6465  CTrait.modify_de
+0000c010: 6c65 6761 7465 6060 2c0a 2020 6060 4354  legate``,.  ``CT
+0000c020: 7261 6974 2e73 6574 6174 7472 5f6f 7269  rait.setattr_ori
+0000c030: 6769 6e61 6c5f 7661 6c75 6560 602c 2060  ginal_value``, `
+0000c040: 6043 5472 6169 742e 706f 7374 5f73 6574  `CTrait.post_set
+0000c050: 6174 7472 5f6f 7269 6769 6e61 6c5f 7661  attr_original_va
+0000c060: 6c75 6560 602c 0a20 2060 6043 5472 6169  lue``,.  ``CTrai
+0000c070: 742e 6973 5f6d 6170 7065 6460 602c 2061  t.is_mapped``, a
+0000c080: 6e64 2060 6043 5472 6169 742e 636f 6d70  nd ``CTrait.comp
+0000c090: 6172 6973 6f6e 5f6d 6f64 6560 602e 2028  arison_mode``. (
+0000c0a0: 2336 3636 2c20 2336 3933 290a 0a43 6861  #666, #693)..Cha
+0000c0b0: 6e67 6573 0a7e 7e7e 7e7e 7e7e 0a0a 2a20  nges.~~~~~~~..* 
+0000c0c0: 5768 656e 2070 6963 6b6c 696e 6720 6120  When pickling a 
+0000c0d0: 6060 4354 7261 6974 6060 2c20 7468 6520  ``CTrait``, the 
+0000c0e0: 6060 7079 5f70 6f73 745f 7365 7461 7474  ``py_post_setatt
+0000c0f0: 7260 6020 616e 6420 6060 7079 5f76 616c  r`` and ``py_val
+0000c100: 6964 6174 6560 600a 2020 6669 656c 6473  idate``.  fields
+0000c110: 2061 7265 2070 6963 6b6c 6564 2064 6972   are pickled dir
+0000c120: 6563 746c 792e 2050 7265 7669 6f75 736c  ectly. Previousl
+0000c130: 792c 2063 616c 6c61 626c 6573 2066 6f72  y, callables for
+0000c140: 2074 686f 7365 2066 6965 6c64 7320 7765   those fields we
+0000c150: 7265 0a20 2072 6570 6c61 6365 6420 7769  re.  replaced wi
+0000c160: 7468 2061 2060 602d 3160 6020 7365 6e74  th a ``-1`` sent
+0000c170: 696e 656c 206f 6e20 7069 636b 6c69 6e67  inel on pickling
+0000c180: 2e20 2823 3738 3029 0a2a 2041 2060 6054  . (#780).* A ``T
+0000c190: 7261 6974 4c69 7374 4576 656e 7460 6020  raitListEvent`` 
+0000c1a0: 6973 206e 6f20 6c6f 6e67 6572 2065 6d69  is no longer emi
+0000c1b0: 7474 6564 2066 6f72 2061 2073 6c69 6365  tted for a slice
+0000c1c0: 2064 656c 6574 696f 6e20 7768 6963 680a   deletion which.
+0000c1d0: 2020 646f 6573 6e27 7420 6368 616e 6765    doesn't change
+0000c1e0: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
+0000c1f0: 2074 6865 206c 6973 742e 2028 466f 7220   the list. (For 
+0000c200: 6578 616d 706c 652c 2060 6465 6c20 6f62  example, `del ob
+0000c210: 6a2e 6d79 6c69 7374 5b32 3a5d 600a 2020  j.mylist[2:]`.  
+0000c220: 6f6e 2061 206c 6973 7420 7468 6174 206f  on a list that o
+0000c230: 6e6c 7920 6861 7320 3220 656c 656d 656e  nly has 2 elemen
+0000c240: 7473 2e29 2028 2337 3430 290a 2a20 5468  ts.) (#740).* Th
+0000c250: 6520 6060 6164 6465 6460 6020 616e 6420  e ``added`` and 
+0000c260: 6060 7265 6d6f 7665 6460 6020 6174 7472  ``removed`` attr
+0000c270: 6962 7574 6573 206f 6e20 6120 6060 5472  ibutes on a ``Tr
+0000c280: 6169 744c 6973 7445 7665 6e74 6060 2061  aitListEvent`` a
+0000c290: 7265 206e 6f77 0a20 2061 6c77 6179 7320  re now.  always 
+0000c2a0: 6c69 7374 7320 636f 6e74 6169 6e69 6e67  lists containing
+0000c2b0: 2074 6865 2061 6464 6564 206f 7220 7265   the added or re
+0000c2c0: 6d6f 7665 6420 656c 656d 656e 7473 2e20  moved elements. 
+0000c2d0: 5072 6576 696f 7573 6c79 2c20 7468 6f73  Previously, thos
+0000c2e0: 650a 2020 6c69 7374 7320 7765 7265 206e  e.  lists were n
+0000c2f0: 6573 7465 6420 696e 7369 6465 2061 6e6f  ested inside ano
+0000c300: 7468 6572 206c 6973 7420 696e 2073 6f6d  ther list in som
+0000c310: 6520 6361 7365 732e 2028 2337 3731 290a  e cases. (#771).
+0000c320: 2a20 4368 616e 6765 2060 6049 6e73 7461  * Change ``Insta
+0000c330: 6e63 6528 4953 6f6d 6549 6e74 6572 6661  nce(ISomeInterfa
+0000c340: 6365 2960 6020 746f 2075 7365 2061 6e20  ce)`` to use an 
+0000c350: 6060 6973 696e 7374 616e 6365 6060 2063  ``isinstance`` c
+0000c360: 6865 636b 206f 6e0a 2020 7472 6169 7420  heck on.  trait 
+0000c370: 7365 7420 696e 7374 6561 6420 6f66 2075  set instead of u
+0000c380: 7369 6e67 2074 6865 2064 796e 616d 6963  sing the dynamic
+0000c390: 2069 6e74 6572 6661 6365 2063 6865 636b   interface check
+0000c3a0: 6572 2e20 2823 3633 3029 0a2a 2043 7265  er. (#630).* Cre
+0000c3b0: 6174 6520 616e 206e 6577 2060 6041 6273  ate an new ``Abs
+0000c3c0: 7472 6163 7456 6965 7745 6c65 6d65 6e74  tractViewElement
+0000c3d0: 6060 2061 6273 7472 6163 7420 6261 7365  `` abstract base
+0000c3e0: 2063 6c61 7373 2c20 616e 6420 7265 6769   class, and regi
+0000c3f0: 7374 6572 0a20 2074 6865 2054 7261 6974  ster.  the Trait
+0000c400: 7355 4920 6060 5669 6577 456c 656d 656e  sUI ``ViewElemen
+0000c410: 7460 6020 6173 2069 6d70 6c65 6d65 6e74  t`` as implement
+0000c420: 696e 6720 6974 2e20 5468 6973 2070 6176  ing it. This pav
+0000c430: 6573 2074 6865 2077 6179 2066 6f72 0a20  es the way for. 
+0000c440: 2072 656d 6f76 616c 206f 6620 5472 6169   removal of Trai
+0000c450: 7473 2055 4920 696d 706f 7274 7320 6672  ts UI imports fr
+0000c460: 6f6d 2054 7261 6974 732e 2028 2336 3137  om Traits. (#617
+0000c470: 290a 2a20 6060 5669 6577 456c 656d 656e  ).* ``ViewElemen
+0000c480: 7473 6060 2061 7265 206e 6f77 2063 6f6d  ts`` are now com
+0000c490: 7075 7465 6420 6c61 7a69 6c79 2c20 696e  puted lazily, in
+0000c4a0: 7374 6561 6420 6f66 2061 7420 6060 4861  stead of at ``Ha
+0000c4b0: 7354 7261 6974 7360 600a 2020 7375 6263  sTraits``.  subc
+0000c4c0: 6c61 7373 2063 7265 6174 696f 6e20 7469  lass creation ti
+0000c4d0: 6d65 2e20 5468 6973 2072 656d 6f76 6573  me. This removes
+0000c4e0: 2061 2060 6074 7261 6974 7375 6960 6020   a ``traitsui`` 
+0000c4f0: 696d 706f 7274 2066 726f 6d0a 2020 7468  import from.  th
+0000c500: 6520 6060 7472 6169 742e 6861 735f 7472  e ``trait.has_tr
+0000c510: 6169 7473 6060 206d 6f64 756c 652e 2028  aits`` module. (
+0000c520: 2336 3134 290a 2a20 5468 6520 6060 7472  #614).* The ``tr
+0000c530: 6169 7473 2e75 7469 6c2e 636c 6561 6e5f  aits.util.clean_
+0000c540: 6669 6c65 6e61 6d65 6060 2075 7469 6c69  filename`` utili
+0000c550: 7479 206e 6f77 2075 7365 7320 6120 6469  ty now uses a di
+0000c560: 6666 6572 656e 7420 616c 676f 7269 7468  fferent algorith
+0000c570: 6d2c 0a20 2061 6e64 2073 686f 756c 6420  m,.  and should 
+0000c580: 646f 2061 2062 6574 7465 7220 6a6f 6220  do a better job 
+0000c590: 7769 7468 2061 6363 656e 7465 6420 616e  with accented an
+0000c5a0: 6420 556e 6963 6f64 6520 7465 7874 2e20  d Unicode text. 
+0000c5b0: 2823 3538 3929 0a2a 2046 6c6f 6174 696e  (#589).* Floatin
+0000c5c0: 672d 706f 696e 7420 616e 6420 696e 7465  g-point and inte
+0000c5d0: 6765 7220 6368 6563 6b73 2061 7265 206e  ger checks are n
+0000c5e0: 6f77 206d 6f72 6520 636f 6e73 6973 7465  ow more consiste
+0000c5f0: 6e74 2062 6574 7765 656e 2063 6c61 7373  nt between class
+0000c600: 6573 2e0a 2020 496e 2070 6172 7469 6375  es..  In particu
+0000c610: 6c61 722c 2060 6042 6173 6549 6e74 6060  lar, ``BaseInt``
+0000c620: 2076 616c 6964 6174 696f 6e20 6e6f 7720   validation now 
+0000c630: 6d61 7463 6865 7320 6060 496e 7460 6020  matches ``Int`` 
+0000c640: 7661 6c69 6461 7469 6f6e 2c20 616e 640a  validation, and.
+0000c650: 2020 6060 5261 6e67 6560 6020 7479 7065    ``Range`` type
+0000c660: 2063 6865 636b 7320 6e6f 7720 6d61 7463   checks now matc
+0000c670: 6820 7468 6f73 6520 7573 6564 2069 6e20  h those used in 
+0000c680: 6060 496e 7460 6020 616e 6420 6060 466c  ``Int`` and ``Fl
+0000c690: 6f61 7460 602e 2028 2335 3838 290a 2a20  oat``. (#588).* 
+0000c6a0: 416e 2065 7863 6570 7469 6f6e 206f 7468  An exception oth
+0000c6b0: 6572 2074 6861 6e20 6060 5472 6169 7445  er than ``TraitE
+0000c6c0: 7272 6f72 6060 2072 6169 7365 6420 6475  rror`` raised du
+0000c6d0: 7269 6e67 2076 616c 6964 6174 696f 6e20  ring validation 
+0000c6e0: 6f66 2061 0a20 2063 6f6d 706f 756e 6420  of a.  compound 
+0000c6f0: 7472 6169 7420 7769 6c6c 206e 6f77 2062  trait will now b
+0000c700: 6520 7072 6f70 6167 6174 6564 2e20 5072  e propagated. Pr
+0000c710: 6576 696f 7573 6c79 2c20 7468 6174 2065  eviously, that e
+0000c720: 7863 6570 7469 6f6e 2077 6f75 6c64 0a20  xception would. 
+0000c730: 2062 6520 7377 616c 6c6f 7765 642e 2028   be swallowed. (
+0000c740: 2335 3831 290a 2a20 5472 6169 7473 206e  #581).* Traits n
+0000c750: 6f20 6c6f 6e67 6572 2068 6173 2061 2072  o longer has a r
+0000c760: 756e 7469 6d65 2064 6570 656e 6465 6e63  untime dependenc
+0000c770: 7920 6f6e 2074 6865 2060 6073 6978 6060  y on the ``six``
+0000c780: 2070 6163 6b61 6765 2e20 2823 3633 3829   package. (#638)
+0000c790: 0a2a 2055 7365 2070 6963 6b6c 6520 7072  .* Use pickle pr
+0000c7a0: 6f74 6f63 6f6c 2033 2069 6e73 7465 6164  otocol 3 instead
+0000c7b0: 206f 6620 7069 636b 6c65 2070 726f 746f   of pickle proto
+0000c7c0: 636f 6c20 3120 7768 656e 2077 7269 7469  col 1 when writi
+0000c7d0: 6e67 2070 6963 6b6c 6564 0a20 206f 626a  ng pickled.  obj
+0000c7e0: 6563 7420 7374 6174 6520 746f 2061 2066  ect state to a f
+0000c7f0: 696c 6520 696e 2060 6063 6f6e 6669 6775  ile in ``configu
+0000c800: 7265 5f74 7261 6974 7360 602e 2028 2337  re_traits``. (#7
+0000c810: 3936 290a 2a20 496e 2060 6074 7261 6974  96).* In ``trait
+0000c820: 732e 7465 7374 696e 672e 6f70 7469 6f6e  s.testing.option
+0000c830: 616c 5f64 6570 656e 6465 6e63 6965 7360  al_dependencies`
+0000c840: 602c 206d 616b 6520 7375 7265 2060 6074  `, make sure ``t
+0000c850: 7261 6974 7375 692e 6170 6960 6020 6973  raitsui.api`` is
+0000c860: 0a20 2061 7661 696c 6162 6c65 2077 6865  .  available whe
+0000c870: 6e65 7665 7220 6060 7472 6169 7473 7569  never ``traitsui
+0000c880: 6060 2069 732e 2028 2336 3136 290a 2a20  `` is. (#616).* 
+0000c890: 6060 5472 6169 7449 6e73 7461 6e63 6560  ``TraitInstance`
+0000c8a0: 6020 6e6f 7720 696e 6865 7269 7473 2064  ` now inherits d
+0000c8b0: 6972 6563 746c 7920 6672 6f6d 2060 6054  irectly from ``T
+0000c8c0: 7261 6974 4861 6e64 6c65 7260 6020 696e  raitHandler`` in
+0000c8d0: 7374 6561 6420 6f66 0a20 2028 7468 6520  stead of.  (the 
+0000c8e0: 6e6f 7720 7265 6d6f 7665 6429 2060 6054  now removed) ``T
+0000c8f0: 6869 7343 6c61 7373 6060 2e20 2823 3736  hisClass``. (#76
+0000c900: 3129 0a0a 4669 7865 730a 7e7e 7e7e 7e0a  1)..Fixes.~~~~~.
+0000c910: 0a2a 2046 6978 2061 2075 7365 206f 6620  .* Fix a use of 
+0000c920: 7468 6520 756e 7375 7070 6f72 7465 6420  the unsupported 
+0000c930: 6060 5661 6c69 6461 7465 5472 6169 742e  ``ValidateTrait.
+0000c940: 696e 745f 7261 6e67 6560 602e 2028 2338  int_range``. (#8
+0000c950: 3035 290a 2a20 5265 6d6f 7665 2075 6e6e  05).* Remove unn
+0000c960: 6563 6573 7361 7279 2060 6063 6f70 7960  ecessary ``copy`
+0000c970: 6020 6d65 7468 6f64 206f 7665 7272 6964  ` method overrid
+0000c980: 6520 6672 6f6d 2060 6054 7261 6974 5365  e from ``TraitSe
+0000c990: 744f 626a 6563 7460 602e 2028 2337 3539  tObject``. (#759
+0000c9a0: 290a 2a20 4669 7820 6060 5472 6169 744c  ).* Fix ``TraitL
+0000c9b0: 6973 744f 626a 6563 742e 636c 6561 7260  istObject.clear`
+0000c9c0: 6020 746f 2069 7373 7565 2074 6865 2061  ` to issue the a
+0000c9d0: 7070 726f 7072 6961 7465 2069 7465 6d73  ppropriate items
+0000c9e0: 2065 7665 6e74 2e20 2823 3733 3229 0a2a   event. (#732).*
+0000c9f0: 2046 6978 2063 6f6e 6675 7369 6e67 2065   Fix confusing e
+0000ca00: 7272 6f72 206d 6573 7361 6765 2077 6865  rror message whe
+0000ca10: 6e20 6060 5b4e 6f6e 655d 6060 2070 6173  n ``[None]`` pas
+0000ca20: 7365 6420 696e 746f 0a20 2060 604c 6973  sed into.  ``Lis
+0000ca30: 7428 5468 6973 2861 6c6c 6f77 5f6e 6f6e  t(This(allow_non
+0000ca40: 653d 4661 6c73 6529 2960 602e 2028 2337  e=False))``. (#7
+0000ca50: 3334 290a 2a20 4669 7820 6e61 6d65 2d6d  34).* Fix name-m
+0000ca60: 616e 676c 696e 6720 6f66 2064 6f75 626c  angling of doubl
+0000ca70: 652d 756e 6465 7273 636f 7265 2070 7269  e-underscore pri
+0000ca80: 7661 7465 206d 6574 686f 6473 2069 6e20  vate methods in 
+0000ca90: 636c 6173 7365 7320 7768 6f73 650a 2020  classes whose.  
+0000caa0: 6e61 6d65 2062 6567 696e 7320 7769 7468  name begins with
+0000cab0: 2061 6e20 756e 6465 7273 636f 7265 2e20   an underscore. 
+0000cac0: 2823 3732 3429 0a2a 2046 6978 2060 6062  (#724).* Fix ``b
+0000cad0: 7974 6573 5f65 6469 746f 7260 6020 616e  ytes_editor`` an
+0000cae0: 6420 6060 7061 7373 776f 7264 5f65 6469  d ``password_edi
+0000caf0: 746f 7260 6020 6275 6773 2c20 616e 6420  tor`` bugs, and 
+0000cb00: 6164 6420 7465 7374 7320 666f 720a 2020  add tests for.  
+0000cb10: 616c 6c20 6564 6974 6f72 2066 6163 746f  all editor facto
+0000cb20: 7269 6573 2e20 2823 3636 3029 0a2a 2046  ries. (#660).* F
+0000cb30: 6978 2063 6f65 7263 696f 6e20 6661 7374  ix coercion fast
+0000cb40: 2076 616c 6964 6174 696f 6e20 7479 7065   validation type
+0000cb50: 2074 6f20 646f 2061 6e20 6578 6163 7420   to do an exact 
+0000cb60: 7479 7065 2063 6865 636b 2069 6e73 7465  type check inste
+0000cb70: 6164 206f 660a 2020 616e 2069 6e73 7461  ad of.  an insta
+0000cb80: 6e63 6520 6368 6563 6b2e 2054 6869 7320  nce check. This 
+0000cb90: 656e 7375 7265 7320 7468 6174 2069 6e73  ensures that ins
+0000cba0: 7461 6e63 6573 206f 6620 7375 6263 6c61  tances of subcla
+0000cbb0: 7373 6573 206f 6620 7468 650a 2020 7461  sses of the.  ta
+0000cbc0: 7267 6574 2074 7970 6520 6172 6520 7072  rget type are pr
+0000cbd0: 6f70 6572 6c79 2063 6f6e 7665 7274 6564  operly converted
+0000cbe0: 2074 6f20 7468 6520 7461 7267 6574 2074   to the target t
+0000cbf0: 7970 652e 2046 6f72 2065 7861 6d70 6c65  ype. For example
+0000cc00: 2c0a 2020 6966 2060 6054 7275 6560 6020  ,.  if ``True`` 
+0000cc10: 6973 2061 7373 6967 6e65 6420 746f 2061  is assigned to a
+0000cc20: 2074 7261 6974 206f 6620 7479 7065 2060   trait of type `
+0000cc30: 6043 496e 7460 602c 2074 6865 2072 6573  `CInt``, the res
+0000cc40: 756c 7469 6e67 0a20 2076 616c 7565 2069  ulting.  value i
+0000cc50: 7320 6e6f 7720 6060 3160 602e 2050 7265  s now ``1``. Pre
+0000cc60: 7669 6f75 736c 792c 2069 7420 7761 7320  viously, it was 
+0000cc70: 6060 5472 7565 6060 2e20 2823 3634 3729  ``True``. (#647)
+0000cc80: 0a2a 2046 6978 2060 6042 6173 6552 616e  .* Fix ``BaseRan
+0000cc90: 6765 6060 2074 6f20 6163 6365 7074 2074  ge`` to accept t
+0000cca0: 6865 2073 616d 6520 7661 6c75 6573 2061  he same values a
+0000ccb0: 7320 6060 5261 6e67 6560 602e 2028 2335  s ``Range``. (#5
+0000ccc0: 3833 290a 2a20 4669 7820 696e 7465 6765  83).* Fix intege
+0000ccd0: 7220 6060 5261 6e67 6560 6020 746f 2061  r ``Range`` to a
+0000cce0: 6363 6570 7420 696e 7465 6765 722d 6c69  ccept integer-li
+0000ccf0: 6b65 206f 626a 6563 7473 2e20 2823 3538  ke objects. (#58
+0000cd00: 3229 0a2a 2046 6978 2066 6c6f 6174 696e  2).* Fix floatin
+0000cd10: 672d 706f 696e 7420 6060 5261 6e67 6560  g-point ``Range`
+0000cd20: 6020 746f 2061 6363 6570 7420 666c 6f61  ` to accept floa
+0000cd30: 742d 6c69 6b65 2076 616c 7565 732e 2028  t-like values. (
+0000cd40: 2335 3739 290a 2a20 4669 7820 6120 6d69  #579).* Fix a mi
+0000cd50: 7373 696e 6720 696d 706f 7274 2069 6e20  ssing import in 
+0000cd60: 7468 6520 6164 6170 7461 7469 6f6e 2062  the adaptation b
+0000cd70: 656e 6368 6d61 726b 2073 6372 6970 742e  enchmark script.
+0000cd80: 2028 2335 3735 290a 2a20 4669 7820 6973   (#575).* Fix is
+0000cd90: 7375 6573 2077 6974 6820 7468 6520 6060  sues with the ``
+0000cda0: 6669 6c65 6e61 6d65 6060 2061 7267 756d  filename`` argum
+0000cdb0: 656e 7420 746f 2060 6063 6f6e 6669 6775  ent to ``configu
+0000cdc0: 7265 5f74 7261 6974 7360 602e 2028 2335  re_traits``. (#5
+0000cdd0: 3732 290a 2a20 4669 7820 6120 706f 7373  72).* Fix a poss
+0000cde0: 6962 6c65 2073 6567 6661 756c 7420 6672  ible segfault fr
+0000cdf0: 6f6d 2063 6172 656c 6573 7320 6669 656c  om careless fiel
+0000ce00: 6420 7265 2d61 7373 6967 6e6d 656e 7473  d re-assignments
+0000ce10: 2069 6e0a 2020 6060 6374 7261 6974 732e   in.  ``ctraits.
+0000ce20: 6360 602e 2028 2338 3434 290a 0a44 6570  c``. (#844)..Dep
+0000ce30: 7265 6361 7469 6f6e 730a 7e7e 7e7e 7e7e  recations.~~~~~~
+0000ce40: 7e7e 7e7e 7e7e 0a0a 2a20 5468 6520 6060  ~~~~~~..* The ``
+0000ce50: 4e4f 5f43 4f4d 5041 5245 6060 2c20 6060  NO_COMPARE``, ``
+0000ce60: 4f42 4a45 4354 5f49 4445 4e54 4954 595f  OBJECT_IDENTITY_
+0000ce70: 434f 4d50 4152 4560 6020 616e 6420 6060  COMPARE`` and ``
+0000ce80: 5249 4348 5f43 4f4d 5041 5245 6060 0a20  RICH_COMPARE``. 
+0000ce90: 2063 6f6e 7374 616e 7473 2061 7265 2064   constants are d
+0000cea0: 6570 7265 6361 7465 642e 2055 7365 2074  eprecated. Use t
+0000ceb0: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
+0000cec0: 206d 656d 6265 7273 206f 6620 7468 650a   members of the.
+0000ced0: 2020 6060 436f 6d70 6172 6973 6f6e 4d6f    ``ComparisonMo
+0000cee0: 6465 6060 2065 6e75 6d65 7261 7469 6f6e  de`` enumeration
+0000cef0: 2069 6e73 7465 6164 2e20 2823 3731 3929   instead. (#719)
+0000cf00: 0a2a 2054 6865 2060 6055 6e69 636f 6465  .* The ``Unicode
+0000cf10: 6060 2c20 6060 4355 6e69 636f 6465 6060  ``, ``CUnicode``
+0000cf20: 2c20 6060 4261 7365 556e 6963 6f64 6560  , ``BaseUnicode`
+0000cf30: 6020 616e 6420 6060 4261 7365 4355 6e69  ` and ``BaseCUni
+0000cf40: 636f 6465 6060 2074 7261 6974 0a20 2074  code`` trait.  t
+0000cf50: 7970 6573 2061 7265 2064 6570 7265 6361  ypes are depreca
+0000cf60: 7465 642e 2055 7365 2060 6053 7472 6060  ted. Use ``Str``
+0000cf70: 2c20 6060 4353 7472 6060 2c20 6060 4261  , ``CStr``, ``Ba
+0000cf80: 7365 5374 7260 6020 616e 6420 6060 4261  seStr`` and ``Ba
+0000cf90: 7365 4353 7472 6060 0a20 2069 6e73 7465  seCStr``.  inste
+0000cfa0: 6164 2e20 2823 3634 3829 0a2a 2054 6865  ad. (#648).* The
+0000cfb0: 2060 604c 6f6e 6760 602c 2060 6043 4c6f   ``Long``, ``CLo
+0000cfc0: 6e67 6060 2c20 6060 4261 7365 4c6f 6e67  ng``, ``BaseLong
+0000cfd0: 6060 2061 6e64 2060 6042 6173 6543 4c6f  `` and ``BaseCLo
+0000cfe0: 6e67 6060 2074 7261 6974 2074 7970 6573  ng`` trait types
+0000cff0: 2061 7265 0a20 2064 6570 7265 6361 7465   are.  deprecate
+0000d000: 642e 2055 7365 2060 6049 6e74 6060 2c20  d. Use ``Int``, 
+0000d010: 6060 4349 6e74 6060 2c20 6060 4261 7365  ``CInt``, ``Base
+0000d020: 496e 7460 6020 616e 6420 6060 4261 7365  Int`` and ``Base
+0000d030: 4349 6e74 6060 2069 6e73 7465 6164 2e0a  CInt`` instead..
+0000d040: 2020 2823 3634 352c 2023 3537 3329 0a2a    (#645, #573).*
+0000d050: 2054 6865 2060 6041 6461 7074 6564 546f   The ``AdaptedTo
+0000d060: 6060 2074 7261 6974 2074 7970 6520 6973  `` trait type is
+0000d070: 2064 6570 7265 6361 7465 642e 2055 7365   deprecated. Use
+0000d080: 2060 6053 7570 706f 7274 7360 6020 696e   ``Supports`` in
+0000d090: 7374 6561 642e 2028 2337 3630 290a 2a20  stead. (#760).* 
+0000d0a0: 5468 6520 666f 6c6c 6f77 696e 6720 7472  The following tr
+0000d0b0: 6169 7420 7479 7065 2061 6c69 6173 6573  ait type aliases
+0000d0c0: 2061 7265 2064 6570 7265 6361 7465 642e   are deprecated.
+0000d0d0: 2053 6565 2074 6865 2064 6f63 756d 656e   See the documen
+0000d0e0: 7461 7469 6f6e 2066 6f72 0a20 2072 6563  tation for.  rec
+0000d0f0: 6f6d 6d65 6e64 6564 2072 6570 6c61 636d  ommended replacm
+0000d100: 656e 7473 2e20 6060 6661 6c73 6560 602c  ents. ``false``,
+0000d110: 2060 6074 7275 6560 602c 2060 6075 6e64   ``true``, ``und
+0000d120: 6566 696e 6564 6060 2c20 6060 4c69 7374  efined``, ``List
+0000d130: 496e 7460 602c 0a20 2060 604c 6973 7446  Int``,.  ``ListF
+0000d140: 6c6f 6174 6060 2c20 6060 4c69 7374 5374  loat``, ``ListSt
+0000d150: 7260 602c 2060 604c 6973 7455 6e69 636f  r``, ``ListUnico
+0000d160: 6465 6060 2c20 6060 4c69 7374 436f 6d70  de``, ``ListComp
+0000d170: 6c65 7860 602c 2060 604c 6973 7442 6f6f  lex``, ``ListBoo
+0000d180: 6c60 602c 0a20 2060 604c 6973 7446 756e  l``,.  ``ListFun
+0000d190: 6374 696f 6e60 602c 2060 604c 6973 744d  ction``, ``ListM
+0000d1a0: 6574 686f 6460 602c 2060 604c 6973 7454  ethod``, ``ListT
+0000d1b0: 6869 7360 602c 2060 6044 6963 7453 7472  his``, ``DictStr
+0000d1c0: 416e 7960 602c 0a20 2060 6044 6963 7453  Any``,.  ``DictS
+0000d1d0: 7472 5374 7260 602c 2060 6044 6963 7453  trStr``, ``DictS
+0000d1e0: 7472 496e 7460 602c 2060 6044 6963 7453  trInt``, ``DictS
+0000d1f0: 7472 466c 6f61 7460 602c 2060 6044 6963  trFloat``, ``Dic
+0000d200: 7453 7472 426f 6f6c 6060 2c0a 2020 6060  tStrBool``,.  ``
+0000d210: 4469 6374 5374 724c 6973 7460 602e 2028  DictStrList``. (
+0000d220: 2336 3237 290a 2a20 5573 6520 6f66 2074  #627).* Use of t
+0000d230: 6865 2060 6066 696c 656e 616d 6560 6020  he ``filename`` 
+0000d240: 6172 6775 6d65 6e74 2074 6f20 6060 636f  argument to ``co
+0000d250: 6e66 6967 7572 655f 7472 6169 7473 6060  nfigure_traits``
+0000d260: 2028 666f 7220 7374 6f72 696e 670a 2020   (for storing.  
+0000d270: 7374 6174 6520 746f 206f 7220 7265 7374  state to or rest
+0000d280: 6f72 696e 6720 7374 6174 6520 6672 6f6d  oring state from
+0000d290: 2070 6963 6b6c 6520 6669 6c65 7329 2069   pickle files) i
+0000d2a0: 7320 6465 7072 6563 6174 6564 2e20 2823  s deprecated. (#
+0000d2b0: 3739 3229 0a2a 2054 6865 2060 6054 7261  792).* The ``Tra
+0000d2c0: 6974 5475 706c 6560 602c 2060 6054 7261  itTuple``, ``Tra
+0000d2d0: 6974 4c69 7374 6060 2061 6e64 2060 6054  itList`` and ``T
+0000d2e0: 7261 6974 4469 6374 6060 2074 7261 6974  raitDict`` trait
+0000d2f0: 2068 616e 646c 6572 730a 2020 6172 6520   handlers.  are 
+0000d300: 6465 7072 6563 6174 6564 2e20 5573 6520  deprecated. Use 
+0000d310: 7468 6520 6060 5475 706c 6560 602c 2060  the ``Tuple``, `
+0000d320: 604c 6973 7460 6020 616e 6420 6060 4469  `List`` and ``Di
+0000d330: 6374 6060 2074 7261 6974 2074 7970 6573  ct`` trait types
+0000d340: 2069 6e73 7465 6164 2e0a 2020 2823 3737   instead..  (#77
+0000d350: 3029 0a2a 2055 7365 206f 6620 6060 4354  0).* Use of ``CT
+0000d360: 7261 6974 2e64 6566 6175 6c74 5f76 616c  rait.default_val
+0000d370: 7565 6060 2066 6f72 2073 6574 7469 6e67  ue`` for setting
+0000d380: 2064 6566 6175 6c74 2076 616c 7565 2069   default value i
+0000d390: 6e66 6f72 6d61 7469 6f6e 2069 730a 2020  nformation is.  
+0000d3a0: 6465 7072 6563 6174 6564 2e20 5573 6520  deprecated. Use 
+0000d3b0: 6060 4354 7261 6974 2e73 6574 5f64 6566  ``CTrait.set_def
+0000d3c0: 6175 6c74 5f76 616c 7565 6060 2069 6e73  ault_value`` ins
+0000d3d0: 7465 6164 2e20 2823 3632 3029 0a2a 2055  tead. (#620).* U
+0000d3e0: 7365 206f 6620 7468 6520 6060 7269 6368  se of the ``rich
+0000d3f0: 5f63 6f6d 7061 7265 6060 2074 7261 6974  _compare`` trait
+0000d400: 206d 6574 6164 6174 6120 6973 2064 6570   metadata is dep
+0000d410: 7265 6361 7465 642e 2055 7365 2074 6865  recated. Use the
+0000d420: 0a20 2060 6063 6f6d 7061 7269 736f 6e5f  .  ``comparison_
+0000d430: 6d6f 6465 6060 206d 6574 6164 6174 6120  mode`` metadata 
+0000d440: 696e 7374 6561 642e 2028 2335 3938 290a  instead. (#598).
+0000d450: 0a52 656d 6f76 616c 730a 7e7e 7e7e 7e7e  .Removals.~~~~~~
+0000d460: 7e7e 0a0a 2a20 5079 7468 6f6e 2032 2063  ~~..* Python 2 c
+0000d470: 6f6d 7061 7469 6269 6c69 7479 2073 7570  ompatibility sup
+0000d480: 706f 7274 2063 6f64 6520 6861 7320 6265  port code has be
+0000d490: 656e 2072 656d 6f76 6564 2e20 2823 3633  en removed. (#63
+0000d4a0: 382c 2023 3634 3429 0a2a 2054 7261 6974  8, #644).* Trait
+0000d4b0: 7320 6361 7465 676f 7269 6573 2068 6176  s categories hav
+0000d4c0: 6520 6265 656e 2072 656d 6f76 6564 2e20  e been removed. 
+0000d4d0: 2823 3536 3829 0a2a 2054 6865 2066 6f6c  (#568).* The fol
+0000d4e0: 6c6f 7769 6e67 2074 7261 6974 2068 616e  lowing trait han
+0000d4f0: 646c 6572 7320 6861 7665 2062 6565 6e20  dlers have been 
+0000d500: 7265 6d6f 7665 643a 2060 6054 6869 7343  removed: ``ThisC
+0000d510: 6c61 7373 6060 2c0a 2020 6060 5472 6169  lass``,.  ``Trai
+0000d520: 7443 6c61 7373 6060 2c20 6060 5472 6169  tClass``, ``Trai
+0000d530: 7445 7870 7265 7373 696f 6e60 602c 2060  tExpression``, `
+0000d540: 6054 7261 6974 4361 6c6c 6162 6c65 6060  `TraitCallable``
+0000d550: 2c20 6060 5472 6169 7453 7472 696e 6760  , ``TraitString`
+0000d560: 602c 0a20 2060 6054 7261 6974 5261 6e67  `,.  ``TraitRang
+0000d570: 6560 602c 2060 6054 7261 6974 5765 616b  e``, ``TraitWeak
+0000d580: 5265 6660 602e 2028 2337 3832 2c20 2337  Ref``. (#782, #7
+0000d590: 3131 2c20 2336 3939 2c20 2336 3938 2c20  11, #699, #698, 
+0000d5a0: 2336 3235 2c20 2335 3933 2c20 2335 3837  #625, #593, #587
+0000d5b0: 2c0a 2020 2336 3430 290a 2a20 6060 4354  ,.  #640).* ``CT
+0000d5c0: 7261 6974 2e72 6963 685f 636f 6d70 6172  rait.rich_compar
+0000d5d0: 6560 6020 6861 7320 6265 656e 2072 656d  e`` has been rem
+0000d5e0: 6f76 6564 2e20 2823 3539 3829 0a2a 2054  oved. (#598).* T
+0000d5f0: 6865 2060 6063 5472 6169 742e 6361 7374  he ``cTrait.cast
+0000d600: 6060 206d 6574 686f 6420 6861 7320 6265  `` method has be
+0000d610: 656e 2072 656d 6f76 6564 2e20 2823 3636  en removed. (#66
+0000d620: 3329 0a2a 2054 6865 206d 6167 6963 616c  3).* The magical
+0000d630: 2060 6054 7261 6974 5661 6c75 6560 6020   ``TraitValue`` 
+0000d640: 616e 6420 6173 736f 6369 6174 6564 206d  and associated m
+0000d650: 6163 6869 6e65 7279 2068 6176 6520 6265  achinery have be
+0000d660: 656e 2072 656d 6f76 6564 2e20 2823 3635  en removed. (#65
+0000d670: 3829 0a2a 2054 6865 2060 6047 656e 6572  8).* The ``Gener
+0000d680: 6963 6060 2074 7261 6974 2074 7970 6520  ic`` trait type 
+0000d690: 6861 7320 6265 656e 2072 656d 6f76 6564  has been removed
+0000d6a0: 2e20 2823 3635 3729 0a2a 2054 6865 2060  . (#657).* The `
+0000d6b0: 6055 5374 7260 6020 7472 6169 7420 7479  `UStr`` trait ty
+0000d6c0: 7065 2061 6e64 2060 6048 6173 556e 6971  pe and ``HasUniq
+0000d6d0: 7565 5374 7269 6e67 7360 6020 636c 6173  ueStrings`` clas
+0000d6e0: 7320 6861 7665 2062 6565 6e20 7265 6d6f  s have been remo
+0000d6f0: 7665 642e 0a20 2028 2336 3534 290a 2a20  ved..  (#654).* 
+0000d700: 5468 6520 6060 7374 725f 6669 6e64 6060  The ``str_find``
+0000d710: 2061 6e64 2060 6073 7472 5f72 6669 6e64   and ``str_rfind
+0000d720: 6060 2068 656c 7065 7220 6675 6e63 7469  `` helper functi
+0000d730: 6f6e 7320 6861 7665 2062 6565 6e20 7265  ons have been re
+0000d740: 6d6f 7665 642e 2028 2336 3333 290a 2a20  moved. (#633).* 
+0000d750: 5468 6520 676c 6f62 616c 2060 605f 7472  The global ``_tr
+0000d760: 6169 745f 6e6f 7469 6669 6361 7469 6f6e  ait_notification
+0000d770: 5f68 616e 646c 6572 6060 2068 6173 2062  _handler`` has b
+0000d780: 6565 6e20 7265 6d6f 7665 642e 2028 2336  een removed. (#6
+0000d790: 3139 290a 2a20 6060 4261 7365 5472 6169  19).* ``BaseTrai
+0000d7a0: 7448 616e 646c 6572 2e72 6570 7260 6020  tHandler.repr`` 
+0000d7b0: 6861 7320 6265 656e 2072 656d 6f76 6564  has been removed
+0000d7c0: 2e20 2823 3539 3929 0a2a 2060 6048 6173  . (#599).* ``Has
+0000d7d0: 5472 6169 7473 2e74 7261 6974 5f6d 6f6e  Traits.trait_mon
+0000d7e0: 6974 6f72 6060 2077 6173 2075 6e64 6f63  itor`` was undoc
+0000d7f0: 756d 656e 7465 642c 2075 6e74 6573 7465  umented, unteste
+0000d800: 642c 2061 6e64 2062 726f 6b65 6e2c 2061  d, and broken, a
+0000d810: 6e64 0a20 2068 6173 2062 6565 6e20 7265  nd.  has been re
+0000d820: 6d6f 7665 642e 2028 2335 3730 290a 2a20  moved. (#570).* 
+0000d830: 5468 6520 6060 5472 6169 7449 6e73 7461  The ``TraitInsta
+0000d840: 6e63 6560 6020 7472 6169 7420 6861 6e64  nce`` trait hand
+0000d850: 6c65 7220 286e 6f74 2074 6f20 6265 2063  ler (not to be c
+0000d860: 6f6e 6675 7365 640a 2020 7769 7468 2074  onfused.  with t
+0000d870: 6865 2060 6049 6e73 7461 6e63 6560 6020  he ``Instance`` 
+0000d880: 7472 6169 7420 7479 7065 2920 6e6f 206c  trait type) no l
+0000d890: 6f6e 6765 7220 7375 7070 6f72 7473 2061  onger supports a
+0000d8a0: 6461 7074 6174 696f 6e2e 2028 2336 3431  daptation. (#641
+0000d8b0: 290a 2a20 5468 6520 6060 4479 6e61 6d69  ).* The ``Dynami
+0000d8c0: 6356 6965 7760 6020 616e 6420 6060 4861  cView`` and ``Ha
+0000d8d0: 7344 796e 616d 6963 5669 6577 7360 6020  sDynamicViews`` 
+0000d8e0: 636c 6173 7365 7320 6861 7665 2062 6565  classes have bee
+0000d8f0: 6e20 7265 6d6f 7665 640a 2020 6672 6f6d  n removed.  from
+0000d900: 2054 7261 6974 7320 616e 6420 6d6f 7665   Traits and move
+0000d910: 6420 746f 2054 7261 6974 7355 4920 696e  d to TraitsUI in
+0000d920: 7374 6561 642e 2028 2336 3039 290a 2a20  stead. (#609).* 
+0000d930: 6060 4469 6374 5374 724c 6f6e 6760 6020  ``DictStrLong`` 
+0000d940: 6861 7320 6265 656e 2072 656d 6f76 6564  has been removed
+0000d950: 2e20 2823 3537 3329 0a0a 5465 7374 2073  . (#573)..Test s
+0000d960: 7569 7465 0a7e 7e7e 7e7e 7e7e 7e7e 7e0a  uite.~~~~~~~~~~.
+0000d970: 0a2a 2046 6978 2076 6172 696f 7573 2074  .* Fix various t
+0000d980: 6573 7473 2074 6f20 6265 2072 6570 6561  ests to be repea
+0000d990: 7461 626c 652e 2028 2338 3032 2c20 2337  table. (#802, #7
+0000d9a0: 3239 290a 2a20 4669 7820 6465 7072 6563  29).* Fix deprec
+0000d9b0: 6174 696f 6e20 7761 726e 696e 6773 2069  ation warnings i
+0000d9c0: 6e20 7468 6520 7465 7374 2073 7569 7465  n the test suite
+0000d9d0: 206f 7574 7075 742e 2028 2338 3230 2c20   output. (#820, 
+0000d9e0: 2338 3034 2c20 2337 3136 290a 2a20 4164  #804, #716).* Ad
+0000d9f0: 6420 6d61 6368 696e 6572 7920 666f 7220  d machinery for 
+0000da00: 7465 7374 696e 6720 756e 7069 636b 6c69  testing unpickli
+0000da10: 6e67 206f 6620 6869 7374 6f72 6963 616c  ng of historical
+0000da20: 2070 6963 6b6c 6573 2e20 2823 3738 3729   pickles. (#787)
+0000da30: 0a2a 2052 656d 6f76 6520 7072 696e 7420  .* Remove print 
+0000da40: 7374 6174 656d 656e 7473 2066 726f 6d20  statements from 
+0000da50: 7465 7374 2073 7569 7465 2e20 2823 3735  test suite. (#75
+0000da60: 322c 2023 3736 3829 0a2a 2046 6978 2061  2, #768).* Fix a
+0000da70: 2074 6573 7420 746f 2063 6c65 616e 2075   test to clean u
+0000da80: 7020 7468 6520 7468 7265 6164 7320 6974  p the threads it
+0000da90: 2063 7265 6174 6573 2e20 2823 3733 3129   creates. (#731)
+0000daa0: 0a2a 2041 6464 2074 6573 7473 2066 6f72  .* Add tests for
+0000dab0: 2065 7874 656e 6465 6420 7472 6169 7420   extended trait 
+0000dac0: 6368 616e 6765 2069 7373 7565 7320 2335  change issues #5
+0000dad0: 3337 2061 6e64 2023 3533 3820 2823 3534  37 and #538 (#54
+0000dae0: 3329 0a2a 204f 7468 6572 206d 696e 6f72  3).* Other minor
+0000daf0: 2074 6573 7420 6669 7865 732e 2028 2337   test fixes. (#7
+0000db00: 3030 2c20 2338 3231 290a 0a44 6f63 756d  00, #821)..Docum
+0000db10: 656e 7461 7469 6f6e 0a7e 7e7e 7e7e 7e7e  entation.~~~~~~~
+0000db20: 7e7e 7e7e 7e7e 0a0a 2a20 496d 7072 6f76  ~~~~~~..* Improv
+0000db30: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+0000db40: 6f66 2074 7261 6974 2063 6f6e 7461 696e  of trait contain
+0000db50: 6572 206f 626a 6563 7473 2e20 2823 3831  er objects. (#81
+0000db60: 3029 0a2a 2049 6d70 726f 7665 2064 6f63  0).* Improve doc
+0000db70: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
+0000db80: 6865 2060 6074 7261 6974 732e 6374 7261  he ``traits.ctra
+0000db90: 6974 7360 6020 6d6f 6475 6c65 2e20 2823  its`` module. (#
+0000dba0: 3832 362c 2023 3832 342c 0a20 2023 3635  826, #824,.  #65
+0000dbb0: 392c 2023 3635 332c 2023 3832 392c 2023  9, #653, #829, #
+0000dbc0: 3833 3629 0a2a 2046 6978 2062 6164 6c79  836).* Fix badly
+0000dbd0: 2066 6f72 6d61 7474 6564 2060 6054 7261   formatted ``Tra
+0000dbe0: 6974 4861 6e64 6c65 7260 6020 646f 6375  itHandler`` docu
+0000dbf0: 6d65 6e74 6174 696f 6e2e 2028 2338 3137  mentation. (#817
+0000dc00: 290a 2a20 4669 7820 616e 6420 696d 7072  ).* Fix and impr
+0000dc10: 6f76 6520 6261 646c 7920 666f 726d 6174  ove badly format
+0000dc20: 7465 6420 7472 6169 7420 7479 7065 7320  ted trait types 
+0000dc30: 646f 6375 6d65 6e74 6174 696f 6e2e 2028  documentation. (
+0000dc40: 2338 3433 290a 2a20 4669 7820 6272 6f6b  #843).* Fix brok
+0000dc50: 656e 206d 6f64 756c 6520 6c69 6e6b 7320  en module links 
+0000dc60: 696e 2073 6563 7469 6f6e 2074 6974 6c65  in section title
+0000dc70: 7320 696e 2041 5049 2064 6f63 756d 656e  s in API documen
+0000dc80: 7461 7469 6f6e 2e20 2823 3832 3329 0a2a  tation. (#823).*
+0000dc90: 2041 6464 6974 696f 6e61 6c20 636c 6173   Additional clas
+0000dca0: 7320 646f 6373 7472 696e 6720 6669 7865  s docstring fixe
+0000dcb0: 732e 2028 2338 3534 290a 2a20 4164 6420  s. (#854).* Add 
+0000dcc0: 6368 616e 6765 6c6f 6720 746f 2062 7569  changelog to bui
+0000dcd0: 6c74 2064 6f63 756d 656e 7461 7469 6f6e  lt documentation
+0000dce0: 2c20 616e 6420 6162 736f 7262 206f 6c64  , and absorb old
+0000dcf0: 2063 6861 6e67 656c 6f67 2069 6e74 6f0a   changelog into.
+0000dd00: 2020 7468 6520 6e65 7720 6f6e 652e 2028    the new one. (
+0000dd10: 2338 3030 2c20 2337 3939 290a 2a20 5265  #800, #799).* Re
+0000dd20: 6d6f 7665 2064 6570 7265 6361 7465 6420  move deprecated 
+0000dd30: 7472 6169 7473 2066 726f 6d20 7468 6520  traits from the 
+0000dd40: 7573 6572 206d 616e 7561 6c2e 2028 2336  user manual. (#6
+0000dd50: 3536 290a 2a20 4669 7820 7661 7269 6f75  56).* Fix variou
+0000dd60: 7320 5370 6869 6e78 2077 6172 6e69 6e67  s Sphinx warning
+0000dd70: 7320 2823 3731 3729 0a2a 2055 7365 2053  s (#717).* Use S
+0000dd80: 5647 2062 6164 6765 7320 696e 2052 4541  VG badges in REA
+0000dd90: 444d 4520 2823 3536 3729 0a0a 4275 696c  DME (#567)..Buil
+0000dda0: 6420 616e 6420 636f 6e74 696e 756f 7573  d and continuous
+0000ddb0: 2069 6e74 6567 7261 7469 6f6e 0a7e 7e7e   integration.~~~
+0000ddc0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+0000ddd0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a2a  ~~~~~~~~~~~~~..*
+0000dde0: 2045 6e61 626c 6520 4320 6173 7365 7274   Enable C assert
+0000ddf0: 7320 696e 2054 7261 7669 7320 4349 2072  s in Travis CI r
+0000de00: 756e 732e 2028 2337 3931 290a 2a20 4162  uns. (#791).* Ab
+0000de10: 6f72 7420 4349 206f 6e20 636f 6d70 696c  ort CI on compil
+0000de20: 6572 2077 6172 6e69 6e67 7320 696e 2054  er warnings in T
+0000de30: 7261 7669 7320 4349 2072 756e 732e 2028  ravis CI runs. (
+0000de40: 2337 3639 290a 2a20 5275 6e20 6120 6060  #769).* Run a ``
+0000de50: 666c 616b 6538 6060 2063 6865 636b 2069  flake8`` check i
+0000de60: 6e20 626f 7468 2054 7261 7669 7320 4349  n both Travis CI
+0000de70: 2061 6e64 2041 7070 7665 796f 7220 7275   and Appveyor ru
+0000de80: 6e73 2e20 2823 3735 332c 2023 3736 3229  ns. (#753, #762)
+0000de90: 0a2a 2043 6865 636b 696e 6720 636f 7079  .* Checking copy
+0000dea0: 7269 6768 7420 7374 6174 656d 656e 7473  right statements
+0000deb0: 2069 6e20 5079 7468 6f6e 2066 696c 6573   in Python files
+0000dec0: 2061 7320 7061 7274 206f 6620 4349 2072   as part of CI r
+0000ded0: 756e 732e 2028 2337 3439 290a 2a20 5475  uns. (#749).* Tu
+0000dee0: 726e 2077 6172 6e69 6e67 7320 696e 746f  rn warnings into
+0000def0: 2065 7272 6f72 7320 7768 656e 2062 7569   errors when bui
+0000df00: 6c64 696e 6720 646f 6375 6d65 6e74 6174  lding documentat
+0000df10: 696f 6e20 696e 2043 492e 2028 2337 3434  ion in CI. (#744
+0000df20: 290a 2a20 4164 6420 6060 676e 7572 6561  ).* Add ``gnurea
+0000df30: 646c 696e 6560 6020 6173 2061 2064 6576  dline`` as a dev
+0000df40: 656c 6f70 6d65 6e74 2064 6570 656e 6465  elopment depende
+0000df50: 6e63 7920 6f6e 206d 6163 4f53 2061 6e64  ncy on macOS and
+0000df60: 204c 696e 7578 2e20 2823 3630 3729 0a2a   Linux. (#607).*
+0000df70: 2041 6464 2061 6e20 6060 6574 7374 6f6f   Add an ``etstoo
+0000df80: 6c2e 7079 6060 206f 7074 696f 6e20 746f  l.py`` option to
+0000df90: 2072 756e 2074 6573 7473 2071 7569 6574   run tests quiet
+0000dfa0: 6c79 2e20 2823 3630 3629 0a2a 2045 6e61  ly. (#606).* Ena
+0000dfb0: 626c 6520 7468 6520 636f 7665 7261 6765  ble the coverage
+0000dfc0: 2065 7874 656e 7369 6f6e 2066 6f72 2074   extension for t
+0000dfd0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+0000dfe0: 2062 7569 6c64 2e20 2823 3830 3729 0a2a   build. (#807).*
+0000dff0: 2052 656d 6f76 6520 6d6f 636b 696e 6720   Remove mocking 
+0000e000: 696e 2064 6f63 756d 656e 7461 7469 6f6e  in documentation
+0000e010: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
+0000e020: 616e 6420 6669 7820 6120 6465 7072 6563  and fix a deprec
+0000e030: 6174 6564 0a20 2063 6f6e 6669 6775 7261  ated.  configura
+0000e040: 7469 6f6e 206f 7074 696f 6e2e 2028 2336  tion option. (#6
+0000e050: 3936 290a 0a4d 6169 6e74 656e 616e 6365  96)..Maintenance
+0000e060: 2061 6e64 2063 6f64 6520 6f72 6761 6e69   and code organi
+0000e070: 7a61 7469 6f6e 0a7e 7e7e 7e7e 7e7e 7e7e  zation.~~~~~~~~~
+0000e080: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+0000e090: 7e7e 7e7e 7e7e 7e7e 0a0a 5468 6973 2072  ~~~~~~~~..This r
+0000e0a0: 656c 6561 7365 2069 6e63 6c75 6465 7320  elease includes 
+0000e0b0: 6120 6c6f 7420 6f66 2072 6566 6163 746f  a lot of refacto
+0000e0c0: 7269 6e67 2061 6e64 206d 616e 7920 6d69  ring and many mi
+0000e0d0: 6e6f 7220 696d 7072 6f76 656d 656e 7473  nor improvements
+0000e0e0: 0a74 6861 7420 7769 6c6c 2070 7269 6d61  .that will prima
+0000e0f0: 7269 6c79 2062 656e 6566 6974 2074 686f  rily benefit tho
+0000e100: 7365 2077 6f72 6b69 6e67 2077 6974 6820  se working with 
+0000e110: 7468 6520 5472 6169 7473 2063 6f64 6562  the Traits codeb
+0000e120: 6173 652e 2054 6865 7365 0a63 6861 6e67  ase. These.chang
+0000e130: 6573 2073 686f 756c 6420 6e6f 7420 6166  es should not af
+0000e140: 6665 6374 2075 7365 722d 7669 7369 626c  fect user-visibl
+0000e150: 6520 6675 6e63 7469 6f6e 616c 6974 792e  e functionality.
+0000e160: 2048 6572 6527 7320 6120 7375 6d6d 6172   Here's a summar
+0000e170: 790a 6f66 2074 6865 206d 6f72 6520 7369  y.of the more si
+0000e180: 676e 6966 6963 616e 7420 6368 616e 6765  gnificant change
+0000e190: 732e 0a0a 2a20 4120 6d61 6a6f 7220 7265  s...* A major re
+0000e1a0: 6661 6374 6f72 2068 6173 2072 656d 6f76  factor has remov
+0000e1b0: 6564 206d 6f73 7420 6f66 2074 6865 2063  ed most of the c
+0000e1c0: 6972 6375 6c61 7220 6465 7065 6e64 656e  ircular dependen
+0000e1d0: 6369 6573 2062 6574 7765 656e 0a20 206d  cies between.  m
+0000e1e0: 6f64 756c 6573 2e20 2823 3733 3029 0a2a  odules. (#730).*
+0000e1f0: 2054 6865 2063 6f64 6562 6173 6520 6973   The codebase is
+0000e200: 206e 6f77 206d 6f73 746c 7920 6060 666c   now mostly ``fl
+0000e210: 616b 6538 6060 2063 6c65 616e 2e20 2823  ake8`` clean. (#
+0000e220: 3738 362c 2023 3735 332c 2023 3734 372c  786, #753, #747,
+0000e230: 2023 3734 382c 2023 3734 362c 0a20 2023   #748, #746,.  #
+0000e240: 3539 3529 0a2a 2043 6f70 7972 6967 6874  595).* Copyright
+0000e250: 2068 6561 6465 7273 2068 6176 6520 6265   headers have be
+0000e260: 656e 206d 6164 6520 636f 6e73 6973 7465  en made consiste
+0000e270: 6e74 2066 6f72 2061 6c6c 2050 7974 686f  nt for all Pytho
+0000e280: 6e20 6669 6c65 732e 2028 2337 3534 290a  n files. (#754).
+0000e290: 2a20 6060 6374 7261 6974 732e 6360 6020  * ``ctraits.c`` 
+0000e2a0: 6861 7320 6265 656e 2072 756e 2074 6872  has been run thr
+0000e2b0: 6f75 6768 2060 6063 6c61 6e67 2d74 6964  ough ``clang-tid
+0000e2c0: 7960 6020 616e 6420 6060 636c 616e 672d  y`` and ``clang-
+0000e2d0: 666f 726d 6174 6060 2069 6e0a 2020 6f72  format`` in.  or
+0000e2e0: 6465 7220 746f 2062 7269 6e67 2069 7420  der to bring it 
+0000e2f0: 636c 6f73 6572 2074 6f20 5045 5020 3720  closer to PEP 7 
+0000e300: 7374 796c 652e 2028 2337 3135 290a 2a20  style. (#715).* 
+0000e310: 4564 6974 6f72 2066 6163 746f 7269 6573  Editor factories
+0000e320: 2068 6176 6520 6265 656e 206d 6f76 6564   have been moved
+0000e330: 2069 6e74 6f20 6120 6e65 7720 6060 7472   into a new ``tr
+0000e340: 6169 7473 2e65 6469 746f 725f 6661 6374  aits.editor_fact
+0000e350: 6f72 6965 7360 600a 2020 6d6f 6475 6c65  ories``.  module
+0000e360: 2c20 746f 2068 656c 7020 636f 6d70 6172  , to help compar
+0000e370: 746d 656e 7461 6c69 7a65 2063 6f64 6520  tmentalize code 
+0000e380: 6465 7065 6e64 656e 6369 6573 206f 6e20  dependencies on 
+0000e390: 5472 6169 7473 5549 2e20 2823 3636 3129  TraitsUI. (#661)
+0000e3a0: 0a2a 2054 7261 6974 2063 6f6e 7461 696e  .* Trait contain
+0000e3b0: 6572 206f 626a 6563 7420 636c 6173 7365  er object classe
+0000e3c0: 7320 2860 6054 7261 6974 4469 6374 4f62  s (``TraitDictOb
+0000e3d0: 6a65 6374 6060 2c20 6060 5472 6169 744c  ject``, ``TraitL
+0000e3e0: 6973 744f 626a 6563 7460 602c 0a20 2060  istObject``,.  `
+0000e3f0: 6054 7261 6974 5365 744f 626a 6563 7460  `TraitSetObject`
+0000e400: 6029 2068 6176 6520 6561 6368 2062 6565  `) have each bee
+0000e410: 6e20 6d6f 7665 6420 696e 746f 2074 6865  n moved into the
+0000e420: 6972 206f 776e 206d 6f64 756c 652c 2061  ir own module, a
+0000e430: 6c6f 6e67 0a20 2077 6974 6820 7468 6569  long.  with thei
+0000e440: 7220 6173 736f 6369 6174 6564 2065 7665  r associated eve
+0000e450: 6e74 2074 7970 652e 2028 2336 3737 290a  nt type. (#677).
+0000e460: 2a20 4d69 7363 656c 6c61 6e65 6f75 7320  * Miscellaneous 
+0000e470: 6f74 6865 7220 6d69 6e6f 7220 6669 7865  other minor fixe
+0000e480: 732c 2072 6566 6163 746f 7269 6e67 7320  s, refactorings 
+0000e490: 616e 6420 636c 6561 6e75 7073 2e0a 2020  and cleanups..  
+0000e4a0: 2823 3738 352c 2023 3737 372c 2023 3735  (#785, #777, #75
+0000e4b0: 302c 2023 3732 362c 2023 3731 342c 2023  0, #726, #714, #
+0000e4c0: 3731 322c 2023 3730 382c 2023 3730 312c  712, #708, #701,
+0000e4d0: 2023 3638 322c 2023 3636 352c 2023 3635   #682, #665, #65
+0000e4e0: 312c 0a20 2023 3635 322c 2023 3633 392c  1,.  #652, #639,
+0000e4f0: 2023 3633 362c 2023 3633 342c 2023 3632   #636, #634, #62
+0000e500: 362c 2023 3633 322c 2023 3631 312c 2023  6, #632, #611, #
+0000e510: 3631 332c 2023 3631 322c 2023 3630 352c  613, #612, #605,
+0000e520: 2023 3630 332c 0a20 2023 3630 302c 2023   #603,.  #600, #
+0000e530: 3539 372c 2023 3538 362c 2023 3538 352c  597, #586, #585,
+0000e540: 2023 3538 342c 2023 3538 302c 2023 3537   #584, #580, #57
+0000e550: 372c 2023 3537 382c 2023 3536 342c 2023  7, #578, #564, #
+0000e560: 3830 3629 0a0a 0a52 656c 6561 7365 2035  806)...Release 5
+0000e570: 2e32 2e30 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .2.0.-----------
+0000e580: 2d2d 0a0a 5265 6c65 6173 6564 3a20 3230  --..Released: 20
+0000e590: 3139 2d31 312d 3138 0a0a 456e 6861 6e63  19-11-18..Enhanc
+0000e5a0: 656d 656e 7473 0a0a 2a20 5375 7070 6f72  ements..* Suppor
+0000e5b0: 7420 696e 7374 616c 6c61 7469 6f6e 2066  t installation f
+0000e5c0: 726f 6d20 736f 7572 6365 2061 7263 6869  rom source archi
+0000e5d0: 7665 732e 2028 2335 3238 290a 0a46 6978  ves. (#528)..Fix
+0000e5e0: 6573 0a0a 2a20 456e 7375 7265 2060 6054  es..* Ensure ``T
+0000e5f0: 7261 6974 4c69 7374 4576 656e 742e 696e  raitListEvent.in
+0000e600: 6465 7860 6020 6973 2061 6c77 6179 7320  dex`` is always 
+0000e610: 616e 2069 6e74 6567 6572 2e20 2823 3534  an integer. (#54
+0000e620: 3829 0a2a 2055 7064 6174 6520 7468 6520  8).* Update the 
+0000e630: 6465 7072 6563 6174 6564 2060 6063 6f6c  deprecated ``col
+0000e640: 6c65 6374 696f 6e73 2e4d 7574 6162 6c65  lections.Mutable
+0000e650: 4d61 7070 696e 6760 6020 696d 706f 7274  Mapping`` import
+0000e660: 2e20 2823 3533 3029 0a2a 2046 6978 2069  . (#530).* Fix i
+0000e670: 6e61 6476 6572 7465 6e74 206d 6f64 6966  nadvertent modif
+0000e680: 6963 6174 696f 6e20 6f66 2074 6865 2060  ication of the `
+0000e690: 6043 6174 6567 6f72 7960 6020 6261 7365  `Category`` base
+0000e6a0: 2063 6c61 7373 2e20 2823 3530 3929 0a2a   class. (#509).*
+0000e6b0: 2052 6577 6f72 6b20 7665 7273 696f 6e20   Rework version 
+0000e6c0: 6861 6e64 6c69 6e67 2069 6e20 6060 7365  handling in ``se
+0000e6d0: 7475 702e 7079 6060 2e20 2823 3531 3529  tup.py``. (#515)
+0000e6e0: 0a2a 2044 6f6e 2774 2061 7574 6f67 656e  .* Don't autogen
+0000e6f0: 6572 6174 6520 646f 6375 6d65 6e74 6174  erate documentat
+0000e700: 696f 6e20 666f 7220 6060 5669 6577 456c  ion for ``ViewEl
+0000e710: 656d 656e 7460 602e 2028 2335 3539 290a  ement``. (#559).
+0000e720: 2a20 456e 7375 7265 2074 6861 7420 616c  * Ensure that al
+0000e730: 6c20 7465 7374 7320 6172 6520 6060 756e  l tests are ``un
+0000e740: 6974 7465 7374 6060 2063 6f6d 7061 7469  ittest`` compati
+0000e750: 626c 652e 2028 2335 3531 290a 0a43 6861  ble. (#551)..Cha
+0000e760: 6e67 6573 0a0a 2a20 5265 706c 6163 6520  nges..* Replace 
+0000e770: 6f63 6375 7265 6e63 6573 206f 6620 6465  occurences of de
+0000e780: 7072 6563 6174 6564 2060 6041 6461 7074  precated ``Adapt
+0000e790: 7354 6f60 6020 7769 7468 2060 6053 7570  sTo`` with ``Sup
+0000e7a0: 706f 7274 7360 602e 2028 2335 3332 290a  ports``. (#532).
+0000e7b0: 2a20 5265 6d6f 7665 2060 6043 6c61 7373  * Remove ``Class
+0000e7c0: 6060 2074 7261 6974 2e20 2823 3532 3029  `` trait. (#520)
+0000e7d0: 0a2a 2044 6570 7265 6361 7465 2060 6043  .* Deprecate ``C
+0000e7e0: 6174 6567 6f72 7960 6020 7472 6169 742e  ategory`` trait.
+0000e7f0: 2028 2335 3130 290a 2a20 4669 7820 7479   (#510).* Fix ty
+0000e800: 706f 7320 696e 2064 6f63 7374 7269 6e67  pos in docstring
+0000e810: 732e 2028 2335 3032 290a 2a20 5573 6520  s. (#502).* Use 
+0000e820: 6465 636f 7261 746f 7220 666f 726d 206f  decorator form o
+0000e830: 6620 6060 636c 6173 736d 6574 686f 6460  f ``classmethod`
+0000e840: 602e 2028 2335 3030 290a 2a20 5265 6d6f  `. (#500).* Remo
+0000e850: 7665 2072 6564 6566 696e 6974 696f 6e20  ve redefinition 
+0000e860: 6f66 2060 604e 756c 6c48 616e 646c 6572  of ``NullHandler
+0000e870: 6060 2e20 2823 3531 3829 0a2a 2041 6464  ``. (#518).* Add
+0000e880: 2061 6e20 696d 706f 7274 2063 6865 636b   an import check
+0000e890: 2068 656c 7065 722e 2028 2335 3231 290a   helper. (#521).
+0000e8a0: 2a20 436c 6561 6e20 7570 2043 7974 686f  * Clean up Cytho
+0000e8b0: 6e20 7465 7374 732e 2028 2335 3535 290a  n tests. (#555).
+0000e8c0: 2a20 436c 6561 6e20 7570 2074 6573 7420  * Clean up test 
+0000e8d0: 6f75 7470 7574 2e20 2823 3535 3329 0a0a  output. (#553)..
+0000e8e0: 4d69 7363 656c 6c61 6e65 6f75 730a 0a2a  Miscellaneous..*
+0000e8f0: 2055 7064 6174 6520 4544 4d20 7665 7273   Update EDM vers
+0000e900: 696f 6e20 6f6e 2043 4920 746f 2076 6572  ion on CI to ver
+0000e910: 7369 6f6e 2032 2e30 2e30 2e20 2823 3536  sion 2.0.0. (#56
+0000e920: 3029 0a2a 2044 6f6e 2774 2066 696e 6973  0).* Don't finis
+0000e930: 6820 6661 7374 206f 6e20 4349 2e20 2823  h fast on CI. (#
+0000e940: 3535 3629 0a2a 2055 7365 2060 6075 6e69  556).* Use ``uni
+0000e950: 7474 6573 7460 6020 746f 2072 756e 2074  ttest`` to run t
+0000e960: 6573 7473 2069 6e20 4349 2e20 2823 3535  ests in CI. (#55
+0000e970: 3229 0a2a 204c 6f77 2d6c 6576 656c 2066  2).* Low-level f
+0000e980: 6978 6573 2061 6e64 2073 7479 6c65 2063  ixes and style c
+0000e990: 6c65 616e 7570 2069 6e20 6060 6574 7374  leanup in ``etst
+0000e9a0: 6f6f 6c2e 7079 6060 2e20 2823 3535 3029  ool.py``. (#550)
+0000e9b0: 0a2a 2041 6464 2060 602d 2d65 6469 7461  .* Add ``--edita
+0000e9c0: 626c 6560 6020 6f70 7469 6f6e 2066 6f72  ble`` option for
+0000e9d0: 2060 6069 6e73 7461 6c6c 6060 2c20 6060   ``install``, ``
+0000e9e0: 7570 6461 7465 6060 2043 4920 636f 6d6d  update`` CI comm
+0000e9f0: 616e 6473 2e20 2823 3534 3629 0a2a 204d  ands. (#546).* M
+0000ea00: 616b 6520 6769 7420 636f 6d6d 6974 2068  ake git commit h
+0000ea10: 6173 6820 6176 6169 6c61 626c 6520 746f  ash available to
+0000ea20: 2061 7263 6869 7665 732e 2028 2335 3236   archives. (#526
+0000ea30: 290a 2a20 4669 7820 7573 6520 6f66 206e  ).* Fix use of n
+0000ea40: 6f6e 2d65 646d 2065 6e76 7320 6173 2062  on-edm envs as b
+0000ea50: 6f6f 7473 7472 6170 2065 6e76 7320 6f6e  ootstrap envs on
+0000ea60: 2057 696e 646f 7773 2e20 2823 3531 3229   Windows. (#512)
+0000ea70: 0a2a 2052 656d 6f76 6520 6564 6d20 696e  .* Remove edm in
+0000ea80: 7374 616c 6c65 6420 7061 636b 6167 6520  stalled package 
+0000ea90: 6265 666f 7265 2069 6e73 7461 6c6c 696e  before installin
+0000eaa0: 6720 6672 6f6d 2073 6f75 7263 652e 2028  g from source. (
+0000eab0: 2335 3136 290a 2a20 4164 6420 6865 6c70  #516).* Add help
+0000eac0: 2074 6578 7420 746f 2063 6c69 636b 206f   text to click o
+0000ead0: 7074 696f 6e73 2e20 2823 3531 3429 0a2a  ptions. (#514).*
+0000eae0: 2056 6172 696f 7573 2063 6c65 616e 7570   Various cleanup
+0000eaf0: 732c 2066 6978 6573 2061 6e64 2065 6e68  s, fixes and enh
+0000eb00: 616e 6365 6d65 6e74 7320 696e 2060 6065  ancements in ``e
+0000eb10: 7473 746f 6f6c 2e70 7960 602e 2028 2335  tstool.py``. (#5
+0000eb20: 3131 290a 0a0a 5265 6c65 6173 6520 352e  11)...Release 5.
+0000eb30: 312e 320a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  1.2.------------
+0000eb40: 2d0a 0a52 656c 6561 7365 643a 2032 3031  -..Released: 201
+0000eb50: 392d 3037 2d30 380a 0a46 6978 6573 0a0a  9-07-08..Fixes..
+0000eb60: 2a20 5472 6169 7473 2064 6f63 756d 656e  * Traits documen
+0000eb70: 7465 7220 6e6f 206c 6f6e 6765 7220 6765  ter no longer ge
+0000eb80: 6e65 7261 7465 7320 6261 6420 7265 5354  nerates bad reST
+0000eb90: 2066 6f72 2074 7261 6974 7320 7768 6f73   for traits whos
+0000eba0: 6520 6465 6669 6e69 7469 6f6e 0a20 2073  e definition.  s
+0000ebb0: 7061 6e73 206d 756c 7469 706c 6520 736f  pans multiple so
+0000ebc0: 7572 6365 206c 696e 6573 2e20 2823 3439  urce lines. (#49
+0000ebd0: 3429 0a0a 0a52 656c 6561 7365 2035 2e31  4)...Release 5.1
+0000ebe0: 2e31 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .1.-------------
+0000ebf0: 0a0a 5265 6c65 6173 6564 3a20 3230 3139  ..Released: 2019
+0000ec00: 2d30 342d 3138 0a0a 4669 7865 730a 0a2a  -04-18..Fixes..*
+0000ec10: 2052 6576 6572 7420 6120 6368 616e 6765   Revert a change
+0000ec20: 2028 2334 3439 2920 7768 6963 6820 6163   (#449) which ac
+0000ec30: 6369 6465 6e74 616c 6c79 2062 726f 6b65  cidentally broke
+0000ec40: 2065 7874 6572 6e61 6c20 7573 6573 206f   external uses o
+0000ec50: 660a 2020 6060 5f70 7932 746f 332e 7374  f.  ``_py2to3.st
+0000ec60: 725f 6669 6e64 6060 2061 6e64 2060 605f  r_find`` and ``_
+0000ec70: 7079 3274 6f33 2e73 7472 5f72 6669 6e64  py2to3.str_rfind
+0000ec80: 6060 2e20 2823 3437 3229 0a0a 5265 6c65  ``. (#472)..Rele
+0000ec90: 6173 6520 352e 312e 300a 2d2d 2d2d 2d2d  ase 5.1.0.------
+0000eca0: 2d2d 2d2d 2d2d 2d0a 0a52 656c 6561 7365  -------..Release
+0000ecb0: 643a 2032 3031 392d 3034 2d31 350a 0a45  d: 2019-04-15..E
+0000ecc0: 6e68 616e 6365 6d65 6e74 730a 0a2a 204d  nhancements..* M
+0000ecd0: 616b 6520 5555 4944 2074 7261 6974 2069  ake UUID trait i
+0000ece0: 6e69 7469 616c 697a 6162 6c65 2e20 2823  nitializable. (#
+0000ecf0: 3435 3929 0a2a 2043 6861 6e67 6520 6465  459).* Change de
+0000ed00: 6661 756c 7420 6060 4669 6c65 4564 6974  fault ``FileEdit
+0000ed10: 6f72 6060 2062 6568 6176 696f 7220 666f  or`` behavior fo
+0000ed20: 7220 6120 6060 4669 6c65 6060 2074 7261  r a ``File`` tra
+0000ed30: 6974 2062 6173 6564 206f 6e0a 2020 7768  it based on.  wh
+0000ed40: 6574 6865 7220 6060 6578 6973 7473 3d54  ether ``exists=T
+0000ed50: 7275 6560 6020 6973 2073 7065 6369 6669  rue`` is specifi
+0000ed60: 6564 2066 6f72 2074 6861 7420 7472 6169  ed for that trai
+0000ed70: 742e 2028 2334 3531 2c20 2334 3637 290a  t. (#451, #467).
+0000ed80: 0a43 6861 6e67 6573 0a0a 2a20 5468 6520  .Changes..* The 
+0000ed90: 6368 616e 6765 7320 6d61 6465 2069 6e20  changes made in 
+0000eda0: 2333 3733 2074 6f20 6d61 6b65 2064 796e  #373 to make dyn
+0000edb0: 616d 6963 616c 6c79 2d61 6464 6564 2074  amically-added t
+0000edc0: 7261 6974 7320 7069 636b 6c65 6162 6c65  raits pickleable
+0000edd0: 2068 6176 650a 2020 6265 656e 2072 6576   have.  been rev
+0000ede0: 6572 7465 642e 2028 2334 3632 290a 2a20  erted. (#462).* 
+0000edf0: 6060 7472 6169 7473 2e61 7069 2e70 7974  ``traits.api.pyt
+0000ee00: 686f 6e5f 7665 7273 696f 6e60 6020 6861  hon_version`` ha
+0000ee10: 7320 6265 656e 2072 656d 6f76 6564 2e20  s been removed. 
+0000ee20: 496e 7465 726e 616c 7320 6861 7665 2062  Internals have b
+0000ee30: 6565 6e0a 2020 7265 6661 6374 6f72 6564  een.  refactored
+0000ee40: 2074 6f20 7573 6520 6060 7369 782e 5059   to use ``six.PY
+0000ee50: 3260 6020 696e 2070 7265 6665 7265 6e63  2`` in preferenc
+0000ee60: 6520 746f 2060 6073 7973 2e76 6572 7369  e to ``sys.versi
+0000ee70: 6f6e 5f69 6e66 6f60 602e 0a20 2028 2334  on_info``..  (#4
+0000ee80: 3439 290a 2a20 446f 6e27 7420 6465 7065  49).* Don't depe
+0000ee90: 6e64 206f 6e20 7468 6520 3372 6420 7061  nd on the 3rd pa
+0000eea0: 7274 7920 6060 6d6f 636b 6060 206c 6962  rty ``mock`` lib
+0000eeb0: 7261 7279 206f 6e20 5079 7468 6f6e 2033  rary on Python 3
+0000eec0: 3b20 7573 650a 2020 6060 756e 6974 7465  ; use.  ``unitte
+0000eed0: 7374 2e6d 6f63 6b60 6020 696e 7374 6561  st.mock`` instea
+0000eee0: 642e 2028 2334 3436 290a 0a46 6978 6573  d. (#446)..Fixes
+0000eef0: 0a0a 2a20 4669 7820 6120 6672 6167 696c  ..* Fix a fragil
+0000ef00: 6520 4e75 6d50 792d 7265 6c61 7465 6420  e NumPy-related 
+0000ef10: 7465 7374 2074 6861 7420 6661 696c 6564  test that failed
+0000ef20: 2028 6060 5275 6e74 696d 6545 7272 6f72   (``RuntimeError
+0000ef30: 3a20 656d 7074 795f 6c69 6b65 0a20 206d  : empty_like.  m
+0000ef40: 6574 686f 6420 616c 7265 6164 7920 6861  ethod already ha
+0000ef50: 7320 6120 646f 6373 7472 696e 6760 6029  s a docstring``)
+0000ef60: 2077 6974 6820 7468 6520 6e65 7765 7374   with the newest
+0000ef70: 2076 6572 7369 6f6e 206f 6620 4e75 6d50   version of NumP
+0000ef80: 792e 0a20 2028 2334 3433 290a 0a4d 6973  y..  (#443)..Mis
+0000ef90: 6365 6c6c 616e 656f 7573 0a0a 2a20 6060  cellaneous..* ``
+0000efa0: 7472 6169 7473 2e5f 7665 7273 696f 6e2e  traits._version.
+0000efb0: 6769 745f 7265 7669 7369 6f6e 6060 206e  git_revision`` n
+0000efc0: 6f77 2067 6976 6573 2074 6865 2066 756c  ow gives the ful
+0000efd0: 6c20 636f 6d6d 6974 2068 6173 6820 2866  l commit hash (f
+0000efe0: 6f72 206c 6f63 616c 0a20 2062 7569 6c64  or local.  build
+0000eff0: 7329 2069 6e73 7465 6164 206f 6620 616e  s) instead of an
+0000f000: 2061 6262 7265 7669 6174 6564 2037 2068   abbreviated 7 h
+0000f010: 6578 2d64 6967 6974 2076 6572 7369 6f6e  ex-digit version
+0000f020: 2e20 2823 3435 3329 0a2a 2046 6978 2063  . (#453).* Fix c
+0000f030: 6f70 7972 6967 6874 2079 6561 7273 2069  opyright years i
+0000f040: 6e20 646f 6375 6d65 6e74 6174 696f 6e20  n documentation 
+0000f050: 6275 696c 642e 2028 2334 3435 290a 2a20  build. (#445).* 
+0000f060: 5265 6e61 6d65 2060 6052 4541 444d 452e  Rename ``README.
+0000f070: 7478 7460 6020 746f 2060 6052 4541 444d  txt`` to ``READM
+0000f080: 452e 7273 7460 602c 2073 6f20 7468 6174  E.rst``, so that
+0000f090: 2047 6974 4875 6220 7265 6e64 6572 7320   GitHub renders 
+0000f0a0: 6974 206e 6963 656c 792e 0a2a 2043 6f64  it nicely..* Cod
+0000f0b0: 6520 636c 6561 6e75 7073 3a20 7265 6d6f  e cleanups: remo
+0000f0c0: 7665 2022 454f 4622 206d 6172 6b65 7273  ve "EOF" markers
+0000f0d0: 2066 726f 6d20 636f 6465 2e20 5265 6d6f   from code. Remo
+0000f0e0: 7665 2060 605f 5f6d 6169 6e5f 5f60 6020  ve ``__main__`` 
+0000f0f0: 626c 6f63 6b73 0a20 2066 6f72 2075 6e69  blocks.  for uni
+0000f100: 7420 7465 7374 732e 2052 656d 6f76 6520  t tests. Remove 
+0000f110: 696d 706f 7274 7320 6f66 2060 6075 6e69  imports of ``uni
+0000f120: 7474 6573 7460 6020 6672 6f6d 2060 6075  ttest`` from ``u
+0000f130: 6e69 7474 6573 745f 746f 6f6c 7360 602e  nittest_tools``.
+0000f140: 0a20 2028 2334 3438 2c20 2334 3436 290a  .  (#448, #446).
+0000f150: 2a20 5570 6461 7465 2054 7261 7669 7320  * Update Travis 
+0000f160: 4349 2061 6e64 2041 7070 7665 796f 7220  CI and Appveyor 
+0000f170: 636f 6e66 6967 7572 6174 696f 6e73 2074  configurations t
+0000f180: 6f20 7275 6e20 7465 7374 7320 6167 6169  o run tests agai
+0000f190: 6e73 740a 2020 616c 6c20 5052 2062 7261  nst.  all PR bra
+0000f1a0: 6e63 6865 732c 206e 6f74 206a 7573 7420  nches, not just 
+0000f1b0: 5052 7320 6167 6169 6e73 7420 6d61 7374  PRs against mast
+0000f1c0: 6572 2e20 2823 3436 3629 0a0a 0a52 656c  er. (#466)...Rel
+0000f1d0: 6561 7365 2035 2e30 2e30 0a2d 2d2d 2d2d  ease 5.0.0.-----
+0000f1e0: 2d2d 2d2d 2d2d 2d2d 0a0a 5265 6c65 6173  --------..Releas
+0000f1f0: 6564 203a 2033 3020 4a61 6e75 6172 7920  ed : 30 January 
+0000f200: 3230 3139 0a0a 5468 6973 206d 616a 6f72  2019..This major
+0000f210: 2072 656c 6561 7365 2061 6363 756d 756c   release accumul
+0000f220: 6174 6573 206d 6f72 6520 7468 616e 2061  ates more than a
+0000f230: 6e20 7965 6172 2773 2077 6f72 7468 206f  n year's worth o
+0000f240: 6620 696d 7072 6f76 656d 656e 7473 2c0a  f improvements,.
+0000f250: 6368 616e 6765 7320 616e 6420 6275 6720  changes and bug 
+0000f260: 6669 7865 7320 746f 2074 6865 2063 6f64  fixes to the cod
+0000f270: 6520 6261 7365 2e0a 0a41 2066 6577 2068  e base...A few h
+0000f280: 6967 686c 6967 6874 7320 6f66 2074 6869  ighlights of thi
+0000f290: 7320 7265 6c65 6173 6520 6172 6520 3a0a  s release are :.
+0000f2a0: 0a2a 2052 656d 6f76 616c 206f 6620 3274  .* Removal of 2t
+0000f2b0: 6f33 2066 6978 6572 7320 616e 6420 7468  o3 fixers and th
+0000f2c0: 6520 7573 6520 6f66 2073 6978 2074 6f20  e use of six to 
+0000f2d0: 7072 6f76 6964 6520 5079 7468 6f6e 2032  provide Python 2
+0000f2e0: 2f33 2063 6f6d 7061 7469 6269 6c69 7479  /3 compatibility
+0000f2f0: 0a2a 2052 656d 6f76 616c 206f 6620 6465  .* Removal of de
+0000f300: 7072 6563 6174 6564 2060 6074 7261 6974  precated ``trait
+0000f310: 732e 7072 6f74 6f63 6f6c 7360 6020 7375  s.protocols`` su
+0000f320: 626d 6f64 756c 6520 616e 6420 7265 6c61  bmodule and rela
+0000f330: 7465 6420 7574 696c 732e 0a2a 204e 6577  ted utils..* New
+0000f340: 2060 6048 6173 5265 7175 6972 6564 5472   ``HasRequiredTr
+0000f350: 6169 7473 6060 2063 6c61 7373 0a2a 2042  aits`` class.* B
+0000f360: 6574 7465 7220 4950 7974 686f 6e20 7461  etter IPython ta
+0000f370: 6220 636f 6d70 6c65 7469 6f6e 2066 6f72  b completion for
+0000f380: 2060 6048 6173 5472 6169 7473 6060 2073   ``HasTraits`` s
+0000f390: 7562 636c 6173 7365 730a 0a43 6861 6e67  ubclasses..Chang
+0000f3a0: 6573 2073 756d 6d61 7279 2073 696e 6365  es summary since
+0000f3b0: 2034 2e36 2e30 0a7e 7e7e 7e7e 7e7e 7e7e   4.6.0.~~~~~~~~~
+0000f3c0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+0000f3d0: 7e7e 0a0a 456e 6861 6e63 656d 656e 7473  ~~..Enhancements
+0000f3e0: 0a0a 2a20 4349 2066 6f72 2064 6f63 756d  ..* CI for docum
+0000f3f0: 656e 7461 7469 6f6e 2028 2334 3331 290a  entation (#431).
+0000f400: 2a20 5265 6d6f 7665 2032 746f 3320 6669  * Remove 2to3 fi
+0000f410: 7865 7273 2028 2334 3330 290a 2a20 456e  xers (#430).* En
+0000f420: 7468 6f75 6768 7420 5370 6869 6e78 2054  thought Sphinx T
+0000f430: 6865 6d65 2066 6f72 2064 6f63 7320 2823  heme for docs (#
+0000f440: 3432 3729 0a2a 204e 6577 2060 6048 6173  427).* New ``Has
+0000f450: 5265 7175 6972 6564 5472 6169 7473 6060  RequiredTraits``
+0000f460: 2063 6c61 7373 2028 2334 3139 290a 2a20   class (#419).* 
+0000f470: 4672 6565 2060 6048 6173 5472 6169 7473  Free ``HasTraits
+0000f480: 6060 2073 7562 636c 6173 7365 7320 6672  `` subclasses fr
+0000f490: 6f6d 2068 6173 6869 6e67 2f63 6f6d 7061  om hashing/compa
+0000f4a0: 7269 6e67 2062 7920 6964 656e 7469 7479  ring by identity
+0000f4b0: 2028 2334 3130 290a 2a20 556e 6966 7920   (#410).* Unify 
+0000f4c0: 616e 6420 6669 7820 6465 6661 756c 7420  and fix default 
+0000f4d0: 6c69 7374 2065 6469 746f 7273 2028 2333  list editors (#3
+0000f4e0: 3936 290a 2a20 4164 6420 6060 5f5f 6469  96).* Add ``__di
+0000f4f0: 725f 5f60 6020 6d65 7468 6f64 2074 6f20  r__`` method to 
+0000f500: 6060 4861 7354 7261 6974 7360 6020 666f  ``HasTraits`` fo
+0000f510: 7220 4950 7974 686f 6e20 7461 6220 636f  r IPython tab co
+0000f520: 6d70 6c65 7469 6f6e 2028 2333 3832 290a  mpletion (#382).
+0000f530: 2a20 5079 7468 6f6e 2033 2063 6f6d 7061  * Python 3 compa
+0000f540: 7469 6269 6c69 7479 2066 6978 6573 2028  tibility fixes (
+0000f550: 2333 3734 290a 2a20 4e65 7720 636f 6e74  #374).* New cont
+0000f560: 6578 7420 6d61 6e61 6765 7220 666f 7220  ext manager for 
+0000f570: 7365 7474 696e 6720 7472 6169 742d 6368  setting trait-ch
+0000f580: 616e 6765 2d65 7665 6e74 2074 7261 6365  ange-event trace
+0000f590: 7220 2823 3336 3529 0a2a 2044 6566 6175  r (#365).* Defau
+0000f5a0: 6c74 2074 7261 6974 2074 7970 6520 636f  lt trait type co
+0000f5b0: 6e73 7461 6e74 7320 2823 3335 3429 0a0a  nstants (#354)..
+0000f5c0: 4368 616e 6765 730a 0a2a 2052 656d 6f76  Changes..* Remov
+0000f5d0: 6520 6465 7072 6563 6174 6564 2060 6074  e deprecated ``t
+0000f5e0: 7261 6974 732e 7072 6f74 6f63 6f6c 7360  raits.protocols`
+0000f5f0: 6020 7375 626d 6f64 756c 6520 616e 6420  ` submodule and 
+0000f600: 7265 6c61 7465 6420 7574 696c 7320 2823  related utils (#
+0000f610: 3433 3529 0a2a 2046 6978 2069 6e76 616c  435).* Fix inval
+0000f620: 6964 2073 7472 696e 6720 6573 6361 7065  id string escape
+0000f630: 7320 2823 3432 3929 0a2a 2041 7070 6c79  s (#429).* Apply
+0000f640: 2074 6865 2022 626c 6163 6b22 2063 6f64   the "black" cod
+0000f650: 6520 7265 666f 726d 6174 7469 6e67 2075  e reformatting u
+0000f660: 7469 6c69 7479 206f 6e20 7468 6520 5472  tility on the Tr
+0000f670: 6169 7473 2063 6f64 6562 6173 6520 2823  aits codebase (#
+0000f680: 3433 3229 0a2a 2055 7064 6174 6520 4349  432).* Update CI
+0000f690: 2074 6f20 7573 6520 6564 6d20 616e 6420   to use edm and 
+0000f6a0: 6574 7374 6f6f 6c20 6d6f 6475 6c65 2028  etstool module (
+0000f6b0: 2334 3230 290a 2a20 436c 6561 6e20 7570  #420).* Clean up
+0000f6c0: 2060 6046 6c6f 6174 6060 2061 6e64 2060   ``Float`` and `
+0000f6d0: 6042 6173 6546 6c6f 6174 6060 2076 616c  `BaseFloat`` val
+0000f6e0: 6964 6174 696f 6e20 2823 3339 3329 0a2a  idation (#393).*
+0000f6f0: 204d 6572 6765 206d 6173 7465 7220 696e   Merge master in
+0000f700: 746f 2043 7974 686f 6e20 706f 7274 2028  to Cython port (
+0000f710: 2333 3730 290a 2a20 446f 6373 2061 6e64  #370).* Docs and
+0000f720: 206d 696e 6f72 2072 6566 6163 746f 7269   minor refactori
+0000f730: 6e67 206f 6620 6060 4d65 7461 4861 7354  ng of ``MetaHasT
+0000f740: 7261 6974 7360 6020 636c 6173 7320 2823  raits`` class (#
+0000f750: 3336 3629 0a2a 2052 656d 6f76 6520 7269  366).* Remove ri
+0000f760: 6469 6375 6c6f 7573 2070 7265 6d61 7475  diculous prematu
+0000f770: 7265 206f 7074 696d 697a 6174 696f 6e20  re optimization 
+0000f780: 2823 3336 3229 0a2a 2041 6464 2073 7570  (#362).* Add sup
+0000f790: 706f 7274 2066 6f72 2050 7949 6e73 7461  port for PyInsta
+0000f7a0: 6c6c 6572 2061 7070 2062 756e 646c 6572  ller app bundler
+0000f7b0: 2028 2333 3631 290a 2a20 4164 6420 6465   (#361).* Add de
+0000f7c0: 7363 7269 7074 696f 6e20 616e 6420 6578  scription and ex
+0000f7d0: 616d 706c 6520 666f 7220 6060 4569 7468  ample for ``Eith
+0000f7e0: 6572 6060 2074 7261 6974 2074 7970 6520  er`` trait type 
+0000f7f0: 2823 3336 3029 0a2a 2044 726f 7020 7375  (#360).* Drop su
+0000f800: 7070 6f72 7420 666f 7220 5079 7468 6f6e  pport for Python
+0000f810: 2032 2e36 2061 6e64 2050 7974 686f 6e20   2.6 and Python 
+0000f820: 3c20 332e 3420 2823 3334 3529 0a2a 2041  < 3.4 (#345).* A
+0000f830: 6464 206d 616b 6520 7461 7267 6574 2066  dd make target f
+0000f840: 6f72 2064 6f63 7365 7420 746f 2062 6520  or docset to be 
+0000f850: 7573 6564 2077 6974 6820 4461 7368 2f5a  used with Dash/Z
+0000f860: 6561 6c20 2823 3138 3029 0a0a 4669 7865  eal (#180)..Fixe
+0000f870: 730a 0a2a 2046 6978 206f 6464 2065 7272  s..* Fix odd err
+0000f880: 6f72 206d 6573 7361 6765 2061 6e64 2077  or message and w
+0000f890: 726f 6e67 2065 7863 6570 7469 6f6e 2074  rong exception t
+0000f8a0: 7970 6520 2823 3432 3629 0a2a 2046 6978  ype (#426).* Fix
+0000f8b0: 2043 6f6c 6f72 2061 6e64 2052 4742 436f   Color and RGBCo
+0000f8c0: 6c6f 7220 646f 6320 7374 7269 6e67 7320  lor doc strings 
+0000f8d0: 2823 3431 3729 0a2a 2046 6978 2075 7365  (#417).* Fix use
+0000f8e0: 206f 6620 6465 7072 6563 6172 6564 2060   of deprecared `
+0000f8f0: 6069 6e73 7065 6374 2e67 6574 6172 6773  `inspect.getargs
+0000f900: 7065 6360 6020 6675 6e63 7469 6f6e 2028  pec`` function (
+0000f910: 2334 3038 290a 2a20 4669 7820 6578 7465  #408).* Fix exte
+0000f920: 6e64 6564 206e 616d 6573 2069 6e20 6060  nded names in ``
+0000f930: 6f6e 5f74 7261 6974 5f63 6861 6e67 6560  on_trait_change`
+0000f940: 6020 6c69 7374 7320 2823 3430 3429 0a2a  ` lists (#404).*
+0000f950: 2053 7570 706f 7274 2055 6e69 636f 6465   Support Unicode
+0000f960: 206f 6e20 7472 6169 7420 646f 6375 6d65   on trait docume
+0000f970: 6e74 6572 206f 6e20 5079 7468 6f6e 2032  nter on Python 2
+0000f980: 2e37 2028 2333 3836 290a 2a20 436c 6561  .7 (#386).* Clea
+0000f990: 7220 6578 6365 7074 696f 6e20 6672 6f6d  r exception from
+0000f9a0: 204e 756d 7079 2070 726f 7065 726c 7920   Numpy properly 
+0000f9b0: 2823 3337 3729 0a2a 2046 6978 2070 6963  (#377).* Fix pic
+0000f9c0: 6b6c 696e 6720 616e 6420 6465 6570 636f  kling and deepco
+0000f9d0: 7079 696e 6720 6275 6720 7769 7468 2064  pying bug with d
+0000f9e0: 796e 616d 6963 616c 6c79 2061 6464 6564  ynamically added
+0000f9f0: 2074 7261 6974 7320 2823 3337 3329 0a2a   traits (#373).*
+0000fa00: 2053 6574 2060 6061 7574 6f5f 7365 742f   Set ``auto_set/
+0000fa10: 656e 7465 725f 7365 7460 6020 6465 6661  enter_set`` defa
+0000fa20: 756c 7420 6f6e 6365 2028 2333 3731 290a  ult once (#371).
+0000fa30: 2a20 4669 7820 7661 6c69 6461 7469 6f6e  * Fix validation
+0000fa40: 206f 6620 6060 5468 6973 6060 2074 7261   of ``This`` tra
+0000fa50: 6974 2028 2333 3533 290a 2a20 4d61 6b65  it (#353).* Make
+0000fa60: 2060 6063 5472 6169 742e 6465 6661 756c   ``cTrait.defaul
+0000fa70: 745f 7661 6c75 655f 666f 7260 6020 7261  t_value_for`` ra
+0000fa80: 6973 6520 6120 6060 5661 6c75 6545 7272  ise a ``ValueErr
+0000fa90: 6f72 6060 2069 6e73 7465 6164 206f 660a  or`` instead of.
+0000faa0: 2020 7365 6720 6661 756c 7469 6e67 2077    seg faulting w
+0000fab0: 6865 6e20 6173 6b65 6420 666f 7220 7468  hen asked for th
+0000fac0: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+0000fad0: 6f66 2061 2074 7261 6974 2074 6861 7420  of a trait that 
+0000fae0: 646f 6573 6e27 740a 2020 6861 7665 206f  doesn't.  have o
+0000faf0: 6e65 2e20 2823 3335 3029 0a2a 2046 6978  ne. (#350).* Fix
+0000fb00: 206d 6973 7573 6520 6f66 2060 6075 6e69   misuse of ``uni
+0000fb10: 7474 6573 742e 6578 7065 6374 6564 4661  ttest.expectedFa
+0000fb20: 696c 7572 6560 6020 6465 636f 7261 746f  ilure`` decorato
+0000fb30: 7220 2823 3334 3629 0a2a 2046 6978 2069  r (#346).* Fix i
+0000fb40: 7373 7565 2077 6974 6820 6f76 6572 7269  ssue with overri
+0000fb50: 6464 656e 2060 6048 6173 5472 6169 7473  dden ``HasTraits
+0000fb60: 2e74 7261 6974 6060 2066 756e 6374 696f  .trait`` functio
+0000fb70: 6e20 2823 3334 3329 0a0a 0a52 656c 6561  n (#343)...Relea
+0000fb80: 7365 2034 2e36 2e30 0a2d 2d2d 2d2d 2d2d  se 4.6.0.-------
+0000fb90: 2d2d 2d2d 2d2d 0a0a 5468 6973 2069 7320  ------..This is 
+0000fba0: 616e 2069 6e63 7265 6d65 6e74 616c 2072  an incremental r
+0000fbb0: 656c 6561 7365 206f 7665 7220 342e 352c  elease over 4.5,
+0000fbc0: 2061 6363 756d 756c 6174 696e 6720 6f76   accumulating ov
+0000fbd0: 6572 2061 2079 6561 7227 7320 776f 7274  er a year's wort
+0000fbe0: 6820 6f66 0a62 7567 6669 7865 7320 616e  h of.bugfixes an
+0000fbf0: 6420 736d 616c 6c20 696d 7072 6f76 656d  d small improvem
+0000fc00: 656e 7473 2074 6f20 7468 6520 636f 6465  ents to the code
+0000fc10: 2e0a 0a48 6967 686c 6967 6874 7320 6f66  ...Highlights of
+0000fc20: 2074 6869 7320 7265 6c65 6173 6520 696e   this release in
+0000fc30: 636c 7564 653a 0a0a 2a20 7375 7070 6f72  clude:..* suppor
+0000fc40: 7420 666f 7220 5079 7468 6f6e 2033 2e34  t for Python 3.4
+0000fc50: 2061 6e64 2033 2e35 2e0a 2a20 6e65 7720   and 3.5..* new 
+0000fc60: 4279 7465 7320 616e 6420 5661 6c69 6461  Bytes and Valida
+0000fc70: 7465 6454 7570 6c65 2074 7261 6974 732e  tedTuple traits.
+0000fc80: 0a2a 2061 206e 6577 2041 7272 6179 4f72  .* a new ArrayOr
+0000fc90: 4e6f 6e65 2074 7261 6974 2077 6869 6368  None trait which
+0000fca0: 2063 6f72 7265 6374 6c79 2068 616e 646c   correctly handl
+0000fcb0: 6573 204e 6f6e 6520 636f 6d70 6172 6973  es None comparis
+0000fcc0: 6f6e 7320 7769 7468 204e 756d 7079 0a20  ons with Numpy. 
+0000fcd0: 2061 7272 6179 732e 0a2a 2063 6c65 616e   arrays..* clean
+0000fce0: 2d75 7020 6f66 2074 6865 2045 5453 436f  -up of the ETSCo
+0000fcf0: 6e66 6967 2063 6f64 6520 666f 7220 5472  nfig code for Tr
+0000fd00: 6169 7473 5549 2074 6f6f 6c6b 6974 2073  aitsUI toolkit s
+0000fd10: 656c 6563 7469 6f6e 2e0a 2a20 6265 7474  election..* bett
+0000fd20: 6572 2063 6f6d 7061 7469 6269 6c69 7479  er compatibility
+0000fd30: 2077 6974 6820 4e75 6d50 7920 7363 616c   with NumPy scal
+0000fd40: 6172 2074 7970 6573 2e0a 2a20 6d61 6e79  ar types..* many
+0000fd50: 206f 7468 6572 2062 7567 6669 7865 7320   other bugfixes 
+0000fd60: 616e 6420 696d 7072 6f76 656d 656e 7473  and improvements
+0000fd70: 2e0a 0a43 6861 6e67 6520 7375 6d6d 6172  ...Change summar
+0000fd80: 7920 7369 6e63 6520 342e 352e 300a 7e7e  y since 4.5.0.~~
+0000fd90: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+0000fda0: 7e7e 7e7e 7e7e 7e7e 0a0a 456e 6861 6e63  ~~~~~~~~..Enhanc
+0000fdb0: 656d 656e 7473 0a0a 2a20 4164 6465 6420  ements..* Added 
+0000fdc0: 6120 6060 4279 7465 7360 6020 5472 6169  a ``Bytes`` Trai
+0000fdd0: 7420 616e 6420 7265 6c61 7465 6420 7472  t and related tr
+0000fde0: 6169 7473 2028 2333 3239 290a 2a20 4164  aits (#329).* Ad
+0000fdf0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+0000fe00: 6669 6e64 696e 6720 7265 736f 7572 6365  finding resource
+0000fe10: 7320 6672 6f6d 207a 6970 7065 6420 5079  s from zipped Py
+0000fe20: 7468 6f6e 2073 6f75 7263 6520 636f 6465  thon source code
+0000fe30: 2028 2333 3136 290a 2a20 4164 6465 6420   (#316).* Added 
+0000fe40: 696e 2d70 6c61 6365 2073 6574 2061 7269  in-place set ari
+0000fe50: 7468 6d65 7469 6320 6f70 6572 6174 696f  thmetic operatio
+0000fe60: 6e73 2066 6f72 2060 6054 7261 6974 5365  ns for ``TraitSe
+0000fe70: 744f 626a 6563 7460 6073 2061 6e64 2061  tObject``s and a
+0000fe80: 6363 6570 740a 2020 6d61 7463 6820 6265  ccept.  match be
+0000fe90: 6861 7669 6f75 7220 6f66 2060 6054 7261  haviour of ``Tra
+0000fea0: 6974 5365 744f 626a 6563 7460 6020 7769  itSetObject`` wi
+0000feb0: 7468 2072 6567 756c 6172 2050 7974 686f  th regular Pytho
+0000fec0: 6e20 7365 7473 2077 6865 6e0a 2020 7065  n sets when.  pe
+0000fed0: 7266 6f72 6d69 6e67 206f 7065 7261 7469  rforming operati
+0000fee0: 6f6e 7320 7769 7468 206e 6f6e 2d73 6574  ons with non-set
+0000fef0: 2074 7970 6573 2028 6567 2e20 6c69 7374   types (eg. list
+0000ff00: 732c 2064 6963 7469 6f6e 6172 6965 7329  s, dictionaries)
+0000ff10: 2028 2332 3839 290a 2a20 4164 6465 6420   (#289).* Added 
+0000ff20: 6120 636f 6e74 6578 7420 6d61 6e61 6765  a context manage
+0000ff30: 7220 746f 2061 6c6c 6f77 2070 726f 7669  r to allow provi
+0000ff40: 7369 6f6e 616c 2073 656c 6563 7469 6f6e  sional selection
+0000ff50: 206f 6620 6120 746f 6f6c 6b69 7420 746f   of a toolkit to
+0000ff60: 0a20 2060 6045 5453 436f 6e66 6967 6060  .  ``ETSConfig``
+0000ff70: 2028 7468 6973 2067 656e 6572 616c 6c79   (this generally
+0000ff80: 2069 6d70 726f 7665 7320 7265 6c69 6162   improves reliab
+0000ff90: 696c 6974 7920 6f66 2074 6f6f 6c6b 6974  ility of toolkit
+0000ffa0: 2073 656c 6563 7469 6f6e 0a20 2066 6f72   selection.  for
+0000ffb0: 2050 7966 6163 6520 616e 6420 5472 6169   Pyface and Trai
+0000ffc0: 7473 5549 292e 2028 2332 3736 290a 2a20  tsUI). (#276).* 
+0000ffd0: 4164 6465 6420 5472 6169 7420 6368 616e  Added Trait chan
+0000ffe0: 6765 2072 6563 6f72 6465 7220 746f 2061  ge recorder to a
+0000fff0: 6964 2069 6e20 6465 6275 6767 696e 6720  id in debugging 
+00010000: 6576 656e 742d 6472 6976 656e 2063 6f64  event-driven cod
+00010010: 652e 2028 2331 3339 290a 2a20 6060 5f5f  e. (#139).* ``__
+00010020: 6961 6464 5f5f 6060 2061 6e64 2060 605f  iadd__`` and ``_
+00010030: 5f69 6d75 6c5f 5f60 6020 696d 706c 656d  _imul__`` implem
+00010040: 656e 7465 6420 6f6e 2054 7261 6974 4c69  ented on TraitLi
+00010050: 7374 4f62 6a65 6374 732e 2028 2331 3635  stObjects. (#165
+00010060: 290a 2a20 4164 6465 6420 6e65 7720 6060  ).* Added new ``
+00010070: 4172 7261 794f 724e 6f6e 6560 6020 7472  ArrayOrNone`` tr
+00010080: 6169 7420 7479 7065 2074 6f20 7265 706c  ait type to repl
+00010090: 6163 6520 7468 650a 2020 6060 4569 7468  ace the.  ``Eith
+000100a0: 6572 284e 6f6e 652c 2041 7272 6179 2960  er(None, Array)`
+000100b0: 6020 6964 696f 6d2e 2020 5468 6520 6f6c  ` idiom.  The ol
+000100c0: 6420 6964 696f 6d20 7265 7375 6c74 7320  d idiom results 
+000100d0: 696e 2077 6172 6e69 6e67 730a 2020 6f6e  in warnings.  on
+000100e0: 204e 756d 5079 203e 3d20 312e 392e 2028   NumPy >= 1.9. (
+000100f0: 2332 3139 290a 2a20 4164 6465 6420 6120  #219).* Added a 
+00010100: 6e65 7720 6060 5661 6c69 6461 7465 6454  new ``ValidatedT
+00010110: 7570 6c65 6060 2074 7261 6974 2074 6861  uple`` trait tha
+00010120: 7420 7375 7070 6f72 7473 2063 7573 746f  t supports custo
+00010130: 6d20 7661 6c69 6461 7469 6f6e 2e20 2823  m validation. (#
+00010140: 3230 3529 0a0a 4368 616e 6765 730a 0a2a  205)..Changes..*
+00010150: 2052 656d 6f76 6564 2072 6564 756e 6461   Removed redunda
+00010160: 6e74 2c20 696e 7465 726e 616c 2060 6045  nt, internal ``E
+00010170: 5453 436f 6e66 6967 6060 2066 726f 6d20  TSConfig`` from 
+00010180: 5472 6169 7473 2063 6f64 6562 6173 652e  Traits codebase.
+00010190: 2028 2333 3237 290a 2a20 4265 7474 6572   (#327).* Better
+000101a0: 2065 7272 6f72 2072 6570 6f72 7469 6e67   error reporting
+000101b0: 2066 6f72 2066 6169 6c65 6420 6174 7472   for failed attr
+000101c0: 6962 7574 6520 6163 6365 7373 2e20 2823  ibute access. (#
+000101d0: 3234 3329 0a2a 2052 656d 6f76 6564 2062  243).* Removed b
+000101e0: 7567 6779 2060 602d 746f 6f6c 6b69 7460  uggy ``-toolkit`
+000101f0: 6020 636f 6d6d 616e 646c 696e 6520 6f70  ` commandline op
+00010200: 7469 6f6e 2060 6045 5453 436f 6e66 6967  tion ``ETSConfig
+00010210: 6060 2e20 2823 3332 3629 0a2a 2052 656d  ``. (#326).* Rem
+00010220: 6f76 6564 2062 7567 6779 2060 602a 6e61  oved buggy ``*na
+00010230: 6d65 7360 6020 706f 7369 7469 6f6e 616c  mes`` positional
+00010240: 2061 7267 756d 656e 7473 2066 726f 6d20   arguments from 
+00010250: 6060 6f6e 5f74 7261 6974 5f63 6861 6e67  ``on_trait_chang
+00010260: 6560 600a 2020 6465 636f 7261 746f 7220  e``.  decorator 
+00010270: 696e 2069 6d70 726f 7665 6420 6172 6775  in improved argu
+00010280: 6d65 6e74 2070 6173 7369 6e67 2028 2332  ment passing (#2
+00010290: 3037 292e 0a2a 2041 6c6c 6f77 2060 6046  07)..* Allow ``F
+000102a0: 6c6f 6174 6060 2061 6e64 2060 6042 6173  loat`` and ``Bas
+000102b0: 6546 6c6f 6174 6060 2074 7261 6974 7320  eFloat`` traits 
+000102c0: 746f 2061 6363 6570 7420 5079 7468 6f6e  to accept Python
+000102d0: 206c 6f6e 6773 2e20 2823 3237 3229 0a2a   longs. (#272).*
+000102e0: 2043 6c65 616e 2d75 7020 616e 6420 6669   Clean-up and fi
+000102f0: 7865 7320 746f 2065 7861 6d70 6c65 2063  xes to example c
+00010300: 6f64 652e 2028 2331 3236 290a 2a20 5265  ode. (#126).* Re
+00010310: 6d6f 7665 206f 7574 6461 7465 6420 6060  move outdated ``
+00010320: 496d 706f 7274 5370 7960 6020 616e 6420  ImportSpy`` and 
+00010330: 6060 496d 706f 7274 4d61 6e61 6765 7260  ``ImportManager`
+00010340: 6020 7574 696c 6974 6965 732e 2028 2331  ` utilities. (#1
+00010350: 3838 290a 2a20 5468 6520 6060 6465 7072  88).* The ``depr
+00010360: 6563 6174 6564 6060 2064 6563 6f72 6174  ecated`` decorat
+00010370: 6f72 206e 6f77 2069 7373 7565 7320 6120  or now issues a 
+00010380: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
+00010390: 6e67 2028 7573 696e 670a 2020 7468 6520  ng (using.  the 
+000103a0: 5079 7468 6f6e 2060 6077 6172 6e69 6e67  Python ``warning
+000103b0: 7360 6020 6d6f 6475 6c65 2920 7261 7468  s`` module) rath
+000103c0: 6572 2074 6861 6e20 6c6f 6767 696e 6720  er than logging 
+000103d0: 6120 7761 726e 696e 6720 7669 610a 2020  a warning via.  
+000103e0: 7468 6520 6060 6c6f 6767 696e 6760 6020  the ``logging`` 
+000103f0: 6d61 6368 696e 6572 792e 2020 4974 206e  machinery.  It n
+00010400: 6f20 6c6f 6e67 6572 2074 7269 6573 2074  o longer tries t
+00010410: 6f20 7265 6d65 6d62 6572 2077 6865 6e0a  o remember when.
+00010420: 2020 6120 7761 726e 696e 6720 6861 7320    a warning has 
+00010430: 6265 656e 2070 7265 7669 6f75 736c 7920  been previously 
+00010440: 6973 7375 6564 2e20 2823 3232 3029 0a2a  issued. (#220).*
+00010450: 2044 6570 7265 6361 7465 6420 6060 4861   Deprecated ``Ha
+00010460: 7354 7261 6974 732e 6765 7428 2960 6020  sTraits.get()`` 
+00010470: 616e 6420 6060 4861 7354 7261 6974 732e  and ``HasTraits.
+00010480: 7365 7428 2960 6020 2823 3139 3029 2e0a  set()`` (#190)..
+00010490: 2a20 5468 6520 6465 6661 756c 7420 6060  * The default ``
+000104a0: 5669 6577 6060 2073 686f 7773 2061 6c6c  View`` shows all
+000104b0: 2028 6e6f 6e2d 6576 656e 7429 2074 7261   (non-event) tra
+000104c0: 6974 7320 7768 6f73 6520 6060 7669 7369  its whose ``visi
+000104d0: 626c 6560 6020 7072 6f70 6572 7479 0a20  ble`` property. 
+000104e0: 2069 7320 6e6f 7420 6060 4661 6c73 6560   is not ``False`
+000104f0: 602e 2050 7269 7661 7465 2074 7261 6974  `. Private trait
+00010500: 7320 6172 6520 7365 7420 6060 7669 7369  s are set ``visi
+00010510: 626c 653d 4661 6c73 6560 6020 6279 2064  ble=False`` by d
+00010520: 6566 6175 6c74 2e20 2823 3233 3429 0a0a  efault. (#234)..
+00010530: 4669 7865 730a 0a2a 2046 6978 2042 6f6f  Fixes..* Fix Boo
+00010540: 6c20 7472 6169 7473 2073 6f20 7468 6174  l traits so that
+00010550: 2076 616c 7565 2073 746f 7265 6420 6973   value stored is
+00010560: 2061 6c77 6179 7320 6120 5079 7468 6f6e   always a Python
+00010570: 2060 6062 6f6f 6c60 6020 2861 6e64 2069   ``bool`` (and i
+00010580: 6e0a 2020 7061 7274 6963 756c 6172 2c20  n.  particular, 
+00010590: 6e6f 7420 6120 4e75 6d50 7920 6060 6e70  not a NumPy ``np
+000105a0: 2e62 6f6f 6c5f 6060 292e 2028 2333 3138  .bool_``). (#318
+000105b0: 290a 2a20 4669 7820 426f 6f6c 2074 7261  ).* Fix Bool tra
+000105c0: 6974 7320 736f 2074 6861 7420 7265 6775  its so that regu
+000105d0: 6c61 7220 7661 6c69 6461 746f 7220 6163  lar validator ac
+000105e0: 6365 7074 7320 4e75 6d70 5079 2773 2060  cepts NumpPy's `
+000105f0: 606e 702e 626f 6f6c 5f60 600a 2020 626f  `np.bool_``.  bo
+00010600: 6f6c 6561 6e20 7661 6c75 6573 2028 6272  olean values (br
+00010610: 696e 6769 6e67 2069 7420 696e 2061 6772  inging it in agr
+00010620: 6565 6d65 6e74 2077 6974 6820 7468 6520  eement with the 
+00010630: 6661 7374 2076 616c 6964 6174 6f72 292e  fast validator).
+00010640: 2028 2333 3032 290a 2a20 4669 7820 7573   (#302).* Fix us
+00010650: 6520 6f66 2060 606e 6578 7460 6020 696e  e of ``next`` in
+00010660: 2060 6054 7261 6974 446f 6375 6d65 6e74   ``TraitDocument
+00010670: 6572 6060 2066 6f72 2050 7974 686f 6e20  er`` for Python 
+00010680: 3320 636f 6d70 6174 6962 696c 6974 792e  3 compatibility.
+00010690: 2028 2332 3933 290a 2a20 4669 7820 6f66   (#293).* Fix of
+000106a0: 662d 6279 2d6f 6e65 2065 7272 6f72 2077  f-by-one error w
+000106b0: 6865 6e20 6060 5472 6169 744c 6973 744f  hen ``TraitListO
+000106c0: 626a 6563 7460 6020 6973 2073 6574 7469  bject`` is setti
+000106d0: 6e67 206f 7220 6465 6c65 7469 6e67 2073  ng or deleting s
+000106e0: 6c69 6365 732e 0a20 2028 2332 3833 290a  lices..  (#283).
+000106f0: 2a20 4669 7820 7265 6665 7265 6e63 6520  * Fix reference 
+00010700: 6379 636c 6573 2063 6175 7365 6420 6279  cycles caused by
+00010710: 2060 6073 796e 635f 7472 6169 7473 6060   ``sync_traits``
+00010720: 2e20 2823 3133 3529 0a2a 2046 6978 2073  . (#135).* Fix s
+00010730: 6f20 7468 6174 2060 6073 7973 2e65 7863  o that ``sys.exc
+00010740: 5f69 6e66 6f28 2960 6020 776f 726b 7320  _info()`` works 
+00010750: 6173 2065 7870 6563 7465 6420 696e 2065  as expected in e
+00010760: 7863 6570 7469 6f6e 2068 616e 646c 6572  xception handler
+00010770: 7320 696e 0a20 2050 7974 686f 6e20 3320  s in.  Python 3 
+00010780: 2823 3236 3629 0a2a 2046 6978 2060 6053  (#266).* Fix ``S
+00010790: 7472 696e 6760 6020 7472 6169 7420 746f  tring`` trait to
+000107a0: 2061 6363 6570 7420 6060 7374 7260 6020   accept ``str`` 
+000107b0: 7375 6263 6c61 7373 6573 2028 6c69 6b65  subclasses (like
+000107c0: 2060 606e 756d 7079 2e73 7472 5f60 6029   ``numpy.str_``)
+000107d0: 2e0a 2020 2823 3236 3729 0a2a 2046 6978  ..  (#267).* Fix
+000107e0: 6564 2069 6e63 6f72 7265 6374 2069 6e20  ed incorrect in 
+000107f0: 6c69 7374 2065 7665 6e74 7320 666f 7220  list events for 
+00010800: 6060 696e 7365 7274 6060 206f 7065 7261  ``insert`` opera
+00010810: 7469 6f6e 7320 7769 7468 2061 6e20 696e  tions with an in
+00010820: 6465 780a 2020 6f75 7473 6964 6520 7468  dex.  outside th
+00010830: 6520 7261 6e67 6520 5b60 602d 6c65 6e28  e range [``-len(
+00010840: 7461 7267 6574 5f6c 6973 7429 6060 2c20  target_list)``, 
+00010850: 6060 6c65 6e28 7461 7267 6574 5f6c 6973  ``len(target_lis
+00010860: 7429 6060 5d2e 2028 2331 3635 290a 2a20  t)``]. (#165).* 
+00010870: 4669 7820 696e 636f 7272 6563 7420 6265  Fix incorrect be
+00010880: 6861 7669 6f75 7220 6f66 2060 6063 6865  haviour of ``che
+00010890: 636b 5f69 6d70 6c65 6d65 6e74 7360 6020  ck_implements`` 
+000108a0: 666f 7220 6f76 6572 7269 6464 656e 206d  for overridden m
+000108b0: 6574 686f 6473 2e0a 2020 2823 3139 3229  ethods..  (#192)
+000108c0: 0a2a 2046 6978 2065 7272 6f72 2077 6865  .* Fix error whe
+000108d0: 6e20 7472 7969 6e67 2074 6f20 6c69 7374  n trying to list
+000108e0: 656e 2074 6f20 7472 6169 7473 2075 7369  en to traits usi
+000108f0: 6e67 206c 6973 7420 6272 6163 6b65 7420  ng list bracket 
+00010900: 6e6f 7461 7469 6f6e 2e20 2823 3139 3529  notation. (#195)
+00010910: 0a2a 2046 6978 2072 6566 6572 656e 6365  .* Fix reference
+00010920: 206c 6561 6b20 696e 2060 6043 4861 7354   leak in ``CHasT
+00010930: 7261 6974 732e 5f6e 6f74 6966 6965 7273  raits._notifiers
+00010940: 6060 2e20 2823 3234 3829 0a2a 2046 6978  ``. (#248).* Fix
+00010950: 2072 6566 6572 656e 6365 206c 6561 6b20   reference leak 
+00010960: 6672 6f6d 2075 7365 206f 6620 6060 4465  from use of ``De
+00010970: 6c65 6761 7465 7354 6f60 602e 2028 2332  legatesTo``. (#2
+00010980: 3630 290a 2a20 496e 7374 616e 6365 2074  60).* Instance t
+00010990: 7261 6974 7320 7765 7265 6e27 7420 696e  raits weren't in
+000109a0: 636c 7564 6564 2069 6e20 7468 6520 7265  cluded in the re
+000109b0: 7375 6c74 206f 6620 6060 7472 6169 7473  sult of ``traits
+000109c0: 2829 6060 2e20 2823 3233 3429 0a0a 0a52  ()``. (#234)...R
+000109d0: 656c 6561 7365 2034 2e35 2e30 0a2d 2d2d  elease 4.5.0.---
+000109e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5472 6169  ----------..Trai
+000109f0: 7473 2069 7320 6e6f 7720 636f 6d70 6174  ts is now compat
+00010a00: 6962 6c65 2077 6974 6820 5079 7468 6f6e  ible with Python
+00010a10: 2033 2120 5468 6520 6c69 6272 6172 7920   3! The library 
+00010a20: 6e6f 7720 7375 7070 6f72 7473 0a50 7974  now supports.Pyt
+00010a30: 686f 6e20 332e 3220 616e 6420 332e 332e  hon 3.2 and 3.3.
+00010a40: 0a0a 5468 6520 7265 6c65 6173 6520 616c  ..The release al
+00010a50: 736f 2069 6e63 6c75 6465 7320 696e 6372  so includes incr
+00010a60: 6561 7365 6420 636f 6465 2063 6f76 6572  eased code cover
+00010a70: 6167 6520 616e 6420 6175 746f 6d61 7469  age and automati
+00010a80: 630a 636f 7665 7261 6765 2072 6570 6f72  c.coverage repor
+00010a90: 7420 7468 726f 7567 6820 636f 7665 7261  t through covera
+00010aa0: 6c6c 732e 696f 2e0a 0a0a 4368 616e 6765  lls.io....Change
+00010ab0: 2073 756d 6d61 7279 2073 696e 6365 2034   summary since 4
+00010ac0: 2e34 2e30 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  .4.0.~~~~~~~~~~~
+00010ad0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
+00010ae0: 0a45 6e68 616e 6365 6d65 6e74 730a 0a2a  .Enhancements..*
+00010af0: 2054 6573 7420 6669 6c65 7320 636c 6561   Test files clea
+00010b00: 6e75 7073 2028 2331 3038 2c20 2331 3131  nups (#108, #111
+00010b10: 2c20 2331 3231 290a 2a20 4164 6420 6175  , #121).* Add au
+00010b20: 746f 6d61 7469 6320 636f 7665 7261 6765  tomatic coverage
+00010b30: 2072 6570 6f72 7473 2028 2331 3130 2c20   reports (#110, 
+00010b40: 2331 3232 290a 2a20 5265 6d6f 7665 6420  #122).* Removed 
+00010b50: 6f62 736f 6c65 7465 2063 6f64 6520 2823  obsolete code (#
+00010b60: 3130 392c 2023 3131 322c 2023 3131 3329  109, #112, #113)
+00010b70: 0a2a 2049 6e63 7265 6173 6564 2074 6573  .* Increased tes
+00010b80: 7420 636f 7665 7261 6765 2028 2331 3134  t coverage (#114
+00010b90: 2c20 2331 3138 290a 2a20 5079 7468 6f6e  , #118).* Python
+00010ba0: 2033 2073 7570 706f 7274 2028 2331 3135   3 support (#115
+00010bb0: 292e 2020 5468 616e 6b73 2059 7665 7320  ).  Thanks Yves 
+00010bc0: 4465 6c6c 6579 2e0a 2a20 416c 6c6f 7720  Delley..* Allow 
+00010bd0: 7365 7474 696e 6720 616e 6420 7265 7365  setting and rese
+00010be0: 7474 696e 6720 7468 6520 676c 6f62 616c  tting the global
+00010bf0: 2061 6461 7074 6174 696f 6e20 6d61 6e61   adaptation mana
+00010c00: 6765 7220 2823 3134 3529 0a2a 2056 6172  ger (#145).* Var
+00010c10: 696f 7573 2064 6f63 756d 656e 7461 7469  ious documentati
+00010c20: 6f6e 2069 6d70 726f 7665 6d65 6e74 7320  on improvements 
+00010c30: 2823 3133 322c 2023 3133 332c 2023 3134  (#132, #133, #14
+00010c40: 382c 2023 3135 3429 2e0a 0a43 6861 6e67  8, #154)...Chang
+00010c50: 6573 0a0a 2a20 5468 6520 496e 7420 7472  es..* The Int tr
+00010c60: 6169 7420 7479 7065 206e 6f77 2061 6363  ait type now acc
+00010c70: 6570 7473 2050 7974 686f 6e20 696e 7473  epts Python ints
+00010c80: 202a 616e 642a 2050 7974 686f 6e20 6c6f   *and* Python lo
+00010c90: 6e67 732c 2061 7320 7765 6c6c 2061 730a  ngs, as well as.
+00010ca0: 2020 696e 7374 616e 6365 7320 6f66 2061    instances of a
+00010cb0: 6e79 2050 7974 686f 6e20 7479 7065 2074  ny Python type t
+00010cc0: 6861 7420 696d 706c 656d 656e 7473 2074  hat implements t
+00010cd0: 6865 2060 605f 5f69 6e64 6578 5f5f 6060  he ``__index__``
+00010ce0: 206d 6574 686f 642e 0a20 2050 7265 7669   method..  Previ
+00010cf0: 6f75 736c 792c 206c 6f6e 6720 696e 7374  ously, long inst
+00010d00: 616e 6365 7320 7765 7265 206e 6f74 2061  ances were not a
+00010d10: 6363 6570 7465 642e 2028 2331 3034 2c20  ccepted. (#104, 
+00010d20: 2331 3233 292e 0a0a 4669 7865 730a 0a2a  #123)...Fixes..*
+00010d30: 2046 6978 2063 7261 7368 2077 6865 6e20   Fix crash when 
+00010d40: 7472 7969 6e67 2074 6f20 7661 6c69 6461  trying to valida
+00010d50: 7465 2061 2070 726f 7065 7274 7920 7468  te a property th
+00010d60: 6174 2068 6173 2062 6565 6e20 6465 6c65  at has been dele
+00010d70: 7465 642e 2028 2331 3338 290a 2a20 4669  ted. (#138).* Fi
+00010d80: 7820 636c 6561 7269 6e67 2065 7863 6570  x clearing excep
+00010d90: 7469 6f6e 2077 6865 6e20 7261 6973 696e  tion when raisin
+00010da0: 6720 6120 5472 6169 7445 7272 6f72 2028  g a TraitError (
+00010db0: 2331 3139 290a 2a20 4669 7820 6175 746f  #119).* Fix auto
+00010dc0: 6d61 7469 6320 6164 6170 7461 7469 6f6e  matic adaptation
+00010dd0: 2077 6865 6e20 6173 7369 676e 696e 6720   when assigning 
+00010de0: 746f 204c 6973 7420 7472 6169 7420 2823  to List trait (#
+00010df0: 3134 3729 0a2a 2046 6978 2073 6f6d 6520  147).* Fix some 
+00010e00: 6374 7261 6974 7320 7265 6663 6f75 6e74  ctraits refcount
+00010e10: 696e 6720 616e 6420 6578 6365 7074 696f  ing and exceptio
+00010e20: 6e20 636c 6561 7269 6e67 2062 7567 7320  n clearing bugs 
+00010e30: 2823 3438 292e 2020 5468 616e 6b73 2059  (#48).  Thanks Y
+00010e40: 7665 730a 2020 4465 6c6c 6579 2e0a 0a0a  ves.  Delley....
+00010e50: 5265 6c65 6173 6520 342e 342e 300a 2d2d  Release 4.4.0.--
+00010e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6865  -----------..The
+00010e70: 206d 616a 6f72 206e 6577 2066 6561 7475   major new featu
+00010e80: 7265 2069 6e20 7468 6973 2072 656c 6561  re in this relea
+00010e90: 7365 2069 7320 6120 6e65 7720 6164 6170  se is a new adap
+00010ea0: 7461 7469 6f6e 206d 6563 6861 6e69 736d  tation mechanism
+00010eb0: 2069 6e20 7468 650a 6060 7472 6169 7473   in the.``traits
+00010ec0: 2e61 6461 7074 6174 696f 6e60 6020 7061  .adaptation`` pa
+00010ed0: 636b 6167 652e 2020 5468 6520 6e65 7720  ckage.  The new 
+00010ee0: 6d65 6368 616e 6973 6d20 6973 2069 6e74  mechanism is int
+00010ef0: 656e 6465 6420 746f 2072 6570 6c61 6365  ended to replace
+00010f00: 2074 6865 0a6f 6c64 6572 2074 7261 6974   the.older trait
+00010f10: 732e 7072 6f74 6f63 6f6c 7320 7061 636b  s.protocols pack
+00010f20: 6167 652e 2020 436f 6465 2077 7269 7474  age.  Code writt
+00010f30: 656e 2061 6761 696e 7374 2060 6074 7261  en against ``tra
+00010f40: 6974 732e 7072 6f74 6f63 6f6c 7360 6020  its.protocols`` 
+00010f50: 7769 6c6c 0a63 6f6e 7469 6e75 6520 746f  will.continue to
+00010f60: 2077 6f72 6b2c 2061 6c74 686f 7567 6820   work, although 
+00010f70: 7468 6520 6060 7472 6169 7473 2e70 726f  the ``traits.pro
+00010f80: 746f 636f 6c73 6060 2041 5049 2068 6173  tocols`` API has
+00010f90: 2062 6565 6e20 6465 7072 6563 6174 6564   been deprecated
+00010fa0: 2c0a 616e 6420 6120 7761 726e 696e 6720  ,.and a warning 
+00010fb0: 7769 6c6c 2062 6520 6c6f 6767 6564 206f  will be logged o
+00010fc0: 6e20 6669 7273 7420 7573 6520 6f66 2060  n first use of `
+00010fd0: 6074 7261 6974 732e 7072 6f74 6f63 6f6c  `traits.protocol
+00010fe0: 7360 602e 2020 5365 6520 7468 650a 2741  s``.  See the.'A
+00010ff0: 6476 616e 6365 6420 546f 7069 6373 2720  dvanced Topics' 
+00011000: 7365 6374 696f 6e20 6f66 2074 6865 2075  section of the u
+00011010: 7365 7220 6d61 6e75 616c 2066 6f72 206d  ser manual for m
+00011020: 6f72 6520 6465 7461 696c 732e 0a0a 5468  ore details...Th
+00011030: 6520 7265 6c65 6173 6520 616c 736f 2069  e release also i
+00011040: 6e63 6c75 6465 7320 696d 7072 6f76 6564  ncludes improved
+00011050: 2073 7570 706f 7274 2066 6f72 2075 7369   support for usi
+00011060: 6e67 2043 7974 686f 6e20 7769 7468 2060  ng Cython with `
+00011070: 6048 6173 5472 6169 7473 6060 0a63 6c61  `HasTraits``.cla
+00011080: 7373 6573 2c20 736f 6d65 206e 6577 2068  sses, some new h
+00011090: 656c 7065 7220 7574 696c 6974 6965 7320  elper utilities 
+000110a0: 666f 7220 7772 6974 696e 6720 756e 6974  for writing unit
+000110b0: 2074 6573 7473 2066 6f72 2054 7261 6974   tests for Trait
+000110c0: 7320 6576 656e 7473 2c0a 616e 6420 6120  s events,.and a 
+000110d0: 7661 7269 6574 7920 6f66 2062 7567 2066  variety of bug f
+000110e0: 6978 6573 2c20 7374 6162 696c 6974 7920  ixes, stability 
+000110f0: 656e 6861 6e63 656d 656e 7473 2c20 616e  enhancements, an
+00011100: 6420 696e 7465 726e 616c 2063 6f64 650a  d internal code.
+00011110: 696d 7072 6f76 656d 656e 7473 2e0a 0a0a  improvements....
+00011120: 4368 616e 6765 2073 756d 6d61 7279 2073  Change summary s
+00011130: 696e 6365 2034 2e33 2e30 0a7e 7e7e 7e7e  ince 4.3.0.~~~~~
+00011140: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00011150: 7e7e 7e7e 7e0a 0a4e 6577 2066 6561 7475  ~~~~~..New featu
+00011160: 7265 730a 0a2a 2054 6865 2061 6461 7074  res..* The adapt
+00011170: 6174 696f 6e20 6d65 6368 616e 6973 6d20  ation mechanism 
+00011180: 696e 2054 7261 6974 732c 2066 6f72 6d65  in Traits, forme
+00011190: 726c 7920 6261 7365 6420 6f6e 2074 6865  rly based on the
+000111a0: 2027 7472 6169 7473 2e70 726f 746f 636f   'traits.protoco
+000111b0: 6c73 270a 2020 7061 636b 6167 652c 2068  ls'.  package, h
+000111c0: 6173 2062 6565 6e20 7265 706c 6163 6564  as been replaced
+000111d0: 2077 6974 6820 7468 6520 6d6f 7265 2072   with the more r
+000111e0: 6f62 7573 7420 2774 7261 6974 732e 6164  obust 'traits.ad
+000111f0: 6170 7461 7469 6f6e 270a 2020 7061 636b  aptation'.  pack
+00011200: 6167 652e 2028 2335 3129 0a2a 2041 6464  age. (#51).* Add
+00011210: 6564 2075 7469 6c69 7479 2066 756e 6374  ed utility funct
+00011220: 696f 6e20 666f 7220 696d 706f 7274 696e  ion for importin
+00011230: 6720 7379 6d62 6f6c 7320 286e 616d 652c  g symbols (name,
+00011240: 2063 6c61 7373 6573 2c20 6675 6e63 7469   classes, functi
+00011250: 6f6e 7329 0a20 2062 7920 6e61 6d65 3a20  ons).  by name: 
+00011260: 2774 7261 6974 732e 7574 696c 2e61 7069  'traits.util.api
+00011270: 2e69 6d70 6f72 745f 7379 6d62 6f6c 272e  .import_symbol'.
+00011280: 2028 2335 3129 0a2a 2055 7365 7273 2063   (#51).* Users c
+00011290: 616e 2073 6574 2061 2067 6c6f 6261 6c20  an set a global 
+000112a0: 7472 6163 6572 2c20 7768 6963 6820 7265  tracer, which re
+000112b0: 6365 6976 6573 2061 6c6c 2074 7261 6974  ceives all trait
+000112c0: 7320 6368 616e 6765 2065 7665 6e74 733a  s change events:
+000112d0: 0a20 2060 6074 7261 6974 732e 7472 6169  .  ``traits.trai
+000112e0: 745f 6e6f 7469 6669 6572 732e 7365 745f  t_notifiers.set_
+000112f0: 6368 616e 6765 5f65 7665 6e74 5f74 7261  change_event_tra
+00011300: 6365 7273 6060 2e20 2823 3739 290a 0a45  cers``. (#79)..E
+00011310: 6e68 616e 6365 6d65 6e74 730a 0a2a 2055  nhancements..* U
+00011320: 7064 6174 6520 6265 6e63 686d 6172 6b20  pdate benchmark 
+00011330: 7363 7269 7074 2e20 2823 3534 290a 2a20  script. (#54).* 
+00011340: 7472 6169 7473 2e75 7469 6c2e 6465 7072  traits.util.depr
+00011350: 6563 6174 6564 3a20 7573 6520 6d6f 6475  ecated: use modu
+00011360: 6c65 206c 6f67 6765 7220 696e 7374 6561  le logger instea
+00011370: 6420 6f66 2072 6f6f 7420 6c6f 6767 6572  d of root logger
+00011380: 2e20 2823 3539 290a 2a20 5072 6f76 6964  . (#59).* Provid
+00011390: 6520 616e 2069 6e66 6f72 6d61 7469 7665  e an informative
+000113a0: 206d 6573 7361 6765 2069 6e20 4164 6170   message in Adap
+000113b0: 7461 7469 6f6e 4572 726f 722e 2028 2336  tationError. (#6
+000113c0: 3229 0a2a 2041 6c6c 6f77 2048 6173 5472  2).* Allow HasTr
+000113d0: 6169 7473 2063 6c61 7373 6573 2074 6f20  aits classes to 
+000113e0: 6265 2063 7974 686f 6e69 7a65 642e 2028  be cythonized. (
+000113f0: 2337 3329 0a2a 2049 6d70 726f 7665 2074  #73).* Improve t
+00011400: 6573 7473 2066 6f72 2063 7974 686f 6e69  ests for cythoni
+00011410: 7a61 7469 6f6e 2073 7570 706f 7274 2e20  zation support. 
+00011420: 2823 3735 290a 2a20 4578 7465 6e64 696e  (#75).* Extendin
+00011430: 6720 7661 7269 6f75 7320 7472 6169 7420  g various trait 
+00011440: 7465 7374 696e 6720 6865 6c70 6572 7320  testing helpers 
+00011450: 2823 3533 290a 0a52 6566 6163 746f 7269  (#53)..Refactori
+00011460: 6e67 0a0a 2a20 5468 6520 5472 6169 7473  ng..* The Traits
+00011470: 206e 6f74 6966 6963 6174 696f 6e20 636f   notification co
+00011480: 6465 2068 6173 2062 6565 6e20 7265 776f  de has been rewo
+00011490: 726b 6564 2074 6f20 7265 6d6f 7665 2063  rked to remove c
+000114a0: 6f64 6520 6475 706c 6963 6174 696f 6e2c  ode duplication,
+000114b0: 0a20 2061 6e64 2074 6573 7420 636f 7665  .  and test cove
+000114c0: 7261 6765 206f 6620 7468 6174 2063 6f64  rage of that cod
+000114d0: 6520 6861 7320 6265 656e 2073 6967 6e69  e has been signi
+000114e0: 6669 6361 6e74 6c79 2069 6d70 726f 7665  ficantly improve
+000114f0: 642e 2028 2337 3929 0a0a 4669 7865 730a  d. (#79)..Fixes.
+00011500: 0a2a 2046 6978 2072 6163 6520 636f 6e64  .* Fix race cond
+00011510: 6974 696f 6e20 7768 656e 2072 656d 6f76  ition when remov
+00011520: 696e 6720 6120 7472 6169 7473 206c 6973  ing a traits lis
+00011530: 7465 6e65 722e 2028 2335 3729 0a2a 2046  tener. (#57).* F
+00011540: 6978 2075 676c 7920 696e 7465 7261 6374  ix ugly interact
+00011550: 696f 6e20 6265 7477 6565 6e20 4465 6c65  ion between Dele
+00011560: 6761 7465 7354 6f20 6368 616e 6765 2068  gatesTo change h
+00011570: 616e 646c 6572 732c 2064 796e 616d 6963  andlers, dynamic
+00011580: 2063 6861 6e67 650a 2020 6861 6e64 6c65   change.  handle
+00011590: 7273 2061 6e64 2074 776f 206c 6576 656c  rs and two level
+000115a0: 7320 6f66 2064 796e 616d 6963 2069 6e69  s of dynamic ini
+000115b0: 7469 616c 697a 6174 696f 6e2e 2028 2336  tialization. (#6
+000115c0: 3329 0a2a 2055 7365 2061 204e 756c 6c48  3).* Use a NullH
+000115d0: 616e 646c 6572 2066 6f72 2061 6c6c 2027  andler for all '
+000115e0: 7472 6169 7473 2720 6c6f 6767 6572 732e  traits' loggers.
+000115f0: 2028 2336 3429 0a2a 2046 6978 2072 6163   (#64).* Fix rac
+00011600: 6520 636f 6e64 6974 696f 6e20 696e 2054  e condition in T
+00011610: 7261 6974 4368 616e 6765 4e6f 7469 6679  raitChangeNotify
+00011620: 5772 6170 7065 722e 6c69 7374 656e 6572  Wrapper.listener
+00011630: 5f64 656c 6574 6564 2028 2336 3629 0a2a  _deleted (#66).*
+00011640: 2046 6978 206c 6561 6b69 6e67 206e 6f74   Fix leaking not
+00011650: 6966 6965 7273 2e20 2823 3638 290a 2a20  ifiers. (#68).* 
+00011660: 4669 7820 6661 696c 696e 6720 7370 6563  Fix failing spec
+00011670: 6961 6c20 696e 7374 616e 6365 2074 7261  ial instance tra
+00011680: 6974 2065 7665 6e74 732e 2028 2337 3829  it events. (#78)
+00011690: 0a2a 2046 6978 2068 6964 696e 6720 4b65  .* Fix hiding Ke
+000116a0: 7945 7272 6f72 2065 7863 6570 7469 6f6e  yError exception
+000116b0: 2069 6e73 6964 6520 7472 6169 7420 6465   inside trait de
+000116c0: 6661 756c 7420 696e 6974 6961 6c69 7a65  fault initialize
+000116d0: 206d 6574 686f 642e 0a20 2028 2338 3129   method..  (#81)
+000116e0: 0a2a 2046 6978 2041 6461 7074 6572 206f  .* Fix Adapter o
+000116f0: 626a 6563 7420 696e 6974 6961 6c69 7a61  bject initializa
+00011700: 7469 6f6e 2e20 2823 3933 290a 2a20 4669  tion. (#93).* Fi
+00011710: 7820 6379 636c 6963 2067 6172 6261 6765  x cyclic garbage
+00011720: 2061 7269 7369 6e67 2066 726f 6d20 7573   arising from us
+00011730: 6520 6f66 2074 6865 2057 6561 6b52 6566  e of the WeakRef
+00011740: 2074 7261 6974 2074 7970 652e 2028 2339   trait type. (#9
+00011750: 3529 0a2a 2060 6054 7261 6974 5365 744f  5).* ``TraitSetO
+00011760: 626a 6563 742e 636f 7079 6060 206e 6f77  bject.copy`` now
+00011770: 2072 6574 7572 6e73 2061 2070 6c61 696e   returns a plain
+00011780: 2072 6174 6865 7220 7468 616e 2061 6e0a   rather than an.
+00011790: 2020 756e 696e 6974 6961 6c69 7a65 6420    uninitialized 
+000117a0: 6060 5472 6169 7453 6574 4f62 6a65 6374  ``TraitSetObject
+000117b0: 6060 2069 6e73 7461 6e63 652e 2028 2339  `` instance. (#9
+000117c0: 3729 0a2a 2046 6978 2063 7963 6c69 6320  7).* Fix cyclic 
+000117d0: 6761 7262 6167 6520 6172 6973 696e 6720  garbage arising 
+000117e0: 6672 6f6d 2064 796e 616d 6963 2074 7261  from dynamic tra
+000117f0: 6974 2063 6861 6e67 6520 6861 6e64 6c65  it change handle
+00011800: 7273 2e20 2823 3130 3129 0a0a 0a52 656c  rs. (#101)...Rel
+00011810: 6561 7365 7320 342e 332e 3020 2d20 332e  eases 4.3.0 - 3.
+00011820: 362e 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  6.0.------------
+00011830: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4368 616e  ----------..Chan
+00011840: 6765 6c6f 6773 2075 6e61 7661 696c 6162  gelogs unavailab
+00011850: 6c65 2e0a 0a0a 5265 6c65 6173 6520 332e  le....Release 3.
+00011860: 352e 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  5.0.------------
+00011870: 2d0a 0a52 656c 6561 7365 643a 2032 3031  -..Released: 201
+00011880: 302d 3130 2d31 350a 0a45 6e68 616e 6365  0-10-15..Enhance
+00011890: 6d65 6e74 730a 0a2a 2061 6464 696e 6720  ments..* adding 
+000118a0: 7375 7070 6f72 7420 666f 7220 6472 6f70  support for drop
+000118b0: 2d64 6f77 6e20 6d65 6e75 2069 6e20 4275  -down menu in Bu
+000118c0: 7474 6f6e 2074 7261 6974 732c 2062 7574  tton traits, but
+000118d0: 206f 6e6c 7920 666f 7220 7174 2062 6163   only for qt bac
+000118e0: 6b65 6e64 0a2a 2061 6464 696e 6720 2773  kend.* adding 's
+000118f0: 686f 775f 6e6f 7465 626f 6f6b 5f6d 656e  how_notebook_men
+00011900: 7527 206f 7074 696f 6e20 746f 204c 6973  u' option to Lis
+00011910: 7445 6469 746f 7220 736f 2074 6861 7420  tEditor so that 
+00011920: 7468 6520 7573 6572 2063 616e 0a20 2072  the user can.  r
+00011930: 6967 6874 2d63 6c69 636b 2061 6e64 2073  ight-click and s
+00011940: 686f 7720 6f72 2068 6964 6520 7468 6520  how or hide the 
+00011950: 636f 6e74 6578 7420 6d65 6e75 2028 5174  context menu (Qt
+00011960: 290a 2a20 6164 6465 6420 7365 6c65 6374  ).* added select
+00011970: 696f 6e20 7261 6e67 6520 7472 6169 7473  ion range traits
+00011980: 2074 6f20 6d61 6b65 2069 7420 706f 7373   to make it poss
+00011990: 6962 6c65 2066 6f72 2075 7365 7273 2074  ible for users t
+000119a0: 6f20 7265 706c 6163 650a 2020 7365 6c65  o replace.  sele
+000119b0: 6374 6564 2074 6578 740a 0a46 6978 6573  cted text..Fixes
+000119c0: 0a0a 2a20 6669 7865 6420 6e75 6c6c 2063  ..* fixed null c
+000119d0: 6f6c 6f72 2065 6469 746f 7220 746f 2077  olor editor to w
+000119e0: 6f72 6b20 7769 7468 2074 7570 6c65 730a  ork with tuples.
+000119f0: 2a20 6275 6720 7768 656e 206f 7065 6e69  * bug when openi
+00011a00: 6e67 2061 2076 6965 7720 7769 7468 2074  ng a view with t
+00011a10: 6865 2054 6f6f 6c62 6172 4275 7474 6f6e  he ToolbarButton
+00011a20: 0a0a 0a52 656c 6561 7365 2033 2e34 2e30  ...Release 3.4.0
+00011a30: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
+00011a40: 5265 6c65 6173 6564 3a20 3230 3130 2d30  Released: 2010-0
+00011a50: 352d 3236 0a0a 456e 6861 6e63 656d 656e  5-26..Enhancemen
+00011a60: 7473 0a0a 2a20 6164 6469 6e67 206e 6577  ts..* adding new
+00011a70: 2065 7861 6d70 6c65 2074 6f20 6d61 6b65   example to make
+00011a80: 2074 6573 7469 6e67 2072 6762 2063 6f6c   testing rgb col
+00011a90: 6f72 2065 6469 746f 7220 6561 7369 6572  or editor easier
+00011aa0: 0a0a 4669 7865 730a 0a2a 2066 6978 6564  ..Fixes..* fixed
+00011ab0: 204e 756d 6572 6963 436f 6c75 6d6e 2074   NumericColumn t
+00011ac0: 6f20 6e6f 7420 6578 7065 6374 206f 626a  o not expect obj
+00011ad0: 6563 7420 746f 2068 6176 6520 6d6f 6465  ect to have mode
+00011ae0: 6c5f 7365 6c65 6374 696f 6e20 6174 7472  l_selection attr
+00011af0: 6962 7574 652c 0a20 2061 6e64 2072 656d  ibute,.  and rem
+00011b00: 6f76 6564 206d 6f72 6520 6465 6164 2074  oved more dead t
+00011b10: 6865 6d69 6e67 2063 6f64 650a 2a20 6669  heming code.* fi
+00011b20: 7865 6420 4150 4920 6275 6773 2077 6974  xed API bugs wit
+00011b30: 6820 7468 6520 4e75 6d65 7269 6343 6f6c  h the NumericCol
+00011b40: 756d 6e20 7768 6572 6520 6974 7320 6675  umn where its fu
+00011b50: 6e63 7469 6f6e 2073 6967 6e61 7475 7265  nction signature
+00011b60: 730a 2020 6469 6666 6572 6564 2066 726f  s.  differed fro
+00011b70: 6d20 6974 7320 6261 7365 2063 6c61 7373  m its base class
+00011b80: 2c20 6275 7420 7468 6520 6361 6c6c 696e  , but the callin
+00011b90: 6720 636f 6465 2065 7870 6563 7465 6420  g code expected 
+00011ba0: 7468 656d 2074 6f20 616c 6c0a 2020 6265  them to all.  be
+00011bb0: 2074 6865 2073 616d 650a 2a20 6669 7865   the same.* fixe
+00011bc0: 6420 6275 6720 7768 6963 6820 7761 7320  d bug which was 
+00011bd0: 7265 6c61 7465 6420 746f 2074 7970 6520  related to type 
+00011be0: 6e61 6d65 2065 7272 6f72 7320 6361 7573  name errors caus
+00011bf0: 6564 2077 6865 6e20 7275 6e6e 696e 6720  ed when running 
+00011c00: 5370 6869 6e78 0a2a 2077 6865 6e20 7573  Sphinx.* when us
+00011c10: 696e 6720 4669 6c65 2865 7869 7374 733d  ing File(exists=
+00011c20: 5472 7565 292c 2062 6520 7375 7265 2074  True), be sure t
+00011c30: 6f20 7661 6c69 6461 7465 2074 6865 2074  o validate the t
+00011c40: 7970 6520 6f66 2074 6865 2076 616c 7565  ype of the value
+00011c50: 0a20 2066 6972 7374 2062 6566 6f72 6520  .  first before 
+00011c60: 7573 696e 6720 6f73 2e70 6174 682e 6973  using os.path.is
+00011c70: 6669 6c65 2829 0a0a 0a52 656c 6561 7365  file()...Release
+00011c80: 2033 2e33 2e30 0a2d 2d2d 2d2d 2d2d 2d2d   3.3.0.---------
+00011c90: 2d2d 2d2d 0a0a 5265 6c65 6173 6564 3a20  ----..Released: 
+00011ca0: 3230 3130 2d30 322d 3234 0a0a 456e 6861  2010-02-24..Enha
+00011cb0: 6e63 656d 656e 7473 0a0a 5468 6520 6d61  ncements..The ma
+00011cc0: 6a6f 7220 656e 6861 6e63 656d 656e 7420  jor enhancement 
+00011cd0: 7468 6973 2072 656c 6561 7365 2069 7320  this release is 
+00011ce0: 7468 6174 2074 6865 2065 6e74 6972 6520  that the entire 
+00011cf0: 5472 6169 7473 2070 6163 6b61 6765 2068  Traits package h
+00011d00: 6173 2062 6565 6e0a 6368 616e 6765 6420  as been.changed 
+00011d10: 746f 2075 7365 2072 656c 6174 6976 6520  to use relative 
+00011d20: 696d 706f 7274 7320 736f 2074 6861 7420  imports so that 
+00011d30: 6974 2063 616e 2062 6520 696e 7374 616c  it can be instal
+00011d40: 6c65 6420 6173 2061 2073 7562 2d70 6163  led as a sub-pac
+00011d50: 6b61 6765 0a69 6e73 6964 6520 616e 6f74  kage.inside anot
+00011d60: 6865 7220 6c61 7267 6572 206c 6962 7261  her larger libra
+00011d70: 7279 206f 7220 7061 636b 6167 652e 2020  ry or package.  
+00011d80: 5468 6973 2077 6173 206e 6f74 2070 7265  This was not pre
+00011d90: 7669 6f75 736c 7920 706f 7373 6962 6c65  viously possible
+00011da0: 2c0a 7369 6e63 6520 7468 6520 7661 7269  ,.since the vari
+00011db0: 6f75 7320 6d6f 6475 6c65 7320 696e 7369  ous modules insi
+00011dc0: 6465 2054 7261 6974 7320 776f 756c 6420  de Traits would 
+00011dd0: 696d 706f 7274 2065 6163 6820 6f74 6865  import each othe
+00011de0: 7220 6469 7265 6374 6c79 0a74 6872 6f75  r directly.throu
+00011df0: 6768 2022 7472 6169 7473 2e5b 6d6f 6475  gh "traits.[modu
+00011e00: 6c65 5d22 2e20 204d 616e 7920 7468 616e  le]".  Many than
+00011e10: 6b73 2074 6f20 4461 7272 656e 2044 616c  ks to Darren Dal
+00011e20: 6520 666f 7220 7468 650a 7061 7463 682e  e for the.patch.
+00011e30: 0a0a 4669 7865 730a 0a54 6865 7265 2068  ..Fixes..There h
+00011e40: 6176 6520 6265 656e 206e 756d 6572 6f75  ave been numerou
+00011e50: 7320 6d69 6e6f 7220 6275 6766 6978 6573  s minor bugfixes
+00011e60: 2073 696e 6365 2074 6865 206c 6173 7420   since the last 
+00011e70: 7265 6c65 6173 652e 2020 5468 6520 6d6f  release.  The mo
+00011e80: 7374 206e 6f74 6162 6c65 0a6f 6e65 7320  st notable.ones 
+00011e90: 6172 653a 0a0a 2a20 4d61 6e79 2066 6978  are:..* Many fix
+00011ea0: 6573 2069 6e76 6f6c 7665 206d 616b 696e  es involve makin
+00011eb0: 6720 5472 6169 7473 2055 4920 6d6f 7265  g Traits UI more
+00011ec0: 2072 6f62 7573 7420 6966 2077 7850 7974   robust if wxPyt
+00011ed0: 686f 6e20 6973 206e 6f74 2069 6e73 7461  hon is not insta
+00011ee0: 6c6c 6564 0a20 206f 6e20 6120 7379 7374  lled.  on a syst
+00011ef0: 656d 2e20 2049 6e20 7468 6520 7061 7374  em.  In the past
+00011f00: 2c20 7765 2068 6176 6520 6265 656e 2061  , we have been a
+00011f10: 626c 6520 746f 2075 7365 2051 7420 6966  ble to use Qt if
+00011f20: 2069 7420 7761 7320 616c 736f 0a20 2069   it was also.  i
+00011f30: 6e73 7461 6c6c 6564 2c20 6275 7420 7265  nstalled, but re
+00011f40: 6d6f 7669 6e67 2057 7820 776f 756c 6420  moving Wx would 
+00011f50: 6c65 6164 2074 6f20 6120 7661 7269 6574  lead to a variet
+00011f60: 7920 6f66 206c 6974 746c 6520 6275 6773  y of little bugs
+00011f70: 2069 6e20 7661 7269 6f75 730a 2020 706c   in various.  pl
+00011f80: 6163 6573 2e20 2057 6527 7665 2073 7175  aces.  We've squ
+00011f90: 6173 6865 6420 6120 6e75 6d62 6572 206f  ashed a number o
+00011fa0: 6620 7468 6573 652e 2020 5765 2776 6520  f these.  We've 
+00011fb0: 616c 736f 2061 6464 6564 2062 6574 7465  also added bette
+00011fc0: 7220 6368 6563 6b73 0a20 2074 6f20 6d61  r checks.  to ma
+00011fd0: 6b65 2073 7572 6520 7765 2772 6520 7365  ke sure we're se
+00011fe0: 6c65 6374 696e 6720 7468 6520 7269 6768  lecting the righ
+00011ff0: 7420 746f 6f6c 6b69 7420 6174 2069 6d70  t toolkit at imp
+00012000: 6f72 7420 616e 6420 6174 2072 756e 7469  ort and at runti
+00012010: 6d65 2e0a 2a20 4120 6e61 7374 7920 6379  me..* A nasty cy
+00012020: 636c 6963 2072 6566 6572 656e 6365 2077  clic reference w
+00012030: 6173 2064 6973 636f 7665 7265 6420 616e  as discovered an
+00012040: 6420 656c 696d 696e 6174 6564 2069 6e20  d eliminated in 
+00012050: 4465 6c65 6761 7465 7354 6f20 7472 6169  DelegatesTo trai
+00012060: 7473 2e0a 2a20 5468 6520 556e 6465 6669  ts..* The Undefi
+00012070: 6e65 6420 616e 6420 556e 696e 6974 6961  ned and Uninitia
+00012080: 6c69 7a65 6420 5472 6169 7473 2077 6572  lized Traits wer
+00012090: 6520 6d61 6465 2069 6e74 6f20 7472 7565  e made into true
+000120a0: 2073 696e 676c 6574 6f6e 732e 0a2a 204d   singletons..* M
+000120b0: 7563 6820 6f66 2074 6865 2069 6e63 6f6e  uch of the incon
+000120c0: 7369 7374 656e 7420 666f 726d 6174 7469  sistent formatti
+000120d0: 6e67 2061 6372 6f73 7320 7468 6520 656e  ng across the en
+000120e0: 7469 7265 2054 7261 6974 7320 736f 7572  tire Traits sour
+000120f0: 6365 2068 6173 0a20 2062 6565 6e20 656c  ce has.  been el
+00012100: 696d 696e 6174 6564 2061 6e64 206e 6f72  iminated and nor
+00012110: 6d61 6c69 7a65 6420 2874 6162 732f 7370  malized (tabs/sp
+00012120: 6163 6573 2c20 6c69 6e65 2065 6e64 696e  aces, line endin
+00012130: 6773 292e 0a0a 0a52 656c 6561 7365 2033  gs)....Release 3
+00012140: 2e32 2e30 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .2.0.-----------
+00012150: 2d2d 0a0a 5265 6c65 6173 6564 3a20 3230  --..Released: 20
+00012160: 3039 2d30 372d 3135 0a0a 456e 6861 6e63  09-07-15..Enhanc
+00012170: 656d 656e 7473 0a0a 2a20 496d 706c 656d  ements..* Implem
+00012180: 656e 7465 6420 6564 6974 6162 6c65 5f6c  ented editable_l
+00012190: 6162 656c 7320 6174 7472 6962 7574 6520  abels attribute 
+000121a0: 696e 2074 6865 2054 6162 756c 6172 4564  in the TabularEd
+000121b0: 6974 6f72 2066 6f72 2065 6e61 626c 696e  itor for enablin
+000121c0: 6720 6564 6974 696e 6720 6f66 2074 6865  g editing of the
+000121d0: 206c 6162 656c 7320 2869 2e65 2e20 7468   labels (i.e. th
+000121e0: 6520 6669 7273 7420 636f 6c75 6d6e 290a  e first column).
+000121f0: 2a20 5361 7669 6e67 2f72 6573 746f 7269  * Saving/restori
+00012200: 6e67 2077 696e 646f 7720 706f 7369 7469  ng window positi
+00012210: 6f6e 7320 776f 726b 7320 7769 7468 206d  ons works with m
+00012220: 756c 7469 706c 6520 6469 7370 6c61 7973  ultiple displays
+00012230: 206f 6620 6469 6666 6572 656e 7420 7369   of different si
+00012240: 7a65 730a 2a20 4e65 7720 5072 6f67 7265  zes.* New Progre
+00012250: 7373 4564 6974 6f72 0a2a 2043 6861 6e67  ssEditor.* Chang
+00012260: 6564 2064 6566 6175 6c74 2063 6f6c 6f72  ed default color
+00012270: 7320 666f 7220 5461 626c 6545 6469 746f  s for TableEdito
+00012280: 720a 2a20 4164 6465 6420 7375 7070 6f72  r.* Added suppor
+00012290: 7420 666f 7220 4854 4d4c 4564 6974 6f72  t for HTMLEditor
+000122a0: 2066 6f72 2051 5420 6261 636b 656e 6420   for QT backend 
+000122b0: 7573 696e 6720 5174 5765 624b 6974 0a2a  using QtWebKit.*
+000122c0: 2049 6d70 726f 7665 6420 7375 7070 6f72   Improved suppor
+000122d0: 7420 666f 7220 6f70 656e 696e 6720 6c69  t for opening li
+000122e0: 6e6b 7320 696e 2065 7874 6572 6e61 6c20  nks in external 
+000122f0: 6272 6f77 7365 7220 6672 6f6d 2048 544d  browser from HTM
+00012300: 4c45 6469 746f 720a 2a20 4164 6465 6420  LEditor.* Added 
+00012310: 7375 7070 6f72 7420 666f 7220 5461 6275  support for Tabu
+00012320: 6c61 7245 6469 746f 7220 666f 7220 5154  larEditor for QT
+00012330: 2062 6163 6b65 6e64 0a2a 2041 6464 6564   backend.* Added
+00012340: 2073 7570 706f 7274 2066 6f72 206d 6172   support for mar
+00012350: 6b69 6e67 2075 7020 7468 6520 436f 6465  king up the Code
+00012360: 4564 6974 6f72 2c20 696e 636c 7564 696e  Editor, includin
+00012370: 6720 6164 6469 6e67 2073 7175 6967 676c  g adding squiggl
+00012380: 6573 2061 6e64 2064 696d 6d69 6e67 206c  es and dimming l
+00012390: 696e 6573 0a2a 2041 6464 6564 2053 6561  ines.* Added Sea
+000123a0: 7263 6845 6469 746f 720a 2a20 496d 7072  rchEditor.* Impr
+000123b0: 6f76 6564 2075 6e69 636f 6465 2073 7570  oved unicode sup
+000123c0: 706f 7274 0a2a 2043 6861 6e67 6564 2062  port.* Changed b
+000123d0: 6568 6176 696f 7220 6f66 2052 616e 6765  ehavior of Range
+000123e0: 4564 6974 6f72 2074 6578 7420 626f 7820  Editor text box 
+000123f0: 746f 206e 6f74 2061 7574 6f2d 7365 740a  to not auto-set.
+00012400: 2a20 4164 6465 6420 7375 7070 6f72 7420  * Added support 
+00012410: 696e 2052 616e 6765 4564 6974 6f72 2066  in RangeEditor f
+00012420: 6f72 2073 7065 6369 6679 696e 6720 7468  or specifying th
+00012430: 6520 6d65 7468 6f64 2074 6f20 6576 616c  e method to eval
+00012440: 7561 7465 206e 6577 2076 616c 7565 732e  uate new values.
+00012450: 0a2a 2041 6464 2044 6566 6175 6c74 4f76  .* Add DefaultOv
+00012460: 6572 7269 6465 2065 6469 746f 7220 6661  erride editor fa
+00012470: 6374 6f72 7920 636f 7572 7465 7379 2053  ctory courtesy S
+00012480: 74c3 a966 616e 2076 616e 2064 6572 2057  t..fan van der W
+00012490: 616c 740a 2a20 5265 6d6f 7665 6420 7379  alt.* Removed sy
+000124a0: 732e 6578 6974 2829 2063 616c 6c20 6672  s.exit() call fr
+000124b0: 6f6d 2053 6176 6548 616e 646c 6572 2e65  om SaveHandler.e
+000124c0: 7869 7428 290a                           xit().
```

### Comparing `traits-6.4.1/LICENSE-CC-BY-3.0.txt` & `traits-6.4.2/LICENSE-CC-BY-3.0.txt`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/LICENSE.txt` & `traits-6.4.2/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 This software is OSI Certified Open Source Software.
 OSI Certified is a certification mark of the Open Source Initiative.
 
-(C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+(C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `traits-6.4.1/PKG-INFO` & `traits-6.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traits
-Version: 6.4.1
+Version: 6.4.2
 Summary: Observable typed attributes for Python classes
 Home-page: http://docs.enthought.com/traits
 Download-URL: https://pypi.python.org/pypi/traits
 Author: Enthought
 Author-email: info@enthought.com
 License: BSD
 Project-URL: Issue Tracker, https://github.com/enthought/traits/issues
@@ -15,26 +15,25 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: examples
 License-File: LICENSE-CC-BY-3.0.txt
 License-File: LICENSE.txt
 
@@ -76,15 +75,15 @@
 or can opt to allow the use of only a fixed or open set of trait attributes
 within the class. Trait attributes defined by a class are automatically
 inherited by any subclass derived from the class.
 
 Dependencies
 ------------
 
-Traits requires Python >= 3.6.
+Traits requires Python >= 3.7.
 
 Traits has the following optional dependencies:
 
 * `NumPy <http://pypi.python.org/pypi/numpy>`_ to support the trait types
   for arrays.
 * `TraitsUI <https://pypi.python.org/pypi/traitsui>`_ to support GUI
   Views.
```

### Comparing `traits-6.4.1/README.rst` & `traits-6.4.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 or can opt to allow the use of only a fixed or open set of trait attributes
 within the class. Trait attributes defined by a class are automatically
 inherited by any subclass derived from the class.
 
 Dependencies
 ------------
 
-Traits requires Python >= 3.6.
+Traits requires Python >= 3.7.
 
 Traits has the following optional dependencies:
 
 * `NumPy <http://pypi.python.org/pypi/numpy>`_ to support the trait types
   for arrays.
 * `TraitsUI <https://pypi.python.org/pypi/traitsui>`_ to support GUI
   Views.
```

### Comparing `traits-6.4.1/docs/Makefile` & `traits-6.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/make.bat` & `traits-6.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/_static/default.css` & `traits-6.4.2/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/_static/e-logo-rev.png` & `traits-6.4.2/docs/source/_static/e-logo-rev.png`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/_static/et.ico` & `traits-6.4.2/docs/source/_static/et.ico`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/_templates/search.html` & `traits-6.4.2/docs/source/_templates/search.html`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/conf.py` & `traits-6.4.2/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -58,15 +58,15 @@
 
 # The master toctree document.
 master_doc = "index"
 
 # General substitutions.
 project = "traits"
 copyright = """\
-(C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+(C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 All rights reserved.
 """
 
 # The default replacements for |version| and |release|, also used in various
 # other places throughout the built documents.
 version_info = {}
 traits_init_path = os.path.join("..", "..", "traits", "__init__.py")
```

### Comparing `traits-6.4.1/docs/source/traits_api_reference/editor_factories.rst` & `traits-6.4.2/docs/source/traits_api_reference/editor_factories.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/has_traits.rst` & `traits-6.4.2/docs/source/traits_api_reference/has_traits.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/index.rst` & `traits-6.4.2/docs/source/traits_api_reference/index.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/trait_base.rst` & `traits-6.4.2/docs/source/traits_api_reference/trait_base.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/trait_handlers.rst` & `traits-6.4.2/docs/source/traits_api_reference/trait_handlers.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/trait_notifiers.rst` & `traits-6.4.2/docs/source/traits_api_reference/trait_notifiers.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/trait_types.rst` & `traits-6.4.2/docs/source/traits_api_reference/trait_types.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/traits.adaptation.rst` & `traits-6.4.2/docs/source/traits_api_reference/traits.adaptation.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/traits.observation.rst` & `traits-6.4.2/docs/source/traits_api_reference/traits.observation.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/traits.testing.rst` & `traits-6.4.2/docs/source/traits_api_reference/traits.testing.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_api_reference/traits.util.rst` & `traits-6.4.2/docs/source/traits_api_reference/traits.util.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_tutorial/introduction.rst` & `traits-6.4.2/docs/source/traits_tutorial/introduction.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/advanced.rst` & `traits-6.4.2/docs/source/traits_user_manual/advanced.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/appendix.rst` & `traits-6.4.2/docs/source/traits_user_manual/appendix.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/custom.rst` & `traits-6.4.2/docs/source/traits_user_manual/custom.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/debugging.rst` & `traits-6.4.2/docs/source/traits_user_manual/debugging.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/deferring.rst` & `traits-6.4.2/docs/source/traits_user_manual/deferring.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/defining.rst` & `traits-6.4.2/docs/source/traits_user_manual/defining.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/images/adaptation.png` & `traits-6.4.2/docs/source/traits_user_manual/images/adaptation.png`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/index.rst` & `traits-6.4.2/docs/source/traits_user_manual/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ============================
 Traits |version| User Manual
 ============================
 
 :Authors: David C. Morrill, Janet M. Swisher, and Enthought developers
-:Copyright: | (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+:Copyright: | (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
             | All rights reserved.
 
 Contents
 ========
 
 .. toctree::
     :maxdepth: 3
```

### Comparing `traits-6.4.1/docs/source/traits_user_manual/installation.rst` & `traits-6.4.2/docs/source/traits_user_manual/installation.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/internals.rst` & `traits-6.4.2/docs/source/traits_user_manual/internals.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/intro.rst` & `traits-6.4.2/docs/source/traits_user_manual/intro.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/listening.rst` & `traits-6.4.2/docs/source/traits_user_manual/listening.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/notification.rst` & `traits-6.4.2/docs/source/traits_user_manual/notification.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/docs/source/traits_user_manual/testing.rst` & `traits-6.4.2/docs/source/traits_user_manual/testing.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/default.css` & `traits-6.4.2/examples/tutorials/doc_examples/default.css`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/doc_examples.rst` & `traits-6.4.2/examples/tutorials/doc_examples/doc_examples.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/__init__.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-"""
-This directory contains a collection of the various examples taken from the
-Traits documentation.
-"""
+# wildcard.py --- Example of using a wildcard with a trait
+#                 attribute name
+from traits.api import Any, HasTraits
+
+
+class Person(HasTraits):
+    temp_ = Any
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/adapt_metadata.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/adapt_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/add_class_trait.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/add_class_trait.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/all_traits_features.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/all_traits_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/all_wildcard.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/all_wildcard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/bad_self_ref.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/bad_self_ref.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/cached_prop.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/cached_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/circular_definition.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/circular_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/compound.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/compound.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/configure_traits.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/configure_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/custom_traithandler.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/custom_traithandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/deferring_notification.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/deferring_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/delegate.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/delegate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/disallow.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/disallow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/dynamic_notification.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/dynamic_notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/event.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/instance_trait_defaults.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/instance_trait_defaults.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/interface_definition.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/interface_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/interface_implementation.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/interface_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/keywords.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/lesson.desc` & `traits-6.4.2/examples/tutorials/doc_examples/examples/lesson.desc`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/list_notifier.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/list_notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/mapped.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/mapped.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/metadata.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/minimal.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/minimal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/object_trait_attrs.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/object_trait_attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/observe_decorator.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/observe_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/observe_different_events.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/observe_different_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/observe_method.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/observe_method.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/observe_optional.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/observe_optional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/observe_post_init.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/observe_post_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/override_default.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/override_default.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/post_init_notification.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/post_init_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/prototype_prefix.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/prototype_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/simple_adapter.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/simple_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/static_notification.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/static_notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/temp_wildcard.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/temp_wildcard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/this.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/this.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/trait_reuse.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/trait_reuse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/trait_subclass.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/trait_subclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/traitprefixmap.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/traitprefixmap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/transient_metadata.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/transient_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/use_custom_th.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/use_custom_th.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/widget.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-# wildcard.py --- Example of using a wildcard with a trait
-#                 attribute name
-from traits.api import Any, HasTraits
+# wildcard_all.py --- Example of using a wildcard with all trait
+#                     attribute names
+from traits.api import HasTraits, Any
 
 
 class Person(HasTraits):
-    temp_ = Any
+    _ = Any
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard_all.py` & `traits-6.4.2/traits/testing/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-# wildcard_all.py --- Example of using a wildcard with all trait
-#                     attribute names
-from traits.api import HasTraits, Any
+""" Scripts and assert tools related to running unit tests.
 
-
-class Person(HasTraits):
-    _ = Any
+These scripts also allow running test suites in separate processes and
+aggregating the results.
+"""
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard_name.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/wildcard_rules.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/wildcard_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/doc_examples/examples/wizard.py` & `traits-6.4.2/examples/tutorials/doc_examples/examples/wizard.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/0_introduction.py` & `traits-6.4.2/examples/tutorials/introduction/0_introduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/1_validation.py` & `traits-6.4.2/examples/tutorials/introduction/1_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/2_initialization.py` & `traits-6.4.2/examples/tutorials/introduction/2_initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/3_observation.py` & `traits-6.4.2/examples/tutorials/introduction/3_observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/4_properties.py` & `traits-6.4.2/examples/tutorials/introduction/4_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/5_documentation.py` & `traits-6.4.2/examples/tutorials/introduction/5_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/6_visualization.py` & `traits-6.4.2/examples/tutorials/introduction/6_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/introduction/default.css` & `traits-6.4.2/examples/tutorials/introduction/default.css`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/introduction/images/sample_0001.png` & `traits-6.4.2/examples/tutorials/introduction/images/sample_0001.png`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/introduction/images/sample_0002.png` & `traits-6.4.2/examples/tutorials/introduction/images/sample_0002.png`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/introduction/index.rst` & `traits-6.4.2/examples/tutorials/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/decorators/cached_property.py` & `traits-6.4.2/examples/tutorials/traits_4.0/decorators/cached_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/decorators/on_trait_change.py` & `traits-6.4.2/examples/tutorials/traits_4.0/decorators/on_trait_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/default.css` & `traits-6.4.2/examples/tutorials/traits_4.0/default.css`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/delegation/delegation.py` & `traits-6.4.2/examples/tutorials/traits_4.0/delegation/delegation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/extended_trait_change/extended_trait_change.py` & `traits-6.4.2/examples/tutorials/traits_4.0/extended_trait_change/extended_trait_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/extended_trait_change/properties.py` & `traits-6.4.2/examples/tutorials/traits_4.0/extended_trait_change/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/getstate_setstate/getstate.py` & `traits-6.4.2/examples/tutorials/traits_4.0/getstate_setstate/getstate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/interfaces/interfaces.py` & `traits-6.4.2/examples/tutorials/traits_4.0/interfaces/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/trait_types/core_traits.py` & `traits-6.4.2/examples/tutorials/traits_4.0/trait_types/core_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/trait_types/new_types.py` & `traits-6.4.2/examples/tutorials/traits_4.0/trait_types/new_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/traits_4.0/trait_types/trait_types.py` & `traits-6.4.2/examples/tutorials/traits_4.0/trait_types/trait_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/examples/tutorials/tutor.py` & `traits-6.4.2/examples/tutorials/tutor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/image_LICENSE.txt` & `traits-6.4.2/image_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/setup.py` & `traits-6.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -16,15 +16,15 @@
 
 # Version information; update this by hand when making a new bugfix or feature
 # release. The actual package version is autogenerated from this information
 # together with information from the version control system, and then injected
 # into the package source.
 MAJOR = 6
 MINOR = 4
-MICRO = 1
+MICRO = 2
 PRERELEASE = ""
 IS_RELEASED = True
 
 # If this file is part of a Git export (for example created with "git archive",
 # or downloaded from GitHub), ARCHIVE_COMMIT_HASH gives the full hash of the
 # commit that was exported.
 ARCHIVE_COMMIT_HASH = "$Format:%H$"
@@ -36,15 +36,15 @@
 # Paths to the autogenerated version file and the Git directory.
 HERE = os.path.abspath(os.path.dirname(__file__))
 VERSION_FILE = os.path.join(HERE, "traits", "version.py")
 GIT_DIRECTORY = os.path.join(HERE, ".git")
 
 # Template for the autogenerated version file.
 VERSION_FILE_TEMPLATE = '''\
-# (C) Copyright 2005-2022 {company}, Inc., Austin, TX
+# (C) Copyright 2005-2023 {company}, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -272,15 +272,14 @@
         Intended Audience :: Science/Research
         License :: OSI Approved :: BSD License
         Operating System :: MacOS :: MacOS X
         Operating System :: Microsoft :: Windows
         Operating System :: POSIX :: Linux
         Programming Language :: Python
         Programming Language :: Python :: 3
-        Programming Language :: Python :: 3.6
         Programming Language :: Python :: 3.7
         Programming Language :: Python :: 3.8
         Programming Language :: Python :: 3.9
         Programming Language :: Python :: 3.10
         Programming Language :: Python :: 3.11
         Programming Language :: Python :: Implementation :: CPython
         Topic :: Scientific/Engineering
@@ -299,28 +298,33 @@
         "Documentation": "https://docs.enthought.com/traits",
         "Source Code": "https://github.com/enthought/traits",
     },
     install_requires=[],
     extras_require={
         "docs": [
             "enthought-sphinx-theme",
-            "Sphinx>=2.1.0",
+            # Doc builds are hanging with pygments 2.15.0 and 2.15.1.
+            # Maybe related: https://github.com/pygments/pygments/issues/2427
+            "pygments<2.15",
+            "Sphinx",
             "sphinx-copybutton",
         ],
         "test": [
             "Cython",
             "flake8",
             "flake8-ets",
             "mypy",
             "numpy",
             "pyface",
-            "PySide2; python_version < '3.8'",
-            "PySide6; python_version >= '3.8' and python_version < '3.11'",
+            # Doc builds are hanging with pygments 2.15.0 and 2.15.1.
+            # Maybe related: https://github.com/pygments/pygments/issues/2427
+            "pygments<2.15",
+            "PySide6; python_version >= '3.7' and python_version < '3.12'",
             "setuptools",
-            "Sphinx>=2.1.0",
+            "Sphinx",
             "traitsui",
         ],
         "examples": [
             # dependencies for examples
             "numpy",
             "pillow",
         ]
@@ -340,10 +344,10 @@
     entry_points={
         "etsdemo_data": [
             "introduction = traits.examples._etsdemo_info:introduction",
         ],
     },
     license="BSD",
     packages=setuptools.find_packages(include=["traits", "traits.*"]),
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     zip_safe=False,
 )
```

### Comparing `traits-6.4.1/traits/__init__.py` & `traits-6.4.2/traits/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/adaptation_error.py` & `traits-6.4.2/traits/adaptation/adaptation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/adaptation_manager.py` & `traits-6.4.2/traits/adaptation/adaptation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/adaptation_offer.py` & `traits-6.4.2/traits/adaptation/adaptation_offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/adapter.py` & `traits-6.4.2/traits/adaptation/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/api.py` & `traits-6.4.2/traits/adaptation/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/abc_examples.py` & `traits-6.4.2/traits/adaptation/tests/abc_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/benchmark.py` & `traits-6.4.2/traits/adaptation/tests/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/interface_examples.py` & `traits-6.4.2/traits/adaptation/tests/interface_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/lazy_examples.py` & `traits-6.4.2/traits/adaptation/tests/lazy_examples.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/test_adaptation_manager.py` & `traits-6.4.2/traits/adaptation/tests/test_adaptation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/test_adaptation_offer.py` & `traits-6.4.2/traits/adaptation/tests/test_adaptation_offer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/test_adapter.py` & `traits-6.4.2/traits/adaptation/tests/test_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/adaptation/tests/test_global_adaptation_manager.py` & `traits-6.4.2/traits/adaptation/tests/test_global_adaptation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/api.py` & `traits-6.4.2/traits/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/base_trait_handler.py` & `traits-6.4.2/traits/base_trait_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/constants.py` & `traits-6.4.2/traits/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/ctrait.py` & `traits-6.4.2/traits/ctrait.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/ctraits.c` & `traits-6.4.2/traits/ctraits.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+// (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 // All rights reserved.
 //
 // This software is provided without warranty under the terms of the BSD
 // license included in LICENSE.txt and may be redistributed only under
 // the conditions described in the aforementioned license. The license
 // is also available online at http://www.enthought.com/licenses/BSD.txt
 //
```

### Comparing `traits-6.4.1/traits/editor_factories.py` & `traits-6.4.2/traits/editor_factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/etsconfig/__init__.py` & `traits-6.4.2/traits/etsconfig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/etsconfig/etsconfig.py` & `traits-6.4.2/traits/etsconfig/etsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/etsconfig/tests/test_etsconfig.py` & `traits-6.4.2/traits/etsconfig/tests/test_etsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/_etsdemo_info.py` & `traits-6.4.2/traits/examples/_etsdemo_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/0_introduction.py` & `traits-6.4.2/traits/examples/introduction/0_introduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/1_validation.py` & `traits-6.4.2/traits/examples/introduction/1_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/2_initialization.py` & `traits-6.4.2/traits/examples/introduction/2_initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/3_observation.py` & `traits-6.4.2/traits/examples/introduction/3_observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/4_properties.py` & `traits-6.4.2/traits/examples/introduction/4_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/5_documentation.py` & `traits-6.4.2/traits/examples/introduction/5_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/6_visualization.py` & `traits-6.4.2/traits/examples/introduction/6_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/examples/introduction/default.css` & `traits-6.4.2/traits/examples/introduction/default.css`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/traits/examples/introduction/images/sample_0001.png` & `traits-6.4.2/traits/examples/introduction/images/sample_0001.png`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/traits/examples/introduction/images/sample_0002.png` & `traits-6.4.2/traits/examples/introduction/images/sample_0002.png`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/traits/examples/introduction/index.rst` & `traits-6.4.2/traits/examples/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/traits/examples/tests/test_etsdemo_info.py` & `traits-6.4.2/traits/examples/tests/test_etsdemo_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/has_traits.py` & `traits-6.4.2/traits/has_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -52,15 +52,14 @@
     Undefined,
     is_none,
     not_event,
     not_false,
 )
 from .trait_errors import TraitError
 from .util.deprecated import deprecated
-from .util._traitsui_helpers import check_traitsui_major_version
 from .trait_converters import check_trait, mapped_trait_for, trait_for
 
 
 #  Set CHECK_INTERFACES to one of the following values:
 #
 #  - 0: Does not check to see if classes implement their declared interfaces.
 #  - 1: Ensures that classes implement the interfaces they say they do, and
@@ -1901,18 +1900,14 @@
         view_elements = view_elements()
 
         # The following test should only succeed for objects created before
         # traits has been fully initialized (such as the default Handler):
         if view_elements is None:
             return None
 
-        # Provide a nicer failure mode when upgrading to Traits using
-        # TraitsUI 6.x
-        check_traitsui_major_version(7)
-
         if name:
             if view_element is None:
                 # If only a name was specified, return the ViewElement it
                 # matches, if any:
                 result = view_elements.find(name)
                 if (result is None) and (handler is not None):
                     method = getattr(handler, name, None)
```

### Comparing `traits-6.4.1/traits/interface_checker.py` & `traits-6.4.2/traits/interface_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_anytrait_filter.py` & `traits-6.4.2/traits/observation/_anytrait_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_dict_change_event.py` & `traits-6.4.2/traits/observation/_dict_change_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_dict_item_observer.py` & `traits-6.4.2/traits/observation/_dict_item_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_dsl_grammar.lark` & `traits-6.4.2/traits/observation/_dsl_grammar.lark`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/traits/observation/_filtered_trait_observer.py` & `traits-6.4.2/traits/observation/_filtered_trait_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_generated_parser.py` & `traits-6.4.2/traits/observation/_generated_parser.py`

 * *Files identical despite different names*

### Comparing `traits-6.4.1/traits/observation/_has_traits_helpers.py` & `traits-6.4.2/traits/observation/_has_traits_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_i_notifier.py` & `traits-6.4.2/traits/observation/_i_notifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_i_observer.py` & `traits-6.4.2/traits/observation/_i_observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_list_change_event.py` & `traits-6.4.2/traits/observation/_list_change_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_list_item_observer.py` & `traits-6.4.2/traits/observation/_list_item_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_metadata_filter.py` & `traits-6.4.2/traits/observation/_metadata_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_named_trait_observer.py` & `traits-6.4.2/traits/observation/_named_trait_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_observe.py` & `traits-6.4.2/traits/observation/_observe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_observer_change_notifier.py` & `traits-6.4.2/traits/observation/_observer_change_notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_observer_graph.py` & `traits-6.4.2/traits/observation/_observer_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_set_change_event.py` & `traits-6.4.2/traits/observation/_set_change_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_set_item_observer.py` & `traits-6.4.2/traits/observation/_set_item_observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_testing.py` & `traits-6.4.2/traits/observation/_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_trait_added_observer.py` & `traits-6.4.2/traits/observation/_trait_added_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_trait_change_event.py` & `traits-6.4.2/traits/observation/_trait_change_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/_trait_event_notifier.py` & `traits-6.4.2/traits/observation/_trait_event_notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/api.py` & `traits-6.4.2/traits/observation/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/exception_handling.py` & `traits-6.4.2/traits/observation/exception_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/expression.py` & `traits-6.4.2/traits/observation/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/i_observable.py` & `traits-6.4.2/traits/observation/i_observable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/observe.py` & `traits-6.4.2/traits/observation/observe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/parsing.py` & `traits-6.4.2/traits/observation/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_dict_change_event.py` & `traits-6.4.2/traits/observation/tests/test_dict_change_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_dict_item_observer.py` & `traits-6.4.2/traits/observation/tests/test_dict_item_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_exception_handling.py` & `traits-6.4.2/traits/observation/tests/test_exception_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_expression.py` & `traits-6.4.2/traits/observation/tests/test_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_filtered_trait_observer.py` & `traits-6.4.2/traits/observation/tests/test_filtered_trait_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_generated_parser.py` & `traits-6.4.2/traits/observation/tests/test_generated_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_has_traits_helpers.py` & `traits-6.4.2/traits/observation/tests/test_has_traits_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_list_change_event.py` & `traits-6.4.2/traits/observation/tests/test_list_change_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_list_item_observer.py` & `traits-6.4.2/traits/observation/tests/test_list_item_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_metadata_filter.py` & `traits-6.4.2/traits/observation/tests/test_metadata_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_named_trait_observer.py` & `traits-6.4.2/traits/observation/tests/test_named_trait_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_observe.py` & `traits-6.4.2/traits/observation/tests/test_observe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_observer_change_notifier.py` & `traits-6.4.2/traits/observation/tests/test_observer_change_notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_observer_graph.py` & `traits-6.4.2/traits/observation/tests/test_observer_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_parsing.py` & `traits-6.4.2/traits/observation/tests/test_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_set_change_event.py` & `traits-6.4.2/traits/observation/tests/test_set_change_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_set_item_observer.py` & `traits-6.4.2/traits/observation/tests/test_set_item_observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_trait_added_observer.py` & `traits-6.4.2/traits/observation/tests/test_trait_added_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_trait_change_event.py` & `traits-6.4.2/traits/observation/tests/test_trait_change_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/observation/tests/test_trait_event_notifier.py` & `traits-6.4.2/traits/observation/tests/test_trait_event_notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/__init__.py` & `traits-6.4.2/traits/util/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-""" Scripts and assert tools related to running unit tests.
-
-These scripts also allow running test suites in separate processes and
-aggregating the results.
-"""
+from .deprecated import deprecated
+from .event_tracer import record_events
+from .import_symbol import import_symbol
```

### Comparing `traits-6.4.1/traits/testing/api.py` & `traits-6.4.2/traits/testing/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/doctest_tools.py` & `traits-6.4.2/traits/testing/doctest_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/nose_tools.py` & `traits-6.4.2/traits/testing/nose_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/optional_dependencies.py` & `traits-6.4.2/traits/testing/optional_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/tests/test_nose_tools.py` & `traits-6.4.2/traits/testing/tests/test_nose_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/tests/test_optional_dependencies.py` & `traits-6.4.2/traits/testing/tests/test_optional_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/tests/test_unittest_tools.py` & `traits-6.4.2/traits/testing/tests/test_unittest_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/testing/unittest_tools.py` & `traits-6.4.2/traits/testing/unittest_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/check_observe_timing.py` & `traits-6.4.2/traits/tests/check_observe_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/check_timing.py` & `traits-6.4.2/traits/tests/check_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test-data/historical-pickles/generate_pickles.py` & `traits-6.4.2/traits/tests/test-data/historical-pickles/generate_pickles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_abc.py` & `traits-6.4.2/traits/tests/test_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_any.py` & `traits-6.4.2/traits/tests/test_any.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_anytrait_static_notifiers.py` & `traits-6.4.2/traits/tests/test_anytrait_static_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_array.py` & `traits-6.4.2/traits/tests/test_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_array_or_none.py` & `traits-6.4.2/traits/tests/test_array_or_none.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_automatic_adaptation.py` & `traits-6.4.2/traits/tests/test_automatic_adaptation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_bool.py` & `traits-6.4.2/traits/tests/test_bool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_callable.py` & `traits-6.4.2/traits/tests/test_callable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_class_traits.py` & `traits-6.4.2/traits/tests/test_class_traits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_clone.py` & `traits-6.4.2/traits/tests/test_clone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_complex.py` & `traits-6.4.2/traits/tests/test_complex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_configure_traits.py` & `traits-6.4.2/traits/tests/test_configure_traits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -151,8 +151,12 @@
         model = Model()
         with mock.patch.object(self.toolkit, "view_application") as mock_view:
             mock_view.return_value = True
             with warnings.catch_warnings(record=True) as captured_warnings:
                 warnings.simplefilter("always", DeprecationWarning)
                 model.configure_traits()
         mock_view.assert_called_once()
-        self.assertEqual(len(captured_warnings), 0)
+
+        all_warnings = "".join(
+            str(warning.message) for warning in captured_warnings
+        )
+        self.assertNotIn("edit argument", all_warnings)
```

### Comparing `traits-6.4.1/traits/tests/test_constant.py` & `traits-6.4.2/traits/tests/test_constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_constants.py` & `traits-6.4.2/traits/tests/test_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_container_events.py` & `traits-6.4.2/traits/tests/test_container_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_copy_traits.py` & `traits-6.4.2/traits/tests/test_copy_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_copyable_trait_names.py` & `traits-6.4.2/traits/tests/test_copyable_trait_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_ctraits.py` & `traits-6.4.2/traits/tests/test_ctraits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_cythonized_traits.py` & `traits-6.4.2/traits/tests/test_cythonized_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_date.py` & `traits-6.4.2/traits/tests/test_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_datetime.py` & `traits-6.4.2/traits/tests/test_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_delegate.py` & `traits-6.4.2/traits/tests/test_delegate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_deprecated_handlers.py` & `traits-6.4.2/traits/tests/test_deprecated_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_dict.py` & `traits-6.4.2/traits/tests/test_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_directory.py` & `traits-6.4.2/traits/tests/test_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_dynamic_notifiers.py` & `traits-6.4.2/traits/tests/test_dynamic_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_dynamic_trait_definition.py` & `traits-6.4.2/traits/tests/test_dynamic_trait_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_editor_factories.py` & `traits-6.4.2/traits/tests/test_editor_factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_enum.py` & `traits-6.4.2/traits/tests/test_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_event_order.py` & `traits-6.4.2/traits/tests/test_event_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_expression.py` & `traits-6.4.2/traits/tests/test_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_extended_notifiers.py` & `traits-6.4.2/traits/tests/test_extended_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_extended_trait_change.py` & `traits-6.4.2/traits/tests/test_extended_trait_change.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_file.py` & `traits-6.4.2/traits/tests/test_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_float.py` & `traits-6.4.2/traits/tests/test_float.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_float_range.py` & `traits-6.4.2/traits/tests/test_float_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_get_traits.py` & `traits-6.4.2/traits/tests/test_get_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_has_required_traits.py` & `traits-6.4.2/traits/tests/test_has_required_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_has_traits.py` & `traits-6.4.2/traits/tests/test_has_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_historical_unpickling.py` & `traits-6.4.2/traits/tests/test_historical_unpickling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_instance.py` & `traits-6.4.2/traits/tests/test_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_int_range_long.py` & `traits-6.4.2/traits/tests/test_int_range_long.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_integer.py` & `traits-6.4.2/traits/tests/test_integer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_integer_range.py` & `traits-6.4.2/traits/tests/test_integer_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_interface_checker.py` & `traits-6.4.2/traits/tests/test_interface_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_interfaces.py` & `traits-6.4.2/traits/tests/test_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_keyword_args.py` & `traits-6.4.2/traits/tests/test_keyword_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_list.py` & `traits-6.4.2/traits/tests/test_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_list_events.py` & `traits-6.4.2/traits/tests/test_list_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_listeners.py` & `traits-6.4.2/traits/tests/test_listeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_long_traits.py` & `traits-6.4.2/traits/tests/test_long_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_map.py` & `traits-6.4.2/traits/tests/test_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_new_notifiers.py` & `traits-6.4.2/traits/tests/test_new_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_none.py` & `traits-6.4.2/traits/tests/test_none.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_observe.py` & `traits-6.4.2/traits/tests/test_observe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_pickle_validated_dict.py` & `traits-6.4.2/traits/tests/test_pickle_validated_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_prefix_list.py` & `traits-6.4.2/traits/tests/test_prefix_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_prefix_map.py` & `traits-6.4.2/traits/tests/test_prefix_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_property_delete.py` & `traits-6.4.2/traits/tests/test_property_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_property_notifications.py` & `traits-6.4.2/traits/tests/test_property_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_python_properties.py` & `traits-6.4.2/traits/tests/test_python_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_range.py` & `traits-6.4.2/traits/tests/test_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_readonly.py` & `traits-6.4.2/traits/tests/test_readonly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_regression.py` & `traits-6.4.2/traits/tests/test_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_rich_compare.py` & `traits-6.4.2/traits/tests/test_rich_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_special_event_handlers.py` & `traits-6.4.2/traits/tests/test_special_event_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_static_notifiers.py` & `traits-6.4.2/traits/tests/test_static_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_str_handler.py` & `traits-6.4.2/traits/tests/test_str_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_string.py` & `traits-6.4.2/traits/tests/test_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_sync_traits.py` & `traits-6.4.2/traits/tests/test_sync_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_target.py` & `traits-6.4.2/traits/tests/test_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_time.py` & `traits-6.4.2/traits/tests/test_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_base.py` & `traits-6.4.2/traits/tests/test_trait_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_change_event_tracer.py` & `traits-6.4.2/traits/tests/test_trait_change_event_tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_converters.py` & `traits-6.4.2/traits/tests/test_trait_converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_cycle.py` & `traits-6.4.2/traits/tests/test_trait_cycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_default_initializer.py` & `traits-6.4.2/traits/tests/test_trait_default_initializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_dict_list_set_event.py` & `traits-6.4.2/traits/tests/test_trait_dict_list_set_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_dict_object.py` & `traits-6.4.2/traits/tests/test_trait_dict_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_exceptions.py` & `traits-6.4.2/traits/tests/test_trait_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_get_set.py` & `traits-6.4.2/traits/tests/test_trait_get_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_list_dict.py` & `traits-6.4.2/traits/tests/test_trait_list_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_list_object.py` & `traits-6.4.2/traits/tests/test_trait_list_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_prefix_list.py` & `traits-6.4.2/traits/tests/test_trait_prefix_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_set_object.py` & `traits-6.4.2/traits/tests/test_trait_set_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_trait_types.py` & `traits-6.4.2/traits/tests/test_trait_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_traits.py` & `traits-6.4.2/traits/tests/test_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_traits_listener.py` & `traits-6.4.2/traits/tests/test_traits_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_tuple.py` & `traits-6.4.2/traits/tests/test_tuple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_type.py` & `traits-6.4.2/traits/tests/test_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_ui_notifiers.py` & `traits-6.4.2/traits/tests/test_ui_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_undefined.py` & `traits-6.4.2/traits/tests/test_undefined.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_unicode_traits.py` & `traits-6.4.2/traits/tests/test_unicode_traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_union.py` & `traits-6.4.2/traits/tests/test_union.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_uuid.py` & `traits-6.4.2/traits/tests/test_uuid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_validated_tuple.py` & `traits-6.4.2/traits/tests/test_validated_tuple.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_version.py` & `traits-6.4.2/traits/tests/test_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_view_elements.py` & `traits-6.4.2/traits/tests/test_view_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/test_weak_ref.py` & `traits-6.4.2/traits/tests/test_weak_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/tests/tuple_test_mixin.py` & `traits-6.4.2/traits/tests/tuple_test_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_base.py` & `traits-6.4.2/traits/trait_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_converters.py` & `traits-6.4.2/traits/trait_converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_dict_object.py` & `traits-6.4.2/traits/trait_dict_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_errors.py` & `traits-6.4.2/traits/trait_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_factory.py` & `traits-6.4.2/traits/trait_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_handler.py` & `traits-6.4.2/traits/trait_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_handlers.py` & `traits-6.4.2/traits/trait_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_list_object.py` & `traits-6.4.2/traits/trait_list_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_notifiers.py` & `traits-6.4.2/traits/trait_notifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_numeric.py` & `traits-6.4.2/traits/trait_numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_set_object.py` & `traits-6.4.2/traits/trait_set_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_type.py` & `traits-6.4.2/traits/trait_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/trait_types.py` & `traits-6.4.2/traits/trait_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/traits.py` & `traits-6.4.2/traits/traits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/traits_listener.py` & `traits-6.4.2/traits/traits_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/async_trait_wait.py` & `traits-6.4.2/traits/util/async_trait_wait.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/camel_case.py` & `traits-6.4.2/traits/util/camel_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/clean_strings.py` & `traits-6.4.2/traits/util/clean_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/deprecated.py` & `traits-6.4.2/traits/util/deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/event_tracer.py` & `traits-6.4.2/traits/util/event_tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/home_directory.py` & `traits-6.4.2/traits/util/home_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/import_symbol.py` & `traits-6.4.2/traits/util/import_symbol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/resource.py` & `traits-6.4.2/traits/util/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_async_trait_wait.py` & `traits-6.4.2/traits/util/tests/test_async_trait_wait.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_camel_case.py` & `traits-6.4.2/traits/util/tests/test_camel_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_clean_strings.py` & `traits-6.4.2/traits/util/tests/test_clean_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_deprecated.py` & `traits-6.4.2/traits/util/tests/test_deprecated.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_import_symbol.py` & `traits-6.4.2/traits/util/tests/test_import_symbol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_message_records.py` & `traits-6.4.2/traits/util/tests/test_message_records.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_record_containers.py` & `traits-6.4.2/traits/util/tests/test_record_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_record_events.py` & `traits-6.4.2/traits/util/tests/test_record_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_resource.py` & `traits-6.4.2/traits/util/tests/test_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_trait_documenter.py` & `traits-6.4.2/traits/util/tests/test_trait_documenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/tests/test_weakidddict.py` & `traits-6.4.2/traits/util/tests/test_weakidddict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/toposort.py` & `traits-6.4.2/traits/util/toposort.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/trait_documenter.py` & `traits-6.4.2/traits/util/trait_documenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/util/weakiddict.py` & `traits-6.4.2/traits/util/weakiddict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
```

### Comparing `traits-6.4.1/traits/version.py` & `traits-6.4.2/traits/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (C) Copyright 2005-2022 Enthought, Inc., Austin, TX
+# (C) Copyright 2005-2023 Enthought, Inc., Austin, TX
 # All rights reserved.
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
@@ -12,11 +12,11 @@
 Version information for this Traits distribution.
 
 This file is autogenerated by the Traits setup.py script.
 """
 
 #: The full version of the package, including a development suffix
 #: for unreleased versions of the package.
-version = "6.4.1"
+version = "6.4.2"
 
 #: The Git revision from which this release was made.
-git_revision = "5bb7f22adbc5e3b4416369e00002a47dcc4ff2aa"
+git_revision = "93583b90bdc43c6174bf5d5a532802edbfafc6ef"
```

### Comparing `traits-6.4.1/traits.egg-info/PKG-INFO` & `traits-6.4.2/traits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traits
-Version: 6.4.1
+Version: 6.4.2
 Summary: Observable typed attributes for Python classes
 Home-page: http://docs.enthought.com/traits
 Download-URL: https://pypi.python.org/pypi/traits
 Author: Enthought
 Author-email: info@enthought.com
 License: BSD
 Project-URL: Issue Tracker, https://github.com/enthought/traits/issues
@@ -15,26 +15,25 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: examples
 License-File: LICENSE-CC-BY-3.0.txt
 License-File: LICENSE.txt
 
@@ -76,15 +75,15 @@
 or can opt to allow the use of only a fixed or open set of trait attributes
 within the class. Trait attributes defined by a class are automatically
 inherited by any subclass derived from the class.
 
 Dependencies
 ------------
 
-Traits requires Python >= 3.6.
+Traits requires Python >= 3.7.
 
 Traits has the following optional dependencies:
 
 * `NumPy <http://pypi.python.org/pypi/numpy>`_ to support the trait types
   for arrays.
 * `TraitsUI <https://pypi.python.org/pypi/traitsui>`_ to support GUI
   Views.
```

### Comparing `traits-6.4.1/traits.egg-info/SOURCES.txt` & `traits-6.4.2/traits.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,14 @@
 traits/tests/test-data/historical-pickles/hipt-t5.2.0-p0-float-ctrait.pkl
 traits/tests/test-data/historical-pickles/hipt-t5.2.0-p1-float-ctrait.pkl
 traits/tests/test-data/historical-pickles/hipt-t5.2.0-p2-float-ctrait.pkl
 traits/tests/test-data/historical-pickles/hipt-t5.2.0-p3-float-ctrait.pkl
 traits/tests/test-data/historical-pickles/hipt-t5.2.0-p4-float-ctrait.pkl
 traits/tests/test-data/historical-pickles/hipt-t5.2.0-p5-float-ctrait.pkl
 traits/util/__init__.py
-traits/util/_traitsui_helpers.py
 traits/util/api.py
 traits/util/async_trait_wait.py
 traits/util/camel_case.py
 traits/util/clean_strings.py
 traits/util/deprecated.py
 traits/util/event_tracer.py
 traits/util/home_directory.py
@@ -410,9 +409,8 @@
 traits/util/tests/test_deprecated.py
 traits/util/tests/test_import_symbol.py
 traits/util/tests/test_message_records.py
 traits/util/tests/test_record_containers.py
 traits/util/tests/test_record_events.py
 traits/util/tests/test_resource.py
 traits/util/tests/test_trait_documenter.py
-traits/util/tests/test_traitsui_helpers.py
 traits/util/tests/test_weakidddict.py
```

