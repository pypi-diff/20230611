# Comparing `tmp/pytorch_partial_tagger-0.1.6.tar.gz` & `tmp/pytorch_partial_tagger-0.1.7.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.6.tar` & `pytorch_partial_tagger-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,42 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/notebooks/basic.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/training.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/__init__.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/tag.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/text.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/helpers.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/test_matchers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/data/__init__.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/data/test_core.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/data/batch/test_tag.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/LICENSE
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/metric.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/__init__.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/tag.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/text.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/helpers.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_matchers.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_metric.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_recognizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/__init__.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/test_core.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/conftest.py
+-rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/test_tag.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/test_text.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.6/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.7/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/notebooks/basic.ipynb` & `pytorch_partial_tagger-0.1.7/notebooks/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/tagger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import torch
 from torch.nn import Module
 
 from .crf.nn import CRF
-from .data.batch.text import TaggerInputs
 from .decoders import ViterbiDecoder
 from .encoders import BaseEncoder
 
 
 class SequenceTagger(Module):
     """Sequence tagger.
 
@@ -21,15 +20,15 @@
         super(SequenceTagger, self).__init__()
 
         self.encoder = encoder
         self.crf = CRF(encoder.get_hidden_size())
         self.decoder = decoder
 
     def forward(
-        self, inputs: TaggerInputs, mask: torch.Tensor
+        self, inputs: dict[str, torch.Tensor], mask: torch.Tensor
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Computes log potentials and tag sequence.
 
         Args:
             inputs: An inputs representing input data feeding into an embedder.
             mask: A [batch_size, sequence_length] boolean tensor.
 
@@ -39,9 +38,15 @@
             The float tensor representing log potentials and
             the integer tensor representing tag sequence.
         """
         log_potentials = self.crf(self.encoder(inputs), mask)
         tag_indices = self.decoder(log_potentials, mask)
         return log_potentials, tag_indices
 
-    def predict(self, inputs: TaggerInputs, mask: torch.Tensor) -> torch.Tensor:
+    def predict(
+        self, inputs: dict[str, torch.Tensor], mask: torch.Tensor
+    ) -> torch.Tensor:
         return self(inputs, mask)[1]
+
+    @property
+    def padding_index(self) -> int:
+        return self.decoder.padding_index
```

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/training.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
 
 from .crf import functional as F
 from .data import Dataset, LabelSet
-from .data.batch.tag import CharBasedTagsBatch, TagFactory
-from .data.batch.text import TextBatch
-from .encoders.transformer import EncoderType
+from .data.batch import Collator
+from .data.batch.tag import TagsBatch
+from .data.batch.text import BaseTokenizer, TextBatch
+from .decoders.viterbi import Contrainer, ViterbiDecoder
+from .encoders import BaseEncoderFactory
+from .metric import Metric
 from .recognizer import Recognizer
-from .utils import Collator, Metric, create_tagger, create_tokenizer
+from .tagger import SequenceTagger
 
 
 class SlantedTriangular:
     def __init__(self, max_steps: int, cut_frac: float = 0.1, ratio: int = 16):
         self.__cut_frac = cut_frac
         self.__cut = int(max_steps * cut_frac)
         self.__ratio = ratio
@@ -64,33 +67,35 @@
 
     return supervised_loss + balancing_coefficient * expected_entity_ratio_loss
 
 
 class Trainer:
     def __init__(
         self,
-        model_name: str = "roberta-base",
+        tokenizer: BaseTokenizer,
+        encoder_factory: BaseEncoderFactory,
         batch_size: int = 15,
         num_epochs: int = 20,
         learning_rate: float = 2e-5,
         gradient_clip_value: float = 5.0,
+        target_entity_ratio: float = 0.15,
+        entity_ratio_margin: float = 0.05,
+        balancing_coefficient: int = 10,
         padding_index: int = -1,
-        unknown_index: int = -100,
-        tokenizer_args: dict | None = None,
-        encoder_type: EncoderType = "default",
     ):
-        self.__model_name = model_name
+        self.__tokenizer = tokenizer
+        self.__encoder_factory = encoder_factory
         self.__batch_size = batch_size
         self.__num_epochs = num_epochs
         self.__learning_rate = learning_rate
         self.__gradient_clip_value = gradient_clip_value
+        self.__target_entity_ratio = target_entity_ratio
+        self.__entity_ratio_margin = entity_ratio_margin
+        self.__balancing_coefficient = balancing_coefficient
         self.__padding_index = padding_index
-        self.__unknown_index = unknown_index
-        self.__tokenizer_args = tokenizer_args
-        self.__encoder_type = encoder_type
 
     def __call__(
         self,
         train_dataset: Dataset,
         validation_dataset: Dataset,
         device: torch.device,
         logger: Logger | None = None,
@@ -104,23 +109,28 @@
         labels = set()
         for _, tags in train_dataset:
             for tag in tags:
                 if tag.label not in labels:
                     labels.add(tag.label)
         label_set = LabelSet(labels)
 
-        # Create a tagger
-        tagger = create_tagger(
-            self.__model_name, label_set, self.__padding_index, self.__encoder_type
+        tagger = SequenceTagger(
+            self.__encoder_factory.create(label_set),
+            ViterbiDecoder(
+                self.__padding_index,
+                Contrainer(
+                    label_set.get_start_states(),
+                    label_set.get_end_states(),
+                    label_set.get_transitions(),
+                ),
+            ),
         )
         tagger.to(device)
 
-        # Create a collator
-        tokenizer = create_tokenizer(self.__model_name, self.__tokenizer_args)
-        collator = Collator(tokenizer)
+        collator = Collator(self.__tokenizer, label_set)
 
         train_dataloader = DataLoader(
             train_dataset,  # type:ignore
             collate_fn=collator,
             batch_size=self.__batch_size,
         )
         validation_dataloader = DataLoader(
@@ -142,31 +152,33 @@
 
         for epoch in range(1, self.__num_epochs + 1):
             epoch_loss = 0.0
             tagger.train()
 
             for text_batch, tags_batch in train_dataloader:
                 text_batch = cast(TextBatch, text_batch)
-                tags_batch = cast(CharBasedTagsBatch, tags_batch)
+                tags_batch = cast(TagsBatch, tags_batch)
+
+                text_batch.to(device)
+                tags_batch.to(device)
 
                 optimizer.zero_grad()
 
-                mask = text_batch.get_mask(device)
-                log_potentials, _ = tagger(text_batch.get_tagger_inputs(device), mask)
+                mask = text_batch.mask
 
-                tag_factory = TagFactory(text_batch.tokenized_texts, label_set)
-                tags_bitmap = tag_factory.create_tag_bitmap(
-                    tags_batch, device, self.__padding_index, self.__unknown_index
-                )
+                log_potentials, _ = tagger(text_batch.tagger_inputs, mask)
 
                 loss = expected_entity_ratio_loss(
                     log_potentials,
-                    tags_bitmap,
+                    tags_batch.get_tag_bitmap(),
                     mask,
                     label_set.get_outside_index(),
+                    self.__target_entity_ratio,
+                    self.__entity_ratio_margin,
+                    self.__balancing_coefficient,
                 )
                 loss.backward()
 
                 torch.nn.utils.clip_grad_value_(
                     tagger.parameters(), clip_value=self.__gradient_clip_value
                 )
 
@@ -175,27 +187,26 @@
 
                 epoch_loss += loss.item() * text_batch.size
 
             tagger.eval()
             metric = Metric()
             for text_batch, tags_batch in validation_dataloader:
                 text_batch = cast(TextBatch, text_batch)
-                tags_batch = cast(CharBasedTagsBatch, tags_batch)
+                tags_batch = cast(TagsBatch, tags_batch)
 
-                tag_indices = tagger.predict(
-                    text_batch.get_tagger_inputs(device),
-                    text_batch.get_mask(device),
-                )
+                text_batch.to(device)
+                tags_batch.to(device)
+
+                tag_indices = tagger.predict(text_batch.tagger_inputs, text_batch.mask)
 
-                tag_factory = TagFactory(text_batch.tokenized_texts, label_set)
-                predictions = tag_factory.create_char_based_tags(
-                    tag_indices, self.__padding_index
+                predictions = text_batch.create_char_based_tags(
+                    tag_indices, label_set, tagger.padding_index
                 )
 
-                metric(predictions, tags_batch)
+                metric(predictions, tags_batch.char_based)
 
             scores = metric.get_scores()
 
             if best_f1_score < scores["f1_score"]:
                 best_f1_score = scores["f1_score"]
                 best_tagger_state.truncate(0)
                 best_tagger_state.seek(0)
@@ -208,8 +219,8 @@
                     **{f"validation_{key}": value for key, value in scores.items()},
                 }
             )
 
         best_tagger_state.seek(0)
         tagger.load_state_dict(torch.load(best_tagger_state))
 
-        return Recognizer(tagger, tokenizer, label_set, self.__padding_index)
+        return Recognizer(tagger, self.__tokenizer, label_set)
```

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from bisect import bisect_left
 from collections.abc import Iterator
 from dataclasses import dataclass
+from enum import Enum, auto
 
 
 @dataclass(frozen=True, eq=True)
 class Span:
     start: int
     length: int
 
@@ -24,32 +25,14 @@
         return self.span.start
 
     @property
     def length(self) -> int:
         return self.span.length
 
 
-@dataclass(frozen=True, eq=True)
-class CharBasedTags:
-    tags: tuple[Tag, ...]
-    text: str
-
-    def __iter__(self) -> Iterator[Tag]:
-        yield from self.tags
-
-    def __repr__(self) -> str:
-        tag_strs = []
-        for tag in self:
-            start = tag.start
-            end = tag.start + tag.length
-            tag_str = f"{self.text[start:end]} ({tag.label})"
-            tag_strs.append(tag_str)
-        return f"({', '.join(tag_strs)})"
-
-
 class TokenizedText:
     def __init__(
         self,
         text: str,
         char_spans: tuple[Span | None, ...],
         token_indices: tuple[int, ...],
         addtional_token: str = "[Token]",
@@ -101,14 +84,45 @@
 
         return Span(
             char_span_start.start,
             char_span_end.start + char_span_end.length - char_span_start.start,
         )
 
 
+@dataclass(frozen=True, eq=True)
+class CharBasedTags:
+    tags: tuple[Tag, ...]
+    text: str
+
+    def __iter__(self) -> Iterator[Tag]:
+        yield from self.tags
+
+    def __repr__(self) -> str:
+        tag_strs = []
+        for tag in self:
+            start = tag.start
+            end = tag.start + tag.length
+            tag_str = f"{self.text[start:end]} ({tag.label})"
+            tag_strs.append(tag_str)
+        return f"({', '.join(tag_strs)})"
+
+    def convert_to_token_based(self, tokenized_text: TokenizedText) -> "TokenBasedTags":
+        if self.text != tokenized_text.get_text():
+            raise ValueError("The text doesn't match")
+
+        tags = []
+        for tag in self.tags:
+            start = tokenized_text.convert_to_token_index(tag.start)
+            end = tokenized_text.convert_to_token_index(tag.start + tag.length - 1)
+            length = end - start + 1
+            tags.append(Tag(Span(start, length), tag.label))
+
+        return TokenBasedTags(tuple(tags), tokenized_text)
+
+
 @dataclass(frozen=True)
 class TokenBasedTags:
     tags: tuple[Tag, ...]
     tokenized_text: TokenizedText
 
     def __iter__(self) -> Iterator[Tag]:
         yield from self.tags
@@ -121,40 +135,104 @@
             tag_str = " ".join(
                 self.tokenized_text.get_token(token_index)
                 for token_index in range(start, end)
             )
             tag_strs.append(f"{tag_str} ({tag.label})")
         return f"({', '.join(tag_strs)})"
 
-    def get_char_based_tags(self) -> CharBasedTags:
+    @property
+    def num_tokens(self) -> int:
+        return self.tokenized_text.num_tokens
+
+    def convert_to_char_based(self) -> CharBasedTags:
         tags = []
         for tag in self.tags:
             char_span = self.tokenized_text.convert_to_char_span(tag.span)
             if char_span is not None:
                 tags.append(Tag(char_span, tag.label))
         return CharBasedTags(tuple(tags), self.tokenized_text.get_text())
 
+    def get_tag_indices(
+        self, label_set: LabelSet, unknown_index: int = -100
+    ) -> list[int]:
+        tag_indices = [unknown_index] * self.tokenized_text.num_tokens
+
+        for token_index in range(self.tokenized_text.num_tokens):
+            span = self.tokenized_text.get_char_span(token_index)
+            if span is None:
+                tag_indices[token_index] = label_set.get_outside_index()
+
+        for tag in self.tags:
+            start = tag.start
+            end = tag.start + tag.length - 1
+            if start == end:
+                tag_indices[start] = label_set.get_unit_index(tag.label)
+            else:
+                tag_indices[start] = label_set.get_start_index(tag.label)
+                tag_indices[start + 1 : end] = [
+                    label_set.get_inside_index(tag.label)
+                ] * (end - start - 1)
+                tag_indices[end] = label_set.get_end_index(tag.label)
+
+        return tag_indices
+
+    def get_tag_bitmap(self, label_set: LabelSet) -> list[list[bool]]:
+        tag_bitmap = [
+            [False] * label_set.get_tag_size() for _ in range(self.num_tokens)
+        ]
+        for token_index in range(self.num_tokens):
+            span = self.tokenized_text.get_char_span(token_index)
+            if span is None:
+                tag_bitmap[token_index][label_set.get_outside_index()] = True
+
+        for tag in sorted(
+            self,
+            key=lambda tag: (tag.start, tag.start + tag.length),
+        ):
+            start = tag.start
+            end = tag.start + tag.length - 1  # inclusive
+            if start == end:
+                tag_bitmap[start][label_set.get_unit_index(tag.label)] = True
+            else:
+                tag_bitmap[start][label_set.get_start_index(tag.label)] = True
+                for i in range(start + 1, end):
+                    tag_bitmap[i][label_set.get_inside_index(tag.label)] = True
+                tag_bitmap[end][label_set.get_end_index(tag.label)] = True
+
+        for bit in tag_bitmap:
+            if sum(bit) == 0:
+                bit[:] = [True] * label_set.get_tag_size()
+
+        return tag_bitmap
+
+
+class Status(Enum):
+    START = auto()
+    INSIDE = auto()
+    END = auto()
+    UNIT = auto()
+
 
 class LabelSet:
     def __init__(self, labels: set[str]):
         self.__labels = [*sorted(labels)]
-        self.__status_kind = 4  # start, inside, end, unit
+        self.__status_size = len(Status)  # start, inside, end, unit
 
         self.__start_indices = [
             *range(
                 1,
                 self.get_tag_size(),
-                self.__status_kind,
+                self.__status_size,
             )
         ]
         self.__unit_indices = [
             *range(
-                self.__status_kind,
+                self.__status_size,
                 self.get_tag_size(),
-                self.__status_kind,
+                self.__status_size,
             )
         ]
 
         self.__label_ids = dict(zip(self.__labels, self.__start_indices))
 
     def __contains__(self, label: str) -> bool:
         i = bisect_left(self.__labels, label)
@@ -183,25 +261,43 @@
         return self.__labels
 
     def get_label_size(self) -> int:
         return len(self.__labels)
 
     def get_tag_size(self) -> int:
         # (start, inside, end, unit) * label + outside status
-        return self.__status_kind * self.get_label_size() + 1
+        return self.__status_size * self.get_label_size() + 1
 
     def get_label(self, index: int) -> str | None:
         if index < 0 or index >= self.get_tag_size():
             raise ValueError("Invalid index.")
 
         if index == self.get_outside_index():
             return None
 
         return self.__labels[bisect_left(self.__unit_indices, index)]
 
+    def get_status(self, index: int) -> Status | None:
+        if index < 0 or index >= self.get_tag_size():
+            raise ValueError("Invalid index.")
+
+        label = self.get_label(index)
+        if label is None:
+            return None
+        elif self.get_start_index(label) == index:
+            return Status.START
+        elif self.get_inside_index(label) == index:
+            return Status.INSIDE
+        elif self.get_end_index(label) == index:
+            return Status.END
+        elif self.get_unit_index(label) == index:
+            return Status.UNIT
+        else:
+            raise ValueError("Invalid index.")
+
     def get_start_states(self) -> list[bool]:
         states = [False] * self.get_tag_size()
         # Always allowed starts from outside status
         states[self.get_outside_index()] = True
 
         for labeled_start_index in self.__start_indices:
             labeled_unit_index = labeled_start_index + 3
```

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/viterbi.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,34 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 
 import torch
 from torch.nn import Module
 
-from ..data.batch.text import TaggerInputs
+from ..data.core import LabelSet
 
 
 class BaseEncoder(Module, metaclass=ABCMeta):
     """Base class of all encoders."""
 
     @abstractmethod
-    def forward(self, inputs: TaggerInputs) -> torch.Tensor:
+    def forward(self, inputs: dict[str, torch.Tensor]) -> torch.Tensor:
         """Encode the given inputs to a tensor.
 
         Args:
             inputs: A dictionary that maps a string key to a tensor value.
 
         Returns:
             A [batch_size, sequence_length, hidden_size] float tensor.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_hidden_size(self) -> int:
         raise NotImplementedError
+
+
+class BaseEncoderFactory(metaclass=ABCMeta):
+    @abstractmethod
+    def create(self, label_set: LabelSet) -> BaseEncoder:
+        raise NotImplementedError
```

### Comparing `pytorch_partial_tagger-0.1.6/tests/conftest.py` & `pytorch_partial_tagger-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/tests/helpers.py` & `pytorch_partial_tagger-0.1.7/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/tests/test_matchers.py` & `pytorch_partial_tagger-0.1.7/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.7/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.7/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.7/tests/data/test_core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/tests/data/batch/test_tag.py` & `pytorch_partial_tagger-0.1.7/tests/data/batch/test_text.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,44 @@
+from __future__ import annotations
+
 import pytest
 import torch
-from transformers import AutoTokenizer
 
 from partial_tagger.data import CharBasedTags, LabelSet, Span, Tag
-from partial_tagger.data.batch.tag import TagFactory
 from partial_tagger.data.batch.text import TransformerTokenizer
 
 
-@pytest.fixture
-def tokenizer() -> TransformerTokenizer:
-    return TransformerTokenizer(AutoTokenizer.from_pretrained("distilroberta-base"))
-
-
-@pytest.fixture
-def label_set() -> LabelSet:
-    return LabelSet({"ORG", "LOC", "PER", "MISC"})
-
-
+@pytest.mark.parametrize(
+    "text, tag_indices, tags",
+    [
+        (
+            "Tokyo is the capital of Japan.",
+            torch.tensor([[0, 1, 3, 0, 0, 0, 0, 4, 0, 0]]),
+            (Tag(Span(0, 5), "LOC"), Tag(Span(24, 5), "LOC")),
+        ),
+        (
+            "John Doe",
+            torch.tensor([[0, 16, 16, 0]]),
+            (Tag(Span(0, 4), "PER"), Tag(Span(5, 3), "PER")),
+        ),
+        (
+            "John Doe",
+            torch.tensor([[0, 13, 15, 0]]),
+            (Tag(Span(0, 8), "PER"),),
+        ),
+    ],
+)
 def test_char_based_tags_are_valid(
-    tokenizer: TransformerTokenizer, label_set: LabelSet
+    tokenizer: TransformerTokenizer,
+    label_set: LabelSet,
+    text: str,
+    tag_indices: torch.Tensor,
+    tags: tuple[Tag],
 ) -> None:
-    text = "Tokyo is the capital of Japan."
-    tag_indices = torch.tensor([[0, 1, 3, 0, 0, 0, 0, 4, 0, 0]])
-
-    expected = CharBasedTags(
-        (Tag(Span(0, 5), "LOC"), Tag(Span(24, 5), "LOC")), text=text
-    )
+    expected = CharBasedTags(tags, text)
 
     text_batch = tokenizer((text,))
-    tag_factory = TagFactory(text_batch.tokenized_texts, label_set)
 
-    char_based_tags_batch = tag_factory.create_char_based_tags(tag_indices)
+    char_based_tags_batch = text_batch.create_char_based_tags(tag_indices, label_set)
 
     assert len(char_based_tags_batch) == 1
     assert char_based_tags_batch[0] == expected
-
-
-def test_tag_indices_are_valid(
-    tokenizer: TransformerTokenizer, label_set: LabelSet
-) -> None:
-    text = "Tokyo is the capital of Japan."
-    tags = CharBasedTags((Tag(Span(0, 5), "LOC"), Tag(Span(24, 5), "LOC")), text=text)
-    unknown_index = -100
-
-    expected = torch.tensor([[0, 1, 3, -100, -100, -100, -100, 4, -100, 0]])
-
-    text_batch = tokenizer((text,))
-    tag_factory = TagFactory(text_batch.tokenized_texts, label_set)
-
-    tag_indices = tag_factory.create_tag_indices(
-        (tags,), torch.device("cpu"), unknown_index=unknown_index
-    )
-
-    assert torch.equal(tag_indices, expected)
```

### Comparing `pytorch_partial_tagger-0.1.6/.gitignore` & `pytorch_partial_tagger-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/LICENSE` & `pytorch_partial_tagger-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/README.md` & `pytorch_partial_tagger-0.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 Import all dependencies first:
 
 ```py
 import torch
 
 from partial_tagger.data import CharBasedTags
-from partial_tagger.training import Trainer
-from partial_tagger.utils import Metric, create_tag
+from partial_tagger.metric import Metric
+from partial_tagger.utils import create_tag, create_trainer
 ```
 
 Prepare your own datasets.
 Each item of dataset must have a string and tags. A string represents `text` below.
 Tags represent a collection of tags, where each tag has a start, a length, and a label, which are defined as `tags` below.
 A start represents a position in `text` where a tag starts.
 A length represents a distance in `text` between the beginning of a tag and the end of a tag.
@@ -47,18 +47,18 @@
 You could evaluate the performance of your tagger using `Metric` as below.
 
 
 ```py
 
 device = torch.device("cuda")
 
-trainer = Trainer()
+trainer = create_trainer()
 recognizer = trainer(train_dataset, validation_dataset, device)
 
-texts, ground_truths = zip(*test_dataset, strict=True)
+texts, ground_truths = zip(*test_dataset)
 
 batch_size = 15
 predictions = recognizer(texts, batch_size, device)
 
 metric = Metric()
 metric(predictions, ground_truths)
 
@@ -69,8 +69,10 @@
 
 ```bash
 pip install pytorch-partial-tagger
 ```
 
 ## References
 
+ - Yuta Tsuboi, Hisashi Kashima, Shinsuke Mori, Hiroki Oda, and Yuji Matsumoto. 2008. [Training Conditional Random Fields Using Incomplete Annotations](https://aclanthology.org/C08-1113/). In _Proceedings of the 22nd International Conference on Computational Linguistics (Coling 2008)_, pages 897–904, Manchester, UK. Coling 2008 Organizing Committee.
+- Alexander Rush. 2020. [Torch-Struct: Deep Structured Prediction Library](https://aclanthology.org/2020.acl-demos.38/). In _Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics: System Demonstrations_, pages 335–342, Online. Association for Computational Linguistics.
 - Thomas Effland and Michael Collins. 2021. [Partially Supervised Named Entity Recognition via the Expected Entity Ratio Loss](https://aclanthology.org/2021.tacl-1.78/). _Transactions of the Association for Computational Linguistics_, 9:1320–1335.
```

### Comparing `pytorch_partial_tagger-0.1.6/pyproject.toml` & `pytorch_partial_tagger-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.6/PKG-INFO` & `pytorch_partial_tagger-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.6
+Version: 0.1.7
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -32,16 +32,16 @@
 
 Import all dependencies first:
 
 ```py
 import torch
 
 from partial_tagger.data import CharBasedTags
-from partial_tagger.training import Trainer
-from partial_tagger.utils import Metric, create_tag
+from partial_tagger.metric import Metric
+from partial_tagger.utils import create_tag, create_trainer
 ```
 
 Prepare your own datasets.
 Each item of dataset must have a string and tags. A string represents `text` below.
 Tags represent a collection of tags, where each tag has a start, a length, and a label, which are defined as `tags` below.
 A start represents a position in `text` where a tag starts.
 A length represents a distance in `text` between the beginning of a tag and the end of a tag.
@@ -72,18 +72,18 @@
 You could evaluate the performance of your tagger using `Metric` as below.
 
 
 ```py
 
 device = torch.device("cuda")
 
-trainer = Trainer()
+trainer = create_trainer()
 recognizer = trainer(train_dataset, validation_dataset, device)
 
-texts, ground_truths = zip(*test_dataset, strict=True)
+texts, ground_truths = zip(*test_dataset)
 
 batch_size = 15
 predictions = recognizer(texts, batch_size, device)
 
 metric = Metric()
 metric(predictions, ground_truths)
 
@@ -94,8 +94,10 @@
 
 ```bash
 pip install pytorch-partial-tagger
 ```
 
 ## References
 
+ - Yuta Tsuboi, Hisashi Kashima, Shinsuke Mori, Hiroki Oda, and Yuji Matsumoto. 2008. [Training Conditional Random Fields Using Incomplete Annotations](https://aclanthology.org/C08-1113/). In _Proceedings of the 22nd International Conference on Computational Linguistics (Coling 2008)_, pages 897–904, Manchester, UK. Coling 2008 Organizing Committee.
+- Alexander Rush. 2020. [Torch-Struct: Deep Structured Prediction Library](https://aclanthology.org/2020.acl-demos.38/). In _Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics: System Demonstrations_, pages 335–342, Online. Association for Computational Linguistics.
 - Thomas Effland and Michael Collins. 2021. [Partially Supervised Named Entity Recognition via the Expected Entity Ratio Loss](https://aclanthology.org/2021.tacl-1.78/). _Transactions of the Association for Computational Linguistics_, 9:1320–1335.
```

