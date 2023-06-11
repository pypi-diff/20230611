# Comparing `tmp/pyquizzer-0.0.1a2.tar.gz` & `tmp/pyquizzer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquizzer-0.0.1a2.tar", max compression
+gzip compressed data, was "pyquizzer-0.0.2.tar", max compression
```

## Comparing `pyquizzer-0.0.1a2.tar` & `pyquizzer-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rwxr-xr-x   0        0        0       11 2023-06-04 06:57:15.811368 pyquizzer-0.0.1a2/README.md
--rw-r--r--   0        0        0      420 2023-06-11 08:13:09.079190 pyquizzer-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 06:53:20.851812 pyquizzer-0.0.1a2/pyquizzer.py
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 pyquizzer-0.0.1a2/PKG-INFO
+-rwxr-xr-x   0        0        0       11 2023-06-04 06:57:15.811368 pyquizzer-0.0.2/README.md
+-rwxr-xr-x   0        0        0       35 2023-06-11 09:12:23.455506 pyquizzer-0.0.2/changelog.md
+-rw-r--r--   0        0        0      892 2023-06-11 09:15:39.622786 pyquizzer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 06:53:20.851812 pyquizzer-0.0.2/pyquizzer.py
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 pyquizzer-0.0.2/PKG-INFO
```

