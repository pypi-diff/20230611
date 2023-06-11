# Comparing `tmp/cici.tools-0.1.3.tar.gz` & `tmp/cici.tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici.tools-0.1.3.tar", last modified: Wed May 17 09:08:12 2023, max compression
+gzip compressed data, was "cici.tools-0.1.4.tar", last modified: Sun Jun 11 18:08:44 2023, max compression
```

## Comparing `cici.tools-0.1.3.tar` & `cici.tools-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.450373 cici.tools-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 09:08:08.000000 cici.tools-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 09:08:12.450373 cici.tools-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-05-17 09:08:08.000000 cici.tools-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.446372 cici.tools-0.1.3/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 09:08:09.000000 cici.tools-0.1.3/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.449373 cici.tools-0.1.3/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6752 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.449373 cici.tools-0.1.3/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-05-17 09:08:08.000000 cici.tools-0.1.3/cici/schema/gitlab-ci.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 09:08:12.448372 cici.tools-0.1.3/cici.tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-17 09:08:12.000000 cici.tools-0.1.3/cici.tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-17 09:08:12.450373 cici.tools-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-17 09:08:09.000000 cici.tools-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.898304 cici.tools-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-11 18:08:42.000000 cici.tools-0.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-11 18:08:42.000000 cici.tools-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-06-11 18:08:44.898304 cici.tools-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5401 2023-06-11 18:08:42.000000 cici.tools-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.895300 cici.tools-0.1.4/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.896302 cici.tools-0.1.4/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7260 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.897303 cici.tools-0.1.4/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.897303 cici.tools-0.1.4/cici/providers/brettops/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.898304 cici.tools-0.1.4/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.896302 cici.tools-0.1.4/cici.tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-11 18:08:44.899306 cici.tools-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-06-11 18:08:42.000000 cici.tools-0.1.4/setup.py
```

### Comparing `cici.tools-0.1.3/cici/cli/bundle.py` & `cici.tools-0.1.4/cici/cli/bundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,44 +7,24 @@
 
 from jsonschema import validate
 from ruamel.yaml import YAML as _YAML
 from ruamel.yaml.scalarstring import DoubleQuotedScalarString
 from termcolor import colored
 
 from ..constants import SCHEMA_DIR
+from ..utils import merge_dict
 
 
 class YAML(_YAML):
     def dumps(self, data, **kw):
         stream = StringIO()
         _YAML.dump(self, data, stream, **kw)
         return stream.getvalue()
 
 
-def merge_dict(orig: dict, new: dict) -> dict:
-    final = {}
-
-    all_keys = sorted(list(set(orig.keys()) | set(new.keys())))
-    for key in all_keys:
-        if key in orig and key in new:
-            if isinstance(orig[key], dict):
-                if not isinstance(new[key], dict):
-                    raise NotImplementedError("Can't merge dict and non-dict keys")
-                final[key] = merge_dict(orig[key], new[key])
-            else:
-                final[key] = new[key]  # new takes precedence
-        elif key in orig:
-            final[key] = orig[key]
-        elif key in new:
-            final[key] = new[key]
-        else:
-            raise NotImplementedError("This should not possible")
-    return final
-
-
 def simplify_job(data, job):
     job = copy.deepcopy(job)
 
     if not "extends" in job:
         return job
 
     extends = job["extends"]
@@ -139,17 +119,18 @@
         handle.write("# this CI file was generated by cici; do not hand-edit\n")
         blocks = [
             yaml.dumps({key: group_data[key]}).rstrip() for key in sorted(group_data)
         ]
         handle.write("\n\n".join(blocks) + "\n")
 
 
-def bundle_command(args):
+def bundle_command(parser, args):
     config_file = args.config_path / "config.yml"
     gitlab_file = args.config_path / "gitlab" / "main.yml"
+    pipeline_file = args.config_path / "pipeline.yml"
 
     args.output_path = Path(args.output_path)
     if args.groups:
         args.groups = [group.strip() for group in args.groups.split(",")]
 
     yaml = YAML()
     if config_file.exists():
@@ -162,14 +143,20 @@
     data = yaml.load(text)
 
     schema_file = SCHEMA_DIR / "gitlab-ci.json"
 
     schema = json.load(open(schema_file))
     validate(data, schema=schema)
 
+    if pipeline_file.exists():
+        yaml.load(open(pipeline_file).read())
+        # pipeline = read_pipeline(pipeline_data)
+        # for var in pipeline.variables:
+        #     print(var)
+
     # get reserved words
     keywords = {key for key in schema["properties"].keys() if key not in ("pages",)}
 
     # get jobs
     jobs = {key: value for key, value in data.items() if key not in keywords}
 
     if not args.groups:
@@ -220,7 +207,45 @@
             )
             straight_copy(data, groups[group_name], "stages")
             straight_copy(data, groups[group_name], "workflow")
 
     for group_name, group_data in groups.items():
         validate(group_data, schema=schema)
         write_ci_file(args.output_path, group_name=group_name, group_data=group_data)
+
+
+def bundle_parser(subparsers):
+    parser = subparsers.add_parser(
+        "bundle", help="distill a CI file to a job and its dependencies"
+    )
+    parser.add_argument(
+        "config_path",
+        metavar="DIR",
+        nargs="?",
+        type=Path,
+        default=(Path.cwd() / ".cici").absolute(),
+    )
+    parser.add_argument(
+        "-a",
+        "--all",
+        dest="include_hidden_jobs",
+        action="store_true",
+        help="include hidden jobs in output",
+    )
+    parser.add_argument("-g", "--groups", help="job group patterns")
+    parser.add_argument(
+        "-o",
+        "--output",
+        metavar="DIR",
+        dest="output_path",
+        type=Path,
+        default=Path.cwd().absolute(),
+    )
+    parser.add_argument(
+        "-p",
+        "--pipeline",
+        metavar="DIR",
+        dest="pipeline_name",
+        default=str(Path.cwd().name),
+    )
+    parser.set_defaults(func=bundle_command)
+    return parser
```

### Comparing `cici.tools-0.1.3/cici/cli/update.py` & `cici.tools-0.1.4/cici/cli/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,17 +89,24 @@
 def update_includes(includes):
     if not isinstance(includes, list):
         return includes
 
     return [update_include(include) for include in includes]
 
 
-def update_command(args):
+def update_command(parser, args):
     yaml = ruamel.yaml.YAML()
     data = yaml.load(open(args.filename))
 
     if "include" in data:
         data["include"] = update_includes(data["include"])
 
     with open(args.filename, "w") as handle:
         yaml.indent(mapping=2, sequence=4, offset=2)
         yaml.dump(data, handle)
+
+
+def update_parser(subparsers):
+    parser = subparsers.add_parser("update")
+    parser.add_argument("filename", nargs="?", default=".gitlab-ci.yml")
+    parser.set_defaults(func=update_command)
+    return parser
```

### Comparing `cici.tools-0.1.3/cici/schema/LICENSE.gitlab` & `cici.tools-0.1.4/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.3/cici/schema/gitlab-ci.json` & `cici.tools-0.1.4/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.3/setup.py` & `cici.tools-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
 
@@ -26,15 +26,15 @@
             "cici = cici.__main__:main",
         ],
     },
     install_requires=install_requires,
     python_requires=">=3.6",
     keywords="ci pipeline python",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

