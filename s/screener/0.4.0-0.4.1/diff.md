# Comparing `tmp/screener-0.4.0.tar.gz` & `tmp/screener-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screener-0.4.0.tar", max compression
+gzip compressed data, was "screener-0.4.1.tar", max compression
```

## Comparing `screener-0.4.0.tar` & `screener-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1808 2023-06-09 12:49:06.826100 screener-0.4.0/README.md
--rw-r--r--   0        0        0     2514 2023-06-09 12:49:06.826100 screener-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.4.0/screener/__init__.py
--rw-r--r--   0        0        0     1987 2023-06-09 12:49:06.826100 screener-0.4.0/screener/__main__.py
--rw-r--r--   0        0        0      313 2023-06-09 12:49:06.826100 screener-0.4.0/screener/checker.py
--rw-r--r--   0        0        0      859 2023-06-09 12:49:06.827100 screener-0.4.0/screener/diagnostic.py
--rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.4.0/screener/parser/__init__.py
--rw-r--r--   0        0        0      960 2023-06-09 12:49:06.827100 screener-0.4.0/screener/parser/epub.py
--rw-r--r--   0        0        0      902 2023-06-09 12:49:06.827100 screener-0.4.0/screener/parser/kindle.py
--rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.4.0/screener/reader/__init__.py
--rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.4.0/screener/reader/abstract.py
--rw-r--r--   0        0        0      796 2023-06-07 19:00:57.535328 screener-0.4.0/screener/reader/epub.py
--rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.4.0/screener/reader/kindle.py
--rw-r--r--   0        0        0     1040 2023-06-09 12:49:06.827100 screener-0.4.0/screener/utils.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 screener-0.4.0/setup.py
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 screener-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1808 2023-06-09 12:49:06.826100 screener-0.4.1/README.md
+-rw-r--r--   0        0        0     2549 2023-06-11 13:17:10.597748 screener-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.4.1/screener/__init__.py
+-rw-r--r--   0        0        0     2022 2023-06-11 13:17:10.597748 screener-0.4.1/screener/__main__.py
+-rw-r--r--   0        0        0      313 2023-06-09 12:49:06.826100 screener-0.4.1/screener/checker.py
+-rw-r--r--   0        0        0      859 2023-06-09 12:49:06.827100 screener-0.4.1/screener/diagnostic.py
+-rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.4.1/screener/parser/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-09 12:49:06.827100 screener-0.4.1/screener/parser/epub.py
+-rw-r--r--   0        0        0      902 2023-06-09 12:49:06.827100 screener-0.4.1/screener/parser/kindle.py
+-rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.4.1/screener/reader/__init__.py
+-rw-r--r--   0        0        0      806 2023-06-11 13:17:10.597748 screener-0.4.1/screener/reader/abstract.py
+-rw-r--r--   0        0        0      831 2023-06-11 13:17:10.598748 screener-0.4.1/screener/reader/epub.py
+-rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.4.1/screener/reader/kindle.py
+-rw-r--r--   0        0        0     1040 2023-06-09 12:49:06.827100 screener-0.4.1/screener/utils.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 screener-0.4.1/setup.py
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 screener-0.4.1/PKG-INFO
```

### Comparing `screener-0.4.0/README.md` & `screener-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `screener-0.4.0/pyproject.toml` & `screener-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Screener"
-version = "0.4.0"
+version = "0.4.1"
 description = "Check e-book files for security and privacy issues."
 authors = ["Tom Kuson <mail@tjkuson.me>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "screener", from = "." },
 ]
@@ -23,15 +23,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 mypy = "^1.2.0"
 types-beautifulsoup4 = "^4.12.0.5"
-ruff = "^0.0.271"
+ruff = "^0.0.272"
 ssort = "^0.11.6"
 
 [tool.black]
 line-length = 88
 target-version = ["py310"]
 
 [tool.ruff]
@@ -79,14 +79,17 @@
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
 
 [tool.ruff.flake8-type-checking]
 strict = true
 
+[tool.mypy]
+exclude = ["dist"]
+
 [[tool.mypy.overrides]]
 module = ["ebooklib", "ebooklib.epub", "mobi", "kindle"]
 ignore_missing_imports = true
 
 [tool.poetry.scripts]
 screener = "screener.__main__:main"
```

### Comparing `screener-0.4.0/screener/__main__.py` & `screener-0.4.1/screener/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,27 +16,26 @@
         usage="%(prog)s [OPTION] [FILE]...",
         description="Check e-book files for security and privacy issues.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
-        version=f"{parser.prog} version 0.4.0",
+        version=f"{parser.prog} version 0.4.1",
     )
     parser.add_argument("files", nargs="*")
     return parser
 
 
 def check_file(
     file: Path,
 ) -> Checker:
     """Check file."""
-    extension = file.suffix
     checker = Checker(file)
-    match extension:
+    match extension := file.suffix:
         case ".epub":
             with EpubFileReader(file) as epub:
                 parse_epub(checker, epub.file_path)
         case ".azw3" | ".mobi":
             with KindleFileReader(file) as azw3:
                 parse_kindle(checker, azw3.file_path)
         case _:
@@ -47,23 +46,25 @@
 
 def main() -> None:
     """Read system args and check e-book files."""
     parser = init_argparse()
     args = parser.parse_args()
     if not args.files:
         print("No files specified. Run with -h for help.", file=sys.stderr)
+    exit_code = 0
     for file in args.files:
         if file == "-":
             print("stdin not supported", file=sys.stderr)
             continue
         checker = check_file(Path(file))
         if checker.diagnostics:
+            exit_code = 1
             for diagnostic in checker.diagnostics:
                 print(diagnostic)
-            sys.exit(1)
-        print(f"{checker.file_path.name} is safe")
+        else:
+            print(f"{checker.file_path.name} is safe")
 
-    sys.exit()
+    sys.exit(exit_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `screener-0.4.0/screener/diagnostic.py` & `screener-0.4.1/screener/diagnostic.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.0/screener/parser/epub.py` & `screener-0.4.1/screener/parser/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.0/screener/parser/kindle.py` & `screener-0.4.1/screener/parser/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.0/screener/reader/abstract.py` & `screener-0.4.1/screener/reader/abstract.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,8 +23,7 @@
     def __exit__(
         self: AbstractReader,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Run on exit of runtime context."""
-        ...
```

### Comparing `screener-0.4.0/screener/reader/epub.py` & `screener-0.4.1/screener/reader/epub.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 class EpubFileReader(AbstractReader):
     """Handle epub files."""
 
     def __init__(self: EpubFileReader, file_path: Path) -> None:
         """Initialize the class."""
         super().__init__(file_path)
+        self.book: epub.EpubBook
 
     def __enter__(self: EpubFileReader) -> EpubFileReader:
         """Runtime context."""
         with warnings.catch_warnings():
-            # Have to do this because of bug in ebooklib
+            # Have to do this because of bug in ebooklib.
             warnings.simplefilter("ignore")
             self.book = epub.read_epub(self.file_path, options={"ignore_ncx": False})
         return self
```

### Comparing `screener-0.4.0/screener/reader/kindle.py` & `screener-0.4.1/screener/reader/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.0/screener/utils.py` & `screener-0.4.1/screener/utils.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.0/setup.py` & `screener-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['EbookLib>=0.18,<0.19', 'beautifulsoup4>=4.12.2,<5.0.0', 'mobi>=0.3.3,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['screener = screener.__main__:main']}
 
 setup_kwargs = {
     'name': 'screener',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Check e-book files for security and privacy issues.',
     'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreener is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
     'author': 'Tom Kuson',
     'author_email': 'mail@tjkuson.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tjkuson/screener/',
```

### Comparing `screener-0.4.0/PKG-INFO` & `screener-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screener
-Version: 0.4.0
+Version: 0.4.1
 Summary: Check e-book files for security and privacy issues.
 Home-page: https://github.com/tjkuson/screener/
 License: LGPL-3.0-only
 Keywords: ebook,security,privacy,epub,mobi,kindle
 Author: Tom Kuson
 Author-email: mail@tjkuson.me
 Requires-Python: >=3.10,<4.0
```

