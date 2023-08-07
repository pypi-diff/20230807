# Comparing `tmp/django-unicorn-0.9.3.tar.gz` & `tmp/django-unicorn-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-unicorn-0.9.3.tar", last modified: Mon Nov 23 00:59:15 2020, max compression
+gzip compressed data, was "django-unicorn-0.9.4.tar", last modified: Wed Nov 25 01:43:10 2020, max compression
```

## Comparing `django-unicorn-0.9.3.tar` & `django-unicorn-0.9.4.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0     1065 2020-11-06 22:18:18.986820 django-unicorn-0.9.3/LICENSE
--rw-r--r--   0        0        0     3661 2020-11-23 00:49:23.218742 django-unicorn-0.9.3/README.md
--rw-r--r--   0        0        0        0 2020-11-06 22:18:18.987360 django-unicorn-0.9.3/django_unicorn/__init__.py
--rw-r--r--   0        0        0     3533 2020-11-06 22:18:18.987496 django-unicorn-0.9.3/django_unicorn/call_method_parser.py
--rw-r--r--   0        0        0    21943 2020-11-12 03:15:07.883751 django-unicorn-0.9.3/django_unicorn/components.py
--rw-r--r--   0        0        0      228 2020-11-06 22:18:18.988062 django-unicorn-0.9.3/django_unicorn/db.py
--rw-r--r--   0        0        0       44 2020-11-06 22:18:18.988296 django-unicorn-0.9.3/django_unicorn/errors.py
--rw-r--r--   0        0        0     2309 2020-11-06 22:18:18.988638 django-unicorn-0.9.3/django_unicorn/management/commands/startunicorn.py
--rw-r--r--   0        0        0     1948 2020-11-06 22:18:18.988829 django-unicorn-0.9.3/django_unicorn/serializer.py
--rw-r--r--   0        0        0      402 2020-11-06 22:18:18.988972 django-unicorn-0.9.3/django_unicorn/settings.py
--rw-r--r--   0        0        0      133 2020-11-06 22:18:18.989232 django-unicorn-0.9.3/django_unicorn/static/js/.babelrc.json
--rw-r--r--   0        0        0     2490 2020-11-19 00:27:26.046838 django-unicorn-0.9.3/django_unicorn/static/js/attribute.js
--rw-r--r--   0        0        0     9166 2020-11-22 20:43:49.721708 django-unicorn-0.9.3/django_unicorn/static/js/component.js
--rw-r--r--   0        0        0     1581 2020-11-06 22:18:18.990073 django-unicorn-0.9.3/django_unicorn/static/js/delayers.js
--rw-r--r--   0        0        0     7783 2020-11-23 00:57:22.681645 django-unicorn-0.9.3/django_unicorn/static/js/element.js
--rw-r--r--   0        0        0     9736 2020-11-23 00:43:38.356319 django-unicorn-0.9.3/django_unicorn/static/js/eventListeners.js
--rw-r--r--   0        0        0     3222 2020-11-22 20:43:58.195008 django-unicorn-0.9.3/django_unicorn/static/js/messageSender.js
--rw-r--r--   0        0        0    11698 2020-11-06 22:18:18.991478 django-unicorn-0.9.3/django_unicorn/static/js/morphdom/2.6.1/morphdom-umd.min.js
--rw-r--r--   0        0        0    27358 2020-11-06 22:18:18.991950 django-unicorn-0.9.3/django_unicorn/static/js/morphdom/2.6.1/morphdom.js
--rw-r--r--   0        0        0      794 2020-11-12 03:24:06.036066 django-unicorn-0.9.3/django_unicorn/static/js/morphdom/2.6.1/options.js
--rw-r--r--   0        0        0     1108 2020-11-06 22:18:18.992662 django-unicorn-0.9.3/django_unicorn/static/js/unicorn.js
--rw-r--r--   0        0        0    20159 2020-11-23 00:59:05.706333 django-unicorn-0.9.3/django_unicorn/static/js/unicorn.min.js
--rw-r--r--   0        0        0     4015 2020-11-22 20:44:06.695825 django-unicorn-0.9.3/django_unicorn/static/js/utils.js
--rw-r--r--   0        0        0      304 2020-11-06 22:18:18.993906 django-unicorn-0.9.3/django_unicorn/templates/unicorn/errors.html
--rw-r--r--   0        0        0      478 2020-11-06 22:18:18.994470 django-unicorn-0.9.3/django_unicorn/templates/unicorn/scripts.html
--rw-r--r--   0        0        0        0 2020-11-06 22:18:18.994744 django-unicorn-0.9.3/django_unicorn/templatetags/__init__.py
--rw-r--r--   0        0        0     1355 2020-11-06 22:18:18.995017 django-unicorn-0.9.3/django_unicorn/templatetags/unicorn.py
--rw-r--r--   0        0        0      293 2020-11-06 22:18:18.995250 django-unicorn-0.9.3/django_unicorn/urls.py
--rw-r--r--   0        0        0      282 2020-11-06 22:18:18.995463 django-unicorn-0.9.3/django_unicorn/utils.py
--rw-r--r--   0        0        0    13313 2020-11-12 03:25:43.119153 django-unicorn-0.9.3/django_unicorn/views.py
--rw-r--r--   0        0        0     1120 2020-11-23 00:59:09.184116 django-unicorn-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     4685 2020-11-23 00:59:16.509975 django-unicorn-0.9.3/setup.py
--rw-r--r--   0        0        0     4524 2020-11-23 00:59:16.510396 django-unicorn-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-11-06 22:18:18.986820 django-unicorn-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3661 2020-11-23 00:49:23.218742 django-unicorn-0.9.4/README.md
+-rw-r--r--   0        0        0        0 2020-11-06 22:18:18.987360 django-unicorn-0.9.4/django_unicorn/__init__.py
+-rw-r--r--   0        0        0     3533 2020-11-06 22:18:18.987496 django-unicorn-0.9.4/django_unicorn/call_method_parser.py
+-rw-r--r--   0        0        0    22827 2020-11-25 01:39:52.786478 django-unicorn-0.9.4/django_unicorn/components.py
+-rw-r--r--   0        0        0      228 2020-11-06 22:18:18.988062 django-unicorn-0.9.4/django_unicorn/db.py
+-rw-r--r--   0        0        0       44 2020-11-06 22:18:18.988296 django-unicorn-0.9.4/django_unicorn/errors.py
+-rw-r--r--   0        0        0     2309 2020-11-06 22:18:18.988638 django-unicorn-0.9.4/django_unicorn/management/commands/startunicorn.py
+-rw-r--r--   0        0        0     1948 2020-11-06 22:18:18.988829 django-unicorn-0.9.4/django_unicorn/serializer.py
+-rw-r--r--   0        0        0      402 2020-11-06 22:18:18.988972 django-unicorn-0.9.4/django_unicorn/settings.py
+-rw-r--r--   0        0        0      133 2020-11-06 22:18:18.989232 django-unicorn-0.9.4/django_unicorn/static/js/.babelrc.json
+-rw-r--r--   0        0        0     2490 2020-11-19 00:27:26.046838 django-unicorn-0.9.4/django_unicorn/static/js/attribute.js
+-rw-r--r--   0        0        0     9166 2020-11-22 20:43:49.721708 django-unicorn-0.9.4/django_unicorn/static/js/component.js
+-rw-r--r--   0        0        0     1581 2020-11-06 22:18:18.990073 django-unicorn-0.9.4/django_unicorn/static/js/delayers.js
+-rw-r--r--   0        0        0     8177 2020-11-25 00:32:03.363740 django-unicorn-0.9.4/django_unicorn/static/js/element.js
+-rw-r--r--   0        0        0     9351 2020-11-25 00:45:38.729666 django-unicorn-0.9.4/django_unicorn/static/js/eventListeners.js
+-rw-r--r--   0        0        0     3222 2020-11-22 20:43:58.195008 django-unicorn-0.9.4/django_unicorn/static/js/messageSender.js
+-rw-r--r--   0        0        0    11698 2020-11-06 22:18:18.991478 django-unicorn-0.9.4/django_unicorn/static/js/morphdom/2.6.1/morphdom-umd.min.js
+-rw-r--r--   0        0        0    27358 2020-11-06 22:18:18.991950 django-unicorn-0.9.4/django_unicorn/static/js/morphdom/2.6.1/morphdom.js
+-rw-r--r--   0        0        0      794 2020-11-12 03:24:06.036066 django-unicorn-0.9.4/django_unicorn/static/js/morphdom/2.6.1/options.js
+-rw-r--r--   0        0        0     1108 2020-11-06 22:18:18.992662 django-unicorn-0.9.4/django_unicorn/static/js/unicorn.js
+-rw-r--r--   0        0        0    20321 2020-11-25 01:41:44.398565 django-unicorn-0.9.4/django_unicorn/static/js/unicorn.min.js
+-rw-r--r--   0        0        0     4069 2020-11-25 00:44:24.382543 django-unicorn-0.9.4/django_unicorn/static/js/utils.js
+-rw-r--r--   0        0        0      694 2020-11-24 02:51:43.389968 django-unicorn-0.9.4/django_unicorn/static/svg/oval.svg
+-rw-r--r--   0        0        0     1784 2020-11-24 02:47:01.534045 django-unicorn-0.9.4/django_unicorn/static/svg/rings.svg
+-rw-r--r--   0        0        0     2794 2020-11-24 02:48:45.150935 django-unicorn-0.9.4/django_unicorn/static/svg/spinning-circles.svg
+-rw-r--r--   0        0        0      304 2020-11-06 22:18:18.993906 django-unicorn-0.9.4/django_unicorn/templates/unicorn/errors.html
+-rw-r--r--   0        0        0      478 2020-11-06 22:18:18.994470 django-unicorn-0.9.4/django_unicorn/templates/unicorn/scripts.html
+-rw-r--r--   0        0        0        0 2020-11-06 22:18:18.994744 django-unicorn-0.9.4/django_unicorn/templatetags/__init__.py
+-rw-r--r--   0        0        0     1355 2020-11-06 22:18:18.995017 django-unicorn-0.9.4/django_unicorn/templatetags/unicorn.py
+-rw-r--r--   0        0        0      293 2020-11-06 22:18:18.995250 django-unicorn-0.9.4/django_unicorn/urls.py
+-rw-r--r--   0        0        0      282 2020-11-06 22:18:18.995463 django-unicorn-0.9.4/django_unicorn/utils.py
+-rw-r--r--   0        0        0    13313 2020-11-25 01:34:21.558682 django-unicorn-0.9.4/django_unicorn/views.py
+-rw-r--r--   0        0        0     1120 2020-11-25 01:41:57.681661 django-unicorn-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     4721 2020-11-25 01:43:10.867389 django-unicorn-0.9.4/setup.py
+-rw-r--r--   0        0        0     4524 2020-11-25 01:43:10.868153 django-unicorn-0.9.4/PKG-INFO
```

### Comparing `django-unicorn-0.9.3/LICENSE` & `django-unicorn-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/README.md` & `django-unicorn-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/call_method_parser.py` & `django-unicorn-0.9.4/django_unicorn/call_method_parser.py`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/components.py` & `django-unicorn-0.9.4/django_unicorn/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,15 +306,23 @@
             for key in attributes.keys():
                 if key in form.fields:
                     field = form.fields[key]
 
                     if key in form.cleaned_data:
                         cleaned_value = form.cleaned_data[key]
                         value = field.widget.format_value(cleaned_value)
-                        frontend_context_variables[key] = value
+
+                        # Don't update the frontend variable if the only change is
+                        # stripping off the whitespace from the field value
+                        # https://docs.djangoproject.com/en/stable/ref/forms/fields/#django.forms.CharField.strip
+                        if (
+                            not hasattr(frontend_context_variables[key], "strip")
+                            or frontend_context_variables[key].strip() != value
+                        ):
+                            frontend_context_variables[key] = value
 
         encoded_frontend_context_variables = serializer.dumps(
             frontend_context_variables
         )
 
         return encoded_frontend_context_variables
 
@@ -419,15 +427,20 @@
     def _set_property(self, name, value):
         # Get the correct value type by using the form if it is available
         data = self._attributes()
         data[name] = value
         form = self._get_form(data)
 
         if form and name in form.fields and name in form.cleaned_data:
-            value = form.cleaned_data[name]
+            # The Django form CharField validator will remove whitespace
+            # from the field value. Ignore that update if it's the
+            # only thing different from the validator
+            # https://docs.djangoproject.com/en/stable/ref/forms/fields/#django.forms.CharField.strip
+            if not hasattr(value, "strip") or form.cleaned_data[name] != value.strip():
+                value = form.cleaned_data[name]
 
         updating_function_name = f"updating_{name}"
         if hasattr(self, updating_function_name):
             getattr(self, updating_function_name)(value)
 
         try:
             setattr(self, name, value)
```

### Comparing `django-unicorn-0.9.3/django_unicorn/management/commands/startunicorn.py` & `django-unicorn-0.9.4/django_unicorn/management/commands/startunicorn.py`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/serializer.py` & `django-unicorn-0.9.4/django_unicorn/serializer.py`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/attribute.js` & `django-unicorn-0.9.4/django_unicorn/static/js/attribute.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/component.js` & `django-unicorn-0.9.4/django_unicorn/static/js/component.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/delayers.js` & `django-unicorn-0.9.4/django_unicorn/static/js/delayers.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/element.js` & `django-unicorn-0.9.4/django_unicorn/static/js/element.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -223,14 +223,29 @@
             parentElement = parentElement.parent;
         }
 
         return parentElement;
     }
 
     /**
+     * Handle loading for the element.
+     */
+    handleLoading() {
+        if (this.loading) {
+            if (this.loading.attr) {
+                this.el[this.loading.attr] = this.loading.attr;
+            } else if (this.loading.class) {
+                this.el.classList.add(this.loading.class);
+            } else if (this.loading.removeClass) {
+                this.el.classList.remove(this.loading.removeClass);
+            }
+        }
+    }
+
+    /**
      * Check if another `Element` is the same as this `Element`.
      * @param {Element} other
      */
     isSame(other) {
         // Use isSameNode (not isEqualNode) because we want to check the nodes reference the same object
         return this.el.isSameNode(other.el);
     }
```

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/eventListeners.js` & `django-unicorn-0.9.4/django_unicorn/static/js/eventListeners.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -7,14 +7,52 @@
     toKebabCase,
 } from "./utils.js";
 import {
     Element
 } from "./element.js";
 
 /**
+ * Handles loading elements in the component.
+ * @param {Component} component Component.
+ * @param {Element} targetElement Targetted element.
+ */
+function handleLoading(component, targetElement) {
+    targetElement.handleLoading();
+
+    // Look at all elements with a loading attribute
+    component.loadingEls.forEach((loadingElement) => {
+        if (loadingElement.target) {
+            let targetedEl = $(`#${loadingElement.target}`, component.root);
+
+            if (!targetedEl) {
+                component.keyEls.forEach((keyElement) => {
+                    if (!targetedEl && keyElement.key === loadingElement.target) {
+                        targetedEl = keyElement.el;
+                    }
+                });
+            }
+
+            if (targetedEl) {
+                if (targetElement.el.isSameNode(targetedEl)) {
+                    if (loadingElement.loading.hide) {
+                        loadingElement.hide();
+                    } else if (loadingElement.loading.show) {
+                        loadingElement.show();
+                    }
+                }
+            }
+        } else if (loadingElement.loading.hide) {
+            loadingElement.hide();
+        } else if (loadingElement.loading.show) {
+            loadingElement.show();
+        }
+    });
+}
+
+/**
  * Adds an action event listener to the document for each type of event (e.g. click, keyup, etc).
  * Added at the document level because validation errors would sometimes remove the
  * events when attached directly to the element.
  * @param {Component} component Component that contains the element.
  * @param {string} eventType Event type to listen for.
  */
 export function addActionEventListener(component, eventType) {
@@ -139,61 +177,21 @@
                                     originalSpecialVariable,
                                     data
                                 );
                             }
                         }
                     });
 
-                    if (targetElement.loading) {
-                        if (targetElement.loading.attr) {
-                            targetElement.el[targetElement.loading.attr] =
-                                targetElement.loading.attr;
-                        } else if (targetElement.loading.class) {
-                            targetElement.el.classList.add(targetElement.loading.class);
-                        } else if (targetElement.loading.removeClass) {
-                            targetElement.el.classList.remove(
-                                targetElement.loading.removeClass
-                            );
-                        }
-                    }
-
-                    // Look at all elements with a loading attribute
-                    component.loadingEls.forEach((loadingElement) => {
-                        if (loadingElement.target) {
-                            let targetedEl = $(`#${loadingElement.target}`, component.root);
-
-                            if (!targetedEl) {
-                                component.keyEls.forEach((keyElement) => {
-                                    if (!targetedEl && keyElement.key === loadingElement.target) {
-                                        targetedEl = keyElement.el;
-                                    }
-                                });
-                            }
-
-                            if (targetedEl) {
-                                if (targetElement.el.isSameNode(targetedEl)) {
-                                    if (loadingElement.loading.hide) {
-                                        loadingElement.hide();
-                                    } else if (loadingElement.loading.show) {
-                                        loadingElement.show();
-                                    }
-                                }
-                            }
-                        } else if (loadingElement.loading.hide) {
-                            loadingElement.hide();
-                        } else if (loadingElement.loading.show) {
-                            loadingElement.show();
-                        }
-                    });
-
                     if (action.key) {
                         if (action.key === toKebabCase(event.key)) {
+                            handleLoading(component, targetElement);
                             component.callMethod(action.name);
                         }
                     } else {
+                        handleLoading(component, targetElement);
                         component.callMethod(action.name);
                     }
                 }
             });
         }
     });
 }
```

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/messageSender.js` & `django-unicorn-0.9.4/django_unicorn/static/js/messageSender.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/morphdom/2.6.1/morphdom-umd.min.js` & `django-unicorn-0.9.4/django_unicorn/static/js/morphdom/2.6.1/morphdom-umd.min.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/morphdom/2.6.1/morphdom.js` & `django-unicorn-0.9.4/django_unicorn/static/js/morphdom/2.6.1/morphdom.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/morphdom/2.6.1/options.js` & `django-unicorn-0.9.4/django_unicorn/static/js/morphdom/2.6.1/options.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/unicorn.js` & `django-unicorn-0.9.4/django_unicorn/static/js/unicorn.js`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/unicorn.min.js` & `django-unicorn-0.9.4/django_unicorn/static/js/unicorn.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -155,14 +155,19 @@
                     for (var e = this.parent; e && !e.isUnicorn;) {
                         if (e.el.getAttribute("unicorn:checksum")) return null;
                         e = e.parent
                     }
                     return e
                 }
             }, {
+                key: "handleLoading",
+                value: function() {
+                    this.loading && (this.loading.attr ? this.el[this.loading.attr] = this.loading.attr : this.loading.class ? this.el.classList.add(this.loading.class) : this.loading.removeClass && this.el.classList.remove(this.loading.removeClass))
+                }
+            }, {
                 key: "isSame",
                 value: function(e) {
                     return this.el.isSameNode(e.el)
                 }
             }, {
                 key: "getValue",
                 value: function() {
@@ -355,26 +360,26 @@
                     if (1 === t.nodeType || 11 === t.nodeType)
                         for (var i = t.firstChild; i;) {
                             var n = o(i);
                             n && (m[n] = i), e(i), i = i.nextSibling
                         }
                 }(t);
                 var C, U, V = t,
-                    M = V.nodeType,
-                    L = i.nodeType;
+                    L = V.nodeType,
+                    M = i.nodeType;
                 if (!f)
-                    if (1 === M) 1 === L ? b(t, i) || (d(t), V = function(e, t) {
+                    if (1 === L) 1 === M ? b(t, i) || (d(t), V = function(e, t) {
                         for (var i = e.firstChild; i;) {
                             var n = i.nextSibling;
                             t.appendChild(i), i = n
                         }
                         return t
                     }(t, (C = i.nodeName, (U = i.namespaceURI) && "http://www.w3.org/1999/xhtml" !== U ? v.createElementNS(U, C) : v.createElement(C)))) : V = i;
-                    else if (3 === M || 8 === M) {
-                    if (L === M) return V.nodeValue !== i.nodeValue && (V.nodeValue = i.nodeValue), V;
+                    else if (3 === L || 8 === L) {
+                    if (M === L) return V.nodeValue !== i.nodeValue && (V.nodeValue = i.nodeValue), V;
                     V = i
                 }
                 if (V === i) d(t);
                 else {
                     if (i.isSameNode && i.isSameNode(V)) return;
                     if (w(V, i, f), p)
                         for (var O = 0, P = p.length; O < P; O++) {
@@ -454,20 +459,31 @@
             })).catch((function(i) {
                 e.actionQueue = [], e.currentActionQueue = null, e.lastTriggeringElements = [], s(t) && t(null, null, i)
             }))
         }
     }
 
     function C(e, t) {
+        t.handleLoading(), e.loadingEls.forEach((function(i) {
+            if (i.target) {
+                var n = u("#".concat(i.target), e.root);
+                n || e.keyEls.forEach((function(e) {
+                    n || e.key !== i.target || (n = e.el)
+                })), n && t.el.isSameNode(n) && (i.loading.hide ? i.hide() : i.loading.show && i.show())
+            } else i.loading.hide ? i.hide() : i.loading.show && i.show()
+        }))
+    }
+
+    function U(e, t) {
         e.document.addEventListener(t, (function(i) {
             var n = new m(i.target);
             n && !n.isUnicorn && (n = n.getUnicornParent()), n && n.isUnicorn && n.actions.length > 0 && e.actionEvents[t].forEach((function(t) {
-                var r, s = t.action,
-                    a = t.element;
-                n.isSame(a) && (e.walker(a.el, (function(t) {
+                var r = t.action,
+                    s = t.element;
+                n.isSame(s) && (e.walker(s.el, (function(t) {
                     e.modelEls.filter((function(e) {
                         return e.el.isSameNode(t)
                     })).forEach((function(t) {
                         if (o(t.model) && t.model.isLazy) {
                             var i = {
                                 type: "syncInput",
                                 payload: {
@@ -489,50 +505,47 @@
                                     pk: t.db.pk,
                                     fields: {}
                                 }
                             };
                             i.payload.fields[t.field.name] = t.getValue(), e.actionQueue.push(i)
                         }
                     }))
-                })), s.isPrevent && i.preventDefault(), s.isStop && i.stopPropagation(), function(e) {
+                })), r.isPrevent && i.preventDefault(), r.isStop && i.stopPropagation(), function(e) {
                     if (!l(e = e.trim(), "(") || !e.endsWith(")")) return [];
                     e = e.slice(e.indexOf("(") + 1, e.length - 1);
                     for (var t = [], i = "", n = !1, r = !1, o = 0, s = 0, a = 0; a < e.length; a++) {
                         var u = e.charAt(a);
                         i += u, "[" === u ? s++ : "]" === u ? s-- : "(" === u ? o++ : ")" === u ? o-- : "{" === u || "}" === u || ("'" === u ? n = !n : '"' === u ? r = !r : "," === u && (n || r || 0 !== s || 0 !== o || (i = i.slice(0, i.length - 1), t.push(i), i = ""))), a === e.length - 1 && (n || r || 0 !== s || 0 !== o || (t.push(i.trim()), i = ""))
                     }
                     return t
-                }(s.name).forEach((function(e) {
+                }(r.name).forEach((function(e) {
                     if (e.startsWith("$event")) {
                         e = e.trim().slice(e.indexOf("$event") + 6).trim();
                         var t = "$event".concat(e),
                             n = i,
-                            r = !1;
+                            s = !1;
                         e.split(".").forEach((function(e) {
                             if (e = e.trim())
                                 if (e.endsWith("()")) {
                                     var t = e.slice(0, e.length - 2);
                                     n = n[t]()
-                                } else o(n[e]) ? n = n[e] : r = !0
-                        })), r ? (console.error("'".concat(t, "' could not be retrieved")), s.name = s.name.replace(t, "")) : n && ("string" == typeof n && (n = '"'.concat(n, '"')), s.name = s.name.replace(t, n))
+                                } else o(n[e]) ? n = n[e] : s = !0
+                        })), s ? (console.error("'".concat(t, "' could not be retrieved")), r.name = r.name.replace(t, "")) : n && ("string" == typeof n && (n = '"'.concat(n, '"')), r.name = r.name.replace(t, n))
                     }
-                })), n.loading && (n.loading.attr ? n.el[n.loading.attr] = n.loading.attr : n.loading.class ? n.el.classList.add(n.loading.class) : n.loading.removeClass && n.el.classList.remove(n.loading.removeClass)), e.loadingEls.forEach((function(t) {
-                    if (t.target) {
-                        var i = u("#".concat(t.target), e.root);
-                        i || e.keyEls.forEach((function(e) {
-                            i || e.key !== t.target || (i = e.el)
-                        })), i && n.el.isSameNode(i) && (t.loading.hide ? t.hide() : t.loading.show && t.show())
-                    } else t.loading.hide ? t.hide() : t.loading.show && t.show()
-                })), s.key ? s.key === ((r = i.key) ? r.match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g).map((function(e) {
-                    return e.toLowerCase()
-                })).join("-") : "") && e.callMethod(s.name) : e.callMethod(s.name))
+                })), r.key ? r.key === function(e) {
+                    if (!e) return "";
+                    var t = e.match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g);
+                    return t ? t.map((function(e) {
+                        return e.toLowerCase()
+                    })).join("-") : e
+                }(i.key) && (C(e, n), e.callMethod(r.name)) : (C(e, n), e.callMethod(r.name)))
             }))
         }))
     }
-    var U = function() {
+    var V = function() {
             function e(i) {
                 if (t(this, e), this.id = i.id, this.name = i.name, this.messageUrl = i.messageUrl, this.csrfTokenHeaderName = i.csrfTokenHeaderName, l(this.name, ".")) {
                     var n = this.name.split(".");
                     this.name = n[n.length - 2]
                 }
                 this.data = i.data, this.syncUrl = "".concat(this.messageUrl, "/").concat(this.name), this.document = i.document || document, this.walker = i.walker || c, this.root = void 0, this.modelEls = [], this.dbEls = [], this.loadingEls = [], this.keyEls = [], this.errors = {}, this.poll = {}, this.actionQueue = [], this.currentActionQueue = null, this.lastTriggeringElements = [], this.actionEvents = {}, this.attachedEventTypes = [], this.attachedModelEvents = [], this.attachedDbEvents = [], this.init(), this.refreshEventListeners(), this.initPolling()
             }
@@ -610,15 +623,15 @@
                                     action: t,
                                     element: i
                                 }) : (e.actionEvents[t.eventType] = [{
                                     action: t,
                                     element: i
                                 }], e.attachedEventTypes.some((function(e) {
                                     return e === t.eventType
-                                })) || (e.attachedEventTypes.push(t.eventType), C(e, t.eventType)))
+                                })) || (e.attachedEventTypes.push(t.eventType), U(e, t.eventType)))
                             })))
                         }
                     }))
                 }
             }, {
                 key: "callMethod",
                 value: function(e, t) {
@@ -707,28 +720,28 @@
             }, {
                 key: "queueMessage",
                 value: function(e, t) {
                     -1 === e ? d(w, 250, !1)(this, t) : d(w, e, !1)(this, t)
                 }
             }]), e
         }(),
-        V = "",
+        L = "",
         M = {};
     return e.call = function(e, t) {
         var i;
         if (Object.keys(M).forEach((function(t) {
                 if (r(i)) {
                     var n = M[t];
                     n.name === e && (i = n)
                 }
             })), !i) throw Error("No component found for: ", e);
         i.callMethod(t, (function(e) {
             console.error(e)
         }))
     }, e.componentInit = function(e) {
-        e.messageUrl = V, e.csrfTokenHeaderName = "X-CSRFToken";
-        var t = new U(e);
+        e.messageUrl = L, e.csrfTokenHeaderName = "X-CSRFToken";
+        var t = new V(e);
         t.init(), M[t.id] = t, t.setModelValues(), t.setDbModelValues()
     }, e.init = function(e) {
-        V = e
+        L = e
     }, e
 }({});
```

### Comparing `django-unicorn-0.9.3/django_unicorn/static/js/utils.js` & `django-unicorn-0.9.4/django_unicorn/static/js/utils.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -86,18 +86,23 @@
  * @param {string} str The string to be converted.
  */
 export function toKebabCase(str) {
     if (!str) {
         return "";
     }
 
-    return str
-        .match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g)
-        .map((x) => x.toLowerCase())
-        .join("-");
+    const match = str.match(
+        /[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g
+    );
+
+    if (!match) {
+        return str;
+    }
+
+    return match.map((x) => x.toLowerCase()).join("-");
 }
 
 /**
  * Traverses the DOM looking for child elements.
  */
 export function walk(el, callback) {
     const walker = document.createTreeWalker(
```

### Comparing `django-unicorn-0.9.3/django_unicorn/templatetags/unicorn.py` & `django-unicorn-0.9.4/django_unicorn/templatetags/unicorn.py`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/django_unicorn/views.py` & `django-unicorn-0.9.4/django_unicorn/views.py`

 * *Files identical despite different names*

### Comparing `django-unicorn-0.9.3/pyproject.toml` & `django-unicorn-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-unicorn"
-version = "0.9.3"
+version = "0.9.4"
 description = "A magical full-stack framework for Django."
 authors = ["Adam Hill <unicorn@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/adamghill/django-unicorn/"
 homepage = "https://www.django-unicorn.com"
 keywords = ["django", "python", "javascript", "fullstack"]
```

### Comparing `django-unicorn-0.9.3/setup.py` & `django-unicorn-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
  'django_unicorn.management.commands',
  'django_unicorn.templatetags']
 
 package_data = \
 {'': ['*'],
  'django_unicorn': ['static/js/*',
                     'static/js/morphdom/2.6.1/*',
+                    'static/svg/*',
                     'templates/unicorn/*']}
 
 install_requires = \
 ['beautifulsoup4>=4.9.1,<5.0.0',
  'django>=3.0.0',
  'orjson>=3.2.1,<4.0.0',
  'shortuuid>=1.0.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'django-unicorn',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'A magical full-stack framework for Django.',
     'long_description': '# django-unicorn\n\n![PyPI](https://img.shields.io/pypi/v/django-unicorn?color=blue&style=flat-square)\n\n![GitHub Release Date](https://img.shields.io/github/release-date/adamghill/django-unicorn?style=flat-square)\n\n<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->\n\n[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)\n\n<!-- ALL-CONTRIBUTORS-BADGE:END -->\n\nThe magical fullstack framework for Django. ✨\n\n`django-unicorn` provides a way to use backend Django code and regular Django templates to create interactive experiences without investing in a separate frontend framework.\n\n## Why?\n\nBuilding server-side sites in Django with the ORM and template engine is so pleasant, but once you need more interactivity on the frontend, there is a lot more ambiguity. Should you build out an entire API in Django REST framework? Should you use React or Vue.js (or some) other frontend framework?\n\nIt seems like there should be an easier way to create interactive experiences.\n\n## A note\n\n`django-unicorn` is still beta and the API will likely change on the way to version 1.0.0. All efforts will be made to include an easy upgrade path. 1.0.0 will signify that the public API won\'t change until the next major release.\n\n# Detailed documentation\n\nhttps://www.django-unicorn.com\n\n# Developing\n\n1. `git clone git@github.com:adamghill/django-unicorn.git`\n1. `poetry install`\n1. `poetry run example/manage.py migrate`\n1. `poetry run example/manage.py runserver 0:8000`\n1. Go to `localhost:8000` in your browser\n1. To install in another project `pip install -e ../django-unicorn`\n\n## Run unittests\n\n1. `poetry run pytest`\n1. `npm run test`\n\n## Minify Javascript\n\n1. `npm install`\n1. `npm run build`\n\n## Bump version\n\n1. `npm run build`\n1. `poetry version major|minor|patch`\n1. Commit/tag/push version bump\n1. `poetry publish --build -r test`\n1. Make sure test package can be installed as expected (https://test.pypi.org/project/django-unicorn/)\n1. `poetry publish`\n1. Make sure live package can be installed as expected (https://pypi.org/project/django-unicorn/)\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://adamghill.com"><img src="https://avatars0.githubusercontent.com/u/317045?v=4" width="100px;" alt=""/><br /><sub><b>Adam Hill</b></sub></a><br /><a href="https://github.com/adamghill/django-unicorn/commits?author=adamghill" title="Code">💻</a> <a href="https://github.com/adamghill/django-unicorn/commits?author=adamghill" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://python3.ninja"><img src="https://avatars1.githubusercontent.com/u/44167?v=4" width="100px;" alt=""/><br /><sub><b>Andres Vargas</b></sub></a><br /><a href="https://github.com/adamghill/django-unicorn/commits?author=zodman" title="Code">💻</a></td>\n    <td align="center"><a href="http://iskra.ml"><img src="https://avatars3.githubusercontent.com/u/6555851?v=4" width="100px;" alt=""/><br /><sub><b>Eddy Ernesto del Valle Pino</b></sub></a><br /><a href="https://github.com/adamghill/django-unicorn/commits?author=edelvalle" title="Code">💻</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-enable -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
     'author': 'Adam Hill',
     'author_email': 'unicorn@adamghill.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.django-unicorn.com',
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['django_unicorn', 'django_unicorn.management.commands',
 'django_unicorn.templatetags'] package_data = \ {'': ['*'], 'django_unicorn':
-['static/js/*', 'static/js/morphdom/2.6.1/*', 'templates/unicorn/*']}
-install_requires = \ ['beautifulsoup4>=4.9.1,<5.0.0', 'django>=3.0.0',
-'orjson>=3.2.1,<4.0.0', 'shortuuid>=1.0.1,<2.0.0'] setup_kwargs = { 'name':
-'django-unicorn', 'version': '0.9.3', 'description': 'A magical full-stack
-framework for Django.', 'long_description': '# django-unicorn\n\n![PyPI](https:
-//img.shields.io/pypi/v/django-unicorn?color=blue&style=flat-square)\n\n!
-[GitHub Release Date](https://img.shields.io/github/release-date/adamghill/
-django-unicorn?style=flat-square)\n\n\n\n[![All Contributors](https://
-img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)]
-(#contributors-)\n\n\n\nThe magical fullstack framework for Django.
-â¨\n\n`django-unicorn` provides a way to use backend Django code and regular
-Django templates to create interactive experiences without investing in a
-separate frontend framework.\n\n## Why?\n\nBuilding server-side sites in Django
-with the ORM and template engine is so pleasant, but once you need more
-interactivity on the frontend, there is a lot more ambiguity. Should you build
-out an entire API in Django REST framework? Should you use React or Vue.js (or
-some) other frontend framework?\n\nIt seems like there should be an easier way
-to create interactive experiences.\n\n## A note\n\n`django-unicorn` is still
-beta and the API will likely change on the way to version 1.0.0. All efforts
-will be made to include an easy upgrade path. 1.0.0 will signify that the
-public API won\'t change until the next major release.\n\n# Detailed
-documentation\n\nhttps://www.django-unicorn.com\n\n# Developing\n\n1. `git
-clone git@github.com:adamghill/django-unicorn.git`\n1. `poetry install`\n1.
-`poetry run example/manage.py migrate`\n1. `poetry run example/manage.py
-runserver 0:8000`\n1. Go to `localhost:8000` in your browser\n1. To install in
-another project `pip install -e ../django-unicorn`\n\n## Run unittests\n\n1.
-`poetry run pytest`\n1. `npm run test`\n\n## Minify Javascript\n\n1. `npm
-install`\n1. `npm run build`\n\n## Bump version\n\n1. `npm run build`\n1.
-`poetry version major|minor|patch`\n1. Commit/tag/push version bump\n1. `poetry
-publish --build -r test`\n1. Make sure test package can be installed as
-expected (https://test.pypi.org/project/django-unicorn/)\n1. `poetry
-publish`\n1. Make sure live package can be installed as expected (https://
-pypi.org/project/django-unicorn/)\n\n## Contributors â¨\n\nThanks goes to
-these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):\n\n\n\n\n
+['static/js/*', 'static/js/morphdom/2.6.1/*', 'static/svg/*', 'templates/
+unicorn/*']} install_requires = \ ['beautifulsoup4>=4.9.1,<5.0.0',
+'django>=3.0.0', 'orjson>=3.2.1,<4.0.0', 'shortuuid>=1.0.1,<2.0.0']
+setup_kwargs = { 'name': 'django-unicorn', 'version': '0.9.4', 'description':
+'A magical full-stack framework for Django.', 'long_description': '# django-
+unicorn\n\n![PyPI](https://img.shields.io/pypi/v/django-
+unicorn?color=blue&style=flat-square)\n\n![GitHub Release Date](https://
+img.shields.io/github/release-date/adamghill/django-unicorn?style=flat-
+square)\n\n\n\n[![All Contributors](https://img.shields.io/badge/
+all_contributors-3-orange.svg?style=flat-square)](#contributors-)\n\n\n\nThe
+magical fullstack framework for Django. â¨\n\n`django-unicorn` provides a way
+to use backend Django code and regular Django templates to create interactive
+experiences without investing in a separate frontend framework.\n\n##
+Why?\n\nBuilding server-side sites in Django with the ORM and template engine
+is so pleasant, but once you need more interactivity on the frontend, there is
+a lot more ambiguity. Should you build out an entire API in Django REST
+framework? Should you use React or Vue.js (or some) other frontend
+framework?\n\nIt seems like there should be an easier way to create interactive
+experiences.\n\n## A note\n\n`django-unicorn` is still beta and the API will
+likely change on the way to version 1.0.0. All efforts will be made to include
+an easy upgrade path. 1.0.0 will signify that the public API won\'t change
+until the next major release.\n\n# Detailed documentation\n\nhttps://
+www.django-unicorn.com\n\n# Developing\n\n1. `git clone git@github.com:
+adamghill/django-unicorn.git`\n1. `poetry install`\n1. `poetry run example/
+manage.py migrate`\n1. `poetry run example/manage.py runserver 0:8000`\n1. Go
+to `localhost:8000` in your browser\n1. To install in another project `pip
+install -e ../django-unicorn`\n\n## Run unittests\n\n1. `poetry run pytest`\n1.
+`npm run test`\n\n## Minify Javascript\n\n1. `npm install`\n1. `npm run
+build`\n\n## Bump version\n\n1. `npm run build`\n1. `poetry version
+major|minor|patch`\n1. Commit/tag/push version bump\n1. `poetry publish --build
+-r test`\n1. Make sure test package can be installed as expected (https://
+test.pypi.org/project/django-unicorn/)\n1. `poetry publish`\n1. Make sure live
+package can be installed as expected (https://pypi.org/project/django-unicorn/
+)\n\n## Contributors â¨\n\nThanks goes to these wonderful people ([emoji key]
+(https://allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n
 
       Adam_Hill       Andres_Vargas Eddy_Ernesto_del_Valle_Pino
 
      ð» â ï    ð»             ð»
 \n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
 all-contributors/all-contributors) specification. Contributions of any kind
 welcome!\n', 'author': 'Adam Hill', 'author_email': 'unicorn@adamghill.com',
```

### Comparing `django-unicorn-0.9.3/PKG-INFO` & `django-unicorn-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-unicorn
-Version: 0.9.3
+Version: 0.9.4
 Summary: A magical full-stack framework for Django.
 Home-page: https://www.django-unicorn.com
 License: MIT
 Keywords: django,python,javascript,fullstack
 Author: Adam Hill
 Author-email: unicorn@adamghill.com
 Requires-Python: >=3.6,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-unicorn Version: 0.9.3 Summary: A magical
+Metadata-Version: 2.1 Name: django-unicorn Version: 0.9.4 Summary: A magical
 full-stack framework for Django. Home-page: https://www.django-unicorn.com
 License: MIT Keywords: django,python,javascript,fullstack Author: Adam Hill
 Author-email: unicorn@adamghill.com Requires-Python: >=3.6,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist:
```

