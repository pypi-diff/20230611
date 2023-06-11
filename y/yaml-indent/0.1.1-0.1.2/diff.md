# Comparing `tmp/yaml_indent-0.1.1.tar.gz` & `tmp/yaml_indent-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_indent-0.1.1.tar", max compression
+gzip compressed data, was "yaml_indent-0.1.2.tar", max compression
```

## Comparing `yaml_indent-0.1.1.tar` & `yaml_indent-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-06-08 11:39:30.751856 yaml_indent-0.1.1/LICENSE
--rw-r--r--   0        0        0     1525 2023-06-09 08:19:25.573057 yaml_indent-0.1.1/README.md
--rw-r--r--   0        0        0      410 2023-06-09 14:29:30.292178 yaml_indent-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 11:19:16.282076 yaml_indent-0.1.1/yaml_indent/__init__.py
--rwxr-xr-x   0        0        0     2611 2023-06-09 14:41:45.327691 yaml_indent-0.1.1/yaml_indent/yaml_indent.py
--rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 yaml_indent-0.1.1/setup.py
--rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 yaml_indent-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-11 08:48:40.402953 yaml_indent-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1599 2023-06-11 08:48:40.402953 yaml_indent-0.1.2/README.md
+-rw-r--r--   0        0        0      608 2023-06-11 09:22:19.042831 yaml_indent-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 08:48:40.402953 yaml_indent-0.1.2/yaml_indent/__init__.py
+-rwxr-xr-x   0        0        0     2914 2023-06-11 09:14:11.152191 yaml_indent-0.1.2/yaml_indent/yaml_indent.py
+-rw-r--r--   0        0        0     2277 1970-01-01 00:00:00.000000 yaml_indent-0.1.2/PKG-INFO
```

### Comparing `yaml_indent-0.1.1/LICENSE` & `yaml_indent-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_indent-0.1.1/README.md` & `yaml_indent-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,78 @@
-# YAML Indent
-
+Metadata-Version: 2.1
+Name: yaml-indent
+Version: 0.1.2
+Summary: 
+Author: Knut Olav Bøhmer
+Author-email: bohmer@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Requires-Dist: configparser (>=5.3.0,<6.0.0)
+Requires-Dist: ruamel-yaml (>=0.17.31,<0.18.0)
+Project-URL: Bug Tracker, https://github.com/knobo/yaml-indent/issues
+Project-URL: Documentation, https://github.com/knobo/yaml-indent/wiki
+Project-URL: Repository, https://github.com/knobo/yaml-indent
+Description-Content-Type: text/markdown
 
-## Overview
+# YAML Indent
 
-yaml-indent is a Python utility for formatting YAML files with correct
-indentation. It reads in a YAML file, processes it, and outputs a new
-YAML file with proper indentation, making the file more readable and
-manageable.
-
-## How it Works
-
-The utility makes use of the PyYAML library to parse the input YAML
-file, and re-dumps the YAML data into the output file with correct
-indentation.
+`yaml-indent` is a Python script to re-indent YAML files according to configurable or default indentation rules. It uses the `ruamel.yaml` library for parsing and writing YAML.
 
 ## Installation
 
-To use this utility, you must have Python 3 installed on your
-system. Additionally, you need to install the PyYAML library. You can
-install it using pip:
+The script requires Python 3.
 
 ``` sh
 pip install yaml-indent
 ```
 
-You can then clone this repository to your local machine.
-
 ## Usage
 
-To use this utility, you need to run the Python script yaml_indent.py
-with two arguments: the input YAML file and the output YAML file. 
-
-Here is an example:
+You can run `yaml-indent` from the command line with the following syntax:
 
 ``` sh
-yaml-indent input.yaml output.yaml
+yaml-indent <input_file> [-o <output_file>] [-i]
 ```
 
-In this command, input.yaml is the YAML file you want to format and
-output.yaml is the file where the formatted YAML will be written. If
-output.yaml already exists, it will be overwritten.
+Where:
+
+- `<input_file>` is the path to the input YAML file to be re-indented.
+- `-o <output_file>` (optional) is the path to the output file where the indented YAML will be written.
+- `-i` (optional) if set, the input file will be edited in place.
+
+If no output file is specified and `-i` is not set, the indented YAML will be printed to the standard output.
 
+## Configuration
+
+`yaml-indent` looks for a `.yaml_indent.ini` configuration file in the
+current directory and all parent directories up to the home
+directory. The configuration file should be in the INI format and can
+specify the `mapping`, `sequence`, and `offset` indentation values
+under the `YAML` section.
+
+Here's an example:
+
+```ini
+[YAML]
+mapping=4
+sequence=4
+offset=0
+```
 ## Contributing
 
 Contributions to this project are welcome. If you find a bug or think
 of a feature that this utility could benefit from, please open an
 issue or submit a pull request.
 
 ## Source Code
 
-The source code for this project is hosted on GitHub. You can access it at [https://github.com/knobo/yaml-indent](https://github.com/knobo/yaml-indent).
-
+The source code for this project is hosted on GitHub. You can access
+it at [https://github.com/knobo/yaml-indent](https://github.com/knobo/yaml-indent).
 
 ## License
 
 This project is open source under the terms of the GPL License.
 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yaml_indent-0.1.1/yaml_indent/yaml_indent.py` & `yaml_indent-0.1.2/yaml_indent/yaml_indent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,94 @@
 #!/usr/bin/env python3
-
+""" A program to indent yaml files """
 import argparse
 import configparser
 import os
-from ruamel.yaml import YAML
 import sys
+from ruamel.yaml import YAML
 
-def find_config_file():
-    # Start from the current directory
-    dir_path = os.getcwd()
+
+def find_config_file(dir_path):
+    '''Finds config file for files in dir_path'''
     home_dir = os.path.expanduser("~")  # Home directory path
     while dir_path != home_dir:  # Stop at the home directory
         config_path = os.path.join(dir_path, '.yaml_indent.ini')
         if os.path.exists(config_path):
             return config_path
         # Go up to the parent directory
         dir_path = os.path.dirname(dir_path)
     return None
 
+
 def process_yaml_file(input_file, output_file=None, in_place=False):
+    '''Indent input_file according to default rules or rules found in the
+    config_file'''
+
     yaml = YAML()
 
     # Check for a configuration file
-    config_path = find_config_file()
+    config_path = find_config_file(os.path.dirname(input_file))
     if config_path:
         config = configparser.ConfigParser()
         config.read(config_path)
         # Get the mapping, sequence, and offset values from the config file
         mapping = config.getint('YAML', 'mapping', fallback=2)
         sequence = config.getint('YAML', 'sequence', fallback=4)
         offset = config.getint('YAML', 'offset', fallback=2)
     else:
         mapping, sequence, offset = 2, 4, 2  # Default values
 
     yaml.indent(mapping=mapping, sequence=sequence, offset=offset)
 
     # Open the input YAML file and load the data
-    with open(input_file, 'r') as stream:
+    with open(input_file, 'r', encoding='UTF-8') as stream:
         try:
             data = yaml.load(stream)
         except Exception as exc:
             print(exc)
-    
+
     # Open the output file and dump the data with correct indenting
     if in_place:
-        with open(input_file, 'w') as outfile:
+        with open(input_file, 'w', encoding='UTF-8') as outfile:
             try:
                 yaml.dump(data, outfile)
             except Exception as exc:
                 print(exc)
     elif output_file:
-        with open(output_file, 'w') as outfile:
+        with open(output_file, 'w', encoding='UTF-8') as outfile:
             try:
                 yaml.dump(data, outfile)
             except Exception as exc:
                 print(exc)
     else:
         try:
             yaml.dump(data, sys.stdout)
         except Exception as exc:
             print(exc)
 
+
 def main():
+    '''Parse arguments and indent files'''
+
     parser = argparse.ArgumentParser()
-    parser.add_argument('input_file', help='The input YAML file to be indented')
-    parser.add_argument('-o', '--output_file', nargs='?', default=argparse.SUPPRESS,
-                        help='The output file where the indented YAML will be written')
+    parser.add_argument(
+        'input_file',
+        help='The input YAML file to be indented'
+    )
+    parser.add_argument(
+        '-o', '--output_file', nargs='?',
+        default=argparse.SUPPRESS,
+        help='The output file where the indented YAML will be written'
+    )
     parser.add_argument('-i', '--in_place', action='store_true',
                         help='If set, the input file will be edited in place')
     args = parser.parse_args()
-    
-    process_yaml_file(args.input_file, getattr(args, 'output_file', None), args.in_place)
+
+    process_yaml_file(
+        args.input_file,
+        getattr(args, 'output_file', None),
+        args.in_place
+    )
+
 
 if __name__ == "__main__":
     main()
```

