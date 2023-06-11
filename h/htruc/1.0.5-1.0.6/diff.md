# Comparing `tmp/htruc-1.0.5.tar.gz` & `tmp/htruc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htruc-1.0.5.tar", last modified: Wed Jun 22 07:46:19 2022, max compression
+gzip compressed data, was "htruc-1.0.6.tar", last modified: Sun Jun 11 08:08:35 2023, max compression
```

## Comparing `htruc-1.0.5.tar` & `htruc-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-06-22 07:46:19.770655 htruc-1.0.5/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2172 2022-06-22 07:46:19.770655 htruc-1.0.5/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.0.5/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-06-22 07:46:19.770655 htruc-1.0.5/htruc/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.0.5/htruc/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    10953 2022-06-22 07:43:40.000000 htruc-1.0.5/htruc/catalog.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8928 2022-06-21 08:43:02.000000 htruc-1.0.5/htruc/cli.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-06-22 07:46:19.770655 htruc-1.0.5/htruc/repos/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.0.5/htruc/repos/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.0.5/htruc/repos/_generic.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2475 2022-06-21 08:37:28.000000 htruc-1.0.5/htruc/repos/_github.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-06-22 07:46:19.770655 htruc-1.0.5/htruc/schemas/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1220 2022-06-20 10:01:21.000000 htruc-1.0.5/htruc/schemas/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1021 2022-06-20 10:01:21.000000 htruc-1.0.5/htruc/schemas/upgrade_path.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.0.5/htruc/types.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1605 2022-06-20 10:01:21.000000 htruc-1.0.5/htruc/utils.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2875 2022-06-20 10:01:21.000000 htruc-1.0.5/htruc/validator.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-06-22 07:46:19.770655 htruc-1.0.5/htruc.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2172 2022-06-22 07:46:19.000000 htruc-1.0.5/htruc.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      418 2022-06-22 07:46:19.000000 htruc-1.0.5/htruc.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2022-06-22 07:46:19.000000 htruc-1.0.5/htruc.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2022-06-22 07:46:19.000000 htruc-1.0.5/htruc.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      150 2022-06-22 07:46:19.000000 htruc-1.0.5/htruc.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2022-06-22 07:46:19.000000 htruc-1.0.5/htruc.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2022-06-22 07:46:19.770655 htruc-1.0.5/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2022-06-22 07:33:49.000000 htruc-1.0.5/setup.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2172 2023-06-11 08:08:35.135407 htruc-1.0.6/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1191 2023-06-11 08:04:36.000000 htruc-1.0.6/README.md
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    11099 2023-06-11 08:07:33.000000 htruc-1.0.6/htruc/catalog.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8928 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/cli.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc/repos/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      118 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/repos/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      492 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/repos/_generic.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2517 2023-06-11 08:07:10.000000 htruc-1.0.6/htruc/repos/_github.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc/schemas/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1220 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/schemas/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1021 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/schemas/upgrade_path.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      130 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/types.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1605 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/utils.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2875 2023-06-11 08:04:36.000000 htruc-1.0.6/htruc/validator.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:08:35.135407 htruc-1.0.6/htruc.egg-info/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2172 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      418 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        1 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       41 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/entry_points.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      150 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/requires.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        6 2023-06-11 08:08:35.000000 htruc-1.0.6/htruc.egg-info/top_level.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       38 2023-06-11 08:08:35.135407 htruc-1.0.6/setup.cfg
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3799 2023-06-11 08:08:20.000000 htruc-1.0.6/setup.py
```

### Comparing `htruc-1.0.5/PKG-INFO` & `htruc-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.5
+Version: 1.0.6
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
 Description: 
         <img src="./img/HTRUC.png" width=300 align=right>
```

### Comparing `htruc-1.0.5/README.md` & `htruc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `htruc-1.0.5/htruc/catalog.py` & `htruc-1.0.6/htruc/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,18 @@
     data = {}
     if local_directory:
         data.update(get_local_yaml(directory=local_directory, keep_valid_only=False))
         if check_link:
             for uri in data:
                 # We update the catalog if needs be by checking each repo
                 if "github.com" in uri:
-                    data[uri] = get_github_repo_yaml(address=uri, access_token=access_token)
+                    print(f"Fetching {uri} remotely to update metrics")
+                    results = get_github_repo_yaml(address=uri, access_token=access_token)
+                    if results:
+                        data[uri] = results
     if get_distant:
         if isinstance(organizations, str):
             organizations = (organizations, )
         for orga in organizations:
             data.update(
                 get_htr_united_repos(
                     access_token=access_token,
```

### Comparing `htruc-1.0.5/htruc/cli.py` & `htruc-1.0.6/htruc/cli.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.5/htruc/repos/_github.py` & `htruc-1.0.6/htruc/repos/_github.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     user, repo_name = re.findall("github.com/([^/]+)/([^/]+)", address)[0]
     if repo_name.endswith(".git"):
         repo_name = repo_name[:-4]
     g = Github(access_token)
     repo = g.get_repo(f"{user}/{repo_name}")
     try:
         text = repo.get_contents("htr-united.yml").decoded_content.decode()
+        print("--- Found htr-united.yml")
     except UnknownObjectException as e:
         return None
     try:
         return parse_yaml(text)
     except yaml.parser.ParserError:
         print(f"Parse error on {user}/{repo_name}")
         if raise_on_parse_error:
```

### Comparing `htruc-1.0.5/htruc/schemas/__init__.py` & `htruc-1.0.6/htruc/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.5/htruc/schemas/upgrade_path.py` & `htruc-1.0.6/htruc/schemas/upgrade_path.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.5/htruc/utils.py` & `htruc-1.0.6/htruc/utils.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.5/htruc/validator.py` & `htruc-1.0.6/htruc/validator.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.5/htruc.egg-info/PKG-INFO` & `htruc-1.0.6/htruc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.5
+Version: 1.0.6
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
 Description: 
         <img src="./img/HTRUC.png" width=300 align=right>
```

### Comparing `htruc-1.0.5/setup.py` & `htruc-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'htruc'
 DESCRIPTION = 'HTRUC, a toolkit for HTR-United cataloging'
 URL = 'https://github.com/htr-united/htrvc'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

