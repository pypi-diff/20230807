# Comparing `tmp/matlab-proxy-0.7.2.tar.gz` & `tmp/matlab-proxy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-proxy-0.7.2.tar", last modified: Tue Jul 11 10:01:55 2023, max compression
+gzip compressed data, was "matlab-proxy-0.7.3.tar", last modified: Mon Aug  7 09:28:25 2023, max compression
```

## Comparing `matlab-proxy-0.7.2.tar` & `matlab-proxy-0.7.3.tar`

### file list

```diff
@@ -1,163 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1289896 2023-07-11 10:01:38.000000 matlab-proxy-0.7.2/gui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/public/
--rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/actionCreators/
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/actionCreators/actionCreators.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/actionCreators/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/components/App/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/App/3p/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.412932 matlab-proxy-0.7.2/gui/src/components/App/3p/css/
--rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/css/site7.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.woff
--rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
--rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
--rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/bug_reports/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/bug_reports/workaround.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/App.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/MATLAB-env-blur.png
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/App/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Confirmation/
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Confirmation/Confirmation.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Confirmation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/Controls.css
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/Controls.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/feedback.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/help.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/sign-out.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/start.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Controls/terminate.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Error/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Error/Error.css
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Error/Error.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Error/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Help/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Help/Help.css
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Help/Help.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Help/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.416932 matlab-proxy-0.7.2/gui/src/components/Information/
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Information/Information.css
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Information/Information.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Information/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/ExistingLicense.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/ExistingLicense.js
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/LicensingGatherer.css
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/MHLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/NLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/MatlabJsd.css
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/MatlabJsd.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/MatlabJsd/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/Overlay/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.css
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/Overlay/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.css
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/gripper.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-ok.svg
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/jest.config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/reducers/
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/reducers/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/reducers/reducers.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/selectors/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/selectors/selectors.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/setupTests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.408932 matlab-proxy-0.7.2/gui/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/gui/src/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/gui/src/test/utils/react-test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    50370 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/app_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/default_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/devel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/icons/matlab.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/matlab/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/matlab/startup.m
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/list_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/matlab_proxy/util/mwi/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/custom_http_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/mwi/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/matlab_proxy/util/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:01:55.420932 matlab-proxy-0.7.2/matlab_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 10:01:21.000000 matlab-proxy-0.7.2/matlab_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:01:55.424932 matlab-proxy-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-11 10:00:42.000000 matlab-proxy-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.382018 matlab-proxy-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-08-07 09:28:25.382018 matlab-proxy-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.354018 matlab-proxy-0.7.3/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1289979 2023-08-07 09:28:00.000000 matlab-proxy-0.7.3/gui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.354018 matlab-proxy-0.7.3/gui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.354018 matlab-proxy-0.7.3/gui/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.354018 matlab-proxy-0.7.3/gui/src/actionCreators/
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/actionCreators/actionCreators.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/actionCreators/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.358018 matlab-proxy-0.7.3/gui/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.346018 matlab-proxy-0.7.3/gui/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.358018 matlab-proxy-0.7.3/gui/src/components/App/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.346018 matlab-proxy-0.7.3/gui/src/components/App/3p/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.358018 matlab-proxy-0.7.3/gui/src/components/App/3p/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/css/site7.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.362018 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-eps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-eps.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-eps.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.346018 matlab-proxy-0.7.3/gui/src/components/App/3p/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.362018 matlab-proxy-0.7.3/gui/src/components/App/3p/images/bug_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/images/bug_reports/workaround.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.346018 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.362018 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/App.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/MATLAB-env-blur.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/App/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.362018 matlab-proxy-0.7.3/gui/src/components/Confirmation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Confirmation/Confirmation.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Confirmation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.366018 matlab-proxy-0.7.3/gui/src/components/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/Controls.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/Controls.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/feedback.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/sign-out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Controls/terminate.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.366018 matlab-proxy-0.7.3/gui/src/components/EntitlementSelector/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/EntitlementSelector/EntitlementSelector.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/EntitlementSelector/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.366018 matlab-proxy-0.7.3/gui/src/components/Error/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Error/Error.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Error/Error.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Error/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.366018 matlab-proxy-0.7.3/gui/src/components/Help/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Help/Help.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Help/Help.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Help/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.366018 matlab-proxy-0.7.3/gui/src/components/Information/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Information/Information.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Information/Information.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Information/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.370018 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/ExistingLicense.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/ExistingLicense.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/LicensingGatherer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/MHLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/NLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.370018 matlab-proxy-0.7.3/gui/src/components/MatlabJsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/MatlabJsd/MatlabJsd.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/MatlabJsd/MatlabJsd.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/MatlabJsd/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.370018 matlab-proxy-0.7.3/gui/src/components/Overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Overlay/Overlay.css
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Overlay/Overlay.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/Overlay/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.370018 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/OverlayTrigger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/gripper.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/trigger-error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/trigger-ok.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/jest.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.370018 matlab-proxy-0.7.3/gui/src/reducers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/reducers/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/reducers/reducers.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.374018 matlab-proxy-0.7.3/gui/src/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/selectors/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/selectors/selectors.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/setupTests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.350018 matlab-proxy-0.7.3/gui/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.374018 matlab-proxy-0.7.3/gui/src/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/gui/src/test/utils/react-test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.374018 matlab-proxy-0.7.3/matlab_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25621 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50528 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/app_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/default_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/devel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.378018 matlab-proxy-0.7.3/matlab_proxy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/icons/matlab.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.378018 matlab-proxy-0.7.3/matlab_proxy/matlab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/matlab/startup.m
+-rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.378018 matlab-proxy-0.7.3/matlab_proxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/list_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.382018 matlab-proxy-0.7.3/matlab_proxy/util/mwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/custom_http_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.382018 matlab-proxy-0.7.3/matlab_proxy/util/mwi/embedded_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/embedded_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/embedded_connector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/embedded_connector/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/mwi/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/matlab_proxy/util/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:28:25.378018 matlab-proxy-0.7.3/matlab_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 09:27:33.000000 matlab-proxy-0.7.3/matlab_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 09:28:25.382018 matlab-proxy-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-07 09:27:02.000000 matlab-proxy-0.7.3/setup.py
```

### Comparing `matlab-proxy-0.7.2/LICENSE.md` & `matlab-proxy-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/PKG-INFO` & `matlab-proxy-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
```

### Comparing `matlab-proxy-0.7.2/README.md` & `matlab-proxy-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/README.md` & `matlab-proxy-0.7.3/gui/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/package-lock.json` & `matlab-proxy-0.7.3/gui/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999765783429787%*

 * *Differences: {"'dependencies'": "{'@testing-library/user-event': {'version': '14.4.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@testing-library/user-event/-/user-event-14.4.3.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-kCUc5MEwaEMakkO5x7aoD+DLi02ehmEM2QCGWvNqAS1dV/fAvORWEjnjsEIvml59M7Y5kCkWN6fCCyPOe8OL6Q=='}}",*

 * * "'packages'": "{'': {'devDependencies': {'@testing-library/user-event': '^14.4.3'}}, "*

 * *               "'node_modules/@testing-library/user-event': {'version': '14 […]*

```diff
@@ -2527,18 +2527,18 @@
                 "@types/testing-library__react-hooks": "^3.4.0"
             },
             "resolved": "https://registry.npmjs.org/@testing-library/react-hooks/-/react-hooks-3.7.0.tgz",
             "version": "3.7.0"
         },
         "@testing-library/user-event": {
             "dev": true,
-            "integrity": "sha512-oZ0Ib5I4Z2pUEcoo95cT1cr6slco9WY7yiPpG+RGNkj8YcYgJnM7pXmYmorNOReh8MIGcKSqXyeGjxnr8YiZbA==",
+            "integrity": "sha512-kCUc5MEwaEMakkO5x7aoD+DLi02ehmEM2QCGWvNqAS1dV/fAvORWEjnjsEIvml59M7Y5kCkWN6fCCyPOe8OL6Q==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/@testing-library/user-event/-/user-event-7.2.1.tgz",
-            "version": "7.2.1"
+            "resolved": "https://registry.npmjs.org/@testing-library/user-event/-/user-event-14.4.3.tgz",
+            "version": "14.4.3"
         },
         "@tootallnate/once": {
             "integrity": "sha512-RbzJvlNzmRq5c3O09UipeuXno4tA1FE6ikOjxZK0tuxVv3412l64l5t1W5pj4+rJq9vpkm/kwiR07aZXnsKPxw==",
             "resolved": "https://registry.npmjs.org/@tootallnate/once/-/once-1.1.2.tgz",
             "version": "1.1.2"
         },
         "@trysound/sax": {
@@ -13107,15 +13107,15 @@
                 "reselect": "^4.0.0"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.11.0",
                 "@testing-library/jest-dom": "^4.2.4",
                 "@testing-library/react": "^11.2.6",
                 "@testing-library/react-hooks": "^3.4.1",
-                "@testing-library/user-event": "^7.2.1",
+                "@testing-library/user-event": "^14.4.3",
                 "fetch-mock": "^9.10.7",
                 "react-test-renderer": "^16.13.1",
                 "redux-mock-store": "^1.5.4"
             },
             "name": "matlab-proxy",
             "version": "0.1.0"
         },
@@ -16862,20 +16862,24 @@
             },
             "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
             "version": "7.2.0"
         },
         "node_modules/@testing-library/user-event": {
             "dev": true,
-            "integrity": "sha512-oZ0Ib5I4Z2pUEcoo95cT1cr6slco9WY7yiPpG+RGNkj8YcYgJnM7pXmYmorNOReh8MIGcKSqXyeGjxnr8YiZbA==",
+            "engines": {
+                "node": ">=12",
+                "npm": ">=6"
+            },
+            "integrity": "sha512-kCUc5MEwaEMakkO5x7aoD+DLi02ehmEM2QCGWvNqAS1dV/fAvORWEjnjsEIvml59M7Y5kCkWN6fCCyPOe8OL6Q==",
             "peerDependencies": {
-                "@testing-library/dom": ">=5"
+                "@testing-library/dom": ">=7.21.4"
             },
-            "resolved": "https://registry.npmjs.org/@testing-library/user-event/-/user-event-7.2.1.tgz",
-            "version": "7.2.1"
+            "resolved": "https://registry.npmjs.org/@testing-library/user-event/-/user-event-14.4.3.tgz",
+            "version": "14.4.3"
         },
         "node_modules/@tootallnate/once": {
             "engines": {
                 "node": ">= 6"
             },
             "integrity": "sha512-RbzJvlNzmRq5c3O09UipeuXno4tA1FE6ikOjxZK0tuxVv3412l64l5t1W5pj4+rJq9vpkm/kwiR07aZXnsKPxw==",
             "resolved": "https://registry.npmjs.org/@tootallnate/once/-/once-1.1.2.tgz",
```

### Comparing `matlab-proxy-0.7.2/gui/package.json` & `matlab-proxy-0.7.3/gui/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'devDependencies'": "{'@testing-library/user-event': '^14.4.3'}"}*

```diff
@@ -27,15 +27,15 @@
         "reselect": "^4.0.0"
     },
     "devDependencies": {
         "@babel/preset-env": "^7.11.0",
         "@testing-library/jest-dom": "^4.2.4",
         "@testing-library/react": "^11.2.6",
         "@testing-library/react-hooks": "^3.4.1",
-        "@testing-library/user-event": "^7.2.1",
+        "@testing-library/user-event": "^14.4.3",
         "fetch-mock": "^9.10.7",
         "react-test-renderer": "^16.13.1",
         "redux-mock-store": "^1.5.4"
     },
     "eslintConfig": {
         "extends": "react-app"
     },
```

### Comparing `matlab-proxy-0.7.2/gui/public/favicon.ico` & `matlab-proxy-0.7.3/gui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/public/index.html` & `matlab-proxy-0.7.3/gui/public/index.html`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/actionCreators/actionCreators.spec.js` & `matlab-proxy-0.7.3/gui/src/actionCreators/actionCreators.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/actionCreators/index.js` & `matlab-proxy-0.7.3/gui/src/actionCreators/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,23 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import {
     SET_TRIGGER_POSITION,
     SET_TUTORIAL_HIDDEN,
     SET_OVERLAY_VISIBILITY,
     REQUEST_SERVER_STATUS,
     RECEIVE_SERVER_STATUS,
     REQUEST_SET_LICENSING,
+    REQUEST_UPDATE_LICENSING,
     REQUEST_TERMINATE_INTEGRATION,
     REQUEST_STOP_MATLAB,
     REQUEST_START_MATLAB,
     REQUEST_ENV_CONFIG,
     RECEIVE_SET_LICENSING,
+    RECEIVE_UPDATE_LICENSING,
     RECEIVE_TERMINATE_INTEGRATION,
     RECEIVE_STOP_MATLAB,
     RECEIVE_START_MATLAB,
     RECEIVE_ERROR,
     RECEIVE_ENV_CONFIG,
     SET_AUTH_STATUS,
     SET_AUTH_TOKEN
@@ -98,14 +100,28 @@
 export function receiveSetLicensing(status) {
     return {
         type: RECEIVE_SET_LICENSING,
         status
     };
 }
 
+export function requestUpdateLicensing() {
+    return {
+        type: REQUEST_UPDATE_LICENSING,
+    };
+}
+
+export function receiveUpdateLicensing(status) {
+    return {
+        type: RECEIVE_UPDATE_LICENSING,
+        status
+    };
+}
+
+
 export function requestTerminateIntegration() {
     return {
         type: REQUEST_TERMINATE_INTEGRATION,
     };
 }
 
 export function receiveTerminateIntegration(status) {
@@ -237,14 +253,35 @@
         const response = await fetchWithTimeout(dispatch, './set_licensing_info', options, 15000);
         const data = await response.json();
         dispatch(receiveSetLicensing(data));
 
     }
 }
 
+export function fetchUpdateLicensing(info) {
+    return async function(dispatch, getState) {
+
+        const options = {
+            method: 'PUT',
+            mode: 'same-origin',
+            cache: 'no-cache',
+            credentials: 'same-origin',
+            headers: {
+                'Content-Type': 'application/json'
+            },
+            body: JSON.stringify(info),
+        }
+
+        dispatch(requestUpdateLicensing());
+        const response = await fetchWithTimeout(dispatch, './update_entitlement', options, 1500);
+        const data = await response.json();
+        dispatch(receiveUpdateLicensing(data));
+    }
+}
+
 export function fetchUnsetLicensing() {
     return async function(dispatch, getState) {
 
         const options = {
             method: 'DELETE',
             mode: 'same-origin',
             cache: 'no-cache',
```

### Comparing `matlab-proxy-0.7.2/gui/src/actions/index.js` & `matlab-proxy-0.7.3/gui/src/actions/index.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,21 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 export const SET_TRIGGER_POSITION = 'SET_TRIGGER_POSITION';
 export const SET_TUTORIAL_HIDDEN = 'SET_TUTORIAL_HIDDEN';
 export const SET_OVERLAY_VISIBILITY = 'SET_OVERLAY_VISIBILITY';
 export const REQUEST_SERVER_STATUS = 'REQUEST_SERVER_STATUS';
 export const RECEIVE_SERVER_STATUS = 'RECEIVE_SERVER_STATUS';
 export const REQUEST_SET_LICENSING = 'REQUEST_SET_LICENSING';
+export const REQUEST_UPDATE_LICENSING = 'REQUEST_UPDATE_LICENSING';
 export const REQUEST_TERMINATE_INTEGRATION = 'REQUEST_TERMINATE_INTEGRATION';
 export const REQUEST_STOP_MATLAB = 'REQUEST_STOP_MATLAB';
 export const REQUEST_START_MATLAB = 'REQUEST_START_MATLAB';
 export const RECEIVE_SET_LICENSING = 'RECEIVE_SET_LICENSING';
+export const RECEIVE_UPDATE_LICENSING = 'RECEIVE_UPDATE_LICENSING';
 export const RECEIVE_TERMINATE_INTEGRATION = 'RECEIVE_TERMINATE_INTEGRATION';
 export const RECEIVE_STOP_MATLAB = 'RECEIVE_STOP_MATLAB';
 export const RECEIVE_START_MATLAB = 'RECEIVE_START_MATLAB';
 export const RECEIVE_ERROR = 'RECEIVE_ERROR';
 export const REQUEST_ENV_CONFIG = 'REQUEST_ENV_CONFIG';
 export const RECEIVE_ENV_CONFIG = 'RECEIVE_ENV_CONFIG';
 export const SET_AUTH_STATUS = 'SET_AUTH_STATUS';
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/css/bootstrap.min.css` & `matlab-proxy-0.7.3/gui/src/components/App/3p/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/css/site7.min.css` & `matlab-proxy-0.7.3/gui/src/components/App/3p/css/site7.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-eps.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.ttf` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-eps.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-eps.woff` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-eps.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-pictograms.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks-pictograms.woff` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks-pictograms.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.ttf` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/fonts/mathworks.woff` & `matlab-proxy-0.7.3/gui/src/components/App/3p/fonts/mathworks.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/images/bug_reports/workaround.gif` & `matlab-proxy-0.7.3/gui/src/components/App/3p/images/bug_reports/workaround.gif`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg` & `matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/3p/images/responsive/global/ico-sprite.png` & `matlab-proxy-0.7.3/gui/src/components/App/3p/images/responsive/global/ico-sprite.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/App.css` & `matlab-proxy-0.7.3/gui/src/components/App/App.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/App.spec.js` & `matlab-proxy-0.7.3/gui/src/components/App/App.spec.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import React from 'react';
 import {
     render,
     fireEvent
 } from '../../test/utils/react-test';
 import App from './index';
@@ -180,15 +180,15 @@
         const {
             container
         } = render( < App / > , {
             initialState: initialState,
         });
 
 
-        const paragraphElements = [...container.getElementsByTagName('p')];
+        const paragraphElements = [...container.getElementsByTagName('pre')];
 
 
         expect(
             paragraphElements.some((p) =>
                 p.textContent.includes('integration terminated')
             )
         ).toBe(true);
@@ -204,15 +204,15 @@
 
         const {
             container
         } = render( < App / > , {
             initialState: initialState,
         });
 
-        const paragraphElements = [...container.getElementsByTagName('p')];
+        const paragraphElements = [...container.getElementsByTagName('pre')];
 
         expect(
             paragraphElements.some((p) =>
                 p.textContent.includes(initialState.error.message)
             )
         ).toBe(true);
     });
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/MATLAB-env-blur.png` & `matlab-proxy-0.7.3/gui/src/components/App/MATLAB-env-blur.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/App/index.js` & `matlab-proxy-0.7.3/gui/src/components/App/index.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -31,37 +31,45 @@
     selectMatlabUp,
     selectError,
     selectLoadUrl,
     selectIsConnectionError,
     selectHasFetchedEnvConfig,
     selectAuthEnabled,
     selectIsAuthenticated,
-} from '../../selectors';
+    selectLicensingMhlmHasEntitlements,
+    selectIsEntitled,
+    selectLicensingInfo,
+} from "../../selectors";
+
 import {
     setOverlayVisibility,
     fetchServerStatus,
     fetchEnvConfig,
     updateAuthStatus,
 } from '../../actionCreators';
 import blurredBackground from './MATLAB-env-blur.png';
+import EntitlementSelector from "../EntitlementSelector";
 
 function App() {
     const dispatch = useDispatch();
 
     const overlayVisible = useSelector(selectOverlayVisible);
     const fetchStatusPeriod = useSelector(selectFetchStatusPeriod);
     const hasFetchedServerStatus = useSelector(selectHasFetchedServerStatus);
     const hasFetchedEnvConfig = useSelector(selectHasFetchedEnvConfig);
     const licensingProvided = useSelector(selectLicensingProvided);
+    const hasEntitlements = useSelector(selectLicensingMhlmHasEntitlements);
+    const isEntitled = useSelector(selectIsEntitled);
     const matlabUp = useSelector(selectMatlabUp);
     const error = useSelector(selectError);
     const loadUrl = useSelector(selectLoadUrl);
     const isConnectionError = useSelector(selectIsConnectionError);
     const isAuthenticated = useSelector(selectIsAuthenticated)
     const authEnabled = useSelector(selectAuthEnabled);
+    const licensingInfo = useSelector(selectLicensingInfo);
 
     const baseUrl = useMemo(() => {
         const url = document.URL
         return url.split(window.location.origin)[1].split('index.html')[0]
     }, [])
 
     const toggleOverlayVisible = useCallback(
@@ -168,26 +176,38 @@
         }, [dispatch, baseUrl]);
 
         // Display one of:
         // * Confirmation
         // * Help
         // * Error
         // * License gatherer
+        // * License selector
         // * Status Information
         let overlayContent;
 
         if (dialog) {
             // TODO Inline confirmation component build
             overlayContent = dialog;
         }
         // Give precendence to token auth over licensing info ie. once after token auth is done, show licensing if not provided.
         else if ((!licensingProvided) && hasFetchedServerStatus && (!authEnabled || isAuthenticated)) {
             overlayContent = < LicensingGatherer role = "licensing"
             aria - describedby = "license-window" / > ;
         }
+        // Show license selector if the user has entitlements and is not currently entitled
+        else if (hasEntitlements && !isEntitled) {
+            const options = licensingInfo.entitlements.map((entitlement) => ({
+                label: entitlement.license_number,
+                value: entitlement.id,
+            }));
+            overlayContent = < EntitlementSelector options = {
+                options
+            }
+            />;
+        }
         // in all other cases, we will either ask for the token, 
         else if (!dialog) {
             overlayContent = ( <
                 Information closeHandler = {
                     toggleOverlayVisible
                 } >
                 <
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/Confirmation/Confirmation.spec.js` & `matlab-proxy-0.7.3/gui/src/components/Confirmation/Confirmation.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Confirmation/index.js` & `matlab-proxy-0.7.3/gui/src/components/Confirmation/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/Controls.css` & `matlab-proxy-0.7.3/gui/src/components/Controls/Controls.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/Controls.spec.js` & `matlab-proxy-0.7.3/gui/src/components/Controls/Controls.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/feedback.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/feedback.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/help.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/help.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/index.js` & `matlab-proxy-0.7.3/gui/src/components/Controls/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/restart.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/restart.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/sign-out.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/sign-out.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/start.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/start.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/stop.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/stop.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Controls/terminate.svg` & `matlab-proxy-0.7.3/gui/src/components/Controls/terminate.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Error/Error.spec.js` & `matlab-proxy-0.7.3/gui/src/components/Error/Error.spec.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import React from 'react';
 import Error from './index';
 import {
     render
 } from '../../test/utils/react-test';
 
@@ -25,15 +25,15 @@
                     const {
                         container
                     } = render( < Error message = {
                             message
                         }
                         />);
 
-                        const paragraphs = [...container.getElementsByTagName('p')];
+                        const paragraphs = [...container.getElementsByTagName('pre')];
 
                         expect(paragraphs.some((p) => p.textContent === message)).toBeTruthy();
                     });
 
                 it('should display error logs without crashing', () => {
                     const {
                         debug,
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/Error/index.js` & `matlab-proxy-0.7.3/gui/src/components/Error/index.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import React from 'react';
 import PropTypes from 'prop-types';
 import Linkify from 'react-linkify';
 import './Error.css';
 
 function Error({
@@ -37,17 +37,17 @@
         span className = {
             `alert_icon icon-alert-error`
         } > < /span> <
         h4 className = "modal-title alert_heading" > Error < /h4> <
         /div> <
         div className = "modal-body" >
         <
-        p > {
+        pre > {
             message
-        } < /p> <
+        } < /pre> <
         Linkify > {
             logReport
         } < /Linkify> {
             children
         } <
         /div> <
         /div> <
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/Help/Help.spec.js` & `matlab-proxy-0.7.3/gui/src/components/Help/Help.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Help/index.js` & `matlab-proxy-0.7.3/gui/src/components/Help/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Information/Information.css` & `matlab-proxy-0.7.3/gui/src/components/Information/Information.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Information/Information.spec.js` & `matlab-proxy-0.7.3/gui/src/components/Information/Information.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Information/index.js` & `matlab-proxy-0.7.3/gui/src/components/Information/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import React, {
     useRef,
     useState
 } from 'react';
 import PropTypes from 'prop-types';
 import {
@@ -73,17 +73,25 @@
     const errorMessageNode = error ? ( <
         div className = "error-container alert alert-danger" >
         <
         p > < strong > Error < /strong></p >
         <
         Linkify >
         <
-        div className = "error-text" > {
+        div className = "error-text" > < pre style = {
+            {
+                backgroundColor: 'hsla(0,0%,100%,0)',
+                border: 'none',
+                fontFamily: 'inherit',
+                fontSize: '15px'
+            }
+        } > {
             error.message
-        } < /div> <
+        } < /pre></div >
+        <
         /Linkify> <
         /div>
     ) : null;
 
     const errorLogsNode = (error && error.logs !== null && error.logs.length > 0) ? ( <
         div className = "expand_collapse error-logs-container" >
         <
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/ExistingLicense.js` & `matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/ExistingLicense.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js` & `matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/MHLM.js` & `matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/MHLM.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import React, {
     useState,
     useEffect,
     useMemo
 } from 'react';
 import {
@@ -10,15 +10,15 @@
     useDispatch
 } from 'react-redux';
 import {
     selectLicensingMhlmUsername,
     selectWsEnv
 } from '../../selectors';
 import {
-    fetchSetLicensing
+    fetchSetLicensing,
 } from '../../actionCreators';
 
 // Send a generated nonce to the login iframe
 function setLoginNonce(username) {
     const clientNonce = (Math.random() + "").substr(2);
     const noncePayload = {
         event: "init",
@@ -95,15 +95,14 @@
     useEffect(() => {
 
         const handler = event => {
 
             // Only process events that are related to the iframe setup
             if (event.origin === mhlmLoginHostname) {
                 const data = JSON.parse(event.data);
-
                 if (data.event === 'nonce') {
                     initLogin(
                         data.clientTransactionId,
                         data.transactionId,
                         sourceId
                     );
                 } else if (data.event === 'login') {
```

### Comparing `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/NLM.js` & `matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/NLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/LicensingGatherer/index.js` & `matlab-proxy-0.7.3/gui/src/components/LicensingGatherer/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/MatlabJsd/MatlabJsd.spec.js` & `matlab-proxy-0.7.3/gui/src/components/MatlabJsd/MatlabJsd.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.css` & `matlab-proxy-0.7.3/gui/src/components/Overlay/Overlay.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Overlay/Overlay.spec.js` & `matlab-proxy-0.7.3/gui/src/components/Overlay/Overlay.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/Overlay/index.js` & `matlab-proxy-0.7.3/gui/src/components/Overlay/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.css` & `matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/OverlayTrigger.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js` & `matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js` & `matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/index.js` & `matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-error.svg` & `matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/trigger-error.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/components/OverlayTrigger/trigger-ok.svg` & `matlab-proxy-0.7.3/gui/src/components/OverlayTrigger/trigger-ok.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/index.js` & `matlab-proxy-0.7.3/gui/src/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/logo.svg` & `matlab-proxy-0.7.3/gui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/reducers/index.js` & `matlab-proxy-0.7.3/gui/src/reducers/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/reducers/reducers.spec.js` & `matlab-proxy-0.7.3/gui/src/reducers/reducers.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/selectors/index.js` & `matlab-proxy-0.7.3/gui/src/selectors/index.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import {
     createSelector
 } from 'reselect';
 
 export const selectTutorialHidden = state => state.tutorialHidden;
 export const selectServerStatus = state => state.serverStatus;
@@ -100,25 +100,38 @@
     selectLicensingInfo,
     licensingInfo => Object.prototype.hasOwnProperty.call(licensingInfo, 'type')
 );
 
 export const selectLicensingIsMhlm = createSelector(
     selectLicensingInfo,
     selectLicensingProvided,
-    (licensingInfo, licensingProvided) => licensingProvided && licensingInfo.type === 'MHLM'
+    (licensingInfo, licensingProvided) => licensingProvided && licensingInfo.type === 'mhlm'
 );
 
 export const selectLicensingMhlmUsername = createSelector(
     selectLicensingInfo,
     selectLicensingIsMhlm,
     (licensingInfo, isMhlm) => isMhlm ? licensingInfo.emailAddress : ''
 );
 
+// Selector to check if the license type is mhlm and entitlements property is not empty
+export const selectLicensingMhlmHasEntitlements = createSelector(
+    selectLicensingIsMhlm,
+    selectLicensingInfo,
+    (isMhlm, licensingInfo) => isMhlm && licensingInfo.entitlements && licensingInfo.entitlements.length > 0
+);
+
+export const selectIsEntitled = createSelector(
+    selectLicensingInfo,
+    selectLicensingMhlmHasEntitlements,
+    (licensingInfo, entitlementIdInfo) => entitlementIdInfo && licensingInfo.entitlementId
+);
+
 // TODO Are these overkill? Perhaps just selecting status would be enough
-// TODO Could be used for detected intermedia failures, such as server being
+// TODO Could be used for detected intermediate failures, such as server being
 // temporarily inaccessible
 export const selectMatlabPending = createSelector(
     selectMatlabStatus,
     matlabStatus => matlabStatus === 'starting'
 );
 
 export const selectOverlayVisible = createSelector(
```

### Comparing `matlab-proxy-0.7.2/gui/src/selectors/selectors.spec.js` & `matlab-proxy-0.7.3/gui/src/selectors/selectors.spec.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// Copyright (c) 2020-2022 The MathWorks, Inc.
+// Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import * as selectors from './index';
 const _ = require('lodash');
 
 describe('selectors', () => {
     let modifiedState;
     let state = {
@@ -16,15 +16,15 @@
         error: null,
         serverStatus: {
             matlabStatus: 'up',
             matlabVersion: 'R2020b',
             isSubmitting: true,
             hasFetched: false,
             licensingInfo: {
-                type: 'MHLM',
+                type: 'mhlm',
                 emailAddress: 'abc@mathworks.com',
             },
             fetchFailCount: 2,
         },
         authInfo: {
             authEnabled: false,
             authStatus: false,
```

### Comparing `matlab-proxy-0.7.2/gui/src/serviceWorker.js` & `matlab-proxy-0.7.3/gui/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/gui/src/test/utils/react-test.js` & `matlab-proxy-0.7.3/gui/src/test/utils/react-test.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/__init__.py` & `matlab-proxy-0.7.3/matlab_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/app.py` & `matlab-proxy-0.7.3/matlab_proxy/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 import matlab_proxy
 from matlab_proxy import settings, util
 from matlab_proxy.app_state import AppState
 from matlab_proxy.default_configuration import config
 from matlab_proxy.util import list_servers, mwi
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
-from matlab_proxy.util.mwi.exceptions import AppError, InvalidTokenError, LicensingError
+from matlab_proxy.util.mwi.exceptions import (
+    AppError,
+    InvalidTokenError,
+    LicensingError,
+)
 
 mimetypes.add_type("font/woff", ".woff")
 mimetypes.add_type("font/woff2", ".woff2")
 mimetypes.add_type("font/eot", ".eot")
 mimetypes.add_type("font/ttf", ".ttf")
 mimetypes.add_type("application/json", ".map")
 mimetypes.add_type("image/png", ".ico")
@@ -105,20 +109,20 @@
     """
     state = app["state"]
 
     return web.json_response(
         {
             "matlab": {
                 "status": await state.get_matlab_state(),
-                "version": state.settings["matlab_version"],
+                "version": state.settings.get("matlab_version", "Unknown"),
             },
             "licensing": marshal_licensing_info(state.licensing),
             "loadUrl": loadUrl,
             "error": marshal_error(state.error),
-            "wsEnv": state.settings["ws_env"],
+            "wsEnv": state.settings.get("ws_env", ""),
         }
     )
 
 
 async def get_env_config(req):
     """API Endpoint to get Matlab Web Desktop environment specific configuration.
 
@@ -156,15 +160,14 @@
 
 async def authenticate_request(req):
     """API Endpoint to authenticate request to access server
 
     Returns:
         JSONResponse: JSONResponse object containing information about authentication status and error if any.
     """
-    state = req.app["state"]
     if await token_auth.authenticate_request(req):
         logger.debug("!!!!!! REQUEST IS AUTHORIZED !!!!")
         authStatus = True
         error = None
     else:
         logger.debug("!!!!!! REQUEST IS NOT AUTHORIZED !!!!")
         authStatus = False
@@ -252,22 +255,49 @@
         else:
             raise Exception(
                 'License type must be "NLM" or "MHLM" or "ExistingLicense"!'
             )
     except Exception as e:
         raise web.HTTPBadRequest(text="Error with licensing!")
 
-    # Start MATLAB if licensing is complete
-    if state.is_licensed() is True and not isinstance(state.error, LicensingError):
-        # Start MATLAB
-        await state.start_matlab(restart_matlab=True)
+    # This is true for a user who has only one license associated with their account
+    await __start_matlab_if_licensed(state)
+
+    return await create_status_response(req.app)
+
+
+async def update_entitlement(req):
+    """API endpoint to update selected entitlement to start MATLAB with.
+
+    Args:
+        req (HTTPRequest): HTTPRequest Object
+
+    Returns:
+        JSONResponse: JSONResponse object containing updated information on the state of MATLAB among other information.
+    """
+    state = req.app["state"]
+    data = await req.json()
+    lic_type = data.get("type")
+
+    # Set the entitlement id only if we are not already licensed
+    if lic_type == "mhlm" and not state.is_licensed():
+        entitlement_id = data.get("entitlement_id")
+        logger.debug(f"Received type: {lic_type}, entitlement_id: {entitlement_id}")
+        await state.update_user_selected_entitlement_info(entitlement_id)
+        await __start_matlab_if_licensed(state)
 
     return await create_status_response(req.app)
 
 
+async def __start_matlab_if_licensed(state):
+    # Start MATLAB if licensing is complete
+    if state.is_licensed() and not isinstance(state.error, LicensingError):
+        await state.start_matlab(restart_matlab=True)
+
+
 async def licensing_info_delete(req):
     """API Endpoint to stop MATLAB and remove licensing details.
 
     Args:
         req (HTTPRequest): HTTPRequest Object
     Returns:
         JSONResponse: JSONResponse object containing updated information on the state of MATLAB among other information.
@@ -675,14 +705,15 @@
     app.router.add_route(
         "POST", f"{base_url}/authenticate_request", authenticate_request
     )
     app.router.add_route("GET", f"{base_url}/get_env_config", get_env_config)
     app.router.add_route("PUT", f"{base_url}/start_matlab", start_matlab)
     app.router.add_route("DELETE", f"{base_url}/stop_matlab", stop_matlab)
     app.router.add_route("PUT", f"{base_url}/set_licensing_info", set_licensing_info)
+    app.router.add_route("PUT", f"{base_url}/update_entitlement", update_entitlement)
     app.router.add_route(
         "DELETE", f"{base_url}/set_licensing_info", licensing_info_delete
     )
     app.router.add_route(
         "DELETE", f"{base_url}/terminate_integration", termination_integration_delete
     )
     app.router.add_route("*", f"{base_url}/", root_redirect)
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy/app_state.py` & `matlab-proxy-0.7.3/matlab_proxy/app_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import asyncio
 import json
 import logging
 import os
 import time
 from collections import deque
@@ -11,18 +11,17 @@
 from matlab_proxy import util
 from matlab_proxy.util import mw, mwi, system, windows
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
 from matlab_proxy.util.mwi.exceptions import (
     EmbeddedConnectorError,
     EntitlementError,
-    InternalError,
+    FatalError,
     LicensingError,
     MatlabError,
-    MatlabInstallError,
     OnlineLicensingError,
     XvfbError,
     log_error,
 )
 from matlab_proxy.constants import CONNECTOR_SECUREPORT_FILENAME
 
 logger = mwi.logger.get()
@@ -66,19 +65,20 @@
         }
 
         self.licensing = None
         self.tasks = {}
         self.logs = {
             "matlab": deque(maxlen=200),
         }
-        self.error = None
-        # Start in an error state if MATLAB is not present
-        if not self.is_matlab_present():
-            self.error = MatlabInstallError("'matlab' executable not found in PATH")
-            logger.error("'matlab' executable not found in PATH")
+
+        # Initialize with the error state from the initialization of settings
+        self.error = settings["error"]
+
+        if self.error is not None:
+            self.logs["matlab"].clear()
             return
 
         # Keep track of when the Embedded connector starts.
         # Would be initialized appropriately by get_embedded_connector_state() task.
         self.embedded_connector_start_time = None
 
         # Keep track of the state of the Embedded Connector.
@@ -149,16 +149,16 @@
                 f"!!! Launching MATLAB without providing any additional licensing information. This requires MATLAB to have been activated on the machine from which its being launched !!!"
             )
 
             # Delete old licensing mode info from cache to ensure its wiped out first before persisting new info.
             self.__delete_cached_licensing_file()
 
         # NLM Connection String set in environment
-        elif self.settings["nlm_conn_str"] is not None:
-            nlm_licensing_str = self.settings["nlm_conn_str"]
+        elif self.settings.get("nlm_conn_str", None) is not None:
+            nlm_licensing_str = self.settings.get("nlm_conn_str")
             logger.debug(f"Found NLM:[{nlm_licensing_str}] set in environment")
             logger.debug(f"Using NLM string to connect ... ")
             self.licensing = {
                 "type": "nlm",
                 "conn_str": nlm_licensing_str,
             }
 
@@ -327,15 +327,14 @@
         Args:
             identity_token (String): Identity token of the user.
             email_addr (String): Email address of the user.
             source_id (String): Unique random string generated for the user.
             entitlements (list, optional): Eligible Entitlements of the user. Defaults to [].
             entitlement_id (String, optional): ID of an entitlement. Defaults to None.
         """
-
         try:
             token_data = await mw.fetch_expand_token(
                 self.settings["mwa_api_endpoint"], identity_token, source_id
             )
 
             self.licensing = {
                 "type": "mhlm",
@@ -392,34 +391,25 @@
                     and self.licensing.get("entitlement_id") is not None
                 ):
                     return True
             elif self.licensing["type"] == "existing_license":
                 return True
         return False
 
-    def is_matlab_present(self):
-        """Is MATLAB install accessible?
-
-        Returns:
-            Boolean: True if MATLAB is present in the system. False otherwise.
-        """
-
-        return self.settings["matlab_path"] is not None
-
     async def update_entitlements(self):
         """Speaks to MW and updates MHLM entitlements
 
         Raises:
-            InternalError: When licensing is None or when licensing type is not MHLM.
+            FatalError: When licensing is None or when licensing type is not MHLM.
 
         Returns:
             Boolean: True if update was successful
         """
         if self.licensing is None or self.licensing["type"] != "mhlm":
-            raise InternalError(
+            raise FatalError(
                 "MHLM licensing must be configured to update entitlements!"
             )
 
         try:
             # Fetch an access token
             access_token_data = await mw.fetch_access_token(
                 self.settings["mwa_api_endpoint"],
@@ -430,42 +420,61 @@
             # Fetch entitlements
             entitlements = await mw.fetch_entitlements(
                 self.settings["mhlm_api_endpoint"],
                 access_token_data["token"],
                 self.settings["matlab_version"],
             )
 
-        except OnlineLicensingError as e:
-            self.error = e
-            log_error(logger, e)
-            return False
         except EntitlementError as e:
             self.error = e
             log_error(logger, e)
             self.licensing["identity_token"] = None
             self.licensing["source_id"] = None
             self.licensing["expiry"] = None
             self.licensing["first_name"] = None
             self.licensing["last_name"] = None
             self.licensing["display_name"] = None
             self.licensing["user_id"] = None
             self.licensing["profile_id"] = None
             self.licensing["entitlements"] = []
             self.licensing["entitlement_id"] = None
+            # To ensure that any entitlement errors are displayed on the control panel,
+            # the function returns true. The cached license file only contains the license type
+            # and the user's email address. These two attributes are necessary for preventing
+            # the LicenseGatherer step from becoming stuck on the front-end side.
+            # Additionally, displaying the license type and user email address on the
+            # information panel makes it worthwhile to maintain these attributes in the state.
+            return True
+
+        except OnlineLicensingError as e:
+            self.error = e
+            log_error(logger, e)
+            return False
+
+        # Keeping base error class at the last to catch any uncaught licensing related issues
+        except OnlineLicensingError as e:
+            self.error = e
+            log_error(logger, e)
             return False
 
         self.licensing["entitlements"] = entitlements
 
-        # If there is only one non-expired entitlement, set it as active
-        # TODO Also, for now, set the first entitlement as active if there are multiple
-        self.licensing["entitlement_id"] = entitlements[0]["id"]
+        # Auto-select the entitlement if only one entitlement is returned from MHLM
+        if len(entitlements) == 1:
+            self.licensing["entitlement_id"] = entitlements[0]["id"]
 
         # Successful update
         return True
 
+    # Set the entitlement information on app state as well as the cached file
+    async def update_user_selected_entitlement_info(self, entitlement_id):
+        self.licensing["entitlement_id"] = entitlement_id
+        logger.debug(f"Successfully set {entitlement_id} as the entitlement_id")
+        self.persist_licensing()
+
     def persist_licensing(self):
         """Saves licensing information to file"""
         if self.licensing is None:
             self.__delete_cached_licensing_file()
 
         elif self.licensing["type"] in ["mhlm", "nlm", "existing_license"]:
             logger.debug("Saving licensing information...")
@@ -700,34 +709,16 @@
         return None
 
     async def start_matlab(self, restart_matlab=False):
         """Start MATLAB.
 
         Args:
             restart_matlab (bool, optional): Whether to restart MATLAB. Defaults to False.
-
-        Raises:
-            Exception: When MATLAB is already running and restart is False.
-            Exception: When MATLAB is not licensed.
         """
 
-        # FIXME
-        if await self.get_matlab_state() != "down" and restart_matlab is False:
-            raise Exception("MATLAB already running/starting!")
-
-        # FIXME
-        if not self.is_licensed():
-            raise Exception("MATLAB is not licensed!")
-
-        if not self.is_matlab_present():
-            self.error = MatlabInstallError("'matlab' executable not found in PATH")
-            logger.error("'matlab' executable not found in PATH")
-            self.logs["matlab"].clear()
-            return
-
         # Ensure that previous processes are stopped
         await self.stop_matlab()
 
         # Clear MATLAB errors and logging
         self.error = None
         self.logs["matlab"].clear()
 
@@ -915,18 +906,18 @@
                 self.matlab_port = int(f.read())
                 logger.debug(
                     f"MATLAB Ready file successfully read, matlab_port set to: {self.matlab_port}"
                 )
 
         loop = util.get_event_loop()
         # Start all tasks relevant to MATLAB process
-        self.tasks["matlab_stderr_reader_posix()"] = loop.create_task(
+        self.tasks["matlab_stderr_reader_posix"] = loop.create_task(
             __matlab_stderr_reader_posix()
         )
-        self.tasks["track_embedded_connector_state()"] = loop.create_task(
+        self.tasks["track_embedded_connector_state"] = loop.create_task(
             __track_embedded_connector_state()
         )
         self.tasks["update_matlab_port"] = loop.create_task(
             __update_matlab_port(self.MATLAB_PORT_CHECK_DELAY_IN_SECONDS)
         )
 
     """
@@ -1100,15 +1091,15 @@
                             )
                             try:
                                 matlab.terminate()
                                 matlab.wait()
                             except:
                                 pass
 
-        logger.info("Stopped (any running)MATLAB process.")
+        logger.info("Stopped (any running) MATLAB process.")
 
         # Terminating Xvfb
         if system.is_posix():
             xvfb = self.processes["xvfb"]
             if xvfb is not None and xvfb.returncode is None:
                 logger.info(f"Terminating Xvfb (PID={xvfb.pid})")
                 xvfb.terminate()
@@ -1133,14 +1124,16 @@
         self.tasks = {}
 
         # Clear logs if MATLAB stopped intentionally
         logger.debug("Clearing logs!")
         self.logs["matlab"].clear()
         logger.debug("Cleared any logs created by the MATLAB process.")
 
+        # Update matlab_port information in the event of intentionally stopping MATLAB
+        self.matlab_port = None
         logger.debug("Completed Shutdown!!!")
 
     async def handle_matlab_output(self):
         """Parse MATLAB output from stdout and raise errors if any."""
         matlab = self.processes["matlab"]
 
         # Wait for MATLAB process to exit
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy/default_configuration.py` & `matlab-proxy-0.7.3/matlab_proxy/default_configuration.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/devel.py` & `matlab-proxy-0.7.3/matlab_proxy/devel.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/icons/matlab.svg` & `matlab-proxy-0.7.3/matlab_proxy/icons/matlab.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/matlab/startup.m` & `matlab-proxy-0.7.3/matlab_proxy/matlab/startup.m`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/settings.py` & `matlab-proxy-0.7.3/matlab_proxy/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,81 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 
+from pathlib import Path
 import os
 import shutil
 import socket
 import ssl
-import sys
 import tempfile
 import uuid
 import xml.etree.ElementTree as ET
-from pathlib import Path
 
 import matlab_proxy
 from matlab_proxy.constants import VERSION_INFO_FILE_NAME
 from matlab_proxy.util import mwi, system
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
+from matlab_proxy.util.mwi.exceptions import (
+    FatalError,
+    MatlabInstallError,
+    UIVisibleFatalError,
+)
 
 logger = mwi.logger.get()
 
 
-def get_matlab_root_path():
+def get_matlab_executable_and_root_path():
     """Returns the path from the MWI_CUSTOM_MATLAB_ROOT environment variable if valid, else returns
     MATLAB root based on the matlab executable if found on the system path.
 
     Returns:
-        pathlib.Path: pathlib.Path object to MATLAB root.
+        pathlib.Path: pathlib.Path objects to MATLAB executable & MATLAB root.
     """
+
+    # Use custom matlab root path if provided.
     custom_matlab_root_path = os.environ.get(mwi_env.get_env_name_custom_matlab_root())
 
-    if custom_matlab_root_path and mwi.validators.validate_custom_matlab_root_path(
-        Path(custom_matlab_root_path)
-    ):
-        return custom_matlab_root_path
+    if custom_matlab_root_path:
+        matlab_root_path = Path(custom_matlab_root_path)
 
-    which_matlab = shutil.which("matlab")
+        # Terminate process if invalid Custom Path was provided!
+        mwi.validators.terminate_on_invalid_matlab_root_path(
+            matlab_root_path, is_custom_matlab_root=True
+        )
 
-    return Path(which_matlab).resolve().parent.parent if which_matlab else None
+        # Generate executable path from root path
+        matlab_executable_path = matlab_root_path / "bin" / "matlab"
+        if system.is_windows():
+            matlab_executable_path = matlab_executable_path.with_suffix(".exe")
 
+        logger.info(
+            f"Using Custom MATLAB Executable: {matlab_executable_path} with Root: {matlab_root_path}"
+        )
+        return matlab_executable_path, matlab_root_path
 
-def get_matlab_executable_path(matlab_root_path: Path):
-    """Returns path to the MATLAB executable based on the OS
+    # Custom matlab root not specified, search for MATLAB on system path
+    matlab_executable_path = shutil.which("matlab")
 
-    Args:
-        matlab_root_path (Path): Path to MATLAB Root
+    if matlab_executable_path:
+        matlab_root_path = Path(matlab_executable_path).resolve().parent.parent
+        mwi.validators.terminate_on_invalid_matlab_root_path(
+            matlab_root_path, is_custom_matlab_root=False
+        )
+        logger.info(
+            f"Found MATLAB Executable: {matlab_executable_path} with Root: {matlab_root_path}"
+        )
+        return matlab_executable_path, matlab_root_path
 
-    Returns:
-        [Path | None]: Path to MATLAB executable if a valid MATLAB root path is supplied else return None
-    """
-    if not matlab_root_path:
-        return None
+    # Control only gets here if custom matlab root was not set AND which matlab returned no results.
+    # Note, error messages are formatted as multi-line strings and the front end displays them as is.
+    error_message = f"""Unable to find MATLAB on the system PATH.
+Add MATLAB to the system PATH, and restart matlab-proxy."""
 
-    return (
-        matlab_root_path / "bin" / "matlab"
-        if system.is_posix()
-        else matlab_root_path / "bin" / "matlab.exe"
-    )
+    logger.info(error_message)
+    raise MatlabInstallError(error_message)
 
 
 def get_matlab_version(matlab_root_path):
     """Returns MATLAB version from VersionInfo.xml file present at matlab_root_path
 
     Args:
         matlab_root_path (pathlib.Path): pathlib.Path to MATLAB root.
@@ -96,14 +113,15 @@
 
 def get_dev_settings(config):
     devel_file = Path(__file__).resolve().parent / "./devel.py"
     mwi_config_folder = get_mwi_config_folder(dev=True)
     ws_env, ws_env_suffix = get_ws_env_settings()
     mwi_auth_token = token_auth.generate_mwi_auth_token()
     return {
+        "error": None,
         "matlab_path": Path(),
         "matlab_version": "R2020b",
         "matlab_cmd": [
             "python",
             "-u",
             str(devel_file),
             "matlab",
@@ -121,15 +139,14 @@
         "mwa_api_endpoint": f"https://login{ws_env_suffix}.mathworks.com/authenticationws/service/v4",
         "mhlm_api_endpoint": f"https://licensing{ws_env_suffix}.mathworks.com/mls/service/v1/entitlement/list",
         "mwa_login": f"https://login{ws_env_suffix}.mathworks.com",
         "mwi_custom_http_headers": mwi.custom_http_headers.get(),
         "env_config": mwi.validators.validate_env_config(config),
         "ssl_context": None,
         "mwi_logs_root_dir": get_mwi_logs_root_dir(dev=True),
-        "mwi_proxy_lock_file_name": "mwi_proxy.lock",
         "mw_context_tags": get_mw_context_tags(matlab_proxy.get_default_config_name()),
         "mwi_server_url": None,
         "mwi_is_token_auth_enabled": mwi_auth_token != None,
         "mwi_auth_status": False,
         "mwi_auth_token": mwi_auth_token,
         "mwi_auth_token_name": mwi_env.get_env_name_mwi_auth_token().lower(),
         "mwi_use_existing_license": mwi.validators.validate_use_existing_licensing(
@@ -144,14 +161,21 @@
 
     Args:
         config : Dictionary as specified by the default_configuration.py file. Used to customize the app.
         dev (bool, optional): development environment. Defaults to False.
 
     Returns:
         Dict: Containing data on how to start MATLAB among other information.
+
+    Raises:
+        Initialization of settings is not exception safe.
+        Exceptions of Type UIVisibleFatalError are not propagated upwards, and are instead set in the error data member.
+        This will allow for the app to error out gracefully in the front end as well.
+
+        All other exceptions will propagate upwards and result in the app to shutdown.
     """
 
     if dev:
         settings = get_dev_settings(config_name)
 
         # If running tests using Pytest, it will set environment variable TEST to true before running tests.
         # Will make test env specific changes before returning the settings.
@@ -165,106 +189,135 @@
             # Randomly picks an available port and updates the value of settings['app_port'] .
             s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             s.bind(("", 0))
             settings["app_port"] = s.getsockname()[1]
             s.close()
 
             # Set NLM Connection string. Server will start using this connection string for licensing
-            settings["nlm_conn_str"] = "abc@nlm"
-
-        return settings
+            settings["nlm_conn_str"] = "123@nlm"
 
     else:
-        matlab_startup_file = str(
-            Path(__file__).resolve().parent / "matlab" / "startup.m"
-        )
-        matlab_path = get_matlab_root_path()
-        matlab_executable_path = get_matlab_executable_path(Path(matlab_path))
-        ws_env, ws_env_suffix = get_ws_env_settings()
-
-        ssl_key_file, ssl_cert_file = mwi.validators.validate_ssl_key_and_cert_file(
-            os.getenv(mwi_env.get_env_name_ssl_key_file(), None),
-            os.getenv(mwi_env.get_env_name_ssl_cert_file(), None),
-        )
+        settings = {"error": None}
 
-        mwi_auth_token = token_auth.generate_mwi_auth_token()
+        # Initializing server settings separately allows us to return
+        # a minimal set of settings required to launch the server even if
+        # there is an exception thrown when creating the matlab specific settings.
+        settings.update(get_server_settings(config_name))
 
-        # MATLAB Proxy gives precedence to the licensing information conveyed
-        # by the user. If MLM_LICENSE_FILE is set, it should be prioritised over
-        # other ways of licensing. But existence of license_info.xml in matlab/licenses
-        # folder may cause hinderance in this workflow. So specifying -licmode as 'file'
-        # overrides license_info.xml and enforces MLM_LICENSE_FILE to be the topmost priority
-
-        # NLM Connection String provided by MLM_LICENSE_FILE environment variable
-        nlm_conn_str = mwi.validators.validate_mlm_license_file(
-            os.environ.get(mwi_env.get_env_name_network_license_manager())
-        )
-        matlab_lic_mode = ["-licmode", "file"] if nlm_conn_str else ""
+        try:
+            # Update settings with matlab specific values.
+            settings.update(get_matlab_settings())
+        except UIVisibleFatalError as error:
+            logger.error(f"Exception raised during initialization: {error}")
+            settings["error"] = error
+            # Exceptions of this kind must propagate to the UI.
+            # Returning settings that have been created without exceptions
+            pass
 
-        # flag to hide MATLAB Window
-        flag_to_hide_desktop = (
-            "-noDisplayDesktop" if system.is_windows() else "-nodesktop"
-        )
+    return settings
+
+
+def get_server_settings(config_name):
+    """Get the settings required to launch the MATLAB-PROXY web server.
+
+    Args:
+    config : Dictionary as specified by the default_configuration.py file. Used to customize the app.
+    dev (bool, optional): development environment. Defaults to False.
 
-        # All config related to matlab-proxy will be saved to user's home folder.
-        # This will allow for other user's to launch the integration from the same system
-        # and not have their config's overwritten.
-        mwi_config_folder = get_mwi_config_folder()
-        return {
-            "matlab_path": matlab_path,
-            "matlab_version": get_matlab_version(matlab_path),
-            "matlab_cmd": [
-                matlab_executable_path,
-                "-nosplash",
-                flag_to_hide_desktop,
-                "-softwareopengl",
-                *matlab_lic_mode,
-                "-r",
-                f"try; run('{matlab_startup_file}'); catch ME; disp(ME.message); end;",
-            ],
-            "create_xvfb_cmd": create_xvfb_cmd,
-            "base_url": mwi.validators.validate_base_url(
-                os.getenv(mwi_env.get_env_name_base_url(), "")
-            ),
-            "app_port": mwi.validators.validate_app_port_is_free(
-                os.getenv(mwi_env.get_env_name_app_port())
-            ),
-            # Set default to host interface to 0.0.0.0
-            "host_interface": os.environ.get(
-                mwi_env.get_env_name_app_host(), "0.0.0.0"
-            ),
-            "mwapikey": str(uuid.uuid4()),
-            "matlab_protocol": "https",
-            "nlm_conn_str": nlm_conn_str,
-            "matlab_config_file": mwi_config_folder / "proxy_app_config.json",
-            "ws_env": ws_env,
-            "mwa_api_endpoint": f"https://login{ws_env_suffix}.mathworks.com/authenticationws/service/v4",
-            "mhlm_api_endpoint": f"https://licensing{ws_env_suffix}.mathworks.com/mls/service/v1/entitlement/list",
-            "mwa_login": f"https://login{ws_env_suffix}.mathworks.com",
-            "mwi_custom_http_headers": mwi.custom_http_headers.get(),
-            "env_config": mwi.validators.validate_env_config(config_name),
-            "ssl_context": get_ssl_context(
-                ssl_cert_file=ssl_cert_file, ssl_key_file=ssl_key_file
-            ),
-            # This directory will be used to store connector.securePort(matlab_ready_file) and its corresponding files. This will be
-            # a central place to store logs of all the running instances of MATLAB launched by matlab-proxy
-            "mwi_logs_root_dir": get_mwi_logs_root_dir(),
-            # Name of the lock file which will be created by this instance of matlab-proxy process.
-            "mwi_proxy_lock_file_name": "mwi_proxy.lock",
-            "mw_context_tags": get_mw_context_tags(config_name),
-            # The url where the matlab-proxy server is accessible at
-            "mwi_server_url": None,
-            "mwi_is_token_auth_enabled": mwi_auth_token != None,
-            "mwi_auth_status": False,
-            "mwi_auth_token": mwi_auth_token,
-            "mwi_auth_token_name": mwi_env.get_env_name_mwi_auth_token().lower(),
-            "mwi_use_existing_license": mwi.validators.validate_use_existing_licensing(
-                os.getenv(mwi_env.get_env_name_mwi_use_existing_license(), "")
-            ),
-        }
+    Raises:
+    This function is not exception safe, and all exceptions will result in the termination of the app.
+    If you need to add exceptions which need to be presented in the UI, add them to get_matlab_settings
+    """
+    mwi_auth_token = token_auth.generate_mwi_auth_token()
+    mwi_config_folder = get_mwi_config_folder()
+    ssl_key_file, ssl_cert_file = mwi.validators.validate_ssl_key_and_cert_file(
+        os.getenv(mwi_env.get_env_name_ssl_key_file(), None),
+        os.getenv(mwi_env.get_env_name_ssl_cert_file(), None),
+    )
+    return {
+        "create_xvfb_cmd": create_xvfb_cmd,
+        "base_url": mwi.validators.validate_base_url(
+            os.getenv(mwi_env.get_env_name_base_url(), "")
+        ),
+        # Set default to host interface to 0.0.0.0
+        "host_interface": os.environ.get(mwi_env.get_env_name_app_host(), "0.0.0.0"),
+        # not_exception_safe, can_terminate_process by throwing FatalError
+        "app_port": mwi.validators.validate_app_port_is_free(
+            os.getenv(mwi_env.get_env_name_app_port())
+        ),
+        "env_config": mwi.validators.validate_env_config(config_name),
+        "mwapikey": str(uuid.uuid4()),
+        "matlab_protocol": "https",
+        "matlab_config_file": mwi_config_folder / "proxy_app_config.json",
+        "mwi_custom_http_headers": mwi.custom_http_headers.get(),
+        # This directory will be used to store connector.securePort(matlab_ready_file) and its corresponding files. This will be
+        # a central place to store logs of all the running instances of MATLAB launched by matlab-proxy
+        "mwi_logs_root_dir": get_mwi_logs_root_dir(),
+        "mw_context_tags": get_mw_context_tags(config_name),
+        # The url where the matlab-proxy server is accessible at
+        "mwi_server_url": None,
+        "mwi_is_token_auth_enabled": mwi_auth_token != None,
+        "mwi_auth_status": False,
+        "mwi_auth_token": mwi_auth_token,
+        "mwi_auth_token_name": mwi_env.get_env_name_mwi_auth_token().lower(),
+        "mwi_use_existing_license": mwi.validators.validate_use_existing_licensing(
+            os.getenv(mwi_env.get_env_name_mwi_use_existing_license(), "")
+        ),
+        "ssl_context": get_ssl_context(
+            ssl_cert_file=ssl_cert_file, ssl_key_file=ssl_key_file
+        ),
+    }
+
+
+def get_matlab_settings():
+    """Returns the settings required to start MATLAB.
+
+    Returns:
+        Dict: Containing data on how to start MATLAB among other information.
+    Raises:
+    This function is not exception safe, and all exceptions will result in the termination of the app.
+    Unless they are of type UIVisibleFatalError
+    """
+
+    matlab_executable_path, matlab_root_path = get_matlab_executable_and_root_path()
+
+    ws_env, ws_env_suffix = get_ws_env_settings()
+
+    # MATLAB Proxy gives precedence to the licensing information conveyed
+    # by the user. If MLM_LICENSE_FILE is set, it should be prioritised over
+    # other ways of licensing. But existence of license_info.xml in matlab/licenses
+    # folder may cause hinderance in this workflow. So specifying -licmode as 'file'
+    # overrides license_info.xml and enforces MLM_LICENSE_FILE to be the topmost priority
+
+    # NLM Connection String provided by MLM_LICENSE_FILE environment variable
+    nlm_conn_str = mwi.validators.validate_mlm_license_file(
+        os.environ.get(mwi_env.get_env_name_network_license_manager())
+    )
+    matlab_lic_mode = ["-licmode", "file"] if nlm_conn_str else ""
+    # flag to hide MATLAB Window
+    flag_to_hide_desktop = "-noDisplayDesktop" if system.is_windows() else "-nodesktop"
+    matlab_startup_file = str(Path(__file__).resolve().parent / "matlab" / "startup.m")
+    return {
+        "matlab_path": matlab_root_path,
+        "matlab_version": get_matlab_version(matlab_root_path),
+        "matlab_cmd": [
+            matlab_executable_path,
+            "-nosplash",
+            flag_to_hide_desktop,
+            "-softwareopengl",
+            *matlab_lic_mode,
+            "-r",
+            f"try; run('{matlab_startup_file}'); catch ME; disp(ME.message); end;",
+        ],
+        "ws_env": ws_env,
+        "mwa_api_endpoint": f"https://login{ws_env_suffix}.mathworks.com/authenticationws/service/v4",
+        "mhlm_api_endpoint": f"https://licensing{ws_env_suffix}.mathworks.com/mls/service/v1/entitlement/list",
+        "mwa_login": f"https://login{ws_env_suffix}.mathworks.com",
+        "nlm_conn_str": nlm_conn_str,
+    }
 
 
 def get_mw_context_tags(extension_name):
     """Returns a string which combines existing MW_CONTEXT_TAGS value and context tags
     specific to where matlab-proxy is being launched from.
 
     Returns:
@@ -344,18 +397,19 @@
     if ssl_cert_file != None:
         try:
             ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
             ssl_context.load_cert_chain(ssl_cert_file, ssl_key_file)
             logger.debug(f"Using SSL certification!")
         except Exception as e:
             # Something was wrong with the certificates provided
-            logger.error("SSL certificates provided are invalid. Aborting...")
+            error_message = "SSL certificates provided are invalid. Aborting..."
+            logger.error(error_message)
             traceback.print_exc()
             logger.info("==== Fatal error : ===")
             print(e)
             # printing stack trace
             logger.info("======================")
-            sys.exit(1)
+            raise FatalError(error_message)
     else:
         ssl_context = None
 
     return ssl_context
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/__init__.py` & `matlab-proxy-0.7.3/matlab_proxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/event_loop.py` & `matlab-proxy-0.7.3/matlab_proxy/util/event_loop.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/list_servers.py` & `matlab-proxy-0.7.3/matlab_proxy/util/list_servers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mw.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 
 import asyncio
 import os
 import select
 import xml.etree.ElementTree as ET
 
 import aiohttp
@@ -65,15 +65,15 @@
                 )
 
             root = ET.fromstring(await res.text())
             entitlement_el = root.find("entitlements")
 
             if entitlement_el is None or len(entitlement_el) == 0:
                 raise EntitlementError(
-                    f"Your MathWorks account is not linked to a valid license for MATLAB {matlab_release}."
+                    f"Your MathWorks account is not linked to a valid license for MATLAB {matlab_release}.\nSign out and login with a licensed user."
                 )
 
             entitlements = entitlement_el.findall("entitlement")
 
             return [
                 {
                     "id": entitlement.find("id").text,
@@ -81,15 +81,15 @@
                     "license_number": entitlement.find("license_number").text,
                 }
                 for entitlement in entitlements
             ]
 
 
 async def fetch_expand_token(mwa_api_endpoint, identity_token, source_id):
-    """Asynchronously fetch tokens from MWA API after MHLM licensing is successful.
+    """Asynchronously fetch tokens from MWA API endpoint.
 
     Args:
         mwa_api_endpoint (String): URL of the MWA API endpoint.
         identity_token (String): Identity token received from MHLM servers by the front end.
         source_id (String): Source ID received from MHLM servers by the front end.
 
     Raises:
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/custom_http_headers.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/custom_http_headers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/helpers.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/embedded_connector/helpers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/embedded_connector/request.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/embedded_connector/request.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/environment_variables.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/environment_variables.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/exceptions.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 
 
 class AppError(Exception):
     """A Generic Parent class which inherits the Exception class.
     This class will be inherited by other classes representing specific exceptions.
 
     The Parameterized constructor stores the message, logs and stacktrace.
@@ -13,27 +13,37 @@
 
     def __init__(self, message, logs=None, stacktrace=None):
         self.message = message
         self.logs = logs
         self.stacktrace = stacktrace
 
 
-class InternalError(AppError):
-    """A Class which inherits the AppError class.
-    This class represents any Internal Error within the App
+class FatalError(AppError):
+    """An error which indicates that matlab-proxy web server cannot be brought up.
+    Args:
+        AppError (Class): Parent Class containing attributes to store
+        messages, logs and stacktrace.
+    """
+
+    pass
+
+
+class UIVisibleFatalError(AppError):
+    """A Class with inherits from the AppError class.
+    This class is used to represent Fatal Errors which need to be propagated to the front end.
 
     Args:
         AppError (Class): Parent Class containing attributes to store
         messages, logs and stacktrace.
     """
 
     pass
 
 
-class MatlabInstallError(AppError):
+class MatlabInstallError(UIVisibleFatalError):
     """A Class which inherits the AppError class.
 
     This class represents errors with MATLAB Installation.
 
     Args:
         AppError (Class): Parent Class containing attributes to store
         messages, logs and stacktrace.
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/logger.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/logger.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/token_auth.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/token_auth.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/mwi/validators.py` & `matlab-proxy-0.7.3/matlab_proxy/util/mwi/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,32 +8,28 @@
 Original code: if( input ):
 With validator: if (valid(input)):
 
 Exceptions are thrown to signal failure.
 """
 import errno
 import os
-import socket
-import sys
 from pathlib import Path
-
+import pkg_resources
+import socket
 from typing import List
 
-import pkg_resources
 
 import matlab_proxy
+from matlab_proxy import util
+from matlab_proxy.util import system
 from matlab_proxy.constants import VERSION_INFO_FILE_NAME
 
 from . import environment_variables as mwi_env
-from matlab_proxy.util import system
 from . import logger as mwi_logger
-
-from matlab_proxy import util
-
-from .exceptions import MatlabError
+from .exceptions import MatlabInstallError, FatalError
 
 logger = mwi_logger.get()
 
 
 def validate_mlm_license_file(nlm_connections_str):
     """Validates and returns input if it passes validation.
     Throws exception when validation fails.
@@ -134,18 +130,17 @@
         s.bind(("", int(port)))
         s.close()
 
         # Was able to allocate port. Validation passed.
         return port
     except socket.error as e:
         if e.errno == errno.EADDRINUSE:
-            logger.error(
-                f"The port {port} is not available. Please set another value for the environment variable {mwi_env.get_env_name_app_port()}"
-            )
-            sys.exit(1)
+            error_message = f"The port {port} is not available. Please set another value for the environment variable {mwi_env.get_env_name_app_port()}"
+            logger.error(error_message)
+            raise FatalError(error_message)
         else:
             raise e
 
 
 def validate_base_url(base_url):
     """Validates base_url set in the env variable MWI_BASE_URL.
 
@@ -161,18 +156,17 @@
     """
     validated_base_url = ""
     if base_url == "":
         validated_base_url = ""
 
     else:
         if not base_url.startswith("/"):
-            logger.error(
-                f'The value of environment variable {mwi_env.get_env_name_base_url()} must start with "/" '
-            )
-            sys.exit(1)
+            error_message = f'The value of environment variable {mwi_env.get_env_name_base_url()} must start with "/" '
+            logger.error(error_message)
+            raise FatalError(error_message)
 
         validated_base_url = base_url[:-1] if base_url.endswith("/") else base_url
 
     return validated_base_url
 
 
 def validate_env_config(config):
@@ -194,25 +188,25 @@
         default_config_keys = available_configs[
             matlab_proxy.get_default_config_name()
         ].keys()
         env_config = available_configs[config]
 
         for key in default_config_keys:
             if not key in env_config:
-                logger.error(f"{key} missing in the provided {config} configuration")
-                sys.exit(1)
+                error_message = f"{key} missing in the provided {config} configuration"
+                logger.error(error_message)
+                raise FatalError(error_message)
 
         logger.debug(f"Successfully validated provided {config} configuration")
         return env_config
 
     else:
-        logger.error(
-            f"{config} is not a valid config. Available configs are : {list(available_configs.keys())}"
-        )
-        sys.exit(1)
+        error_message = f"{config} is not a valid config. Available configs are : {list(available_configs.keys())}"
+        logger.error(error_message)
+        raise FatalError(error_message)
 
 
 def __get_configs():
     """Iterates over the 'entry_points' of the installed packages in the current python
     environment and loads the 'matlab_proxy_configs' entry point values into the 'configs' Dict.
 
     Returns:
@@ -231,16 +225,17 @@
 def validate_ssl_cert_file(a_ssl_cert_file):
     """Ensures that its a valid readable file"""
 
     # Empty strings are valid inputs
     if a_ssl_cert_file:
         # String is not empty, check to see if the file exists
         if not os.path.isfile(a_ssl_cert_file):
-            logger.error(f"MWI_SSL_CERT_FILE is not a valid file: {a_ssl_cert_file}")
-            sys.exit(1)
+            error_message = f"MWI_SSL_CERT_FILE is not a valid file: {a_ssl_cert_file}"
+            logger.error(error_message)
+            raise FatalError(error_message)
 
     # string is either empty, or is a valid file on disk
     return a_ssl_cert_file
 
 
 def validate_ssl_key_and_cert_file(a_ssl_key_file, a_ssl_cert_file):
     """Ensures that its a valid readable file"""
@@ -251,26 +246,30 @@
 
     # Implies atleast one value is not None.
 
     # Cert file is either empty or valid file.
     cert_file = validate_ssl_cert_file(a_ssl_cert_file=a_ssl_cert_file)
 
     if cert_file is None and a_ssl_key_file is not None:
-        logger.error(f"MWI_SSL_CERT_FILE must be provided to use the MWI_SSL_KEY_FILE")
-        sys.exit(1)
+        error_message = (
+            f"MWI_SSL_CERT_FILE must be provided to use the MWI_SSL_KEY_FILE"
+        )
+        logger.error(error_message)
+        raise FatalError(error_message)
 
     if a_ssl_key_file is None and cert_file is not None:
         logger.info(
             f"MWI_SSL_KEY_FILE is not provided, ensure that your MWI_SSL_CERT_FILE : '{cert_file}' contains a private key"
         )
 
     if a_ssl_key_file:
         if not os.path.isfile(a_ssl_key_file):
-            logger.error(f"MWI_SSL_KEY_FILE is not a valid file: {a_ssl_key_file}")
-            sys.exit(1)
+            error_message = f"MWI_SSL_KEY_FILE is not a valid file: {a_ssl_key_file}"
+            logger.error(error_message)
+            raise FatalError(error_message)
 
     logger.info(
         f"SSL Keys provided were: MWI_SSL_CERT_FILE: {a_ssl_cert_file} & MWI_SSL_KEY_FILE: {a_ssl_key_file}"
     )
     return a_ssl_key_file, a_ssl_cert_file
 
 
@@ -282,15 +281,15 @@
 
     Returns:
         bool: if use_existing_license is set to true
     """
     return True if use_existing_license.casefold() == "true" else False
 
 
-def validate_paths(paths: List[Path]):
+def __validate_if_paths_exist(paths: List[Path]):
     """Validates if  paths of directories or files exists on the file system.
 
     Args:
         paths ([pathlib.Path]): List of pathlib.Path's to directories or files
 
     Raises:
         OSError: When an invalid path is supplied
@@ -301,34 +300,52 @@
     for path in paths:
         if not util.is_valid_path(path):
             raise OSError(f"Supplied invalid path:{path}")
 
     return paths
 
 
-def validate_custom_matlab_root_path(matlab_root: Path):
+def terminate_on_invalid_matlab_root_path(
+    matlab_root: Path, is_custom_matlab_root: bool
+):
     """Validate if path supplied is MATLAB_ROOT by checking for the existence of VersionInfo.xml file
     at matlab_root
 
     Args:
         path (pathlib.Path): path to MATLAB root
 
     Returns:
         pathlib.Path | None: pathlib.Path if a valid path to MATLAB root is supplied else None
+
+    Raises:
+        MatlabInstallError
     """
+    error_string = f"""Unable to find MATLAB at: {matlab_root}"""
+
+    if is_custom_matlab_root:
+        error_string += f"""\nEdit the environment variable {mwi_env.get_env_name_custom_matlab_root()} to the correct path, and restart matlab-proxy."""
+    else:
+        error_string += f"\nUpdate your system PATH, and restart matlab-proxy."
+
+    #  Check your system PATH, or the value in environment variable {mwi_env.get_env_name_custom_matlab_root()}.
+    #  Restart matlab-proxy after fixing the issue, to continue."""
     try:
         matlab_root = matlab_root
-        validate_paths([matlab_root])
-        logger.debug(f"Supplied valid MATLAB root path:{matlab_root}")
+        __validate_if_paths_exist([matlab_root])
+        logger.debug(
+            f"Specified MATLAB root path:{matlab_root} exists, continuing to verify its validity..."
+        )
     except OSError as exc:
         logger.error(". ".join(exc.args))
-        sys.exit(1)
+        raise MatlabInstallError(error_string)
 
     version_info_file_path = matlab_root / VERSION_INFO_FILE_NAME
 
     if not version_info_file_path.is_file():
-        logger.error(
-            f" {VERSION_INFO_FILE_NAME} file doesn't exist at the provided path :{matlab_root}"
+        log_error_string = (
+            error_string
+            + f"Failed to locate {VERSION_INFO_FILE_NAME} at this location."
         )
-        sys.exit(1)
+        logger.error(log_error_string)
+        raise MatlabInstallError(error_string)
 
     return matlab_root
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/system.py` & `matlab-proxy-0.7.3/matlab_proxy/util/system.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy/util/windows.py` & `matlab-proxy-0.7.3/matlab_proxy/util/windows.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.7.2/matlab_proxy.egg-info/PKG-INFO` & `matlab-proxy-0.7.3/matlab_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
```

### Comparing `matlab-proxy-0.7.2/matlab_proxy.egg-info/SOURCES.txt` & `matlab-proxy-0.7.3/matlab_proxy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 gui/src/components/Controls/help.svg
 gui/src/components/Controls/index.js
 gui/src/components/Controls/restart.svg
 gui/src/components/Controls/sign-out.svg
 gui/src/components/Controls/start.svg
 gui/src/components/Controls/stop.svg
 gui/src/components/Controls/terminate.svg
+gui/src/components/EntitlementSelector/EntitlementSelector.spec.js
+gui/src/components/EntitlementSelector/index.js
 gui/src/components/Error/Error.css
 gui/src/components/Error/Error.spec.js
 gui/src/components/Error/index.js
 gui/src/components/Help/Help.css
 gui/src/components/Help/Help.spec.js
 gui/src/components/Help/index.js
 gui/src/components/Information/Information.css
```

### Comparing `matlab-proxy-0.7.2/setup.py` & `matlab-proxy-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The MathWorks, Inc.
+# Copyright (c) 2020-2023 The MathWorks, Inc.
 import os
 from pathlib import Path
 from shutil import which
 
 import setuptools
 from setuptools.command.install import install
 
@@ -61,15 +61,15 @@
 INSTALL_REQUIRES = ["aiohttp>=3.7.4", "psutil", "aiohttp_session[secure]"]
 
 HERE = Path(__file__).parent.resolve()
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="matlab-proxy",
-    version="0.7.2",
+    version="0.7.3",
     url=config["doc_url"],
     author="The MathWorks, Inc.",
     author_email="cloud@mathworks.com",
     license="MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE",
     description="Python® package enables you to launch MATLAB® and access it from a web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

