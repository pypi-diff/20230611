# Comparing `tmp/wxee-0.3.3.tar.gz` & `tmp/wxee-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxee-0.3.3.tar", last modified: Sat Aug 27 23:28:36 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `wxee-0.3.3.tar` & `wxee-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,17 @@
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2022-08-27 23:28:36.104582 wxee-0.3.3/
--rw-r--r--   0 az        (1000) az        (1000)    35149 2021-08-01 18:32:34.000000 wxee-0.3.3/LICENSE
--rw-rw-r--   0 az        (1000) az        (1000)     8309 2022-08-27 23:28:36.104582 wxee-0.3.3/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)     6046 2022-08-27 20:44:19.000000 wxee-0.3.3/README.rst
--rw-rw-r--   0 az        (1000) az        (1000)       38 2022-08-27 23:28:36.104582 wxee-0.3.3/setup.cfg
--rw-rw-r--   0 az        (1000) az        (1000)     1831 2022-08-27 23:27:56.000000 wxee-0.3.3/setup.py
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2022-08-27 23:28:36.104582 wxee-0.3.3/test/
--rw-r--r--   0 az        (1000) az        (1000)      399 2021-09-13 02:26:24.000000 wxee-0.3.3/test/test_accessors.py
--rw-r--r--   0 az        (1000) az        (1000)     5170 2021-10-21 00:49:15.000000 wxee-0.3.3/test/test_collection.py
--rw-r--r--   0 az        (1000) az        (1000)     4830 2022-08-27 21:45:11.000000 wxee-0.3.3/test/test_image.py
--rw-r--r--   0 az        (1000) az        (1000)      921 2021-10-21 00:49:15.000000 wxee-0.3.3/test/test_params.py
--rw-rw-r--   0 az        (1000) az        (1000)    14504 2022-08-27 23:23:11.000000 wxee-0.3.3/test/test_time_series.py
--rw-rw-r--   0 az        (1000) az        (1000)     6981 2022-08-27 20:44:16.000000 wxee-0.3.3/test/test_utils.py
--rw-rw-r--   0 az        (1000) az        (1000)     2753 2021-11-02 05:48:02.000000 wxee-0.3.3/test/test_xarray.py
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2022-08-27 23:28:36.104582 wxee-0.3.3/wxee/
--rw-rw-r--   0 az        (1000) az        (1000)      189 2022-08-27 23:27:56.000000 wxee-0.3.3/wxee/__init__.py
--rw-rw-r--   0 az        (1000) az        (1000)      737 2021-08-28 19:59:54.000000 wxee-0.3.3/wxee/accessors.py
--rw-rw-r--   0 az        (1000) az        (1000)     2187 2021-10-21 00:49:14.000000 wxee-0.3.3/wxee/climatology.py
--rw-rw-r--   0 az        (1000) az        (1000)     9351 2022-08-27 20:44:16.000000 wxee-0.3.3/wxee/collection.py
--rw-rw-r--   0 az        (1000) az        (1000)       24 2021-10-18 01:59:28.000000 wxee-0.3.3/wxee/constants.py
--rw-rw-r--   0 az        (1000) az        (1000)      210 2022-08-27 21:23:06.000000 wxee-0.3.3/wxee/exceptions.py
--rw-rw-r--   0 az        (1000) az        (1000)    11298 2022-08-27 21:50:15.000000 wxee-0.3.3/wxee/image.py
--rw-rw-r--   0 az        (1000) az        (1000)     1197 2021-10-21 05:11:10.000000 wxee-0.3.3/wxee/interpolation.py
--rw-rw-r--   0 az        (1000) az        (1000)      968 2021-10-18 01:59:28.000000 wxee-0.3.3/wxee/params.py
--rw-rw-r--   0 az        (1000) az        (1000)    35691 2022-08-27 23:20:56.000000 wxee-0.3.3/wxee/time_series.py
--rw-rw-r--   0 az        (1000) az        (1000)     7860 2022-08-27 23:09:56.000000 wxee-0.3.3/wxee/utils.py
--rw-rw-r--   0 az        (1000) az        (1000)     4752 2021-11-02 05:48:02.000000 wxee-0.3.3/wxee/xarray.py
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2022-08-27 23:28:36.104582 wxee-0.3.3/wxee.egg-info/
--rw-rw-r--   0 az        (1000) az        (1000)     8309 2022-08-27 23:28:36.000000 wxee-0.3.3/wxee.egg-info/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)      527 2022-08-27 23:28:36.000000 wxee-0.3.3/wxee.egg-info/SOURCES.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2022-08-27 23:28:36.000000 wxee-0.3.3/wxee.egg-info/dependency_links.txt
--rw-rw-r--   0 az        (1000) az        (1000)      315 2022-08-27 23:28:36.000000 wxee-0.3.3/wxee.egg-info/requires.txt
--rw-rw-r--   0 az        (1000) az        (1000)        5 2022-08-27 23:28:36.000000 wxee-0.3.3/wxee.egg-info/top_level.txt
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/accessors.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/climatology.py
+-rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/collection.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/constants.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/exceptions.py
+-rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/image.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/interpolation.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/params.py
+-rw-r--r--   0        0        0    35987 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/time_series.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/utils.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 wxee-0.4.0/wxee/xarray.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wxee-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 wxee-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 wxee-0.4.0/README.rst
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 wxee-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 wxee-0.4.0/PKG-INFO
```

### Comparing `wxee-0.3.3/PKG-INFO` & `wxee-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,201 +1,231 @@
 Metadata-Version: 2.1
 Name: wxee
-Version: 0.3.3
+Version: 0.4.0
 Summary: Earth Engine to xarray interface
-Home-page: https://github.com/aazuspan/wxee
-Author: Aaron Zuspan
-Author-email: aazuspan@gmail.com
-License: GPLv3+
-Description: .. image:: https://raw.githubusercontent.com/aazuspan/wxee/main/docs/_static/wxee.png
-           :alt: wxee .-- -..-
-           :width: 200
-           :target: https://github.com/aazuspan/wxee
-        
-        |
-        
-        .. image:: https://img.shields.io/badge/Earth%20Engine%20API-Python-green
-           :alt: Earth Engine Python
-           :target: https://developers.google.com/earth-engine/tutorials/community/intro-to-python-api
-        .. image:: https://img.shields.io/pypi/v/wxee
-           :alt: PyPI
-           :target: https://pypi.org/project/wxee/
-        .. image:: https://img.shields.io/conda/vn/conda-forge/wxee.svg
-           :alt: conda-forge
-           :target: https://anaconda.org/conda-forge/wxee
-        .. image:: https://colab.research.google.com/assets/colab-badge.svg
-           :alt: Open in Colab
-           :target: https://colab.research.google.com/github/aazuspan/wxee/blob/main/docs/examples/image_collection_to_xarray.ipynb
-        .. image:: https://readthedocs.org/projects/wxee/badge/?version=latest&style=flat
-           :alt: Read the Docs
-           :target: https://wxee.readthedocs.io/en/latest/?badge=latest
-        .. image:: https://github.com/aazuspan/wxee/actions/workflows/tests.yml/badge.svg
-           :alt: Build status
-           :target: https://github.com/aazuspan/wxee
-        .. image:: https://codecov.io/gh/aazuspan/wxee/branch/main/graph/badge.svg?token=OeSeq4b7NF
-           :alt: Code coverage
-           :target: https://codecov.io/gh/aazuspan/wxee
-        
-        ------------
-        
-        .. image:: https://raw.githubusercontent.com/aazuspan/wxee/main/docs/_static/demo_001.gif
-          :alt: Demo downloading weather data to xarray using wxee.
-        
-        
-        What is wxee?
-        -------------
-        `wxee <https://github.com/aazuspan/wxee>`_ was built to make processing gridded, mesoscale time series data quick 
-        and easy by integrating the data catalog and processing power of `Google Earth Engine <https://earthengine.google.com/>`_ with the 
-        flexibility of `xarray <https://github.com/pydata/xarray>`_, with no complicated setup required. To accomplish this, wxee implements 
-        convenient methods for data processing, aggregation, downloading, and ingestion.
-        
-        `wxee <https://github.com/aazuspan/wxee>`_ can be found in the `Earth Engine Developer Resources <https://developers.google.com/earth-engine/tutorials/community/developer-resources#python>`_!
-        
-        
-        Features
-        --------
-        * Time series image collections to `xarray <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`_, `NetCDF <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`_, or `GeoTIFF <https://wxee.readthedocs.io/en/latest/examples/downloading_images_and_collections.html>`_ in one line of code
-        * `Climatological anomalies <https://wxee.readthedocs.io/en/latest/examples/climatology_anomaly.html>`_ and temporal `aggregation <https://wxee.readthedocs.io/en/latest/examples/temporal_aggregation.html>`_, `interpolation <https://wxee.readthedocs.io/en/latest/examples/temporal_interpolation.html>`_, `smoothing <https://wxee.readthedocs.io/en/latest/generated/wxee.time_series.TimeSeries.rolling_time.html>`_, and `gap-filling <https://wxee.readthedocs.io/en/latest/generated/wxee.time_series.TimeSeries.fill_gaps.html>`_ in Earth Engine
-        * `Color composite plots <https://wxee.readthedocs.io/en/latest/examples/color_composites.html>`_ from **xarray** datasets
-        * Parallel processing for fast downloads
-        
-        
-        To see some of the capabilities of wxee and try it yourself, check out the interactive notebooks `here <https://wxee.readthedocs.io/en/latest/examples.html>`_!
-        
-        Install
-        ------------
-        
-        Pip
-        ~~~
-        
-        .. code-block:: bash
-        
-           pip install wxee
-        
-        Conda
-        ~~~~~
-        
-        .. code-block:: bash
-        
-            conda install -c conda-forge wxee
-        
-        From Source
-        ~~~~~~~~~~~
-        
-        .. code-block:: bash
-        
-           git clone https://github.com/aazuspan/wxee
-           cd wxee
-           make install
-        
-        
-        Quickstart
-        ----------
-        
-        Setup
-        ~~~~~
-        Once you have access to Google Earth Engine, just import and initialize :code:`ee` and :code:`wxee`.
-        
-        .. code-block:: python
-           
-           import ee
-           import wxee
-        
-           wxee.Initialize()
-        
-        
-        Download Images
-        ~~~~~~~~~~~~~~~
-        
-        Download and conversion methods are extended to :code:`ee.Image` and :code:`ee.ImageCollection` using the 
-        :code:`wx` accessor. Just :code:`import wxee` and use the :code:`wx` accessor.
-        
-        xarray
-        ^^^^^^
-        
-        .. code-block:: python
-        
-           ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").wx.to_xarray()
-        
-        NetCDF
-        ^^^^^^
-        
-        .. code-block:: python
-        
-           ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").wx.to_xarray(path="data/gridmet.nc")
-        
-        GeoTIFF
-        ^^^^^^^
-        
-        .. code-block:: python
-        
-           ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").wx.to_tif()
-        
-        
-        Create a Time Series
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        Additional methods for processing image collections in the time dimension are available through the :code:`TimeSeries` subclass.
-        A :code:`TimeSeries` can be created from an existing :code:`ee.ImageCollection`...
-        
-        .. code-block:: python
-        
-           col = ee.ImageCollection("IDAHO_EPSCOR/GRIDMET")
-           ts = col.wx.to_time_series()
-        
-        Or instantiated directly just like you would an :code:`ee.ImageCollection`!
-        
-        .. code-block:: python
-        
-           ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
-        
-        
-        Aggregate Daily Data
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        Many weather datasets are in daily or hourly resolution. These can be aggregated to coarser resolutions using the :code:`aggregate_time`
-        method of the :code:`TimeSeries` class.
-        
-        .. code-block:: python
-        
-           ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
-           monthly_max = ts.aggregate_time(frequency="month", reducer=ee.Reducer.max())
-        
-        Calculate Climatological Means
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Long-term climatological means can be calculated using the :code:`climatology_mean` method of the :code:`TimeSeries` class.
-        
-        .. code-block:: python
-        
-           ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
-           mean_clim = ts.climatology_mean(frequency="month")
-        
-        Contribute
-        ----------
-        
-        Bugs or feature requests are always appreciated! They can be submitted `here <https://github.com/aazuspan/wxee/issues>`_. 
-        
-        Code contributions are also welcome! Please open an `issue <https://github.com/aazuspan/wxee/issues>`_ to discuss implementation, 
-        then follow the steps below. Developer setup instructions can be found `in the docs <https://wxee.readthedocs.io/en/latest/contributing.html>`_.
-        
-        
-        
-        
-        
-Keywords: wxee,xarray,earth-engine
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Project-URL: Homepage, https://github.com/aazuspan/wxee
+Author-email: Aaron Zuspan <aazuspan@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: earth-engine,time-series,xarray
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: doc
+Requires-Python: >=3.8
+Requires-Dist: earthengine-api
+Requires-Dist: joblib
+Requires-Dist: rasterio
+Requires-Dist: requests
+Requires-Dist: rioxarray
+Requires-Dist: tqdm
+Requires-Dist: xarray
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: hvplot; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: matplotlib; extra == 'dev'
+Requires-Dist: mock; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: nbsphinx; extra == 'dev'
+Requires-Dist: netcdf4; extra == 'dev'
+Requires-Dist: plotly>=5.2.2; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: requests-mock; extra == 'dev'
+Requires-Dist: sphinx; extra == 'dev'
+Requires-Dist: sphinx-rtd-theme; extra == 'dev'
+Provides-Extra: doc
+Requires-Dist: nbsphinx; extra == 'doc'
+Requires-Dist: sphinx; extra == 'doc'
+Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
+Requires-Dist: hvplot; extra == 'test'
+Requires-Dist: matplotlib; extra == 'test'
+Requires-Dist: mock; extra == 'test'
+Requires-Dist: netcdf4; extra == 'test'
+Requires-Dist: plotly>=5.2.2; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: requests-mock; extra == 'test'
+Description-Content-Type: text/x-rst
+
+.. image:: https://raw.githubusercontent.com/aazuspan/wxee/main/docs/_static/wxee.png
+   :alt: wxee .-- -..-
+   :width: 200
+   :target: https://github.com/aazuspan/wxee
+
+|
+
+.. image:: https://img.shields.io/badge/Earth%20Engine%20API-Python-green
+   :alt: Earth Engine Python
+   :target: https://developers.google.com/earth-engine/tutorials/community/intro-to-python-api
+.. image:: https://img.shields.io/pypi/v/wxee
+   :alt: PyPI
+   :target: https://pypi.org/project/wxee/
+.. image:: https://img.shields.io/conda/vn/conda-forge/wxee.svg
+   :alt: conda-forge
+   :target: https://anaconda.org/conda-forge/wxee
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+   :alt: Open in Colab
+   :target: https://colab.research.google.com/github/aazuspan/wxee/blob/main/docs/examples/image_collection_to_xarray.ipynb
+.. image:: https://readthedocs.org/projects/wxee/badge/?version=latest&style=flat
+   :alt: Read the Docs
+   :target: https://wxee.readthedocs.io/en/latest/?badge=latest
+.. image:: https://github.com/aazuspan/wxee/actions/workflows/tests.yml/badge.svg
+   :alt: Build status
+   :target: https://github.com/aazuspan/wxee
+.. image:: https://codecov.io/gh/aazuspan/wxee/branch/main/graph/badge.svg?token=OeSeq4b7NF
+   :alt: Code coverage
+   :target: https://codecov.io/gh/aazuspan/wxee
+
+------------
+
+.. image:: https://raw.githubusercontent.com/aazuspan/wxee/main/docs/_static/demo_001.gif
+  :alt: Demo downloading weather data to xarray using wxee.
+
+
+What is wxee?
+-------------
+`wxee <https://github.com/aazuspan/wxee>`_ was built to make processing gridded, mesoscale time series data quick 
+and easy by integrating the data catalog and processing power of `Google Earth Engine <https://earthengine.google.com/>`_ with the 
+flexibility of `xarray <https://github.com/pydata/xarray>`_, with no complicated setup required. To accomplish this, wxee implements 
+convenient methods for data processing, aggregation, downloading, and ingestion.
+
+`wxee <https://github.com/aazuspan/wxee>`__ can be found in the `Earth Engine Developer Resources <https://developers.google.com/earth-engine/tutorials/community/developer-resources#python>`_!
+
+
+Features
+--------
+* Time series image collections to `xarray <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`__, `NetCDF <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`_, or `GeoTIFF <https://wxee.readthedocs.io/en/latest/examples/downloading_images_and_collections.html>`_ in one line of code
+* `Climatological anomalies <https://wxee.readthedocs.io/en/latest/examples/climatology_anomaly.html>`_ and temporal `aggregation <https://wxee.readthedocs.io/en/latest/examples/temporal_aggregation.html>`_, `interpolation <https://wxee.readthedocs.io/en/latest/examples/temporal_interpolation.html>`_, `smoothing <https://wxee.readthedocs.io/en/latest/generated/wxee.time_series.TimeSeries.rolling_time.html>`_, and `gap-filling <https://wxee.readthedocs.io/en/latest/generated/wxee.time_series.TimeSeries.fill_gaps.html>`_ in Earth Engine
+* `Color composite plots <https://wxee.readthedocs.io/en/latest/examples/color_composites.html>`_ from **xarray** datasets
+* Parallel processing for fast downloads
+
+
+To see some of the capabilities of wxee and try it yourself, check out the interactive notebooks `here <https://wxee.readthedocs.io/en/latest/examples.html>`__!
+
+Install
+------------
+
+Pip
+~~~
+
+.. code-block:: bash
+
+   pip install wxee
+
+Conda
+~~~~~
+
+.. code-block:: bash
+
+    conda install -c conda-forge wxee
+
+From Source
+~~~~~~~~~~~
+
+.. code-block:: bash
+
+   git clone https://github.com/aazuspan/wxee
+   cd wxee
+   make install
+
+
+Quickstart
+----------
+
+Setup
+~~~~~
+Once you have access to Google Earth Engine, just import and initialize :code:`ee` and :code:`wxee`.
+
+.. code-block:: python
+   
+   import ee
+   import wxee
+
+   wxee.Initialize()
+
+
+Download Images
+~~~~~~~~~~~~~~~
+
+Download and conversion methods are extended to :code:`ee.Image` and :code:`ee.ImageCollection` using the 
+:code:`wx` accessor. Just :code:`import wxee` and use the :code:`wx` accessor.
+
+xarray
+^^^^^^
+
+.. code-block:: python
+
+   ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").wx.to_xarray()
+
+NetCDF
+^^^^^^
+
+.. code-block:: python
+
+   ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").wx.to_xarray(path="data/gridmet.nc")
+
+GeoTIFF
+^^^^^^^
+
+.. code-block:: python
+
+   ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").wx.to_tif()
+
+
+Create a Time Series
+~~~~~~~~~~~~~~~~~~~~
+
+Additional methods for processing image collections in the time dimension are available through the :code:`TimeSeries` subclass.
+A :code:`TimeSeries` can be created from an existing :code:`ee.ImageCollection`...
+
+.. code-block:: python
+
+   col = ee.ImageCollection("IDAHO_EPSCOR/GRIDMET")
+   ts = col.wx.to_time_series()
+
+Or instantiated directly just like you would an :code:`ee.ImageCollection`!
+
+.. code-block:: python
+
+   ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
+
+
+Aggregate Daily Data
+~~~~~~~~~~~~~~~~~~~~
+
+Many weather datasets are in daily or hourly resolution. These can be aggregated to coarser resolutions using the :code:`aggregate_time`
+method of the :code:`TimeSeries` class.
+
+.. code-block:: python
+
+   ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
+   monthly_max = ts.aggregate_time(frequency="month", reducer=ee.Reducer.max())
+
+Calculate Climatological Means
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Long-term climatological means can be calculated using the :code:`climatology_mean` method of the :code:`TimeSeries` class.
+
+.. code-block:: python
+
+   ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
+   mean_clim = ts.climatology_mean(frequency="month")
+
+Contribute
+----------
+
+Bugs or feature requests are always appreciated! They can be submitted `here <https://github.com/aazuspan/wxee/issues>`__. 
+
+Code contributions are also welcome! Please open an `issue <https://github.com/aazuspan/wxee/issues>`__ to discuss implementation, 
+then follow the steps below. Developer setup instructions can be found `in the docs <https://wxee.readthedocs.io/en/latest/contributing.html>`__.
+
+
```

### Comparing `wxee-0.3.3/README.rst` & `wxee-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 What is wxee?
 -------------
 `wxee <https://github.com/aazuspan/wxee>`_ was built to make processing gridded, mesoscale time series data quick 
 and easy by integrating the data catalog and processing power of `Google Earth Engine <https://earthengine.google.com/>`_ with the 
 flexibility of `xarray <https://github.com/pydata/xarray>`_, with no complicated setup required. To accomplish this, wxee implements 
 convenient methods for data processing, aggregation, downloading, and ingestion.
 
-`wxee <https://github.com/aazuspan/wxee>`_ can be found in the `Earth Engine Developer Resources <https://developers.google.com/earth-engine/tutorials/community/developer-resources#python>`_!
+`wxee <https://github.com/aazuspan/wxee>`__ can be found in the `Earth Engine Developer Resources <https://developers.google.com/earth-engine/tutorials/community/developer-resources#python>`_!
 
 
 Features
 --------
-* Time series image collections to `xarray <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`_, `NetCDF <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`_, or `GeoTIFF <https://wxee.readthedocs.io/en/latest/examples/downloading_images_and_collections.html>`_ in one line of code
+* Time series image collections to `xarray <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`__, `NetCDF <https://wxee.readthedocs.io/en/latest/examples/image_collection_to_xarray.html>`_, or `GeoTIFF <https://wxee.readthedocs.io/en/latest/examples/downloading_images_and_collections.html>`_ in one line of code
 * `Climatological anomalies <https://wxee.readthedocs.io/en/latest/examples/climatology_anomaly.html>`_ and temporal `aggregation <https://wxee.readthedocs.io/en/latest/examples/temporal_aggregation.html>`_, `interpolation <https://wxee.readthedocs.io/en/latest/examples/temporal_interpolation.html>`_, `smoothing <https://wxee.readthedocs.io/en/latest/generated/wxee.time_series.TimeSeries.rolling_time.html>`_, and `gap-filling <https://wxee.readthedocs.io/en/latest/generated/wxee.time_series.TimeSeries.fill_gaps.html>`_ in Earth Engine
 * `Color composite plots <https://wxee.readthedocs.io/en/latest/examples/color_composites.html>`_ from **xarray** datasets
 * Parallel processing for fast downloads
 
 
-To see some of the capabilities of wxee and try it yourself, check out the interactive notebooks `here <https://wxee.readthedocs.io/en/latest/examples.html>`_!
+To see some of the capabilities of wxee and try it yourself, check out the interactive notebooks `here <https://wxee.readthedocs.io/en/latest/examples.html>`__!
 
 Install
 ------------
 
 Pip
 ~~~
 
@@ -161,13 +161,13 @@
 
    ts = wxee.TimeSeries("IDAHO_EPSCOR/GRIDMET")
    mean_clim = ts.climatology_mean(frequency="month")
 
 Contribute
 ----------
 
-Bugs or feature requests are always appreciated! They can be submitted `here <https://github.com/aazuspan/wxee/issues>`_. 
+Bugs or feature requests are always appreciated! They can be submitted `here <https://github.com/aazuspan/wxee/issues>`__. 
 
-Code contributions are also welcome! Please open an `issue <https://github.com/aazuspan/wxee/issues>`_ to discuss implementation, 
-then follow the steps below. Developer setup instructions can be found `in the docs <https://wxee.readthedocs.io/en/latest/contributing.html>`_.
+Code contributions are also welcome! Please open an `issue <https://github.com/aazuspan/wxee/issues>`__ to discuss implementation, 
+then follow the steps below. Developer setup instructions can be found `in the docs <https://wxee.readthedocs.io/en/latest/contributing.html>`__.
```

### Comparing `wxee-0.3.3/wxee/accessors.py` & `wxee-0.4.0/wxee/accessors.py`

 * *Files identical despite different names*

### Comparing `wxee-0.3.3/wxee/climatology.py` & `wxee-0.4.0/wxee/climatology.py`

 * *Files identical despite different names*

### Comparing `wxee-0.3.3/wxee/collection.py` & `wxee-0.4.0/wxee/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import tempfile
+import warnings
 from typing import List, Optional
 
 import ee  # type: ignore
 import xarray as xr
 from joblib import Parallel, delayed  # type: ignore
 from tqdm.auto import tqdm  # type: ignore
 
@@ -70,16 +71,14 @@
     ) -> xr.Dataset:
         """Convert an image collection to an xarray.Dataset. The :code:`system:time_start` property of each image in the
         collection is used to arrange the time dimension, and each image variable is loaded as a separate array in
         the dataset.
 
         Parameters
         ----------
-        path : str, optional
-            The path to save the dataset to as a NetCDF. If none is given, the dataset will be stored in memory.
         region : ee.Geometry, optional
             The region to download the images within. If none is provided, the :code:`geometry` of the image collection
             will be used. If geometry varies between images in the collection, the region will encompass all images
             which may lead to very large arrays and download limits.
         scale : int, optional
             The scale to download the array at in the CRS units. If none is provided, the :code:`projection.nominalScale`
             of the images will be used.
@@ -111,15 +110,14 @@
 
         Examples
         --------
         >>> col = ee.ImageCollection("IDAHO_EPSCOR/GRIDMET").filterDate("2020-09-08", "2020-09-15")
         >>> col.wx.to_xarray(scale=40000, crs="EPSG:5070", nodata=-9999)
         """
         with tempfile.TemporaryDirectory(prefix=constants.TMP_PREFIX) as tmp:
-
             files = self._obj.wx.to_tif(
                 out_dir=tmp,
                 region=region,
                 scale=scale,
                 crs=crs,
                 file_per_band=True,
                 masked=masked,
@@ -128,14 +126,19 @@
                 progress=progress,
                 max_attempts=max_attempts,
             )
 
             ds = _dataset_from_files(files, masked, nodata)
 
         if path:
+            msg = (
+                "The path argument is deprecated and will be removed in a future "
+                "release. Use the `xarray.Dataset.to_netcdf` method instead."
+            )
+            warnings.warn(category=DeprecationWarning, message=msg)
             ds.to_netcdf(path, mode="w")
 
         return ds
 
     def to_tif(
         self,
         out_dir: str = ".",
```

### Comparing `wxee-0.3.3/wxee/image.py` & `wxee-0.4.0/wxee/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tempfile
 import warnings
 from typing import List, Optional
 
 import ee  # type: ignore
 import rasterio  # type: ignore
 import xarray as xr
-from urllib3.exceptions import ProtocolError  # type: ignore
+from urllib3.exceptions import ProtocolError
 
 from wxee import constants
 from wxee.accessors import wx_accessor
 from wxee.exceptions import DownloadError, MissingPropertyError
 from wxee.utils import (
     _dataset_from_files,
     _download_url,
@@ -37,16 +37,14 @@
         max_attempts: int = 10,
     ) -> xr.Dataset:
         """Convert an image to an xarray.Dataset. The :code:`system:time_start` property of the image is used to set the
         time dimension, and each image variable is loaded as a separate array in the dataset.
 
         Parameters
         ----------
-        path : str, optional
-            The path to save the dataset to as a NetCDF. If none is given, the dataset will be stored in memory.
         region : ee.Geometry, optional
             The region to download the image within. If none is provided, the :code:`geometry` of the image will be used.
         scale : int, optional
             The scale to download the array at in the CRS units. If none is provided, the :code:`projection.nominalScale`
             of the image will be used.
         crs : str, default "EPSG:4326"
             The coordinate reference system to download the array in.
@@ -88,14 +86,19 @@
                 max_attempts=max_attempts,
                 progress=progress,
             )
 
             ds = _dataset_from_files(files, masked, nodata)
 
         if path:
+            msg = (
+                "The path argument is deprecated and will be removed in a future "
+                "release. Use the `xarray.Dataset.to_netcdf` method instead."
+            )
+            warnings.warn(category=DeprecationWarning, message=msg)
             ds.to_netcdf(path, mode="w")
 
         return ds
 
     def to_tif(
         self,
         out_dir: str = ".",
```

### Comparing `wxee-0.3.3/wxee/interpolation.py` & `wxee-0.4.0/wxee/interpolation.py`

 * *Files identical despite different names*

### Comparing `wxee-0.3.3/wxee/params.py` & `wxee-0.4.0/wxee/params.py`

 * *Files identical despite different names*

### Comparing `wxee-0.3.3/wxee/time_series.py` & `wxee-0.4.0/wxee/time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 import ee  # type: ignore
 import pandas as pd  # type: ignore
-import plotly.express as px  # type: ignore
-import plotly.graph_objects as go  # type: ignore
 
 from wxee.climatology import Climatology, ClimatologyFrequencyEnum
 from wxee.exceptions import MissingPropertyError
 from wxee.interpolation import InterpolationMethodEnum
 from wxee.params import ParamEnum
 from wxee.utils import _millis_to_datetime, _normalize
 
+if TYPE_CHECKING:
+    import plotly.graph_objects as go  # type: ignore
+
 
 class TimeFrequencyEnum(ParamEnum):
     """Parameters defining generic time frequnecies."""
 
     year = "year"
     month = "month"
     week = "week"
@@ -166,22 +167,30 @@
             df_dict[prop] = vals
 
         collection_id = self.get("system:id").getInfo()
         df = pd.DataFrame.from_dict(df_dict)
         df.index.id = collection_id
         return df
 
-    def timeline(self) -> go.Figure:  # pragma: no cover
+    def timeline(self) -> "go.Figure":  # pragma: no cover
         """Generate an interactive plot showing the acquisition time of each image in the time series.
 
         Returns
         -------
         go.Figure
             A Plotly graph object interactive plot showing the acquisition time of each image in the time series.
         """
+        try:
+            import plotly.express as px  # type: ignore
+        except ImportError:
+            raise ImportError(
+                "The `plotly` package is required for this feature. "
+                "Please install it with `pip install plotly` and try again."
+            ) from None
+
         df = self.dataframe(props=["system:id", "system:time_start"])
         df["y"] = 0
 
         fig = px.line(
             df,
             x="system:time_start",
             y="y",
```

### Comparing `wxee-0.3.3/wxee/utils.py` & `wxee-0.4.0/wxee/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from typing import Any, List, Tuple, Union
 from zipfile import ZipFile
 
 import ee  # type: ignore
 import joblib  # type: ignore
 import rasterio  # type: ignore
 import requests
+import rioxarray  # type: ignore
 import xarray as xr
 from requests.adapters import HTTPAdapter
 from tqdm.auto import tqdm  # type: ignore
-from urllib3.util.retry import Retry  # type: ignore
+from urllib3.util.retry import Retry
 
 
 def Initialize(**kwargs: Any) -> None:
     """Initialize Earth Engine using the high-volume endpoint designed for automated requests.
 
     Parameters
     ----------
@@ -153,15 +154,15 @@
 
 
 def _dataarray_from_file(file: str, masked: bool, nodata: int) -> xr.DataArray:
     """Create an xarray.DataArray from a single file by parsing datetimes and variables from the file name.
 
     The file name must follow the format "{dimension}.{coordinate}.{variable}.{extension}".
     """
-    da = xr.open_rasterio(file)
+    da = rioxarray.open_rasterio(file)
     dim, coord, var = _parse_filename(file)
 
     da = da.expand_dims({dim: [coord]}).rename(var).squeeze("band").drop_vars("band")
 
     # Mask the nodata values. This will convert int datasets to float.
     if masked:
         da = da.where(da != nodata)
```

### Comparing `wxee-0.3.3/wxee/xarray.py` & `wxee-0.4.0/wxee/xarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,47 +61,49 @@
         >>> ds.wx.rgb(bands=["B4", "B3", "B2"], stretch=0.85, col_wrap=4)
 
         Generate an interactive plot using a near-infrared false color composite. The aspect argument will be passed
         to the plotting function.
 
         >>> ds.wx.rgb(bands=["B8", "B4", "B3"], stretch=0.85, interactive=True, aspect=1.2)
         """
-        if bands:
+        if bands is not None:
             if len(bands) != 3:
                 raise ValueError(f"Bands must be a list with exactly 3 names.")
         else:
-            bands = list(self._obj.var())[:3]
+            bands = list(self._obj.var())[:3]  # type: ignore
 
             # Raise a different error if the bands were identified implicitly to avoid confusion
-            if len(bands) != 3:
+            if len(bands) != 3:  # type: ignore
                 raise ValueError(
                     f"The Dataset must contain at least 3 data variables for RGB plotting."
                 )
 
         da = self._obj[bands].to_array(name="rgb")
 
         da = da.wx.normalize(stretch)
 
         if interactive:
             try:
                 import hvplot.xarray  # type: ignore
             except ImportError:
                 raise ImportError(
                     "The `hvplot` package is required for interactive plots. Run `pip install hvplot`."
-                )
-
-            default_kwargs = {"widget_location": "bottom", "widget_type": "scrubber"}
-
-            for k, v in default_kwargs.items():
-                if k not in kwargs:
-                    kwargs[k] = v
+                ) from None
 
-            return da.hvplot.rgb(x="x", y="y", bands="variable", **kwargs)
+            default_kwargs = {
+                "groupby": "time",
+                "widget_location": "bottom",
+                "widget_type": "scrubber",
+            }
+            return da.hvplot.rgb(
+                x="x", y="y", bands="variable", **{**default_kwargs, **kwargs}
+            )
 
-        return da.plot.imshow(col="time", **kwargs)
+        default_kwargs = {"col": "time"}
+        return da.plot.imshow(**{**default_kwargs, **kwargs})
 
 
 @xr.register_dataarray_accessor("wx")
 class DataArrayAccessor:
     def __init__(self, obj: xr.DataArray):
         self._obj = obj
```

