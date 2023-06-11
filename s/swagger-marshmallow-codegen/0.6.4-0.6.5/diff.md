# Comparing `tmp/swagger-marshmallow-codegen-0.6.4.tar.gz` & `tmp/swagger-marshmallow-codegen-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swagger-marshmallow-codegen-0.6.4.tar", last modified: Tue Jan 26 12:44:54 2021, max compression
+gzip compressed data, was "swagger-marshmallow-codegen-0.6.5.tar", last modified: Sat Jun 10 17:51:50 2023, max compression
```

## Comparing `swagger-marshmallow-codegen-0.6.4.tar` & `swagger-marshmallow-codegen-0.6.5.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/
--rw-r--r--   0 nao        (501) staff       (20)     8489 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/PKG-INFO
--rw-r--r--   0 nao        (501) staff       (20)     5980 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/README.md
--rw-r--r--   0 nao        (501) staff       (20)      617 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/setup.cfg
--rw-r--r--   0 nao        (501) staff       (20)      972 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/setup.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/
--rw-r--r--   0 nao        (501) staff       (20)      100 2021-01-26 12:29:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)       92 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/__main__.py
--rw-r--r--   0 nao        (501) staff       (20)       22 2021-01-26 12:29:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/_version.py
--rw-r--r--   0 nao        (501) staff       (20)     2097 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/cmd.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/
--rw-r--r--   0 nao        (501) staff       (20)     2952 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)      560 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/config.py
--rw-r--r--   0 nao        (501) staff       (20)     5129 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/context.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v2/
--rw-r--r--   0 nao        (501) staff       (20)        0 2020-10-31 17:56:00.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v2/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)     3283 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v2/accessor.py
--rw-r--r--   0 nao        (501) staff       (20)    26172 2020-11-15 05:14:34.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v2/codegen.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v3/
--rw-r--r--   0 nao        (501) staff       (20)        0 2020-10-31 17:56:00.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v3/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)      260 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v3/accessor.py
--rw-r--r--   0 nao        (501) staff       (20)       56 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v3/codegen.py
--rw-r--r--   0 nao        (501) staff       (20)       88 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/constants.py
--rw-r--r--   0 nao        (501) staff       (20)     4056 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/dispatcher.py
--rw-r--r--   0 nao        (501) staff       (20)     3408 2020-11-07 17:29:16.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/driver.py
--rw-r--r--   0 nao        (501) staff       (20)      779 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/evil.py
--rw-r--r--   0 nao        (501) staff       (20)     1094 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/fields.py
--rw-r--r--   0 nao        (501) staff       (20)     1014 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/langhelpers.py
--rw-r--r--   0 nao        (501) staff       (20)     3485 2021-01-26 11:24:06.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/lifting.py
--rw-r--r--   0 nao        (501) staff       (20)       97 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/loading.py
--rw-r--r--   0 nao        (501) staff       (20)     7280 2021-01-26 11:40:12.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/resolver.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/schema/
--rw-r--r--   0 nao        (501) staff       (20)      119 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/schema/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)     2987 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/schema/extra.py
--rw-r--r--   0 nao        (501) staff       (20)     3602 2020-11-04 04:08:27.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/schema/legacy.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/
--rw-r--r--   0 nao        (501) staff       (20)      143 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/00simple-object.py
--rw-r--r--   0 nao        (501) staff       (20)      222 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/01simple-primitive.py
--rw-r--r--   0 nao        (501) staff       (20)      305 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/02nesting.py
--rw-r--r--   0 nao        (501) staff       (20)      233 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/03self-nesting.py
--rw-r--r--   0 nao        (501) staff       (20)      317 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/04inline-nesting.py
--rw-r--r--   0 nao        (501) staff       (20)      225 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/05additionalProperties-without-properties.py
--rw-r--r--   0 nao        (501) staff       (20)      406 2020-11-07 12:10:15.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/06additionalProperties.py
--rw-r--r--   0 nao        (501) staff       (20)      487 2020-11-07 12:10:15.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/07additionalProperties-with-bool.py
--rw-r--r--   0 nao        (501) staff       (20)        0 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v2dst/__init__.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/
--rw-r--r--   0 nao        (501) staff       (20)      143 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/00simple-object.py
--rw-r--r--   0 nao        (501) staff       (20)      222 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/01simple-primitive.py
--rw-r--r--   0 nao        (501) staff       (20)      305 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/02nesting.py
--rw-r--r--   0 nao        (501) staff       (20)      233 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/03self-nesting.py
--rw-r--r--   0 nao        (501) staff       (20)      317 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/04inline-nesting.py
--rw-r--r--   0 nao        (501) staff       (20)      225 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/05additionalProperties-without-properties.py
--rw-r--r--   0 nao        (501) staff       (20)      406 2020-11-07 12:10:15.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/06additionalProperties.py
--rw-r--r--   0 nao        (501) staff       (20)      487 2020-11-07 12:10:15.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/07additionalProperties-with-bool.py
--rw-r--r--   0 nao        (501) staff       (20)        0 2020-11-04 18:05:41.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/tests/v3dst/__init__.py
--rw-r--r--   0 nao        (501) staff       (20)     1520 2021-01-26 11:45:01.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/validate.py
-drwxr-xr-x   0 nao        (501) staff       (20)        0 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/
--rw-r--r--   0 nao        (501) staff       (20)     8489 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/PKG-INFO
--rw-r--r--   0 nao        (501) staff       (20)     2660 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/SOURCES.txt
--rw-r--r--   0 nao        (501) staff       (20)        1 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/dependency_links.txt
--rw-r--r--   0 nao        (501) staff       (20)       86 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/entry_points.txt
--rw-r--r--   0 nao        (501) staff       (20)        1 2020-02-06 16:13:29.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/not-zip-safe
--rw-r--r--   0 nao        (501) staff       (20)      124 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/requires.txt
--rw-r--r--   0 nao        (501) staff       (20)       28 2021-01-26 12:44:54.000000 swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/top_level.txt
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.770500 swagger-marshmallow-codegen-0.6.5/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1063 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/LICENSE
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     6612 2023-06-10 17:51:50.770500 swagger-marshmallow-codegen-0.6.5/PKG-INFO
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     5980 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/README.md
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      617 2023-06-10 17:51:50.770500 swagger-marshmallow-codegen-0.6.5/setup.cfg
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      991 2023-06-10 17:43:32.000000 swagger-marshmallow-codegen-0.6.5/setup.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.759666 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      100 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       92 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/__main__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       22 2023-06-10 17:51:31.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/_version.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2097 2023-06-10 17:28:57.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/cmd.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.759666 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2952 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      560 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/config.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     5129 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/context.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.759666 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v2/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v2/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     3283 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v2/accessor.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)    26172 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v2/codegen.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.759666 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v3/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v3/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      260 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v3/accessor.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       56 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v3/codegen.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       88 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/constants.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     4056 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/dispatcher.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     3408 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/driver.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      779 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/evil.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1094 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/fields.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1014 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/langhelpers.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     3485 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/lifting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       80 2023-06-10 17:43:32.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/loading.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     7280 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/resolver.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.770500 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/schema/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      119 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/schema/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2987 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/schema/extra.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     3602 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/schema/legacy.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.748833 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.770500 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      143 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/00simple-object.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      222 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/01simple-primitive.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      305 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/02nesting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      233 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/03self-nesting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      317 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/04inline-nesting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      225 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/05additionalProperties-without-properties.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      406 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/06additionalProperties.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      487 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/07additionalProperties-with-bool.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v2dst/__init__.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.770500 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      143 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/00simple-object.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      222 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/01simple-primitive.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      305 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/02nesting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      233 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/03self-nesting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      317 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/04inline-nesting.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      225 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/05additionalProperties-without-properties.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      406 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/06additionalProperties.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      487 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/07additionalProperties-with-bool.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/tests/v3dst/__init__.py
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     1520 2023-06-10 17:24:40.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/validate.py
+drwxr-xr-x   0 podhmo    (1000) podhmo    (1000)        0 2023-06-10 17:51:50.759666 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     6612 2023-06-10 17:51:50.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)     2668 2023-06-10 17:51:50.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        1 2023-06-10 17:51:50.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       86 2023-06-10 17:51:50.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/entry_points.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)        1 2023-06-10 17:25:29.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/not-zip-safe
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)      131 2023-06-10 17:51:50.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/requires.txt
+-rw-r--r--   0 podhmo    (1000) podhmo    (1000)       28 2023-06-10 17:51:50.000000 swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/top_level.txt
```

### Comparing `swagger-marshmallow-codegen-0.6.4/PKG-INFO` & `swagger-marshmallow-codegen-0.6.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,254 +1,257 @@
 Metadata-Version: 2.1
 Name: swagger-marshmallow-codegen
-Version: 0.6.4
+Version: 0.6.5
 Summary: "generating marshmallow's schema from swagger definition file"
 Home-page: https://github.com/podhmo/swagger-marshmallow-codegen
 Author: podhmo
 Author-email: ababjam61+github@gmail.com
 License: UNKNOWN
-Description: swagger-marshmallow-codegen ![Python package](https://github.com/podhmo/swagger-marshmallow-codegen/workflows/Python%20package/badge.svg) [![PyPi version](https://img.shields.io/pypi/v/swagger-marshmallow-codegen.svg)](https://pypi.python.org/pypi/swagger-marshmallow-codegen) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/download/releases/3.7.0/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
-        ========================================
-        
-        concepts
-        --------
-        
-        - Code generation is better than meta programming
-        - Don't touch me(generated code) if you can
-        
-        todo: write down detail.
-        
-        examples
-        --------
-        
-        ``` bash
-        $ swagger-marshmallow-codegen definition.yaml > definition.py
-        ```
-        
-        definition.yaml
-        
-        ``` yaml
-        # todo: gentle example
-        definitions:
-          default:
-            properties:
-              string:
-                type: string
-                default: "default"
-              integer:
-                type: integer
-                default: 10
-              boolean:
-                type: boolean
-                default: true
-              date:
-                type: string
-                format: date
-                default: 2000-01-01
-              datetime:
-                type: string
-                format: date-time
-                default: 2000-01-01T01:01:01Z
-              object:
-                type: object
-                properties:
-                  name:
-                    type: string
-                    default: foo
-                  age:
-                    type: integer
-                    default: 20
-                default:
-                  name: foo
-                  age: 20
-              array:
-                type: array
-                items:
-                  type: integer
-                default:
-                  - 1
-                  - 2
-                  - 3
-        
-          length-validation:
-            type: object
-            properties:
-              s0:
-                type: string
-              s1:
-                type: string
-                maxLength: 10
-              s2:
-                type: string
-                minLength: 5
-              s3:
-                type: string
-                maxLength: 10
-                minLength: 5
-        
-          maximum-validation:
-            type: object
-            properties:
-              n0:
-                type: number
-                maximum: 100
-              n1:
-                type: number
-                maximum: 100
-                exclusiveMaximum: true
-              n2:
-                type: number
-                maximum: 100
-                exclusiveMaximum: false
-              m0:
-                type: number
-                minimum: 100
-              m1:
-                type: number
-                minimum: 100
-                exclusiveMinimum: true
-              m2:
-                type: number
-                minimum: 100
-                exclusiveMinimum: false
-        
-          regex-validation:
-            type: object
-            properties:
-              team:
-                type: string
-                pattern: team[1-9][0-9]+
-              team2:
-                type: string
-                pattern: team[1-9][0-9]+
-                maxLength: 10
-        
-          array-validation:
-            type: object
-            properties:
-              nums:
-                type: array
-                items:
-                  type: integer
-                maxItems: 10
-                minItems: 1
-                uniqueItems: true
-        
-          color:
-            type: string
-            enum:
-              - R
-              - G
-              - B
-          yen:
-            type: integer
-            enum:
-              - 1
-              - 5
-              - 10
-              - 50
-              - 100
-              - 500
-              - 1000
-              - 5000
-              - 10000
-          huge-yen:
-            typ
-        ```
-        
-        
-        definition.py
-        
-        ``` python
-        # -*- coding:utf-8 -*-
-        # this is auto-generated by swagger-marshmallow-codegen
-        from marshmallow import (
-            Schema,
-            fields
-        )
-        import datetime
-        from collections import OrderedDict
-        from marshmallow.validate import (
-            Length,
-            OneOf,
-            Regexp
-        )
-        from swagger_marshmallow_codegen.validate import (
-            ItemsRange,
-            MultipleOf,
-            Range,
-            Unique
-        )
-        import re
-        
-        
-        class Default(Schema):
-            string = fields.String(missing=lambda: 'default')
-            integer = fields.Integer(missing=lambda: 10)
-            boolean = fields.Boolean(missing=lambda: True)
-            date = fields.Date(missing=lambda: datetime.date(2000, 1, 1))
-            datetime = fields.DateTime(missing=lambda: datetime.datetime(2000, 1, 1, 1, 1, 1))
-            object = fields.Nested('DefaultObject', missing=lambda: OrderedDict([('name', 'foo'), ('age', 20)]))
-            array = fields.List(fields.Integer(), missing=lambda: [1, 2, 3])
-        
-        
-        class DefaultObject(Schema):
-            name = fields.String(missing=lambda: 'foo')
-            age = fields.Integer(missing=lambda: 20)
-        
-        
-        class Length_validation(Schema):
-            s0 = fields.String()
-            s1 = fields.String(validate=[Length(min=None, max=10, equal=None)])
-            s2 = fields.String(validate=[Length(min=5, max=None, equal=None)])
-            s3 = fields.String(validate=[Length(min=5, max=10, equal=None)])
-        
-        
-        class Maximum_validation(Schema):
-            n0 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
-            n1 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=False)])
-            n2 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
-            m0 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
-            m1 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=False, max_inclusive=True)])
-            m2 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
-        
-        
-        class Regex_validation(Schema):
-            team = fields.String(validate=[Regexp(regex=re.compile('team[1-9][0-9]+'))])
-            team2 = fields.String(validate=[Length(min=None, max=10, equal=None), Regexp(regex=re.compile('team[1-9][0-9]+'))])
-        
-        
-        class Array_validation(Schema):
-            nums = fields.List(fields.Integer(), validate=[ItemsRange(min=1, max=10, min_inclusive=True, max_inclusive=True), Unique()])
-        
-        
-        class Enum_validation(Schema):
-            name = fields.String(required=True)
-            money = fields.Integer(validate=[OneOf(choices=[1, 5, 10, 50, 100, 500, 1000, 5000, 10000], labels=[])])
-            deposit = fields.Integer(validate=[MultipleOf(n=10000)])
-            color = fields.String(required=True, validate=[OneOf(choices=['R', 'G', 'B'], labels=[])])
-        ```
-        
-        customization:
-        --------------
-        
-        todo: write down
-        
-        <https://github.com/podhmo/swagger-marshmallow-codegen/issues/1>
-        
-        todo:
-        -----
-        
-        -  `x-marshmallow-name`
-        
-          [image]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen.svg?branch=master
-          [1]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen
-        
 Keywords: swagger,codegen,marshmallow,code-generation,schema
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: testing
+License-File: LICENSE
+
+swagger-marshmallow-codegen ![Python package](https://github.com/podhmo/swagger-marshmallow-codegen/workflows/Python%20package/badge.svg) [![PyPi version](https://img.shields.io/pypi/v/swagger-marshmallow-codegen.svg)](https://pypi.python.org/pypi/swagger-marshmallow-codegen) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/download/releases/3.7.0/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
+========================================
+
+concepts
+--------
+
+- Code generation is better than meta programming
+- Don't touch me(generated code) if you can
+
+todo: write down detail.
+
+examples
+--------
+
+``` bash
+$ swagger-marshmallow-codegen definition.yaml > definition.py
+```
+
+definition.yaml
+
+``` yaml
+# todo: gentle example
+definitions:
+  default:
+    properties:
+      string:
+        type: string
+        default: "default"
+      integer:
+        type: integer
+        default: 10
+      boolean:
+        type: boolean
+        default: true
+      date:
+        type: string
+        format: date
+        default: 2000-01-01
+      datetime:
+        type: string
+        format: date-time
+        default: 2000-01-01T01:01:01Z
+      object:
+        type: object
+        properties:
+          name:
+            type: string
+            default: foo
+          age:
+            type: integer
+            default: 20
+        default:
+          name: foo
+          age: 20
+      array:
+        type: array
+        items:
+          type: integer
+        default:
+          - 1
+          - 2
+          - 3
+
+  length-validation:
+    type: object
+    properties:
+      s0:
+        type: string
+      s1:
+        type: string
+        maxLength: 10
+      s2:
+        type: string
+        minLength: 5
+      s3:
+        type: string
+        maxLength: 10
+        minLength: 5
+
+  maximum-validation:
+    type: object
+    properties:
+      n0:
+        type: number
+        maximum: 100
+      n1:
+        type: number
+        maximum: 100
+        exclusiveMaximum: true
+      n2:
+        type: number
+        maximum: 100
+        exclusiveMaximum: false
+      m0:
+        type: number
+        minimum: 100
+      m1:
+        type: number
+        minimum: 100
+        exclusiveMinimum: true
+      m2:
+        type: number
+        minimum: 100
+        exclusiveMinimum: false
+
+  regex-validation:
+    type: object
+    properties:
+      team:
+        type: string
+        pattern: team[1-9][0-9]+
+      team2:
+        type: string
+        pattern: team[1-9][0-9]+
+        maxLength: 10
+
+  array-validation:
+    type: object
+    properties:
+      nums:
+        type: array
+        items:
+          type: integer
+        maxItems: 10
+        minItems: 1
+        uniqueItems: true
+
+  color:
+    type: string
+    enum:
+      - R
+      - G
+      - B
+  yen:
+    type: integer
+    enum:
+      - 1
+      - 5
+      - 10
+      - 50
+      - 100
+      - 500
+      - 1000
+      - 5000
+      - 10000
+  huge-yen:
+    typ
+```
+
+
+definition.py
+
+``` python
+# -*- coding:utf-8 -*-
+# this is auto-generated by swagger-marshmallow-codegen
+from marshmallow import (
+    Schema,
+    fields
+)
+import datetime
+from collections import OrderedDict
+from marshmallow.validate import (
+    Length,
+    OneOf,
+    Regexp
+)
+from swagger_marshmallow_codegen.validate import (
+    ItemsRange,
+    MultipleOf,
+    Range,
+    Unique
+)
+import re
+
+
+class Default(Schema):
+    string = fields.String(missing=lambda: 'default')
+    integer = fields.Integer(missing=lambda: 10)
+    boolean = fields.Boolean(missing=lambda: True)
+    date = fields.Date(missing=lambda: datetime.date(2000, 1, 1))
+    datetime = fields.DateTime(missing=lambda: datetime.datetime(2000, 1, 1, 1, 1, 1))
+    object = fields.Nested('DefaultObject', missing=lambda: OrderedDict([('name', 'foo'), ('age', 20)]))
+    array = fields.List(fields.Integer(), missing=lambda: [1, 2, 3])
+
+
+class DefaultObject(Schema):
+    name = fields.String(missing=lambda: 'foo')
+    age = fields.Integer(missing=lambda: 20)
+
+
+class Length_validation(Schema):
+    s0 = fields.String()
+    s1 = fields.String(validate=[Length(min=None, max=10, equal=None)])
+    s2 = fields.String(validate=[Length(min=5, max=None, equal=None)])
+    s3 = fields.String(validate=[Length(min=5, max=10, equal=None)])
+
+
+class Maximum_validation(Schema):
+    n0 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
+    n1 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=False)])
+    n2 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
+    m0 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
+    m1 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=False, max_inclusive=True)])
+    m2 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
+
+
+class Regex_validation(Schema):
+    team = fields.String(validate=[Regexp(regex=re.compile('team[1-9][0-9]+'))])
+    team2 = fields.String(validate=[Length(min=None, max=10, equal=None), Regexp(regex=re.compile('team[1-9][0-9]+'))])
+
+
+class Array_validation(Schema):
+    nums = fields.List(fields.Integer(), validate=[ItemsRange(min=1, max=10, min_inclusive=True, max_inclusive=True), Unique()])
+
+
+class Enum_validation(Schema):
+    name = fields.String(required=True)
+    money = fields.Integer(validate=[OneOf(choices=[1, 5, 10, 50, 100, 500, 1000, 5000, 10000], labels=[])])
+    deposit = fields.Integer(validate=[MultipleOf(n=10000)])
+    color = fields.String(required=True, validate=[OneOf(choices=['R', 'G', 'B'], labels=[])])
+```
+
+customization:
+--------------
+
+todo: write down
+
+<https://github.com/podhmo/swagger-marshmallow-codegen/issues/1>
+
+todo:
+-----
+
+-  `x-marshmallow-name`
+
+  [image]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen.svg?branch=master
+  [1]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen
+
+
```

### Comparing `swagger-marshmallow-codegen-0.6.4/README.md` & `swagger-marshmallow-codegen-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/setup.cfg` & `swagger-marshmallow-codegen-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/setup.py` & `swagger-marshmallow-codegen-0.6.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from setuptools import setup, find_packages
 
 install_requires = [
-    "dictknife",
-    "PyYAML",
+    "dictknife[load]>=0.14.0",  # for ruamel.yaml
     "prestring",
     "marshmallow>=3.0.0",
     "magicalimport",
     "typing_extensions",
 ]
 
 docs_extras = []
```

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/cmd.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/cmd.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/__init__.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/config.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/config.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/context.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/context.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v2/accessor.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v2/accessor.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/codegen/v2/codegen.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/codegen/v2/codegen.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/dispatcher.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/dispatcher.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/driver.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/driver.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/evil.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/evil.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/fields.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/fields.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/langhelpers.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/langhelpers.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/lifting.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/lifting.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/resolver.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/resolver.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/schema/extra.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/schema/extra.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/schema/legacy.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/schema/legacy.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen/validate.py` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen/validate.py`

 * *Files identical despite different names*

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/PKG-INFO` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,254 +1,257 @@
 Metadata-Version: 2.1
 Name: swagger-marshmallow-codegen
-Version: 0.6.4
+Version: 0.6.5
 Summary: "generating marshmallow's schema from swagger definition file"
 Home-page: https://github.com/podhmo/swagger-marshmallow-codegen
 Author: podhmo
 Author-email: ababjam61+github@gmail.com
 License: UNKNOWN
-Description: swagger-marshmallow-codegen ![Python package](https://github.com/podhmo/swagger-marshmallow-codegen/workflows/Python%20package/badge.svg) [![PyPi version](https://img.shields.io/pypi/v/swagger-marshmallow-codegen.svg)](https://pypi.python.org/pypi/swagger-marshmallow-codegen) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/download/releases/3.7.0/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
-        ========================================
-        
-        concepts
-        --------
-        
-        - Code generation is better than meta programming
-        - Don't touch me(generated code) if you can
-        
-        todo: write down detail.
-        
-        examples
-        --------
-        
-        ``` bash
-        $ swagger-marshmallow-codegen definition.yaml > definition.py
-        ```
-        
-        definition.yaml
-        
-        ``` yaml
-        # todo: gentle example
-        definitions:
-          default:
-            properties:
-              string:
-                type: string
-                default: "default"
-              integer:
-                type: integer
-                default: 10
-              boolean:
-                type: boolean
-                default: true
-              date:
-                type: string
-                format: date
-                default: 2000-01-01
-              datetime:
-                type: string
-                format: date-time
-                default: 2000-01-01T01:01:01Z
-              object:
-                type: object
-                properties:
-                  name:
-                    type: string
-                    default: foo
-                  age:
-                    type: integer
-                    default: 20
-                default:
-                  name: foo
-                  age: 20
-              array:
-                type: array
-                items:
-                  type: integer
-                default:
-                  - 1
-                  - 2
-                  - 3
-        
-          length-validation:
-            type: object
-            properties:
-              s0:
-                type: string
-              s1:
-                type: string
-                maxLength: 10
-              s2:
-                type: string
-                minLength: 5
-              s3:
-                type: string
-                maxLength: 10
-                minLength: 5
-        
-          maximum-validation:
-            type: object
-            properties:
-              n0:
-                type: number
-                maximum: 100
-              n1:
-                type: number
-                maximum: 100
-                exclusiveMaximum: true
-              n2:
-                type: number
-                maximum: 100
-                exclusiveMaximum: false
-              m0:
-                type: number
-                minimum: 100
-              m1:
-                type: number
-                minimum: 100
-                exclusiveMinimum: true
-              m2:
-                type: number
-                minimum: 100
-                exclusiveMinimum: false
-        
-          regex-validation:
-            type: object
-            properties:
-              team:
-                type: string
-                pattern: team[1-9][0-9]+
-              team2:
-                type: string
-                pattern: team[1-9][0-9]+
-                maxLength: 10
-        
-          array-validation:
-            type: object
-            properties:
-              nums:
-                type: array
-                items:
-                  type: integer
-                maxItems: 10
-                minItems: 1
-                uniqueItems: true
-        
-          color:
-            type: string
-            enum:
-              - R
-              - G
-              - B
-          yen:
-            type: integer
-            enum:
-              - 1
-              - 5
-              - 10
-              - 50
-              - 100
-              - 500
-              - 1000
-              - 5000
-              - 10000
-          huge-yen:
-            typ
-        ```
-        
-        
-        definition.py
-        
-        ``` python
-        # -*- coding:utf-8 -*-
-        # this is auto-generated by swagger-marshmallow-codegen
-        from marshmallow import (
-            Schema,
-            fields
-        )
-        import datetime
-        from collections import OrderedDict
-        from marshmallow.validate import (
-            Length,
-            OneOf,
-            Regexp
-        )
-        from swagger_marshmallow_codegen.validate import (
-            ItemsRange,
-            MultipleOf,
-            Range,
-            Unique
-        )
-        import re
-        
-        
-        class Default(Schema):
-            string = fields.String(missing=lambda: 'default')
-            integer = fields.Integer(missing=lambda: 10)
-            boolean = fields.Boolean(missing=lambda: True)
-            date = fields.Date(missing=lambda: datetime.date(2000, 1, 1))
-            datetime = fields.DateTime(missing=lambda: datetime.datetime(2000, 1, 1, 1, 1, 1))
-            object = fields.Nested('DefaultObject', missing=lambda: OrderedDict([('name', 'foo'), ('age', 20)]))
-            array = fields.List(fields.Integer(), missing=lambda: [1, 2, 3])
-        
-        
-        class DefaultObject(Schema):
-            name = fields.String(missing=lambda: 'foo')
-            age = fields.Integer(missing=lambda: 20)
-        
-        
-        class Length_validation(Schema):
-            s0 = fields.String()
-            s1 = fields.String(validate=[Length(min=None, max=10, equal=None)])
-            s2 = fields.String(validate=[Length(min=5, max=None, equal=None)])
-            s3 = fields.String(validate=[Length(min=5, max=10, equal=None)])
-        
-        
-        class Maximum_validation(Schema):
-            n0 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
-            n1 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=False)])
-            n2 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
-            m0 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
-            m1 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=False, max_inclusive=True)])
-            m2 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
-        
-        
-        class Regex_validation(Schema):
-            team = fields.String(validate=[Regexp(regex=re.compile('team[1-9][0-9]+'))])
-            team2 = fields.String(validate=[Length(min=None, max=10, equal=None), Regexp(regex=re.compile('team[1-9][0-9]+'))])
-        
-        
-        class Array_validation(Schema):
-            nums = fields.List(fields.Integer(), validate=[ItemsRange(min=1, max=10, min_inclusive=True, max_inclusive=True), Unique()])
-        
-        
-        class Enum_validation(Schema):
-            name = fields.String(required=True)
-            money = fields.Integer(validate=[OneOf(choices=[1, 5, 10, 50, 100, 500, 1000, 5000, 10000], labels=[])])
-            deposit = fields.Integer(validate=[MultipleOf(n=10000)])
-            color = fields.String(required=True, validate=[OneOf(choices=['R', 'G', 'B'], labels=[])])
-        ```
-        
-        customization:
-        --------------
-        
-        todo: write down
-        
-        <https://github.com/podhmo/swagger-marshmallow-codegen/issues/1>
-        
-        todo:
-        -----
-        
-        -  `x-marshmallow-name`
-        
-          [image]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen.svg?branch=master
-          [1]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen
-        
 Keywords: swagger,codegen,marshmallow,code-generation,schema
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: testing
+License-File: LICENSE
+
+swagger-marshmallow-codegen ![Python package](https://github.com/podhmo/swagger-marshmallow-codegen/workflows/Python%20package/badge.svg) [![PyPi version](https://img.shields.io/pypi/v/swagger-marshmallow-codegen.svg)](https://pypi.python.org/pypi/swagger-marshmallow-codegen) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/download/releases/3.7.0/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
+========================================
+
+concepts
+--------
+
+- Code generation is better than meta programming
+- Don't touch me(generated code) if you can
+
+todo: write down detail.
+
+examples
+--------
+
+``` bash
+$ swagger-marshmallow-codegen definition.yaml > definition.py
+```
+
+definition.yaml
+
+``` yaml
+# todo: gentle example
+definitions:
+  default:
+    properties:
+      string:
+        type: string
+        default: "default"
+      integer:
+        type: integer
+        default: 10
+      boolean:
+        type: boolean
+        default: true
+      date:
+        type: string
+        format: date
+        default: 2000-01-01
+      datetime:
+        type: string
+        format: date-time
+        default: 2000-01-01T01:01:01Z
+      object:
+        type: object
+        properties:
+          name:
+            type: string
+            default: foo
+          age:
+            type: integer
+            default: 20
+        default:
+          name: foo
+          age: 20
+      array:
+        type: array
+        items:
+          type: integer
+        default:
+          - 1
+          - 2
+          - 3
+
+  length-validation:
+    type: object
+    properties:
+      s0:
+        type: string
+      s1:
+        type: string
+        maxLength: 10
+      s2:
+        type: string
+        minLength: 5
+      s3:
+        type: string
+        maxLength: 10
+        minLength: 5
+
+  maximum-validation:
+    type: object
+    properties:
+      n0:
+        type: number
+        maximum: 100
+      n1:
+        type: number
+        maximum: 100
+        exclusiveMaximum: true
+      n2:
+        type: number
+        maximum: 100
+        exclusiveMaximum: false
+      m0:
+        type: number
+        minimum: 100
+      m1:
+        type: number
+        minimum: 100
+        exclusiveMinimum: true
+      m2:
+        type: number
+        minimum: 100
+        exclusiveMinimum: false
+
+  regex-validation:
+    type: object
+    properties:
+      team:
+        type: string
+        pattern: team[1-9][0-9]+
+      team2:
+        type: string
+        pattern: team[1-9][0-9]+
+        maxLength: 10
+
+  array-validation:
+    type: object
+    properties:
+      nums:
+        type: array
+        items:
+          type: integer
+        maxItems: 10
+        minItems: 1
+        uniqueItems: true
+
+  color:
+    type: string
+    enum:
+      - R
+      - G
+      - B
+  yen:
+    type: integer
+    enum:
+      - 1
+      - 5
+      - 10
+      - 50
+      - 100
+      - 500
+      - 1000
+      - 5000
+      - 10000
+  huge-yen:
+    typ
+```
+
+
+definition.py
+
+``` python
+# -*- coding:utf-8 -*-
+# this is auto-generated by swagger-marshmallow-codegen
+from marshmallow import (
+    Schema,
+    fields
+)
+import datetime
+from collections import OrderedDict
+from marshmallow.validate import (
+    Length,
+    OneOf,
+    Regexp
+)
+from swagger_marshmallow_codegen.validate import (
+    ItemsRange,
+    MultipleOf,
+    Range,
+    Unique
+)
+import re
+
+
+class Default(Schema):
+    string = fields.String(missing=lambda: 'default')
+    integer = fields.Integer(missing=lambda: 10)
+    boolean = fields.Boolean(missing=lambda: True)
+    date = fields.Date(missing=lambda: datetime.date(2000, 1, 1))
+    datetime = fields.DateTime(missing=lambda: datetime.datetime(2000, 1, 1, 1, 1, 1))
+    object = fields.Nested('DefaultObject', missing=lambda: OrderedDict([('name', 'foo'), ('age', 20)]))
+    array = fields.List(fields.Integer(), missing=lambda: [1, 2, 3])
+
+
+class DefaultObject(Schema):
+    name = fields.String(missing=lambda: 'foo')
+    age = fields.Integer(missing=lambda: 20)
+
+
+class Length_validation(Schema):
+    s0 = fields.String()
+    s1 = fields.String(validate=[Length(min=None, max=10, equal=None)])
+    s2 = fields.String(validate=[Length(min=5, max=None, equal=None)])
+    s3 = fields.String(validate=[Length(min=5, max=10, equal=None)])
+
+
+class Maximum_validation(Schema):
+    n0 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
+    n1 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=False)])
+    n2 = fields.Number(validate=[Range(min=None, max=100, min_inclusive=True, max_inclusive=True)])
+    m0 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
+    m1 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=False, max_inclusive=True)])
+    m2 = fields.Number(validate=[Range(min=100, max=None, min_inclusive=True, max_inclusive=True)])
+
+
+class Regex_validation(Schema):
+    team = fields.String(validate=[Regexp(regex=re.compile('team[1-9][0-9]+'))])
+    team2 = fields.String(validate=[Length(min=None, max=10, equal=None), Regexp(regex=re.compile('team[1-9][0-9]+'))])
+
+
+class Array_validation(Schema):
+    nums = fields.List(fields.Integer(), validate=[ItemsRange(min=1, max=10, min_inclusive=True, max_inclusive=True), Unique()])
+
+
+class Enum_validation(Schema):
+    name = fields.String(required=True)
+    money = fields.Integer(validate=[OneOf(choices=[1, 5, 10, 50, 100, 500, 1000, 5000, 10000], labels=[])])
+    deposit = fields.Integer(validate=[MultipleOf(n=10000)])
+    color = fields.String(required=True, validate=[OneOf(choices=['R', 'G', 'B'], labels=[])])
+```
+
+customization:
+--------------
+
+todo: write down
+
+<https://github.com/podhmo/swagger-marshmallow-codegen/issues/1>
+
+todo:
+-----
+
+-  `x-marshmallow-name`
+
+  [image]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen.svg?branch=master
+  [1]: https://travis-ci.org/podhmo/swagger-marshmallow-codegen
+
+
```

### Comparing `swagger-marshmallow-codegen-0.6.4/swagger_marshmallow_codegen.egg-info/SOURCES.txt` & `swagger-marshmallow-codegen-0.6.5/swagger_marshmallow_codegen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 swagger_marshmallow_codegen/__init__.py
 swagger_marshmallow_codegen/__main__.py
 swagger_marshmallow_codegen/_version.py
 swagger_marshmallow_codegen/cmd.py
```

