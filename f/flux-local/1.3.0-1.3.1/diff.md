# Comparing `tmp/flux-local-1.3.0.tar.gz` & `tmp/flux-local-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-1.3.0.tar", last modified: Wed May 31 01:52:17 2023, max compression
+gzip compressed data, was "flux-local-1.3.1.tar", last modified: Sun Jun 11 04:43:03 2023, max compression
```

## Comparing `flux-local-1.3.0.tar` & `flux-local-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 01:52:06.000000 flux-local-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-05-31 01:52:17.241509 flux-local-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-31 01:52:06.000000 flux-local-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.237509 flux-local-1.3.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-31 01:52:17.241509 flux-local-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 01:52:06.000000 flux-local-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 04:42:53.000000 flux-local-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-11 04:43:03.138561 flux-local-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-11 04:42:53.000000 flux-local-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.134560 flux-local-1.3.1/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-11 04:43:03.138561 flux-local-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 04:42:53.000000 flux-local-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_manifest.py
```

### Comparing `flux-local-1.3.0/LICENSE` & `flux-local-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/PKG-INFO` & `flux-local-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.3.0
+Version: 1.3.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -321,15 +321,15 @@
           path: ${{ matrix.cluster_path }}
           resource: ${{ matrix.resource }}
       - name: PR Comments
         uses: mshick/add-pr-comment@v2
         if: ${{ steps.diff.outputs.diff != '' }}
         with:
           repo-token: ${{ secrets.GITHUB_TOKEN }}
-          message-id: ${{ matrix.cluster_path }}/${{ matrix.resource }}
+          message-id: ${{ github.event.pull_request.number }}/${{ matrix.cluster_path }}/${{ matrix.resource }}
           message-failure: Unable to post kustomization diff
           message: |
             `````diff
             ${{ steps.diff.outputs.diff }}
             `````
 ```
```

### Comparing `flux-local-1.3.0/README.md` & `flux-local-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
           path: ${{ matrix.cluster_path }}
           resource: ${{ matrix.resource }}
       - name: PR Comments
         uses: mshick/add-pr-comment@v2
         if: ${{ steps.diff.outputs.diff != '' }}
         with:
           repo-token: ${{ secrets.GITHUB_TOKEN }}
-          message-id: ${{ matrix.cluster_path }}/${{ matrix.resource }}
+          message-id: ${{ github.event.pull_request.number }}/${{ matrix.cluster_path }}/${{ matrix.resource }}
           message-failure: Unable to post kustomization diff
           message: |
             `````diff
             ${{ steps.diff.outputs.diff }}
             `````
 ```
```

### Comparing `flux-local-1.3.0/flux_local/command.py` & `flux-local-1.3.1/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/exceptions.py` & `flux-local-1.3.1/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/git_repo.py` & `flux-local-1.3.1/flux_local/git_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,14 +328,26 @@
     docs = await cmd.objects()
     return [
         Kustomization.parse_doc(doc)
         for doc in filter(CLUSTER_KUSTOMIZE_DOMAIN_FILTER, docs)
     ]
 
 
+def find_source_kustomization(
+    search: Path, node_map: dict[Path, Kustomization]
+) -> list[Kustomization]:
+    """Return all source Kustomizations that might manage the specified path."""
+    results = []
+    set(node_map)
+    for parent in search.parents:
+        if node := node_map.get(parent):
+            results.append(node)
+    return results
+
+
 def find_path_parent(search: Path, prefixes: set[Path]) -> Path | None:
     """Return a prefix path that is a parent of the search path."""
     for parent in search.parents:
         if parent in prefixes:
             return parent
     return None
 
@@ -366,57 +378,74 @@
             )
 
         # Source path is relative to the search path. Update to have the
         # full prefix relative to the root.
         for kustomization in docs:
             if not kustomization.source_path:
                 continue
-            _LOGGER.debug(
-                "Updating relative path: %s, %s, %s",
-                root,
-                path,
-                kustomization.source_path,
-            )
             kustomization.source_path = str(
                 ((root / path) / kustomization.source_path).relative_to(root)
             )
+            _LOGGER.debug(
+                "Updated relative path: %s => %s",
+                node_name(kustomization),
+                kustomization.source_path,
+            )
 
         visited |= set({path})
 
         _LOGGER.debug("Found %s Kustomizations", len(docs))
+        result_docs = []
         for doc in docs:
             found_path: Path | None = None
             _LOGGER.debug(
                 "Kustomization '%s' has sourceRef.kind '%s' of '%s'",
                 doc.name,
                 doc.source_kind,
                 doc.source_name,
             )
             if not doc.source_kind or doc.source_kind == GIT_REPO_KIND:
                 found_path = Path(doc.path)
             elif doc.source_kind == OCI_REPO_KIND:
                 for source in path_selector.sources or ():
                     if source.name == doc.source_name:
                         found_path = source.root / doc.path
+                        doc.path = str(found_path)
+                        _LOGGER.debug(
+                            "Updated Source for OCIRepository %s: %s",
+                            doc.name,
+                            doc.path,
+                        )
                         break
+
             elif not doc.source_kind or doc.source_kind == GIT_REPO_KIND:
                 found_path = Path(doc.path)
 
             if not found_path:
                 _LOGGER.debug("Skipping kustomization %s; not known source", doc.name)
                 continue
 
             if not find_path_parent(found_path, visited) and found_path not in visited:
                 path_queue.put(found_path)
             else:
                 _LOGGER.debug("Already visited %s", found_path)
-        kustomizations.extend(docs)
+            result_docs.append(doc)
+        kustomizations.extend(result_docs)
     return kustomizations
 
 
+def node_name(ks: Kustomization) -> str:
+    """Return a unique node name for the Kustomization.
+
+    This includes the path since it needs to be unique within the entire
+    repository since we support multi-cluster.
+    """
+    return f"{ks.namespaced_name} @ {ks.id_name}"
+
+
 def make_clusters(
     kustomizations: list[Kustomization], sources: list[Source] | None = None
 ) -> list[Cluster]:
     """Convert the flat list of Kustomizations into a Cluster.
 
     This will reverse engineer which Kustomizations are root nodes for the cluster
     based on the parent paths. Root Kustomizations are made the cluster and everything
@@ -424,52 +453,53 @@
     """
     if not sources:
         sources = []
 
     # Build a directed graph from a kustomization path to the path
     # of the kustomization that created it.
     graph = networkx.DiGraph()
-    parent_paths = set([Path(ks.path) for ks in kustomizations])
+    node_path_map = {Path(ks.path): ks for ks in kustomizations if ks.source_path}
     for ks in kustomizations:
         if not ks.source_path:
             raise InputException(
                 "Kustomization did not have source path; Old kustomize?"
             )
 
-        # OCIRepositories may be build pointed at a subset of the cluster which can
-        # only be determined based on input command line flags
-        if ks.source_kind == OCI_REPO_KIND:
-            if root := next(
-                map(
-                    source_root, filter(has_source_name(ks.source_name or ""), sources)
-                ),
-                None,
-            ):
-                ks.path = str(root / ks.path)
-                _LOGGER.debug(
-                    "Updated Source for OCIRepository %s: %s", ks.name, ks.path
-                )
-            else:
-                _LOGGER.debug("Excluding OCIRepository without source %s", ks.name)
-                continue
-
-        path = Path(ks.path)
-        graph.add_node(path, ks=ks)
+        graph.add_node(node_name(ks), ks=ks)
 
         # Find the parent Kustomization that produced this based on the
         # matching the kustomize source parent paths with a Kustomization
         # target path.
         source = Path(ks.source_path)
-        if (
-            parent_path := find_path_parent(source, parent_paths)
-        ) and parent_path != path:
-            _LOGGER.debug("Found parent %s => %s", path, parent_path)
-            graph.add_edge(parent_path, path)
+        _LOGGER.debug("--- Examining candidate Kustomization ---")
+        _LOGGER.debug("Ks         : %s", ks.namespaced_name)
+        _LOGGER.debug("Path       : %s", Path(ks.path))
+        _LOGGER.debug("Source path: %s", source)
+        source_kustomizations = find_source_kustomization(source, node_path_map)
+        _LOGGER.debug(
+            "Possible sources: %s", [f"{node_name(ks)}" for ks in source_kustomizations]
+        )
+        if source_kustomizations:
+            while source_kustomizations:
+                candidate = source_kustomizations.pop(0)
+                # These names can be compared since they are within the scope of
+                # the source path so within the same cluster.
+                if candidate.namespaced_name != ks.namespaced_name:
+                    _LOGGER.debug(
+                        "Found parent %s => %s",
+                        ks.namespaced_name,
+                        candidate.namespaced_name,
+                    )
+                    graph.add_edge(node_name(candidate), node_name(ks))
+                else:
+                    _LOGGER.debug(
+                        "Skipping candidate source %s", candidate.namespaced_name
+                    )
         else:
-            _LOGGER.debug("No parent for %s (%s)", path, source)
+            _LOGGER.debug("No parent for %s (source=%s)", node_name(ks), source)
 
     # Clusters are subgraphs within the graph that are connected, with the root
     # node being the cluster itself. All children Kustomizations are flattended.
     _LOGGER.debug("Creating clusters based on connectivity")
     roots = [node for node, degree in graph.in_degree() if degree == 0]
     roots.sort()
     clusters: list[Cluster] = []
```

### Comparing `flux-local-1.3.0/flux_local/helm.py` & `flux-local-1.3.1/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/kustomize.py` & `flux-local-1.3.1/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/manifest.py` & `flux-local-1.3.1/flux_local/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,19 @@
         )
 
     @property
     def id_name(self) -> str:
         """Identifier for the Kustomization in tests"""
         return f"{self.path}"
 
+    @property
+    def namespaced_name(self, sep: str = "/") -> str:
+        """Return the namespace and name concatenated as an id."""
+        return f"{self.namespace}{sep}{self.name}"
+
     _COMPACT_EXCLUDE_FIELDS = {
         "helm_releases": {
             "__all__": HelmRelease._COMPACT_EXCLUDE_FIELDS,
         },
         "cluster_policies": {
             "__all__": ClusterPolicy._COMPACT_EXCLUDE_FIELDS,
         },
```

### Comparing `flux-local-1.3.0/flux_local/tool/build.py` & `flux-local-1.3.1/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/diff.py` & `flux-local-1.3.1/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/flux_local.py` & `flux-local-1.3.1/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/format.py` & `flux-local-1.3.1/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/get.py` & `flux-local-1.3.1/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/selector.py` & `flux-local-1.3.1/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/test.py` & `flux-local-1.3.1/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local/tool/visitor.py` & `flux-local-1.3.1/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/flux_local.egg-info/PKG-INFO` & `flux-local-1.3.1/flux_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.3.0
+Version: 1.3.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -321,15 +321,15 @@
           path: ${{ matrix.cluster_path }}
           resource: ${{ matrix.resource }}
       - name: PR Comments
         uses: mshick/add-pr-comment@v2
         if: ${{ steps.diff.outputs.diff != '' }}
         with:
           repo-token: ${{ secrets.GITHUB_TOKEN }}
-          message-id: ${{ matrix.cluster_path }}/${{ matrix.resource }}
+          message-id: ${{ github.event.pull_request.number }}/${{ matrix.cluster_path }}/${{ matrix.resource }}
           message-failure: Unable to post kustomization diff
           message: |
             `````diff
             ${{ steps.diff.outputs.diff }}
             `````
 ```
```

### Comparing `flux-local-1.3.0/flux_local.egg-info/SOURCES.txt` & `flux-local-1.3.1/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/setup.cfg` & `flux-local-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 1.3.0
+version = 1.3.1
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-1.3.0/tests/test_command.py` & `flux-local-1.3.1/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/tests/test_git_repo.py` & `flux-local-1.3.1/tests/test_git_repo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -340,18 +340,18 @@
 
     clusters = make_clusters(kustomizations)
     assert len(clusters) == 1
     cluster = clusters[0]
     assert cluster.name == "cluster"
     assert cluster.namespace == "flux-system"
     assert [ks.path for ks in cluster.kustomizations] == [
+        "./kubernetes/flux",
         "./kubernetes/apps",
         "./kubernetes/apps/rook-ceph/rook-ceph/app",
         "./kubernetes/apps/volsync/volsync/app",
-        "./kubernetes/flux",
     ]
 
 
 async def test_kustomization_traversal_multi_cluster() -> None:
     """Test discovery of multiple clusters in the repo."""
 
     results = [
```

### Comparing `flux-local-1.3.0/tests/test_helm.py` & `flux-local-1.3.1/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/tests/test_kustomize.py` & `flux-local-1.3.1/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.0/tests/test_manifest.py` & `flux-local-1.3.1/tests/test_manifest.py`

 * *Files identical despite different names*

