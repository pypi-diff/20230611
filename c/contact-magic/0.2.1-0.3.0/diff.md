# Comparing `tmp/contact_magic-0.2.1.tar.gz` & `tmp/contact_magic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.2.1.tar", max compression
+gzip compressed data, was "contact_magic-0.3.0.tar", max compression
```

## Comparing `contact_magic-0.2.1.tar` & `contact_magic-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     4420 2023-06-09 17:09:31.138259 contact_magic-0.2.1/README.md
--rw-r--r--   0        0        0      209 2023-06-09 23:45:46.576485 contact_magic-0.2.1/contact_magic/__init__.py
--rw-r--r--   0        0        0       50 2023-06-09 23:24:56.292562 contact_magic-0.2.1/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     4667 2023-06-09 23:40:08.296999 contact_magic-0.2.1/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-09 23:24:56.315289 contact_magic-0.2.1/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.2.1/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2151 2023-06-09 23:24:56.298589 contact_magic-0.2.1/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1328 2023-06-09 23:24:56.296537 contact_magic-0.2.1/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.2.1/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.2.1/contact_magic/logger.py
--rw-r--r--   0        0        0    11271 2023-06-09 23:24:56.313283 contact_magic-0.2.1/contact_magic/models.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.2.1/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1593 2023-06-09 23:26:11.761609 contact_magic-0.2.1/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.2.1/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-09 23:26:11.764227 contact_magic-0.2.1/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-09 23:26:11.765943 contact_magic-0.2.1/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     2773 2023-06-09 12:44:06.238751 contact_magic-0.2.1/contact_magic/utils.py
--rw-r--r--   0        0        0     1731 2023-06-09 23:49:40.669901 contact_magic-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 contact_magic-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.0/README.md
+-rw-r--r--   0        0        0      210 2023-06-11 08:34:28.960916 contact_magic-0.3.0/contact_magic/__init__.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:28:29.820843 contact_magic-0.3.0/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.0/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     4667 2023-06-10 17:47:50.154037 contact_magic-0.3.0/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-10 00:10:37.387140 contact_magic-0.3.0/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.0/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2151 2023-06-10 00:10:37.388687 contact_magic-0.3.0/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1471 2023-06-10 14:15:09.990381 contact_magic-0.3.0/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.0/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.0/contact_magic/logger.py
+-rw-r--r--   0        0        0    11917 2023-06-10 22:11:15.895054 contact_magic-0.3.0/contact_magic/models.py
+-rw-r--r--   0        0        0     2991 2023-06-10 22:11:15.757144 contact_magic-0.3.0/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.0/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.0/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.0/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-10 00:10:37.399377 contact_magic-0.3.0/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.0/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.0/contact_magic/utils.py
+-rw-r--r--   0        0        0     1710 2023-06-11 08:34:28.956577 contact_magic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.0/PKG-INFO
```

### Comparing `contact_magic-0.2.1/README.md` & `contact_magic-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,26 +38,27 @@
 MASTERSHEET_URL=''
 GOOGLE_PROJECT_ID=''
 GOOGLE_PRIVATE_KEY_ID=''
 GOOGLE_PRIVATE_KEY=''
 GOOGLE_CLIENT_ID=''
 GOOGLE_CLIENT_EMAIL=''
 TIMEZONE="America/New_York"
-ALLOWED_SCRAPER_NAMES='get-case-study, get-company-achievement, get-company-description, get-company-announcement, FALLBACK'
+# list and dict are parsed as JSON.
+ALLOWED_SCRAPER_NAMES='["get-case-study", "get-company-achievement", "get-company-description", "get-company-announcement", "FALLBACK", "search-google"]'
 MAX_WORKERS='5'  # Number of concurrent workers to process. 5-10 is likely enough.
 ```
 
 If you are not using the agency workflows and just want to use the underlying PersonalizationSetttings objects you only
 need to set the following environment variables.
 
 ```python
 COPYFACTORY_API_KEY=''
 SALES_SCRAPERS_API_KEY=''
 # Optional since has default value
-ALLOWED_SCRAPER_NAMES='get-case-study, get-company-achievement, get-company-description, get-company-announcement, FALLBACK'
+ALLOWED_SCRAPER_NAMES='["get-case-study", "get-company-achievement", "get-company-description", "get-company-announcement", "FALLBACK", "search-google"]'
 # Optional since has default value
 MAX_WORKERS='5'
 ```
 
 ## Usage & Examples
 
 The core underlying model you will be using is 'PersonalizationSettings' which is responsible for understanding what
```

### Comparing `contact_magic-0.2.1/contact_magic/conf/settings.py` & `contact_magic-0.3.0/contact_magic/conf/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,12 +123,12 @@
         *_, validation_error = validate_model(self.__class__, self.__dict__)
         if validation_error:
             raise validation_error
         return self
 
     class Config:
         validate_assignment = True
-        env_file = '.env'
-        env_file_encoding = 'utf-8'
+        env_file = ".env"
+        env_file_encoding = "utf-8"
 
 
 SETTINGS = BaseConfig()
```

### Comparing `contact_magic-0.2.1/contact_magic/helpers.py` & `contact_magic-0.3.0/contact_magic/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gspread
 import numpy as np
 import pandas as pd
 
+from contact_magic.conf.settings import SETTINGS
 from contact_magic.integrations.sheets import get_worksheet_from_spreadsheet
 from contact_magic.models import PersonalizationSettings
-from contact_magic.conf.settings import SETTINGS
 
 
 def prepare_data_for_gsheet(
     df: pd.DataFrame, mapping: dict = None, enforced_columns: list = None
 ):
     """
     Converts a dataframe to a list of list to be passed to Gspread or Sheet alternative.
```

### Comparing `contact_magic-0.2.1/contact_magic/integrations/copyfactory.py` & `contact_magic-0.3.0/contact_magic/integrations/copyfactory.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 
 import httpx
 
-from contact_magic.utils import find_item
 from contact_magic.conf.settings import SETTINGS
+from contact_magic.utils import find_item
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 endpoint = "https://app.copyfactory.io/api/v2/generate/"
 
 headers = {"Accept": "application/json", "Authorization": SETTINGS.COPYFACTORY_API_KEY}
```

### Comparing `contact_magic-0.2.1/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.3.0/contact_magic/integrations/sales_scrapers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import logging
 
 import httpx
 
-from contact_magic.utils import fix_website
 from contact_magic.conf.settings import SETTINGS
+from contact_magic.logger import logger
+from contact_magic.utils import fix_website
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 base_url = "https://salesscrapers.dev/api/"
 
 headers = {"Accept": "application/json", "X-API-Key": SETTINGS.SALES_SCRAPERS_API_KEY}
 
@@ -20,14 +21,16 @@
     try:
         session = httpx.AsyncClient(timeout=120)
         retries = 0
         while retries < max_retries:
             res = await session.request(
                 method="get", url=url, headers=headers, params=data
             )
+            if res.status_code == 400:
+                logger.warning("proxy_error", message=res.text)
             if res.status_code == 200:
                 return res.json()
             if res.status_code == 422:
                 validation_errors = res.json().get("detail")
                 for error in validation_errors:
                     if error.get("type") == "value_error.url.scheme":
                         error_key = error.get("loc")[1]
```

### Comparing `contact_magic-0.2.1/contact_magic/integrations/sheets.py` & `contact_magic-0.3.0/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.2.1/contact_magic/models.py` & `contact_magic-0.3.0/contact_magic/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import asyncio
 import re
-from asyncio import QueueEmpty
+from datetime import datetime
 from typing import Any
+from uuid import UUID, uuid4
 
 import numpy as np
 import pandas as pd
 from pydantic import AnyUrl, BaseModel, Field, validator
 
+from contact_magic.asyncio import do_bulk
+from contact_magic.conf.settings import SETTINGS
 from contact_magic.integrations import (
     make_copyfactory_request,
     make_sales_scraper_request,
 )
 from contact_magic.logger import logger
-from contact_magic.utils import get_id_from_url, is_valid_premise_url, replace_keys
-from contact_magic.conf.settings import SETTINGS
+from contact_magic.preprocessors import processors
+from contact_magic.utils import (
+    find_item,
+    get_id_from_url,
+    is_valid_premise_url,
+    replace_keys,
+    replace_values,
+)
 
 
 class DataRow(BaseModel):
     """
     A class to hold a row of data and it's index number
     to sort by after. Converts set data to a dict.
     """
@@ -64,14 +73,21 @@
         default={},
     )
     copyfactory_mapping: dict = Field(
         description="A mapping where the keys are your column names and the "
         "values are the target variable name you want to send to Copyfactory.",
         default={},
     )
+    field_processors: dict = Field(
+        description="A list of fields to validate before "
+        "doing Copyfactory request."
+        "If any of the fields fail validation "
+        "Copyfactory will not be called.",
+        default={},
+    )
 
     @validator("premise_url")
     def validate_premise_url(cls, url):
         return f"{url}/" if not url.endswith("/") else url
 
     @validator("scraper_name")
     def validate_scraper_name(cls, value):
@@ -95,15 +111,15 @@
         Fills in the template with row data.
         either returns the filled in template or an empty string.
         """
         list_pot_keys = re.findall(r"\{(.*?)\}", self.fallback_template)
         copy_of_template = self.fallback_template
         filled_all = True
         for key in list_pot_keys:
-            value = row.data.get(key)
+            value = find_item(row.data, key)
             if not value:
                 filled_all = False
                 continue
             copy_of_template = copy_of_template.replace("{" + key + "}", value)
         return copy_of_template if filled_all else ""
 
     async def run_sales_scraper(self, row: DataRow, col_prefix: str, overwrite=False):
@@ -141,28 +157,51 @@
         if not self.premise_url and not self.premise_id:
             return row, False
         if self.premise_url and self.is_premise_url_valid:
             self.premise_id = get_id_from_url(self.premise_url)
         if not self.copyfactory_mapping and SETTINGS.COPYFACTORY_MAPPING:
             self.copyfactory_mapping = SETTINGS.COPYFACTORY_MAPPING
 
+        row, is_valid = self.run_processors(row)
+        if not is_valid:
+            return row, False
+
         data = (
             replace_keys(row.data, self.copyfactory_mapping)
             if self.copyfactory_mapping
             else row.data
         )
         if cf := await make_copyfactory_request(self.premise_id, variables=data):
             row.data[content_col_name] = cf["content"]
             source = row.data.get(
                 f"{content_col_name}__{self.scraper_name}__scraper_info", {}
             ).get("data_source", "-")
             row.data[source_col_name] = f"{self.scraper_name}, {source}"
             return row, True
         return row, False
 
+    def run_processors(self, row) -> tuple[DataRow, bool]:
+        """
+        Iterate over field processors and break if any don't satisfy.
+        """
+        if not self.field_processors:
+            return row, True
+        for key, processor in self.field_processors.items():
+            if item := find_item(row.data, key):
+                if validation_model := processors.get(
+                    processor.get("type", None), None
+                ):
+                    value, is_value_valid = validation_model(
+                        processor=processor, value=item
+                    ).process()
+                    if is_value_valid is False:
+                        return row, False
+                    row.data = replace_values(row.data, {key: value})
+        return row, True
+
     async def execute(
         self, row: DataRow, content_col_name: str, source_col_name: str
     ) -> tuple[DataRow, bool]:
         """
         Executes the scraper and extends the DataRow as it moves along to
         allow for exploding the DF with more
         datapoints from the scraping + personalization.
@@ -227,15 +266,18 @@
 
 
 class PersonalizationSettings(BaseModel):
     """
     A reference to a list of datapoints to generate for a given contact.
     """
 
+    name: str = ""
     datapoints: list[DataPoint]
+    uid: UUID = Field(default_factory=uuid4)
+    created: datetime = Field(default_factory=datetime.utcnow)
 
     @property
     def get_datapoint_column_names(self) -> list:
         """
         Returns a list of column names and a source field.
         """
         return [dp.col_name for dp in self.datapoints] + [
@@ -277,15 +319,15 @@
                     untouched_rows + self.process_data_rows(jobs),
                     key=lambda dp: dp.index,
                 )
             ],
             columns=df.columns,
         )
 
-    def process_data_rows(self, data: list[DataRow]):
+    def process_data_rows(self, data: list[DataRow]) -> list[DataRow]:
         """
         Process DataRows async.
         :param data:
         :return:
         """
         return asyncio.run(do_bulk([(self.build_row, {"row": row}) for row in data]))
 
@@ -294,42 +336,7 @@
         Iterate over all personalization datapoints and their
         allowed scrapers to extend a row of contact data
         with enrichment and personalized sentences.
         """
         for datapoint in self.datapoints:
             row = await datapoint.build_datapoint(row)
         return row
-
-
-async def do_bulk(ops: list, max_workers: int = SETTINGS.MAX_WORKERS) -> list[DataRow]:
-    """
-    Bulk operation
-    This function can be used to run bulk operations
-    using a limited number of concurrent requests.
-    """
-    results = [None for _ in range(len(ops))]
-
-    queue = asyncio.Queue()
-
-    for job in enumerate(ops):
-        await queue.put(job)
-
-    workers = [_worker(queue, results) for _ in range(max_workers)]
-
-    await asyncio.gather(*workers)
-
-    return results
-
-
-async def _worker(queue, results):
-    while True:
-        try:
-            index, op = queue.get_nowait()
-        except QueueEmpty:
-            break
-
-        try:
-            response = await op[0](**op[1])
-            results[index] = response
-        except Exception:
-            results[index] = None
-        queue.task_done()
```

### Comparing `contact_magic-0.2.1/contact_magic/scripts/agency.py` & `contact_magic-0.3.0/contact_magic/scripts/agency.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from typing import List
 
 import typer
 from rich import print
 from typing_extensions import Annotated
 
 from contact_magic.scripts.run_workflows import run_sheets
-from contact_magic.scripts.update_workflow_approval_metrics import update_rows_approved_and_remaining
+from contact_magic.scripts.update_workflow_approval_metrics import (
+    update_rows_approved_and_remaining,
+)
 
 app = typer.Typer()
 
 
 class ScriptOptions(Enum):
     run_sheets = "run_sheets"
     update_approved = "update_approved"
@@ -48,8 +50,7 @@
                 command()
                 print(f":robot_face: [green]Completed[/green] {name}")
             continue
         for task in tasks:
             print(f":robot_face: [green]Running[/green] {task.value}")
             commands[task.value]()
             print(f":robot_face: [green]Completed[/green] {task.value}")
-
```

### Comparing `contact_magic-0.2.1/contact_magic/scripts/run_workflows.py` & `contact_magic-0.3.0/contact_magic/scripts/run_workflows.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import datetime
 
 import gspread
 import numpy as np
 import pandas as pd
 import pytz
 
+from contact_magic.conf.settings import SETTINGS
 from contact_magic.helpers import (
     get_personalization_settings_from_sheet,
     prepare_data_for_gsheet,
     worksheet_to_dataframe,
 )
 from contact_magic.integrations.sheets import (
     bulk_update,
     get_spreadsheet_by_url,
     get_worksheet_from_spreadsheet,
     update_cell,
 )
-from contact_magic.utils import is_google_workflow_url_valid
 from contact_magic.scripts.logger import logger
-from contact_magic.conf.settings import SETTINGS
+from contact_magic.utils import is_google_workflow_url_valid
 
 
 def get_workflows_to_run(sheet):
     """
     Filter for only active workflows & ones with workflows URLs.
     """
     workflow_values = sheet.get_all_values()
```

### Comparing `contact_magic-0.2.1/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.3.0/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import pandas as pd
 
+from contact_magic.conf.settings import SETTINGS
 from contact_magic.helpers import worksheet_to_dataframe
 from contact_magic.integrations.sheets import (
     get_spreadsheet_by_url,
     get_worksheet_from_spreadsheet,
     update_cell,
 )
-from contact_magic.utils import is_google_workflow_url_valid
 from contact_magic.scripts.logger import logger
-from contact_magic.conf.settings import SETTINGS
+from contact_magic.utils import is_google_workflow_url_valid
 
 
 def update_rows_approved_and_remaining():
     workflows_sheet = get_worksheet_from_spreadsheet(
         get_spreadsheet_by_url(SETTINGS.MASTERSHEET_URL), "Workflows"
     )
     workflow_values = workflows_sheet.get_all_values()
```

### Comparing `contact_magic-0.2.1/contact_magic/utils.py` & `contact_magic-0.3.0/contact_magic/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -95,7 +95,27 @@
             empty[mapping.get(k, k)] = replace_keys(v, mapping)
         elif isinstance(v, list):
             newvalues = [replace_keys(x, mapping) for x in v]
             empty[mapping.get(k, k)] = newvalues
         else:
             empty[mapping.get(k, k)] = v
     return empty
+
+
+def replace_values(dictionary: dict, mapping: dict) -> dict:
+    if not isinstance(dictionary, dict) and not isinstance(mapping, dict):
+        return dictionary
+    empty = {}
+    # special case when it is called for element of array being NOT a dictionary
+    if isinstance(dictionary, str):
+        # nothing to do
+        return dictionary
+
+    for k, v in dictionary.items():
+        if isinstance(v, dict):
+            empty[k] = replace_values(v, mapping)
+        elif isinstance(v, list):
+            newvalues = [replace_values(x, mapping) for x in v]
+            empty[k] = newvalues
+        else:
+            empty[k] = mapping.get(k, v)
+    return empty
```

### Comparing `contact_magic-0.2.1/pyproject.toml` & `contact_magic-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.2.1"
+version = "0.3.0"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
@@ -39,18 +39,16 @@
 oauth2client = "4.1.3"
 oauthlib = "3.1.1"
 python-dotenv = "^1.0.0"
 pydantic = "1.10.8"
 structlog = "23.1.0"
 rich = "^13.4.1"
 
-[tool.flit.metadata.requires-extra]
-dev = [
-    "pre-commit >=2.17.0,<3.0.0",
-]
-
 [tool.poetry.scripts]
 contact-magic = "contact_magic.scripts.agency:app"
 
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.3.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `contact_magic-0.2.1/PKG-INFO` & `contact_magic-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.2.1
+Version: 0.3.0
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -78,26 +78,27 @@
 MASTERSHEET_URL=''
 GOOGLE_PROJECT_ID=''
 GOOGLE_PRIVATE_KEY_ID=''
 GOOGLE_PRIVATE_KEY=''
 GOOGLE_CLIENT_ID=''
 GOOGLE_CLIENT_EMAIL=''
 TIMEZONE="America/New_York"
-ALLOWED_SCRAPER_NAMES='get-case-study, get-company-achievement, get-company-description, get-company-announcement, FALLBACK'
+# list and dict are parsed as JSON.
+ALLOWED_SCRAPER_NAMES='["get-case-study", "get-company-achievement", "get-company-description", "get-company-announcement", "FALLBACK", "search-google"]'
 MAX_WORKERS='5'  # Number of concurrent workers to process. 5-10 is likely enough.
 ```
 
 If you are not using the agency workflows and just want to use the underlying PersonalizationSetttings objects you only
 need to set the following environment variables.
 
 ```python
 COPYFACTORY_API_KEY=''
 SALES_SCRAPERS_API_KEY=''
 # Optional since has default value
-ALLOWED_SCRAPER_NAMES='get-case-study, get-company-achievement, get-company-description, get-company-announcement, FALLBACK'
+ALLOWED_SCRAPER_NAMES='["get-case-study", "get-company-achievement", "get-company-description", "get-company-announcement", "FALLBACK", "search-google"]'
 # Optional since has default value
 MAX_WORKERS='5'
 ```
 
 ## Usage & Examples
 
 The core underlying model you will be using is 'PersonalizationSettings' which is responsible for understanding what
```

