# Comparing `tmp/epub2txt-0.1.3.tar.gz` & `tmp/epub2txt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epub2txt-0.1.3.tar", max compression
+gzip compressed data, was "epub2txt-0.1.4.tar", max compression
```

## Comparing `epub2txt-0.1.3.tar` & `epub2txt-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       95 2023-06-07 01:46:44.620780 epub2txt-0.1.3/epub2txt/__init__.py
--rw-r--r--   0        0        0     4740 2022-06-19 07:23:06.171912 epub2txt-0.1.3/epub2txt/__main__.py
--rw-r--r--   0        0        0      797 2021-02-07 16:14:03.598152 epub2txt-0.1.3/epub2txt/browse_filename.py
--rw-r--r--   0        0        0     4088 2023-06-07 01:42:11.681117 epub2txt-0.1.3/epub2txt/epub2txt.py
--rw-r--r--   0        0        0     1357 2021-02-07 17:17:09.586500 epub2txt-0.1.3/epub2txt/gen_filename.py
--rw-r--r--   0        0        0     1091 2021-02-07 07:51:04.577682 epub2txt-0.1.3/LICENSE
--rw-r--r--   0        0        0      614 2023-06-07 01:46:38.818096 epub2txt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1587 2021-02-08 02:52:25.198192 epub2txt-0.1.3/README.md
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 epub2txt-0.1.3/setup.py
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 epub2txt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-06-11 09:07:45.248748 epub2txt-0.1.4/epub2txt/__init__.py
+-rw-r--r--   0        0        0     4911 2023-06-11 07:08:44.299392 epub2txt-0.1.4/epub2txt/__main__.py
+-rw-r--r--   0        0        0      821 2023-06-11 07:07:56.005713 epub2txt-0.1.4/epub2txt/browse_filename.py
+-rw-r--r--   0        0        0     5093 2023-06-11 09:06:34.713343 epub2txt-0.1.4/epub2txt/epub2txt.py
+-rw-r--r--   0        0        0     1357 2023-06-11 07:07:56.045712 epub2txt-0.1.4/epub2txt/gen_filename.py
+-rw-r--r--   0        0        0     1091 2021-02-07 07:51:04.577682 epub2txt-0.1.4/LICENSE
+-rw-r--r--   0        0        0      614 2023-06-11 09:07:37.594793 epub2txt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1835 2023-06-11 09:18:38.643579 epub2txt-0.1.4/README.md
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 epub2txt-0.1.4/setup.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 epub2txt-0.1.4/PKG-INFO
```

### Comparing `epub2txt-0.1.3/epub2txt/__main__.py` & `epub2txt-0.1.4/epub2txt/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """Convert tmx to epub."""
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name, line-too-long, trailing-whitespace, broad-exception-caught, too-many-statements, unused-import
 from pathlib import Path
 
 import logzero
-from logzero import logger
 
 # from pyquery import PyQuery as pq
 from absl import app, flags
+from logzero import logger
 
 # from tmx2epub.xml_iter import xml_iter
 # do not fire browse_filename if tkiner is not present
 try:
-    import tkinter
+    import tkinter  # noqa
+
     tkinter_available = True
     from .browse_filename import browse_filename
 except ModuleNotFoundError:
     tkinter_available = False
 
-from .gen_filename import gen_filename
+from epub2txt import __version__
+
 from .epub2txt import epub2txt
+from .gen_filename import gen_filename
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "filename",
     "",  # browse to file if empty
     "tmx filename (can be gzip or bz2)",
     short_name="f",
@@ -45,16 +48,15 @@
 
 
 def proc_argv(_):  # pylint: disable=too-many-branches  # noqa: C901
     """Proc_argv in absl."""
     # version = "0.1.0"
 
     if FLAGS.version:
-        from epub2txt import __version__
-        print("tmx2epub %s 20210208, brought to you by mu@qq41947782" % __version__)
+        print(f"tmx2epub {__version__} 20210208, brought to you by mu@qq41947782")
         raise SystemExit(0)
 
     if FLAGS.debug:
         logzero.loglevel(10)  # logging.DEBUG
     else:
         logzero.loglevel(20)  # logging.INFO
 
@@ -70,18 +72,20 @@
         filename = ""
         if tkinter_available:
             try:
                 filename = browse_filename(Path(filename))
             except Exception as exc:
                 logger.error(exc)
                 filename = ""
-            logger.debug(" file selected: %s", filename)       
-        
+            logger.debug(" file selected: %s", filename)
+
     if not filename:
-        logger.info("\n\t Operation canceled or no filename provided, unable to proceed, exiting...")
+        logger.info(
+            "\n\t Operation canceled or no filename provided, unable to proceed, exiting..."
+        )
         raise SystemExit(1)
 
     # filename = getattr(FLAGS, "filename")
     # filename not specified
     if not filename:
         # print("\t **filename not give**n, set to", Path(FLAGS.filename).absolute().parent))
         try:
@@ -118,41 +122,45 @@
     try:
         text = epub2txt(
             FLAGS.filename,
             debug=FLAGS.debug,
         )
     except Exception as exc:
         logger.error("epub2txt exc: %s", exc)
-        raise SystemExit(1)
+        raise SystemExit(1) from exc
 
     if FLAGS.i:
-        print(f"""
+        print(
+            f"""
             {epub2txt.title}
-            {epub2txt.toc}""")
+            {epub2txt.toc}"""
+        )
         raise SystemExit(0)
     if FLAGS.m:
-        print(f"""
+        print(
+            f"""
             {epub2txt.title}
             {epub2txt.toc}
             {epub2txt.metadata}
-            {epub2txt.spine}""")
+            {epub2txt.spine}"""
+        )
         raise SystemExit(0)
 
     logger.debug(" epub generated **%s**", text[:200])
 
     try:
         Path(FLAGS.dest).write_text(text, encoding="utf8")
     except Exception as exc:
         logger.error("Path(FLAGS.dest).write_text exc: %s", exc)
-        raise SystemExit(1)
+        raise SystemExit(1) from exc
 
     logger.info(" epub file: %s", FLAGS.filename)
     logger.info(" text file: %s", FLAGS.dest)
 
 
 def main():
-    """ main. """
+    """main."""
     app.run(proc_argv)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `epub2txt-0.1.3/epub2txt/epub2txt.py` & `epub2txt-0.1.4/epub2txt/epub2txt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """Convert epub to text."""
-# pylint: disable=invalid-name, too-many-branches, too-many-statements, broad-except, deprecated-class
+# pylint: disable=invalid-name, too-many-branches, too-many-statements, too-many-locals, broad-except, deprecated-class, line-too-long, c-extension-no-member
 
 from pathlib import Path
 from typing import Any, Callable, List, Union
 
 try:
     from collections.abc import Iterable  # python 3.10+
 except ImportError:
     from collections import Iterable  # python < 3.10
 
 # the rest
-import io
+# import io
+import tempfile
 from itertools import zip_longest
 
+import ebooklib
 import httpx
 import logzero
 from ebooklib import epub
 from logzero import logger
 from lxml import etree
 
+parser = etree.HTMLParser()
+
 
 def with_func_attrs(**attrs: Any) -> Callable:
     """Deco with_func_attrs."""
 
     def with_attrs(fct: Callable) -> Callable:
         for key, val in attrs.items():
             setattr(fct, key, val)
@@ -62,25 +66,32 @@
         logzero.loglevel(10)
     else:
         logzero.loglevel(20)
 
     # process possible url
     if str(filepath).startswith("http"):
         try:
-            resp = httpx.get(filepath, timeout=30)
+            resp = httpx.get(filepath, timeout=30, follow_redirects=True)
             resp.raise_for_status()
         except Exception as exc:
             logger.error("httpx.get(%s) exc: %s", filepath, exc)
             raise
-        cont = io.BytesIO(resp.content)
+        # cont = io.BytesIO(resp.content)
+        with tempfile.NamedTemporaryFile(mode='w+b', delete=False) as tfile:
+            try:
+                tfile.write(resp.content)
+            except Exception as exc:
+                logger.error(exc)
+                raise
+            file_name = tfile.name
 
         try:
-            book = epub.read_epub(cont)
+            book = epub.read_epub(file_name)
         except Exception as exc:
-            logger.error("epub.read_epub(cont) exc: %s", exc)
+            logger.error("epub.read_epub(%s) exc: %s", file_name, exc)
             raise
     else:
         filepath = Path(filepath)
         try:
             book = epub.read_epub(filepath)
         except Exception as exc:
             logger.error("epub.read_epub(%s) exc: %s", filepath, exc)
@@ -106,25 +117,39 @@
     epub2txt.spine = [elm[0] for elm in book.spine]
 
     # list of ebooklib.epub.EpuNav/ebooklib.epub.EpubHtml
     # [book.get_item_with_id(elm) for elm in epub2txt.spine]
 
     epub2txt.metadata = [*book.metadata.values()]
 
-    contents = [book.get_item_with_id(item[0]).content for item in book.spine]
+    # contents = [book.get_item_with_id(item[0]).content for item in book.spine]
+    contents = [elm.content for elm in book.get_items_of_type(ebooklib.ITEM_DOCUMENT)]
+
+    names = [elm.get_name() for elm in book.get_items_of_type(ebooklib.ITEM_DOCUMENT)]
+
+    epub2txt.names = names
+
+    # content/chapter titles
+    # remove bookmark #: most toc_hrefs correspond to names
+    _ = [Path(elm).with_suffix('.xhtml').as_posix() for elm in epub2txt.toc_hrefs]
+    name2title = dict(zip(_, epub2txt.toc_titles))
+
+    epub2txt.content_titles = [name2title.get(name, "NA") for name in names]
+
     # texts = [pq(content).text() for content in contents]
 
     # Using XPath to find text
     # root = etree.XML(content)
     # tree = etree.ElementTree(root)
     # text = tree.xpath("string()")   # pq(content).text()
 
     texts = []
     for content in contents:
-        root = etree.XML(content)
+        # root = etree.XML(content)
+        root = etree.XML(content, parser=parser)
         tree = etree.ElementTree(root)
         text = tree.xpath("string()")
         texts.append(text)
 
     if clean:
         temp = []
         for text in texts:
```

### Comparing `epub2txt-0.1.3/epub2txt/gen_filename.py` & `epub2txt-0.1.4/epub2txt/gen_filename.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Gen a filename.
 
 Give a file name, gen a filename whose file does not exist by adding extra number
 """
 from pathlib import Path
-from string import ascii_lowercase
 from random import sample
+from string import ascii_lowercase
 
 
 def gen_filename(filename, sep="_", rand=False):
     """Gen a filename.
 
     Give a file name, gen a filename whose file does not exist by adding extra number
     >>> gen_filename('gen_filename.py')
```

### Comparing `epub2txt-0.1.3/LICENSE` & `epub2txt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.3/pyproject.toml` & `epub2txt-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epub2txt"
-version = "0.1.3"
+version = "0.1.4"
 description = "Convert epub to txt with additonal utils"
 authors = ["freemt"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ffreemt/epub2txt"
 
 [tool.poetry.dependencies]
```

### Comparing `epub2txt-0.1.3/README.md` & `epub2txt-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 ## Installation
 
 ```bash
 pip install epub2txt
 # pip install epub2txt -U  # to upgrade
 ```
+## Fixes
+* More resilent to mismatched tags
+* Added `epub2txt.content_titles`, useful for creating metada when needed
 
 ## Usage
 
 ### From command line
 
 ```bash
 # convert test.epub to test.txt
@@ -43,13 +46,16 @@
 url = "https://github.com/ffreemt/tmx2epub/raw/master/tests/1.tmx.epub"
 res = epub2txt(url)
 
 # from a local epub file
 filepath = r"tests\test.epub"
 res = epub2txt(filepath)
 
+# output as a list of chapters
+ch_list = epub2txt(filepath, outputlist=True)
+# chapter titles will be available as epub2txt.content_titles if available
+
 ```
 
 ## TODO
-*   Extract a single chapter
 *   Batch conversion of several epub files
```

### Comparing `epub2txt-0.1.3/setup.py` & `epub2txt-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'tqdm>=4.56.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['epub2txt = epub2txt.__main__:main']}
 
 setup_kwargs = {
     'name': 'epub2txt',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Convert epub to txt with additonal utils',
-    'long_description': '# epub2txt [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05c422da73a14c23b87b0657af9c8df7)](https://www.codacy.com/gh/ffreemt/epub2txt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ffreemt/epub2txt&amp;utm_campaign=Badge_Grade)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/epub2txt.svg)](https://badge.fury.io/py/epub2txt)\n\nConvert epub to txt with additonal utils\n\n<!--- Refer to dualtext-epub\\der_fanger_de_en.py\n\t\t__main__.py refer to tmx2epub.__main__\n--->\n\n## Installation\n\n```bash\npip install epub2txt\n# pip install epub2txt -U  # to upgrade\n```\n\n## Usage\n\n### From command line\n\n```bash\n# convert test.epub to test.txt\nepub2txt -f test.epub\n\n# browse for epub file, txt file will be in the same directory as the epub file\nepub2txt\n\n# show epub book info: title and toc\nepub2txt -i\n\n# show more epub book info: title, toc, metadata, spine (list of stuff packed into the epub)\nepub2txt -m\n\n# show epub2txt version\nepub2txt -V\n\n```\n\n### `python` code\n\n```python\nfrom epub2txt import epub2txt\n# from a url to epub\nurl = "https://github.com/ffreemt/tmx2epub/raw/master/tests/1.tmx.epub"\nres = epub2txt(url)\n\n# from a local epub file\nfilepath = r"tests\\test.epub"\nres = epub2txt(filepath)\n\n```\n\n## TODO\n*   Extract a single chapter\n*   Batch conversion of several epub files\n\n',
+    'long_description': '# epub2txt [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05c422da73a14c23b87b0657af9c8df7)](https://www.codacy.com/gh/ffreemt/epub2txt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ffreemt/epub2txt&amp;utm_campaign=Badge_Grade)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/epub2txt.svg)](https://badge.fury.io/py/epub2txt)\n\nConvert epub to txt with additonal utils\n\n<!--- Refer to dualtext-epub\\der_fanger_de_en.py\n\t\t__main__.py refer to tmx2epub.__main__\n--->\n\n## Installation\n\n```bash\npip install epub2txt\n# pip install epub2txt -U  # to upgrade\n```\n## Fixes\n* More resilent to mismatched tags\n* Added `epub2txt.content_titles`, useful for creating metada when needed\n\n## Usage\n\n### From command line\n\n```bash\n# convert test.epub to test.txt\nepub2txt -f test.epub\n\n# browse for epub file, txt file will be in the same directory as the epub file\nepub2txt\n\n# show epub book info: title and toc\nepub2txt -i\n\n# show more epub book info: title, toc, metadata, spine (list of stuff packed into the epub)\nepub2txt -m\n\n# show epub2txt version\nepub2txt -V\n\n```\n\n### `python` code\n\n```python\nfrom epub2txt import epub2txt\n# from a url to epub\nurl = "https://github.com/ffreemt/tmx2epub/raw/master/tests/1.tmx.epub"\nres = epub2txt(url)\n\n# from a local epub file\nfilepath = r"tests\\test.epub"\nres = epub2txt(filepath)\n\n# output as a list of chapters\nch_list = epub2txt(filepath, outputlist=True)\n# chapter titles will be available as epub2txt.content_titles if available\n\n```\n\n## TODO\n*   Batch conversion of several epub files\n\n',
     'author': 'freemt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ffreemt/epub2txt',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `epub2txt-0.1.3/PKG-INFO` & `epub2txt-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub2txt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert epub to txt with additonal utils
 Home-page: https://github.com/ffreemt/epub2txt
 License: MIT
 Author: freemt
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,14 +29,17 @@
 
 ## Installation
 
 ```bash
 pip install epub2txt
 # pip install epub2txt -U  # to upgrade
 ```
+## Fixes
+* More resilent to mismatched tags
+* Added `epub2txt.content_titles`, useful for creating metada when needed
 
 ## Usage
 
 ### From command line
 
 ```bash
 # convert test.epub to test.txt
@@ -64,14 +67,17 @@
 url = "https://github.com/ffreemt/tmx2epub/raw/master/tests/1.tmx.epub"
 res = epub2txt(url)
 
 # from a local epub file
 filepath = r"tests\test.epub"
 res = epub2txt(filepath)
 
+# output as a list of chapters
+ch_list = epub2txt(filepath, outputlist=True)
+# chapter titles will be available as epub2txt.content_titles if available
+
 ```
 
 ## TODO
-*   Extract a single chapter
 *   Batch conversion of several epub files
```

