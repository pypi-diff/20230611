# Comparing `tmp/mdbook-pdf-outline-0.1.3.tar.gz` & `tmp/mdbook-pdf-outline-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdbook-pdf-outline-0.1.3.tar", last modified: Mon Mar 27 15:56:46 2023, max compression
+gzip compressed data, was "mdbook-pdf-outline-0.1.4.tar", last modified: Sun Jun 11 20:35:04 2023, max compression
```

## Comparing `mdbook-pdf-outline-0.1.3.tar` & `mdbook-pdf-outline-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:56:46.917054 mdbook-pdf-outline-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-27 15:56:28.000000 mdbook-pdf-outline-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-03-27 15:56:46.917054 mdbook-pdf-outline-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-03-27 15:56:28.000000 mdbook-pdf-outline-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:56:46.917054 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 15:56:28.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5550 2023-03-27 15:56:28.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline/mdbook_pdf_outline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:56:46.917054 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-03-27 15:56:46.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-27 15:56:46.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:56:46.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-27 15:56:46.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 15:56:46.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-27 15:56:46.000000 mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-27 15:56:28.000000 mdbook-pdf-outline-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 15:56:46.917054 mdbook-pdf-outline-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-03-27 15:56:28.000000 mdbook-pdf-outline-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:35:04.431235 mdbook-pdf-outline-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-11 20:34:46.000000 mdbook-pdf-outline-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-11 20:35:04.431235 mdbook-pdf-outline-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-11 20:34:46.000000 mdbook-pdf-outline-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:35:04.431235 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:34:46.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6932 2023-06-11 20:34:46.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline/mdbook_pdf_outline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:35:04.431235 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-11 20:35:04.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-11 20:35:04.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:35:04.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-11 20:35:04.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 20:35:04.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 20:35:04.000000 mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 20:34:46.000000 mdbook-pdf-outline-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:35:04.431235 mdbook-pdf-outline-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2122 2023-06-11 20:34:46.000000 mdbook-pdf-outline-0.1.4/setup.py
```

### Comparing `mdbook-pdf-outline-0.1.3/LICENSE` & `mdbook-pdf-outline-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mdbook-pdf-outline-0.1.3/PKG-INFO` & `mdbook-pdf-outline-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: mdbook-pdf-outline
-Version: 0.1.3
-Summary: Tool for generating outlines for PDF files generated by mdbook-pdf.
-Home-page: https://github.com/HollowMan6/mdbook-pdf
-Author: Hollow Man (Domain Address)
-Author-email: hollowman@opensuse.org
-License: GPL-3.0-or-later
-Project-URL: Bug Tracker, https://github.com/HollowMan6/mdbook-pdf/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # mdbook-pdf
 [![](https://dockeri.co/image/hollowman6/mdbook-pdf)](https://hub.docker.com/r/hollowman6/mdbook-pdf)
 
 [![last-commit](https://img.shields.io/github/last-commit/HollowMan6/mdbook-pdf)](https://github.com/HollowMan6/mdbook-pdf/graphs/commit-activity)
 [![release-date](https://img.shields.io/github/release-date/HollowMan6/mdbook-pdf)](https://github.com/HollowMan6/mdbook-pdf/releases)
 [![Crate](https://img.shields.io/crates/v/mdbook-pdf.svg)](https://crates.io/crates/mdbook-pdf)
 ![mdbook-pdf build](https://github.com/HollowMan6/mdbook-pdf/workflows/mdbook-pdf%20build/badge.svg)
@@ -79,20 +64,26 @@
 
 [output.pdf]
 ```
 
 Finally you can build your book and get the PDF file with `mdbook build` command, your PDF file will be available at `book/pdf/output.pdf`.
 
 ## Run with Docker
-You can also use this [docker image](https://hub.docker.com/r/hollowman6/mdbook-pdf) if your book doesn't have dependencies other than mdBook.
+You can also use this [docker image](https://hub.docker.com/r/hollowman6/mdbook-pdf).
 
 ```bash
 docker run --rm -v /path/to/book:/book hollowman6/mdbook-pdf
 ```
 
+If your book have other Rust dependencies, you can install them on your local machine (if using Linux), or if you are not using Linux, download the Linux executables of corresponding architecture to a dir, replace `~/.cargo/bin` with your path.
+
+```bash
+docker run --rm -v /path/to/book:/book -v ~/.cargo/bin:/mdbook hollowman6/mdbook-pdf
+```
+
 ## Configuration
 Support customize PDF paper orientation, scale of the webpage rendering, paper width and height, page margins, generated PDF page ranges, whether to display header and footer as well as customize their formats, and more.
 
 Check [book.toml](https://github.com/HollowMan6/mdbook-pdf/blob/main/test_doc/book.toml#L10-L36) and comments for details for the available configurations of `[output.pdf]`.
 
 ## Common Issues
 1. Support for Firefox in `mdbook-pdf`!
@@ -105,15 +96,15 @@
 
 If you have relative links that link outside the book, please provide the [static hosting site URL](https://github.com/HollowMan6/mdbook-pdf/blob/main/test_doc/book.toml#L17-L18) for it to get fixed.
 
 3. Can you add the bookmark to the PDF reflecting the Table of Contents, just like what [wkhtmltopdf](https://wkhtmltopdf.org/) supported?
 
 This should be realized by Chromium, and an issue has already been filed for this [here](https://bugs.chromium.org/p/chromium/issues/detail?id=781797).
 
-Initial support for the bookmark/outline of the PDF file has already been available ([mdbook-pdf-outline](https://pypi.org/project/mdbook-pdf-outline/)). It is written in Python and is another backend for `mdbook` and should be used with `mdbook-pdf` and ***the [mdbook version](https://github.com/rust-lang/mdBook/pull/1738) mentioned in Common Issues 2 for fixing the broken links in `print.html`***.
+Initial support for the bookmark/outline of the PDF file has already been available ([mdbook-pdf-outline](https://pypi.org/project/mdbook-pdf-outline/)). It is written in Python and is another backend for `mdbook` and should be used with `mdbook-pdf` and ***the [mdbook version](https://github.com/rust-lang/mdBook/pull/1738) mentioned in Common Issues 2 (by `cargo install --git https://github.com/HollowMan6/mdBook mdbook` instead) for fixing the broken links in `print.html`***.
 
 You can install this backend by `pip install mdbook-pdf-outline`.
 
 Remember to put the following to ***the end of*** your `book.toml`, ***after [output.pdf]***:
 
 ```toml
 [output.pdf-outline]
```

### Comparing `mdbook-pdf-outline-0.1.3/README.md` & `mdbook-pdf-outline-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mdbook-pdf-outline
+Version: 0.1.4
+Summary: Tool for generating outlines for PDF files generated by mdbook-pdf.
+Home-page: https://github.com/HollowMan6/mdbook-pdf
+Author: Hollow Man (Domain Address)
+Author-email: hollowman@opensuse.org
+License: GPL-3.0-or-later
+Project-URL: Bug Tracker, https://github.com/HollowMan6/mdbook-pdf/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mdbook-pdf
 [![](https://dockeri.co/image/hollowman6/mdbook-pdf)](https://hub.docker.com/r/hollowman6/mdbook-pdf)
 
 [![last-commit](https://img.shields.io/github/last-commit/HollowMan6/mdbook-pdf)](https://github.com/HollowMan6/mdbook-pdf/graphs/commit-activity)
 [![release-date](https://img.shields.io/github/release-date/HollowMan6/mdbook-pdf)](https://github.com/HollowMan6/mdbook-pdf/releases)
 [![Crate](https://img.shields.io/crates/v/mdbook-pdf.svg)](https://crates.io/crates/mdbook-pdf)
 ![mdbook-pdf build](https://github.com/HollowMan6/mdbook-pdf/workflows/mdbook-pdf%20build/badge.svg)
@@ -64,20 +79,26 @@
 
 [output.pdf]
 ```
 
 Finally you can build your book and get the PDF file with `mdbook build` command, your PDF file will be available at `book/pdf/output.pdf`.
 
 ## Run with Docker
-You can also use this [docker image](https://hub.docker.com/r/hollowman6/mdbook-pdf) if your book doesn't have dependencies other than mdBook.
+You can also use this [docker image](https://hub.docker.com/r/hollowman6/mdbook-pdf).
 
 ```bash
 docker run --rm -v /path/to/book:/book hollowman6/mdbook-pdf
 ```
 
+If your book have other Rust dependencies, you can install them on your local machine (if using Linux), or if you are not using Linux, download the Linux executables of corresponding architecture to a dir, replace `~/.cargo/bin` with your path.
+
+```bash
+docker run --rm -v /path/to/book:/book -v ~/.cargo/bin:/mdbook hollowman6/mdbook-pdf
+```
+
 ## Configuration
 Support customize PDF paper orientation, scale of the webpage rendering, paper width and height, page margins, generated PDF page ranges, whether to display header and footer as well as customize their formats, and more.
 
 Check [book.toml](https://github.com/HollowMan6/mdbook-pdf/blob/main/test_doc/book.toml#L10-L36) and comments for details for the available configurations of `[output.pdf]`.
 
 ## Common Issues
 1. Support for Firefox in `mdbook-pdf`!
@@ -90,15 +111,15 @@
 
 If you have relative links that link outside the book, please provide the [static hosting site URL](https://github.com/HollowMan6/mdbook-pdf/blob/main/test_doc/book.toml#L17-L18) for it to get fixed.
 
 3. Can you add the bookmark to the PDF reflecting the Table of Contents, just like what [wkhtmltopdf](https://wkhtmltopdf.org/) supported?
 
 This should be realized by Chromium, and an issue has already been filed for this [here](https://bugs.chromium.org/p/chromium/issues/detail?id=781797).
 
-Initial support for the bookmark/outline of the PDF file has already been available ([mdbook-pdf-outline](https://pypi.org/project/mdbook-pdf-outline/)). It is written in Python and is another backend for `mdbook` and should be used with `mdbook-pdf` and ***the [mdbook version](https://github.com/rust-lang/mdBook/pull/1738) mentioned in Common Issues 2 for fixing the broken links in `print.html`***.
+Initial support for the bookmark/outline of the PDF file has already been available ([mdbook-pdf-outline](https://pypi.org/project/mdbook-pdf-outline/)). It is written in Python and is another backend for `mdbook` and should be used with `mdbook-pdf` and ***the [mdbook version](https://github.com/rust-lang/mdBook/pull/1738) mentioned in Common Issues 2 (by `cargo install --git https://github.com/HollowMan6/mdBook mdbook` instead) for fixing the broken links in `print.html`***.
 
 You can install this backend by `pip install mdbook-pdf-outline`.
 
 Remember to put the following to ***the end of*** your `book.toml`, ***after [output.pdf]***:
 
 ```toml
 [output.pdf-outline]
```

### Comparing `mdbook-pdf-outline-0.1.3/mdbook_pdf_outline.egg-info/PKG-INFO` & `mdbook-pdf-outline-0.1.4/mdbook_pdf_outline.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdbook-pdf-outline
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool for generating outlines for PDF files generated by mdbook-pdf.
 Home-page: https://github.com/HollowMan6/mdbook-pdf
 Author: Hollow Man (Domain Address)
 Author-email: hollowman@opensuse.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/HollowMan6/mdbook-pdf/issues
 Classifier: Programming Language :: Python :: 3
@@ -79,20 +79,26 @@
 
 [output.pdf]
 ```
 
 Finally you can build your book and get the PDF file with `mdbook build` command, your PDF file will be available at `book/pdf/output.pdf`.
 
 ## Run with Docker
-You can also use this [docker image](https://hub.docker.com/r/hollowman6/mdbook-pdf) if your book doesn't have dependencies other than mdBook.
+You can also use this [docker image](https://hub.docker.com/r/hollowman6/mdbook-pdf).
 
 ```bash
 docker run --rm -v /path/to/book:/book hollowman6/mdbook-pdf
 ```
 
+If your book have other Rust dependencies, you can install them on your local machine (if using Linux), or if you are not using Linux, download the Linux executables of corresponding architecture to a dir, replace `~/.cargo/bin` with your path.
+
+```bash
+docker run --rm -v /path/to/book:/book -v ~/.cargo/bin:/mdbook hollowman6/mdbook-pdf
+```
+
 ## Configuration
 Support customize PDF paper orientation, scale of the webpage rendering, paper width and height, page margins, generated PDF page ranges, whether to display header and footer as well as customize their formats, and more.
 
 Check [book.toml](https://github.com/HollowMan6/mdbook-pdf/blob/main/test_doc/book.toml#L10-L36) and comments for details for the available configurations of `[output.pdf]`.
 
 ## Common Issues
 1. Support for Firefox in `mdbook-pdf`!
@@ -105,15 +111,15 @@
 
 If you have relative links that link outside the book, please provide the [static hosting site URL](https://github.com/HollowMan6/mdbook-pdf/blob/main/test_doc/book.toml#L17-L18) for it to get fixed.
 
 3. Can you add the bookmark to the PDF reflecting the Table of Contents, just like what [wkhtmltopdf](https://wkhtmltopdf.org/) supported?
 
 This should be realized by Chromium, and an issue has already been filed for this [here](https://bugs.chromium.org/p/chromium/issues/detail?id=781797).
 
-Initial support for the bookmark/outline of the PDF file has already been available ([mdbook-pdf-outline](https://pypi.org/project/mdbook-pdf-outline/)). It is written in Python and is another backend for `mdbook` and should be used with `mdbook-pdf` and ***the [mdbook version](https://github.com/rust-lang/mdBook/pull/1738) mentioned in Common Issues 2 for fixing the broken links in `print.html`***.
+Initial support for the bookmark/outline of the PDF file has already been available ([mdbook-pdf-outline](https://pypi.org/project/mdbook-pdf-outline/)). It is written in Python and is another backend for `mdbook` and should be used with `mdbook-pdf` and ***the [mdbook version](https://github.com/rust-lang/mdBook/pull/1738) mentioned in Common Issues 2 (by `cargo install --git https://github.com/HollowMan6/mdBook mdbook` instead) for fixing the broken links in `print.html`***.
 
 You can install this backend by `pip install mdbook-pdf-outline`.
 
 Remember to put the following to ***the end of*** your `book.toml`, ***after [output.pdf]***:
 
 ```toml
 [output.pdf-outline]
```

### Comparing `mdbook-pdf-outline-0.1.3/setup.py` & `mdbook-pdf-outline-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 #!/usr/bin/env python3
 # vim: set fileencoding=utf-8 :
 # vim: set et ts=4 sw=4:
-'''
+"""
   mdbook-pdf-outline
+  An outline (Table of Content) generator for mdBook-pdf.
+
   Author:  Hollow Man <hollowman@opensuse.org>
+  License: GPL-3.0
 
-  Copyright © 2022 Hollow Man(@HollowMan6). All rights reserved.
+  Copyright © 2022-2023 Hollow Man (@HollowMan6). All rights reserved.
 
   This document is free software; you can redistribute it and/or modify it under the terms of the GNU General
   Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option)
   any later version.
-'''
+
+  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
+  warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+  You should have received a copy of the GNU General Public License along with this program.
+  If not, see <http://www.gnu.org/licenses/>.
+"""
 
 from setuptools import setup
 
 # read the contents of README file
 from os import path
+
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-setup(name='mdbook-pdf-outline',
-      version='0.1.3',
-      description='Tool for generating outlines for PDF files generated by mdbook-pdf.',
-      url='https://github.com/HollowMan6/mdbook-pdf',
-      author='Hollow Man (Domain Address)',
-      author_email='hollowman@opensuse.org',
-      license='GPL-3.0-or-later',
-      install_requires=['lxml', 'pypdf'],
-      packages=['mdbook_pdf_outline'],
-      entry_points={'console_scripts': [
-          'mdbook-pdf-outline=mdbook_pdf_outline.mdbook_pdf_outline:main']},
-      long_description=long_description,
-      project_urls={
-          "Bug Tracker": "https://github.com/HollowMan6/mdbook-pdf/issues",
-      },
-      classifiers=[
-          "Programming Language :: Python :: 3",
-          "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-          "Topic :: Text Processing :: Markup :: Markdown",
-      ],
-      long_description_content_type='text/markdown'
-      )
+setup(
+    name="mdbook-pdf-outline",
+    version="0.1.4",
+    description="Tool for generating outlines for PDF files generated by mdbook-pdf.",
+    url="https://github.com/HollowMan6/mdbook-pdf",
+    author="Hollow Man (Domain Address)",
+    author_email="hollowman@opensuse.org",
+    license="GPL-3.0-or-later",
+    install_requires=["lxml", "pypdf"],
+    packages=["mdbook_pdf_outline"],
+    entry_points={
+        "console_scripts": [
+            "mdbook-pdf-outline=mdbook_pdf_outline.mdbook_pdf_outline:main"
+        ]
+    },
+    long_description=long_description,
+    project_urls={
+        "Bug Tracker": "https://github.com/HollowMan6/mdbook-pdf/issues",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Topic :: Text Processing :: Markup :: Markdown",
+    ],
+    long_description_content_type="text/markdown",
+)
```

