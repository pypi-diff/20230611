# Comparing `tmp/SATOSA-8.3.0.tar.gz` & `tmp/SATOSA-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SATOSA-8.3.0.tar", last modified: Thu Jun  8 17:00:28 2023, max compression
+gzip compressed data, was "SATOSA-8.4.0.tar", last modified: Sun Jun 11 17:23:42 2023, max compression
```

## Comparing `SATOSA-8.3.0.tar` & `SATOSA-8.4.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.663773 SATOSA-8.3.0/
--rw-r--r--   0 ivan       (501) staff       (20)    10177 2021-05-24 16:59:06.000000 SATOSA-8.3.0/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)     1313 2021-05-24 16:59:06.000000 SATOSA-8.3.0/NOTICE
--rw-r--r--   0 ivan       (501) staff       (20)      527 2023-06-08 17:00:28.663859 SATOSA-8.3.0/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     3666 2022-11-15 12:05:51.000000 SATOSA-8.3.0/README.md
--rw-r--r--   0 ivan       (501) staff       (20)      433 2023-06-08 17:00:28.664256 SATOSA-8.3.0/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1133 2023-06-08 16:56:21.000000 SATOSA-8.3.0/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.647627 SATOSA-8.3.0/src/
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.650202 SATOSA-8.3.0/src/SATOSA.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)      527 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     2597 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      101 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/entry_points.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2021-05-24 17:00:24.000000 SATOSA-8.3.0/src/SATOSA.egg-info/not-zip-safe
--rw-r--r--   0 ivan       (501) staff       (20)      180 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)        7 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/top_level.txt
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.654048 SATOSA-8.3.0/src/satosa/
--rw-r--r--   0 ivan       (501) staff       (20)      139 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     9928 2021-06-29 12:33:38.000000 SATOSA-8.3.0/src/satosa/attribute_mapping.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.656088 SATOSA-8.3.0/src/satosa/backends/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)    12829 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/apple.py
--rw-r--r--   0 ivan       (501) staff       (20)     2616 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/base.py
--rw-r--r--   0 ivan       (501) staff       (20)     3385 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/bitbucket.py
--rw-r--r--   0 ivan       (501) staff       (20)     4519 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/backends/github.py
--rw-r--r--   0 ivan       (501) staff       (20)     4749 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/linkedin.py
--rw-r--r--   0 ivan       (501) staff       (20)    14092 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/oauth.py
--rw-r--r--   0 ivan       (501) staff       (20)    12243 2023-06-08 16:54:50.000000 SATOSA-8.3.0/src/satosa/backends/openid_connect.py
--rw-r--r--   0 ivan       (501) staff       (20)     4222 2022-11-15 11:31:39.000000 SATOSA-8.3.0/src/satosa/backends/orcid.py
--rw-r--r--   0 ivan       (501) staff       (20)     2895 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/reflector.py
--rw-r--r--   0 ivan       (501) staff       (20)    26768 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/saml2.py
--rw-r--r--   0 ivan       (501) staff       (20)    10977 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/base.py
--rw-r--r--   0 ivan       (501) staff       (20)     2674 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/context.py
--rw-r--r--   0 ivan       (501) staff       (20)      138 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/cookies.py
--rw-r--r--   0 ivan       (501) staff       (20)     1283 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/exception.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.657190 SATOSA-8.3.0/src/satosa/frontends/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/frontends/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     3091 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/frontends/base.py
--rw-r--r--   0 ivan       (501) staff       (20)    22308 2022-11-15 11:31:39.000000 SATOSA-8.3.0/src/satosa/frontends/openid_connect.py
--rw-r--r--   0 ivan       (501) staff       (20)     1961 2022-11-29 13:48:33.000000 SATOSA-8.3.0/src/satosa/frontends/ping.py
--rw-r--r--   0 ivan       (501) staff       (20)    48292 2023-06-08 16:54:50.000000 SATOSA-8.3.0/src/satosa/frontends/saml2.py
--rw-r--r--   0 ivan       (501) staff       (20)     4478 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/internal.py
--rw-r--r--   0 ivan       (501) staff       (20)      756 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/logging_util.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.658000 SATOSA-8.3.0/src/satosa/metadata_creation/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/metadata_creation/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     6949 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/metadata_creation/description.py
--rw-r--r--   0 ivan       (501) staff       (20)     6718 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/metadata_creation/saml_metadata.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.661726 SATOSA-8.3.0/src/satosa/micro_services/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     6542 2021-08-08 14:35:57.000000 SATOSA-8.3.0/src/satosa/micro_services/account_linking.py
--rw-r--r--   0 ivan       (501) staff       (20)     3811 2022-11-16 15:32:44.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_authorization.py
--rw-r--r--   0 ivan       (501) staff       (20)     4915 2022-11-15 11:31:39.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_generation.py
--rw-r--r--   0 ivan       (501) staff       (20)     4296 2023-06-07 16:46:41.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_modifications.py
--rw-r--r--   0 ivan       (501) staff       (20)     1091 2021-06-29 12:33:38.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_policy.py
--rw-r--r--   0 ivan       (501) staff       (20)     2312 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1720 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/base.py
--rw-r--r--   0 ivan       (501) staff       (20)     9180 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/consent.py
--rw-r--r--   0 ivan       (501) staff       (20)     4352 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/custom_logging.py
--rw-r--r--   0 ivan       (501) staff       (20)     5720 2022-11-29 13:44:11.000000 SATOSA-8.3.0/src/satosa/micro_services/custom_routing.py
--rw-r--r--   0 ivan       (501) staff       (20)     2245 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/micro_services/disco.py
--rw-r--r--   0 ivan       (501) staff       (20)     3497 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/hasher.py
--rw-r--r--   0 ivan       (501) staff       (20)     1773 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/micro_services/idp_hinting.py
--rw-r--r--   0 ivan       (501) staff       (20)    24072 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/ldap_attribute_store.py
--rw-r--r--   0 ivan       (501) staff       (20)    13447 2023-06-08 16:39:00.000000 SATOSA-8.3.0/src/satosa/micro_services/primary_identifier.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.663323 SATOSA-8.3.0/src/satosa/micro_services/processors/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)      133 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/base_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)      654 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/gender_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1103 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/hash_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1891 2021-10-24 15:05:53.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/regex_sub_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1695 2021-06-29 12:33:38.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/scope_extractor_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)      678 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/scope_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)      686 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/scope_remover_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)    10452 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/plugin_loader.py
--rw-r--r--   0 ivan       (501) staff       (20)     6486 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/proxy_server.py
--rw-r--r--   0 ivan       (501) staff       (20)     3148 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/response.py
--rw-r--r--   0 ivan       (501) staff       (20)     6934 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/routing.py
--rw-r--r--   0 ivan       (501) staff       (20)      489 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/saml_util.py
--rw-r--r--   0 ivan       (501) staff       (20)     5075 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/satosa_config.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.663637 SATOSA-8.3.0/src/satosa/scripts/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/scripts/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     3277 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/scripts/satosa_saml_metadata.py
--rw-r--r--   0 ivan       (501) staff       (20)     7954 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/state.py
--rw-r--r--   0 ivan       (501) staff       (20)     2538 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/util.py
--rw-r--r--   0 ivan       (501) staff       (20)      250 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/version.py
--rw-r--r--   0 ivan       (501) staff       (20)     1062 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/wsgi.py
--rw-r--r--   0 ivan       (501) staff       (20)     1547 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/yaml.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.958978 SATOSA-8.4.0/
+-rw-r--r--   0 ivan       (501) staff       (20)    10177 2021-05-24 16:59:06.000000 SATOSA-8.4.0/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)     1313 2021-05-24 16:59:06.000000 SATOSA-8.4.0/NOTICE
+-rw-r--r--   0 ivan       (501) staff       (20)      679 2023-06-11 17:23:42.959058 SATOSA-8.4.0/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     3666 2022-11-15 12:05:51.000000 SATOSA-8.4.0/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)      433 2023-06-11 17:23:42.960319 SATOSA-8.4.0/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1346 2023-06-11 17:16:44.000000 SATOSA-8.4.0/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.942622 SATOSA-8.4.0/src/
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.944923 SATOSA-8.4.0/src/SATOSA.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)      679 2023-06-11 17:23:42.000000 SATOSA-8.4.0/src/SATOSA.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     2597 2023-06-11 17:23:42.000000 SATOSA-8.4.0/src/SATOSA.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-11 17:23:42.000000 SATOSA-8.4.0/src/SATOSA.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      101 2023-06-11 17:23:42.000000 SATOSA-8.4.0/src/SATOSA.egg-info/entry_points.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2021-05-24 17:00:24.000000 SATOSA-8.4.0/src/SATOSA.egg-info/not-zip-safe
+-rw-r--r--   0 ivan       (501) staff       (20)      234 2023-06-11 17:23:42.000000 SATOSA-8.4.0/src/SATOSA.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        7 2023-06-11 17:23:42.000000 SATOSA-8.4.0/src/SATOSA.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.948966 SATOSA-8.4.0/src/satosa/
+-rw-r--r--   0 ivan       (501) staff       (20)      139 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     9928 2021-06-29 12:33:38.000000 SATOSA-8.4.0/src/satosa/attribute_mapping.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.951223 SATOSA-8.4.0/src/satosa/backends/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/backends/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)    12829 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/backends/apple.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2616 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/backends/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3385 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/backends/bitbucket.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4519 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/backends/github.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4749 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/backends/linkedin.py
+-rw-r--r--   0 ivan       (501) staff       (20)    14663 2023-06-11 15:38:44.000000 SATOSA-8.4.0/src/satosa/backends/oauth.py
+-rw-r--r--   0 ivan       (501) staff       (20)    12243 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/backends/openid_connect.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4222 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/backends/orcid.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2895 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/backends/reflector.py
+-rw-r--r--   0 ivan       (501) staff       (20)    27371 2023-06-11 15:38:44.000000 SATOSA-8.4.0/src/satosa/backends/saml2.py
+-rw-r--r--   0 ivan       (501) staff       (20)    11448 2023-06-11 17:09:42.000000 SATOSA-8.4.0/src/satosa/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2674 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/context.py
+-rw-r--r--   0 ivan       (501) staff       (20)      138 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/cookies.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1283 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/exception.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.952380 SATOSA-8.4.0/src/satosa/frontends/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/frontends/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3091 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/frontends/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)    22308 2022-11-15 11:31:39.000000 SATOSA-8.4.0/src/satosa/frontends/openid_connect.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1961 2022-11-29 13:48:33.000000 SATOSA-8.4.0/src/satosa/frontends/ping.py
+-rw-r--r--   0 ivan       (501) staff       (20)    48292 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/frontends/saml2.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4478 2022-04-18 11:24:27.000000 SATOSA-8.4.0/src/satosa/internal.py
+-rw-r--r--   0 ivan       (501) staff       (20)      756 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/logging_util.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.953170 SATOSA-8.4.0/src/satosa/metadata_creation/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/metadata_creation/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8551 2023-06-11 15:38:28.000000 SATOSA-8.4.0/src/satosa/metadata_creation/description.py
+-rw-r--r--   0 ivan       (501) staff       (20)     7255 2023-06-11 15:36:59.000000 SATOSA-8.4.0/src/satosa/metadata_creation/saml_metadata.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.956924 SATOSA-8.4.0/src/satosa/micro_services/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6542 2021-08-08 14:35:57.000000 SATOSA-8.4.0/src/satosa/micro_services/account_linking.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3811 2022-11-16 15:32:44.000000 SATOSA-8.4.0/src/satosa/micro_services/attribute_authorization.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4915 2022-11-15 11:31:39.000000 SATOSA-8.4.0/src/satosa/micro_services/attribute_generation.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4296 2023-06-07 16:46:41.000000 SATOSA-8.4.0/src/satosa/micro_services/attribute_modifications.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1091 2021-06-29 12:33:38.000000 SATOSA-8.4.0/src/satosa/micro_services/attribute_policy.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2312 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/micro_services/attribute_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1720 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)     9180 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/micro_services/consent.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4352 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/micro_services/custom_logging.py
+-rw-r--r--   0 ivan       (501) staff       (20)     5720 2022-11-29 13:44:11.000000 SATOSA-8.4.0/src/satosa/micro_services/custom_routing.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2245 2022-04-18 11:24:27.000000 SATOSA-8.4.0/src/satosa/micro_services/disco.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3497 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/hasher.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1773 2022-04-18 11:24:27.000000 SATOSA-8.4.0/src/satosa/micro_services/idp_hinting.py
+-rw-r--r--   0 ivan       (501) staff       (20)    24072 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/ldap_attribute_store.py
+-rw-r--r--   0 ivan       (501) staff       (20)    13447 2023-06-08 16:39:00.000000 SATOSA-8.4.0/src/satosa/micro_services/primary_identifier.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.958494 SATOSA-8.4.0/src/satosa/micro_services/processors/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)      133 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/base_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)      654 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/gender_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1103 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/hash_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1891 2021-10-24 15:05:53.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/regex_sub_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1695 2021-06-29 12:33:38.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/scope_extractor_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)      678 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/scope_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)      686 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/micro_services/processors/scope_remover_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10452 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/plugin_loader.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6486 2023-06-11 15:37:36.000000 SATOSA-8.4.0/src/satosa/proxy_server.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3148 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/response.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6934 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/routing.py
+-rw-r--r--   0 ivan       (501) staff       (20)      489 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/saml_util.py
+-rw-r--r--   0 ivan       (501) staff       (20)     5033 2023-06-11 17:07:21.000000 SATOSA-8.4.0/src/satosa/satosa_config.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-11 17:23:42.958736 SATOSA-8.4.0/src/satosa/scripts/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/scripts/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3999 2023-06-11 15:36:59.000000 SATOSA-8.4.0/src/satosa/scripts/satosa_saml_metadata.py
+-rw-r--r--   0 ivan       (501) staff       (20)     8637 2023-06-11 17:09:27.000000 SATOSA-8.4.0/src/satosa/state.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2538 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/util.py
+-rw-r--r--   0 ivan       (501) staff       (20)      310 2023-06-11 10:18:06.000000 SATOSA-8.4.0/src/satosa/version.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1062 2021-05-24 16:59:06.000000 SATOSA-8.4.0/src/satosa/wsgi.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1547 2022-11-15 12:05:51.000000 SATOSA-8.4.0/src/satosa/yaml.py
```

### Comparing `SATOSA-8.3.0/LICENSE` & `SATOSA-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/NOTICE` & `SATOSA-8.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/PKG-INFO` & `SATOSA-8.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: SATOSA
-Version: 8.3.0
+Version: 8.4.0
 Summary: Protocol proxy (SAML/OIDC).
 Home-page: https://github.com/SUNET/SATOSA
 Author: DIRG
 Author-email: satosa-dev@lists.sunet.se
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ldap
 Provides-Extra: pyop_mongo
 Provides-Extra: pyop_redis
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `SATOSA-8.3.0/README.md` & `SATOSA-8.4.0/README.md`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/setup.py` & `SATOSA-8.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 setup.py
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='SATOSA',
-    version='8.3.0',
+    version='8.4.0',
     description='Protocol proxy (SAML/OIDC).',
     author='DIRG',
     author_email='satosa-dev@lists.sunet.se',
     license='Apache 2.0',
     url='https://github.com/SUNET/SATOSA',
     packages=find_packages('src/'),
     package_dir={'': 'src'},
@@ -21,24 +21,28 @@
         "requests",
         "PyYAML",
         "gunicorn",
         "Werkzeug",
         "click",
         "chevron",
         "cookies-samesite-compat",
+        "importlib-metadata >= 1.7.0; python_version <= '3.8'",
     ],
     extras_require={
         "ldap": ["ldap3"],
         "pyop_mongo": ["pyop[mongo]"],
         "pyop_redis": ["pyop[redis]"],
     },
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         "console_scripts": ["satosa-saml-metadata=satosa.scripts.satosa_saml_metadata:construct_saml_metadata"]
     }
 )
```

### Comparing `SATOSA-8.3.0/src/SATOSA.egg-info/PKG-INFO` & `SATOSA-8.4.0/src/SATOSA.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: SATOSA
-Version: 8.3.0
+Version: 8.4.0
 Summary: Protocol proxy (SAML/OIDC).
 Home-page: https://github.com/SUNET/SATOSA
 Author: DIRG
 Author-email: satosa-dev@lists.sunet.se
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ldap
 Provides-Extra: pyop_mongo
 Provides-Extra: pyop_redis
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `SATOSA-8.3.0/src/SATOSA.egg-info/SOURCES.txt` & `SATOSA-8.4.0/src/SATOSA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/attribute_mapping.py` & `SATOSA-8.4.0/src/satosa/attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/apple.py` & `SATOSA-8.4.0/src/satosa/backends/apple.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/base.py` & `SATOSA-8.4.0/src/satosa/backends/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/bitbucket.py` & `SATOSA-8.4.0/src/satosa/backends/bitbucket.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/github.py` & `SATOSA-8.4.0/src/satosa/backends/github.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/linkedin.py` & `SATOSA-8.4.0/src/satosa/backends/linkedin.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/oauth.py` & `SATOSA-8.4.0/src/satosa/backends/oauth.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,12 +315,20 @@
             ui_description = UIInfoDesc()
             for desc in ui_info.get("description", []):
                 ui_description.add_description(desc[0], desc[1])
             for name in ui_info.get("display_name", []):
                 ui_description.add_display_name(name[0], name[1])
             for logo in ui_info.get("logo", []):
                 ui_description.add_logo(logo["image"], logo["width"], logo["height"], logo["lang"])
+            for keywords in ui_info.get("keywords", []):
+                ui_description.add_keywords(keywords.get("text", []), keywords.get("lang"))
+            for information_url in ui_info.get("information_url", []):
+                ui_description.add_information_url(information_url.get("text"), information_url.get("lang"))
+            for privacy_statement_url in ui_info.get("privacy_statement_url", []):
+                ui_description.add_information_url(
+                    privacy_statement_url.get("text"), privacy_statement_url.get("lang")
+                )
 
             description.ui_info = ui_description
 
     metadata_description.append(description)
     return metadata_description
```

### Comparing `SATOSA-8.3.0/src/satosa/backends/openid_connect.py` & `SATOSA-8.4.0/src/satosa/backends/openid_connect.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/orcid.py` & `SATOSA-8.4.0/src/satosa/backends/orcid.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/reflector.py` & `SATOSA-8.4.0/src/satosa/backends/reflector.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/backends/saml2.py` & `SATOSA-8.4.0/src/satosa/backends/saml2.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,14 +619,22 @@
                 ui_info_desc = UIInfoDesc()
                 for desc in ui_info.get("description", []):
                     ui_info_desc.add_description(desc["text"], desc["lang"])
                 for name in ui_info.get("display_name", []):
                     ui_info_desc.add_display_name(name["text"], name["lang"])
                 for logo in ui_info.get("logo", []):
                     ui_info_desc.add_logo(logo["text"], logo["width"], logo["height"], logo.get("lang"))
+                for keywords in ui_info.get("keywords", []):
+                    ui_info_desc.add_keywords(keywords.get("text", []), keywords.get("lang"))
+                for information_url in ui_info.get("information_url", []):
+                    ui_info_desc.add_information_url(information_url.get("text"), information_url.get("lang"))
+                for privacy_statement_url in ui_info.get("privacy_statement_url", []):
+                    ui_info_desc.add_privacy_statement_url(
+                        privacy_statement_url.get("text"), privacy_statement_url.get("lang")
+                    )
                 description.ui_info = ui_info_desc
 
             entity_descriptions.append(description)
         return entity_descriptions
 
 
 class SAMLEIDASBackend(SAMLBackend, SAMLEIDASBaseModule):
```

### Comparing `SATOSA-8.3.0/src/satosa/base.py` & `SATOSA-8.4.0/src/satosa/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -200,31 +200,46 @@
                 self.config["COOKIE_STATE_NAME"],
                 self.config["STATE_ENCRYPTION_KEY"],
             )
         except SATOSAStateError:
             state = State()
         finally:
             context.state = state
-            msg = "Loaded state {state} from cookie {cookie}".format(state=state, cookie=context.cookie)
+            msg = f"Loaded state {state} from cookie {context.cookie}"
             logline = lu.LOG_FMT.format(id=lu.get_session_id(context.state), message=msg)
             logger.debug(logline)
 
     def _save_state(self, resp, context):
         """
         Saves a state from context to cookie
 
         :type resp: satosa.response.Response
         :type context: satosa.context.Context
 
         :param resp: The response
         :param context: Session context
         """
 
-        cookie = state_to_cookie(context.state, self.config["COOKIE_STATE_NAME"], "/",
-                                 self.config["STATE_ENCRYPTION_KEY"])
+        cookie_name = self.config["COOKIE_STATE_NAME"]
+        cookie = state_to_cookie(
+            context.state,
+            name=cookie_name,
+            path="/",
+            encryption_key=self.config["STATE_ENCRYPTION_KEY"],
+            secure=self.config.get("COOKIE_SECURE"),
+            httponly=self.config.get("COOKIE_HTTPONLY"),
+            samesite=self.config.get("COOKIE_SAMESITE"),
+            max_age=self.config.get("COOKIE_MAX_AGE"),
+        )
+        resp.headers = [
+            (name, value)
+            for (name, value) in resp.headers
+            if name != "Set-Cookie"
+            or not value.startswith(f"{cookie_name}=")
+        ]
         resp.headers.append(tuple(cookie.output().split(": ", 1)))
 
     def run(self, context):
         """
         Runs the satosa proxy with the given context.
 
         :type context: satosa.context.Context
```

### Comparing `SATOSA-8.3.0/src/satosa/context.py` & `SATOSA-8.4.0/src/satosa/context.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/exception.py` & `SATOSA-8.4.0/src/satosa/exception.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/frontends/base.py` & `SATOSA-8.4.0/src/satosa/frontends/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/frontends/openid_connect.py` & `SATOSA-8.4.0/src/satosa/frontends/openid_connect.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/frontends/ping.py` & `SATOSA-8.4.0/src/satosa/frontends/ping.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/frontends/saml2.py` & `SATOSA-8.4.0/src/satosa/frontends/saml2.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/internal.py` & `SATOSA-8.4.0/src/satosa/internal.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/logging_util.py` & `SATOSA-8.4.0/src/satosa/logging_util.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/metadata_creation/description.py` & `SATOSA-8.4.0/src/satosa/metadata_creation/description.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     Description class for UI info
     """
 
     def __init__(self):
         self._description = []
         self._display_name = []
         self._logos = []
+        self._keywords = []
+        self._information_url = []
+        self._privacy_statement_url = []
 
     def add_description(self, text, lang):
         """
         Binds a description to the given language
 
         :type text: str
         :type lang: str
@@ -92,28 +95,80 @@
         """
 
         logo_entry = {"text": text, "width": width, "height": height}
         if lang:
             logo_entry["lang"] = lang
         self._logos.append(logo_entry)
 
+    def add_keywords(self, text, lang):
+        """
+        Binds keywords to the given language
+        :type text: List
+        :type lang: str
+
+        :param text: List of keywords
+        :param lang: language
+        """
+
+        if text:
+            self._keywords.append(
+                {
+                    "text": [_keyword.replace(" ", "+") for _keyword in text],
+                    "lang": lang if lang else "en",
+                }
+            )
+
+    def add_information_url(self, text, lang):
+        """
+        Binds information_url to the given language
+        :type text: str
+        :type lang: str
+
+        :param text: Information URL
+        :param lang: language
+        """
+
+        if text:
+            self._information_url.append({"text": text, "lang": lang if lang else "en"})
+
+    def add_privacy_statement_url(self, text, lang):
+        """
+        Binds privacy_statement_url to the given language
+        :type text: str
+        :type lang: str
+
+        :param text: Privacy statement URL
+        :param lang: language
+        """
+
+        if text:
+            self._privacy_statement_url.append(
+                {"text": text, "lang": lang if lang else "en"}
+            )
+
     def to_dict(self):
         """
         Returns a dictionary representation of the UIInfoDesc object.
         The format is the same as a pysaml2 configuration for ui info.
         :rtype: dict[str, str]
         :return: A dictionary representation
         """
         ui_info = {}
         if self._description:
             ui_info["description"] = self._description
         if self._display_name:
             ui_info["display_name"] = self._display_name
         if self._logos:
             ui_info["logo"] = self._logos
+        if self._keywords:
+            ui_info["keywords"] = self._keywords
+        if self._information_url:
+            ui_info["information_url"] = self._information_url
+        if self._privacy_statement_url:
+            ui_info["privacy_statement_url"] = self._privacy_statement_url
         return {"service": {"idp": {"ui_info": ui_info}}} if ui_info else {}
 
 
 class OrganizationDesc(object):
     """
     Description class for an organization
     """
@@ -223,13 +278,13 @@
         :return: A dictionary representation
         """
         description = {}
         description["entityid"] = self.entity_id
         if self._organization:
             description.update(self._organization.to_dict())
         if self._contact_person:
-            description['contact_person'] = []
+            description["contact_person"] = []
             for person in self._contact_person:
-                description['contact_person'].append(person.to_dict())
+                description["contact_person"].append(person.to_dict())
         if self._ui_info:
             description.update(self._ui_info.to_dict())
         return description
```

### Comparing `SATOSA-8.3.0/src/satosa/metadata_creation/saml_metadata.py` & `SATOSA-8.4.0/src/satosa/metadata_creation/saml_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 from ..frontends.saml2 import SAMLVirtualCoFrontend
 from ..plugin_loader import load_frontends, load_backends
 
 logger = logging.getLogger(__name__)
 
 
 def _create_entity_descriptor(entity_config):
-    cnf = Config().load(copy.deepcopy(entity_config))
+    cnf = entity_config if isinstance(entity_config,  Config) else Config().load(copy.deepcopy(entity_config))
     return entity_descriptor(cnf)
 
 
 def _create_backend_metadata(backend_modules):
     backend_metadata = {}
 
     for plugin_module in backend_modules:
         if isinstance(plugin_module, SAMLBackend):
             logline = "Generating SAML backend '{}' metadata".format(plugin_module.name)
             logger.info(logline)
-            backend_metadata[plugin_module.name] = [_create_entity_descriptor(plugin_module.config["sp_config"])]
+            backend_metadata[plugin_module.name] = [_create_entity_descriptor(plugin_module.sp.config)]
 
     return backend_metadata
 
 
 def _create_mirrored_entity_config(frontend_instance, target_metadata_info, backend_name):
     def _merge_dicts(a, b):
         for key, value in b.items():
@@ -150,7 +150,22 @@
 
     entity_desc, xmldoc = sign_entity_descriptor(entity_descriptor, None, security_context)
 
     if not valid_instance(entity_desc):
         raise ValueError("Could not construct valid EntityDescriptor tag")
 
     return xmldoc
+
+
+def create_entity_descriptor_metadata(entity_descriptor, valid_for=None):
+    """
+    :param entity_descriptor: the entity descriptor to create metadata for
+    :param valid_for: number of hours the metadata should be valid
+    :return: the EntityDescriptor metadata
+
+    :type entity_descriptor: saml2.md.EntityDescriptor]
+    :type valid_for: Optional[int]
+    """
+    if valid_for:
+        entity_descriptor.valid_until = in_a_while(hours=valid_for)
+
+    return str(entity_descriptor)
```

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/account_linking.py` & `SATOSA-8.4.0/src/satosa/micro_services/account_linking.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/attribute_authorization.py` & `SATOSA-8.4.0/src/satosa/micro_services/attribute_authorization.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/attribute_generation.py` & `SATOSA-8.4.0/src/satosa/micro_services/attribute_generation.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/attribute_modifications.py` & `SATOSA-8.4.0/src/satosa/micro_services/attribute_modifications.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/attribute_policy.py` & `SATOSA-8.4.0/src/satosa/micro_services/attribute_policy.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/attribute_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/attribute_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/base.py` & `SATOSA-8.4.0/src/satosa/micro_services/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/consent.py` & `SATOSA-8.4.0/src/satosa/micro_services/consent.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/custom_logging.py` & `SATOSA-8.4.0/src/satosa/micro_services/custom_logging.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/custom_routing.py` & `SATOSA-8.4.0/src/satosa/micro_services/custom_routing.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/disco.py` & `SATOSA-8.4.0/src/satosa/micro_services/disco.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/hasher.py` & `SATOSA-8.4.0/src/satosa/micro_services/hasher.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/idp_hinting.py` & `SATOSA-8.4.0/src/satosa/micro_services/idp_hinting.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/ldap_attribute_store.py` & `SATOSA-8.4.0/src/satosa/micro_services/ldap_attribute_store.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/primary_identifier.py` & `SATOSA-8.4.0/src/satosa/micro_services/primary_identifier.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/processors/gender_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/processors/gender_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/processors/hash_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/processors/hash_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/processors/regex_sub_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/processors/regex_sub_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/processors/scope_extractor_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/processors/scope_extractor_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/processors/scope_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/processors/scope_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/micro_services/processors/scope_remover_processor.py` & `SATOSA-8.4.0/src/satosa/micro_services/processors/scope_remover_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/plugin_loader.py` & `SATOSA-8.4.0/src/satosa/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/proxy_server.py` & `SATOSA-8.4.0/src/satosa/proxy_server.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/response.py` & `SATOSA-8.4.0/src/satosa/response.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/routing.py` & `SATOSA-8.4.0/src/satosa/routing.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/satosa_config.py` & `SATOSA-8.4.0/src/satosa/satosa_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         for parser in parsers:
             self._config = parser(config)
             if self._config is not None:
                 break
 
         # Load sensitive config from environment variables
         for key in SATOSAConfig.sensitive_dict_keys:
-            val = os.environ.get("SATOSA_{key}".format(key=key))
+            val = os.environ.get(f"SATOSA_{key}")
             if val:
                 self._config[key] = val
 
         self._verify_dict(self._config)
 
         # Read plugin configs from dict or file path
         for key in ["BACKEND_MODULES", "FRONTEND_MODULES", "MICRO_SERVICES"]:
@@ -52,15 +52,15 @@
             for config in self._config.get(key, []):
                 for parser in parsers:
                     plugin_config = parser(config)
                     if plugin_config:
                         plugin_configs.append(plugin_config)
                         break
                 else:
-                    raise SATOSAConfigurationError('Failed to load plugin config \'{}\''.format(config))
+                    raise SATOSAConfigurationError(f"Failed to load plugin config '{config}'")
             self._config[key] = plugin_configs
 
         for parser in parsers:
             _internal_attributes = parser(self._config["INTERNAL_ATTRIBUTES"])
             if _internal_attributes is not None:
                 self._config["INTERNAL_ATTRIBUTES"] = _internal_attributes
                 break
@@ -82,16 +82,16 @@
             raise SATOSAConfigurationError("Missing configuration or unknown format")
 
         for key in SATOSAConfig.mandatory_dict_keys:
             if key not in conf:
                 raise SATOSAConfigurationError("Missing key '%s' in config" % key)
 
         for key in SATOSAConfig.sensitive_dict_keys:
-            if key not in conf and "SATOSA_{key}".format(key=key) not in os.environ:
-                raise SATOSAConfigurationError("Missing key '%s' from config and ENVIRONMENT" % key)
+            if key not in conf and f"SATOSA_{key}" not in os.environ:
+                raise SATOSAConfigurationError(f"Missing key '{key}' from config and ENVIRONMENT")
 
     def __getitem__(self, item):
         """
         Returns data bound to the key 'item'.
 
         :type item: str
         :rtype object
```

### Comparing `SATOSA-8.3.0/src/satosa/scripts/satosa_saml_metadata.py` & `SATOSA-8.4.0/src/satosa/scripts/satosa_saml_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,96 @@
 import os
 
 import click
 from saml2.config import Config
 from saml2.sigver import security_context
 
 from ..metadata_creation.saml_metadata import create_entity_descriptors
+from ..metadata_creation.saml_metadata import create_entity_descriptor_metadata
 from ..metadata_creation.saml_metadata import create_signed_entity_descriptor
 from ..satosa_config import SATOSAConfig
 
 
 def _get_security_context(key, cert):
     conf = Config()
     conf.key_file = key
     conf.cert_file = cert
     return security_context(conf)
 
 
-def _create_split_entity_descriptors(entities, secc, valid):
+def _create_split_entity_descriptors(entities, secc, valid, sign=True):
     output = []
     for module_name, eds in entities.items():
         for i, ed in enumerate(eds):
-            output.append((create_signed_entity_descriptor(ed, secc, valid), "{}_{}.xml".format(module_name, i)))
+            ed_str = (
+                create_signed_entity_descriptor(ed, secc, valid)
+                if sign
+                else create_entity_descriptor_metadata(ed, valid)
+            )
+            output.append((ed_str, "{}_{}.xml".format(module_name, i)))
 
     return output
 
 
-def _create_merged_entities_descriptors(entities, secc, valid, name):
+def _create_merged_entities_descriptors(entities, secc, valid, name, sign=True):
     output = []
     frontend_entity_descriptors = [e for sublist in entities.values() for e in sublist]
     for frontend in frontend_entity_descriptors:
-        output.append((create_signed_entity_descriptor(frontend, secc, valid), name))
+        ed_str = (
+            create_signed_entity_descriptor(frontend, secc, valid)
+            if sign
+            else create_entity_descriptor_metadata(frontend, valid)
+        )
+        output.append((ed_str, name))
 
     return output
 
 
 def create_and_write_saml_metadata(proxy_conf, key, cert, dir, valid, split_frontend_metadata=False,
-                                   split_backend_metadata=False):
+                                   split_backend_metadata=False, sign=True):
     """
     Generates SAML metadata for the given PROXY_CONF, signed with the given KEY and associated CERT.
     """
     satosa_config = SATOSAConfig(proxy_conf)
-    secc = _get_security_context(key, cert)
+
+    if sign and (not key or not cert):
+        raise ValueError("Key and cert are required when signing")
+    secc = _get_security_context(key, cert) if sign else None
+
     frontend_entities, backend_entities = create_entity_descriptors(satosa_config)
 
     output = []
     if frontend_entities:
         if split_frontend_metadata:
-            output.extend(_create_split_entity_descriptors(frontend_entities, secc, valid))
+            output.extend(_create_split_entity_descriptors(frontend_entities, secc, valid, sign))
         else:
-            output.extend(_create_merged_entities_descriptors(frontend_entities, secc, valid, "frontend.xml"))
+            output.extend(_create_merged_entities_descriptors(frontend_entities, secc, valid, "frontend.xml", sign))
     if backend_entities:
         if split_backend_metadata:
-            output.extend(_create_split_entity_descriptors(backend_entities, secc, valid))
+            output.extend(_create_split_entity_descriptors(backend_entities, secc, valid, sign))
         else:
-            output.extend(_create_merged_entities_descriptors(backend_entities, secc, valid, "backend.xml"))
+            output.extend(_create_merged_entities_descriptors(backend_entities, secc, valid, "backend.xml", sign))
 
     for metadata, filename in output:
         path = os.path.join(dir, filename)
         print("Writing metadata to '{}'".format(path))
         with open(path, "w") as f:
             f.write(metadata)
 
 
 @click.command()
 @click.argument("proxy_conf")
-@click.argument("key")
-@click.argument("cert")
+@click.argument("key", required=False)
+@click.argument("cert", required=False)
 @click.option("--dir",
               type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True, readable=False,
                               resolve_path=False),
               default=".", help="Where the output files should be written.")
 @click.option("--valid", type=click.INT, default=None, help="Number of hours the metadata should be valid.")
 @click.option("--split-frontend", is_flag=True, type=click.BOOL, default=False,
               help="Create one entity descriptor per file for the frontend metadata")
 @click.option("--split-backend", is_flag=True, type=click.BOOL, default=False,
               help="Create one entity descriptor per file for the backend metadata")
-def construct_saml_metadata(proxy_conf, key, cert, dir, valid, split_frontend, split_backend):
-    create_and_write_saml_metadata(proxy_conf, key, cert, dir, valid, split_frontend, split_backend)
+@click.option("--sign/--no-sign", is_flag=True, type=click.BOOL, default=True,
+              help="Sign the generated metadata")
+def construct_saml_metadata(proxy_conf, key, cert, dir, valid, split_frontend, split_backend, sign):
+    create_and_write_saml_metadata(proxy_conf, key, cert, dir, valid, split_frontend, split_backend, sign)
```

### Comparing `SATOSA-8.3.0/src/satosa/state.py` & `SATOSA-8.4.0/src/satosa/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,50 +21,168 @@
 
 
 logger = logging.getLogger(__name__)
 
 _SESSION_ID_KEY = "SESSION_ID"
 
 
-def state_to_cookie(state, name, path, encryption_key):
+class State(UserDict):
+    """
+    This class holds a state attribute object. A state object must be able to be converted to
+    a json string, otherwise will an exception be raised.
     """
-    Saves a state to a cookie
 
-    :type state: satosa.state.State
-    :type name: str
-    :type path: str
-    :type encryption_key: str
-    :rtype: satosa.cookies.SimpleCookie
+    def __init__(self, urlstate_data=None, encryption_key=None):
+        """
+        If urlstate is empty a new empty state instance will be returned.
 
-    :param state: The state to save
-    :param name: Name identifier of the cookie
-    :param path: Endpoint path the cookie will be associated to
-    :param encryption_key: Key to encrypt the state information
-    :return: A cookie
-    """
+        If urlstate is not empty the constructor will rebuild the state attribute objects
+        from the urlstate string.
+        :type urlstate_data: str
+        :type encryption_key: str
+        :rtype: State
+
+        :param encryption_key: The key to be used for encryption.
+        :param urlstate_data: A string created by the method urlstate in this class.
+        :return: An instance of this class.
+        """
+        self.delete = False
+
+        urlstate_data = {} if urlstate_data is None else urlstate_data
+        if urlstate_data and not encryption_key:
+            raise ValueError("If an 'urlstate_data' is supplied 'encrypt_key' must be specified.")
 
-    cookie_data = "" if state.delete else state.urlstate(encryption_key)
+        if urlstate_data:
+            try:
+                urlstate_data_bytes = urlstate_data.encode("utf-8")
+                urlstate_data_b64decoded = base64.urlsafe_b64decode(urlstate_data_bytes)
+                lzma = LZMADecompressor()
+                urlstate_data_decompressed = lzma.decompress(urlstate_data_b64decoded)
+                urlstate_data_decrypted = _AESCipher(encryption_key).decrypt(
+                    urlstate_data_decompressed
+                )
+                lzma = LZMADecompressor()
+                urlstate_data_decrypted_decompressed = lzma.decompress(urlstate_data_decrypted)
+                urlstate_data_obj = json.loads(urlstate_data_decrypted_decompressed)
+            except Exception as e:
+                error_context = {
+                    "message": "Failed to load state data. Reinitializing empty state.",
+                    "reason": str(e),
+                    "urlstate_data": urlstate_data,
+                }
+                logger.warning(error_context)
+                urlstate_data = {}
+            else:
+                urlstate_data = urlstate_data_obj
+
+        session_id = (
+            urlstate_data[_SESSION_ID_KEY]
+            if urlstate_data and _SESSION_ID_KEY in urlstate_data
+            else uuid4().urn
+        )
+        urlstate_data[_SESSION_ID_KEY] = session_id
+
+        super().__init__(urlstate_data)
+
+    @property
+    def session_id(self):
+        return self.data.get(_SESSION_ID_KEY)
+
+    def urlstate(self, encryption_key):
+        """
+        Will return a url safe representation of the state.
+
+        :type encryption_key: Key used for encryption.
+        :rtype: str
+
+        :return: Url representation av of the state.
+        """
+        lzma = LZMACompressor()
+        urlstate_data = json.dumps(self.data)
+        urlstate_data = lzma.compress(urlstate_data.encode("UTF-8"))
+        urlstate_data += lzma.flush()
+        urlstate_data = _AESCipher(encryption_key).encrypt(urlstate_data)
+        lzma = LZMACompressor()
+        urlstate_data = lzma.compress(urlstate_data)
+        urlstate_data += lzma.flush()
+        urlstate_data = base64.urlsafe_b64encode(urlstate_data)
+        return urlstate_data.decode("utf-8")
+
+    def copy(self):
+        """
+        Returns a deepcopy of the state
+
+        :rtype: satosa.state.State
+
+        :return: A copy of the state
+        """
+        state_copy = State()
+        state_copy.data = copy.deepcopy(self.data)
+        return state_copy
+
+    @property
+    def state_dict(self):
+        """
+        :rtype: dict[str, any]
+        :return: A copy of the state as dictionary.
+        """
+        return copy.deepcopy(self.data)
+
+
+def state_to_cookie(
+    state: State,
+    *,
+    name: str,
+    path: str,
+    encryption_key: str,
+    secure: bool = None,
+    httponly: bool = None,
+    samesite: str = None,
+    max_age: str = None,
+) -> SimpleCookie:
+    """
+    Saves a state to a cookie
 
+    :param state: the data to save
+    :param name: identifier of the cookie
+    :param path: path the cookie will be associated to
+    :param encryption_key: the key to use to encrypt the state information
+    :param secure: whether to include the cookie only when the request is transmitted
+                   over a secure channel
+    :param httponly: whether the cookie should only be accessed only by the server
+    :param samesite: whether the cookie should only be sent with requests
+                     initiated from the same registrable domain
+    :param max_age: indicates the maximum lifetime of the cookie,
+                    represented as the number of seconds until the cookie expires
+    :return: A cookie object
+    """
     cookie = SimpleCookie()
-    cookie[name] = cookie_data
-    cookie[name]["samesite"] = "None"
-    cookie[name]["secure"] = True
+    cookie[name] = "" if state.delete else state.urlstate(encryption_key)
     cookie[name]["path"] = path
-    cookie[name]["max-age"] = 0 if state.delete else ""
+    cookie[name]["secure"] = secure if secure is not None else True
+    cookie[name]["httponly"] = httponly if httponly is not None else ""
+    cookie[name]["samesite"] = samesite if samesite is not None else "None"
+    cookie[name]["max-age"] = (
+        0
+        if state.delete
+        else max_age
+        if max_age is not None
+        else ""
+    )
 
     msg = "Saved state in cookie {name} with properties {props}".format(
         name=name, props=list(cookie[name].items())
     )
     logline = lu.LOG_FMT.format(id=lu.get_session_id(state), message=msg)
     logger.debug(logline)
 
     return cookie
 
 
-def cookie_to_state(cookie_str, name, encryption_key):
+def cookie_to_state(cookie_str: str, name: str, encryption_key: str) -> State:
     """
     Loads a state from a cookie
 
     :type cookie_str: str
     :type name: str
     :type encryption_key: str
     :rtype: satosa.state.State
@@ -74,16 +192,15 @@
     :param encryption_key: Key to encrypt the state information
     :return: A state
     """
     try:
         cookie = SimpleCookie(cookie_str)
         state = State(cookie[name].value, encryption_key)
     except KeyError as e:
-        msg_tmpl = 'No cookie named {name} in {data}'
-        msg = msg_tmpl.format(name=name, data=cookie_str)
+        msg = f'No cookie named {name} in {cookie_str}'
         raise SATOSAStateError(msg) from e
     except ValueError as e:
         msg_tmpl = 'Failed to process {name} from {data}'
         msg = msg_tmpl.format(name=name, data=cookie_str)
         raise SATOSAStateError(msg) from e
     else:
         return state
@@ -152,110 +269,7 @@
         """
         Removes the padding performed by the method _pad.
 
         :type b: bytes
         :rtype: bytes
         """
         return b[:-ord(b[len(b) - 1:])]
-
-
-class State(UserDict):
-    """
-    This class holds a state attribute object. A state object must be able to be converted to
-    a json string, otherwise will an exception be raised.
-    """
-
-    def __init__(self, urlstate_data=None, encryption_key=None):
-        """
-        If urlstate is empty a new empty state instance will be returned.
-
-        If urlstate is not empty the constructor will rebuild the state attribute objects
-        from the urlstate string.
-        :type urlstate_data: str
-        :type encryption_key: str
-        :rtype: State
-
-        :param encryption_key: The key to be used for encryption.
-        :param urlstate_data: A string created by the method urlstate in this class.
-        :return: An instance of this class.
-        """
-        self.delete = False
-
-        urlstate_data = {} if urlstate_data is None else urlstate_data
-        if urlstate_data and not encryption_key:
-            raise ValueError("If an 'urlstate_data' is supplied 'encrypt_key' must be specified.")
-
-        if urlstate_data:
-            try:
-                urlstate_data_bytes = urlstate_data.encode("utf-8")
-                urlstate_data_b64decoded = base64.urlsafe_b64decode(urlstate_data_bytes)
-                lzma = LZMADecompressor()
-                urlstate_data_decompressed = lzma.decompress(urlstate_data_b64decoded)
-                urlstate_data_decrypted = _AESCipher(encryption_key).decrypt(
-                    urlstate_data_decompressed
-                )
-                lzma = LZMADecompressor()
-                urlstate_data_decrypted_decompressed = lzma.decompress(urlstate_data_decrypted)
-                urlstate_data_obj = json.loads(urlstate_data_decrypted_decompressed)
-            except Exception as e:
-                error_context = {
-                    "message": "Failed to load state data. Reinitializing empty state.",
-                    "reason": str(e),
-                    "urlstate_data": urlstate_data,
-                }
-                logger.warning(error_context)
-                urlstate_data = {}
-            else:
-                urlstate_data = urlstate_data_obj
-
-        session_id = (
-            urlstate_data[_SESSION_ID_KEY]
-            if urlstate_data and _SESSION_ID_KEY in urlstate_data
-            else uuid4().urn
-        )
-        urlstate_data[_SESSION_ID_KEY] = session_id
-
-        super().__init__(urlstate_data)
-
-    @property
-    def session_id(self):
-        return self.data.get(_SESSION_ID_KEY)
-
-    def urlstate(self, encryption_key):
-        """
-        Will return a url safe representation of the state.
-
-        :type encryption_key: Key used for encryption.
-        :rtype: str
-
-        :return: Url representation av of the state.
-        """
-        lzma = LZMACompressor()
-        urlstate_data = json.dumps(self.data)
-        urlstate_data = lzma.compress(urlstate_data.encode("UTF-8"))
-        urlstate_data += lzma.flush()
-        urlstate_data = _AESCipher(encryption_key).encrypt(urlstate_data)
-        lzma = LZMACompressor()
-        urlstate_data = lzma.compress(urlstate_data)
-        urlstate_data += lzma.flush()
-        urlstate_data = base64.urlsafe_b64encode(urlstate_data)
-        return urlstate_data.decode("utf-8")
-
-    def copy(self):
-        """
-        Returns a deepcopy of the state
-
-        :rtype: satosa.state.State
-
-        :return: A copy of the state
-        """
-        state_copy = State()
-        state_copy.data = copy.deepcopy(self.data)
-        return state_copy
-
-    @property
-    def state_dict(self):
-        """
-        :rtype: dict[str, any]
-        :return: A copy of the state as dictionary.
-        """
-        return copy.deepcopy(self.data)
```

### Comparing `SATOSA-8.3.0/src/satosa/util.py` & `SATOSA-8.4.0/src/satosa/util.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/wsgi.py` & `SATOSA-8.4.0/src/satosa/wsgi.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.3.0/src/satosa/yaml.py` & `SATOSA-8.4.0/src/satosa/yaml.py`

 * *Files identical despite different names*

