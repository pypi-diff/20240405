# Comparing `tmp/politely-3.3.4.tar.gz` & `tmp/politely-4.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politely-3.3.4.tar", max compression
+gzip compressed data, was "politely-4.0.0a0.tar", max compression
```

## Comparing `politely-3.3.4.tar` & `politely-4.0.0a0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    10991 2024-04-02 13:54:31.018865 politely-3.3.4/README.md
--rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-3.3.4/politely/__init__.py
--rw-r--r--   0        0        0      913 2024-04-02 05:16:13.209308 politely-3.3.4/politely/errors.py
--rw-r--r--   0        0        0      833 2024-04-02 05:16:13.209376 politely-3.3.4/politely/fetchers.py
--rw-r--r--   0        0        0     2934 2024-04-02 13:52:39.166339 politely-3.3.4/politely/modeling_gpt2_scorer.py
--rw-r--r--   0        0        0     1229 2024-04-02 05:16:13.209536 politely-3.3.4/politely/modeling_heuristic_scorer.py
--rw-r--r--   0        0        0      161 2024-04-02 05:16:13.209606 politely-3.3.4/politely/modeling_scorer.py
--rw-r--r--   0        0        0     5379 2024-04-02 08:08:10.933663 politely-3.3.4/politely/rules.py
--rw-r--r--   0        0        0     6708 2024-04-02 13:53:39.371403 politely-3.3.4/politely/styler.py
--rw-r--r--   0        0        0      422 2024-04-02 13:50:49.938029 politely-3.3.4/pyproject.toml
--rw-r--r--   0        0        0    11517 1970-01-01 00:00:00.000000 politely-3.3.4/PKG-INFO
+-rw-r--r--   0        0        0    10895 2024-04-05 04:59:46.503224 politely-4.0.0a0/README.md
+-rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-4.0.0a0/politely/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-05 04:59:46.504517 politely-4.0.0a0/politely/errors.py
+-rw-r--r--   0        0        0      676 2024-04-05 04:59:46.504948 politely-4.0.0a0/politely/fetchers.py
+-rw-r--r--   0        0        0     2949 2024-04-05 04:59:46.505487 politely-4.0.0a0/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1202 2024-04-05 04:59:46.505881 politely-4.0.0a0/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      715 2024-04-05 04:59:46.506199 politely-4.0.0a0/politely/modeling_sbg_scorer.py
+-rw-r--r--   0        0        0      171 2024-04-05 04:59:46.506564 politely-4.0.0a0/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     5372 2024-04-05 04:59:46.507048 politely-4.0.0a0/politely/rules.py
+-rw-r--r--   0        0        0     7024 2024-04-05 04:59:46.507502 politely-4.0.0a0/politely/styler.py
+-rw-r--r--   0        0        0      424 2024-04-05 04:59:46.507879 politely-4.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11423 1970-01-01 00:00:00.000000 politely-4.0.0a0/PKG-INFO
```

### Comparing `politely-3.3.4/README.md` & `politely-4.0.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
-![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://politely.streamlit.app)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Feubinecto%2Fpolitely&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Downloads](https://pepy.tech/badge/politely)](https://pepy.tech/project/politely)
 [![Downloads](https://pepy.tech/badge/politely/week)](https://pepy.tech/project/politely)
```

### Comparing `politely-3.3.4/politely/errors.py` & `politely-4.0.0a0/politely/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import re
-from typing import List
-from politely.rules import RULES
 
 
 class SFNotIncludedError(Exception):
     """
     An exception raised when a sentence does not include a SF.
     """
```

### Comparing `politely-3.3.4/politely/modeling_gpt2_scorer.py` & `politely-4.0.0a0/politely/modeling_gpt2_scorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import random
-from typing import List
 import numpy as np
 from kiwipiepy import Kiwi
 from transformers import AutoTokenizer, GPT2LMHeadModel
-from politely import TAG
 from politely.modeling_scorer import Scorer
+from politely import TAG
 
 
 class GPT2Scorer(Scorer):
     """
-    More accurate than heuristic scorer, but slower.
+    More accurate than heuristic scorer, but slower. Could be made faster with GPU support. 
     """
 
     def __init__(self, device: str = "cpu"):
         import torch
         self.gpt2 = GPT2LMHeadModel.from_pretrained(
             "beomi/kykim-gpt3-kor-small_based_on_gpt2"
         ).to(device)
@@ -31,16 +30,16 @@
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = True
 
     def __call__(
         self,
-        candidates: List[List[str]],
-        logs: dict,
+        candidates: list[list[str]],
+        log: dict,
         kiwi: Kiwi,
         # label_smoothing: https://ratsgo.github.io/insight-notes/docs/interpretable/smoothing
         label_smoothing: float = 0.2,
     ) -> list[float]:
         """
         # label_smoothing: https://ratsgo.github.io/insight-notes/docs/interpretable/smoothing
         이걸 batched processing으로 바꾸고 계속하기. device parameter도 추가하기.
```

### Comparing `politely-3.3.4/politely/modeling_heuristic_scorer.py` & `politely-4.0.0a0/politely/modeling_heuristic_scorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import List
 from kiwipiepy import Kiwi
 from politely import PREFERENCES, CASUAL, POLITE, FORMAL, SEP
 from politely.modeling_scorer import Scorer
 
 
 class HeuristicScorer(Scorer):
 
-    def __call__(self, candidates: List[List[str]], logs: dict, kiwi: Kiwi) -> List[List[float]]:
+    def __call__(self, candidates: list[list[str]], log: dict, kiwi: Kiwi) -> list[list[float]]:
         """
         A naive scoring strategy that relies on the heuristic rules.
         """
-        politeness = logs['honorify']['in']['politeness']
-        original_pairs = logs['analyze']['out'].split(SEP)
+        politeness = log['honorify']['in']['politeness']
+        original_pairs = log['analyze']['out'].split(SEP)
         if politeness == 0:
             boost_pairs = CASUAL & set(original_pairs)
         elif politeness == 1:
             boost_pairs = POLITE & set(original_pairs)
         elif politeness == 2:
             boost_pairs = FORMAL & set(original_pairs)
         else:
```

### Comparing `politely-3.3.4/politely/rules.py` & `politely-4.0.0a0/politely/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,14 @@
             CASUAL - {f"어{TAG}EF", f"어라{TAG}EF"},
             POLITE - {f"어요{TAG}EF"},
             FORMAL
         )
     }
 )
 
-
 # --- 의문형인 경우, formal은 -니까만 가능 --- #
 RULES.update(
     {
         rf"{EFS}{SEP}\?{TAG}SF": (
             CASUAL,
             POLITE,
             {f"습니까{TAG}EF", f"ᆸ니까{TAG}EF", f"시{TAG}EP{SEP}ᆸ니까{TAG}EF"}
@@ -218,25 +217,25 @@
             {f"니{TAG}EF"},
             {f"ᆫ가요{TAG}EF"},
             {f"ᆸ니까{TAG}EF"}
         )
     }
 )
 
+# --- -어요 인 경우, 란다는 사용하지 않음 --- #
+RULES.update(
+    {
+        rf"(?P<MASK>어요{TAG}EF)": (
+            CASUAL - {f"란다{TAG}EF"},
+            {"어요{TAG}EF"},
+            FORMAL
+        )
+    }
+)
 
-# # --- 으세요 -> 으십시오 --- #
-# RULES.update(
-#     {
-#         rf"(?P<MASK>으세요{TAG}EF)": (
-#             {f"어{TAG}EF"},
-#             {f"으세요{TAG}EF"},
-#             {f"ᆸ시오{TAG}EF"}
-#         )
-#     }
-# )
 
 # ---- to be used for scoring -- #
 PREFERENCES = {
     f"어{TAG}EF",
     f"어요{TAG}EF",
     f"어요{TAG}EF",
     f"습니다{TAG}EF",
```

### Comparing `politely-3.3.4/politely/styler.py` & `politely-4.0.0a0/politely/styler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 import itertools
 import re
 from copy import copy, deepcopy
-from typing import Any, Tuple, Dict, Set
 from functools import wraps
 from politely.errors import EFNotSupportedError, SFNotIncludedError, EFNotIncludedError
 from politely.fetchers import fetch_kiwi
 from politely import RULES, SEP, TAG, NULL, SELF
 from politely.modeling_gpt2_scorer import GPT2Scorer
 from politely.modeling_heuristic_scorer import HeuristicScorer
+from politely.modeling_sbg_scorer import SkipBigramScorer
 from politely.modeling_scorer import Scorer
 from politely.rules import EFS
 
 
 def log(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         # get the function signature
         f_out = f(*args, **kwargs)
         names = f.__code__.co_varnames[: f.__code__.co_argcount]
         styler_instance: Styler = args[0]
         # exclude self
-        styler_instance.log[f.__name__] = {"in": dict(zip(names[1:], args[1:])), "out": copy(styler_instance.out)}
-        return f_out # return the out
+        styler_instance.log[f.__name__] = {
+            "in": dict(zip(names[1:], args[1:])),
+            "out": copy(styler_instance.out),
+        }
+        return f_out  # return the out
+
     return wrapper
 
 
 class Styler:
     """
     A rule-based Korean Politeness Styler
     """
-    def __init__(self, strict: bool = False, scorer: str = "heuristic"):
-        #  --- object-owned attributes --- #\
+
+    def __init__(self, strict: bool = False, scorer: str = "sbg"):
+        #  --- object-owned attributes --- #
         if scorer == "heuristic":
             self.scorer: Scorer = HeuristicScorer()
+        elif scorer == "sbg":
+            self.scorer: Scorer = SkipBigramScorer()
         elif scorer == "gpt2":
             try:
                 import torch
             except ImportError:
                 raise ImportError(
-                    "torch (Pytorch) is required to use GPT2Scorer.  Please install it via `pip3 install torch`."
+                    "`torch` (Pytorch) is required to use `GPT2Scorer`. Please install it via `pip3 install torch`."
                 )
             else:
                 self.scorer: Scorer = GPT2Scorer()
         else:
-            raise ValueError(f"scorer should be either 'heuristic' or 'gpt2', but got {scorer}")
+            raise ValueError(
+                f"scorer should be either 'heuristic', `sbg` or 'gpt2', but got {scorer}"
+            )
         self.strict = strict
-        self.out: Any = None
+        self.out: any = None
         self.kiwi = fetch_kiwi()
         self.rules = deepcopy(RULES)
         self.log = dict()
 
     def __call__(self, sent: str, politeness: int) -> str:
         """
         Style a sentence with the given politeness (0, 1, 2)
         """
-        self.setup() \
-            .preprocess(sent) \
-            .analyze() \
-            .check() \
-            .honorify(politeness) \
-            .guess() \
-            .elect() \
-            .conjugate()
+        self.setup().preprocess(sent).analyze().check().honorify(
+            politeness
+        ).guess().elect().conjugate()
         return self.out
 
     def setup(self):
         """
         Reset the out and clear all the logs,
         """
         self.out = None
@@ -84,15 +88,17 @@
 
     @log
     def analyze(self):
         """
         Analyze the sentence and generate the output.
         """
         self.out: str
-        self.out = [f"{token.form}{TAG}{token.tag}" for token in self.kiwi.tokenize(self.out)]
+        self.out = [
+            f"{token.form}{TAG}{token.tag}" for token in self.kiwi.tokenize(self.out)
+        ]
         self.out = SEP.join(self.out)  # to match with the format of the rules
         return self
 
     def check(self):
         """
         Check if your assumption holds. Raises a custom error if any of them does not hold.
         """
@@ -102,15 +108,17 @@
             # assumption 1: every sentence should end with a valid SF. It should be one of: (., !, ?)
             if "SF" not in self.out:
                 raise SFNotIncludedError(self.out)
             # assumption 2: every sentence should include a valid EF. It should match the EFS pattern.
             if "EF" not in self.out:
                 raise EFNotIncludedError(self.out)
             # assumption 3: all EF's should be supported by politely.
-            if not all([re.match(EFS, pair) for pair in self.out.split(SEP) if "EF" in pair]):
+            if not all(
+                [re.match(EFS, pair) for pair in self.out.split(SEP) if "EF" in pair]
+            ):
                 raise EFNotSupportedError(self.out)
         return self
 
     @log
     def honorify(self, politeness: int):
         """
         Determines all the candidates that would properly honorify the sentence.
@@ -119,46 +127,55 @@
         self.out: str
         pair2honorifics = {}
         for pattern in self.rules.keys():
             match = re.search(pattern, self.out)
             if match:
                 # should be only one pair
                 pair = match.group("MASK")
-                honorifics = {honorific.replace(SELF, pair) for honorific in self.rules[pattern][politeness]}
+                honorifics = {
+                    honorific.replace(SELF, pair)
+                    for honorific in self.rules[pattern][politeness]
+                }
                 # progressively narrow down honorifics
-                pair2honorifics[pair] = pair2honorifics.get(pair, honorifics) & honorifics
+                pair2honorifics[pair] = (
+                    pair2honorifics.get(pair, honorifics) & honorifics
+                )
         # get all possible candidates
-        candidates = itertools.product(*[
-            pair2honorifics.get(pair, {pair, })
-            for pair in self.out.split(SEP)  # SEP
-        ])
+        candidates = itertools.product(
+            *[
+                pair2honorifics.get(
+                    pair,
+                    {
+                        pair,
+                    },
+                )
+                for pair in self.out.split(SEP)  # SEP
+            ]
+        )
         # remove empty candidates
         candidates = [
             [pair.split(SEP) for pair in candidate if pair != NULL]
             for candidate in candidates
         ]
         # flatten pairs
-        candidates = [
-            list(itertools.chain(*candidate))
-            for candidate in candidates
-        ]
+        candidates = [list(itertools.chain(*candidate)) for candidate in candidates]
         # a list of candidates
         self.out = candidates
         return self
 
     @log
     def guess(self):
         """
         Guess the scores.
         """
         self.out: list[list[str]]
-        scores = self.scorer(self.out, self.log, self.kiwi)
+        scores = self.scorer(candidates=self.out, log=self.log, kiwi=self.kiwi)
         self.out = [(candidate, score) for candidate, score in zip(self.out, scores)]
         return self
-    
+
     @log
     def elect(self):
         """
         Elect the best candidate.
         """
         self.out: list[tuple[list[str], float]]
         best = max(self.out, key=lambda x: x[1])
@@ -168,25 +185,26 @@
     @log
     def conjugate(self):
         """
         conjugate the best candidate.
         """
         self.out: tuple[list[str], float]
         sent = self.out[0]
-        self.out = self.kiwi.join([(pair.split(TAG)[0], pair.split(TAG)[1]) for pair in sent])
+        self.out = self.kiwi.join(
+            [(pair.split(TAG)[0], pair.split(TAG)[1]) for pair in sent]
+        )
         return self
 
-    def add_rules(self, rules: Dict[str, Tuple[Set,
-                                               Set,
-                                               Set]]):
+    def add_rules(self, rules: dict[str, tuple[set, set, set]]):
         """
         Add rules to the existing rules.
         """
         # check if the rules are in proper format
         for key, _ in rules.items():
             # first, check if the key includes a group with the key; (?<MASK>...)
             # e.g. (?P<MASK>(아빠|아버지){TAG}NNG)
             if not re.search(re.escape(r"(?P<MASK>") + r".*" + re.escape(")"), key):
-                raise ValueError(f"key should include a group with the key; (?P<MASK>...), but got {key}")
+                raise ValueError(
+                    f"key should include a group with the key; (?P<MASK>...), but got {key}"
+                )
         self.rules.update(rules)
         return self
-
```

### Comparing `politely-3.3.4/PKG-INFO` & `politely-4.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politely
-Version: 3.3.4
+Version: 4.0.0a0
 Summary: An explainable styler for the Korean language
 Author: Eu-Bin KIM
 Author-email: tlrndk123@gmail.com
 Requires-Python: >=3.9.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,14 @@
 Requires-Dist: kiwipiepy (>=0.17.0,<0.18.0)
 Requires-Dist: transformers (>=4.39.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
-![Workflow status](https://github.com/eubinecto/politely/actions/workflows/tests.yml/badge.svg)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://politely.streamlit.app)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Feubinecto%2Fpolitely&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Downloads](https://pepy.tech/badge/politely)](https://pepy.tech/project/politely)
 [![Downloads](https://pepy.tech/badge/politely/week)](https://pepy.tech/project/politely)
```

