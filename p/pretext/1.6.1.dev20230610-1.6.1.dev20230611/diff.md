# Comparing `tmp/pretext-1.6.1.dev20230610.tar.gz` & `tmp/pretext-1.6.1.dev20230611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230610.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230611.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230610.tar` & `pretext-1.6.1.dev20230611.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/LICENSE
--rw-r--r--   0        0        0     9664 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/README.md
--rw-r--r--   0        0        0     1901 2023-06-10 06:18:27.949955 pretext-1.6.1.dev20230610/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/__main__.py
--rw-r--r--   0        0        0     8170 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/build.py
--rw-r--r--   0        0        0    22798 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-10 06:18:33.121951 pretext-1.6.1.dev20230610/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/core/resources.py
--rw-r--r--   0        0        0  1034862 2023-06-10 06:18:33.121951 pretext-1.6.1.dev20230610/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/generate.py
--rw-r--r--   0        0        0    24666 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/project.py
--rw-r--r--   0        0        0      516 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-10 06:18:33.189951 pretext-1.6.1.dev20230610/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-10 06:18:33.189951 pretext-1.6.1.dev20230610/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-06-10 06:18:33.165951 pretext-1.6.1.dev20230610/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-06-10 06:18:33.169951 pretext-1.6.1.dev20230610/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-06-10 06:18:33.185951 pretext-1.6.1.dev20230610/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-06-10 06:18:33.189951 pretext-1.6.1.dev20230610/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-06-10 06:18:33.185951 pretext-1.6.1.dev20230610/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-10 06:18:33.189951 pretext-1.6.1.dev20230610/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-10 06:18:33.189951 pretext-1.6.1.dev20230610/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-06-10 06:18:33.189951 pretext-1.6.1.dev20230610/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18416 2023-06-10 06:17:50.301971 pretext-1.6.1.dev20230610/pretext/utils.py
--rw-r--r--   0        0        0     1143 2023-06-10 06:18:27.949955 pretext-1.6.1.dev20230610/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230610/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-11 06:17:18.182685 pretext-1.6.1.dev20230611/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-11 06:17:18.182685 pretext-1.6.1.dev20230611/README.md
+-rw-r--r--   0        0        0     1901 2023-06-11 06:17:54.283451 pretext-1.6.1.dev20230611/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-11 06:17:18.182685 pretext-1.6.1.dev20230611/pretext/__main__.py
+-rw-r--r--   0        0        0     8170 2023-06-11 06:17:18.182685 pretext-1.6.1.dev20230611/pretext/build.py
+-rw-r--r--   0        0        0    25061 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-11 06:17:59.463553 pretext-1.6.1.dev20230611/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/core/resources.py
+-rw-r--r--   0        0        0  1034865 2023-06-11 06:17:59.459553 pretext-1.6.1.dev20230611/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/generate.py
+-rw-r--r--   0        0        0    27228 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-11 06:17:59.531554 pretext-1.6.1.dev20230611/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-11 06:17:59.531554 pretext-1.6.1.dev20230611/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-06-11 06:17:59.507554 pretext-1.6.1.dev20230611/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-06-11 06:17:59.511554 pretext-1.6.1.dev20230611/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-06-11 06:17:59.523554 pretext-1.6.1.dev20230611/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-06-11 06:17:59.531554 pretext-1.6.1.dev20230611/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-06-11 06:17:59.527554 pretext-1.6.1.dev20230611/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-11 06:17:59.531554 pretext-1.6.1.dev20230611/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-11 06:17:59.531554 pretext-1.6.1.dev20230611/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-06-11 06:17:59.527554 pretext-1.6.1.dev20230611/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18416 2023-06-11 06:17:18.186686 pretext-1.6.1.dev20230611/pretext/utils.py
+-rw-r--r--   0        0        0     1143 2023-06-11 06:17:54.287452 pretext-1.6.1.dev20230611/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230611/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230610/LICENSE` & `pretext-1.6.1.dev20230611/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/README.md` & `pretext-1.6.1.dev20230611/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 If you run `echo 'alias pr="poetry run"' >> ~/.bashrc` then restart your
 shell, this becomes less of a mouthful:
 
 ```
 pretext --version     # returns system version
 pr pretext --version  # returns version being developed
 ```
+(On Windows, in PowerShell, you get get such an alias with `Function pr {poetry run @Args}`)
 
 #### Steps on Windows
 
 In windows, you can either use the bash shell and follow the directions above,
 or try [pyenv-win](https://github.com/pyenv-win/pyenv-win#installation). In
 the latter case, make sure to follow all the installation instructions, including
 the **Finish the installation**. Then proceed to follow the directions above to
```

### Comparing `pretext-1.6.1.dev20230610/pretext/__init__.py` & `pretext-1.6.1.dev20230611/pretext/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'd54093037a21ea9071a5d89acd83aee3b2cf790a'
+CORE_COMMIT = 'c90ba4bee68ab6fd4ba41d4831f2bfea13838fb7'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230610/pretext/build.py` & `pretext-1.6.1.dev20230611/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/cli.py` & `pretext-1.6.1.dev20230611/pretext/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -323,37 +323,42 @@
     is_flag=False,
     flag_value="ALL",
     default=None,
     type=click.Choice(ASSETS, case_sensitive=False),
     help="Generates assets for target.  -g [asset] will generate the specific assets given.",
 )
 @click.option(
+    "-q",
+    "--no-generate",
+    is_flag=True,
+    default=False,
+    help="Do not generate assets for target, even if their source has changed since last build.",
+)
+@click.option(
     "-x", "--xmlid", type=click.STRING, help="xml:id of element to be generated."
 )
 @click.option(
     "-p",
     "--project-ptx-override",
     type=(str, str),
     multiple=True,
     help=xml_overlay.USAGE_DESCRIPTION.format("-p"),
 )
 def build(
     target,
     clean,
     generate,
+    no_generate,
     xmlid: t.Optional[str],
     project_ptx_override: t.Tuple[str, str],
 ):
     """
     Build [TARGET] according to settings specified by project.ptx.
 
-    If using certain elements (webwork, latex-image, etc.) then
-    using `--generate` may be necessary for a successful build. Generated
-    assets are cached so they need not be regenerated in subsequent builds unless
-    they are changed.
+    If using elements that require separate generation of assets (e.g., webwork, latex-image, etc.) then these will be generated automatically if their source has changed since the last build.  You can suppress this with the `--no-generate` flag, or force a regeneration with the `--generate` flag.
 
     Certain builds may require installations not included with the CLI, or internet
     access to external servers. Command-line paths
     to non-Python executables may be set in project.ptx. For more details,
     consult the PreTeXt Guide: https://pretextbook.org/documentation.html
     """
 
@@ -371,31 +376,68 @@
     if len(project_ptx_override) > 0:
         messages = project.apply_overlay(overlay)
         for message in messages:
             log.info("project.ptx overlay " + message)
     target = project.target(name=target_name)
     if target_name is None:
         log.info(
-            f"Since no build target was supplied, the first target of the project.ptx manifest ({target.name()}) will be built."
+            f"Since no build target was supplied, the first target of the project.ptx manifest ({target.name()}) will be built.\n"
         )
         target_name = target.name()
     if target is None:
         utils.show_target_hints(target_name, project, task="build")
         log.critical("Exiting without completing build.")
         return
+    # Automatically generate any assets that have changed.
+    if not no_generate:
+        asset_table = target.load_asset_table()
+        asset_hash_dict = target.asset_hash()
+        if asset_table == asset_hash_dict:
+            log.info(
+                "No change in assets requiring generating detected.  To force regeneration of assets, use `-g` flag.\n"
+            )
+        else:
+            for asset in set(asset[0] for asset in asset_hash_dict.keys()):
+                if asset in ["webwork"]:
+                    if (asset, "") not in asset_table or asset_hash_dict[
+                        (asset, "")
+                    ] != asset_table[(asset, "")]:
+                        project.generate(target.name(), asset_list=[asset])
+                elif (asset, "") not in asset_table or asset_hash_dict[
+                    (asset, "")
+                ] != asset_table[(asset, "")]:
+                    project.generate(target.name(), asset_list=[asset])
+                else:
+                    for id in set(
+                        key[1] for key in asset_hash_dict.keys() if key[0] == asset
+                    ):
+                        if (asset, id) not in asset_table or asset_hash_dict[
+                            (asset, id)
+                        ] != asset_table[(asset, id)]:
+                            log.info(
+                                f"\nIt appears the source has changed of an asset that needs to be generated.  Now generating asset: {asset} with xmlid: {id}."
+                            )
+                            project.generate(
+                                target.name(), asset_list=[asset], xmlid=id
+                            )
+            target.save_asset_table(target.asset_hash())
+    else:
+        log.info("Skipping asset generation as requested.")
     if generate == "ALL":
-        log.info("Generating all assets in default formats.")
+        log.info("Generating all assets in default formats as requested.")
+        log.info(
+            "Note: PreTeXt will automatically generate assets that have been changed since your last build, so this option is no longer necessary unless something isn't happening as expected."
+        )
         project.generate(target.name())
     elif generate is not None:
-        log.warning(f"Generating only {generate} assets.")
+        log.info(f"Generating {generate} assets as requested.")
+        log.info(
+            "Note: PreTeXt will automatically generate assets that have been changed since your last build, so this option is no longer necessary unless something isn't happening as expected."
+        )
         project.generate(target.name(), asset_list=[generate])
-    else:
-        log.warning("Assets like latex-images will not be regenerated for this build")
-        log.warning("(previously generated assets will be used if they exist).")
-        log.warning("To generate these assets before building, run `pretext build -g`.")
     project.build(target.name(), clean)
 
 
 # pretext generate
 @main.command(
     short_help="Generate specified assets for specified target",
     context_settings=CONTEXT_SETTINGS,
```

### Comparing `pretext-1.6.1.dev20230610/pretext/codechat.py` & `pretext-1.6.1.dev20230611/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230611/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/core/pretext.py` & `pretext-1.6.1.dev20230611/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/core/resources.py` & `pretext-1.6.1.dev20230611/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/core/resources.zip` & `pretext-1.6.1.dev20230611/pretext/core/resources.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
-Zip file size: 1034862 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 xsl/utilities/
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-10 06:18 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611192 b- defN 23-Jun-10 06:18 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-10 06:18 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-10 06:18 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-10 06:18 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-10 06:18 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-10 06:18 xsl/entities.ent
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-10 06:18 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-10 06:18 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-10 06:18 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-10 06:18 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-10 06:18 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-10 06:18 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-10 06:18 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   111931 b- defN 23-Jun-10 06:18 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-10 06:18 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-10 06:18 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-10 06:18 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-10 06:18 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-10 06:18 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-10 06:18 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-10 06:18 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-10 06:18 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-10 06:18 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-10 06:18 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-10 06:18 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-10 06:18 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx   106649 b- defN 23-Jun-10 06:18 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-10 06:18 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-10 06:18 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-10 06:18 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-10 06:18 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-10 06:18 xsl/README.md
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-10 06:18 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-10 06:18 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-10 06:18 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-10 06:18 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-10 06:18 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-10 06:18 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-10 06:18 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-10 06:18 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-10 06:18 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-10 06:18 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-10 06:18 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-10 06:18 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 xsl/support/play-button/
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-10 06:18 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-10 06:18 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-10 06:18 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-10 06:18 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-10 06:18 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-10 06:18 xsl/support/README.md
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-10 06:18 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-10 06:18 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-10 06:18 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-10 06:18 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-10 06:18 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-10 06:18 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-10 06:18 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-10 06:18 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-10 06:18 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-10 06:18 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-10 06:18 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-10 06:18 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-10 06:18 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-10 06:18 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-10 06:18 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-10 06:18 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-10 06:18 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-10 06:18 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-10 06:18 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-10 06:18 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-10 06:18 xsl/localizations/README.md
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-10 06:18 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-10 06:18 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-10 06:18 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-10 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-10 06:18 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-10 06:18 css/kindle.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-10 06:18 css/update_css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-10 06:18 css/colors_default.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-10 06:18 css/colors_red_blue.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-10 06:18 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-10 06:18 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-10 06:18 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-10 06:18 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-10 06:18 css/colors_blue_green.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-10 06:18 css/mathbook-content.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-10 06:18 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-10 06:18 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-10 06:18 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-10 06:18 css/epub.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-10 06:18 css/mathbook-add-on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-10 06:18 css/setcolors.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-10 06:18 css/pretext_add_on.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-10 06:18 css/mathbook-3.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_green_plum.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-10 06:18 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-10 06:18 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-10 06:18 css/README.md
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-10 06:18 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-10 06:18 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-10 06:18 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-10 06:18 pretext/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-10 06:18 pretext/pretext.cfg
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-10 06:18 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-10 06:18 pretext/module-test.py
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-10 06:18 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-10 06:18 pretext/README.md
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-10 06:18 schema/xml.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-10 06:18 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-10 06:18 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-10 06:18 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-10 06:18 schema/pretext.rnc
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-10 06:18 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-10 06:18 schema/pretext-dev.rng
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-10 06:18 schema/build.sh
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-10 06:18 schema/pretext.xsd
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-10 06:18 schema/README.md
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-10 06:18 schema/pretext-validation-plus.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 script/mjsre/
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-10 06:18 script/mbx
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-10 06:18 script/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 06:18 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-10 06:18 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-10 06:18 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-10 06:18 script/mjsre/mj-sre-page.js
-141 files, 4810372 bytes uncompressed, 1017420 bytes compressed:  78.9%
+Zip file size: 1034865 bytes, number of entries: 141
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/utilities/
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-11 06:17 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   611196 b- defN 23-Jun-11 06:17 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-11 06:17 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-11 06:17 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-11 06:17 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-11 06:17 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-11 06:17 xsl/entities.ent
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-11 06:17 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-11 06:17 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-11 06:17 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-11 06:17 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-11 06:17 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-11 06:17 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-11 06:17 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   111931 b- defN 23-Jun-11 06:17 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-11 06:17 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-11 06:17 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-11 06:17 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-11 06:17 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-11 06:17 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-11 06:17 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-11 06:17 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-11 06:17 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-11 06:17 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-11 06:17 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-11 06:17 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-11 06:17 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx   106649 b- defN 23-Jun-11 06:17 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-11 06:17 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-11 06:17 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-11 06:17 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-11 06:17 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-11 06:17 xsl/README.md
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-11 06:17 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-11 06:17 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-11 06:17 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-11 06:17 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-11 06:17 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-11 06:17 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-11 06:17 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-11 06:17 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-11 06:17 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-11 06:17 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-11 06:17 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-11 06:17 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/support/play-button/
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-11 06:17 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-11 06:17 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-11 06:17 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-11 06:17 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-11 06:17 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-11 06:17 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-11 06:17 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-11 06:17 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-11 06:17 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-11 06:17 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-11 06:17 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-11 06:17 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-11 06:17 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-11 06:17 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-11 06:17 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-11 06:17 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-11 06:17 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-11 06:17 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-11 06:17 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-11 06:17 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-11 06:17 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-11 06:17 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-11 06:17 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-11 06:17 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-11 06:17 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-11 06:17 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-11 06:17 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-11 06:17 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-11 06:17 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-11 06:17 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-11 06:17 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-11 06:17 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-11 06:17 css/kindle.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-11 06:17 css/update_css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-11 06:17 css/colors_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-11 06:17 css/colors_red_blue.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-11 06:17 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-11 06:17 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-11 06:17 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-11 06:17 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-11 06:17 css/colors_blue_green.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-11 06:17 css/mathbook-content.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-11 06:17 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-11 06:17 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-11 06:17 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-11 06:17 css/epub.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-11 06:17 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-11 06:17 css/setcolors.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-11 06:17 css/pretext_add_on.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-11 06:17 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_green_plum.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-11 06:17 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-11 06:17 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-11 06:17 css/README.md
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-11 06:17 css/style_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-11 06:17 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-11 06:17 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-11 06:17 pretext/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-11 06:17 pretext/pretext.cfg
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-11 06:17 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-11 06:17 pretext/module-test.py
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-11 06:17 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-11 06:17 pretext/README.md
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-11 06:17 schema/xml.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-11 06:17 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-11 06:17 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-11 06:17 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-11 06:17 schema/pretext.rnc
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-11 06:17 schema/pretext.rng
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-11 06:17 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-11 06:17 schema/build.sh
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-11 06:17 schema/pretext.xsd
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-11 06:17 schema/README.md
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-11 06:17 schema/pretext-validation-plus.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 script/mjsre/
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-11 06:17 script/mbx
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-11 06:17 script/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 06:17 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-11 06:17 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-11 06:17 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-11 06:17 script/mjsre/mj-sre-page.js
+141 files, 4810376 bytes uncompressed, 1017423 bytes compressed:  78.9%
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -9210,15 +9210,15 @@
           <xsl:call-template name="font-awesome"/>
           <!-- and CSS for the entire interactive, into the head -->
           <xsl:apply-templates select="@css"/>
           <!-- load header libraries (for all "slate") -->
           <xsl:apply-templates select="." mode="header-libraries"/>
         </head>
         <!-- ignore MathJax signals everywhere, then enable selectively -->
-        <body class="pretext ignore-math">
+        <body class="ptx-content ignore-math">
           <!-- potential document-id per-page -->
           <xsl:call-template name="document-id"/>
           <!-- React flag -->
           <xsl:call-template name="react-in-use-flag"/>
           <div>
             <!-- the actual interactive bit          -->
             <xsl:apply-templates select="." mode="size-pixels-style-attribute"/>
```

### Comparing `pretext-1.6.1.dev20230610/pretext/generate.py` & `pretext-1.6.1.dev20230611/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/project.py` & `pretext-1.6.1.dev20230611/pretext/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import pickle
 from lxml import etree as ET
 from lxml.etree import Element
 import os
 import shutil
 import logging
 import tempfile
 from . import utils, generate, core
 from . import build as builder
+from . import ASSETS
 from pathlib import Path
 import sys
 from .config.xml_overlay import ShadowXmlDocument
 import typing as t
+import hashlib
 
 log = logging.getLogger("ptxlogger")
 
 
 class Target:
     def __init__(self, xml_element, project_path):
         # construction is done!
@@ -121,14 +124,67 @@
     def xmlid_root(self):
         ele = self.xml_element().find("xmlid-root")
         if ele is None:
             return None
         else:
             return ele.text.strip()
 
+    def asset_hash(self):
+        asset_hash_dict = {}
+        for asset in ASSETS:
+            if asset == "webwork":
+                # WeBWorK must be regenerated every time *any* of the ww exercises change.
+                if len(self.source_xml().xpath(".//webwork[@*|*]")) == 0:
+                    # Only generate a hash if there are actually ww exercises in the source
+                    continue
+                h = hashlib.sha256()
+                for node in self.source_xml().xpath(".//webwork[@*|*]"):
+                    h.update(ET.tostring(node))
+                asset_hash_dict[(asset, "")] = h.digest()
+            elif asset != "ALL":
+                # everything else can be updated individually, if it has an xml:id
+                if len(self.source_xml().xpath(f".//{asset}")) == 0:
+                    # Only generate a hash if there are actually assets of this type in the source
+                    continue
+                h_no_id = hashlib.sha256()
+                for node in self.source_xml().xpath(f".//{asset}"):
+                    # First see if the node has an xml:id, or if it is a child of a node with an xml:id (but we haven't already made this key)
+                    if (
+                        id := node.xpath("@xml:id") or node.xpath("parent::*/@xml:id")
+                    ) and (asset, id[0]) not in asset_hash_dict:
+                        asset_hash_dict[(asset, id[0])] = hashlib.sha256(
+                            ET.tostring(node)
+                        ).digest()
+                    # otherwise collect all non-id'd nodes into a single hash
+                    else:
+                        h_no_id.update(ET.tostring(node))
+                asset_hash_dict[(asset, "")] = h_no_id.digest()
+        return asset_hash_dict
+
+    def save_asset_table(self, asset_table: dict):
+        """
+        Saves the asset_table to a pickle file in the generated assets directory based on the target name.
+        """
+        with open(
+            self.generated_dir().joinpath(f".{self.name()}_assets.pkl"), "wb"
+        ) as f:
+            pickle.dump(asset_table, f)
+
+    def load_asset_table(self) -> dict:
+        """
+        Loads the asset_table from a pickle file in the generated assets directory based on the target name.
+        """
+        try:
+            with open(
+                self.generated_dir().joinpath(f".{self.name()}_assets.pkl"), "rb"
+            ) as f:
+                return pickle.load(f)
+        except Exception:
+            return {}
+
 
 class Project:
     def __init__(self, project_path=None):
         project_path = project_path or utils.project_path()
         xml_element = ET.parse(project_path / "project.ptx").getroot()
         self.__xml_element = xml_element
         self.__project_path = project_path
```

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230611/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230611/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230611/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-10 06:18 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-10 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-10 06:18 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-10 06:17 README.md
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-10 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-10 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-10 06:17 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-10 06:17 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-10 06:17 source/section-2.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-10 06:18 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-11 06:17 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-11 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-11 06:17 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-11 06:17 README.md
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-11 06:17 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-11 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-11 06:17 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-11 06:17 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-11 06:17 source/section-2.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-11 06:17 .devcontainer/devcontainer.json
 14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230611/pretext/templates/resources/book.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-10 06:18 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-10 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-10 06:18 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-10 06:17 README.md
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-10 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-10 06:17 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-10 06:18 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-11 06:17 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-11 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-11 06:17 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-11 06:17 README.md
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-11 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-11 06:17 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-11 06:17 .devcontainer/devcontainer.json
 10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230611/pretext/templates/resources/demo.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-10 06:18 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-10 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-10 06:18 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-10 06:17 README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-10 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-10 06:17 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-10 06:17 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 source/images/
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-10 06:17 source/sec-features.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-10 06:17 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-10 06:17 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-10 06:17 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-10 06:17 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-10 06:17 source/main.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-10 06:17 source/ch-generate.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-10 06:17 source/backmatter.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-10 06:17 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-10 06:17 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-10 06:17 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-10 06:17 source/ch-features.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-10 06:17 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-10 06:17 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-10 06:17 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-10 06:17 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-10 06:17 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-10 06:17 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-10 06:17 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-10 06:17 source/images/cflag.asy
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-10 06:18 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-11 06:17 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-11 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-11 06:17 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-11 06:17 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-11 06:17 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-11 06:17 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-11 06:17 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 source/images/
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-11 06:17 source/sec-features.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-11 06:17 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-11 06:17 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-11 06:17 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-11 06:17 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-11 06:17 source/main.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-11 06:17 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-11 06:17 source/backmatter.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-11 06:17 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-11 06:17 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-11 06:17 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-11 06:17 source/ch-features.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-11 06:17 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-11 06:17 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-11 06:17 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-11 06:17 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-11 06:17 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-11 06:17 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-11 06:17 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-11 06:17 source/images/cflag.asy
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-11 06:17 .devcontainer/devcontainer.json
 34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230611/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230611/pretext/templates/resources/hello.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-10 06:18 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-10 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-10 06:17 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-10 06:17 README.md
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-10 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-10 06:17 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-10 06:18 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-11 06:17 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-11 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-11 06:17 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-11 06:17 README.md
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-11 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-11 06:17 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-11 06:17 .devcontainer/devcontainer.json
 10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230611/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230611/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-10 06:17 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-10 06:18 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-10 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-10 06:17 project.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-10 06:17 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-10 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-10 06:17 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-10 06:18 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 06:17 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-11 06:17 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-11 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-11 06:17 project.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-11 06:17 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-11 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-11 06:17 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-11 06:17 .devcontainer/devcontainer.json
 11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230610/pretext/utils.py` & `pretext-1.6.1.dev20230611/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230610/pyproject.toml` & `pretext-1.6.1.dev20230611/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230610"
+version = "1.6.1.dev20230611"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230610/PKG-INFO` & `pretext-1.6.1.dev20230611/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230610
+Version: 1.6.1.dev20230611
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -234,14 +234,15 @@
 If you run `echo 'alias pr="poetry run"' >> ~/.bashrc` then restart your
 shell, this becomes less of a mouthful:
 
 ```
 pretext --version     # returns system version
 pr pretext --version  # returns version being developed
 ```
+(On Windows, in PowerShell, you get get such an alias with `Function pr {poetry run @Args}`)
 
 #### Steps on Windows
 
 In windows, you can either use the bash shell and follow the directions above,
 or try [pyenv-win](https://github.com/pyenv-win/pyenv-win#installation). In
 the latter case, make sure to follow all the installation instructions, including
 the **Finish the installation**. Then proceed to follow the directions above to
```

