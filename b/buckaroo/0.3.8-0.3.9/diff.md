# Comparing `tmp/buckaroo-0.3.8.tar.gz` & `tmp/buckaroo-0.3.9.tar.gz`

## Comparing `buckaroo-0.3.8.tar` & `buckaroo-0.3.9.tar`

### file list

```diff
@@ -1,111 +1,110 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.8/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.8/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.8/Untitled.ipynb
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.8/babel.config.js
--rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.8/bike-share-data-explore.ipynb
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo.json
--rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.8/col-ordering.ipynb
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 buckaroo-0.3.8/full_build.sh
--rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.8/gbfs-play.ipynb
--rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.8/gbfs-play2.ipynb
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.8/introduction.ipynb
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.8/notes.txt
--rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.8/package-lock.json
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.8/package.json
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.8/package.json.old
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.8/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.8/tryit.ipynb
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.8/tsconfig.json
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.8/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.8/webpack.lab.config.js
--rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.8/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.8/.yarn/cache/.gitignore
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/_version.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/all_transforms.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/analysis.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/buckaroo_widget.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/channeldata.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/configure_utils.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/lispy.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/pluggable_analysis_framework.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/summary_stats.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/views.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/package.json
--rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
--rw-r--r--   0        0        0    35562 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/399.3e3e7759bcde23618a29.js
--rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/41.dea207301743f71053c5.js
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/480.889b78dbe4b4e9d7c19c.js
--rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
--rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
--rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/remoteEntry.8912bbc931697c534f1a.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/style.js
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0  1691829 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/nbextension/index.js.map
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.8/buckaroo/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/make.bat
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/FAQ.rst
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/conf.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/contributing.rst
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/feature_reference.rst
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/index.rst
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/install.rst
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/using.rst
--rw-r--r--   0        0        0   835431 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/_static/Buckaroo-labled.png
--rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/_static/Statusbar.png
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/articles/dont-use-df-head-buckaroo-instead.rst
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/articles/index.rst
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 buckaroo-0.3.8/docs/source/articles/jupyter-table-widget-comparison.rst
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.8/example-notebooks/testcases-fast.ipynb
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/comp1.tsx
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/index.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/plugin.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/version.ts
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/ColumnsEditor.tsx
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/CommandUtils.ts
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/DCFCell.tsx
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/DFViewer.tsx
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/DependentTabs.tsx
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/OperationDetail.tsx
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/OperationUtils.ts
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/Operations.tsx
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/StatusBar.tsx
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/bakedOperationDefaults.ts
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/gridUtils.ts
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/staticData.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/components/utils.ts
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/dcf-npm.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.8/js/style/icons/filter.svg
--rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.8/static/images/Buckaroo-screenshot.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.8/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 buckaroo-0.3.8/README.md
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 buckaroo-0.3.8/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.9/.#package.json -> paddy@Paddys-MacBook-Air.local.405
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.9/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.9/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.9/Untitled.ipynb
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.9/babel.config.js
+-rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.9/bike-share-data-explore.ipynb
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo.json
+-rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.9/col-ordering.ipynb
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 buckaroo-0.3.9/full_build.sh
+-rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.9/gbfs-play.ipynb
+-rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.9/gbfs-play2.ipynb
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.9/introduction.ipynb
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.9/notes.txt
+-rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.9/package-lock.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 buckaroo-0.3.9/package.json
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.9/package.json.old
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.9/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.9/tryit.ipynb
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.9/tsconfig.json
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 buckaroo-0.3.9/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.9/webpack.lab.config.js
+-rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.9/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.9/.yarn/cache/.gitignore
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/_version.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/all_transforms.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/configure_utils.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/lispy.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/views.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
+-rw-r--r--   0        0        0    35591 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/399.8ed5a96dd47d25e9d3b9.js
+-rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/41.dea207301743f71053c5.js
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/480.889b78dbe4b4e9d7c19c.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
+-rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
+-rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/remoteEntry.694fb0cfcb57cb01a932.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0  1691465 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/nbextension/index.js.map
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.9/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/make.bat
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/conf.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/feature_reference.rst
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/index.rst
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/install.rst
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/using.rst
+-rw-r--r--   0        0        0   835431 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/_static/Buckaroo-labled.png
+-rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/_static/Statusbar.png
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/articles/dont-use-df-head-buckaroo-instead.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/articles/index.rst
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 buckaroo-0.3.9/docs/source/articles/jupyter-table-widget-comparison.rst
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.9/example-notebooks/testcases-fast.ipynb
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/comp1.tsx
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/version.ts
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/ColumnsEditor.tsx
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/CommandUtils.ts
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/DCFCell.tsx
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/DFViewer.tsx
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/DependentTabs.tsx
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/OperationDetail.tsx
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/OperationUtils.ts
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/Operations.tsx
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/StatusBar.tsx
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/bakedOperationDefaults.ts
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/gridUtils.ts
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/staticData.ts
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/components/utils.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/dcf-npm.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.9/js/style/icons/filter.svg
+-rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.9/static/images/Buckaroo-screenshot.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.9/LICENSE.txt
+-rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 buckaroo-0.3.9/README.md
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 buckaroo-0.3.9/PKG-INFO
```

### Comparing `buckaroo-0.3.8/RELEASE.md` & `buckaroo-0.3.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/bike-share-data-explore.ipynb` & `buckaroo-0.3.9/bike-share-data-explore.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/col-ordering.ipynb` & `buckaroo-0.3.9/col-ordering.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/gbfs-play.ipynb` & `buckaroo-0.3.9/gbfs-play.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/gbfs-play2.ipynb` & `buckaroo-0.3.9/gbfs-play2.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/introduction.ipynb` & `buckaroo-0.3.9/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/package-lock.json` & `buckaroo-0.3.9/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999958193979933%*

 * *Differences: {"'packages'": "{'': {'version': '0.3.9'}}", "'version'": "'0.3.9'"}*

```diff
@@ -66,15 +66,15 @@
                 "url-loader": "^4.1.0",
                 "webpack": "^5",
                 "webpack-cli": "^4.5.0",
                 "webpack-dev-server": "^4.0.0"
             },
             "license": "BSD-3-Clause",
             "name": "buckaroo",
-            "version": "0.3.8"
+            "version": "0.3.9"
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
-    "version": "0.3.8"
+    "version": "0.3.9"
 }
```

### Comparing `buckaroo-0.3.8/package.json` & `buckaroo-0.3.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9680706521739131%*

 * *Differences: {"'scripts'": "{'build': 'npm run build:lib && npm run build:nbextension && npm run "*

 * *              "build:labextension'}",*

 * * "'version'": "'0.3.9'"}*

```diff
@@ -141,15 +141,15 @@
     "main": "lib/index.js",
     "name": "buckaroo",
     "repository": {
         "type": "git",
         "url": "https://github.com/paddymul/buckaroo"
     },
     "scripts": {
-        "build": "npm run build:lib && npm run build:labextension",
+        "build": "npm run build:lib && npm run build:nbextension && npm run build:labextension",
         "build-full": "npm run build:lib &&  run build:nbextension && npm run build:labextension",
         "build:all": "npm run build:labextension && npm run build:nbextension && npm run build:widget-examples",
         "build:dev": "npm run build:lib && npm run build:nbextension && npm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "which jupyter && jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:nbextension": "webpack --mode=production --no-devtool",
@@ -166,9 +166,9 @@
         "test": "jest --verbose --passWithNoTests",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.3.8"
+    "version": "0.3.9"
 }
```

### Comparing `buckaroo-0.3.8/package.json.old` & `buckaroo-0.3.9/package.json.old`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/tryit.ipynb` & `buckaroo-0.3.9/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/tsconfig.json` & `buckaroo-0.3.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/webpack.config.js` & `buckaroo-0.3.9/webpack.config.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -94,32 +94,33 @@
     extensions: ['.webpack.js', '.web.js', '.ts', '.js', '.tsx'],
     plugins: [new TsconfigPathsPlugin()],
     fallback: {
         crypto: false
     },
 };
 
-module.exports = [{
-        entry: './examples/index-react18.tsx',
-        output: {
-            path: path.join(__dirname, '/examples/dist'),
-            filename: 'bundle.js'
-        },
-        module: {
-            rules: demoRules,
-        },
-        devtool: 'source-map',
-        externals,
-        resolve,
-        plugins: [new HtmlWebpackPlugin({
-            //template: './examples/index.html'
-            template: './examples/index.html'
-        })],
-        performance
-    },
+module.exports = [
+    // {
+    //     entry: './examples/index-react18.tsx',
+    //       output: {
+    //           path: path.join(__dirname, '/examples/dist'),
+    //           filename: 'bundle.js'
+    //       },
+    //   module: {
+    // 	rules: demoRules,
+    //   },
+    //   devtool: 'source-map',
+    //   externals,
+    //   resolve,
+    //     plugins: [new HtmlWebpackPlugin({
+    //               //template: './examples/index.html'
+    //               template: './examples/index.html'
+    //     })],
+    //     performance
+    // },
 
 
     /**
      * Notebook extension
      *
      * This bundle only contains the part of the JavaScript that is run on load of
      * the notebook.
```

### Comparing `buckaroo-0.3.8/yarn.lock` & `buckaroo-0.3.9/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/__init__.py` & `buckaroo-0.3.9/buckaroo/__init__.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/all_transforms.py` & `buckaroo-0.3.9/buckaroo/all_transforms.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/buckaroo_widget.py` & `buckaroo-0.3.9/buckaroo/buckaroo_widget.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/configure_utils.py` & `buckaroo-0.3.9/buckaroo/configure_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/dcf_transform.py` & `buckaroo-0.3.9/buckaroo/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/df_methods.py` & `buckaroo-0.3.9/buckaroo/df_methods.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/index.html` & `buckaroo-0.3.9/buckaroo/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/lispy.py` & `buckaroo-0.3.9/buckaroo/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/summary_stats.py` & `buckaroo-0.3.9/buckaroo/summary_stats.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/views.py` & `buckaroo-0.3.9/buckaroo/views.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/package.json` & `buckaroo-0.3.9/buckaroo/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672894021739131%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.694fb0cfcb57cb01a932.js'}}",*

 * * "'scripts'": "{'build': 'npm run build:lib && npm run build:nbextension && npm run "*

 * *              "build:labextension'}",*

 * * "'version'": "'0.3.9'"}*

```diff
@@ -81,15 +81,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/paddymul/buckaroo",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8912bbc931697c534f1a.js"
+            "load": "static/remoteEntry.694fb0cfcb57cb01a932.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./buckaroo/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -145,15 +145,15 @@
     "main": "lib/index.js",
     "name": "buckaroo",
     "repository": {
         "type": "git",
         "url": "https://github.com/paddymul/buckaroo"
     },
     "scripts": {
-        "build": "npm run build:lib && npm run build:labextension",
+        "build": "npm run build:lib && npm run build:nbextension && npm run build:labextension",
         "build-full": "npm run build:lib &&  run build:nbextension && npm run build:labextension",
         "build:all": "npm run build:labextension && npm run build:nbextension && npm run build:widget-examples",
         "build:dev": "npm run build:lib && npm run build:nbextension && npm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "which jupyter && jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:nbextension": "webpack --mode=production --no-devtool",
@@ -170,9 +170,9 @@
         "test": "jest --verbose --passWithNoTests",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.3.8"
+    "version": "0.3.9"
 }
```

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js` & `buckaroo-0.3.9/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt` & `buckaroo-0.3.9/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/399.3e3e7759bcde23618a29.js` & `buckaroo-0.3.9/buckaroo/labextension/static/399.8ed5a96dd47d25e9d3b9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1401,11 +1401,11 @@
             r()(o.Z, {
                 insert: "head",
                 singleton: !1
             });
             const l = o.Z.locals || {}
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"buckaroo","version":"0.3.8","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^29.2.0","ag-grid-react":"^29.2.0","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prismjs":"^1.28.0","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-preset-env":"^7.7.2","postcss-nested":"^6.0.0","sass":"^1.53.0","sass-loader":"^13.0.2","react-router":"^6.3.0","react-router-dom":"^5.2.0","rimraf":"^3.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"buckaroo","version":"0.3.9","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:nbextension && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^29.2.0","ag-grid-react":"^29.2.0","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prismjs":"^1.28.0","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-preset-env":"^7.7.2","postcss-nested":"^6.0.0","sass":"^1.53.0","sass-loader":"^13.0.2","react-router":"^6.3.0","react-router-dom":"^5.2.0","rimraf":"^3.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/41.dea207301743f71053c5.js` & `buckaroo-0.3.9/buckaroo/labextension/static/41.dea207301743f71053c5.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/480.889b78dbe4b4e9d7c19c.js` & `buckaroo-0.3.9/buckaroo/labextension/static/480.889b78dbe4b4e9d7c19c.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js` & `buckaroo-0.3.9/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js` & `buckaroo-0.3.9/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js` & `buckaroo-0.3.9/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js` & `buckaroo-0.3.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt` & `buckaroo-0.3.9/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/remoteEntry.8912bbc931697c534f1a.js` & `buckaroo-0.3.9/buckaroo/labextension/static/remoteEntry.694fb0cfcb57cb01a932.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, u, d, l, f, c, s, p, h, v, b, g, m, y, w, k = {
+    var e, r, t, a, o, n, i, u, f, l, d, c, s, p, h, v, b, g, m, y, w, k = {
             5941: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(935), t.e(41), t.e(399), t.e(568)]).then((() => () => t(1568))),
                         "./extension": () => Promise.all([t.e(935), t.e(41), t.e(399), t.e(480)]).then((() => () => t(4480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -45,25 +45,25 @@
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         0: "c008020c7e2133e6c7db",
         41: "dea207301743f71053c5",
-        399: "3e3e7759bcde23618a29",
+        399: "8ed5a96dd47d25e9d3b9",
         480: "889b78dbe4b4e9d7c19c",
         486: "f08778dfb765d893ceaf",
         497: "a76de7c665cc86a1c49a",
         568: "50d29d049ddb62602cc0",
         731: "d4bf968c7a94633ef5a3",
         935: "2832d17fef97c1ec6694"
     } [e] + ".js?v=" + {
         0: "c008020c7e2133e6c7db",
         41: "dea207301743f71053c5",
-        399: "3e3e7759bcde23618a29",
+        399: "8ed5a96dd47d25e9d3b9",
         480: "889b78dbe4b4e9d7c19c",
         486: "f08778dfb765d893ceaf",
         497: "a76de7c665cc86a1c49a",
         568: "50d29d049ddb62602cc0",
         731: "d4bf968c7a94633ef5a3",
         935: "2832d17fef97c1ec6694"
     } [e], P.g = function() {
@@ -74,18 +74,18 @@
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "buckaroo:", P.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
-                    var f = d[l];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var d = f[l];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
             var c = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = e[t];
@@ -120,16 +120,16 @@
                             u = o[r];
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    d = [];
-                return "default" === t && (u("ag-grid-community", "29.3.5", (() => P.e(731).then((() => () => P(1731))))), u("ag-grid-react", "29.3.5", (() => Promise.all([P.e(935), P.e(0), P.e(497)]).then((() => () => P(4e3))))), u("buckaroo", "0.3.8", (() => Promise.all([P.e(935), P.e(41), P.e(399), P.e(568)]).then((() => () => P(1568))))), u("lodash", "4.17.21", (() => P.e(486).then((() => () => P(6486)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (u("ag-grid-community", "29.3.5", (() => P.e(731).then((() => () => P(1731))))), u("ag-grid-react", "29.3.5", (() => Promise.all([P.e(935), P.e(0), P.e(497)]).then((() => () => P(4e3))))), u("buckaroo", "0.3.9", (() => Promise.all([P.e(935), P.e(41), P.e(399), P.e(568)]).then((() => () => P(1568))))), u("lodash", "4.17.21", (() => P.e(486).then((() => () => P(6486)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -165,47 +165,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(u = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, u);
             return t
         }
         var i = [];
         for (n = 1; n < e.length; n++) {
             var u = e[n];
-            i.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return d();
+        return f();
 
-        function d() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var i = 0, u = 1, d = !0;; u++, i++) {
-                var l, f, c = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !d || ("u" == c ? u > a && !o : "" == c != o);
-                if ("u" == f) {
-                    if (!d || "u" != c) return !1
-                } else if (d)
-                    if (c == f)
+            for (var i = 0, u = 1, f = !0;; u++, i++) {
+                var l, d, c = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(l = r[i]))[0])) return !f || ("u" == c ? u > a && !o : "" == c != o);
+                if ("u" == d) {
+                    if (!f || "u" != c) return !1
+                } else if (f)
+                    if (c == d)
                         if (u <= a) {
                             if (l != e[u]) return !1
                         } else {
                             if (o ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (d = !1)
+                            l != e[u] && (f = !1)
                         }
                 else if ("s" != c && "n" != c) {
                     if (o || u <= a) return !1;
-                    d = !1, u--
+                    f = !1, u--
                 } else {
-                    if (u <= a || f < c != o) return !1;
-                    d = !1
-                } else "s" != c && "n" != c && (d = !1, u--)
+                    if (u <= a || d < c != o) return !1;
+                    f = !1
+                } else "s" != c && "n" != c && (f = !1, u--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
@@ -214,29 +214,29 @@
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
-    }, d = (e, r) => {
+    }, f = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", f = (e, r, t, a) => {
-        var o = d(e, t);
+    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
+        var o = f(e, t);
         return n(a, o) || s(l(e, t, o, a)), p(e[t][o])
     }, c = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), v = (h = e => function(r, t, a, o) {
         var n = P.I(r);
         return n && n.then ? n.then(e.bind(e, r, P.S[r], t, a, o)) : e(r, P.S[r], t, a, o)
-    })(((e, r, t, a) => r && P.o(r, t) ? p(u(r, t)) : a())), b = h(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), g = h(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && P.o(r, t) ? p(u(r, t)) : a())), b = h(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), g = h(((e, r, t, a, o) => {
         var n = r && P.o(r, t) && c(r, t, a);
         return n ? p(n) : o()
     })), m = {}, y = {
         1048: () => v("default", "ag-grid-react", (() => Promise.all([P.e(0), P.e(497)]).then((() => () => P(4e3))))),
         2492: () => b("default", "@jupyter-widgets/base", [, [1, 6, 0, 0],
             [1, 4],
             [1, 3],
@@ -289,20 +289,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var a, o, [n, i, u] = t,
-                    d = 0;
+                    f = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) P.o(i, a) && (P.m[a] = i[a]);
                     u && u(P)
                 }
-                for (r && r(t); d < n.length; d++) o = n[d], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < n.length; f++) o = n[f], P.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var E = P(5941);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).buckaroo = E
 })();
```

### Comparing `buckaroo-0.3.8/buckaroo/labextension/static/third-party-licenses.json` & `buckaroo-0.3.9/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/nbextension/index.js` & `buckaroo-0.3.9/buckaroo/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -46916,24 +46916,24 @@
                 }) {
                     const c = e.schema.fields.map((e => e.name));
                     return a.default.createElement("div", {
                         className: "columns-editor",
                         style: {
                             width: "100%"
                         }
-                    }, s.showCommands ? a.default.createElement(l.OperationViewer, {
+                    }, s.showCommands ? a.default.createElement("div", null, a.default.createElement(l.OperationViewer, {
                         operations: n,
                         setOperations: r,
                         activeColumn: t,
                         allColumns: c,
                         commandConfig: i
-                    }) : a.default.createElement("span", null), s.showTransformed ? a.default.createElement(u.DependentTabs, {
+                    }), a.default.createElement(u.DependentTabs, {
                         filledOperations: n,
                         operationResult: o
-                    }) : a.default.createElement("span", null))
+                    })) : a.default.createElement("span", null))
                 }
                 t.ColumnsEditor = p, t.ColumnsEditorEx = function() {
                     const [e, t] = (0, a.useState)(s.bakedOperations), n = {
                         transformed_df: s.EmptyDf,
                         generated_py_code: "default py code",
                         transform_error: void 0
                     };
@@ -46941,16 +46941,15 @@
                         df: c.tableDf,
                         activeColumn: "foo",
                         commandConfig: c.bakedCommandConfig,
                         operations: e,
                         setOperations: t,
                         operationResult: n,
                         widgetConfig: {
-                            showCommands: !0,
-                            showTransformed: !0
+                            showCommands: !0
                         }
                     })
                 }
             },
             414: (e, t) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
@@ -47016,16 +47015,15 @@
                     operation_results: r,
                     commandConfig: o,
                     dfConfig: i,
                     on_dfConfig: s,
                     summaryDf: u
                 }) {
                     const [d, g] = (0, a.useState)("stoptime"), h = {
-                        showCommands: i.showCommands,
-                        showTransformed: i.showTransformed
+                        showCommands: i.showCommands
                     }, f = Object.assign(Object.assign({}, i), {
                         rowsShown: e.data.length || 0
                     });
                     return a.default.createElement("div", {
                         className: "dcf-root flex flex-col",
                         style: {
                             width: "100%",
@@ -47040,15 +47038,15 @@
                     }, a.default.createElement(p.StatusBar, {
                         config: f,
                         setConfig: s
                     }), a.default.createElement(c.DFViewer, {
                         df: i.summaryStats ? u : e,
                         activeCol: d,
                         setActiveCol: g
-                    })), h.showCommands || h.showTransformed ? a.default.createElement(l.ColumnsEditor, {
+                    })), h.showCommands ? a.default.createElement(l.ColumnsEditor, {
                         df: e,
                         activeColumn: d,
                         operations: t,
                         setOperations: n,
                         operationResult: r,
                         commandConfig: o,
                         widgetConfig: h
@@ -47058,16 +47056,14 @@
                     const [e, t] = (0, a.useState)({
                         totalRows: 1309,
                         columns: 30,
                         rowsShown: 500,
                         sampleSize: 1e4,
                         sampled: !0,
                         summaryStats: !1,
-                        reorderdColumns: !1,
-                        showTransformed: !0,
                         showCommands: !0
                     }), [n, r] = (0, a.useState)(g.bakedOperations);
                     return a.default.createElement(h, {
                         origDf: u.tableDf,
                         operations: n,
                         on_operations: r,
                         operation_results: s.baseOperationResults,
@@ -47721,34 +47717,36 @@
                     l = n(9831),
                     u = [{
                         field: "summaryStats",
                         headerName: "Σ",
                         headerTooltip: "Summary Stats",
                         width: 30
                     }, {
-                        field: "reorderdColumns",
-                        headerName: "Θ",
-                        headerTooltip: "Reorder Columns",
-                        width: 30
-                    }, {
-                        field: "showTransformed",
-                        headerName: "Δ",
-                        headerTooltip: "Show Transformation",
-                        width: 30
-                    }, {
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
+                        field: "help",
+                        headerName: "?",
+                        headerTooltip: "Help",
+                        width: 30,
+                        cellRenderer: function(e) {
+                            return a.default.createElement("a", {
+                                href: "https://buckaroo-data.readthedocs.io/en/latest/feature_reference.html",
+                                target: "_blank",
+                                rel: "noopener"
+                            }, "?")
+                        }
+                    }, {
                         field: "totalRows",
                         width: 100
                     }, {
                         field: "columns",
                         width: 100
                     }, {
                         field: "rowsShown",
@@ -47765,74 +47763,64 @@
                     const {
                         totalRows: n,
                         columns: r,
                         rowsShown: o,
                         sampleSize: i,
                         sampled: c,
                         summaryStats: p,
-                        reorderdColumns: d,
-                        showTransformed: g,
-                        showCommands: h
-                    } = e, f = [{
+                        showCommands: d
+                    } = e, g = [{
                         totalRows: l.intFormatter.format(n),
                         columns: r,
                         rowsShown: l.intFormatter.format(o),
                         sampleSize: l.intFormatter.format(i),
-                        sampled: c ? "Ϋ" : "ό",
-                        summaryStats: p ? "Ϋ" : "ό",
-                        reorderdColumns: d ? "Ϋ" : "ό",
-                        showTransformed: g ? "Ϋ" : "ό",
-                        showCommands: h ? "Ϋ" : "ό"
-                    }], v = (0, a.useRef)(null);
+                        sampled: c ? "1" : "0",
+                        summaryStats: p ? "1" : "0",
+                        showCommands: d ? "1" : "0"
+                    }], h = (0, a.useRef)(null);
                     return a.default.createElement("div", {
                         className: "statusBar"
                     }, a.default.createElement("div", {
                         style: {
                             height: 50
                         },
                         className: "theme-hanger ag-theme-alpine-dark"
                     }, a.default.createElement(s.AgGridReact, {
-                        ref: v,
+                        ref: h,
                         onCellClicked: n => {
                             const r = n.column.getColId();
                             "summaryStats" === r ? t(Object.assign(Object.assign({}, e), {
                                 summaryStats: !e.summaryStats
                             })) : "sampled" === r ? t(Object.assign(Object.assign({}, e), {
                                 sampled: !e.sampled
-                            })) : "reorderdColumns" === r ? t(Object.assign(Object.assign({}, e), {
-                                reorderdColumns: !e.reorderdColumns
-                            })) : "showTransformed" === r ? t(Object.assign(Object.assign({}, e), {
-                                showTransformed: !e.showTransformed
                             })) : "showCommands" === r && t(Object.assign(Object.assign({}, e), {
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
-                        rowData: f,
+                        rowData: g,
                         columnDefs: u
                     })))
                 }
                 t.StatusBar = c, t.StatusBarEx = function() {
                     const [e, t] = (0, a.useState)({
                         totalRows: 1309,
                         columns: 30,
                         rowsShown: 500,
                         sampleSize: 1e4,
                         sampled: !0,
                         summaryStats: !1,
-                        reorderdColumns: !0,
-                        showTransformed: !0,
                         showCommands: !0
                     });
                     return a.default.createElement(c, {
                         config: e,
                         setConfig: t
                     })
                 }
@@ -48317,15 +48305,15 @@
             },
             9146: t => {
                 "use strict";
                 t.exports = e
             },
             4147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"buckaroo","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^29.2.0","ag-grid-react":"^29.2.0","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prismjs":"^1.28.0","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-preset-env":"^7.7.2","postcss-nested":"^6.0.0","sass":"^1.53.0","sass-loader":"^13.0.2","react-router":"^6.3.0","react-router-dom":"^5.2.0","rimraf":"^3.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+                e.exports = JSON.parse('{"name":"buckaroo","version":"0.3.9","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"npm run build:lib && npm run build:nbextension && npm run build:labextension","build-full":"npm run build:lib &&  run build:nbextension && npm run build:labextension","build:dev":"npm run build:lib && npm run build:nbextension && npm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"which jupyter && jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"npm run build:labextension && npm run build:nbextension && npm run build:widget-examples","clean":"rimraf dist && npm run clean:lib && npm run clean:labextension && npm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:check":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"npm run build:labextension && npm run build:nbextension","test":"jest --verbose --passWithNoTests","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch .","dev":"webpack-cli serve --mode=development --env development --open"},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","ag-grid-community":"^29.2.0","ag-grid-react":"^29.2.0","lodash":"^4.17.21","react":"^18.0.0","react-dom":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.11","@babel/preset-typescript":"7.16.7","@jupyterlab/builder":"^3.0.1","@types/jest":"^28","@types/node":"^10.11.6","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/webpack-dev-server":"^3.11.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.9.1","@typescript-eslint/parser":"^5.9.1","acorn":"^6.2.0","babel-jest":"^28","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^5.0.0","eslint":"^8.6.0","eslint-config-prettier":"^8.3.0","eslint-plugin-prettier":"^4.0.0","eslint-plugin-react":"^7.28.0","eslint-plugin-react-hooks":"^4.3.0","fs-extra":"^7.0.0","html-loader":"^2.1.2","html-webpack-plugin":"^5.0.0","jest":"^28","lint-staged":"^10.2.11","markdown-loader":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.6.2","prettier-standalone":"^1.3.1-0","prismjs":"^1.28.0","postcss":"^8.4.14","postcss-loader":"^7.0.1","postcss-preset-env":"^7.7.2","postcss-nested":"^6.0.0","sass":"^1.53.0","sass-loader":"^13.0.2","react-router":"^6.3.0","react-router-dom":"^5.2.0","rimraf":"^3.0.2","source-map-loader":"^0.2.4","style-loader":"^2.0.0","svg-url-loader":"^7.1.1","ts-jest":"^28.0.8","ts-loader":"^8.0.14","ts-node":"^9.1.1","tsconfig-paths-webpack-plugin":"^3.3.0","typescript":"^4.4.3","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.5.0","webpack-dev-server":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
             }
         },
         n = {};
 
     function r(e) {
         var o = n[e];
         if (void 0 !== o) return o.exports;
```

### Comparing `buckaroo-0.3.8/buckaroo/nbextension/index.js.LICENSE.txt` & `buckaroo-0.3.9/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/nbextension/index.js.map` & `buckaroo-0.3.9/buckaroo/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/buckaroo/noarch/index.html` & `buckaroo-0.3.9/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/Makefile` & `buckaroo-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/make.bat` & `buckaroo-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/FAQ.rst` & `buckaroo-0.3.9/docs/source/FAQ.rst`

 * *Files 0% similar despite different names*

```diff
@@ -63,7 +63,8 @@
   Imagine you have a `dropcol` command which takes a single column to drop, also imagine that there is a function `dropcols` which takes a list of columns to drop.
 
   It is easier to build the UI to emit individual `dropcol` commands, you will end up with more readable code when you have a single command that drops all columns.
 
   You could write a transform which reads all `dropcol` forms and rewrites it to a single `dropcols` command.
 
   Alternatively, you could write a command that instead of subtractively reducing a dataframe, builds up a new dataframe from an explicit list of columns.  That is also a type of transform that could be written.
+
```

### Comparing `buckaroo-0.3.8/docs/source/conf.py` & `buckaroo-0.3.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/contributing.rst` & `buckaroo-0.3.9/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/feature_reference.rst` & `buckaroo-0.3.9/docs/source/feature_reference.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/index.rst` & `buckaroo-0.3.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/using.rst` & `buckaroo-0.3.9/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/_static/Buckaroo-labled.png` & `buckaroo-0.3.9/docs/source/_static/Buckaroo-labled.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/_static/Statusbar.png` & `buckaroo-0.3.9/docs/source/_static/Statusbar.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.3.9/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/articles/dont-use-df-head-buckaroo-instead.rst` & `buckaroo-0.3.9/docs/source/articles/dont-use-df-head-buckaroo-instead.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/articles/index.rst` & `buckaroo-0.3.9/docs/source/articles/index.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/docs/source/articles/jupyter-table-widget-comparison.rst` & `buckaroo-0.3.9/docs/source/articles/jupyter-table-widget-comparison.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/example-notebooks/testcases-fast.ipynb` & `buckaroo-0.3.9/example-notebooks/testcases-fast.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/dcefwidget.ts` & `buckaroo-0.3.9/js/dcefwidget.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/extension.ts` & `buckaroo-0.3.9/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/plugin.ts` & `buckaroo-0.3.9/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/ColumnsEditor.tsx` & `buckaroo-0.3.9/js/components/ColumnsEditor.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/CommandUtils.ts` & `buckaroo-0.3.9/js/components/CommandUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/DCFCell.tsx` & `buckaroo-0.3.9/js/components/DCFCell.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/DFViewer.tsx` & `buckaroo-0.3.9/js/components/DFViewer.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/DependentTabs.tsx` & `buckaroo-0.3.9/js/components/DependentTabs.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/OperationDetail.tsx` & `buckaroo-0.3.9/js/components/OperationDetail.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/OperationUtils.ts` & `buckaroo-0.3.9/js/components/OperationUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/Operations.tsx` & `buckaroo-0.3.9/js/components/Operations.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/StatusBar.tsx` & `buckaroo-0.3.9/js/components/StatusBar.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/gridUtils.ts` & `buckaroo-0.3.9/js/components/gridUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/staticData.ts` & `buckaroo-0.3.9/js/components/staticData.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/components/utils.ts` & `buckaroo-0.3.9/js/components/utils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/js/style/dcf-npm.css` & `buckaroo-0.3.9/js/style/dcf-npm.css`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/static/images/Buckaroo-screenshot.png` & `buckaroo-0.3.9/static/images/Buckaroo-screenshot.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/.gitignore` & `buckaroo-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/LICENSE.txt` & `buckaroo-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/README.md` & `buckaroo-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.8/pyproject.toml` & `buckaroo-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.3.8"
+version = "0.3.9"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `buckaroo-0.3.8/PKG-INFO` & `buckaroo-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckaroo
-Version: 0.3.8
+Version: 0.3.9
 Summary: Buckaroo - GUI Data wrangling for pandas
 Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

