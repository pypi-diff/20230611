# Comparing `tmp/pyucrop-1.0.0.tar.gz` & `tmp/pyucrop-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyucrop-1.0.0.tar", last modified: Sun Jun 11 09:41:03 2023, max compression
+gzip compressed data, was "dist\pyucrop-1.0.1.tar", last modified: Sun Jun 11 09:46:15 2023, max compression
```

## Comparing `pyucrop-1.0.0.tar` & `pyucrop-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 09:41:03.063507 pyucrop-1.0.0/
--rw-rw-rw-   0        0        0       17 2023-06-11 09:41:00.000000 pyucrop-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2023-06-11 09:41:03.064484 pyucrop-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 09:41:03.055695 pyucrop-1.0.0/pyucrop/
--rw-rw-rw-   0        0        0       34 2023-06-11 09:33:31.000000 pyucrop-1.0.0/pyucrop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 09:41:03.061554 pyucrop-1.0.0/pyucrop.egg-info/
--rw-rw-rw-   0        0        0      474 2023-06-11 09:41:01.000000 pyucrop-1.0.0/pyucrop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-11 09:41:02.000000 pyucrop-1.0.0/pyucrop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 09:41:01.000000 pyucrop-1.0.0/pyucrop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 09:41:01.000000 pyucrop-1.0.0/pyucrop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 09:41:03.066437 pyucrop-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      552 2023-06-11 09:41:00.000000 pyucrop-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:46:15.788117 pyucrop-1.0.1/
+-rw-rw-rw-   0        0        0       17 2023-06-11 09:46:14.000000 pyucrop-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2023-06-11 09:46:15.788117 pyucrop-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 09:46:15.758820 pyucrop-1.0.1/pyucrop/
+-rw-rw-rw-   0        0        0       34 2023-06-11 09:33:31.000000 pyucrop-1.0.1/pyucrop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:46:15.787140 pyucrop-1.0.1/pyucrop/clients/
+-rw-rw-rw-   0        0        0     2285 2023-06-11 09:36:29.000000 pyucrop-1.0.1/pyucrop/clients/client.py
+-rw-rw-rw-   0        0        0     2340 2023-06-10 07:17:34.000000 pyucrop-1.0.1/pyucrop/clients/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:46:15.783234 pyucrop-1.0.1/pyucrop.egg-info/
+-rw-rw-rw-   0        0        0      483 2023-06-11 09:46:15.000000 pyucrop-1.0.1/pyucrop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-11 09:46:15.000000 pyucrop-1.0.1/pyucrop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:46:15.000000 pyucrop-1.0.1/pyucrop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-11 09:46:15.000000 pyucrop-1.0.1/pyucrop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 09:46:15.797882 pyucrop-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-11 09:46:14.000000 pyucrop-1.0.1/setup.py
```

### Comparing `pyucrop-1.0.0/setup.py` & `pyucrop-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 with open(r'C:\Users\User\Desktop\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='pyucrop',
-	version='1.0.0',
+	version='1.0.1',
 	author='Redpiar',
 	author_email='Regeonwix@gmail.com',
-	description='test',
+	description='api for photo',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=['pyucrop'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
```

