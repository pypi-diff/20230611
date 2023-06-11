# Comparing `tmp/ingestor-0.0.2-py3-none-any.whl.zip` & `tmp/ingestor-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 8687 bytes, number of entries: 24
+Zip file size: 8929 bytes, number of entries: 24
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 ingestor/.python-version
+-rw-r--r--  2.0 unx      210 b- defN 80-Jan-01 00:00 ingestor/Dockerfile
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ingestor/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ingestor/bq/__init__.py
--rw-r--r--  2.0 unx      882 b- defN 80-Jan-01 00:00 ingestor/bq/load.py
--rw-r--r--  2.0 unx      417 b- defN 80-Jan-01 00:00 ingestor/bq/options.py
+-rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 ingestor/bq/load.py
+-rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 ingestor/bq/options.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ingestor/bq/schemas/__init__.py
 -rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 ingestor/bq/schemas/author.json
 -rw-r--r--  2.0 unx      375 b- defN 80-Jan-01 00:00 ingestor/bq/schemas/providers.py
--rw-r--r--  2.0 unx      147 b- defN 80-Jan-01 00:00 ingestor/cli.py
+-rw-r--r--  2.0 unx      433 b- defN 80-Jan-01 00:00 ingestor/cli.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 ingestor/common_options.py
--rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 ingestor/entrypoint.py
 -rw-r--r--  2.0 unx      483 b- defN 80-Jan-01 00:00 ingestor/exec.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ingestor/gcs/__init__.py
--rw-r--r--  2.0 unx     1705 b- defN 80-Jan-01 00:00 ingestor/gcs/ingestion.py
--rw-r--r--  2.0 unx     1102 b- defN 80-Jan-01 00:00 ingestor/gcs/options.py
+-rw-r--r--  2.0 unx     1723 b- defN 80-Jan-01 00:00 ingestor/gcs/ingestion.py
+-rw-r--r--  2.0 unx     1111 b- defN 80-Jan-01 00:00 ingestor/gcs/options.py
 -rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 ingestor/gcs/schemas/__init__.py
 -rw-r--r--  2.0 unx      489 b- defN 80-Jan-01 00:00 ingestor/gcs/schemas/author.avsc
 -rw-r--r--  2.0 unx      400 b- defN 80-Jan-01 00:00 ingestor/gcs/schemas/providers.py
--rw-r--r--  2.0 unx     3077 b- defN 80-Jan-01 00:00 ingestor/ingest.py
--rw-r--r--  2.0 unx     1204 b- defN 80-Jan-01 00:00 ingestor/load.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ingestor-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 ingestor-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      685 b- defN 80-Jan-01 00:00 ingestor-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     1900 b- defN 16-Jan-01 00:00 ingestor-0.0.2.dist-info/RECORD
-24 files, 13996 bytes uncompressed, 5603 bytes compressed:  60.0%
+-rw-r--r--  2.0 unx     3095 b- defN 80-Jan-01 00:00 ingestor/ingest.py
+-rw-r--r--  2.0 unx     1222 b- defN 80-Jan-01 00:00 ingestor/load.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ingestor-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 ingestor-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx      685 b- defN 80-Jan-01 00:00 ingestor-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx     1898 b- defN 16-Jan-01 00:00 ingestor-0.0.3.dist-info/RECORD
+24 files, 14521 bytes uncompressed, 5851 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: ingestor/.python-version
 Comment: 
 
+Filename: ingestor/Dockerfile
+Comment: 
+
 Filename: ingestor/__init__.py
 Comment: 
 
 Filename: ingestor/bq/__init__.py
 Comment: 
 
 Filename: ingestor/bq/load.py
@@ -24,17 +27,14 @@
 
 Filename: ingestor/cli.py
 Comment: 
 
 Filename: ingestor/common_options.py
 Comment: 
 
-Filename: ingestor/entrypoint.py
-Comment: 
-
 Filename: ingestor/exec.py
 Comment: 
 
 Filename: ingestor/gcs/__init__.py
 Comment: 
 
 Filename: ingestor/gcs/ingestion.py
@@ -54,20 +54,20 @@
 
 Filename: ingestor/ingest.py
 Comment: 
 
 Filename: ingestor/load.py
 Comment: 
 
-Filename: ingestor-0.0.2.dist-info/WHEEL
+Filename: ingestor-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: ingestor-0.0.2.dist-info/entry_points.txt
+Filename: ingestor-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ingestor-0.0.2.dist-info/METADATA
+Filename: ingestor-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: ingestor-0.0.2.dist-info/RECORD
+Filename: ingestor-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ingestor/bq/load.py

```diff
@@ -1,12 +1,12 @@
 import apache_beam as beam
 from apache_beam.io import ReadFromAvro, WriteToBigQuery, BigQueryDisposition
 
-from bq.schemas.providers import get_schema_by_table
-from bq.options import LoadOptions
+from ingestor.bq.schemas.providers import get_schema_by_table
+from ingestor.bq.options import LoadOptions
 
 
 def execute_pipeline(options: LoadOptions) -> None:
     schema = get_schema_by_table(options.table)
     file_pattern = f"gs://{options.ingestion_bucket}/**/*.arvo"
     with beam.Pipeline(options=options) as p:
         records = p | "Read files" >> ReadFromAvro(file_pattern=file_pattern)
```

## ingestor/bq/options.py

```diff
@@ -1,10 +1,10 @@
 from apache_beam.options.pipeline_options import _BeamArgumentParser
 
-from common_options import CommonOptions
+from ingestor.common_options import CommonOptions
 
 
 class LoadOptions(CommonOptions):
     @classmethod
     def _add_argparse_args(cls, parser: _BeamArgumentParser) -> None:
         parser.add_argument("--bq_project", required=True)
         parser.add_argument("--bq_dataset", required=True)
```

## ingestor/cli.py

```diff
@@ -1,13 +1,25 @@
+import pathlib
+import sys
+
 import click
 
-from ingest import ingest
-from load import load
+try:
+    from ingestor.ingest import ingest
+    from ingestor.load import load
+except (ImportError, ModuleNotFoundError):
+    sys.path.insert(0, pathlib.Path(__file__).parent.parent.as_posix())
+    from ingestor.ingest import ingest
+    from ingestor.load import load
 
 
 @click.group()
 def cli():
     pass
 
 
 cli.add_command(ingest)
 cli.add_command(load)
+
+
+if __name__ == "__main__":
+    cli()
```

## ingestor/gcs/ingestion.py

```diff
@@ -1,13 +1,13 @@
 import apache_beam as beam
 from apache_beam.io.avroio import WriteToAvro
 from beam_nuggets.io import relational_db
 
-from gcs.options import IngestionOptions
-from gcs.schemas.providers import get_schema_by_table
+from ingestor.gcs.options import IngestionOptions
+from ingestor.gcs.schemas.providers import get_schema_by_table
 
 
 def parse_record(record) -> dict:
     record["registration_date"] = record["registration_date"].timestamp()
     return record
```

## ingestor/gcs/options.py

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 from apache_beam.options.pipeline_options import _BeamArgumentParser
 
-from common_options import CommonOptions
+from ingestor.common_options import CommonOptions
 
 
 class IngestionOptions(CommonOptions):
 
     @classmethod
     def _add_argparse_args(cls, parser: _BeamArgumentParser) -> None:
         parser.add_argument("--host", required=True)
```

## ingestor/ingest.py

```diff
@@ -1,11 +1,11 @@
 import click
 
-from gcs.ingestion import execute_pipeline
-from gcs.options import IngestionOptions
+from ingestor.gcs.ingestion import execute_pipeline
+from ingestor.gcs.options import IngestionOptions
 
 
 @click.command("ingest")
 @click.option(
     "--host",
     default="localhost",
     help="The host of the database to connect to."
```

## ingestor/load.py

```diff
@@ -1,11 +1,11 @@
 import click
 
-from bq.load import execute_pipeline
-from bq.options import LoadOptions
+from ingestor.bq.load import execute_pipeline
+from ingestor.bq.options import LoadOptions
 
 
 @click.command("load")
 @click.option(
     "--bq_project",
     required=True,
     help="The name of the BigQuery project to connect to."
```

## Comparing `ingestor-0.0.2.dist-info/METADATA` & `ingestor-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingestor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Apache Beam pipeline that ingests data from a PostgreSQL and writes it to GCS.
 Author: Roman Dryndik
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `ingestor-0.0.2.dist-info/RECORD` & `ingestor-0.0.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ingestor/.python-version,sha256=x5OLXAEqiFrMYtwOBGt5evOSA58NiqmMOpuLLL2psp4,5
+ingestor/Dockerfile,sha256=3HgRewOqKiuMaMk-mPkJhBJdP_RQ1_NOiPcKkH1KhUU,210
 ingestor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ingestor/bq/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ingestor/bq/load.py,sha256=e2W_y-dABfPOligDg3V96YP6TiDXllDE1IHvgiAa6Sg,882
-ingestor/bq/options.py,sha256=NDaj4XS9co2E-stH3FwDnkdVaW-EcTKgl6hxpx7EsAw,417
+ingestor/bq/load.py,sha256=sWgoHfVPZs-xRhaxSbWf3USQP3FxgLNzqqzqOrPOvic,900
+ingestor/bq/options.py,sha256=J1u9CScUNXABE1y1UmDgj14cnxAa37q9EKGk_XbH-T8,426
 ingestor/bq/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ingestor/bq/schemas/author.json,sha256=Q88cRLryXSDhCJNZf7MhgIsmu0V5spXcHdSllpg5ZSk,551
 ingestor/bq/schemas/providers.py,sha256=Z0b3ZE6VXe3eumdU8uWfHphKXEZ_VTiVJnnk4FtvfHY,375
-ingestor/cli.py,sha256=-8m5CfcmDbInrJSmG8g7lh2kZNwvOUxgxbhmkRFL99c,147
+ingestor/cli.py,sha256=0F0hmUDcZzEBIDq-KQ0m6-PeE-OTrXhbdf3cZmIEsbA,433
 ingestor/common_options.py,sha256=1VZ_k-JNr3keXbFKPcIJJS9biPPI1wFLOOdQC7QQlCs,332
-ingestor/entrypoint.py,sha256=h8RKC_jT3VUtAlG-Wq1BF-yzoeOvdh8_8iPcnsUkHk4,59
 ingestor/exec.py,sha256=HbCvrYAO2nswdJpgAWU6y6wNvKh9mfzWSenDztFyyu8,483
 ingestor/gcs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ingestor/gcs/ingestion.py,sha256=yQeA-200TTPLs0UwFvscSUZRhEyMhomDXE-fwN9kSYw,1705
-ingestor/gcs/options.py,sha256=M4lmwEuiWk0Jk0NbKvoQcstWbxZd6aAE8BsXqRIgjU4,1102
+ingestor/gcs/ingestion.py,sha256=Y00oRFBWG4IIU2WFp-317i5dcjxfbZ82COjdGdm31nI,1723
+ingestor/gcs/options.py,sha256=_sPw5ScvJCCWPwoN0DthqYogVjIV0yNB4h0A3nFnvHU,1111
 ingestor/gcs/schemas/__init__.py,sha256=I3spXcDrDoLqKpGiMsyVUG-O_4wNV_HNysry4ZEtjIs,41
 ingestor/gcs/schemas/author.avsc,sha256=_M4BjOkVs_I385mRtvFX4uyk760qR_Rec8Pbls0Vxqs,489
 ingestor/gcs/schemas/providers.py,sha256=LgX4WXA73rMpXOb6mzaOZMsfC3DOjPKXJ0N-oEI2k5k,400
-ingestor/ingest.py,sha256=LNI9eT7SoAfU0DZ-AiNAZcyewqQcpy-Qiar_61_Kfck,3077
-ingestor/load.py,sha256=FhpGE7sPj309LEu0fzT5TAsJJ9vQ83mduuwUsjCdY3E,1204
-ingestor-0.0.2.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-ingestor-0.0.2.dist-info/entry_points.txt,sha256=x4Wv0eyENPFVFNaFrt9T-ROiA7LiLBYzFuj640tlwOE,54
-ingestor-0.0.2.dist-info/METADATA,sha256=GwzTX04fBh_o2ULxZyHtZcsYiMUhdDA29B_A6F7LZCA,685
-ingestor-0.0.2.dist-info/RECORD,,
+ingestor/ingest.py,sha256=8pJLmZqdy6N46tN34PjWeqTQ8_0Tw8dfWyRxZRpv0TY,3095
+ingestor/load.py,sha256=JlEDEuwzFv8kngzDWxQfRja3c8ovLs1PsLPNYY1iNug,1222
+ingestor-0.0.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+ingestor-0.0.3.dist-info/entry_points.txt,sha256=x4Wv0eyENPFVFNaFrt9T-ROiA7LiLBYzFuj640tlwOE,54
+ingestor-0.0.3.dist-info/METADATA,sha256=pZKsmMugCUQ2UqBhqEnjooc9szkRx7JI9cpzcU0Xl5s,685
+ingestor-0.0.3.dist-info/RECORD,,
```

