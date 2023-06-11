# Comparing `tmp/presentpy-0.2.5.tar.gz` & `tmp/presentpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "presentpy-0.2.5.tar", max compression
+gzip compressed data, was "presentpy-0.3.0.tar", max compression
```

## Comparing `presentpy-0.2.5.tar` & `presentpy-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2022-08-07 13:28:24.731194 presentpy-0.2.5/presentpy/__init__.py
--rw-r--r--   0        0        0      460 2022-08-07 13:28:24.731194 presentpy-0.2.5/presentpy/__main__.py
--rw-r--r--   0        0        0     3035 2022-08-07 13:28:24.731194 presentpy-0.2.5/presentpy/code.py
--rw-r--r--   0        0        0      204 2022-08-07 13:28:24.731194 presentpy-0.2.5/presentpy/code_cell_config.py
--rw-r--r--   0        0        0     2294 2022-08-07 13:28:24.731194 presentpy-0.2.5/presentpy/parser.py
--rw-r--r--   0        0        0     3084 2022-08-07 13:28:24.731194 presentpy-0.2.5/presentpy/slides.py
--rw-r--r--   0        0        0    24289 2022-08-07 13:29:27.495474 presentpy-0.2.5/presentpy/templates/Blank-dark.pptx
--rw-r--r--   0        0        0    24409 2022-08-07 13:29:27.495474 presentpy-0.2.5/presentpy/templates/Blank-light.pptx
--rw-r--r--   0        0        0      989 2022-08-07 13:28:24.731194 presentpy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      903 2022-08-07 13:29:28.053710 presentpy-0.2.5/setup.py
--rw-r--r--   0        0        0      724 2022-08-07 13:29:28.054009 presentpy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      879 2023-06-11 20:09:43.044608 presentpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-06-10 20:51:05.738949 presentpy-0.3.0/readme.md
+-rw-r--r--   0        0        0       22 2023-06-11 20:09:43.045296 presentpy-0.3.0/src/presentpy/__init__.py
+-rw-r--r--   0        0        0      644 2023-06-11 20:09:43.046584 presentpy-0.3.0/src/presentpy/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-10 21:37:19.062706 presentpy-0.3.0/src/presentpy/code_slide.py
+-rw-r--r--   0        0        0     1855 2023-06-11 20:09:43.046780 presentpy-0.3.0/src/presentpy/code_slide_source.py
+-rw-r--r--   0        0        0      564 2023-06-11 20:09:43.046960 presentpy-0.3.0/src/presentpy/notebook_processor.py
+-rw-r--r--   0        0        0   131544 2023-06-11 20:24:45.178026 presentpy-0.3.0/src/presentpy/slide_templates/Template-Light.pptx
+-rw-r--r--   0        0        0        0 2023-06-11 20:09:43.055767 presentpy-0.3.0/src/presentpy/writers/__init__.py
+-rw-r--r--   0        0        0     3673 2023-06-11 20:09:43.055929 presentpy-0.3.0/src/presentpy/writers/pptx_writer.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 presentpy-0.3.0/PKG-INFO
```

### Comparing `presentpy-0.2.5/pyproject.toml` & `presentpy-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 [tool.poetry]
 name = "presentpy"
-version = "0.2.5"
-description = "Create presentations from Jupyter Notebooks"
+version = "0.3.0"
+description = "Create slides from Jupyter Notebooks"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
-include = ["presentpy/templates/*.pptx"]
+readme = "readme.md"
+include = ["src/presentpy/**/*"]
 
 [tool.poetry.scripts]
-presentpy = 'presentpy.__main__:process'
+presentpy = "presentpy.__main__:run_presentpy"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-nbconvert = "^6.5.0"
-mistletoe = "^0.8.2"
-python-pptx = "^0.6.21"
-Pygments = "^2.12.0"
 click = "^8.1.3"
+nbconvert = "^7.4.0"
+pygments = "^2.15.1"
+python = "^3.8"
+python-pptx = "^0.6.21"
 
-[tool.poetry.dev-dependencies]
-jupyter = "^1.0.0"
-jupyterlab = "^3.4.4"
-isort = "^5.10.1"
-black = "^22.6.0"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 bump2version = "^1.0.1"
+isort = "^5.12.0"
+pytest = "^7.3.2"
+ruff = "^0.0.272"
+
+[tool.poetry.group.juptyter.dependencies]
+jupyter = "^1.0.0"
+jupyterlab = "^4.0.2"
+
+[tool.ruff]
+select = ["E", "F", "I","C90", "N"]
+ignore = []
+line-length = 120
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
-skip_glob = [".ipynb_checkpoints", "dist"]
-# Structure
-default_section = "THIRDPARTY"
-known_first_party = "presentpy"
-# Import Style
-line_length = 120
-force_grid_wrap = false
-use_parentheses = true
-include_trailing_comma = true
-combine_as_imports = true
-multi_line_output = 3
+profile = "black"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `presentpy-0.2.5/PKG-INFO` & `presentpy-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: presentpy
-Version: 0.2.5
-Summary: Create presentations from Jupyter Notebooks
+Version: 0.3.0
+Summary: Create slides from Jupyter Notebooks
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pygments (>=2.12.0,<3.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: mistletoe (>=0.8.2,<0.9.0)
-Requires-Dist: nbconvert (>=6.5.0,<7.0.0)
+Requires-Dist: nbconvert (>=7.4.0,<8.0.0)
+Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: python-pptx (>=0.6.21,<0.7.0)
+Description-Content-Type: text/markdown
+
+PresentPy
+=========
+
+Create slides from Jupyter Notebooks
+
```

