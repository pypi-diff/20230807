# Comparing `tmp/exotic-3.1.0.zip` & `tmp/exotic-3.2.0.zip`

## zipinfo {}

```diff
@@ -1,119 +1,119 @@
-Zip file size: 6361419 bytes, number of entries: 117
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/exotic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/
--rw-r--r--  2.0 unx      476 b- defN 23-Jul-24 23:33 exotic-3.1.0/requirements.txt
--rw-r--r--  2.0 unx     1682 b- defN 23-Jul-24 23:34 exotic-3.1.0/setup.cfg
--rw-r--r--  2.0 unx    14575 b- defN 23-Jul-24 23:34 exotic-3.1.0/PKG-INFO
--rw-r--r--  2.0 unx     3359 b- defN 23-Jul-24 23:33 exotic-3.1.0/CODE_OF_CONDUCT.md
--rw-r--r--  2.0 unx     1556 b- defN 23-Jul-24 23:33 exotic-3.1.0/.gitignore
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-24 23:33 exotic-3.1.0/CITATION.md
--rw-r--r--  2.0 unx      221 b- defN 23-Jul-24 23:33 exotic-3.1.0/MANIFEST.in
--rw-r--r--  2.0 unx      699 b- defN 23-Jul-24 23:33 exotic-3.1.0/AUTHORS.md
--rwxr-xr-x  2.0 unx      265 b- defN 23-Jul-24 23:33 exotic-3.1.0/run_exotic_windows.bat
--rw-r--r--  2.0 unx     2149 b- defN 23-Jul-24 23:33 exotic-3.1.0/LICENSE
--rwxr-xr-x  2.0 unx     5080 b- defN 23-Jul-24 23:33 exotic-3.1.0/run_exotic_linux.sh
--rw-r--r--  2.0 unx    13141 b- defN 23-Jul-24 23:33 exotic-3.1.0/README.md
--rw-r--r--  2.0 unx     5887 b- defN 23-Jul-24 23:33 exotic-3.1.0/inits.json
--rw-r--r--  2.0 unx     1890 b- defN 23-Jul-24 23:33 exotic-3.1.0/setup.py
--rw-r--r--  2.0 unx      362 b- defN 23-Jul-24 23:33 exotic-3.1.0/pyproject.toml
--rw-r--r--  2.0 unx      201 b- defN 23-Jul-24 23:33 exotic-3.1.0/CONTRIBUTING.md
--rwxr-xr-x  2.0 unx     4756 b- defN 23-Jul-24 23:33 exotic-3.1.0/run_exotic_mac.command
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/exotic/api/
--rw-r--r--  2.0 unx     9481 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/plots.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic/version.py
--rw-r--r--  2.0 unx    80045 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/exotic_gui.py
--rw-r--r--  2.0 unx   117869 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/exotic.py
--rw-r--r--  2.0 unx     1239 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/animate.py
--rw-r--r--  2.0 unx     4752 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/plate_status.py
--rw-r--r--  2.0 unx    11472 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/utils.py
--rw-r--r--  2.0 unx     3027 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/__init__.py
--rw-r--r--  2.0 unx    27708 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/inputs.py
--rw-r--r--  2.0 unx    13768 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/output_files.py
--rw-r--r--  2.0 unx     5592 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/ew.py
--rw-r--r--  2.0 unx    15060 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/colab.py
--rw-r--r--  2.0 unx     4017 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/filters.py
--rw-r--r--  2.0 unx    18359 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/plotting.py
--rw-r--r--  2.0 unx     2916 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/versioning.py
--rw-r--r--  2.0 unx     5981 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/ld.py
--rw-r--r--  2.0 unx    29599 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/nested_linear_fitter.py
--rw-r--r--  2.0 unx     2322 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/__init__.py
--rw-r--r--  2.0 unx    49191 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/elca.py
--rw-r--r--  2.0 unx    17395 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/nea.py
--rw-r--r--  2.0 unx     9803 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/gael_ld.py
--rw-r--r--  2.0 unx     6591 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/plate_solution.py
--rw-r--r--  2.0 unx    14763 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/output_aavso.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/.github/workflows/
--rw-r--r--  2.0 unx      260 b- defN 23-Jul-24 23:33 exotic-3.1.0/.github/dependabot.yml
--rw-r--r--  2.0 unx     1073 b- defN 23-Jul-24 23:33 exotic-3.1.0/.github/workflows/python-publish.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/Images/
--rw-r--r--  2.0 unx    16096 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/German/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/Brazilian_Portuguese/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/English/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/Spanish (Español)/
--rw-r--r--  2.0 unx   223208 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
--rw-r--r--  2.0 unx   155973 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
--rw-r--r--  2.0 unx   611693 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
--rw-r--r--  2.0 unx    10330 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Beispiel_Output.txt
--rw-r--r--  2.0 unx   180681 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
--rw-r--r--  2.0 unx      119 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/translators.md
--rw-r--r--  2.0 unx   132016 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Benutzung-von-GitHub.pdf
--rw-r--r--  2.0 unx    28054 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
--rw-r--r--  2.0 unx      545 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Brazilian_Portuguese/README.md
--rw-r--r--  2.0 unx    11401 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
--rw-r--r--  2.0 unx    86803 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
--rw-r--r--  2.0 unx   725191 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-EXOTIC-Works.pdf
--rw-r--r--  2.0 unx     9236 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
--rw-r--r--  2.0 unx     5893 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
--rw-r--r--  2.0 unx   598255 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
--rw-r--r--  2.0 unx     6151 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
--rw-r--r--  2.0 unx     5902 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
--rw-r--r--  2.0 unx    27943 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
--rw-r--r--  2.0 unx    10067 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/example_output.txt
--rw-r--r--  2.0 unx     2673 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
--rw-r--r--  2.0 unx   243586 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How_to_Use_GitHub.pdf
--rw-r--r--  2.0 unx   229468 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/Introduction-to-Exoplanets.pdf
--rw-r--r--  2.0 unx   112871 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Spanish (Español)/translators.md
--rw-r--r--  2.0 unx   197330 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_planetparams.png
--rw-r--r--  2.0 unx   340120 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/ExoplanetWatch.png
--rw-r--r--  2.0 unx   189180 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/posterior_sample.png
--rw-r--r--  2.0 unx    74050 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_running.png
--rw-r--r--  2.0 unx   187434 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_inputobs.png
--rw-r--r--  2.0 unx   265478 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/transitsimple.jpg
--rw-r--r--  2.0 unx    45485 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_initssaved.png
--rw-r--r--  2.0 unx    57777 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_inputplanetparams.png
--rw-r--r--  2.0 unx   309812 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/HAT-P-32bExample.png
--rw-r--r--  2.0 unx    56356 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/Background_Estimate.png
--rw-r--r--  2.0 unx   617967 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/Hot_pixel_mask.png
--rw-r--r--  2.0 unx    46133 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_inputobsinfo.png
--rw-r--r--  2.0 unx    82591 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_loading.png
--rw-r--r--  2.0 unx    46372 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_saveinits.png
--rw-r--r--  2.0 unx    79523 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/centroids.png
--rw-r--r--  2.0 unx    53508 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_redmode.png
--rw-r--r--  2.0 unx    65879 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_welcome.png
--rw-r--r--  2.0 unx    46727 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_runmode.png
--rw-r--r--  2.0 unx    27673 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/tess.py
--rw-r--r--  2.0 unx     3296 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/lc_fitter_unit_test.py
--rw-r--r--  2.0 unx   597675 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/Multiple_Lightcurve_fit.ipynb
--rw-r--r--  2.0 unx     4597 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/sampledata.json
--rw-r--r--  2.0 unx   248480 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/Exoplanet_Watch_API.ipynb
--rw-r--r--  2.0 unx     2244 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/global_fitter_unit_test.py
--rw-r--r--  2.0 unx    22617 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb
--rwxr-xr-x  2.0 unx     4479 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/interactive_fitter.py
--rw-r--r--  2.0 unx    20643 b- defN 23-Jul-24 23:33 exotic-3.1.0/tests/test_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-24 23:33 exotic-3.1.0/tests/__init__.py
--rw-r--r--  2.0 unx    14575 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/not-zip-safe
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3319 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      494 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/entry_points.txt
-117 files, 7654984 bytes uncompressed, 6342585 bytes compressed:  17.1%
+Zip file size: 6363964 bytes, number of entries: 117
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/exotic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/examples/
+-rwxr-xr-x  2.0 unx     5080 b- defN 23-Aug-07 03:10 exotic-3.2.0/run_exotic_linux.sh
+-rw-r--r--  2.0 unx     2149 b- defN 23-Aug-07 03:10 exotic-3.2.0/LICENSE
+-rw-r--r--  2.0 unx      362 b- defN 23-Aug-07 03:10 exotic-3.2.0/pyproject.toml
+-rw-r--r--  2.0 unx     1556 b- defN 23-Aug-07 03:10 exotic-3.2.0/.gitignore
+-rw-r--r--  2.0 unx     1682 b- defN 23-Aug-07 03:10 exotic-3.2.0/setup.cfg
+-rw-r--r--  2.0 unx     3359 b- defN 23-Aug-07 03:10 exotic-3.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--  2.0 unx      201 b- defN 23-Aug-07 03:10 exotic-3.2.0/CONTRIBUTING.md
+-rw-r--r--  2.0 unx      221 b- defN 23-Aug-07 03:10 exotic-3.2.0/MANIFEST.in
+-rwxr-xr-x  2.0 unx      265 b- defN 23-Aug-07 03:10 exotic-3.2.0/run_exotic_windows.bat
+-rw-r--r--  2.0 unx      476 b- defN 23-Aug-07 03:10 exotic-3.2.0/requirements.txt
+-rwxr-xr-x  2.0 unx     4756 b- defN 23-Aug-07 03:10 exotic-3.2.0/run_exotic_mac.command
+-rw-r--r--  2.0 unx     1890 b- defN 23-Aug-07 03:10 exotic-3.2.0/setup.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Aug-07 03:10 exotic-3.2.0/CITATION.md
+-rw-r--r--  2.0 unx     5887 b- defN 23-Aug-07 03:10 exotic-3.2.0/inits.json
+-rw-r--r--  2.0 unx    13141 b- defN 23-Aug-07 03:10 exotic-3.2.0/README.md
+-rw-r--r--  2.0 unx    14575 b- defN 23-Aug-07 03:10 exotic-3.2.0/PKG-INFO
+-rw-r--r--  2.0 unx      699 b- defN 23-Aug-07 03:10 exotic-3.2.0/AUTHORS.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/.github/workflows/
+-rw-r--r--  2.0 unx      260 b- defN 23-Aug-07 03:10 exotic-3.2.0/.github/dependabot.yml
+-rw-r--r--  2.0 unx     1073 b- defN 23-Aug-07 03:10 exotic-3.2.0/.github/workflows/python-publish.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/Images/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/regions/
+-rw-r--r--  2.0 unx    16096 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/README.md
+-rw-r--r--  2.0 unx   187434 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_inputobs.png
+-rw-r--r--  2.0 unx    56356 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/Background_Estimate.png
+-rw-r--r--  2.0 unx    74050 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_running.png
+-rw-r--r--  2.0 unx   617967 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/Hot_pixel_mask.png
+-rw-r--r--  2.0 unx    46372 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_saveinits.png
+-rw-r--r--  2.0 unx    65879 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_welcome.png
+-rw-r--r--  2.0 unx    57777 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_inputplanetparams.png
+-rw-r--r--  2.0 unx   265478 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/transitsimple.jpg
+-rw-r--r--  2.0 unx    46133 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_inputobsinfo.png
+-rw-r--r--  2.0 unx    82591 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_loading.png
+-rw-r--r--  2.0 unx    79523 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/centroids.png
+-rw-r--r--  2.0 unx    53508 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_redmode.png
+-rw-r--r--  2.0 unx    46727 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_runmode.png
+-rw-r--r--  2.0 unx   309812 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/HAT-P-32bExample.png
+-rw-r--r--  2.0 unx   197330 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_planetparams.png
+-rw-r--r--  2.0 unx   189180 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/posterior_sample.png
+-rw-r--r--  2.0 unx   340120 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/ExoplanetWatch.png
+-rw-r--r--  2.0 unx    45485 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/Images/exotic_initssaved.png
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/regions/Spanish (Español)/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/docs/regions/Brazilian_Portuguese/
+-rw-r--r--  2.0 unx   223208 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
+-rw-r--r--  2.0 unx      119 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/translators.md
+-rw-r--r--  2.0 unx   180681 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
+-rw-r--r--  2.0 unx    10330 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/Beispiel_Output.txt
+-rw-r--r--  2.0 unx   155973 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
+-rw-r--r--  2.0 unx   611693 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
+-rw-r--r--  2.0 unx   132016 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/German/Benutzung-von-GitHub.pdf
+-rw-r--r--  2.0 unx      129 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/Spanish (Español)/translators.md
+-rw-r--r--  2.0 unx   112871 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
+-rw-r--r--  2.0 unx   598255 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
+-rw-r--r--  2.0 unx   725191 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How-EXOTIC-Works.pdf
+-rw-r--r--  2.0 unx     9236 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
+-rw-r--r--  2.0 unx     5893 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
+-rw-r--r--  2.0 unx     6151 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
+-rw-r--r--  2.0 unx    27943 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
+-rw-r--r--  2.0 unx     5902 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
+-rw-r--r--  2.0 unx     2673 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
+-rw-r--r--  2.0 unx    11401 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
+-rw-r--r--  2.0 unx    10067 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/example_output.txt
+-rw-r--r--  2.0 unx   243586 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/How_to_Use_GitHub.pdf
+-rw-r--r--  2.0 unx   229468 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/Introduction-to-Exoplanets.pdf
+-rw-r--r--  2.0 unx    86803 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
+-rw-r--r--  2.0 unx    28054 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
+-rw-r--r--  2.0 unx      545 b- defN 23-Aug-07 03:10 exotic-3.2.0/docs/regions/Brazilian_Portuguese/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 03:10 exotic-3.2.0/exotic/api/
+-rw-r--r--  2.0 unx     1239 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/animate.py
+-rw-r--r--  2.0 unx     9481 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/plots.py
+-rw-r--r--  2.0 unx   117880 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/exotic.py
+-rw-r--r--  2.0 unx    80045 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/exotic_gui.py
+-rw-r--r--  2.0 unx    27708 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/inputs.py
+-rw-r--r--  2.0 unx    13768 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/output_files.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/version.py
+-rw-r--r--  2.0 unx    11472 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/utils.py
+-rw-r--r--  2.0 unx     4752 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/plate_status.py
+-rw-r--r--  2.0 unx     3027 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/__init__.py
+-rw-r--r--  2.0 unx     2916 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/versioning.py
+-rw-r--r--  2.0 unx    31289 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/nested_linear_fitter.py
+-rw-r--r--  2.0 unx    14763 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/output_aavso.py
+-rw-r--r--  2.0 unx    15060 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/colab.py
+-rw-r--r--  2.0 unx     9803 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/gael_ld.py
+-rw-r--r--  2.0 unx    18359 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/plotting.py
+-rw-r--r--  2.0 unx    17395 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/nea.py
+-rw-r--r--  2.0 unx     5589 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/ew.py
+-rw-r--r--  2.0 unx    49191 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/elca.py
+-rw-r--r--  2.0 unx     6591 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/plate_solution.py
+-rw-r--r--  2.0 unx    13655 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/ld.py
+-rw-r--r--  2.0 unx     3348 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/filters.py
+-rw-r--r--  2.0 unx     2322 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic/api/__init__.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3319 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      494 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/requires.txt
+-rw-r--r--  2.0 unx    14575 b- defN 23-Aug-07 03:10 exotic-3.2.0/exotic.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 03:10 exotic-3.2.0/tests/__init__.py
+-rw-r--r--  2.0 unx    20643 b- defN 23-Aug-07 03:10 exotic-3.2.0/tests/test_utils.py
+-rwxr-xr-x  2.0 unx     4479 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/interactive_fitter.py
+-rw-r--r--  2.0 unx   248480 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/Exoplanet_Watch_API.ipynb
+-rw-r--r--  2.0 unx    27754 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/tess.py
+-rw-r--r--  2.0 unx    22617 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb
+-rw-r--r--  2.0 unx     4597 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/sampledata.json
+-rw-r--r--  2.0 unx   597675 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/Multiple_Lightcurve_fit.ipynb
+-rw-r--r--  2.0 unx     2244 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/global_fitter_unit_test.py
+-rw-r--r--  2.0 unx     3296 b- defN 23-Aug-07 03:10 exotic-3.2.0/examples/lc_fitter_unit_test.py
+117 files, 7663768 bytes uncompressed, 6345130 bytes compressed:  17.2%
```

## zipnote {}

```diff
@@ -1,352 +1,352 @@
-Filename: exotic-3.1.0/
+Filename: exotic-3.2.0/
 Comment: 
 
-Filename: exotic-3.1.0/exotic/
+Filename: exotic-3.2.0/.github/
 Comment: 
 
-Filename: exotic-3.1.0/.github/
+Filename: exotic-3.2.0/docs/
 Comment: 
 
-Filename: exotic-3.1.0/docs/
+Filename: exotic-3.2.0/exotic/
 Comment: 
 
-Filename: exotic-3.1.0/examples/
+Filename: exotic-3.2.0/exotic.egg-info/
 Comment: 
 
-Filename: exotic-3.1.0/tests/
+Filename: exotic-3.2.0/tests/
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/
+Filename: exotic-3.2.0/examples/
 Comment: 
 
-Filename: exotic-3.1.0/requirements.txt
+Filename: exotic-3.2.0/run_exotic_linux.sh
 Comment: 
 
-Filename: exotic-3.1.0/setup.cfg
+Filename: exotic-3.2.0/LICENSE
 Comment: 
 
-Filename: exotic-3.1.0/PKG-INFO
+Filename: exotic-3.2.0/pyproject.toml
 Comment: 
 
-Filename: exotic-3.1.0/CODE_OF_CONDUCT.md
+Filename: exotic-3.2.0/.gitignore
 Comment: 
 
-Filename: exotic-3.1.0/.gitignore
+Filename: exotic-3.2.0/setup.cfg
 Comment: 
 
-Filename: exotic-3.1.0/CITATION.md
+Filename: exotic-3.2.0/CODE_OF_CONDUCT.md
 Comment: 
 
-Filename: exotic-3.1.0/MANIFEST.in
+Filename: exotic-3.2.0/CONTRIBUTING.md
 Comment: 
 
-Filename: exotic-3.1.0/AUTHORS.md
+Filename: exotic-3.2.0/MANIFEST.in
 Comment: 
 
-Filename: exotic-3.1.0/run_exotic_windows.bat
+Filename: exotic-3.2.0/run_exotic_windows.bat
 Comment: 
 
-Filename: exotic-3.1.0/LICENSE
+Filename: exotic-3.2.0/requirements.txt
 Comment: 
 
-Filename: exotic-3.1.0/run_exotic_linux.sh
+Filename: exotic-3.2.0/run_exotic_mac.command
 Comment: 
 
-Filename: exotic-3.1.0/README.md
+Filename: exotic-3.2.0/setup.py
 Comment: 
 
-Filename: exotic-3.1.0/inits.json
+Filename: exotic-3.2.0/CITATION.md
 Comment: 
 
-Filename: exotic-3.1.0/setup.py
+Filename: exotic-3.2.0/inits.json
 Comment: 
 
-Filename: exotic-3.1.0/pyproject.toml
+Filename: exotic-3.2.0/README.md
 Comment: 
 
-Filename: exotic-3.1.0/CONTRIBUTING.md
+Filename: exotic-3.2.0/PKG-INFO
 Comment: 
 
-Filename: exotic-3.1.0/run_exotic_mac.command
+Filename: exotic-3.2.0/AUTHORS.md
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/
+Filename: exotic-3.2.0/.github/workflows/
 Comment: 
 
-Filename: exotic-3.1.0/exotic/plots.py
+Filename: exotic-3.2.0/.github/dependabot.yml
 Comment: 
 
-Filename: exotic-3.1.0/exotic/version.py
+Filename: exotic-3.2.0/.github/workflows/python-publish.yml
 Comment: 
 
-Filename: exotic-3.1.0/exotic/exotic_gui.py
+Filename: exotic-3.2.0/docs/Images/
 Comment: 
 
-Filename: exotic-3.1.0/exotic/exotic.py
+Filename: exotic-3.2.0/docs/regions/
 Comment: 
 
-Filename: exotic-3.1.0/exotic/animate.py
+Filename: exotic-3.2.0/docs/README.md
 Comment: 
 
-Filename: exotic-3.1.0/exotic/plate_status.py
+Filename: exotic-3.2.0/docs/Images/exotic_inputobs.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/utils.py
+Filename: exotic-3.2.0/docs/Images/Background_Estimate.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/__init__.py
+Filename: exotic-3.2.0/docs/Images/exotic_running.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/inputs.py
+Filename: exotic-3.2.0/docs/Images/Hot_pixel_mask.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/output_files.py
+Filename: exotic-3.2.0/docs/Images/exotic_saveinits.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/ew.py
+Filename: exotic-3.2.0/docs/Images/exotic_welcome.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/colab.py
+Filename: exotic-3.2.0/docs/Images/exotic_inputplanetparams.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/filters.py
+Filename: exotic-3.2.0/docs/Images/transitsimple.jpg
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/plotting.py
+Filename: exotic-3.2.0/docs/Images/exotic_inputobsinfo.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/versioning.py
+Filename: exotic-3.2.0/docs/Images/exotic_loading.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/ld.py
+Filename: exotic-3.2.0/docs/Images/centroids.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/nested_linear_fitter.py
+Filename: exotic-3.2.0/docs/Images/exotic_redmode.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/__init__.py
+Filename: exotic-3.2.0/docs/Images/exotic_runmode.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/elca.py
+Filename: exotic-3.2.0/docs/Images/HAT-P-32bExample.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/nea.py
+Filename: exotic-3.2.0/docs/Images/exotic_planetparams.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/gael_ld.py
+Filename: exotic-3.2.0/docs/Images/posterior_sample.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/plate_solution.py
+Filename: exotic-3.2.0/docs/Images/ExoplanetWatch.png
 Comment: 
 
-Filename: exotic-3.1.0/exotic/api/output_aavso.py
+Filename: exotic-3.2.0/docs/Images/exotic_initssaved.png
 Comment: 
 
-Filename: exotic-3.1.0/.github/workflows/
+Filename: exotic-3.2.0/docs/regions/German/
 Comment: 
 
-Filename: exotic-3.1.0/.github/dependabot.yml
+Filename: exotic-3.2.0/docs/regions/Spanish (Espa#U00f1ol)/
 Comment: 
 
-Filename: exotic-3.1.0/.github/workflows/python-publish.yml
+Filename: exotic-3.2.0/docs/regions/English/
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/
+Filename: exotic-3.2.0/docs/regions/Brazilian_Portuguese/
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/
+Filename: exotic-3.2.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/README.md
+Filename: exotic-3.2.0/docs/regions/German/translators.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/
+Filename: exotic-3.2.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/Brazilian_Portuguese/
+Filename: exotic-3.2.0/docs/regions/German/Beispiel_Output.txt
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/
+Filename: exotic-3.2.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/Spanish (Espa#U00f1ol)/
+Filename: exotic-3.2.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
+Filename: exotic-3.2.0/docs/regions/German/Benutzung-von-GitHub.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
+Filename: exotic-3.2.0/docs/regions/Spanish (Espa#U00f1ol)/translators.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
+Filename: exotic-3.2.0/docs/regions/Spanish (Espa#U00f1ol)/Introducci#U00f3n a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/Beispiel_Output.txt
+Filename: exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
+Filename: exotic-3.2.0/docs/regions/English/How-EXOTIC-Works.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/translators.md
+Filename: exotic-3.2.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/German/Benutzung-von-GitHub.pdf
+Filename: exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
+Filename: exotic-3.2.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/Brazilian_Portuguese/README.md
+Filename: exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
+Filename: exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
+Filename: exotic-3.2.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How-EXOTIC-Works.pdf
+Filename: exotic-3.2.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
+Filename: exotic-3.2.0/docs/regions/English/example_output.txt
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
+Filename: exotic-3.2.0/docs/regions/English/How_to_Use_GitHub.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
+Filename: exotic-3.2.0/docs/regions/English/Introduction-to-Exoplanets.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
+Filename: exotic-3.2.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
+Filename: exotic-3.2.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
+Filename: exotic-3.2.0/docs/regions/Brazilian_Portuguese/README.md
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/example_output.txt
+Filename: exotic-3.2.0/exotic/api/
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
+Filename: exotic-3.2.0/exotic/animate.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/How_to_Use_GitHub.pdf
+Filename: exotic-3.2.0/exotic/plots.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/English/Introduction-to-Exoplanets.pdf
+Filename: exotic-3.2.0/exotic/exotic.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/Spanish (Espa#U00f1ol)/Introducci#U00f3n a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
+Filename: exotic-3.2.0/exotic/exotic_gui.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/regions/Spanish (Espa#U00f1ol)/translators.md
+Filename: exotic-3.2.0/exotic/inputs.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_planetparams.png
+Filename: exotic-3.2.0/exotic/output_files.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/ExoplanetWatch.png
+Filename: exotic-3.2.0/exotic/version.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/posterior_sample.png
+Filename: exotic-3.2.0/exotic/utils.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_running.png
+Filename: exotic-3.2.0/exotic/plate_status.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_inputobs.png
+Filename: exotic-3.2.0/exotic/__init__.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/transitsimple.jpg
+Filename: exotic-3.2.0/exotic/api/versioning.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_initssaved.png
+Filename: exotic-3.2.0/exotic/api/nested_linear_fitter.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_inputplanetparams.png
+Filename: exotic-3.2.0/exotic/api/output_aavso.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/HAT-P-32bExample.png
+Filename: exotic-3.2.0/exotic/api/colab.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/Background_Estimate.png
+Filename: exotic-3.2.0/exotic/api/gael_ld.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/Hot_pixel_mask.png
+Filename: exotic-3.2.0/exotic/api/plotting.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_inputobsinfo.png
+Filename: exotic-3.2.0/exotic/api/nea.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_loading.png
+Filename: exotic-3.2.0/exotic/api/ew.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_saveinits.png
+Filename: exotic-3.2.0/exotic/api/elca.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/centroids.png
+Filename: exotic-3.2.0/exotic/api/plate_solution.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_redmode.png
+Filename: exotic-3.2.0/exotic/api/ld.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_welcome.png
+Filename: exotic-3.2.0/exotic/api/filters.py
 Comment: 
 
-Filename: exotic-3.1.0/docs/Images/exotic_runmode.png
+Filename: exotic-3.2.0/exotic/api/__init__.py
 Comment: 
 
-Filename: exotic-3.1.0/examples/tess.py
+Filename: exotic-3.2.0/exotic.egg-info/entry_points.txt
 Comment: 
 
-Filename: exotic-3.1.0/examples/lc_fitter_unit_test.py
+Filename: exotic-3.2.0/exotic.egg-info/not-zip-safe
 Comment: 
 
-Filename: exotic-3.1.0/examples/Multiple_Lightcurve_fit.ipynb
+Filename: exotic-3.2.0/exotic.egg-info/top_level.txt
 Comment: 
 
-Filename: exotic-3.1.0/examples/sampledata.json
+Filename: exotic-3.2.0/exotic.egg-info/SOURCES.txt
 Comment: 
 
-Filename: exotic-3.1.0/examples/Exoplanet_Watch_API.ipynb
+Filename: exotic-3.2.0/exotic.egg-info/dependency_links.txt
 Comment: 
 
-Filename: exotic-3.1.0/examples/global_fitter_unit_test.py
+Filename: exotic-3.2.0/exotic.egg-info/requires.txt
 Comment: 
 
-Filename: exotic-3.1.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb
+Filename: exotic-3.2.0/exotic.egg-info/PKG-INFO
 Comment: 
 
-Filename: exotic-3.1.0/examples/interactive_fitter.py
+Filename: exotic-3.2.0/tests/__init__.py
 Comment: 
 
-Filename: exotic-3.1.0/tests/test_utils.py
+Filename: exotic-3.2.0/tests/test_utils.py
 Comment: 
 
-Filename: exotic-3.1.0/tests/__init__.py
+Filename: exotic-3.2.0/examples/interactive_fitter.py
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/PKG-INFO
+Filename: exotic-3.2.0/examples/Exoplanet_Watch_API.ipynb
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/not-zip-safe
+Filename: exotic-3.2.0/examples/tess.py
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/top_level.txt
+Filename: exotic-3.2.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/SOURCES.txt
+Filename: exotic-3.2.0/examples/sampledata.json
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/requires.txt
+Filename: exotic-3.2.0/examples/Multiple_Lightcurve_fit.ipynb
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/dependency_links.txt
+Filename: exotic-3.2.0/examples/global_fitter_unit_test.py
 Comment: 
 
-Filename: exotic-3.1.0/exotic.egg-info/entry_points.txt
+Filename: exotic-3.2.0/examples/lc_fitter_unit_test.py
 Comment: 
 
 Zip file comment:
```

## Comparing `exotic-3.1.0/setup.cfg` & `exotic-3.2.0/setup.cfg`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/PKG-INFO` & `exotic-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotic
-Version: 3.1.0
+Version: 3.2.0
 Summary: EXOTIC: EXOplanet Transit Interpretation Code
 Home-page: https://github.com/rzellem/EXOTIC
 Download-URL: https://github.com/rzellem/EXOTIC/releases/latest
 Author: Exoplanet Watch at NASA JPL
 Author-email: exoplanetwatch@jpl.nasa.gov
 License: Proprietary -- Copyright (c) 2019-present, California Institute of Technology.
 Project-URL: Documentation, https://github.com/rzellem/EXOTIC/wiki
```

## Comparing `exotic-3.1.0/CODE_OF_CONDUCT.md` & `exotic-3.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/.gitignore` & `exotic-3.2.0/.gitignore`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/AUTHORS.md` & `exotic-3.2.0/AUTHORS.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/LICENSE` & `exotic-3.2.0/LICENSE`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/run_exotic_linux.sh` & `exotic-3.2.0/run_exotic_linux.sh`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/README.md` & `exotic-3.2.0/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/inits.json` & `exotic-3.2.0/inits.json`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/setup.py` & `exotic-3.2.0/setup.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/run_exotic_mac.command` & `exotic-3.2.0/run_exotic_mac.command`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/plots.py` & `exotic-3.2.0/exotic/plots.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/exotic_gui.py` & `exotic-3.2.0/exotic/exotic_gui.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/exotic.py` & `exotic-3.2.0/exotic/exotic.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,15 @@
                      "please try again.", error=True)
             ra = input("Input the Right Ascension of target (HH:MM:SS): ")
             dec = input("Input the Declination of target (<sign>DD:MM:SS): ")
 
 
 def standard_filter(ld, filter_):
     if not filter_['filter']:
-        ld.standard_list()
+        LimbDarkening.standard_list()
 
     while True:
         if not filter_['filter']:
             filter_['filter'] = user_input("\nPlease enter in the Filter Name or Abbreviation "
                                            "(EX: Johnson V, V, STB, RJ): ", type_=str)
         if ld.check_standard(filter_):
             break
@@ -1852,15 +1852,15 @@
                     pDict = userpDict
         else:
             pDict = get_planetary_parameters(CandidatePlanetBool, userpDict, pdict=pDict)
 
         ld_obj = LimbDarkening(pDict)
         nonlinear_ld(ld_obj, exotic_infoDict)
 
-        exotic_infoDict['filter'] = ld_obj.filter_type
+        exotic_infoDict['filter'] = ld_obj.filter_name
         exotic_infoDict['filter_desc'] = ld_obj.filter_desc
         exotic_infoDict['wl_min'] = ld_obj.wl_min
         exotic_infoDict['wl_max'] = ld_obj.wl_max
 
         ld0 = ld_obj.ld0
         ld1 = ld_obj.ld1
         ld2 = ld_obj.ld2
```

## Comparing `exotic-3.1.0/exotic/animate.py` & `exotic-3.2.0/exotic/animate.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/plate_status.py` & `exotic-3.2.0/exotic/plate_status.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/utils.py` & `exotic-3.2.0/exotic/utils.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/__init__.py` & `exotic-3.2.0/exotic/__init__.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/inputs.py` & `exotic-3.2.0/exotic/inputs.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/output_files.py` & `exotic-3.2.0/exotic/output_files.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/ew.py` & `exotic-3.2.0/exotic/api/ew.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         Returns
         -------
         (time, flux, fluxerr, airmass, airmass_detrend) : tuple of numpy arrays
         """
         r = urllib.request.urlopen(
             os.path.join(base_uri,self.files['file_data_json'][2:]))
         jdata = json.loads(r.read().decode(r.info().get_param('charset') or 'utf-8'))
-        return np.array(jdata[1:],dtype=np.float).T
+        return np.array(jdata[1:],dtype=float).T
 
 def translate_keys(rdict):
     """ Translates the keys to a compatible format for EXOTIC/ELCA
 
     Parameters
     ----------
     rdict : dict
```

## Comparing `exotic-3.1.0/exotic/api/colab.py` & `exotic-3.2.0/exotic/api/colab.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/filters.py` & `exotic-3.2.0/exotic/api/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 # Sources for FWHM band wavelengths are referenced below, respectively 
 # note that all below units default to nm
-fwhm = {
+__fwhm = {
         # AAVSO, Source(s): AAVSO International Database; https://www.aavso.org/filters
         # Johnson
-        "Johnson U": {"name": "U", "desc": "Johnson U", "fwhm": ("333.8", "398.8")},
-        "Johnson B": {"name": "B", "desc": "Johnson B", "fwhm": ("391.6", "480.6")},
-        "Johnson V": {"name": "V", "desc": "Johnson V", "fwhm": ("502.8", "586.8")},
-        "Johnson R": {"name": "RJ", "desc": "Johnson R", "fwhm": ("590.0", "810.0")},
-        "Johnson I": {"name": "IJ", "desc": "Johnson I", "fwhm": ("780.0", "1020.0")},
+        "Johnson U": {"name": "U", "fwhm": ("333.8", "398.8")},
+        "Johnson B": {"name": "B", "fwhm": ("391.6", "480.6")},
+        "Johnson V": {"name": "V", "fwhm": ("502.8", "586.8")},
+        "Johnson R": {"name": "RJ", "fwhm": ("590.0", "810.0")},
+        "Johnson I": {"name": "IJ", "fwhm": ("780.0", "1020.0")},
 
         # Cousins
-        "Cousins R": {"name": "R", "desc": "Cousins R", "fwhm": ("561.7", "719.7")},
-        "Cousins I": {"name": "I", "desc": "Cousins I", "fwhm": ("721.0", "875.0")},
+        "Cousins R": {"name": "R", "fwhm": ("561.7", "719.7")},
+        "Cousins I": {"name": "I", "fwhm": ("721.0", "875.0")},
 
         # Near-Infrared
-        "Near-Infrared J": {"name": "J", "desc": "Near-Infrared J", "fwhm": ("1040.0", "1360.0")},
-        "Near-Infrared H": {"name": "H", "desc": "Near-Infrared H", "fwhm": ("1420.0", "1780.0")},
-        "Near-Infrared K": {"name": "K", "desc": "Near-Infrared K", "fwhm": ("2015.0", "2385.0")},
+        "Near-Infrared J": {"name": "J", "fwhm": ("1040.0", "1360.0")},
+        "Near-Infrared H": {"name": "H", "fwhm": ("1420.0", "1780.0")},
+        "Near-Infrared K": {"name": "K", "fwhm": ("2015.0", "2385.0")},
 
         # Sloan
-        "Sloan u": {"name": "SU", "desc": "Sloan u", "fwhm": ("321.8", "386.8")},
-        "Sloan g": {"name": "SG", "desc": "Sloan g", "fwhm": ("402.5", "551.5")},
-        "Sloan r": {"name": "SR", "desc": "Sloan r", "fwhm": ("553.1", "693.1")},
-        "Sloan i": {"name": "SI", "desc": "Sloan i", "fwhm": ("697.5", "827.5")},
-        "Sloan z": {"name": "SZ", "desc": "Sloan z", "fwhm": ("841.2", "978.2")},
+        "Sloan u": {"name": "SU", "fwhm": ("321.8", "386.8")},
+        "Sloan g": {"name": "SG", "fwhm": ("402.5", "551.5")},
+        "Sloan r": {"name": "SR", "fwhm": ("553.1", "693.1")},
+        "Sloan i": {"name": "SI", "fwhm": ("697.5", "827.5")},
+        "Sloan z": {"name": "SZ", "fwhm": ("841.2", "978.2")},
 
         # Stromgren
-        "Stromgren u": {"name": "STU", "desc": "Stromgren u", "fwhm": ("336.3", "367.7")},
-        "Stromgren v": {"name": "STV", "desc": "Stromgren v", "fwhm": ("401.5", "418.5")},
-        "Stromgren b": {"name": "STB", "desc": "Stromgren b", "fwhm": ("459.55", "478.05")},
-        "Stromgren y": {"name": "STY", "desc": "Stromgren y", "fwhm": ("536.7", "559.3")},
-        "Stromgren Hbw": {"name": "STHBW", "desc": "Stromgren Hbw", "fwhm": ("481.5", "496.5")},
-        "Stromgren Hbn": {"name": "STHBN", "desc": "Stromgren Hbn", "fwhm": ("487.5", "484.5")},
+        "Stromgren u": {"name": "STU", "fwhm": ("336.3", "367.7")},
+        "Stromgren v": {"name": "STV", "fwhm": ("401.5", "418.5")},
+        "Stromgren b": {"name": "STB", "fwhm": ("459.55", "478.05")},
+        "Stromgren y": {"name": "STY", "fwhm": ("536.7", "559.3")},
+        "Stromgren Hbw": {"name": "STHBW", "fwhm": ("481.5", "496.5")},
+        "Stromgren Hbn": {"name": "STHBN", "fwhm": ("487.5", "484.5")},
 
         # Optec
-        "Optec Wing A": {"name": "MA", "desc": "Optec Wing A", "fwhm": ("706.5", "717.5")},
-        "Optec Wing B": {"name": "MB", "desc": "Optec Wing B", "fwhm": ("748.5", "759.5")},
-        "Optec Wing C": {"name": "MI", "desc": "Optec Wing C", "fwhm": ("1003.0", "1045.0")},
+        "Optec Wing A": {"name": "MA", "fwhm": ("706.5", "717.5")},
+        "Optec Wing B": {"name": "MB", "fwhm": ("748.5", "759.5")},
+        "Optec Wing C": {"name": "MI", "fwhm": ("1003.0", "1045.0")},
 
         # PanSTARRS
-        "PanSTARRS z-short": {"name": "ZS", "desc": "PanSTARRS z-short", "fwhm": ("826.0", "920.0")},
-        "PanSTARRS Y": {"name": "Y", "desc": "PanSTARRS Y", "fwhm": ("946.4", "1054.4")},
-        "PanSTARRS w": {"name": "N/A", "desc": "PanSTARRS w", "fwhm": ("404.2", "845.8")},
+        "PanSTARRS z-short": {"name": "ZS", "fwhm": ("826.0", "920.0")},
+        "PanSTARRS Y": {"name": "Y", "fwhm": ("946.4", "1054.4")},
+        "PanSTARRS w": {"name": "N/A", "fwhm": ("404.2", "845.8")},
 
         # MObs Clear Filter; Source(s): Martin Fowler
-        "MObs CV": {"name": "CV", "desc": "MObs CV", "fwhm": ("350.0", "850.0")},
+        "MObs CV": {"name": "CV", "fwhm": ("350.0", "850.0")},
 
         # Astrodon CBB; Source(s): George Silvis; https://astrodon.com/products/astrodon-exo-planet-filter/
-        "Astrodon ExoPlanet-BB": {"name": "CBB", "desc": "Astrodon ExoPlanet-BB", "fwhm": ("500.0", "1000.0")},
+        "Astrodon ExoPlanet-BB": {"name": "CBB", "fwhm": ("500.0", "1000.0")},
 }
+# expose as fwhm and for convenience set 'desc' field equal to key
+fwhm = {k: v for k, v in __fwhm.items() if (v.update(desc=k),)}
 
 # aliases to back-reference naming standard updates
 fwhm_alias = {
-        "J NIR 1.2 micron": "Near-Infrared J",
-        "J NIR 1.2micron": "Near-Infrared J",
-        "H NIR 1.6 micron": "Near-Infrared H",
-        "H NIR 1.6micron": "Near-Infrared H",
-        "K NIR 2.2 micron": "Near-Infrared K",
-        "K NIR 2.2micron": "Near-Infrared K",
-
         "LCO Bessell B": "Johnson B",
         "LCO Bessell V": "Johnson V",
         "LCO Bessell R": "Cousins R",
         "LCO Bessell I": "Cousins I",
 
+        "J NIR 1.2 micron": "Near-Infrared J",
+        "H NIR 1.6 micron": "Near-Infrared H",
+        "K NIR 2.2 micron": "Near-Infrared K",
+
         "LCO SDSS u'": "Sloan u",
         "LCO SDSS g'": "Sloan g",
         "LCO SDSS r'": "Sloan r",
         "LCO SDSS i'": "Sloan i",
 
-        "LCO Pan-STARRS Y": "PanSTARRS Y",
         "LCO Pan-STARRS zs": "PanSTARRS z-short",
+        "LCO Pan-STARRS Y": "PanSTARRS Y",
         "LCO Pan-STARRS w": "PanSTARRS w",
 
-        "Exop": "Astrodon ExoPlanet-BB",
-
         "Clear (unfiltered) reduced to V sequence": "MObs CV",
+
+        "Exop": "Astrodon ExoPlanet-BB",
 }
```

## Comparing `exotic-3.1.0/exotic/api/plotting.py` & `exotic-3.2.0/exotic/api/plotting.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/versioning.py` & `exotic-3.2.0/exotic/api/versioning.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/nested_linear_fitter.py` & `exotic-3.2.0/exotic/api/nested_linear_fitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from exotic.api.plotting import corner
 from ultranest import ReactiveNestedSampler
 from astropy.timeseries import LombScargle
 
 
 class linear_fitter(object):
 
-    def __init__(self, data, dataerr, bounds=None, prior=None):
+    def __init__(self, data, dataerr, bounds=None, prior=None, labels=None):
         """
         Fit a linear model to data using nested sampling.
 
         Parameters
         ----------
         data : array
             Data to fit.
@@ -69,14 +69,15 @@
             Bounds on parameters. Dictionary of tuples/list
         prior : dict, optional
             Prior on parameters for slope and intercept. Dictionary of tuples/list
         """
         self.data = data
         self.dataerr = dataerr
         self.bounds = bounds
+        self.labels = np.array(labels)
         self.prior = prior.copy() # dict {'m':(0.1,0.5), 'b':(0,1)}
         if bounds is None:
             # use +- 3 sigma prior as bounds
             self.bounds = {
                 'm':[prior['m'][0]-3*prior['m'][1],prior['m'][0]+3*prior['m'][1]],
                 'b':[prior['b'][0]-3*prior['b'][1],prior['b'][0]+3*prior['b'][1]]
             }
@@ -130,16 +131,33 @@
         show_2sigma : bool, optional
             Show a fill between using the 2 sigma limits. Default is False (aka 1 sigma)
         """
 
         # set up the figure        
         fig,ax = plt.subplots(1, figsize=(9,6))
 
-        # plot the data/residuals
-        ax.errorbar(self.epochs, self.residuals*24*60, yerr=self.dataerr*24*60, ls='none', marker='o',color='black')
+        # check if labels are not None
+        if self.labels is not None:
+            # find unique set of labels
+            ulabels = np.unique(self.labels)
+            # set up a color/marker cycle
+            markers = cycle(['o','v','^','<','>','s','*','h','H','D','d','P','X'])
+            colors = cycle(['black','blue','green','orange','purple','grey','magenta','cyan','lime'])
+
+            # plot each label separately
+            for i, ulabel in enumerate(ulabels):
+                # find where the label matches
+                mask = self.labels == ulabel
+                # plot the data/residuals
+                ax.errorbar(self.epochs[mask], self.residuals[mask]*24*60, yerr=self.dataerr[mask]*24*60, 
+                            ls='none', marker=next(markers),color=next(colors), label=ulabel)
+        else:
+            # plot the data/residuals
+            ax.errorbar(self.epochs, self.residuals*24*60, yerr=self.dataerr*24*60, ls='none', marker='o',color='black')
+
         ylower = (self.residuals.mean()-3*np.std(self.residuals))*24*60
         yupper = (self.residuals.mean()+3*np.std(self.residuals))*24*60
 
         # upsample data
         epochs = (np.linspace(self.data.min()-7, self.data.max()+7, 1000) - self.parameters['b'])/self.parameters['m']
 
         # set the y-axis limits
@@ -591,14 +609,27 @@
         0.000153, 0.000349, 0.000149, 0.000146,
         0.000385, 0.000146, 0.000153, 0.000360,
         0.000356, 0.000147, 0.000147, 0.000146,
         0.000363, 0.000142, 0.000357, 0.000368,
         0.000160, 0.000160, 0.000151, 0.000160,
         0.000140, 0.000120, 0.000800, 0.000140 ])
 
+    # labels for a legend
+    labels = np.array([ 'TESS', 'TESS',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar',
+        'TESS', 'EpW', 'ExoClock', 'Unistellar'])
+
     P = 1.360029  # orbital period for your target
 
     Tc_norm = Tc - Tc.min()  #normalize the data to the first observation
     #print(Tc_norm)
     orbit = np.rint(Tc_norm / P)  #number of orbits since first observation (rounded to nearest integer)
     #print(orbit)
 
@@ -613,14 +644,22 @@
     std_dev = np.sqrt(np.diagonal(res.normalized_cov_params)) 
 
     slope = params[1]
     slope_std_dev = std_dev[1]
     intercept = params[0]
     intercept_std_dev = std_dev[0]
 
+    # 3 sigma clip based on residuals
+    calculated = orbit*slope + intercept
+    residuals = (Tc - calculated)/Tc_error
+    mask = np.abs(residuals) < 3
+    Tc = Tc[mask]
+    Tc_error = Tc_error[mask]
+    labels = labels[mask]
+
     #print(res.summary())
     #print("Params =",params)
     #print("Error matrix =",res.normalized_cov_params)
     #print("Standard Deviations =",std_dev)
 
     print("Weighted Linear Least Squares Solution")
     print("T0 =",intercept,"+-",intercept_std_dev)
@@ -634,15 +673,15 @@
 
     # used to plot red overlay in O-C figure
     prior = {
         'm':[slope, slope_std_dev],         # value from WLS (replace with literature value)
         'b':[intercept, intercept_std_dev]  # value from WLS (replace with literature value)
     }
 
-    lf = linear_fitter( Tc, Tc_error, bounds, prior=prior )
+    lf = linear_fitter( Tc, Tc_error, bounds, prior=prior, labels=labels )
 
     lf.plot_triangle()
     plt.subplots_adjust(top=0.9,hspace=0.2,wspace=0.2)
     plt.savefig("posterior.png")
     plt.close()
     print("image saved to: posterior.png")
 
@@ -656,8 +695,8 @@
     fig,ax = lf.plot_periodogram()
     plt.tight_layout()
     plt.savefig("periodogram.png")
     plt.close()
     print("image saved to: periodogram.png")
 
 if __name__ == "__main__":
-    main()
+    main()
```

## Comparing `exotic-3.1.0/exotic/api/__init__.py` & `exotic-3.2.0/exotic/api/__init__.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/elca.py` & `exotic-3.2.0/exotic/api/elca.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/nea.py` & `exotic-3.2.0/exotic/api/nea.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/gael_ld.py` & `exotic-3.2.0/exotic/api/gael_ld.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/plate_solution.py` & `exotic-3.2.0/exotic/api/plate_solution.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic/api/output_aavso.py` & `exotic-3.2.0/exotic/api/output_aavso.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/.github/workflows/python-publish.yml` & `exotic-3.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/README.md` & `exotic-3.2.0/docs/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf` & `exotic-3.2.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf` & `exotic-3.2.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf` & `exotic-3.2.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/German/Beispiel_Output.txt` & `exotic-3.2.0/docs/regions/German/Beispiel_Output.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf` & `exotic-3.2.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/German/Benutzung-von-GitHub.pdf` & `exotic-3.2.0/docs/regions/German/Benutzung-von-GitHub.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf` & `exotic-3.2.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/Brazilian_Portuguese/README.md` & `exotic-3.2.0/docs/regions/Brazilian_Portuguese/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md` & `exotic-3.2.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf` & `exotic-3.2.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How-EXOTIC-Works.pdf` & `exotic-3.2.0/docs/regions/English/How-EXOTIC-Works.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md` & `exotic-3.2.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md` & `exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf` & `exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md` & `exotic-3.2.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md` & `exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf` & `exotic-3.2.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/example_output.txt` & `exotic-3.2.0/docs/regions/English/example_output.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt` & `exotic-3.2.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/How_to_Use_GitHub.pdf` & `exotic-3.2.0/docs/regions/English/How_to_Use_GitHub.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/English/Introduction-to-Exoplanets.pdf` & `exotic-3.2.0/docs/regions/English/Introduction-to-Exoplanets.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx` & `exotic-3.2.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_planetparams.png` & `exotic-3.2.0/docs/Images/exotic_planetparams.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/ExoplanetWatch.png` & `exotic-3.2.0/docs/Images/ExoplanetWatch.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/posterior_sample.png` & `exotic-3.2.0/docs/Images/posterior_sample.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_running.png` & `exotic-3.2.0/docs/Images/exotic_running.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_inputobs.png` & `exotic-3.2.0/docs/Images/exotic_inputobs.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/transitsimple.jpg` & `exotic-3.2.0/docs/Images/transitsimple.jpg`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_initssaved.png` & `exotic-3.2.0/docs/Images/exotic_initssaved.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_inputplanetparams.png` & `exotic-3.2.0/docs/Images/exotic_inputplanetparams.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/HAT-P-32bExample.png` & `exotic-3.2.0/docs/Images/HAT-P-32bExample.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/Background_Estimate.png` & `exotic-3.2.0/docs/Images/Background_Estimate.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/Hot_pixel_mask.png` & `exotic-3.2.0/docs/Images/Hot_pixel_mask.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_inputobsinfo.png` & `exotic-3.2.0/docs/Images/exotic_inputobsinfo.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_loading.png` & `exotic-3.2.0/docs/Images/exotic_loading.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_saveinits.png` & `exotic-3.2.0/docs/Images/exotic_saveinits.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/centroids.png` & `exotic-3.2.0/docs/Images/centroids.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_redmode.png` & `exotic-3.2.0/docs/Images/exotic_redmode.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_welcome.png` & `exotic-3.2.0/docs/Images/exotic_welcome.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/docs/Images/exotic_runmode.png` & `exotic-3.2.0/docs/Images/exotic_runmode.png`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/tess.py` & `exotic-3.2.0/examples/tess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # first create an environment with the proper dependencies + version
 # git clone https://github.com/rzellem/EXOTIC.git
 # cd EXOTIC
 # git checkout tess
-# conda create -n tess python=3.9
-# conda activate tess
-# pip install pandas scipy matplotlib astropy statsmodels cython numpy==1.21.6
-# pip install wotan transitleastsquares pylightcurve lightkurve==2.0.6 ultranest==3.5.6
+# conda create -n tess_exotic python=3.9
+# conda activate tess_exotic
 # pip install .
-# cd examples
+# pip install lightkurve==2.0.6 statsmodels wotan transitleastsquares
+# pip install numpy==1.21.6
+# cd examples/
 # python tess.py -t "HAT-P-18 b"
+
 import os
 import copy
 import json
 import pickle
 import argparse
 import requests
 import numpy as np
@@ -540,15 +541,17 @@
         # degenerate if fit with Rp/Rs and Inclination but could try anyways
 
     print('performing global fit...')
     airmass = np.zeros(len(time[tmask]))
     myfit = lc_fitter(time[tmask]+2457000.0, flux[tmask], phot_std/flux[tmask], airmass, tpars, mybounds, verbose=True)
 
     # create plots
-    myfit.plot_bestfit(title=f"{args.target} Global Fit")
+    fig,ax = myfit.plot_bestfit(title=f"{args.target} Global Fit")
+    # set y_limit between 1 and 99 percentile
+    ax[0].set_ylim([np.percentile(flux, 1)*0.99, np.percentile(flux,99)*1.01])
     plt.savefig( os.path.join( planetdir, planetname+"_global_fit.png"))
     plt.close()
 
     myfit.plot_triangle()
     plt.savefig( os.path.join( planetdir, planetname+"_global_triangle.png"))
     plt.close()
```

## Comparing `exotic-3.1.0/examples/lc_fitter_unit_test.py` & `exotic-3.2.0/examples/lc_fitter_unit_test.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/Multiple_Lightcurve_fit.ipynb` & `exotic-3.2.0/examples/Multiple_Lightcurve_fit.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/sampledata.json` & `exotic-3.2.0/examples/sampledata.json`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/Exoplanet_Watch_API.ipynb` & `exotic-3.2.0/examples/Exoplanet_Watch_API.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/global_fitter_unit_test.py` & `exotic-3.2.0/examples/global_fitter_unit_test.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb` & `exotic-3.2.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/examples/interactive_fitter.py` & `exotic-3.2.0/examples/interactive_fitter.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/tests/test_utils.py` & `exotic-3.2.0/tests/test_utils.py`

 * *Files identical despite different names*

## Comparing `exotic-3.1.0/exotic.egg-info/PKG-INFO` & `exotic-3.2.0/exotic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotic
-Version: 3.1.0
+Version: 3.2.0
 Summary: EXOTIC: EXOplanet Transit Interpretation Code
 Home-page: https://github.com/rzellem/EXOTIC
 Download-URL: https://github.com/rzellem/EXOTIC/releases/latest
 Author: Exoplanet Watch at NASA JPL
 Author-email: exoplanetwatch@jpl.nasa.gov
 License: Proprietary -- Copyright (c) 2019-present, California Institute of Technology.
 Project-URL: Documentation, https://github.com/rzellem/EXOTIC/wiki
```

## Comparing `exotic-3.1.0/exotic.egg-info/SOURCES.txt` & `exotic-3.2.0/exotic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

