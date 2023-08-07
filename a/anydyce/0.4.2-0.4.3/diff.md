# Comparing `tmp/anydyce-0.4.2-py3-none-any.whl.zip` & `tmp/anydyce-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21942 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1013 b- defN 23-Aug-04 20:54 anydyce/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 23-Aug-04 20:55 anydyce/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 20:54 anydyce/py.typed
--rw-r--r--  2.0 unx    61886 b- defN 23-Aug-04 20:54 anydyce/viz.py
--rw-r--r--  2.0 unx     2118 b- defN 23-Aug-04 20:55 anydyce-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    15588 b- defN 23-Aug-04 20:55 anydyce-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 20:55 anydyce-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Aug-04 20:55 anydyce-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      678 b- defN 23-Aug-04 20:55 anydyce-0.4.2.dist-info/RECORD
-9 files, 81431 bytes uncompressed, 20782 bytes compressed:  74.5%
+Zip file size: 22064 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1013 b- defN 23-Aug-07 11:44 anydyce/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-07 11:45 anydyce/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 11:44 anydyce/py.typed
+-rw-r--r--  2.0 unx    62524 b- defN 23-Aug-07 11:44 anydyce/viz.py
+-rw-r--r--  2.0 unx     2118 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15588 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      678 b- defN 23-Aug-07 11:45 anydyce-0.4.3.dist-info/RECORD
+9 files, 82069 bytes uncompressed, 20904 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: anydyce/py.typed
 Comment: 
 
 Filename: anydyce/viz.py
 Comment: 
 
-Filename: anydyce-0.4.2.dist-info/LICENSE
+Filename: anydyce-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: anydyce-0.4.2.dist-info/METADATA
+Filename: anydyce-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: anydyce-0.4.2.dist-info/WHEEL
+Filename: anydyce-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: anydyce-0.4.2.dist-info/top_level.txt
+Filename: anydyce-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: anydyce-0.4.2.dist-info/RECORD
+Filename: anydyce-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anydyce/_version.py

```diff
@@ -1,3 +1,3 @@
-__vers_str__ = "0.4.2"
-__version__ = (0, 4, 2)
+__vers_str__ = "0.4.3"
+__version__ = (0, 4, 3)
```

## anydyce/viz.py

```diff
@@ -240,14 +240,32 @@
             self._file_name = file_name
         else:
             self._file_name = file_name + "." + file_type.lower()
 
         self._file_type = file_type
 
     @beartype
+    def _repr_png_(self):
+        r"""
+        [Rich
+        display](https://ipython.readthedocs.io/en/stable/config/integrating.html#integrating-rich-display)
+        hook method used by IPython to display PNG images.
+        """
+        return self._data if self._file_type is ImageType.PNG else None
+
+    @beartype
+    def _repr_svg_(self):
+        r"""
+        [Rich
+        display](https://ipython.readthedocs.io/en/stable/config/integrating.html#integrating-rich-display)
+        hook method used by IPython to display SVG images.
+        """
+        return self._data if self._file_type is ImageType.SVG else None
+
+    @beartype
     def download_link(self) -> str:
         return f'<a download="{self._file_name}" href="{self._mime_pfx}{urllib.parse.quote(self._data)}" target="_blank">Download {self._file_type.value} image</a>'
 
 
 @dataclass(frozen=True)
 class _PlotWidgetsDataclass:
     # Widget to trigger updates (hack)
```

## Comparing `anydyce-0.4.2.dist-info/LICENSE` & `anydyce-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anydyce-0.4.2.dist-info/METADATA` & `anydyce-0.4.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydyce
-Version: 0.4.2
+Version: 0.4.3
 Summary: Visualization tools for dyce
 Home-page: https://posita.github.io/anydyce/
 Author: Matt Bogosian
 Author-email: matt@bogosian.net
 License: MIT License
 Project-URL: Source Repository, https://github.com/posita/anydyce/
 Classifier: Topic :: Education
@@ -51,19 +51,19 @@
 
 *Copyright and other protections apply.
 Please see the accompanying ``LICENSE`` file for rights and restrictions governing use of this software.
 All rights not expressly waived or licensed are reserved.
 If that file is missing or appears to be modified from its original, then please contact the author before viewing or using this software in any capacity.*
 
 [![Tests](https://github.com/posita/anydyce/actions/workflows/on-push.yaml/badge.svg)](https://github.com/posita/anydyce/actions/workflows/on-push.yaml)
-[![Version](https://img.shields.io/pypi/v/anydyce/0.4.2.svg)](https://pypi.org/project/anydyce/0.4.2/)
-[![Development Stage](https://img.shields.io/pypi/status/anydyce/0.4.2.svg)](https://pypi.org/project/anydyce/0.4.2/)
-[![License](https://img.shields.io/pypi/l/anydyce/0.4.2.svg)](http://opensource.org/licenses/MIT)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/anydyce/0.4.2.svg)](https://pypi.org/project/anydyce/0.4.2/)
-[![Supported Python Implementations](https://img.shields.io/pypi/implementation/anydyce/0.4.2.svg)](https://pypi.org/project/anydyce/0.4.2/)
+[![Version](https://img.shields.io/pypi/v/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
+[![Development Stage](https://img.shields.io/pypi/status/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
+[![License](https://img.shields.io/pypi/l/anydyce/0.4.3.svg)](http://opensource.org/licenses/MIT)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
+[![Supported Python Implementations](https://img.shields.io/pypi/implementation/anydyce/0.4.3.svg)](https://pypi.org/project/anydyce/0.4.3/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![``dyce``-powered!](https://raw.githubusercontent.com/posita/dyce/latest/docs/dyce-powered.svg)](https://posita.github.io/dyce/)
 [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/latest/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
 [![Bear-ified™](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.rtfd.io/)
 
 # ``anydyce`` – visualization tools for [``dyce``](https://posita.github.io/dyce/)
 
@@ -112,15 +112,15 @@
     Notebooks can also be downloaded and shared as ``.ipynb`` files.
 
 ### Interactive quick start
 
 Probably the _easiest_ way to start tinkering with ``anydyce`` is with [JupyterLite](https://jupyterlite.readthedocs.io/):
 [![Try dyce](https://jupyterlite.readthedocs.io/en/latest/_static/badge.svg)](https://posita.github.io/anydyce/0.4/jupyter/lab/?path=anydyce_intro.ipynb)
 
-The [``quickstart-local.sh`` script](https://github.com/posita/anydyce/blob/v0.4.2/quickstart-local.sh) will create a local [virtual environment](https://docs.python.org/3/library/venv.html) to bootstrap a local Jupyter server with ``anydyce`` installed and open a web browser to the [introduction notebook](https://github.com/posita/anydyce/blob/v0.4.2/docs/notebooks/anydyce_intro-ipynb).
+The [``quickstart-local.sh`` script](https://github.com/posita/anydyce/blob/v0.4.3/quickstart-local.sh) will create a local [virtual environment](https://docs.python.org/3/library/venv.html) to bootstrap a local Jupyter server with ``anydyce`` installed and open a web browser to the [introduction notebook](https://github.com/posita/anydyce/blob/v0.4.3/docs/notebooks/anydyce_intro-ipynb).
 
 [Binder](https://mybinder.org/) is another great resource that you can use to share notebooks from your Git repositories (including [Gists](https://gist.github.com/)):
 [![Try dyce](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/posita/anydyce/HEAD?labpath=docs%2Fnotebooks%2Fanydyce_intro.ipynb)
 
 !!! danger "JupyterLite and Binder may not save your work!"
 
     JupyterLite attempts to make use of your browser’s local storage for saving notebook changes.
@@ -160,20 +160,20 @@
 >>> plot_burst(ax, 2@H(6))
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_1_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Basic plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_1_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_1_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Basic plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_1.py"><code>plot_burst_1.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_1.py"><code>plot_burst_1.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_1.py"
 ```
 </details>
 
 The outer ring can also be used to compare two histograms directly.
@@ -193,20 +193,20 @@
 ... )
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_2_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: 2d6 vs. 4dF plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_2_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_2_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: 2d6 vs. 4dF plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_2.py"><code>plot_burst_2.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_2.py"><code>plot_burst_2.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_2.py"
 ```
 </details>
 
 Labels can even be overridden for interesting, at-a-glance displays.
@@ -232,20 +232,20 @@
 ... }), inner_cmap="RdYlBu_r", outer_formatter=d20formatter)
 >>> matplotlib.pyplot.show()  # doctest: +SKIP
 
 ```
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_3_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Advanced plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_3_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_3_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Advanced plot_burst example" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3_dark.png#gh-dark-mode-only"></span>
 </picture>
 
 <details>
-<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.2/docs/assets/plot_burst_3.py"><code>plot_burst_3.py</code></a></summary>
+<summary>Source: <a href="https://raw.githubusercontent.com/posita/anydyce/v0.4.3/docs/assets/plot_burst_3.py"><code>plot_burst_3.py</code></a></summary>
 
 ``` python
 --8<-- "docs/assets/plot_burst_3.py"
 ```
 </details>
 
 ### Requirements
```

## Comparing `anydyce-0.4.2.dist-info/RECORD` & `anydyce-0.4.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 anydyce/__init__.py,sha256=1zShVHUd-3Egv_IEZRXRuEt-guDibac52vdqF4PFzPw,1013
-anydyce/_version.py,sha256=DO4MBYmd5SMSjQWxqorQ7ZVtJ-_ySPOdrRh2R2OziDA,48
+anydyce/_version.py,sha256=kSXQbq9njMgdVeU0OAkd7--1UhdE2bK5TW8D3_qbV-0,48
 anydyce/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-anydyce/viz.py,sha256=-cKWEr7RUkvPX-Nzt_JGMsPXUymiZZAXi_CIbuLXZC0,61886
-anydyce-0.4.2.dist-info/LICENSE,sha256=_JjbEsiZFa2_MFppzXtZckKs7MUOjvKD79kok876VbM,2118
-anydyce-0.4.2.dist-info/METADATA,sha256=QzaotTmQv4bWpBsDzlgT3gmfP8VS1jWHm632pywwqP8,15588
-anydyce-0.4.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-anydyce-0.4.2.dist-info/top_level.txt,sha256=DiuY4cmvZIdl2Tc2SI-fYfLfRr_gkQP529FQPLng2LM,8
-anydyce-0.4.2.dist-info/RECORD,,
+anydyce/viz.py,sha256=ooiJuzN8SPXjm90nr9HMIwHR9-xsu90SqgOge_3uM8U,62524
+anydyce-0.4.3.dist-info/LICENSE,sha256=_JjbEsiZFa2_MFppzXtZckKs7MUOjvKD79kok876VbM,2118
+anydyce-0.4.3.dist-info/METADATA,sha256=afYNqpWszP0OlMZQs3PVAfG7SznBMx-wJH537Md1WQM,15588
+anydyce-0.4.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+anydyce-0.4.3.dist-info/top_level.txt,sha256=DiuY4cmvZIdl2Tc2SI-fYfLfRr_gkQP529FQPLng2LM,8
+anydyce-0.4.3.dist-info/RECORD,,
```

