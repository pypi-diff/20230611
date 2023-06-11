# Comparing `tmp/unipressed-1.1.0.tar.gz` & `tmp/unipressed-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipressed-1.1.0.tar", max compression
+gzip compressed data, was "unipressed-1.2.0.tar", max compression
```

## Comparing `unipressed-1.1.0.tar` & `unipressed-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,37 @@
--rw-r--r--   0        0        0     1071 2022-08-03 12:47:50.444610 unipressed-1.1.0/LICENSE
--rw-r--r--   0        0        0    21175 2022-09-12 11:18:15.811713 unipressed-1.1.0/README.md
--rw-r--r--   0        0        0     1600 2022-09-12 11:17:33.103306 unipressed-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       83 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/__init__.py
--rw-r--r--   0        0        0     1045 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/__init__.py
--rw-r--r--   0        0        0      480 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/arba.py
--rw-r--r--   0        0        0      590 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/citations.py
--rw-r--r--   0        0        0     6827 2022-08-27 12:12:46.298538 unipressed-1.1.0/unipressed/dataset/core.py
--rw-r--r--   0        0        0      456 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/database.py
--rw-r--r--   0        0        0      486 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/diseases.py
--rw-r--r--   0        0        0        0 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/__init__.py
--rw-r--r--   0        0        0     1719 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/arba.py
--rw-r--r--   0        0        0     1260 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/citations.py
--rw-r--r--   0        0        0      940 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/database.py
--rw-r--r--   0        0        0      906 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/diseases.py
--rw-r--r--   0        0        0     1408 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/keywords.py
--rw-r--r--   0        0        0     1003 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/locations.py
--rw-r--r--   0        0        0     2157 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/proteomes.py
--rw-r--r--   0        0        0     2758 2022-08-26 12:21:27.486760 unipressed-1.1.0/unipressed/dataset/generated_types/taxonomy.py
--rw-r--r--   0        0        0     3881 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/generated_types/uniparc.py
--rw-r--r--   0        0        0    42173 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/generated_types/uniprotkb.py
--rw-r--r--   0        0        0     2653 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/generated_types/uniref.py
--rw-r--r--   0        0        0     2086 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/generated_types/unirule.py
--rw-r--r--   0        0        0      601 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/keywords.py
--rw-r--r--   0        0        0      495 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/locations.py
--rw-r--r--   0        0        0      495 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/proteomes.py
--rw-r--r--   0        0        0     6804 2022-08-27 12:12:46.298538 unipressed-1.1.0/unipressed/dataset/search.py
--rw-r--r--   0        0        0      665 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/taxonomy.py
--rw-r--r--   0        0        0      235 2022-08-23 17:28:08.268736 unipressed-1.1.0/unipressed/dataset/type_vars.py
--rw-r--r--   0        0        0      623 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/uniparc.py
--rw-r--r--   0        0        0      715 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/uniprotkb.py
--rw-r--r--   0        0        0      503 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/uniref.py
--rw-r--r--   0        0        0      527 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/dataset/unirule.py
--rw-r--r--   0        0        0       71 2022-08-26 12:21:27.490760 unipressed-1.1.0/unipressed/id_mapping/__init__.py
--rw-r--r--   0        0        0     2924 2022-09-12 11:21:32.873304 unipressed-1.1.0/unipressed/id_mapping/core.py
--rw-r--r--   0        0        0     3390 2022-08-22 15:57:58.412004 unipressed-1.1.0/unipressed/id_mapping/types.py
--rw-r--r--   0        0        0      444 2022-08-23 15:06:14.038467 unipressed-1.1.0/unipressed/util.py
--rw-r--r--   0        0        0    22530 1970-01-01 00:00:00.000000 unipressed-1.1.0/setup.py
--rw-r--r--   0        0        0    21947 1970-01-01 00:00:00.000000 unipressed-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 12:43:55.653550 unipressed-1.2.0/LICENSE
+-rw-r--r--   0        0        0    21175 2023-06-05 12:43:55.657549 unipressed-1.2.0/README.md
+-rw-r--r--   0        0        0     1600 2023-06-11 07:14:56.292402 unipressed-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-05 14:00:21.355796 unipressed-1.2.0/unipressed/dataset/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-05 13:57:49.292173 unipressed-1.2.0/unipressed/dataset/arba.py
+-rw-r--r--   0        0        0      590 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/dataset/citations.py
+-rw-r--r--   0        0        0     6939 2023-06-11 07:14:56.292402 unipressed-1.2.0/unipressed/dataset/core.py
+-rw-r--r--   0        0        0      456 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/dataset/database.py
+-rw-r--r--   0        0        0      486 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/dataset/diseases.py
+-rw-r--r--   0        0        0     1695 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/arba.py
+-rw-r--r--   0        0        0     1254 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/citations.py
+-rw-r--r--   0        0        0      934 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/database.py
+-rw-r--r--   0        0        0      900 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/diseases.py
+-rw-r--r--   0        0        0     1402 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/keywords.py
+-rw-r--r--   0        0        0      997 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/locations.py
+-rw-r--r--   0        0        0     2081 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/proteomes.py
+-rw-r--r--   0        0        0     2752 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/taxonomy.py
+-rw-r--r--   0        0        0     3907 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/uniparc.py
+-rw-r--r--   0        0        0    27932 2023-06-11 07:14:56.300402 unipressed-1.2.0/unipressed/dataset/generated_types/uniprotkb.py
+-rw-r--r--   0        0        0     2419 2023-06-11 07:14:56.300402 unipressed-1.2.0/unipressed/dataset/generated_types/uniref.py
+-rw-r--r--   0        0        0     2056 2023-06-11 07:14:56.300402 unipressed-1.2.0/unipressed/dataset/generated_types/unirule.py
+-rw-r--r--   0        0        0      601 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/keywords.py
+-rw-r--r--   0        0        0      495 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/locations.py
+-rw-r--r--   0        0        0      495 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/proteomes.py
+-rw-r--r--   0        0        0     6804 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/search.py
+-rw-r--r--   0        0        0      665 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/taxonomy.py
+-rw-r--r--   0        0        0      235 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/type_vars.py
+-rw-r--r--   0        0        0      623 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/uniparc.py
+-rw-r--r--   0        0        0      715 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/uniprotkb.py
+-rw-r--r--   0        0        0      503 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/uniref.py
+-rw-r--r--   0        0        0      527 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/unirule.py
+-rw-r--r--   0        0        0       71 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/id_mapping/__init__.py
+-rw-r--r--   0        0        0     2913 2023-06-05 13:55:45.672479 unipressed-1.2.0/unipressed/id_mapping/core.py
+-rw-r--r--   0        0        0     3390 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/id_mapping/types.py
+-rw-r--r--   0        0        0      444 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/util.py
+-rw-r--r--   0        0        0    21998 1970-01-01 00:00:00.000000 unipressed-1.2.0/PKG-INFO
```

### Comparing `unipressed-1.1.0/LICENSE` & `unipressed-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/README.md` & `unipressed-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/pyproject.toml` & `unipressed-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unipressed"
-version = "1.1.0"
+version = "1.2.0"
 description = "Comprehensive Python client for the Uniprot REST API"
 authors = ["Michael Milton <michael.r.milton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://multimeric.github.io/Unipressed"
 repository = "https://github.com/multimeric/Unipressed"
```

### Comparing `unipressed-1.1.0/unipressed/dataset/__init__.py` & `unipressed-1.2.0/unipressed/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/citations.py` & `unipressed-1.2.0/unipressed/dataset/citations.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/core.py` & `unipressed-1.2.0/unipressed/dataset/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,21 +40,27 @@
     @classmethod
     def search(
         cls,
         query: QueryType,
         format: FormatType | Literal["json"] = "json",
         fields: Iterable[FieldsType] | None = None,
         size: int = 500,
+        include_isoform: bool = True,
     ) -> Search[QueryType, JsonResultType, FieldsType, FormatType]:
         """
         Creates an object that can be used to perform a search query over this dataset.
         Refer to the [unipressed.dataset.search.Search][] reference for more information on how to use it.
         """
         return Search[QueryType, JsonResultType, FieldsType, FormatType](
-            query=query, format=format, dataset=cls.name(), fields=fields, size=size
+            query=query,
+            format=format,
+            dataset=cls.name(),
+            fields=fields,
+            size=size,
+            include_isoform=include_isoform,
         )
 
     @overload
     @classmethod
     def fetch_one(
         cls, id: str, format: Literal["json"] = "json", parse: Literal[True] = True
     ) -> JsonResultType:
@@ -157,15 +163,14 @@
 
 class FetchManyClient(DatasetClient[QueryType, JsonResultType, FieldsType, FormatType]):
     """
     Dataset subclass for datasets that can be queried by multiple IDs. Not all datasets support this.
     """
 
     @classmethod
-    @abstractmethod
     def _bulk_id_param(cls) -> str:
         """
         The name of the GET query parameter used to define the list of IDs in a bulk query.
         """
         return cls._bulk_endpoint()
 
     @classmethod
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/arba.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/arba.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,35 +18,33 @@
     organism: NotRequired[str]
     "Organism [OS]\ne.g. saccharomyces"
     taxonomy: NotRequired[str]
     "Taxonomy [OC]\ne.g. human"
     ec: NotRequired[str]
     "Enzyme classification [EC]\ne.g. 1.1.2.3"
     cc_cofactor: NotRequired[str]
-    "Cc cofactor\ne.g. 29105"
+    "Cofactor\ne.g. 29105"
     cc_catalytic_activity: NotRequired[str]
-    "Cc catalytic activity\ne.g. tyrosine"
+    "Catalytic activity\ne.g. tyrosine"
     cc_activity_regulation: NotRequired[str]
-    "Cc activity regulation\ne.g. inhibited"
+    "Activity regulation\ne.g. inhibited"
     cc_pathway: NotRequired[str]
-    "Cc pathway\ne.g. metabolism"
+    "Pathway\ne.g. metabolism"
     cc_subcellular_location: NotRequired[str]
-    "Cc subcellular location\ne.g. membrane"
+    "Subcellular location term\ne.g. membrane"
     cc_subcellular_location_note: NotRequired[str]
-    "Cc subcellular location note\ne.g. membrane"
+    "Note\ne.g. membrane"
     cc_domain: NotRequired[str]
-    "Cc domain\ne.g. conformation"
+    "Domain comments [CC]\ne.g. conformation"
     family: NotRequired[str]
     "Protein family\ne.g. pa28"
     cc_similarity: NotRequired[str]
-    "Cc similarity\ne.g. phosphatase"
+    "Comment similarity\ne.g. phosphatase"
     keyword: NotRequired[str]
     "Keyword [KW]\ne.g. chromosomal"
 
 
 ArbaQuery: TypeAlias = Union[ArbaQueryDict, str]
 ArbaArba: TypeAlias = Literal[
     "rule_id", "statistics", "taxonomic_scope", "annotation_covered"
 ]
-ArbaFields: TypeAlias = Literal[
-    ArbaArba,
-]
+ArbaFields: TypeAlias = Literal[ArbaArba,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/citations.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/citations.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,10 +39,8 @@
     "first_page",
     "last_page",
     "volume",
     "reference",
     "lit_abstract",
     "statistics",
 ]
-CitationsFields: TypeAlias = Literal[
-    CitationsLiterature,
-]
+CitationsFields: TypeAlias = Literal[CitationsLiterature,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/database.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,8 @@
     "doi_id",
     "link_type",
     "server",
     "dbUrl",
     "category",
     "statistics",
 ]
-DatabaseFields: TypeAlias = Literal[
-    DatabaseCrossReference,
-]
+DatabaseFields: TypeAlias = Literal[DatabaseCrossReference,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/diseases.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/diseases.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,8 @@
     "acronym",
     "definition",
     "alternative_names",
     "cross_references",
     "keywords",
     "statistics",
 ]
-DiseasesFields: TypeAlias = Literal[
-    DiseasesDisease,
-]
+DiseasesFields: TypeAlias = Literal[DiseasesDisease,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/keywords.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/keywords.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,10 +30,8 @@
     "synonyms",
     "gene_ontologies",
     "links",
     "children",
     "parents",
     "statistics",
 ]
-KeywordsFields: TypeAlias = Literal[
-    KeywordsKeyword,
-]
+KeywordsFields: TypeAlias = Literal[KeywordsKeyword,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/locations.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,10 +32,8 @@
     "note",
     "references",
     "links",
     "is_a",
     "part_of",
     "statistics",
 ]
-LocationsFields: TypeAlias = Literal[
-    LocationsSubcellularLocation,
-]
+LocationsFields: TypeAlias = Literal[LocationsSubcellularLocation,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/proteomes.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/proteomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,19 @@
     "Genome Assembly\ne.g. GCA_000001405.27"
     cpd: NotRequired[Cpd]
     "CPD (Complete Proteome Detector)\ne.g. 1\n* 1: Standard\n* 2: Close to standard (high value)\n* 3: Close to standard (low value)\n* 4: Outlier (high value)\n* 5: Outlier (low value)\n* 6: Unknown"
     busco: NotRequired[
         tuple[
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
         ]
     ]
     "BUSCO (Complete %)\ne.g. 97"
 
 
 ProteomesQuery: TypeAlias = Union[ProteomesQueryDict, str]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/taxonomy.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/taxonomy.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,10 +82,8 @@
     "lineage",
     "strains",
     "parent",
     "hosts",
     "links",
     "statistics",
 ]
-TaxonomyFields: TypeAlias = Literal[
-    TaxonomyTaxonomy,
-]
+TaxonomyFields: TypeAlias = Literal[TaxonomyTaxonomy,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/uniparc.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/uniparc.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,32 +26,28 @@
     taxonomy_id: NotRequired[str]
     "Taxonomy id"
     gene: NotRequired[str]
     "Gene name [GN]\ne.g. sample gene"
     protein: NotRequired[str]
     "Protein name\ne.g. sample protein"
     database: NotRequired[str]
-    "Database\ne.g. sample database\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBLWGS: EMBLWGS\n* EMBL_CON: EMBL_CON\n* EMBL_TPA: EMBL_TPA\n* EMBL_TSA: EMBL_TSA\n* Ensembl: Ensembl\n* EPO: EPO\n* FlyBase: FlyBase\n* H-InvDB: H-InvDB\n* IPI: IPI\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* PIR: PIR\n* PIRARC: PIRARC\n* PRF: PRF\n* RefSeq: RefSeq\n* REMTREMBL: REMTREMBL\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TREMBLNEW: TREMBLNEW\n* TREMBL_VARSPLIC: TREMBL_VARSPLIC\n* TROME: TROME\n* UNIMES: UNIMES\n* USPTO: USPTO\n* VectorBase: VectorBase\n* VEGA: VEGA\n* WormBase: WormBase\n* WBParaSite: WBParaSite"
+    "Database\ne.g. sample database\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBL_CON: EMBL_CON\n* EMBL_TPA: EMBL_TPA\n* EMBL_TSA: EMBL_TSA\n* EMBLWGS: EMBLWGS\n* Ensembl: Ensembl\n* EnsemblRapid: EnsemblRapid\n* EPO: EPO\n* FlyBase: FlyBase\n* FusionGDB: FusionGDB\n* H-InvDB: H-InvDB\n* IPI: IPI\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* PIR: PIR\n* PIRARC: PIRARC\n* PRF: PRF\n* RefSeq: RefSeq\n* REMTREMBL: REMTREMBL\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TREMBLNEW: TREMBLNEW\n* TREMBL_VARSPLIC: TREMBL_VARSPLIC\n* TROME: TROME\n* UNIMES: UNIMES\n* USPTO: USPTO\n* VectorBase: VectorBase\n* VEGA: VEGA\n* WBParaSite: WBParaSite\n* WormBase: WormBase"
     active: NotRequired[str]
-    "Active\ne.g. sample active\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBLWGS: EMBLWGS\n* EMBL_CON: EMBL_CON\n* EMBL_TSA: EMBL_TSA\n* Ensembl: Ensembl\n* EPO: EPO\n* FlyBase: FlyBase\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* RefSeq: RefSeq\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TROME: TROME\n* USPTO: USPTO\n* VEGA: VEGA\n* WormBase: WormBase\n* WBParaSite: WBParaSite"
+    "Active\ne.g. sample active\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBL_CON: EMBL_CON\n* EMBL_TSA: EMBL_TSA\n* EMBLWGS: EMBLWGS\n* Ensembl: Ensembl\n* EnsemblRapid: EnsemblRapid\n* EPO: EPO\n* FlyBase: FlyBase\n* FusionGDB: FusionGDB\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* RefSeq: RefSeq\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TROME: TROME\n* USPTO: USPTO\n* VEGA: VEGA\n* WBParaSite: WBParaSite\n* WormBase: WormBase"
     checksum: NotRequired[str]
     "Checksum (CRC64/MD5)\ne.g. sample checksum"
     length: NotRequired[
         tuple[
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
         ]
     ]
     "Sequence length\ne.g. [100 TO 300]"
     dbid: NotRequired[str]
     "Database ID\ne.g. AAC02967"
     feature_id: NotRequired[str]
@@ -61,17 +57,15 @@
 
 
 UniparcQuery: TypeAlias = Union[UniparcQueryDict, str]
 UniparcNamesTaxonomy: TypeAlias = Literal[
     "upi", "gene", "organism_id", "organism", "protein", "proteome"
 ]
 UniparcSequences: TypeAlias = Literal["checksum", "length", "sequence"]
-UniparcMiscellaneous: TypeAlias = Literal[
-    "accession",
-]
+UniparcMiscellaneous: TypeAlias = Literal["accession",]
 UniparcDateOf: TypeAlias = Literal["first_seen", "last_seen"]
 UniparcFamilyDomains: TypeAlias = Literal[
     "CDD",
     "Gene3D",
     "HAMAP",
     "PANTHER",
     "Pfam",
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/uniref.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/uniref.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,57 +21,45 @@
     "Cluster name\ne.g. sample name"
     identity: NotRequired[Identity]
     "Sequence identity\ne.g. sample identity\n* 1.0: 100%\n* 0.9: 90%\n* 0.5: 50%"
     count: NotRequired[
         tuple[
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
         ]
     ]
     "Cluster size\ne.g. [100 TO 300]"
     length: NotRequired[
         tuple[
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
             Union[
                 int,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
         ]
     ]
     "Sequence length\ne.g. [100 TO 300]"
     created: NotRequired[
         tuple[
             Union[
                 date,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
             Union[
                 date,
-                Literal[
-                    "*",
-                ],
+                Literal["*",],
             ],
         ]
     ]
     "Date published\ne.g. [2011-10-10 TO 2019-10-10]"
     uniprot_id: NotRequired[str]
     "UniProtKB ID/AC\ne.g. sample uniprot id"
     upi: NotRequired[str]
@@ -86,13 +74,11 @@
 
 UnirefQuery: TypeAlias = Union[UnirefQueryDict, str]
 UnirefNamesTaxonomy: TypeAlias = Literal[
     "id", "name", "common_taxon", "common_taxonid", "organism_id", "organism"
 ]
 UnirefSequences: TypeAlias = Literal["identity", "length", "sequence"]
 UnirefMiscellaneous: TypeAlias = Literal["types", "members", "count"]
-UnirefDateOf: TypeAlias = Literal[
-    "created",
-]
+UnirefDateOf: TypeAlias = Literal["created",]
 UnirefFields: TypeAlias = Literal[
     UnirefNamesTaxonomy, UnirefSequences, UnirefMiscellaneous, UnirefDateOf
 ]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/generated_types/unirule.py` & `unipressed-1.2.0/unipressed/dataset/generated_types/unirule.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,35 +20,35 @@
     organism: NotRequired[str]
     "Organism [OS]\ne.g. saccharomyces"
     taxonomy: NotRequired[str]
     "Taxonomy [OC]\ne.g. human"
     ec: NotRequired[str]
     "Enzyme classification [EC]\ne.g. 1.1.2.3"
     cc_cofactor: NotRequired[str]
-    "Cc cofactor\ne.g. 29105"
+    "Cofactor\ne.g. 29105"
     cc_cofactor_note: NotRequired[str]
-    "Cc cofactor note\ne.g. subunit"
+    "Cofactor note\ne.g. subunit"
     cc_catalytic_activity: NotRequired[str]
-    "Cc catalytic activity\ne.g. tyrosine"
+    "Catalytic activity\ne.g. tyrosine"
     cc_activity_regulation: NotRequired[str]
-    "Cc activity regulation\ne.g. inhibited"
+    "Activity regulation\ne.g. inhibited"
     cc_pathway: NotRequired[str]
-    "Cc pathway\ne.g. metabolism"
+    "Pathway\ne.g. metabolism"
     cc_subcellular_location: NotRequired[str]
-    "Cc subcellular location\ne.g. membrane"
+    "Subcellular location term\ne.g. membrane"
     cc_subcellular_location_note: NotRequired[str]
-    "Cc subcellular location note\ne.g. membrane"
+    "Note\ne.g. membrane"
     cc_induction: NotRequired[str]
-    "Cc induction\ne.g. calcium"
+    "Induction\ne.g. calcium"
     cc_domain: NotRequired[str]
-    "Cc domain\ne.g. conformation"
+    "Domain comments [CC]\ne.g. conformation"
     family: NotRequired[str]
     "Protein family\ne.g. pa28"
     cc_similarity: NotRequired[str]
-    "Cc similarity\ne.g. phosphatase"
+    "Comment similarity\ne.g. phosphatase"
     go: NotRequired[str]
     "Gene Ontology [GO]\ne.g. 0009986"
     keyword: NotRequired[str]
     "Keyword [KW]\ne.g. chromosomal"
 
 
 UniruleQuery: TypeAlias = Union[UniruleQueryDict, str]
@@ -56,10 +56,8 @@
     "rule_id",
     "template_entries",
     "statistics",
     "taxonomic_scope",
     "annotation_covered",
     "predicted_protein_name",
 ]
-UniruleFields: TypeAlias = Literal[
-    UniruleUnirule,
-]
+UniruleFields: TypeAlias = Literal[UniruleUnirule,]
```

### Comparing `unipressed-1.1.0/unipressed/dataset/keywords.py` & `unipressed-1.2.0/unipressed/dataset/keywords.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/search.py` & `unipressed-1.2.0/unipressed/dataset/search.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/taxonomy.py` & `unipressed-1.2.0/unipressed/dataset/taxonomy.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/uniparc.py` & `unipressed-1.2.0/unipressed/dataset/uniparc.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/uniprotkb.py` & `unipressed-1.2.0/unipressed/dataset/uniprotkb.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/dataset/unirule.py` & `unipressed-1.2.0/unipressed/dataset/unirule.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/unipressed/id_mapping/core.py` & `unipressed-1.2.0/unipressed/id_mapping/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,8 +82,8 @@
                 raise IdMappingError(
                     "UniProt has not yet processed the results, consider using time.sleep() to wait until they are complete."
                 )
             else:
                 yield from parsed["results"]
 
 
-IdMappingResult: TypeAlias = TypedDict("IdMappingResult", {"from": str, "to": str})
+IdMappingResult = TypedDict("IdMappingResult", {"from": str, "to": str})
```

### Comparing `unipressed-1.1.0/unipressed/id_mapping/types.py` & `unipressed-1.2.0/unipressed/id_mapping/types.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.1.0/setup.py` & `unipressed-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,311 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: unipressed
+Version: 1.2.0
+Summary: Comprehensive Python client for the Uniprot REST API
+Home-page: https://multimeric.github.io/Unipressed
+License: MIT
+Author: Michael Milton
+Author-email: michael.r.milton@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
+Project-URL: Repository, https://github.com/multimeric/Unipressed
+Description-Content-Type: text/markdown
 
-packages = \
-['unipressed',
- 'unipressed.dataset',
- 'unipressed.dataset.generated_types',
- 'unipressed.id_mapping']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.28.1,<3.0.0', 'typing-extensions>=4.3.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'unipressed',
-    'version': '1.1.0',
-    'description': 'Comprehensive Python client for the Uniprot REST API',
-    'long_description': '# Unipressed\n\n**Please visit the [project website](https://multimeric.github.io/Unipressed/) for more comprehensive documentation.**\n\n## Introduction\n\nUnipressed (Uniprot REST) is an API client for the protein database [Uniprot](https://www.uniprot.org/).\nIt provides thoroughly typed and documented code to ensure your use of the library is easy, fast, and correct!\n\n### Example\nLet\'s say we\'re interested in very long proteins that are encoded within a chloroplast, in any organism:\n\n```python\nfrom unipressed import UniprotkbClient\n\nfor record in UniprotkbClient.search(\n    query={\n        "and_": [\n            {"organelle": "chloroplast"},\n            {"length": (5000, "*")}\n        ]\n    },\n    fields=["length", "gene_names"]\n).each_record():\n    display(record)\n```\n\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">\n<span style="font-weight: bold">{</span>\n    <span style="color: #008000; text-decoration-color: #008000">\'primaryAccession\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'A0A088CK67\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'genes\'</span>: <span style="font-weight: bold">[</span>\n        <span style="font-weight: bold">{</span>\n            <span style="color: #008000; text-decoration-color: #008000">\'geneName\'</span>: <span style="font-weight: bold">{</span>\n                <span style="color: #008000; text-decoration-color: #008000">\'evidences\'</span>: <span style="font-weight: bold">[{</span><span style="color: #008000; text-decoration-color: #008000">\'evidenceCode\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'ECO:0000313\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'source\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'EMBL\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'id\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'AID67672.1\'</span><span style="font-weight: bold">}]</span>,\n                <span style="color: #008000; text-decoration-color: #008000">\'value\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'ftsH\'</span>\n            <span style="font-weight: bold">}</span>\n        <span style="font-weight: bold">}</span>\n    <span style="font-weight: bold">]</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'sequence\'</span>: <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">\'length\'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5242</span><span style="font-weight: bold">}</span>\n<span style="font-weight: bold">}</span>\n</pre>\n\n\n\n### Advantages\n\n* Detailed type hints for autocompleting queries as you type\n* Autocompletion for return fields\n* Documentation for each field\n* Automatic results parsing, for `json`, `tsv`, `list`, and `xml`\n* Built-in pagination, so you don\'t have to handle any of that yourself!\n* Most of the API is automatically generated, ensuring very rapid updates whenever the API changes\n* Thoroughly tested, with 41 unit tests and counting!\n\n## Usage\n\n### Installation\n\nIf you\'re using poetry:\n```bash\npoetry add unipressed\n```\n\nOtherwise:\n```bash\npip install unipressed\n```\n\n### Dataset Clients\n\nThe `unipressed` module exports a client object for each UniProt dataset:\n\n```python\nfrom unipressed import UniprotkbClient, UniparcClient\n```\n\nWith one of these clients, you can search the dataset:\n\n```python\nrecords = UniprotkbClient.search({\n    "length": (5000, 6000)\n}).each_record()\n\n# Show the first record\nnext(records)\n```\n\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">\n<span style="font-weight: bold">{</span>\n    <span style="color: #008000; text-decoration-color: #008000">\'entryType\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'UniProtKB reviewed (Swiss-Prot)\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'primaryAccession\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'Q96RW7\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'secondaryAccessions\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'uniProtkbId\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'HMCN1_HUMAN\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'entryAudit\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'annotationScore\'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'organism\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'proteinExistence\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'1: Evidence at protein level\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'proteinDescription\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'genes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'comments\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'features\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'keywords\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'references\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'uniProtKBCrossReferences\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'sequence\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'extraAttributes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>\n<span style="font-weight: bold">}</span>\n</pre>\n\n\n\nYou can request a single record by ID:\n\n```python\nUniprotkbClient.fetch_one("Q96RW7")\n```\n\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">\n<span style="font-weight: bold">{</span>\n    <span style="color: #008000; text-decoration-color: #008000">\'entryType\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'UniProtKB reviewed (Swiss-Prot)\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'primaryAccession\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'Q96RW7\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'secondaryAccessions\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'uniProtkbId\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'HMCN1_HUMAN\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'entryAudit\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'annotationScore\'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'organism\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'proteinExistence\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'1: Evidence at protein level\'</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'proteinDescription\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'genes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'comments\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'features\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'keywords\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'references\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'uniProtKBCrossReferences\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'sequence\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n    <span style="color: #008000; text-decoration-color: #008000">\'extraAttributes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>\n<span style="font-weight: bold">}</span>\n</pre>\n\n\n\nYou can also request multiple records:\n\n```python\nUniprotkbClient.fetch_many(["A0A0C5B5G6", "A0A1B0GTW7"])\n```\n\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">\n<span style="font-weight: bold">[</span>\n    <span style="font-weight: bold">{</span>\n        <span style="color: #008000; text-decoration-color: #008000">\'entryType\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'UniProtKB reviewed (Swiss-Prot)\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'primaryAccession\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'A0A0C5B5G6\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'uniProtkbId\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'MOTSC_HUMAN\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'entryAudit\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'annotationScore\'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'organism\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'proteinExistence\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'1: Evidence at protein level\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'proteinDescription\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'genes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'comments\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'features\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'geneLocations\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'keywords\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'references\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'uniProtKBCrossReferences\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'sequence\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'extraAttributes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>\n    <span style="font-weight: bold">}</span>,\n    <span style="font-weight: bold">{</span>\n        <span style="color: #008000; text-decoration-color: #008000">\'entryType\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'UniProtKB reviewed (Swiss-Prot)\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'primaryAccession\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'A0A1B0GTW7\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'secondaryAccessions\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'uniProtkbId\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'CIROP_HUMAN\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'entryAudit\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'annotationScore\'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'organism\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'proteinExistence\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'1: Evidence at protein level\'</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'proteinDescription\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'genes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'comments\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'features\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'keywords\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'references\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'uniProtKBCrossReferences\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'sequence\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,\n        <span style="color: #008000; text-decoration-color: #008000">\'extraAttributes\'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>\n    <span style="font-weight: bold">}</span>\n<span style="font-weight: bold">]</span>\n</pre>\n\n\n\n### ID Mapping\n\nUnipressed also provides one other unique client, which is designed for mapping identifiers. You provide the source and destination database (both of which will autocomplete in VS Code), and a list of identifiers for the source database.\n\n```python\nfrom unipressed import IdMappingClient\nrequest = IdMappingClient.submit(\n    source="UniProtKB_AC-ID", dest="Gene_Name", ids={"A1L190", "A0JP26", "A0PK11"}\n)\nlist(request.each_result())\n```\n\n\n<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,\'DejaVu Sans Mono\',consolas,\'Courier New\',monospace">\n<span style="font-weight: bold">[</span>\n    <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">\'from\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'A1L190\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'to\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'SYCE3\'</span><span style="font-weight: bold">}</span>,\n    <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">\'from\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'A0PK11\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'to\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'CLRN2\'</span><span style="font-weight: bold">}</span>,\n    <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">\'from\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'A0JP26\'</span>, <span style="color: #008000; text-decoration-color: #008000">\'to\'</span>: <span style="color: #008000; text-decoration-color: #008000">\'POTEB3\'</span><span style="font-weight: bold">}</span>\n<span style="font-weight: bold">]</span>\n</pre>\n\n\n\nNote that, if you submit a large number of IDs, you might need to add a `sleep()` call between submitting the request and retrieving the results.\n\n### Query Syntax\n\nThe query syntax refers to the values you pass in to the `query` argument of the `search()` method.\n\nIn general, you can\'t go wrong by following the type hints.\nI strongly recommend using something like [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) for [Visual Studio Code](https://code.visualstudio.com/), which will provide automatic completions and warn you when you have used the wrong syntax.\n\nIf you already know how to use the Uniprot query language, you can always just input your queries as strings:\n\n```python\nUniprotkbClient.search(query="(gene:BRCA*) AND (organism_id:10090)")\n```\n\nHowever, if you want some built-in query validation and code completion using Python\'s type system, then you can instead use a dictionary.\nThe simplest query is a dictionary with a single key: \n\n```python\nUniprotkbClient.search(query={"family": "kinase"})\n```\n\nYou can compile more complex queries using the `and_`, `or_` and `not_` keys.\nThese first two operators take a list of query dictionaries: \n\n```python\nUniprotkbClient.search(query={\n    "and_": [\n        {"family": "kinase"},\n        {"organism_id": "9606"},\n    ]\n})\n```\n\nMost "leaf" nodes of the query tree (ie those that aren\'t operators like `and_`) are strings, integers or floats, which you input as normal Python literals as you can see above.\nFor string fields, you also have access to wildcards, namely the `*` character. \nFor example, if you want every human protein belonging to a gene whose name starts with `PRO`, you could use:\n\n```python\nUniprotkbClient.search(query={\n    "and_": [\n        {"gene": "PRO*"},\n        {"organism_id": "9606"},\n    ]\n})\n```\n\nA few query fields are *ranges*, which you input using a tuple with two elements, indicating the start and end of the range.\nIf you use the literal `"*"` then you can leave the range open at one end. \nFor example, this query returns any protein that is in the range $[5000, \\infty)$\n\n```python\nUniprotkbClient.search(query={"length": (5000, "*")})\n```\n\nFinally, a few query fields take dates.\nThese you input as a Python `datetime.date` object.\nFor example, to find proteins added to UniProt since July 2022, we would do:\n\n```python\nfrom datetime import date\n\nUniprotkbClient.search(query={"date_created": (date(2022, 7, 1), "*")})\n```\n\n### Use with Visual Studio Code\nTo get VS Code to offer suggestions, press the `Trigger Suggest` shortcut which is usually bound to `Ctrl + Space`.\nIn particular, code completion generally won\'t work *until* you open a string literal using a quotation mark.\n\nSecondly, to get live access to the documentation, you can either use the `Show Hover` shortcut, which is usually bound to `Ctrl + K, Ctrl + I`, or you can install the [`docs-view`](https://marketplace.visualstudio.com/items?itemName=bierner.docs-view) extension, which lets you view the docstrings in the sidebar without interfering with your code.\n',
-    'author': 'Michael Milton',
-    'author_email': 'michael.r.milton@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://multimeric.github.io/Unipressed',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+# Unipressed
 
+**Please visit the [project website](https://multimeric.github.io/Unipressed/) for more comprehensive documentation.**
+
+## Introduction
+
+Unipressed (Uniprot REST) is an API client for the protein database [Uniprot](https://www.uniprot.org/).
+It provides thoroughly typed and documented code to ensure your use of the library is easy, fast, and correct!
+
+### Example
+Let's say we're interested in very long proteins that are encoded within a chloroplast, in any organism:
+
+```python
+from unipressed import UniprotkbClient
+
+for record in UniprotkbClient.search(
+    query={
+        "and_": [
+            {"organelle": "chloroplast"},
+            {"length": (5000, "*")}
+        ]
+    },
+    fields=["length", "gene_names"]
+).each_record():
+    display(record)
+```
+
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">
+<span style="font-weight: bold">{</span>
+    <span style="color: #008000; text-decoration-color: #008000">'primaryAccession'</span>: <span style="color: #008000; text-decoration-color: #008000">'A0A088CK67'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'genes'</span>: <span style="font-weight: bold">[</span>
+        <span style="font-weight: bold">{</span>
+            <span style="color: #008000; text-decoration-color: #008000">'geneName'</span>: <span style="font-weight: bold">{</span>
+                <span style="color: #008000; text-decoration-color: #008000">'evidences'</span>: <span style="font-weight: bold">[{</span><span style="color: #008000; text-decoration-color: #008000">'evidenceCode'</span>: <span style="color: #008000; text-decoration-color: #008000">'ECO:0000313'</span>, <span style="color: #008000; text-decoration-color: #008000">'source'</span>: <span style="color: #008000; text-decoration-color: #008000">'EMBL'</span>, <span style="color: #008000; text-decoration-color: #008000">'id'</span>: <span style="color: #008000; text-decoration-color: #008000">'AID67672.1'</span><span style="font-weight: bold">}]</span>,
+                <span style="color: #008000; text-decoration-color: #008000">'value'</span>: <span style="color: #008000; text-decoration-color: #008000">'ftsH'</span>
+            <span style="font-weight: bold">}</span>
+        <span style="font-weight: bold">}</span>
+    <span style="font-weight: bold">]</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'sequence'</span>: <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">'length'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5242</span><span style="font-weight: bold">}</span>
+<span style="font-weight: bold">}</span>
+</pre>
+
+
+
+### Advantages
+
+* Detailed type hints for autocompleting queries as you type
+* Autocompletion for return fields
+* Documentation for each field
+* Automatic results parsing, for `json`, `tsv`, `list`, and `xml`
+* Built-in pagination, so you don't have to handle any of that yourself!
+* Most of the API is automatically generated, ensuring very rapid updates whenever the API changes
+* Thoroughly tested, with 41 unit tests and counting!
+
+## Usage
+
+### Installation
+
+If you're using poetry:
+```bash
+poetry add unipressed
+```
+
+Otherwise:
+```bash
+pip install unipressed
+```
+
+### Dataset Clients
+
+The `unipressed` module exports a client object for each UniProt dataset:
+
+```python
+from unipressed import UniprotkbClient, UniparcClient
+```
+
+With one of these clients, you can search the dataset:
+
+```python
+records = UniprotkbClient.search({
+    "length": (5000, 6000)
+}).each_record()
+
+# Show the first record
+next(records)
+```
+
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">
+<span style="font-weight: bold">{</span>
+    <span style="color: #008000; text-decoration-color: #008000">'entryType'</span>: <span style="color: #008000; text-decoration-color: #008000">'UniProtKB reviewed (Swiss-Prot)'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'primaryAccession'</span>: <span style="color: #008000; text-decoration-color: #008000">'Q96RW7'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'secondaryAccessions'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'uniProtkbId'</span>: <span style="color: #008000; text-decoration-color: #008000">'HMCN1_HUMAN'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'entryAudit'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'annotationScore'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'organism'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'proteinExistence'</span>: <span style="color: #008000; text-decoration-color: #008000">'1: Evidence at protein level'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'proteinDescription'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'genes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'comments'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'features'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'keywords'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'references'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'uniProtKBCrossReferences'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'sequence'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'extraAttributes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>
+<span style="font-weight: bold">}</span>
+</pre>
+
+
+
+You can request a single record by ID:
+
+```python
+UniprotkbClient.fetch_one("Q96RW7")
+```
+
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">
+<span style="font-weight: bold">{</span>
+    <span style="color: #008000; text-decoration-color: #008000">'entryType'</span>: <span style="color: #008000; text-decoration-color: #008000">'UniProtKB reviewed (Swiss-Prot)'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'primaryAccession'</span>: <span style="color: #008000; text-decoration-color: #008000">'Q96RW7'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'secondaryAccessions'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'uniProtkbId'</span>: <span style="color: #008000; text-decoration-color: #008000">'HMCN1_HUMAN'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'entryAudit'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'annotationScore'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'organism'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'proteinExistence'</span>: <span style="color: #008000; text-decoration-color: #008000">'1: Evidence at protein level'</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'proteinDescription'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'genes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'comments'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'features'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'keywords'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'references'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'uniProtKBCrossReferences'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'sequence'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+    <span style="color: #008000; text-decoration-color: #008000">'extraAttributes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>
+<span style="font-weight: bold">}</span>
+</pre>
+
+
+
+You can also request multiple records:
+
+```python
+UniprotkbClient.fetch_many(["A0A0C5B5G6", "A0A1B0GTW7"])
+```
+
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">
+<span style="font-weight: bold">[</span>
+    <span style="font-weight: bold">{</span>
+        <span style="color: #008000; text-decoration-color: #008000">'entryType'</span>: <span style="color: #008000; text-decoration-color: #008000">'UniProtKB reviewed (Swiss-Prot)'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'primaryAccession'</span>: <span style="color: #008000; text-decoration-color: #008000">'A0A0C5B5G6'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'uniProtkbId'</span>: <span style="color: #008000; text-decoration-color: #008000">'MOTSC_HUMAN'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'entryAudit'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'annotationScore'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'organism'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'proteinExistence'</span>: <span style="color: #008000; text-decoration-color: #008000">'1: Evidence at protein level'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'proteinDescription'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'genes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'comments'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'features'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'geneLocations'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'keywords'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'references'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'uniProtKBCrossReferences'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'sequence'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'extraAttributes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>
+    <span style="font-weight: bold">}</span>,
+    <span style="font-weight: bold">{</span>
+        <span style="color: #008000; text-decoration-color: #008000">'entryType'</span>: <span style="color: #008000; text-decoration-color: #008000">'UniProtKB reviewed (Swiss-Prot)'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'primaryAccession'</span>: <span style="color: #008000; text-decoration-color: #008000">'A0A1B0GTW7'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'secondaryAccessions'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'uniProtkbId'</span>: <span style="color: #008000; text-decoration-color: #008000">'CIROP_HUMAN'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'entryAudit'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'annotationScore'</span>: <span style="color: #008080; text-decoration-color: #008080; font-weight: bold">5.0</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'organism'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'proteinExistence'</span>: <span style="color: #008000; text-decoration-color: #008000">'1: Evidence at protein level'</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'proteinDescription'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'genes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'comments'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'features'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'keywords'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'references'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'uniProtKBCrossReferences'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'sequence'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>,
+        <span style="color: #008000; text-decoration-color: #008000">'extraAttributes'</span>: <span style="color: #808000; text-decoration-color: #808000">...</span>
+    <span style="font-weight: bold">}</span>
+<span style="font-weight: bold">]</span>
+</pre>
+
+
+
+### ID Mapping
+
+Unipressed also provides one other unique client, which is designed for mapping identifiers. You provide the source and destination database (both of which will autocomplete in VS Code), and a list of identifiers for the source database.
+
+```python
+from unipressed import IdMappingClient
+request = IdMappingClient.submit(
+    source="UniProtKB_AC-ID", dest="Gene_Name", ids={"A1L190", "A0JP26", "A0PK11"}
+)
+list(request.each_result())
+```
+
+
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace">
+<span style="font-weight: bold">[</span>
+    <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">'from'</span>: <span style="color: #008000; text-decoration-color: #008000">'A1L190'</span>, <span style="color: #008000; text-decoration-color: #008000">'to'</span>: <span style="color: #008000; text-decoration-color: #008000">'SYCE3'</span><span style="font-weight: bold">}</span>,
+    <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">'from'</span>: <span style="color: #008000; text-decoration-color: #008000">'A0PK11'</span>, <span style="color: #008000; text-decoration-color: #008000">'to'</span>: <span style="color: #008000; text-decoration-color: #008000">'CLRN2'</span><span style="font-weight: bold">}</span>,
+    <span style="font-weight: bold">{</span><span style="color: #008000; text-decoration-color: #008000">'from'</span>: <span style="color: #008000; text-decoration-color: #008000">'A0JP26'</span>, <span style="color: #008000; text-decoration-color: #008000">'to'</span>: <span style="color: #008000; text-decoration-color: #008000">'POTEB3'</span><span style="font-weight: bold">}</span>
+<span style="font-weight: bold">]</span>
+</pre>
+
+
+
+Note that, if you submit a large number of IDs, you might need to add a `sleep()` call between submitting the request and retrieving the results.
+
+### Query Syntax
+
+The query syntax refers to the values you pass in to the `query` argument of the `search()` method.
+
+In general, you can't go wrong by following the type hints.
+I strongly recommend using something like [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) for [Visual Studio Code](https://code.visualstudio.com/), which will provide automatic completions and warn you when you have used the wrong syntax.
+
+If you already know how to use the Uniprot query language, you can always just input your queries as strings:
+
+```python
+UniprotkbClient.search(query="(gene:BRCA*) AND (organism_id:10090)")
+```
+
+However, if you want some built-in query validation and code completion using Python's type system, then you can instead use a dictionary.
+The simplest query is a dictionary with a single key: 
+
+```python
+UniprotkbClient.search(query={"family": "kinase"})
+```
+
+You can compile more complex queries using the `and_`, `or_` and `not_` keys.
+These first two operators take a list of query dictionaries: 
+
+```python
+UniprotkbClient.search(query={
+    "and_": [
+        {"family": "kinase"},
+        {"organism_id": "9606"},
+    ]
+})
+```
+
+Most "leaf" nodes of the query tree (ie those that aren't operators like `and_`) are strings, integers or floats, which you input as normal Python literals as you can see above.
+For string fields, you also have access to wildcards, namely the `*` character. 
+For example, if you want every human protein belonging to a gene whose name starts with `PRO`, you could use:
+
+```python
+UniprotkbClient.search(query={
+    "and_": [
+        {"gene": "PRO*"},
+        {"organism_id": "9606"},
+    ]
+})
+```
+
+A few query fields are *ranges*, which you input using a tuple with two elements, indicating the start and end of the range.
+If you use the literal `"*"` then you can leave the range open at one end. 
+For example, this query returns any protein that is in the range $[5000, \infty)$
+
+```python
+UniprotkbClient.search(query={"length": (5000, "*")})
+```
+
+Finally, a few query fields take dates.
+These you input as a Python `datetime.date` object.
+For example, to find proteins added to UniProt since July 2022, we would do:
+
+```python
+from datetime import date
+
+UniprotkbClient.search(query={"date_created": (date(2022, 7, 1), "*")})
+```
+
+### Use with Visual Studio Code
+To get VS Code to offer suggestions, press the `Trigger Suggest` shortcut which is usually bound to `Ctrl + Space`.
+In particular, code completion generally won't work *until* you open a string literal using a quotation mark.
+
+Secondly, to get live access to the documentation, you can either use the `Show Hover` shortcut, which is usually bound to `Ctrl + K, Ctrl + I`, or you can install the [`docs-view`](https://marketplace.visualstudio.com/items?itemName=bierner.docs-view) extension, which lets you view the docstrings in the sidebar without interfering with your code.
 
-setup(**setup_kwargs)
```

