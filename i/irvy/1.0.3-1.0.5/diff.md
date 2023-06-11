# Comparing `tmp/irvy-1.0.3.tar.gz` & `tmp/irvy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irvy-1.0.3.tar", last modified: Sun Jun 11 10:08:07 2023, max compression
+gzip compressed data, was "irvy-1.0.5.tar", last modified: Sun Jun 11 21:40:11 2023, max compression
```

## Comparing `irvy-1.0.3.tar` & `irvy-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.957610 irvy-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 10:08:07.957610 irvy-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-11 10:07:45.000000 irvy-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/generators/PlaywrightGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/generators/SeleniumGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/irvy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:07:45.000000 irvy-1.0.3/irvy/utils/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:08:07.953609 irvy-1.0.3/irvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 10:08:07.000000 irvy-1.0.3/irvy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:08:07.957610 irvy-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 10:07:45.000000 irvy-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:40:11.097295 irvy-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-11 21:40:11.097295 irvy-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-11 21:39:57.000000 irvy-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:40:11.093294 irvy-1.0.5/irvy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:40:11.097295 irvy-1.0.5/irvy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/generators/PlaywrightGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/generators/SeleniumGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/irvy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:40:11.097295 irvy-1.0.5/irvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:39:57.000000 irvy-1.0.5/irvy/utils/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:40:11.097295 irvy-1.0.5/irvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-11 21:40:11.000000 irvy-1.0.5/irvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-11 21:40:11.000000 irvy-1.0.5/irvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:40:11.000000 irvy-1.0.5/irvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-11 21:40:11.000000 irvy-1.0.5/irvy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 21:40:11.000000 irvy-1.0.5/irvy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:40:11.097295 irvy-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-11 21:39:57.000000 irvy-1.0.5/setup.py
```

### Comparing `irvy-1.0.3/PKG-INFO` & `irvy-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irvy
-Version: 1.0.3
+Version: 1.0.5
 Summary: A brief description of your project
 Description-Content-Type: text/markdown
 
 # Irvy
 
 Irvy simplifies the setup process for test automation using Selenium or Playwright across multiple programming languages. It serves as a valuable tool for both novice automation engineers and seasoned professionals, facilitating a seamless transition between programming languages such as Java, C#, or JavaScript by providing comparable building blocks.
 
@@ -115,17 +115,15 @@
 |-- src/
     |-- tests/
         |-- test_example.js OR test_example.py OR test_example.cs
 |-- node_modules/ OR venv/ OR packages/
 ```
 
 
-
-https://github.com/automationpi/irvy/assets/82222256/89dbfc66-d8ff-4405-bf88-d5291cbf25df
-
+https://github.com/automationpi/irvy/assets/82222256/4a780b2c-8779-4980-a568-1dd715bb319e
 
 
 
 # Technologies and Frameworks
 Depending on the language and tool you choose, Irvy will use different testing frameworks:
 ```
 Python: Irvy will use Pytest for both Selenium and Playwright projects.
```

### Comparing `irvy-1.0.3/README.md` & `irvy-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -109,17 +109,15 @@
 |-- src/
     |-- tests/
         |-- test_example.js OR test_example.py OR test_example.cs
 |-- node_modules/ OR venv/ OR packages/
 ```
 
 
-
-https://github.com/automationpi/irvy/assets/82222256/89dbfc66-d8ff-4405-bf88-d5291cbf25df
-
+https://github.com/automationpi/irvy/assets/82222256/4a780b2c-8779-4980-a568-1dd715bb319e
 
 
 
 # Technologies and Frameworks
 Depending on the language and tool you choose, Irvy will use different testing frameworks:
 ```
 Python: Irvy will use Pytest for both Selenium and Playwright projects.
```

### Comparing `irvy-1.0.3/irvy/generators/PlaywrightGenerator.py` & `irvy-1.0.5/irvy/generators/PlaywrightGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.3/irvy/generators/SeleniumGenerator.py` & `irvy-1.0.5/irvy/generators/SeleniumGenerator.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.3/irvy/irvy.py` & `irvy-1.0.5/irvy/irvy.py`

 * *Files identical despite different names*

### Comparing `irvy-1.0.3/irvy.egg-info/PKG-INFO` & `irvy-1.0.5/irvy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irvy
-Version: 1.0.3
+Version: 1.0.5
 Summary: A brief description of your project
 Description-Content-Type: text/markdown
 
 # Irvy
 
 Irvy simplifies the setup process for test automation using Selenium or Playwright across multiple programming languages. It serves as a valuable tool for both novice automation engineers and seasoned professionals, facilitating a seamless transition between programming languages such as Java, C#, or JavaScript by providing comparable building blocks.
 
@@ -115,17 +115,15 @@
 |-- src/
     |-- tests/
         |-- test_example.js OR test_example.py OR test_example.cs
 |-- node_modules/ OR venv/ OR packages/
 ```
 
 
-
-https://github.com/automationpi/irvy/assets/82222256/89dbfc66-d8ff-4405-bf88-d5291cbf25df
-
+https://github.com/automationpi/irvy/assets/82222256/4a780b2c-8779-4980-a568-1dd715bb319e
 
 
 
 # Technologies and Frameworks
 Depending on the language and tool you choose, Irvy will use different testing frameworks:
 ```
 Python: Irvy will use Pytest for both Selenium and Playwright projects.
```

### Comparing `irvy-1.0.3/setup.py` & `irvy-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Open the README file.
 with open(file="README.md", mode="r") as readme_handle:
     long_description = readme_handle.read()
 
 setup(
     name='irvy',
-    version='1.0.3',
+    version='1.0.5',
     description='A brief description of your project',  # add this
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # this should automatically find your packages
     include_package_data=True,
     install_requires=[
         # list of dependencies
```

