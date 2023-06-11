# Comparing `tmp/turbo_docs-0.8.5.tar.gz` & `tmp/turbo_docs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.8.5.tar", last modified: Sat Jun  3 19:01:56 2023, max compression
+gzip compressed data, was "turbo_docs-0.9.0.tar", last modified: Sun Jun 11 16:43:01 2023, max compression
```

## Comparing `turbo_docs-0.8.5.tar` & `turbo_docs-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.375188 turbo_docs-0.8.5/
--rw-rw-rw-   0        0        0     2314 2023-06-03 19:01:56.375188 turbo_docs-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2023-06-03 18:58:36.000000 turbo_docs-0.8.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 19:01:56.376176 turbo_docs-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-06-03 18:58:56.000000 turbo_docs-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.352435 turbo_docs-0.8.5/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.5/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.366150 turbo_docs-0.8.5/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.5/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.5/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0      731 2023-06-03 18:58:36.000000 turbo_docs-0.8.5/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1036 2023-05-29 19:09:40.000000 turbo_docs-0.8.5/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.372170 turbo_docs-0.8.5/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.5/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.5/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2854 2023-06-03 18:58:36.000000 turbo_docs-0.8.5/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.8.5/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-03 19:01:56.362300 turbo_docs-0.8.5/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2314 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 19:01:56.000000 turbo_docs-0.8.5/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.849555 turbo_docs-0.9.0/
+-rw-rw-rw-   0        0        0     3430 2023-06-11 16:43:01.847559 turbo_docs-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2933 2023-06-11 16:42:38.000000 turbo_docs-0.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 16:43:01.850557 turbo_docs-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-06-11 16:42:54.000000 turbo_docs-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.822259 turbo_docs-0.9.0/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.0/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.837005 turbo_docs-0.9.0/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.0/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0      596 2023-06-11 13:01:46.000000 turbo_docs-0.9.0/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0      898 2023-06-11 13:04:26.000000 turbo_docs-0.9.0/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.845469 turbo_docs-0.9.0/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.0/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-06-11 12:56:58.000000 turbo_docs-0.9.0/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2022 2023-06-11 15:15:54.000000 turbo_docs-0.9.0/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.9.0/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:01.833987 turbo_docs-0.9.0/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     3430 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 16:43:01.000000 turbo_docs-0.9.0/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.8.5/PKG-INFO` & `turbo_docs-0.9.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,85 @@
-Metadata-Version: 2.1
-Name: turbo_docs
-Version: 0.8.5
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 # Turbo Docs
 
-Turbo Docs is a Python script that utilizes OpenAI's GPT API to generate README.md files and docstrings for your Python projects automatically.
-
-## Requirements
+Turbo Docs is a Python tool designed to help developers generate a well-formatted README.md file for their repository and perform other tasks related to gathering information from their codebase.
 
-To use Turbo Docs, you will need to have the following Python packages installed:
+## Installation
 
-- setuptools
-- wheel
-- twine
-- requests
-- openai
-- click
-- pyperclip
-- redbaron
-- gitpython
-- toml
+You can install Turbo Docs using pip:
 
-You can install them using the requirements.txt and requirements.dev.txt files in the repository.
+```bash
+pip install turbo_docs
+```
 
 ## Usage
 
-To generate a README.md or docstrings for the current directory, you can run the `generate.py` script in the `turbo_docs` folder:
+Turbo Docs provides command line options for various tasks, such as generating a README.md file, or copying the formatted directory text to the clipboard. To use Turbo Docs, run the following command in your terminal:
 
 ```bash
-# install tubro_docs
-pip install turbo_docs
-
-# command line interface
-turbo_docs [--copy] [--readme] [--docstring]
+turbo_docs [options]
 ```
 
-You can use the optional flags:
-- `--copy`: Copy the directory text to clipboard.
-- `--readme`: Generate README.md file.
-- `--docstring`: Generate and insert docstrings for each function.
+### Available Options
+
+- `--copy`: Copy the formatted text of the entire directory to clipboard. This can be useful when working with GPT. Example:
+
+  ```
+  turbo_docs --copy
+  ```
 
-## Customization
+- `--readme`: Generate a well-formatted README.md file for the repository. Example:
 
-You can modify the files and directories that are excluded from the documentation generation by editing the `exclude.toml` file in the root of the repository. 
+  ```
+  turbo_docs --readme
+  ```
 
-Example syntax to exclude requirements files:
+## Configuration
+
+To configure Turbo Docs, create a `turbo_docs.toml` file in the root of your project and specify the files and directories to ignore. The following example shows how to exclude different types of files and directories:
 
 ```toml
-exclude = [
-  "requirements.*"
+ignore = 
+    "__pycache__",
+    "venv",
+    "build",
+    "dist",
+    "*.egg-info",
+    ".git",
+    "README.md",  # This is recommended so that --readme doesn't include the readme file itself
 ]
 ```
 
-## Modules
+## Files and Folders Overview
+
+Here's an overview of the files and folders in the Turbo Docs repository:
 
-Turbo Docs consists of three main modules:
+- `turbo_docs\commands\readme.py`: Contains the `readme` function that generates a README.md file using the OpenAI API.
+- `turbo_docs\commands\__init__.py`: The init file for the `turbo_docs.commands` package.
+- `turbo_docs\generate.py`: The main module containing the `driver` function which is the entry point for the script.
+- `turbo_docs\utils\cli_options.py`: Contains the functions for adding command-line options, such as `copy` and `readme`.
+- `turbo_docs\utils\directory.py`: Contains utility functions for working with directories and reading text from files.
+- `turbo_docs\utils\openai_api.py`: Contains utility functions for interacting with the OpenAI API.
+- `turbo_docs\__init__.py`: The init file for the `turbo_docs` package.
+- `.gitignore`: A list of files and directories to be ignored by GIT.
+- `exclude.toml`: Example toml configuration file for specifying files or directories to exclude.
+- `requirements.txt`: Lists all the required Python packages for Turbo Docs.
+- `setup.py`: Sets up the Turbo Docs Python package.
+- `turbo_docs.toml`: The Turbo Docs configuration file.
+
+## Dependencies
+
+Turbo Docs uses the following Python packages:
+
+- `requests`
+- `openai`
+- `click`
+- `pyperclip`
+- `redbaron`
+- `gitpython`
+- `toml`
+- `pathspec`
 
-1. `turbo_docs.commands.docstring`: Contains functions to generate docstrings for Python functions using GPT-3 text completion model.
-2. `turbo_docs.commands.readme`: Contains a function to generate a README.md file using the OpenAI API.
-3. `turbo_docs.utils`: Contains utility functions and decorators for working with CLI options, directories, and the OpenAI API.
+Please make sure these packages are installed before running Turbo Docs.
 
-## Contributing
+## License
 
-Contributions are always welcome! If you have ideas for improvements or bug fixes, please open an issue or submit a pull request.
+Turbo Docs is released under the MIT License. See the LICENSE file for more details.
```

### Comparing `turbo_docs-0.8.5/setup.py` & `turbo_docs-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.8.5",
+	version="0.9.0",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
 		"gitpython",
     	"toml",
+        "pathspec",
 	],
 	entry_points={
 		"console_scripts": [
 			"turbo_docs=turbo_docs.generate:driver"
 		],
 	},
 	classifiers=[
```

### Comparing `turbo_docs-0.8.5/turbo_docs/generate.py` & `turbo_docs-0.9.0/turbo_docs/generate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import click
 import pyperclip
-from turbo_docs.commands import docstring as docstring_module
 from turbo_docs.commands import readme as readme_module
 from turbo_docs.utils import directory, cli_options
 
 
 @click.command()
 @cli_options.copy
 @cli_options.readme
-@cli_options.docstring
 def driver(
         copy: bool,
         readme: bool,
-        docstring: bool,
 ) -> None:
     """
-    Generate a README or docstring for the current directory.
+    Pull text from all files in the current directory and apply the following commands:
+
+    'turbo_docs --copy' copies the text to clipboard
+        Useful for wokring with ChatGPT
+
+    'turbo_docs --readme' generates a README.md file
+        Useful for keeping documentation up to date
     """
-    files = directory.get_files()
-    dir_text = "\n\n".join(
-        [f"{name}:\n\n{content}" for name, content in files.items()])
+    dir_text = directory.get_repo_text()
 
-    # Copy directory text to clipboard if specified
     if copy:
         pyperclip.copy(dir_text)
         print("(--copy) Directory text copied to clipboard")
 
-    # Generate docstring for each function if specified
-    if docstring:
-        docstring_module.docstring(files)
-
-    # Generate README.md file if specified
     if readme:
         readme_module.readme(dir_text)
+        print("(--readme) README.md file generated")
 
 
 if __name__ == '__main__':
     driver()
```

### Comparing `turbo_docs-0.8.5/turbo_docs/utils/openai_api.py` & `turbo_docs-0.9.0/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

