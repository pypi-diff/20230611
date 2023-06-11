# Comparing `tmp/velesresearch-0.0.6.tar.gz` & `tmp/velesresearch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velesresearch-0.0.6.tar", max compression
+gzip compressed data, was "velesresearch-0.0.7.tar", max compression
```

## Comparing `velesresearch-0.0.6.tar` & `velesresearch-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-10 19:45:41.718124 velesresearch-0.0.6/LICENSE
--rw-r--r--   0        0        0     1438 2023-06-10 19:45:41.718124 velesresearch-0.0.6/README.md
--rw-r--r--   0        0        0      657 2023-06-10 19:45:41.722124 velesresearch-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      158 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/__init__.py
--rw-r--r--   0        0        0     1589 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/options.py
--rw-r--r--   0        0        0     6825 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/structure.py
--rw-r--r--   0        0        0     1945 2023-06-10 19:45:41.722124 velesresearch-0.0.6/velesresearch/tools.py
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 velesresearch-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-11 02:01:05.236054 velesresearch-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1707 2023-06-11 02:01:05.236054 velesresearch-0.0.7/README.md
+-rw-r--r--   0        0        0      825 2023-06-11 02:01:05.240054 velesresearch-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/__init__.py
+-rw-r--r--   0        0        0      795 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/options.py
+-rw-r--r--   0        0        0     6562 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/structure.py
+-rw-r--r--   0        0        0     2358 2023-06-11 02:01:05.240054 velesresearch-0.0.7/velesresearch/tools.py
+-rw-r--r--   0        0        0     2473 1970-01-01 00:00:00.000000 velesresearch-0.0.7/PKG-INFO
```

### Comparing `velesresearch-0.0.6/LICENSE` & `velesresearch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.6/README.md` & `velesresearch-0.0.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,17 @@
     <img alt="Veles logo, text Veles with Veles' rune instead of V." src="Veles-logo.svg" width=60%>
   </picture>
 </p>
 <br>
 
 <!-- badges: start -->
 
-![PyPI](https://img.shields.io/pypi/v/velesresearch)
-![GitHub](https://img.shields.io/github/license/jakub-jedrusiak/VelesResearch)
+[![PyPI](https://img.shields.io/pypi/v/velesresearch)](https://pypi.org/project/velesresearch/)
+[![GitHub](https://img.shields.io/badge/license-GPL--3.0-informational)](https://github.com/jakub-jedrusiak/VelesResearch/blob/main/LICENSE)
+[![codecov](https://codecov.io/gh/jakub-jedrusiak/VelesResearch/branch/main/graph/badge.svg?token=CGc3zeDxFi)](https://codecov.io/gh/jakub-jedrusiak/VelesResearch)
 
 <!-- badges: end -->
 
 Veles is a free and open source python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
 
 Veles is in pre-alpha development, but the goal features are:
```

### Comparing `velesresearch-0.0.6/velesresearch/structure.py` & `velesresearch-0.0.7/velesresearch/structure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,57 @@
 "Structural elements of the survey"
 from collections.abc import Sequence
 from json import JSONEncoder, dumps
+from pydantic import BaseModel, validator
 import numpy as np
 from .options import QuestionOptions, PageOptions, SurveyOptions
 
 
-class Question:
+class Question(BaseModel):
     "General question class"
-
-    def __init__(
-        self,
-        label: str,
-        question_type: str,
-        question_text: str,
-        *answers: str | Sequence[str],
-        options: QuestionOptions | None = None,
-        description: str | None = None,
-    ):
-        self.label = label
-        self.question_type = question_type
-        self.question_text = question_text
-        self.answers = list(np.concatenate([answers]).flat)
-        self.options = options
-        self.description = description
+    label: str
+    question_type: str
+    question_text: str
+    answers: str | Sequence[str]
+    options: QuestionOptions | None = None
+    description: str | None = None
 
     def __str__(self):
         answers = "  - " + "\n  - ".join(self.answers)
         return (
             f"{self.label}:\n  {self.question_text} ({self.question_type})\n{answers}"
         )
 
     def __repr__(self):
         return f"Question({self.label})"
 
 
-class Page:
+class Page(BaseModel):
     "General page class"
-
-    def __init__(
-        self,
-        label: str,
-        *questions: Question | Sequence[Question],
-        title: str | None = None,
-        description: str | None = None,
-        options: PageOptions | None = None,
-    ):
-        self.label = label
-        self.questions = list(np.concatenate([questions]).flat)
-        self.title = title
-        self.description = description
-        self.options = options
-
-        # Exception if there are questions with the same label
-        for question in enumerate(self.questions):
-            if question[1].label in [
-                q.label
-                for q in self.questions[: question[0]]
-                + self.questions[question[0] + 1 :]
-            ]:
-                raise ValueError(f"Multiple questions with label '{question[1].label}'")
+    label: str
+    questions: Question | Sequence[Question]
+    title: str | None = None
+    description: str | None = None
+    options: PageOptions | None = None
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if isinstance(self.questions, Question):
+            self.questions = [self.questions]
+
+    @validator("questions")
+    def check_labels(cls, questions):
+        "Exception if there are questions with the same label"
+        if not isinstance(questions, Question):
+            labels = []
+            for question in questions:
+                labels.append(question.label)
+            if len(labels) != len(set(labels)):
+                raise ValueError("Questions labels in page must be unique")
+        return questions
 
     def __str__(self):
         page = f"Page {self.label}:\n"
         for i in enumerate(self.questions):
             page += f"  {i[0] + 1}. {i[1].label}\n"
         return page
 
@@ -74,35 +63,36 @@
             return self.questions[index]
         if isinstance(index, str):
             for question in self.questions:
                 if question.label == index:
                     return question
 
 
-class Survey:
+class Survey(BaseModel):
     "General survey class"
-
-    def __init__(
-        self,
-        *pages: Page | Sequence[Page],
-        title: str | None = None,
-        description: str | None = None,
-        options: SurveyOptions | None = None,
-    ):
-        self.pages = list(np.concatenate([pages]).flat)
-        self.title = title
-        self.description = description
-        self.options = options
-
-        # Exception if there are pages with the same label
-        for page in enumerate(self.pages):
-            if page[1].label in [
-                p.label for p in self.pages[: page[0]] + self.pages[page[0] + 1 :]
-            ]:
-                raise ValueError(f"Multiple pages with label '{page[1].label}'")
+    pages: Page | Sequence[Page]
+    title: str | None = None
+    description: str | None = None
+    options: SurveyOptions | None = None
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if isinstance(self.pages, Page):
+            self.pages = [self.pages]
+
+    @validator("pages")
+    def check_labels(cls, pages):
+        "Exception if there are pages with the same label"
+        if not isinstance(pages, Page):
+            labels = []
+            for page in pages:
+                labels.append(page.label)
+            if len(labels) != len(set(labels)):
+                raise ValueError("Pages labels in survey must be unique")
+        return pages
 
     def create(self):
         "Saves survey to survey.json file"
         json = dumps(obj=self, cls=SurveyEncoder, indent=2)
         survey_file = open("survey.json", "w", encoding="utf-8")
         survey_file.write(json)
         survey_file.close()
```

### Comparing `velesresearch-0.0.6/velesresearch/tools.py` & `velesresearch-0.0.7/velesresearch/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 "Functions and wrappers for creating survey structure"
 from collections.abc import Sequence
+from pydantic import validate_arguments
+import numpy as np
 from .structure import Question, Page, Survey
 from .options import QuestionOptions, PageOptions, SurveyOptions
 
 
 def question(
     label: str,
     question_type: str,
     question_text: str,
     *answers: str | Sequence[str],
     options: QuestionOptions | None = None,
     description: str | None = None,
 ) -> Question:
     "Wrapper around Question class"
+    answers = list(np.concatenate([answers]).flat)
     return Question(
-        label,
-        question_type,
-        question_text,
-        answers,
+        label=label,
+        question_type=question_type,
+        question_text=question_text,
+        answers=answers,
         options=options,
         description=description,
     )
 
 
+@validate_arguments
 def questionnaire(
     label: str,
     items: Sequence[str] | str,
     answers: Sequence[str] | str,
     question_type: str = "radio",
-    options: QuestionOptions = None,
-    description: str = None,
+    options: QuestionOptions | None = None,
+    description: str | None = None,
 ) -> list[Question]:
     "Convert whole questionnaire to Question objects list"
     q_list = []
     for i in enumerate(items):
         q_list.append(
             Question(
-                f"{label}_{i[0] + 1}",
-                question_type,
-                i[1],
-                answers,
+                label=f"{label}_{i[0] + 1}",
+                question_type=question_type,
+                question_text=i[1],
+                answers=answers,
                 options=options,
                 description=description,
             )
         )
     return q_list
 
 
@@ -51,22 +55,32 @@
     label: str,
     *questions: Question | Sequence[Question],
     title: str | None = None,
     description: str | None = None,
     options: PageOptions | None = None,
 ) -> Page:
     "Wrapper around Page class"
-    return Page(label, questions, title=title, description=description, options=options)
+    questions = list(np.concatenate([questions]).flat)
+    return Page(
+        label=label,
+        questions=questions,
+        title=title,
+        description=description,
+        options=options,
+    )
 
 
 def survey(
     *pages: Page | Sequence[Page],
     title: str | None = None,
     description: str | None = None,
     options: SurveyOptions | None = None,
     create_file: bool = True,
 ) -> Survey:
     "Create Survey object from pages, create json file"
-    survey_obj = Survey(pages, title=title, description=description, options=options)
+    pages = list(np.concatenate([pages]).flat)
+    survey_obj = Survey(
+        pages=pages, title=title, description=description, options=options
+    )
     if create_file:
         survey_obj.create()
     return survey_obj
```

### Comparing `velesresearch-0.0.6/PKG-INFO` & `velesresearch-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: velesresearch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Veles is a free and open source python survey tool for researchers.
 Home-page: https://github.com/jakub-jedrusiak/VelesResearch
 License: GPL-3.0-or-later
 Author: Jakub Jędrusiak
 Author-email: kuba23031999@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Project-URL: Documentation, https://jakub-jedrusiak.github.io/VelesDocs
 Project-URL: Repository, https://github.com/jakub-jedrusiak/VelesResearch
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="/figs/Veles-logo-white.svg">
@@ -23,16 +23,17 @@
     <img alt="Veles logo, text Veles with Veles' rune instead of V." src="Veles-logo.svg" width=60%>
   </picture>
 </p>
 <br>
 
 <!-- badges: start -->
 
-![PyPI](https://img.shields.io/pypi/v/velesresearch)
-![GitHub](https://img.shields.io/github/license/jakub-jedrusiak/VelesResearch)
+[![PyPI](https://img.shields.io/pypi/v/velesresearch)](https://pypi.org/project/velesresearch/)
+[![GitHub](https://img.shields.io/badge/license-GPL--3.0-informational)](https://github.com/jakub-jedrusiak/VelesResearch/blob/main/LICENSE)
+[![codecov](https://codecov.io/gh/jakub-jedrusiak/VelesResearch/branch/main/graph/badge.svg?token=CGc3zeDxFi)](https://codecov.io/gh/jakub-jedrusiak/VelesResearch)
 
 <!-- badges: end -->
 
 Veles is a free and open source python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
 
 Veles is in pre-alpha development, but the goal features are:
```

