# Comparing `tmp/distool-0.1.6.tar.gz` & `tmp/distool-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distool-0.1.6.tar", last modified: Mon Apr  3 17:05:07 2023, max compression
+gzip compressed data, was "distool-0.1.7.tar", last modified: Sun Jun 11 14:18:30 2023, max compression
```

## Comparing `distool-0.1.6.tar` & `distool-0.1.7.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.587885 distool-0.1.6/
--rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-02-27 19:53:19.000000 distool-0.1.6/LICENSE.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)     5948 2023-04-03 17:05:07.587948 distool-0.1.6/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     5115 2023-02-27 21:04:34.000000 distool-0.1.6/README.md
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.582498 distool-0.1.6/distool/
--rw-r--r--   0 michilegorov   (501) staff       (20)      191 2023-02-27 20:02:22.000000 distool-0.1.6/distool/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.583470 distool-0.1.6/distool/base/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/base/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      569 2023-02-27 19:15:03.000000 distool-0.1.6/distool/base/estimators.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.583722 distool-0.1.6/distool/data/
--rw-r--r--   0 michilegorov   (501) staff       (20)    97180 2023-03-25 08:36:09.000000 distool-0.1.6/distool/data/symptoms.json
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.585428 distool-0.1.6/distool/feature_extraction/
--rw-r--r--   0 michilegorov   (501) staff       (20)       97 2023-02-27 19:15:03.000000 distool-0.1.6/distool/feature_extraction/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3072 2023-03-18 12:35:30.000000 distool-0.1.6/distool/feature_extraction/anamnesis.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     4913 2023-04-02 19:07:00.000000 distool-0.1.6/distool/feature_extraction/extractors.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      499 2023-03-12 08:11:10.000000 distool-0.1.6/distool/feature_extraction/symptom.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2505 2023-03-25 07:58:05.000000 distool-0.1.6/distool/feature_extraction/symptom_collection.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      327 2023-02-27 19:15:03.000000 distool-0.1.6/distool/feature_extraction/symptom_status.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.585738 distool-0.1.6/distool/interpretation/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/interpretation/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1749 2023-03-18 12:35:30.000000 distool-0.1.6/distool/interpretation/explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.586156 distool-0.1.6/distool/models/
--rw-r--r--   0 michilegorov   (501) staff       (20)       88 2023-02-27 19:15:03.000000 distool-0.1.6/distool/models/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      576 2023-02-27 19:15:03.000000 distool-0.1.6/distool/models/classifiers.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.586586 distool-0.1.6/distool/tests/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.586861 distool-0.1.6/distool/tests/classifier/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/classifier/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      511 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/classifier/test_classifier.py
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/conftest.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.587110 distool-0.1.6/distool/tests/explainer/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/explainer/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      880 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/explainer/test_explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.587357 distool-0.1.6/distool/tests/extractors/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/extractors/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1132 2023-03-18 12:35:30.000000 distool-0.1.6/distool/tests/extractors/test_symptom_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-02-27 19:15:03.000000 distool-0.1.6/distool/tests/test_base.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.583247 distool-0.1.6/distool.egg-info/
--rw-r--r--   0 michilegorov   (501) staff       (20)     5948 2023-04-03 17:05:07.000000 distool-0.1.6/distool.egg-info/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     1064 2023-04-03 17:05:07.000000 distool-0.1.6/distool.egg-info/SOURCES.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-04-03 17:05:07.000000 distool-0.1.6/distool.egg-info/dependency_links.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-04-03 17:05:07.000000 distool-0.1.6/distool.egg-info/requires.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-04-03 17:05:07.000000 distool-0.1.6/distool.egg-info/top_level.txt
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-04-03 17:05:07.587730 distool-0.1.6/examples/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.6/examples/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1102 2023-02-27 19:15:03.000000 distool-0.1.6/examples/pipeline_example.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      115 2023-02-04 10:03:31.000000 distool-0.1.6/pyproject.toml
--rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-04-03 17:05:07.588147 distool-0.1.6/setup.cfg
--rw-r--r--   0 michilegorov   (501) staff       (20)     1317 2023-04-03 17:05:03.000000 distool-0.1.6/setup.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.460397 distool-0.1.7/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-02-27 19:53:19.000000 distool-0.1.7/LICENSE.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)      792 2023-06-11 14:18:30.460489 distool-0.1.7/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5115 2023-02-27 21:04:34.000000 distool-0.1.7/README.md
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.453827 distool-0.1.7/distool/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      191 2023-02-27 20:02:22.000000 distool-0.1.7/distool/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.454897 distool-0.1.7/distool/base/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/base/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      569 2023-02-27 19:15:03.000000 distool-0.1.7/distool/base/estimators.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.455232 distool-0.1.7/distool/data/
+-rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-06-11 14:13:26.000000 distool-0.1.7/distool/data/symptoms.json
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.457171 distool-0.1.7/distool/feature_extraction/
+-rw-r--r--   0 michilegorov   (501) staff       (20)       97 2023-02-27 19:15:03.000000 distool-0.1.7/distool/feature_extraction/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3377 2023-06-11 14:13:26.000000 distool-0.1.7/distool/feature_extraction/anamnesis.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     4913 2023-04-02 19:07:00.000000 distool-0.1.7/distool/feature_extraction/extractors.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      499 2023-03-12 08:11:10.000000 distool-0.1.7/distool/feature_extraction/symptom.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2505 2023-03-25 07:58:05.000000 distool-0.1.7/distool/feature_extraction/symptom_collection.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      327 2023-02-27 19:15:03.000000 distool-0.1.7/distool/feature_extraction/symptom_status.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.457524 distool-0.1.7/distool/interpretation/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/interpretation/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1749 2023-03-18 12:35:30.000000 distool-0.1.7/distool/interpretation/explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.457762 distool-0.1.7/distool/metrics/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:13:04.000000 distool-0.1.7/distool/metrics/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.458140 distool-0.1.7/distool/metrics/extractor/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:13:04.000000 distool-0.1.7/distool/metrics/extractor/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-06-11 14:13:26.000000 distool-0.1.7/distool/metrics/extractor/compute.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     7449 2023-06-11 14:13:26.000000 distool-0.1.7/distool/metrics/extractor/create_showcase.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.458497 distool-0.1.7/distool/models/
+-rw-r--r--   0 michilegorov   (501) staff       (20)       88 2023-02-27 19:15:03.000000 distool-0.1.7/distool/models/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      576 2023-06-11 14:13:29.000000 distool-0.1.7/distool/models/classifiers.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.458935 distool-0.1.7/distool/tests/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.459320 distool-0.1.7/distool/tests/classifier/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/classifier/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      511 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/classifier/test_classifier.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/conftest.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.459660 distool-0.1.7/distool/tests/explainer/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/explainer/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      880 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/explainer/test_explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.459926 distool-0.1.7/distool/tests/extractors/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/extractors/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1132 2023-03-18 12:35:30.000000 distool-0.1.7/distool/tests/extractors/test_symptom_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-02-27 19:15:03.000000 distool-0.1.7/distool/tests/test_base.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.454645 distool-0.1.7/distool.egg-info/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      792 2023-06-11 14:18:30.000000 distool-0.1.7/distool.egg-info/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1212 2023-06-11 14:18:30.000000 distool-0.1.7/distool.egg-info/SOURCES.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-06-11 14:18:30.000000 distool-0.1.7/distool.egg-info/dependency_links.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-06-11 14:18:30.000000 distool-0.1.7/distool.egg-info/requires.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-06-11 14:18:30.000000 distool-0.1.7/distool.egg-info/top_level.txt
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-06-11 14:18:30.460238 distool-0.1.7/examples/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.7/examples/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1102 2023-02-27 19:15:03.000000 distool-0.1.7/examples/pipeline_example.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      115 2023-02-04 10:03:31.000000 distool-0.1.7/pyproject.toml
+-rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-06-11 14:18:30.460734 distool-0.1.7/setup.cfg
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1219 2023-06-11 14:18:27.000000 distool-0.1.7/setup.py
```

### Comparing `distool-0.1.6/LICENSE.txt` & `distool-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/PKG-INFO` & `distool-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: distool
-Version: 0.1.6
-Summary: Disease processing tool kit
-Home-page: https://github.com/nirma-patient-intake/disease/
-Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
-Author: NIRMA Team of ITMO University
-Author-email: egorovmichil9@gmail.com
-License: MIT
-Keywords: NLP,Disease,Health Condition
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Классификатор заболеваний
 
 **Patient-intake** - модуль, обеспечивающий дистанционное взаимодействие пациента и медицинского учреждения с помощью диалоговых агентов. Реализован на языке Python.
 
 Модуль позволяет предсказывать возможное заболевание пациента на основе введенной им информации, присваивать диагнозу степень срочности приема, а также выводить интерпретацию результатов работы модели. Для обучения модели создан датасет, содержащий информацию о болезнях и их симптомах.
 
 Модуль поддерживает анализ текстов на русском языке.
```

### Comparing `distool-0.1.6/distool/base/estimators.py` & `distool-0.1.7/distool/base/estimators.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/distool/feature_extraction/anamnesis.py` & `distool-0.1.7/distool/feature_extraction/anamnesis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, List, Union
+from typing import Dict, List, Tuple, Union
 
 import numpy as np
 from spacy.tokens import Span
 
 from distool.feature_extraction.symptom import Symptom
 from distool.feature_extraction.symptom_collection import SymptomCollection
 from distool.feature_extraction.symptom_status import SymptomStatus
@@ -71,7 +71,15 @@
     def get_marks(self, as_number: bool = True) -> Union[List[SymptomStatus], np.array]:
         marks = list(self._symptoms_marks.values())
 
         if as_number:
             marks = np.array([mark.value for mark in marks])
 
         return marks
+
+    def get_marks_with_symptom_ids(
+        self, as_number: bool = True
+    ) -> List[Tuple[str, Union[SymptomStatus, int]]]:
+        marks = self.get_marks(as_number)
+        symptom_ids = map(lambda x: x.id_name, list(self._symptoms_marks.keys()))
+
+        return list(zip(symptom_ids, marks))
```

### Comparing `distool-0.1.6/distool/feature_extraction/extractors.py` & `distool-0.1.7/distool/feature_extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/distool/feature_extraction/symptom_collection.py` & `distool-0.1.7/distool/feature_extraction/symptom_collection.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/distool/interpretation/explainer.py` & `distool-0.1.7/distool/interpretation/explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/distool/models/classifiers.py` & `distool-0.1.7/distool/models/classifiers.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/distool/tests/explainer/test_explainer.py` & `distool-0.1.7/distool/tests/explainer/test_explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/distool/tests/extractors/test_symptom_extractor.py` & `distool-0.1.7/distool/tests/extractors/test_symptom_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.6/examples/pipeline_example.py` & `distool-0.1.7/examples/pipeline_example.py`

 * *Files identical despite different names*

