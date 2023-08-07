# Comparing `tmp/buckaroo-0.3.6.tar.gz` & `tmp/buckaroo-0.3.7.tar.gz`

## Comparing `buckaroo-0.3.6.tar` & `buckaroo-0.3.7.tar`

### file list

```diff
@@ -1,104 +1,110 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.6/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.6/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.6/Untitled.ipynb
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.6/babel.config.js
--rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.6/bike-share-data-explore.ipynb
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo.json
--rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.6/col-ordering.ipynb
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 buckaroo-0.3.6/full_build.sh
--rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.6/gbfs-play.ipynb
--rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.6/gbfs-play2.ipynb
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.6/introduction.ipynb
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.6/notes.txt
--rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.6/package-lock.json
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.6/package.json
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.6/package.json.old
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.6/setup.py
--rw-r--r--   0        0        0    45329 2020-02-02 00:00:00.000000 buckaroo-0.3.6/stock-returns.ipynb
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.6/tryit.ipynb
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.6/tsconfig.json
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.6/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.6/webpack.lab.config.js
--rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.6/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.6/.yarn/cache/.gitignore
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/_version.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/all_transforms.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/buckaroo_widget.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/channeldata.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/configure_utils.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/lispy.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/summary_stats.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/views.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/package.json
--rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
--rw-r--r--   0        0        0    35955 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/399.50690b06cf528166a430.js
--rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/41.dea207301743f71053c5.js
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js
--rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
--rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
--rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/remoteEntry.e0e4ad417ed29f6a520a.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/style.js
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0  1691829 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/nbextension/index.js.map
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.6/buckaroo/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/make.bat
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/FAQ.rst
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/conf.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/contributing.rst
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/index.rst
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/install.rst
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/using.rst
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.6/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.6/example-notebooks/testcases-fast.ipynb
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/comp1.tsx
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/index.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/plugin.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/version.ts
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/ColumnsEditor.tsx
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/CommandUtils.ts
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/DCFCell.tsx
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/DFViewer.tsx
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/DependentTabs.tsx
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/OperationDetail.tsx
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/OperationUtils.ts
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/Operations.tsx
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/StatusBar.tsx
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/bakedOperationDefaults.ts
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/gridUtils.ts
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/staticData.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/components/utils.ts
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/dcf-npm.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.6/js/style/icons/filter.svg
--rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.6/static/images/Buckaroo-screenshot.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.6/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 buckaroo-0.3.6/README.md
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 buckaroo-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.7/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.7/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.7/Untitled.ipynb
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.7/babel.config.js
+-rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.7/bike-share-data-explore.ipynb
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo.json
+-rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.7/col-ordering.ipynb
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 buckaroo-0.3.7/full_build.sh
+-rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.7/gbfs-play.ipynb
+-rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.7/gbfs-play2.ipynb
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.7/introduction.ipynb
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.7/notes.txt
+-rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.7/package-lock.json
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.7/package.json
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.7/package.json.old
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.7/setup.py
+-rw-r--r--   0        0        0    45329 2020-02-02 00:00:00.000000 buckaroo-0.3.7/stock-returns.ipynb
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.7/tryit.ipynb
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.7/tsconfig.json
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.7/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.7/webpack.lab.config.js
+-rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.7/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.7/.yarn/cache/.gitignore
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/_version.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/all_transforms.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/configure_utils.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/lispy.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/views.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
+-rw-r--r--   0        0        0    35562 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/399.268551e45b21a7199251.js
+-rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/41.dea207301743f71053c5.js
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/480.889b78dbe4b4e9d7c19c.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
+-rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
+-rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/remoteEntry.5f509df8faa7459a6959.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0  1691829 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/nbextension/index.js.map
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.7/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/.#FAQ.rst -> paddy@Paddys-MacBook-Air.local.405
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/.#conf.py -> paddy@Paddys-MacBook-Air.local.405
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/conf.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/feature_reference.rst
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/index.rst
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/install.rst
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/using.rst
+-rw-r--r--   0        0        0   835431 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/_static/Buckaroo-labled.png
+-rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/_static/Statusbar.png
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/_static/embed-bundle.js.LICENSE.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.7/docs/source/articles/.#jupyter-table-widget-comparison.rst -> paddy@Paddys-MacBook-Air.local.405
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.7/example-notebooks/testcases-fast.ipynb
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/comp1.tsx
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/version.ts
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/ColumnsEditor.tsx
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/CommandUtils.ts
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/DCFCell.tsx
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/DFViewer.tsx
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/DependentTabs.tsx
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/OperationDetail.tsx
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/OperationUtils.ts
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/Operations.tsx
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/StatusBar.tsx
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/bakedOperationDefaults.ts
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/gridUtils.ts
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/staticData.ts
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/components/utils.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/dcf-npm.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.7/js/style/icons/filter.svg
+-rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.7/static/images/Buckaroo-screenshot.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 buckaroo-0.3.7/README.md
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 buckaroo-0.3.7/PKG-INFO
```

### Comparing `buckaroo-0.3.6/RELEASE.md` & `buckaroo-0.3.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/bike-share-data-explore.ipynb` & `buckaroo-0.3.7/bike-share-data-explore.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/col-ordering.ipynb` & `buckaroo-0.3.7/col-ordering.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/gbfs-play.ipynb` & `buckaroo-0.3.7/gbfs-play.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/gbfs-play2.ipynb` & `buckaroo-0.3.7/gbfs-play2.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/introduction.ipynb` & `buckaroo-0.3.7/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/package-lock.json` & `buckaroo-0.3.7/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999958193979933%*

 * *Differences: {"'packages'": "{'': {'version': '0.2.2'}}", "'version'": "'0.2.2'"}*

```diff
@@ -66,15 +66,15 @@
                 "url-loader": "^4.1.0",
                 "webpack": "^5",
                 "webpack-cli": "^4.5.0",
                 "webpack-dev-server": "^4.0.0"
             },
             "license": "BSD-3-Clause",
             "name": "buckaroo",
-            "version": "0.2.1"
+            "version": "0.2.2"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
@@ -16159,9 +16159,9 @@
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "license": "MIT",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `buckaroo-0.3.6/package.json` & `buckaroo-0.3.7/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -166,9 +166,9 @@
         "test": "jest --verbose --passWithNoTests",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `buckaroo-0.3.6/package.json.old` & `buckaroo-0.3.7/package.json.old`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/stock-returns.ipynb` & `buckaroo-0.3.7/stock-returns.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/tryit.ipynb` & `buckaroo-0.3.7/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/tsconfig.json` & `buckaroo-0.3.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/webpack.config.js` & `buckaroo-0.3.7/webpack.config.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/yarn.lock` & `buckaroo-0.3.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/__init__.py` & `buckaroo-0.3.7/buckaroo/__init__.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/all_transforms.py` & `buckaroo-0.3.7/buckaroo/all_transforms.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/buckaroo_widget.py` & `buckaroo-0.3.7/buckaroo/buckaroo_widget.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/configure_utils.py` & `buckaroo-0.3.7/buckaroo/configure_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/dcf_transform.py` & `buckaroo-0.3.7/buckaroo/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/df_methods.py` & `buckaroo-0.3.7/buckaroo/df_methods.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/index.html` & `buckaroo-0.3.7/buckaroo/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/lispy.py` & `buckaroo-0.3.7/buckaroo/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/summary_stats.py` & `buckaroo-0.3.7/buckaroo/summary_stats.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/views.py` & `buckaroo-0.3.7/buckaroo/views.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/package.json` & `buckaroo-0.3.7/buckaroo/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96796875%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5f509df8faa7459a6959.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -81,15 +81,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/paddymul/buckaroo",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e0e4ad417ed29f6a520a.js"
+            "load": "static/remoteEntry.5f509df8faa7459a6959.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./buckaroo/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -170,9 +170,9 @@
         "test": "jest --verbose --passWithNoTests",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js` & `buckaroo-0.3.7/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt` & `buckaroo-0.3.7/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/399.50690b06cf528166a430.js` & `buckaroo-0.3.7/buckaroo/labextension/static/399.268551e45b21a7199251.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -49,24 +49,24 @@
             }) {
                 const u = e.schema.fields.map((e => e.name));
                 return l.default.createElement("div", {
                     className: "columns-editor",
                     style: {
                         width: "100%"
                     }
-                }, i.showCommands ? l.default.createElement(s.OperationViewer, {
+                }, i.showCommands ? l.default.createElement("div", null, l.default.createElement(s.OperationViewer, {
                     operations: n,
                     setOperations: a,
                     activeColumn: t,
                     allColumns: u,
                     commandConfig: o
-                }) : l.default.createElement("span", null), i.showTransformed ? l.default.createElement(d.DependentTabs, {
+                }), l.default.createElement(d.DependentTabs, {
                     filledOperations: n,
                     operationResult: r
-                }) : l.default.createElement("span", null))
+                })) : l.default.createElement("span", null))
             }
             t.ColumnsEditor = c, t.ColumnsEditorEx = function() {
                 const [e, t] = (0, l.useState)(i.bakedOperations), n = {
                     transformed_df: i.EmptyDf,
                     generated_py_code: "default py code",
                     transform_error: void 0
                 };
@@ -74,16 +74,15 @@
                     df: u.tableDf,
                     activeColumn: "foo",
                     commandConfig: u.bakedCommandConfig,
                     operations: e,
                     setOperations: t,
                     operationResult: n,
                     widgetConfig: {
-                        showCommands: !0,
-                        showTransformed: !0
+                        showCommands: !0
                     }
                 })
             }
         },
         3537: (e, t) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
@@ -147,16 +146,15 @@
                 operation_results: a,
                 commandConfig: r,
                 dfConfig: o,
                 on_dfConfig: i,
                 summaryDf: d
             }) {
                 const [m, f] = (0, l.useState)("stoptime"), p = {
-                    showCommands: o.showCommands,
-                    showTransformed: o.showTransformed
+                    showCommands: o.showCommands
                 }, b = Object.assign(Object.assign({}, o), {
                     rowsShown: e.data.length || 0
                 });
                 return l.default.createElement("div", {
                     className: "dcf-root flex flex-col",
                     style: {
                         width: "100%",
@@ -171,15 +169,15 @@
                 }, l.default.createElement(c.StatusBar, {
                     config: b,
                     setConfig: i
                 }), l.default.createElement(u.DFViewer, {
                     df: o.summaryStats ? d : e,
                     activeCol: m,
                     setActiveCol: f
-                })), p.showCommands || p.showTransformed ? l.default.createElement(s.ColumnsEditor, {
+                })), p.showCommands ? l.default.createElement(s.ColumnsEditor, {
                     df: e,
                     activeColumn: m,
                     operations: t,
                     setOperations: n,
                     operationResult: a,
                     commandConfig: r,
                     widgetConfig: p
@@ -189,16 +187,14 @@
                 const [e, t] = (0, l.useState)({
                     totalRows: 1309,
                     columns: 30,
                     rowsShown: 500,
                     sampleSize: 1e4,
                     sampled: !0,
                     summaryStats: !1,
-                    reorderdColumns: !1,
-                    showTransformed: !0,
                     showCommands: !0
                 }), [n, a] = (0, l.useState)(f.bakedOperations);
                 return l.default.createElement(p, {
                     origDf: d.tableDf,
                     operations: n,
                     on_operations: a,
                     operation_results: i.baseOperationResults,
@@ -846,34 +842,36 @@
                 s = n(214),
                 d = [{
                     field: "summaryStats",
                     headerName: "Σ",
                     headerTooltip: "Summary Stats",
                     width: 30
                 }, {
-                    field: "reorderdColumns",
-                    headerName: "Θ",
-                    headerTooltip: "Reorder Columns",
-                    width: 30
-                }, {
-                    field: "showTransformed",
-                    headerName: "Δ",
-                    headerTooltip: "Show Transformation",
-                    width: 30
-                }, {
                     field: "showCommands",
                     headerName: "λ",
                     headerTooltip: "Show Commands",
                     width: 30
                 }, {
                     field: "sampled",
                     headerName: "Ξ",
                     headerTooltip: "Sampled",
                     width: 30
                 }, {
+                    field: "help",
+                    headerName: "?",
+                    headerTooltip: "Help",
+                    width: 30,
+                    cellRenderer: function(e) {
+                        return l.default.createElement("a", {
+                            href: "https://buckaroo-data.readthedocs.io/en/latest/feature_reference.html",
+                            target: "_blank",
+                            rel: "noopener"
+                        }, "?")
+                    }
+                }, {
                     field: "totalRows",
                     width: 100
                 }, {
                     field: "columns",
                     width: 100
                 }, {
                     field: "rowsShown",
@@ -890,74 +888,64 @@
                 const {
                     totalRows: n,
                     columns: a,
                     rowsShown: r,
                     sampleSize: o,
                     sampled: u,
                     summaryStats: c,
-                    reorderdColumns: m,
-                    showTransformed: f,
-                    showCommands: p
-                } = e, b = [{
+                    showCommands: m
+                } = e, f = [{
                     totalRows: s.intFormatter.format(n),
                     columns: a,
                     rowsShown: s.intFormatter.format(r),
                     sampleSize: s.intFormatter.format(o),
-                    sampled: u ? "Ϋ" : "ό",
-                    summaryStats: c ? "Ϋ" : "ό",
-                    reorderdColumns: m ? "Ϋ" : "ό",
-                    showTransformed: f ? "Ϋ" : "ό",
-                    showCommands: p ? "Ϋ" : "ό"
-                }], g = (0, l.useRef)(null);
+                    sampled: u ? "1" : "0",
+                    summaryStats: c ? "1" : "0",
+                    showCommands: m ? "1" : "0"
+                }], p = (0, l.useRef)(null);
                 return l.default.createElement("div", {
                     className: "statusBar"
                 }, l.default.createElement("div", {
                     style: {
                         height: 50
                     },
                     className: "theme-hanger ag-theme-alpine-dark"
                 }, l.default.createElement(i.AgGridReact, {
-                    ref: g,
+                    ref: p,
                     onCellClicked: n => {
                         const a = n.column.getColId();
                         "summaryStats" === a ? t(Object.assign(Object.assign({}, e), {
                             summaryStats: !e.summaryStats
                         })) : "sampled" === a ? t(Object.assign(Object.assign({}, e), {
                             sampled: !e.sampled
-                        })) : "reorderdColumns" === a ? t(Object.assign(Object.assign({}, e), {
-                            reorderdColumns: !e.reorderdColumns
-                        })) : "showTransformed" === a ? t(Object.assign(Object.assign({}, e), {
-                            showTransformed: !e.showTransformed
                         })) : "showCommands" === a && t(Object.assign(Object.assign({}, e), {
                             showCommands: !e.showCommands
                         }))
                     },
                     gridOptions: {
                         rowSelection: "single"
                     },
                     defaultColDef: {
                         type: "left-aligned",
                         cellStyle: {
                             textAlign: "left"
                         }
                     },
-                    rowData: b,
+                    rowData: f,
                     columnDefs: d
                 })))
             }
             t.StatusBar = u, t.StatusBarEx = function() {
                 const [e, t] = (0, l.useState)({
                     totalRows: 1309,
                     columns: 30,
                     rowsShown: 500,
                     sampleSize: 1e4,
                     sampled: !0,
                     summaryStats: !1,
-                    reorderdColumns: !0,
-                    showTransformed: !0,
                     showCommands: !0
                 });
                 return l.default.createElement(u, {
                     config: e,
                     setConfig: t
                 })
             }
@@ -1413,11 +1401,11 @@
             r()(o.Z, {
                 insert: "head",
                 singleton: !1
             });
             const l = o.Z.locals || {}
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"buckaroo","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^29.2.0","ag-grid-react":"^29.2.0","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prismjs":"^1.28.0","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-preset-env":"^7.7.2","postcss-nested":"^6.0.0","sass":"^1.53.0","sass-loader":"^13.0.2","react-router":"^6.3.0","react-router-dom":"^5.2.0","rimraf":"^3.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"buckaroo","version":"0.2.2","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^29.2.0","ag-grid-react":"^29.2.0","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prismjs":"^1.28.0","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-preset-env":"^7.7.2","postcss-nested":"^6.0.0","sass":"^1.53.0","sass-loader":"^13.0.2","react-router":"^6.3.0","react-router-dom":"^5.2.0","rimraf":"^3.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/41.dea207301743f71053c5.js` & `buckaroo-0.3.7/buckaroo/labextension/static/41.dea207301743f71053c5.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js` & `buckaroo-0.3.7/buckaroo/labextension/static/480.889b78dbe4b4e9d7c19c.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
                         for (var r in e) "default" !== r && Object.prototype.hasOwnProperty.call(e, r) && n(t, e, r);
                     return i(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             });
             const u = r(2492),
-                a = r(9764),
+                a = r(6303),
                 c = r(8657),
                 s = o(r(8399)),
                 l = {
                     id: "buckaroo:plugin",
                     requires: [u.IJupyterWidgetRegistry],
                     optional: [a.IThemeManager],
                     activate: function(e, t, r) {
```

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js` & `buckaroo-0.3.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js` & `buckaroo-0.3.7/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js` & `buckaroo-0.3.7/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js` & `buckaroo-0.3.7/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt` & `buckaroo-0.3.7/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/remoteEntry.e0e4ad417ed29f6a520a.js` & `buckaroo-0.3.7/buckaroo/labextension/static/remoteEntry.5f509df8faa7459a6959.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, u, l, d, f, c, s, p, h, v, b, g, m, y, w, k = {
+    var e, r, t, a, o, n, i, d, u, l, f, c, s, p, h, v, b, g, m, y, w, k = {
             5941: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(935), t.e(41), t.e(399), t.e(568)]).then((() => () => t(1568))),
                         "./extension": () => Promise.all([t.e(935), t.e(41), t.e(399), t.e(480)]).then((() => () => t(4480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -45,26 +45,26 @@
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         0: "c008020c7e2133e6c7db",
         41: "dea207301743f71053c5",
-        399: "50690b06cf528166a430",
-        480: "c541de2b54a15c8f7330",
+        399: "268551e45b21a7199251",
+        480: "889b78dbe4b4e9d7c19c",
         486: "f08778dfb765d893ceaf",
         497: "a76de7c665cc86a1c49a",
         568: "50d29d049ddb62602cc0",
         731: "d4bf968c7a94633ef5a3",
         935: "2832d17fef97c1ec6694"
     } [e] + ".js?v=" + {
         0: "c008020c7e2133e6c7db",
         41: "dea207301743f71053c5",
-        399: "50690b06cf528166a430",
-        480: "c541de2b54a15c8f7330",
+        399: "268551e45b21a7199251",
+        480: "889b78dbe4b4e9d7c19c",
         486: "f08778dfb765d893ceaf",
         497: "a76de7c665cc86a1c49a",
         568: "50d29d049ddb62602cc0",
         731: "d4bf968c7a94633ef5a3",
         935: "2832d17fef97c1ec6694"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
@@ -72,34 +72,34 @@
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "buckaroo:", P.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
-            var i, u;
+            var i, d;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var f = l[d];
+                for (var u = document.getElementsByTagName("script"), l = 0; l < u.length; l++) {
+                    var f = u[l];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
+            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
             var c = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), d && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -111,25 +111,25 @@
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 P.o(P.S, t) || (P.S[t] = {});
                 var n = P.S[t],
                     i = "buckaroo",
-                    u = (e, r, t, a) => {
+                    d = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            u = o[r];
-                        (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (o[r] = {
+                            d = o[r];
+                        (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    l = [];
-                return "default" === t && (u("ag-grid-community", "29.3.5", (() => P.e(731).then((() => () => P(1731))))), u("ag-grid-react", "29.3.5", (() => Promise.all([P.e(935), P.e(0), P.e(497)]).then((() => () => P(4e3))))), u("buckaroo", "0.2.1", (() => Promise.all([P.e(935), P.e(41), P.e(399), P.e(568)]).then((() => () => P(1568))))), u("lodash", "4.17.21", (() => P.e(486).then((() => () => P(6486)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    u = [];
+                return "default" === t && (d("ag-grid-community", "29.3.5", (() => P.e(731).then((() => () => P(1731))))), d("ag-grid-react", "29.3.5", (() => Promise.all([P.e(935), P.e(0), P.e(497)]).then((() => () => P(4e3))))), d("buckaroo", "0.2.2", (() => Promise.all([P.e(935), P.e(41), P.e(399), P.e(568)]).then((() => () => P(1568))))), d("lodash", "4.17.21", (() => P.e(486).then((() => () => P(6486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -148,110 +148,110 @@
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var o = e[a],
                 n = (typeof o)[0];
             if (a >= r.length) return "u" == n;
             var i = r[a],
-                u = (typeof i)[0];
-            if (n != u) return "o" == n && "n" == u || "s" == u || "u" == n;
+                d = (typeof i)[0];
+            if (n != d) return "o" == n && "n" == d || "s" == d || "u" == n;
             if ("o" != n && "u" != n && o != i) return o < i;
             a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(u = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, u);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(d = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
             return t
         }
         var i = [];
         for (n = 1; n < e.length; n++) {
-            var u = e[n];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            var d = e[n];
+            i.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? i.pop() + " " + i.pop() : o(d))
         }
-        return l();
+        return u();
 
-        function l() {
+        function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, f, c = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !l || ("u" == c ? u > a && !o : "" == c != o);
+            for (var i = 0, d = 1, u = !0;; d++, i++) {
+                var l, f, c = d < e.length ? (typeof e[d])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !u || ("u" == c ? d > a && !o : "" == c != o);
                 if ("u" == f) {
-                    if (!l || "u" != c) return !1
-                } else if (l)
+                    if (!u || "u" != c) return !1
+                } else if (u)
                     if (c == f)
-                        if (u <= a) {
-                            if (d != e[u]) return !1
+                        if (d <= a) {
+                            if (l != e[d]) return !1
                         } else {
-                            if (o ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (o ? l > e[d] : l < e[d]) return !1;
+                            l != e[d] && (u = !1)
                         }
                 else if ("s" != c && "n" != c) {
-                    if (o || u <= a) return !1;
-                    l = !1, u--
+                    if (o || d <= a) return !1;
+                    u = !1, d--
                 } else {
-                    if (u <= a || f < c != o) return !1;
-                    l = !1
-                } else "s" != c && "n" != c && (l = !1, u--)
+                    if (d <= a || f < c != o) return !1;
+                    u = !1
+                } else "s" != c && "n" != c && (u = !1, d--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, u = (e, r) => {
+    }, d = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
-    }, l = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", f = (e, r, t, a) => {
-        var o = l(e, t);
-        return n(a, o) || s(d(e, t, o, a)), p(e[t][o])
+    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", f = (e, r, t, a) => {
+        var o = u(e, t);
+        return n(a, o) || s(l(e, t, o, a)), p(e[t][o])
     }, c = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, o) {
         var n = P.I(r);
         return n && n.then ? n.then(e.bind(e, r, P.S[r], t, a, o)) : e(r, P.S[r], t, a, o)
-    })(((e, r, t, a) => r && P.o(r, t) ? p(u(r, t)) : a())), b = h(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), g = h(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && P.o(r, t) ? p(d(r, t)) : a())), b = h(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), g = h(((e, r, t, a, o) => {
         var n = r && P.o(r, t) && c(r, t, a);
         return n ? p(n) : o()
     })), m = {}, y = {
         1048: () => v("default", "ag-grid-react", (() => Promise.all([P.e(0), P.e(497)]).then((() => () => P(4e3))))),
         2492: () => b("default", "@jupyter-widgets/base", [, [1, 6, 0, 0],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1
         ]),
         4439: () => g("default", "lodash", [1, 4, 17, 21], (() => P.e(486).then((() => () => P(6486))))),
-        9764: () => b("default", "@jupyterlab/apputils", [1, 3, 6, 4]),
+        6303: () => b("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
         8497: () => g("default", "ag-grid-community", [2, 29, 3, 5], (() => P.e(731).then((() => () => P(1731)))))
     }, w = {
         399: [1048, 2492, 4439],
-        480: [9764],
+        480: [6303],
         497: [8497]
     }, P.f.consumes = (e, r) => {
         P.o(w, e) && w[e].forEach((e => {
             if (P.o(m, e)) return r.push(m[e]);
             var t = r => {
                     m[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
@@ -288,21 +288,21 @@
                             n = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var a, o, [n, i, u] = t,
-                    l = 0;
+                var a, o, [n, i, d] = t,
+                    u = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) P.o(i, a) && (P.m[a] = i[a]);
-                    u && u(P)
+                    d && d(P)
                 }
-                for (r && r(t); l < n.length; l++) o = n[l], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < n.length; u++) o = n[u], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var E = P(5941);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).buckaroo = E
 })();
```

### Comparing `buckaroo-0.3.6/buckaroo/labextension/static/third-party-licenses.json` & `buckaroo-0.3.7/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/nbextension/index.js` & `buckaroo-0.3.7/buckaroo/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/nbextension/index.js.LICENSE.txt` & `buckaroo-0.3.7/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/nbextension/index.js.map` & `buckaroo-0.3.7/buckaroo/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/buckaroo/noarch/index.html` & `buckaroo-0.3.7/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/docs/Makefile` & `buckaroo-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/docs/make.bat` & `buckaroo-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/docs/source/FAQ.rst` & `buckaroo-0.3.7/docs/source/FAQ.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 .. Buckaroo documentation master file, created by
    sphinx-quickstart on Wed Apr 19 14:07:15 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Buckaroo - FAQ
 ==========================================
+
+* **Does Buckaroo work in Visual Studio Code**
+
+  As of 0.3.6 Buckaroo works properly in Visual Studio Code.  You must install the `Visual Studio Code Jupyter Extension <https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter>`_ and the `Jupyter Renderer extension <https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter-renderers>`_.  Then install buckaroo from pip and everything should work.
+
 *  **Are there any similar projects to Buckaroo?**
 
 There are a couple of projects like Buckaroo that aim to provide a better table widget and pandas editing experience.
 
 #. `Mito <https://github.com/mito-ds/monorepo>`_.  Source Available table/code editing widget for Jupyter.  More aimed at easing transition to pandas from excel users.  GNU Affero licensed
 #. `Microsoft DataWrangler <https://github.com/microsoft/vscode-data-wrangler>`_ .  Closed source, provides a very similar experience inside of VSCode's notebook experience.  Only works inside of VSCode by the `VS Marketplace Terms of Use <https://cdn.vsassets.io/v/M190_20210811.1/_content/Microsoft-Visual-Studio-Marketplace-Terms-of-Use.pdf>`_
 #. `IpyDatagrid <https://github.com/bloomberg/ipydatagrid>`_.  Open source.  Bloomberg's Jupyter table widget. I used the ipydatagrid repo structure as the basis for buckaroo (js build setup only)
```

### Comparing `buckaroo-0.3.6/docs/source/conf.py` & `buckaroo-0.3.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/docs/source/contributing.rst` & `buckaroo-0.3.7/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/docs/source/index.rst` & `buckaroo-0.3.7/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
    This project is under active development.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    using
+   feature_reference
    install
    contributing
    FAQ
 
 Indices and tables
 ==================
```

### Comparing `buckaroo-0.3.6/docs/source/using.rst` & `buckaroo-0.3.7/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.3.7/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/example-notebooks/testcases-fast.ipynb` & `buckaroo-0.3.7/example-notebooks/testcases-fast.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/dcefwidget.ts` & `buckaroo-0.3.7/js/dcefwidget.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/extension.ts` & `buckaroo-0.3.7/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/plugin.ts` & `buckaroo-0.3.7/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/ColumnsEditor.tsx` & `buckaroo-0.3.7/js/components/ColumnsEditor.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 //import {bakedCommandConfig} from './bakedOperationDefaults';
 import { DependentTabs, OperationResult } from './DependentTabs';
 import { tableDf, bakedCommandConfig } from './staticData'
 
 export type OperationSetter = (ops: Operation[]) => void;
 export interface WidgetConfig {
   showCommands:boolean;
-  showTransformed:boolean;
+//  showTransformed:boolean;
 }
 
 
 export function ColumnsEditor({
   df,
   activeColumn,
   operations,
@@ -32,26 +32,26 @@
   widgetConfig:WidgetConfig
 }) {
   const allColumns = df.schema.fields.map((field) => field.name);
   //console.log('Columns Editor, commandConfig', commandConfig);
   return (
     <div className="columns-editor" style={{ width: '100%' }}>
       {(widgetConfig.showCommands) ? (
+	<div>
       <OperationViewer
         operations={operations}
         setOperations={setOperations}
         activeColumn={activeColumn}
         allColumns={allColumns}
-        commandConfig={commandConfig}
-	  />) : <span></span>}
-    {(widgetConfig.showTransformed) ?(
+        commandConfig={commandConfig}/>
       <DependentTabs
         filledOperations={operations}
         operationResult={operationResult}
 	/>
+    </div>
     ) : <span></span>}
     </div>
   );
 }
 
 export function ColumnsEditorEx() {
   const [operations, setOperations] = useState(bakedOperations);
@@ -66,11 +66,11 @@
     <ColumnsEditor
       df={tableDf}
       activeColumn={'foo'}
       commandConfig={bakedCommandConfig}
       operations={operations}
       setOperations={setOperations}
     operationResult={baseOperationResults}
-    widgetConfig={{showCommands:true, showTransformed:true}}
+    widgetConfig={{showCommands:true}}
     />
   );
 }
```

### Comparing `buckaroo-0.3.6/js/components/CommandUtils.ts` & `buckaroo-0.3.7/js/components/CommandUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/DCFCell.tsx` & `buckaroo-0.3.7/js/components/DCFCell.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   operation_results: OperationResult;
   commandConfig: CommandConfigT;
   dfConfig: DfConfig;
   on_dfConfig: unknown;
   summaryDf: DFWhole
 }) {
   const [activeCol, setActiveCol] = useState('stoptime');
-  const widgetConfig: WidgetConfig = {showCommands:dfConfig.showCommands, showTransformed:dfConfig.showTransformed}
+  const widgetConfig: WidgetConfig = {showCommands:dfConfig.showCommands}
   const localDfConfig = {...dfConfig, 'rowsShown': origDf.data.length || 0}
   return (
     <div
       className="dcf-root flex flex-col"
       style={{ width: '100%', height: '100%' }}
     >
       <div
@@ -51,15 +51,15 @@
         <StatusBar config={localDfConfig} setConfig={on_dfConfig} />
         <DFViewer
           df={(dfConfig.summaryStats ? summaryDf : origDf) }
           activeCol={activeCol}
           setActiveCol={setActiveCol}
         />
       </div>
-    {(widgetConfig.showCommands || widgetConfig.showTransformed) ? (
+    {(widgetConfig.showCommands) ? (
       <ColumnsEditor
         df={origDf}
         activeColumn={activeCol}
         operations={operations}
         setOperations={on_operations}
         operationResult={operation_results}
         commandConfig={commandConfig}
@@ -73,17 +73,16 @@
   const [sampleConfig, setConfig] = useState<DfConfig>({
     totalRows: 1309,
     columns: 30,
     rowsShown: 500,
     sampleSize: 10_000,
     sampled: true,
     summaryStats: false,
-    reorderdColumns: false,
-    showTransformed: true,
-    showCommands: true
+    showCommands: true,
+    //reorderdColumns: false,
   });
   const [operations, setOperations] = useState<Operation[]>(bakedOperations);
   return (
     <WidgetDCFCell
       origDf={tableDf}
       operations={operations}
       on_operations={setOperations}
```

### Comparing `buckaroo-0.3.6/js/components/DFViewer.tsx` & `buckaroo-0.3.7/js/components/DFViewer.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/DependentTabs.tsx` & `buckaroo-0.3.7/js/components/DependentTabs.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/OperationDetail.tsx` & `buckaroo-0.3.7/js/components/OperationDetail.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/OperationUtils.ts` & `buckaroo-0.3.7/js/components/OperationUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/Operations.tsx` & `buckaroo-0.3.7/js/components/Operations.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/StatusBar.tsx` & `buckaroo-0.3.7/js/components/StatusBar.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -14,93 +14,93 @@
 export interface DfConfig {
   totalRows: number;
   columns: number;
   rowsShown: number;
   sampleSize: number;
   sampled: boolean;
   summaryStats: boolean;
-  reorderdColumns: boolean;
   showCommands:boolean;
-  showTransformed:boolean;
+  //reorderdColumns: boolean;
 }
 
+
 const columnDefs: ColDef[] = [
   { field: 'summaryStats',
     headerName:'Σ',
     headerTooltip:'Summary Stats',
     width:30
   },
-  { field: 'reorderdColumns',
-  headerName: "Θ",
-  headerTooltip:"Reorder Columns",
-  width:30
-},
-  { field: 'showTransformed',
-  headerName:"Δ",
-  headerTooltip:"Show Transformation",
-  width:30
-},
+//   { field: 'reorderdColumns',
+//   headerName: "Θ",
+//   headerTooltip:"Reorder Columns",
+//   width:30
+// },
   { field: 'showCommands',
   headerName: "λ",
   headerTooltip:"Show Commands",
   width:30
 },
 
   { field: 'sampled',
   headerName: "Ξ",
   headerTooltip:"Sampled",
   width:30
 },
+  { field: 'help',
+  headerName: "?",
+  headerTooltip:"Help",
+    width:30,
+    cellRenderer: function(params:any) {
+      return <a href="https://buckaroo-data.readthedocs.io/en/latest/feature_reference.html" target="_blank" rel="noopener">?</a>}
+},
+
   { field: 'totalRows', width:100},
   { field: 'columns', width:100 },
   { field: 'rowsShown', width:120},
   { field: 'sampleSize', width:120 }
 ];
 
 export function StatusBar({ config, setConfig }: { config:any, setConfig:any }) {
   const {
     totalRows,
     columns,
     rowsShown,
     sampleSize,
     sampled,
     summaryStats,
-    reorderdColumns,
-    showTransformed,
-    showCommands
+    showCommands,
+    //reorderdColumns
   } = config;
 
   const rowData = [
     {
       totalRows: intFormatter.format(totalRows),
       columns,
       rowsShown : intFormatter.format(rowsShown),
       sampleSize : intFormatter.format(sampleSize),
-      sampled: sampled  ? "Ϋ" : "ό",
-      summaryStats: summaryStats ? "Ϋ" : "ό",
-      reorderdColumns: reorderdColumns ? "Ϋ" : "ό",
-      showTransformed: showTransformed ? "Ϋ" : "ό",
-      showCommands: showCommands ? "Ϋ" : "ό",
+      sampled: sampled  ? "1" : "0",
+      summaryStats: summaryStats ? "1" : "0",
+      // reorderdColumns: reorderdColumns ? "Ϋ" : "ό",
+      showCommands: showCommands ? "1" : "0"
     },
   ];
 
   const updateDict = (event:any) => {
     const colName = event.column.getColId();
     if (colName === 'summaryStats') {
       setConfig({ ...config, summaryStats: !config.summaryStats });
     }
     else if (colName === 'sampled') {
       setConfig({ ...config, sampled: !config.sampled });
-    } else if (colName === 'reorderdColumns') {
-      setConfig({ ...config, reorderdColumns: !config.reorderdColumns });
-    } else if (colName === 'showTransformed') {
-      setConfig({ ...config, showTransformed: !config.showTransformed });
     } else if (colName === 'showCommands') {
       setConfig({ ...config, showCommands: !config.showCommands });
     }
+    // } else if (colName === 'reorderdColumns') {
+    //   setConfig({ ...config, reorderdColumns: !config.reorderdColumns });
+
   };
   const gridOptions: GridOptions = {
     rowSelection: 'single',
   };
 
   const gridRef = useRef<AgGridReact<unknown>>(null);
   const defaultColDef = {
@@ -127,14 +127,13 @@
   const [sampleConfig, setConfig] = useState<DfConfig>({
     totalRows: 1309,
     columns: 30,
     rowsShown: 500,
     sampleSize: 10_000,
     sampled: true,
     summaryStats: false,
-    reorderdColumns: true,
-    showTransformed: true,
     showCommands: true,
+    //reorderdColumns: true,
   });
 
   return <StatusBar config={sampleConfig} setConfig={setConfig} />;
 }
```

### Comparing `buckaroo-0.3.6/js/components/gridUtils.ts` & `buckaroo-0.3.7/js/components/gridUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/staticData.ts` & `buckaroo-0.3.7/js/components/staticData.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/components/utils.ts` & `buckaroo-0.3.7/js/components/utils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/js/style/dcf-npm.css` & `buckaroo-0.3.7/js/style/dcf-npm.css`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/static/images/Buckaroo-screenshot.png` & `buckaroo-0.3.7/static/images/Buckaroo-screenshot.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/.gitignore` & `buckaroo-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/LICENSE.txt` & `buckaroo-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/README.md` & `buckaroo-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.6/pyproject.toml` & `buckaroo-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.3.6"
+version = "0.3.7"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `buckaroo-0.3.6/PKG-INFO` & `buckaroo-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckaroo
-Version: 0.3.6
+Version: 0.3.7
 Summary: Buckaroo - GUI Data wrangling for pandas
 Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

