# Comparing `tmp/ipydatawidgets-4.3.3.tar.gz` & `tmp/ipydatawidgets-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipydatawidgets-4.3.3.tar", last modified: Sun Feb 19 22:33:21 2023, max compression
+gzip compressed data, was "ipydatawidgets-4.3.4.tar", last modified: Sun Jun 11 17:22:22 2023, max compression
```

## Comparing `ipydatawidgets-4.3.3.tar` & `ipydatawidgets-4.3.4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.618106 ipydatawidgets-4.3.3/
--rw-rw-rw-   0        0        0     3190 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      790 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1004 2023-02-19 22:33:21.619106 ipydatawidgets-4.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3195 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.465496 ipydatawidgets-4.3.3/examples/
--rw-rw-rw-   0        0        0   698713 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/examples/DataImage.ipynb
--rw-rw-rw-   0        0        0    76901 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/examples/introduction.ipynb
--rw-rw-rw-   0        0        0     3164 2018-09-12 17:08:46.000000 ipydatawidgets-4.3.3/examples/test.ipynb
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.469496 ipydatawidgets-4.3.3/ipydatawidgets/
--rw-rw-rw-   0        0        0      308 2018-09-13 11:29:06.000000 ipydatawidgets-4.3.3/ipydatawidgets/__init__.py
--rw-rw-rw-   0        0        0       74 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/ipydatawidgets/_frontend.py
--rw-rw-rw-   0        0        0       74 2023-02-19 22:17:49.000000 ipydatawidgets-4.3.3/ipydatawidgets/_version.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.481500 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/
--rw-rw-rw-   0        0        0      222 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.485501 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/
--rw-rw-rw-   0        0        0      356 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/extension.js
--rw-rw-rw-   0        0        0    62774 2023-02-19 22:31:54.000000 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/index.js
--rw-rw-rw-   0        0        0      120 2023-02-19 22:31:54.000000 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/index.js.LICENSE.txt
--rw-rw-rw-   0        0        0   358927 2023-02-19 22:31:54.000000 ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/index.js.map
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.499487 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/
--rw-rw-rw-   0        0        0      497 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/__init__.py
--rw-rw-rw-   0        0        0      935 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/media.py
--rw-rw-rw-   0        0        0     4875 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/serializers.py
--rw-rw-rw-   0        0        0     1633 2018-09-12 17:08:46.000000 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/traits.py
--rw-rw-rw-   0        0        0     4206 2023-02-19 22:17:10.000000 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/union.py
--rw-rw-rw-   0        0        0     5981 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/ipydatawidgets/ndarray/widgets.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.511497 ipydatawidgets-4.3.3/ipydatawidgets/tests/
--rw-rw-rw-   0        0        0        0 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/conftest.py
--rw-rw-rw-   0        0        0      493 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/test_nbextension_path.py
--rw-rw-rw-   0        0        0     5074 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/test_ndarray_serializers.py
--rw-rw-rw-   0        0        0     4401 2018-09-12 17:08:46.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/test_ndarray_trait.py
--rw-rw-rw-   0        0        0     4401 2023-02-17 22:54:18.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/test_union.py
--rw-rw-rw-   0        0        0     4243 2023-02-19 22:17:10.000000 ipydatawidgets-4.3.3/ipydatawidgets/tests/test_widgets.py
--rw-rw-rw-   0        0        0      549 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/ipydatawidgets/widgets.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.477498 ipydatawidgets-4.3.3/ipydatawidgets.egg-info/
--rw-rw-rw-   0        0        0     1004 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/ipydatawidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3794 2023-02-19 22:33:21.000000 ipydatawidgets-4.3.3/ipydatawidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/ipydatawidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/ipydatawidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/ipydatawidgets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.437489 ipydatawidgets-4.3.3/jupyter-config/
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.512498 ipydatawidgets-4.3.3/jupyter-config/notebook.d/
--rw-rw-rw-   0        0        0       78 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/jupyter-config/notebook.d/jupyter-datawidgets.json
--rw-rw-rw-   0        0        0       84 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/lerna.json
--rw-rw-rw-   0        0        0      840 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/package.json
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.441490 ipydatawidgets-4.3.3/packages/
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.517502 ipydatawidgets-4.3.3/packages/jlabextension/
--rw-rw-rw-   0        0        0       45 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/packages/jlabextension/.npmignore
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.519504 ipydatawidgets-4.3.3/packages/jlabextension/dist/
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.520504 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/
--rw-rw-rw-   0        0        0     1738 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/package.json
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.533515 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/
--rw-rw-rw-   0        0        0    51232 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js
--rw-rw-rw-   0        0        0      120 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js.LICENSE.txt
--rw-rw-rw-   0        0        0    10694 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/824.9dfde28e806c4451c997.js
--rw-rw-rw-   0        0        0      502 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/880.b9ae0dbdfd88fcbf13dc.js
--rw-rw-rw-   0        0        0     6812 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/remoteEntry.63f06fe503a74d4c345d.js
--rw-rw-rw-   0        0        0      118 2023-02-19 22:33:18.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/style.js
--rw-rw-rw-   0        0        0     5258 2023-02-19 22:33:20.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/third-party-licenses.json
--rw-rw-rw-   0        0        0     1269 2023-02-19 22:33:15.000000 ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets-7.1.2.tgz
--rw-rw-rw-   0        0        0     1676 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jlabextension/package.json
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.535517 ipydatawidgets-4.3.3/packages/jlabextension/src/
--rw-rw-rw-   0        0        0     1444 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jlabextension/src/index.ts
--rw-rw-rw-   0        0        0      233 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jlabextension/tsconfig.json
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.542523 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/
--rw-rw-rw-   0        0        0       45 2018-09-13 10:13:45.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/.npmignore
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.547527 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/dist/
--rw-rw-rw-   0        0        0    62161 2023-02-19 22:31:54.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/dist/index.js
--rw-rw-rw-   0        0        0      120 2023-02-19 22:31:54.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/dist/index.js.LICENSE.txt
--rw-rw-rw-   0        0        0   357964 2023-02-19 22:31:54.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/dist/index.js.map
--rw-rw-rw-   0        0        0     2124 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/package.json
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.561058 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/
--rw-rw-rw-   0        0        0     1070 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/base.ts
--rw-rw-rw-   0        0        0      445 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/extension.ts
--rw-rw-rw-   0        0        0      175 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/index.ts
--rw-rw-rw-   0        0        0     3876 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/media.ts
--rw-rw-rw-   0        0        0     1234 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/ndarray.ts
--rw-rw-rw-   0        0        0      220 2018-09-13 11:29:06.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/version.ts
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.563059 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/
--rw-rw-rw-   0        0        0     1649 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/karma.conf.js
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.577070 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/
--rw-rw-rw-   0        0        0     1162 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/common.spec.ts
--rw-rw-rw-   0        0        0     3071 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/dummy-manager.spec.ts
--rw-rw-rw-   0        0        0     4270 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/media.spec.ts
--rw-rw-rw-   0        0        0     4836 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/ndarray.spec.ts
--rw-rw-rw-   0        0        0      403 2018-09-13 10:13:45.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/tsconfig.json
--rw-rw-rw-   0        0        0    11425 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/union.spec.ts
--rw-rw-rw-   0        0        0      683 2018-09-13 10:13:45.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/util.spec.ts
--rw-rw-rw-   0        0        0      266 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tsconfig.json
--rw-rw-rw-   0        0        0     1751 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/jupyter-datawidgets/webpack.config.js
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.580073 ipydatawidgets-4.3.3/packages/serializers/
--rw-rw-rw-   0        0        0     1638 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/package.json
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.591082 ipydatawidgets-4.3.3/packages/serializers/src/
--rw-rw-rw-   0        0        0     2460 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/src/common.ts
--rw-rw-rw-   0        0        0      549 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/packages/serializers/src/compression.ts
--rw-rw-rw-   0        0        0      204 2018-09-13 10:13:45.000000 ipydatawidgets-4.3.3/packages/serializers/src/index.ts
--rw-rw-rw-   0        0        0     9720 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/src/ndarray.ts
--rw-rw-rw-   0        0        0     5478 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/src/union.ts
--rw-rw-rw-   0        0        0      417 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/packages/serializers/src/util.ts
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.593085 ipydatawidgets-4.3.3/packages/serializers/tests/
--rw-rw-rw-   0        0        0     1597 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tests/karma.conf.js
-drwxrwxrwx   0        0        0        0 2023-02-19 22:33:21.615104 ipydatawidgets-4.3.3/packages/serializers/tests/src/
--rw-rw-rw-   0        0        0     3927 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/common.spec.ts
--rw-rw-rw-   0        0        0     3071 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/dummy-manager.spec.ts
--rw-rw-rw-   0        0        0    16010 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/ndarray.spec.ts
--rw-rw-rw-   0        0        0     2424 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/testhelper.spec.ts
--rw-rw-rw-   0        0        0      403 2018-09-13 10:13:45.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/tsconfig.json
--rw-rw-rw-   0        0        0    15929 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/union.spec.ts
--rw-rw-rw-   0        0        0     1174 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/packages/serializers/tests/src/util.spec.ts
--rw-rw-rw-   0        0        0      162 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/packages/serializers/tsconfig.json
--rw-rw-rw-   0        0        0      141 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      135 2018-03-19 16:18:48.000000 ipydatawidgets-4.3.3/pytest.ini
--rw-rw-rw-   0        0        0      524 2023-02-19 22:33:21.621108 ipydatawidgets-4.3.3/setup.cfg
--rw-rw-rw-   0        0        0     3481 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/setup.py
--rw-rw-rw-   0        0        0      363 2023-02-17 22:28:37.000000 ipydatawidgets-4.3.3/tsconfig-base.json
--rw-rw-rw-   0        0        0      202 2020-05-12 11:18:23.000000 ipydatawidgets-4.3.3/tsconfig.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.753657 ipydatawidgets-4.3.4/
+-rw-rw-rw-   0        0        0     3190 2017-07-31 17:16:59.000000 ipydatawidgets-4.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      790 2022-05-18 11:26:06.000000 ipydatawidgets-4.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1004 2023-06-11 17:22:22.754657 ipydatawidgets-4.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3195 2020-12-18 21:51:19.000000 ipydatawidgets-4.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.302653 ipydatawidgets-4.3.4/examples/
+-rw-rw-rw-   0        0        0   698713 2022-05-17 17:41:29.000000 ipydatawidgets-4.3.4/examples/DataImage.ipynb
+-rw-rw-rw-   0        0        0    76901 2022-05-17 17:41:25.000000 ipydatawidgets-4.3.4/examples/introduction.ipynb
+-rw-rw-rw-   0        0        0     3164 2022-05-17 17:41:28.000000 ipydatawidgets-4.3.4/examples/test.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.309655 ipydatawidgets-4.3.4/ipydatawidgets/
+-rw-rw-rw-   0        0        0      308 2020-03-16 13:21:55.000000 ipydatawidgets-4.3.4/ipydatawidgets/__init__.py
+-rw-rw-rw-   0        0        0       74 2020-03-16 13:23:18.000000 ipydatawidgets-4.3.4/ipydatawidgets/_frontend.py
+-rw-rw-rw-   0        0        0       74 2023-06-11 16:34:57.000000 ipydatawidgets-4.3.4/ipydatawidgets/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.353651 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/
+-rw-rw-rw-   0        0        0      222 2017-07-31 15:54:30.000000 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.377649 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/
+-rw-rw-rw-   0        0        0      356 2018-10-16 17:08:34.000000 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/extension.js
+-rw-rw-rw-   0        0        0    62774 2023-06-11 17:21:56.000000 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/index.js
+-rw-rw-rw-   0        0        0      120 2023-06-11 17:21:56.000000 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/index.js.LICENSE.txt
+-rw-rw-rw-   0        0        0   358927 2023-06-11 17:21:56.000000 ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/index.js.map
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.393650 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/
+-rw-rw-rw-   0        0        0      497 2020-03-16 13:23:18.000000 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/__init__.py
+-rw-rw-rw-   0        0        0      935 2020-03-16 13:23:18.000000 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/media.py
+-rw-rw-rw-   0        0        0     4875 2022-08-22 15:58:28.000000 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/serializers.py
+-rw-rw-rw-   0        0        0     1633 2022-08-22 15:58:28.000000 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/traits.py
+-rw-rw-rw-   0        0        0     4255 2023-06-11 15:08:33.000000 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/union.py
+-rw-rw-rw-   0        0        0     5981 2022-08-22 10:22:32.000000 ipydatawidgets-4.3.4/ipydatawidgets/ndarray/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.410653 ipydatawidgets-4.3.4/ipydatawidgets/tests/
+-rw-rw-rw-   0        0        0        0 2017-08-14 12:10:43.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/__init__.py
+-rw-rw-rw-   0        0        0     1479 2022-08-22 15:20:42.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/conftest.py
+-rw-rw-rw-   0        0        0      493 2017-08-15 11:32:34.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/test_nbextension_path.py
+-rw-rw-rw-   0        0        0     5074 2022-08-22 10:22:32.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/test_ndarray_serializers.py
+-rw-rw-rw-   0        0        0     4401 2018-06-05 06:43:52.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/test_ndarray_trait.py
+-rw-rw-rw-   0        0        0     4401 2020-03-16 13:23:18.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/test_union.py
+-rw-rw-rw-   0        0        0     4243 2023-06-11 15:08:05.000000 ipydatawidgets-4.3.4/ipydatawidgets/tests/test_widgets.py
+-rw-rw-rw-   0        0        0      549 2018-10-18 11:37:56.000000 ipydatawidgets-4.3.4/ipydatawidgets/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.351653 ipydatawidgets-4.3.4/ipydatawidgets.egg-info/
+-rw-rw-rw-   0        0        0     1004 2023-06-11 17:22:22.000000 ipydatawidgets-4.3.4/ipydatawidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3794 2023-06-11 17:22:22.000000 ipydatawidgets-4.3.4/ipydatawidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 17:22:22.000000 ipydatawidgets-4.3.4/ipydatawidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-06-11 17:22:22.000000 ipydatawidgets-4.3.4/ipydatawidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-11 17:22:22.000000 ipydatawidgets-4.3.4/ipydatawidgets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.208653 ipydatawidgets-4.3.4/jupyter-config/
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.420650 ipydatawidgets-4.3.4/jupyter-config/notebook.d/
+-rw-rw-rw-   0        0        0       78 2018-03-05 16:31:29.000000 ipydatawidgets-4.3.4/jupyter-config/notebook.d/jupyter-datawidgets.json
+-rw-rw-rw-   0        0        0       84 2022-08-22 10:22:32.000000 ipydatawidgets-4.3.4/lerna.json
+-rw-rw-rw-   0        0        0      840 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/package.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.219653 ipydatawidgets-4.3.4/packages/
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.425652 ipydatawidgets-4.3.4/packages/jlabextension/
+-rw-rw-rw-   0        0        0       45 2018-03-08 16:29:54.000000 ipydatawidgets-4.3.4/packages/jlabextension/.npmignore
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.427652 ipydatawidgets-4.3.4/packages/jlabextension/dist/
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.429653 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/
+-rw-rw-rw-   0        0        0     1738 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/package.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.453655 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/
+-rw-rw-rw-   0        0        0    51232 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js
+-rw-rw-rw-   0        0        0      120 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js.LICENSE.txt
+-rw-rw-rw-   0        0        0    10694 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/824.9dfde28e806c4451c997.js
+-rw-rw-rw-   0        0        0      502 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/880.b9ae0dbdfd88fcbf13dc.js
+-rw-rw-rw-   0        0        0     6812 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/remoteEntry.f97952eab67caf5bb845.js
+-rw-rw-rw-   0        0        0      118 2023-06-11 17:22:17.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/style.js
+-rw-rw-rw-   0        0        0     5258 2023-06-11 17:22:20.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/third-party-licenses.json
+-rw-rw-rw-   0        0        0     1269 2023-06-11 17:22:07.000000 ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets-7.1.2.tgz
+-rw-rw-rw-   0        0        0     1676 2022-08-22 17:02:08.000000 ipydatawidgets-4.3.4/packages/jlabextension/package.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.455652 ipydatawidgets-4.3.4/packages/jlabextension/src/
+-rw-rw-rw-   0        0        0     1444 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/jlabextension/src/index.ts
+-rw-rw-rw-   0        0        0      233 2022-05-17 17:46:23.000000 ipydatawidgets-4.3.4/packages/jlabextension/tsconfig.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.467653 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/
+-rw-rw-rw-   0        0        0       45 2019-07-04 11:25:27.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/.npmignore
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.473654 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/dist/
+-rw-rw-rw-   0        0        0    62161 2023-06-11 17:21:56.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/dist/index.js
+-rw-rw-rw-   0        0        0      120 2023-06-11 17:21:56.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/dist/index.js.LICENSE.txt
+-rw-rw-rw-   0        0        0   357964 2023-06-11 17:21:56.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/dist/index.js.map
+-rw-rw-rw-   0        0        0     2124 2022-08-22 17:02:08.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/package.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.489652 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/
+-rw-rw-rw-   0        0        0     1070 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/base.ts
+-rw-rw-rw-   0        0        0      445 2020-03-16 13:21:55.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/extension.ts
+-rw-rw-rw-   0        0        0      175 2020-03-16 13:23:18.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/index.ts
+-rw-rw-rw-   0        0        0     3876 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/media.ts
+-rw-rw-rw-   0        0        0     1234 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/ndarray.ts
+-rw-rw-rw-   0        0        0      220 2020-03-16 13:21:55.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/version.ts
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.508651 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/
+-rw-rw-rw-   0        0        0     1649 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/karma.conf.js
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.626650 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/
+-rw-rw-rw-   0        0        0     1162 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/common.spec.ts
+-rw-rw-rw-   0        0        0     3071 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/dummy-manager.spec.ts
+-rw-rw-rw-   0        0        0     4270 2020-12-18 21:51:19.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/media.spec.ts
+-rw-rw-rw-   0        0        0     4836 2020-12-18 21:51:19.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/ndarray.spec.ts
+-rw-rw-rw-   0        0        0      403 2019-07-04 11:25:27.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/tsconfig.json
+-rw-rw-rw-   0        0        0    11425 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/union.spec.ts
+-rw-rw-rw-   0        0        0      683 2019-07-04 11:25:27.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/util.spec.ts
+-rw-rw-rw-   0        0        0      266 2022-05-17 17:41:58.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tsconfig.json
+-rw-rw-rw-   0        0        0     1751 2022-05-03 09:58:54.000000 ipydatawidgets-4.3.4/packages/jupyter-datawidgets/webpack.config.js
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.633671 ipydatawidgets-4.3.4/packages/serializers/
+-rw-rw-rw-   0        0        0     1638 2022-08-22 17:02:08.000000 ipydatawidgets-4.3.4/packages/serializers/package.json
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.645652 ipydatawidgets-4.3.4/packages/serializers/src/
+-rw-rw-rw-   0        0        0     2460 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/serializers/src/common.ts
+-rw-rw-rw-   0        0        0      549 2020-03-16 13:23:18.000000 ipydatawidgets-4.3.4/packages/serializers/src/compression.ts
+-rw-rw-rw-   0        0        0      204 2019-07-04 11:25:27.000000 ipydatawidgets-4.3.4/packages/serializers/src/index.ts
+-rw-rw-rw-   0        0        0     9720 2022-08-26 15:20:26.000000 ipydatawidgets-4.3.4/packages/serializers/src/ndarray.ts
+-rw-rw-rw-   0        0        0     5478 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/serializers/src/union.ts
+-rw-rw-rw-   0        0        0      417 2020-03-16 13:21:55.000000 ipydatawidgets-4.3.4/packages/serializers/src/util.ts
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.648677 ipydatawidgets-4.3.4/packages/serializers/tests/
+-rw-rw-rw-   0        0        0     1597 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/serializers/tests/karma.conf.js
+drwxrwxrwx   0        0        0        0 2023-06-11 17:22:22.751652 ipydatawidgets-4.3.4/packages/serializers/tests/src/
+-rw-rw-rw-   0        0        0     3927 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/common.spec.ts
+-rw-rw-rw-   0        0        0     3071 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/dummy-manager.spec.ts
+-rw-rw-rw-   0        0        0    16010 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/ndarray.spec.ts
+-rw-rw-rw-   0        0        0     2424 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/testhelper.spec.ts
+-rw-rw-rw-   0        0        0      403 2019-07-04 11:25:27.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/tsconfig.json
+-rw-rw-rw-   0        0        0    15929 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/union.spec.ts
+-rw-rw-rw-   0        0        0     1174 2020-03-16 13:21:55.000000 ipydatawidgets-4.3.4/packages/serializers/tests/src/util.spec.ts
+-rw-rw-rw-   0        0        0      162 2022-05-17 17:46:28.000000 ipydatawidgets-4.3.4/packages/serializers/tsconfig.json
+-rw-rw-rw-   0        0        0      141 2022-05-17 13:56:04.000000 ipydatawidgets-4.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      135 2017-08-14 19:15:34.000000 ipydatawidgets-4.3.4/pytest.ini
+-rw-rw-rw-   0        0        0      524 2023-06-11 17:22:22.761653 ipydatawidgets-4.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     3481 2022-08-22 10:22:33.000000 ipydatawidgets-4.3.4/setup.py
+-rw-rw-rw-   0        0        0      363 2022-05-17 17:46:23.000000 ipydatawidgets-4.3.4/tsconfig-base.json
+-rw-rw-rw-   0        0        0      202 2020-03-16 13:21:55.000000 ipydatawidgets-4.3.4/tsconfig.json
```

### Comparing `ipydatawidgets-4.3.3/LICENSE.txt` & `ipydatawidgets-4.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/MANIFEST.in` & `ipydatawidgets-4.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/PKG-INFO` & `ipydatawidgets-4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipydatawidgets
-Version: 4.3.3
+Version: 4.3.4
 Summary: A set of widgets to help facilitate reuse of large datasets across widgets
 Home-page: https://github.com/vidartf/ipydatawidgets
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
```

### Comparing `ipydatawidgets-4.3.3/README.md` & `ipydatawidgets-4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/examples/DataImage.ipynb` & `ipydatawidgets-4.3.4/examples/DataImage.ipynb`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/examples/introduction.ipynb` & `ipydatawidgets-4.3.4/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/examples/test.ipynb` & `ipydatawidgets-4.3.4/examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/index.js` & `ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/index.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/nbextension/static/index.js.map` & `ipydatawidgets-4.3.4/ipydatawidgets/nbextension/static/index.js.map`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/ndarray/media.py` & `ipydatawidgets-4.3.4/ipydatawidgets/ndarray/media.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/ndarray/serializers.py` & `ipydatawidgets-4.3.4/ipydatawidgets/ndarray/serializers.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/ndarray/traits.py` & `ipydatawidgets-4.3.4/ipydatawidgets/ndarray/traits.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/ndarray/union.py` & `ipydatawidgets-4.3.4/ipydatawidgets/ndarray/union.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
             silent = False
         if silent is not True:
             # we explicitly compare silent to True just in case the equality
             # comparison above returns something other than True/False
             obj._notify_trait(self.name, old_value, new_value)
 
     def subclass_init(self, cls):
-        cls._instance_inits.append(self.instance_init)
+        if hasattr(cls, "_instance_inits"):
+            cls._instance_inits.append(self.instance_init)
         return super().subclass_init(cls)
 
     def instance_init(self, inst):
         inst.observe(self._on_instance_value_change, self.name)
 
     def _on_instance_value_change(self, change):
         inst = change['owner']
```

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/ndarray/widgets.py` & `ipydatawidgets-4.3.4/ipydatawidgets/ndarray/widgets.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/tests/conftest.py` & `ipydatawidgets-4.3.4/ipydatawidgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/tests/test_ndarray_serializers.py` & `ipydatawidgets-4.3.4/ipydatawidgets/tests/test_ndarray_serializers.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/tests/test_ndarray_trait.py` & `ipydatawidgets-4.3.4/ipydatawidgets/tests/test_ndarray_trait.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/tests/test_union.py` & `ipydatawidgets-4.3.4/ipydatawidgets/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/tests/test_widgets.py` & `ipydatawidgets-4.3.4/ipydatawidgets/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets/widgets.py` & `ipydatawidgets-4.3.4/ipydatawidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets.egg-info/PKG-INFO` & `ipydatawidgets-4.3.4/ipydatawidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipydatawidgets
-Version: 4.3.3
+Version: 4.3.4
 Summary: A set of widgets to help facilitate reuse of large datasets across widgets
 Home-page: https://github.com/vidartf/ipydatawidgets
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
```

### Comparing `ipydatawidgets-4.3.3/ipydatawidgets.egg-info/SOURCES.txt` & `ipydatawidgets-4.3.4/ipydatawidgets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 packages/jlabextension/tsconfig.json
 packages/jlabextension/dist/jupyterlab-datawidgets-7.1.2.tgz
 packages/jlabextension/dist/jupyterlab-datawidgets/package.json
 packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js
 packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js.LICENSE.txt
 packages/jlabextension/dist/jupyterlab-datawidgets/static/824.9dfde28e806c4451c997.js
 packages/jlabextension/dist/jupyterlab-datawidgets/static/880.b9ae0dbdfd88fcbf13dc.js
-packages/jlabextension/dist/jupyterlab-datawidgets/static/remoteEntry.63f06fe503a74d4c345d.js
+packages/jlabextension/dist/jupyterlab-datawidgets/static/remoteEntry.f97952eab67caf5bb845.js
 packages/jlabextension/dist/jupyterlab-datawidgets/static/style.js
 packages/jlabextension/dist/jupyterlab-datawidgets/static/third-party-licenses.json
 packages/jlabextension/src/index.ts
 packages/jupyter-datawidgets/.npmignore
 packages/jupyter-datawidgets/package.json
 packages/jupyter-datawidgets/tsconfig.json
 packages/jupyter-datawidgets/webpack.config.js
```

### Comparing `ipydatawidgets-4.3.3/package.json` & `ipydatawidgets-4.3.4/package.json`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/package.json` & `ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static\\\\remoteEntry.f97952eab67caf5bb845.js'}}"}*

```diff
@@ -20,15 +20,15 @@
     "files": [
         "build/*.js"
     ],
     "homepage": "https://github.com/vidartf/jupyter-datawidgets",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static\\remoteEntry.63f06fe503a74d4c345d.js"
+            "load": "static\\remoteEntry.f97952eab67caf5bb845.js"
         },
         "extension": "build/index.js",
         "outputDir": "dist/jupyterlab-datawidgets",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js` & `ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/511.22f7942246884696c751.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/824.9dfde28e806c4451c997.js` & `ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/824.9dfde28e806c4451c997.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/remoteEntry.63f06fe503a74d4c345d.js` & `ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/remoteEntry.f97952eab67caf5bb845.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, u, l, s, d, f, p, c, h, v, b, g, m = {
-            614: (e, r, t) => {
+            545: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(170), t.e(880)]).then((() => () => t(880))),
                         "./extension": () => Promise.all([t.e(170), t.e(880)]).then((() => () => t(880)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -269,10 +269,10 @@
                     u && u(w)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkjupyterlab_datawidgets = self.webpackChunkjupyterlab_datawidgets || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var j = w(614);
+    var j = w(545);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-datawidgets"] = j
 })();
```

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets/static/third-party-licenses.json` & `ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/dist/jupyterlab-datawidgets-7.1.2.tgz` & `ipydatawidgets-4.3.4/packages/jlabextension/dist/jupyterlab-datawidgets-7.1.2.tgz`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/package.json` & `ipydatawidgets-4.3.4/packages/jlabextension/package.json`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jlabextension/src/index.ts` & `ipydatawidgets-4.3.4/packages/jlabextension/src/index.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/dist/index.js` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/dist/index.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/dist/index.js.map` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/dist/index.js.map`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/package.json` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/package.json`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/base.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/base.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/media.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/media.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/src/ndarray.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/src/ndarray.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/karma.conf.js` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/common.spec.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/common.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/dummy-manager.spec.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/dummy-manager.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/media.spec.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/media.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/ndarray.spec.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/ndarray.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/union.spec.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/union.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/tests/src/util.spec.ts` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/tests/src/util.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/jupyter-datawidgets/webpack.config.js` & `ipydatawidgets-4.3.4/packages/jupyter-datawidgets/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/package.json` & `ipydatawidgets-4.3.4/packages/serializers/package.json`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/src/common.ts` & `ipydatawidgets-4.3.4/packages/serializers/src/common.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/src/compression.ts` & `ipydatawidgets-4.3.4/packages/serializers/src/compression.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/src/ndarray.ts` & `ipydatawidgets-4.3.4/packages/serializers/src/ndarray.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/src/union.ts` & `ipydatawidgets-4.3.4/packages/serializers/src/union.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/karma.conf.js` & `ipydatawidgets-4.3.4/packages/serializers/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/src/common.spec.ts` & `ipydatawidgets-4.3.4/packages/serializers/tests/src/common.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/src/dummy-manager.spec.ts` & `ipydatawidgets-4.3.4/packages/serializers/tests/src/dummy-manager.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/src/ndarray.spec.ts` & `ipydatawidgets-4.3.4/packages/serializers/tests/src/ndarray.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/src/testhelper.spec.ts` & `ipydatawidgets-4.3.4/packages/serializers/tests/src/testhelper.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/src/union.spec.ts` & `ipydatawidgets-4.3.4/packages/serializers/tests/src/union.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/packages/serializers/tests/src/util.spec.ts` & `ipydatawidgets-4.3.4/packages/serializers/tests/src/util.spec.ts`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/setup.cfg` & `ipydatawidgets-4.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ipydatawidgets-4.3.3/setup.py` & `ipydatawidgets-4.3.4/setup.py`

 * *Files identical despite different names*

