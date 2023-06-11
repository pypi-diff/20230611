# Comparing `tmp/imfdatapy-0.1.5.tar.gz` & `tmp/imfdatapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfdatapy-0.1.5.tar", max compression
+gzip compressed data, was "imfdatapy-1.0.0.tar", max compression
```

## Comparing `imfdatapy-0.1.5.tar` & `imfdatapy-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0      597 2022-11-25 20:06:40.703244 imfdatapy-0.1.5/LICENSE
--rw-r--r--   0        0        0     1747 2022-11-26 13:44:50.762985 imfdatapy-0.1.5/README.md
--rw-r--r--   0        0        0      616 2022-11-26 14:11:08.516731 imfdatapy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       25 2022-11-26 13:45:57.430923 imfdatapy-0.1.5/src/imfdatapy/__inti__.py
--rw-r--r--   0        0        0    19160 2022-11-26 14:10:44.518285 imfdatapy-0.1.5/src/imfdatapy/imf.py
--rw-r--r--   0        0        0      451 2022-11-26 13:49:49.131183 imfdatapy-0.1.5/src/imfdatapy/logging.conf
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 imfdatapy-0.1.5/setup.py
--rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 imfdatapy-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0      594 2022-11-27 14:20:15.392057 imfdatapy-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1747 2023-06-02 22:04:02.014967 imfdatapy-1.0.0/README.md
+-rw-r--r--   0        0        0      650 2023-06-02 22:25:01.350361 imfdatapy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-06-02 22:00:02.348989 imfdatapy-1.0.0/src/imfdatapy/__inti__.py
+-rw-r--r--   0        0        0    48494 2023-06-02 22:01:03.626563 imfdatapy-1.0.0/src/imfdatapy/imf.py
+-rw-r--r--   0        0        0     1536 2023-06-02 22:01:03.637718 imfdatapy-1.0.0/src/imfdatapy/imf_log.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 imfdatapy-1.0.0/setup.py
+-rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 imfdatapy-1.0.0/PKG-INFO
```

### Comparing `imfdatapy-0.1.5/LICENSE` & `imfdatapy-1.0.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache License, v2.0
 
-Copyright (c) 2022, Irina Klein, Sou-Cheng T. Choi
+Copyright (c) 2022, Irina Klein, Sou-Cheng Choi
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `imfdatapy-0.1.5/README.md` & `imfdatapy-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 bop = BOP(search_terms=["current account, total, credit"], countries=["US"], period='Q',
 start_date="2000", end_date="2022")
 df = bop.download_data()
 ```
 
 ## Contributing
 
-Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a [Code of Conduct](CONDUCT.md). By contributing to this project, you agree to abide by its terms.
+Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a [Code of Conduct](conduct.md). By contributing to this project, you agree to abide by its terms.
 
 ## License
 
 `imfdatapy` was created by Sou-Cheng T. Choi and Irina Klein, Illinois Institute of Technology. It is licensed under the terms of the Apache License, v2.0.
 
 With regard to the terms for using IMF data, please refer to IMF's [Copyright and Usage](https://www.imf.org/external/terms.htm) and pay special attention to the 
 section _SPECIAL TERMS AND CONDITIONS PERTAINING TO THE USE OF DATA_.
```

### Comparing `imfdatapy-0.1.5/pyproject.toml` & `imfdatapy-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imfdatapy"
-version = "0.1.5"
+version = "1.0.0"
 description = "A package for data discovery and extraction from the IMF!"
 authors = ["Irina Klein, Sou-Cheng T. Choi"]
 license = "Apache v2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.15, <3.11"
@@ -12,14 +12,15 @@
 pandas = ">=1.3.5"
 requests = ">=2.23.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
-myst-nb = {version = "^0.17.1", python = "^3.7.15"}
-sphinx-autoapi = "^2.0.0"
+myst-nb = {version = "^0.16", python = "^3.7.15"}
+sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.1.1"
+python-semantic-release = "^7.34.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `imfdatapy-0.1.5/setup.py` & `imfdatapy-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.21.6', 'pandas>=1.3.5', 'requests>=2.23.0']
 
 setup_kwargs = {
     'name': 'imfdatapy',
-    'version': '0.1.5',
+    'version': '1.0.0',
     'description': 'A package for data discovery and extraction from the IMF!',
-    'long_description': '# imfdatapy\n\nA package for data discovery and extraction from the International Monetary Fund (IMF)!\nThis repository contains Python source code and Jupyter notebooks with examples on how to extract data from the IMF.\n\n## Installation\n\n```bash\n    $ pip install imfdatapy\n```\n\n## Usage\n\n`imfdatapy` can be used to search through and extract data as follows. The examples below show how to search through the IFS (International Financial Statistics) and BOP (Balance of Payments) using ```serach_terms``` and download all the data with matching economic indicator names.\n\n```python\nfrom imfdatapy.imf import *\nifs = IFS(search_terms=["gross domestic product, real"], countries=["US"], period=\'Q\',\nstart_date="2000", end_date="2022")\ndf = ifs.download_data()\n\nbop = BOP(search_terms=["current account, total, credit"], countries=["US"], period=\'Q\',\nstart_date="2000", end_date="2022")\ndf = bop.download_data()\n```\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a [Code of Conduct](CONDUCT.md). By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`imfdatapy` was created by Sou-Cheng T. Choi and Irina Klein, Illinois Institute of Technology. It is licensed under the terms of the Apache License, v2.0.\n\nWith regard to the terms for using IMF data, please refer to IMF\'s [Copyright and Usage](https://www.imf.org/external/terms.htm) and pay special attention to the \nsection _SPECIAL TERMS AND CONDITIONS PERTAINING TO THE USE OF DATA_.  \n\n\n## Credits\n\n`imfdatapy` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).',
+    'long_description': '# imfdatapy\n\nA package for data discovery and extraction from the International Monetary Fund (IMF)!\nThis repository contains Python source code and Jupyter notebooks with examples on how to extract data from the IMF.\n\n## Installation\n\n```bash\n    $ pip install imfdatapy\n```\n\n## Usage\n\n`imfdatapy` can be used to search through and extract data as follows. The examples below show how to search through the IFS (International Financial Statistics) and BOP (Balance of Payments) using ```serach_terms``` and download all the data with matching economic indicator names.\n\n```python\nfrom imfdatapy.imf import *\nifs = IFS(search_terms=["gross domestic product, real"], countries=["US"], period=\'Q\',\nstart_date="2000", end_date="2022")\ndf = ifs.download_data()\n\nbop = BOP(search_terms=["current account, total, credit"], countries=["US"], period=\'Q\',\nstart_date="2000", end_date="2022")\ndf = bop.download_data()\n```\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a [Code of Conduct](conduct.md). By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`imfdatapy` was created by Sou-Cheng T. Choi and Irina Klein, Illinois Institute of Technology. It is licensed under the terms of the Apache License, v2.0.\n\nWith regard to the terms for using IMF data, please refer to IMF\'s [Copyright and Usage](https://www.imf.org/external/terms.htm) and pay special attention to the \nsection _SPECIAL TERMS AND CONDITIONS PERTAINING TO THE USE OF DATA_.  \n\n\n## Credits\n\n`imfdatapy` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).',
     'author': 'Irina Klein, Sou-Cheng T. Choi',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `imfdatapy-0.1.5/PKG-INFO` & `imfdatapy-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imfdatapy
-Version: 0.1.5
+Version: 1.0.0
 Summary: A package for data discovery and extraction from the IMF!
 License: Apache v2.0
 Author: Irina Klein, Sou-Cheng T. Choi
 Requires-Python: >=3.7.15,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -39,15 +39,15 @@
 bop = BOP(search_terms=["current account, total, credit"], countries=["US"], period='Q',
 start_date="2000", end_date="2022")
 df = bop.download_data()
 ```
 
 ## Contributing
 
-Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a [Code of Conduct](CONDUCT.md). By contributing to this project, you agree to abide by its terms.
+Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a [Code of Conduct](conduct.md). By contributing to this project, you agree to abide by its terms.
 
 ## License
 
 `imfdatapy` was created by Sou-Cheng T. Choi and Irina Klein, Illinois Institute of Technology. It is licensed under the terms of the Apache License, v2.0.
 
 With regard to the terms for using IMF data, please refer to IMF's [Copyright and Usage](https://www.imf.org/external/terms.htm) and pay special attention to the 
 section _SPECIAL TERMS AND CONDITIONS PERTAINING TO THE USE OF DATA_.
```

