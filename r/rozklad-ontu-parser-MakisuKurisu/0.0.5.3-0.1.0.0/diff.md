# Comparing `tmp/rozklad_ontu_parser_makisukurisu-0.0.5.3.tar.gz` & `tmp/rozklad_ontu_parser_makisukurisu-0.1.0.0.tar.gz`

## Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3.tar` & `rozklad_ontu_parser_makisukurisu-0.1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/run_lint.bat
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/run_lint.sh
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/example.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/base.py
--rw-r--r--   0        0        0    21272 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/dataclasses.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/enums.py
--rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/parser.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/sender.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/LICENSE
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/readme.md
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/run_lint.bat
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/run_lint.sh
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/__init__.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/base.py
+-rw-r--r--   0        0        0    21447 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/dataclasses.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/enums.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/js_parser.py
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/parser.py
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/sender.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/LICENSE
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/readme.md
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.1.0.0/PKG-INFO
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/.github/ISSUE_TEMPLATE/feature_request.md` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/.github/workflows/pylint.yml` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/.github/workflows/pylint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.11", "3.12"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install pylint
         pip install -r requirements.txt
     - name: Analysing the code with pylint
       run: |
-        pylint ontu_parser --disable=R0903
+        pylint ontu_parser --disable=R0903,W1203
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/.github/workflows/python-publish.yml` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/example.py` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/example.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,31 +5,26 @@
 
 # To test Library from source code, use this import:
 
 # from classes import Parser
 
 # An example of how to pass arguments to Firefox browser created by selenium
 # Add arguments inside 'browser_settings' and see what happens
-parser = Parser(
-    kwargs={
-        'notbot': {
-            'browser_settings': {
-            }
-        }
-    }
-)
+parser = Parser()
 
-schedule = parser.parse(all_time=True)
+schedule = parser.parse(all_time=False)
 for day_name, pairs in schedule.items():
-    print(f'{day_name}:\n')
+    print(f"{day_name}:\n")
     for pair in pairs:
         if not pair.lessons:
             continue
-        print(f'{pair.pair_no}:')
+        print(f"{pair.pair_no}:")
         for lesson in pair.lessons:
             print(
                 f'{lesson.lesson_date}: '
                 f'{lesson.teacher["short"]} - '
                 f'{lesson.lesson_name["short"]}'
-                f' - In auditorium: {lesson.auditorium}' if lesson.auditorium else ''
+                f' - In auditorium: {lesson.auditorium}'
+                if lesson.auditorium
+                else ""
             )
-            print(f'Card: {lesson.lesson_info}\n')
+            print(f"Card: {lesson.lesson_info}\n")
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/base.py` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/base.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/dataclasses.py` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
     Contains classes needed to get data
     Like Faculty or Group, provides methods to get names, ids, etc.
 """
 from urllib.parse import parse_qsl
-from attrs import define
 
+from attrs import define
 from bs4.element import Tag
 
-from .base import BaseClass
+from ontu_parser.classes.base import BaseClass
 
 
 class BaseTag(BaseClass):
     """Base Tag Class for parsing BS4 tags from responses"""
 
     @classmethod
     def from_tag(cls, tag):
@@ -392,15 +392,17 @@
             pair_tags.pop()
         return day_name, pair_tags
 
     def _prepare_tags(self, tags):
         """Parses bs4 tags to list of Pair objects"""
         prepared_tags: list[StudentsPair] = []
         for tag in tags:
-            prepared_tags.append(StudentsPair.from_tag(tag, subgroup_id=self.subgroup_id))
+            prepared_tags.append(
+                StudentsPair.from_tag(tag, subgroup_id=self.subgroup_id)
+            )
         return prepared_tags
 
     def _get_week(self):
         """Iteratively loops trough table to get data for all days"""
         table_body = self.schedule_tag.tbody
         days = table_body.find_all(attrs={"class": "day"})
         for day in days:
@@ -442,15 +444,17 @@
 
     @staticmethod
     def _check_tag(tag: Tag):
         pass
 
     def parse_tag(self):
         """This method parses bs4 and stores data from it in object's fields"""
-        pair_no_text = self.pair_tag.attrs.get("data-title-caption", self.__pair_no_not_specified)
+        pair_no_text = self.pair_tag.attrs.get(
+            "data-title-caption", self.__pair_no_not_specified
+        )
         if pair_no_text != self.__pair_no_not_specified:
             self.pair_no = int(pair_no_text.split()[0])
         else:
             self.pair_no = 0
 
         pair_name_tag = self.pair_tag.find(name="p", attrs={"class": "text-leader"})
         pair_name = pair_name_tag.text.strip() if pair_name_tag else None
@@ -570,22 +574,26 @@
         """Return id of the department"""
         key_dict = dict(parse_qsl(self.get_department_link()))
         return int(key_dict["dep"])
 
     def get_department_name(self) -> dict[str, str]:
         """Returns name of the faculty"""
         name = {"short": "", "full": ""}
-        short_name_span = self.department.find(name="span", attrs={"class": "branding-bar"})
+        short_name_span = self.department.find(
+            name="span", attrs={"class": "branding-bar"}
+        )
         full_name_span = self.department.find(name="div", attrs={"class": "slide-back"})
         name["short"] = short_name_span.text.strip() if short_name_span else ""
         full_name = full_name_span.text.strip() if full_name_span else ""
         name["full"] = full_name
         if full_name:
             words = full_name.split()
-            name["full"] = " ".join([x.capitalize() if len(x) > 2 else x for x in words])
+            name["full"] = " ".join(
+                [x.capitalize() if len(x) > 2 else x for x in words]
+            )
         return name
 
 
 @define
 class Teacher(BaseTag):
     """Describes teacher from BS4 tag"""
 
@@ -636,16 +644,20 @@
         """Return id of teacher"""
         key_dict = dict(parse_qsl(self.get_teacher_link()))
         return int(key_dict["teacher"])
 
     def get_teacher_name(self) -> dict[str, str]:
         """Returns name of the faculty"""
         name = {"short": "", "full": ""}
-        short_name_span = self.teacher.find(name="span", attrs={"class": "branding-bar"})
+        short_name_span = self.teacher.find(
+            name="span", attrs={"class": "branding-bar"}
+        )
         full_name_span = self.teacher.find(name="div", attrs={"class": "slide-back"})
         name["short"] = short_name_span.text.strip() if short_name_span else ""
         full_name = full_name_span.text.strip() if full_name_span else ""
         name["full"] = full_name
         if full_name:
             words = full_name.split()
-            name["full"] = " ".join([x.capitalize() if len(x) > 2 else x for x in words])
+            name["full"] = " ".join(
+                [x.capitalize() if len(x) > 2 else x for x in words]
+            )
         return name
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/enums.py` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """Enumerators"""
-from enum import Enum
+from enum import Enum, StrEnum
 
 
 class RequestsEnum:
     """Contains information for Requests library"""
 
-    class Methods(Enum):
+    class Methods(StrEnum):
         """Contains used HTTP Methods for requests"""
 
         GET = "GET"
         POST = "POST"
 
-        CHOICES = [GET, POST]
+        @classmethod
+        def choices(cls):
+            """Returns list of available choices
+
+            Returns:
+                list[str]: list of available choices
+            """
+            return [cls.GET.value, cls.POST.value]
 
     class Codes(Enum):
         """Contains used HTTP response codes"""
 
         OK = 200
+        SERVICE_UNAVAILABLE = 503
 
     @classmethod
     def code_ok(cls):
         """
         OK code
 
         Returns:
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/ontu_parser/classes/parser.py` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/ontu_parser/classes/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for parser class"""
-from requests import Response
 from bs4 import BeautifulSoup
+from requests import Response
 
 from .base import BaseClass
+from .dataclasses import (Department, Faculty, Group, StudentsSchedule,
+                          Teacher, TeacherSchedule)
 from .enums import RequestsEnum
-from .dataclasses import Faculty, Group, StudentsSchedule, Department, Teacher, TeacherSchedule
 from .sender import Sender
 
 
 class Parser(BaseClass):
     """Parser class to get information from Rozklad ONTU"""
 
     sender: Sender = None
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/LICENSE` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/pyproject.toml` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rozklad_ontu_parser_MakisuKurisu"
-version = "0.0.5.3"
+version = "0.1.0.0"
 authors = [
   {  name="Pavlo Pohorieltsev", email="667strets@gmail.com"  },
 ]
 description = "Package for parsing data from rozklad.ontu.edu.ua"
 readme = "readme.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
 ]
 dynamic = ["dependencies"]
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/readme.md` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.5.3/PKG-INFO` & `rozklad_ontu_parser_makisukurisu-0.1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rozklad_ontu_parser_MakisuKurisu
-Version: 0.0.5.3
+Version: 0.1.0.0
 Summary: Package for parsing data from rozklad.ontu.edu.ua
 Project-URL: Homepage, https://github.com/makisukurisu/rozklad-ontu-parser
 Project-URL: Bug Tracker, https://github.com/makisukurisu/rozklad-ontu-parser/issues
 Author-email: Pavlo Pohorieltsev <667strets@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Requires-Dist: attrs>=22.1.0
-Requires-Dist: beautifulsoup4>=4.11.1
-Requires-Dist: requests>=2.28.1
-Requires-Dist: selenium>=4.4.3
+Requires-Python: >=3.11
+Requires-Dist: attrs<24.0.0,>=23.2.0
+Requires-Dist: beautifulsoup4<5.0.0,>=4.12.3
+Requires-Dist: requests<3.0.0,>=2.31.0
 Description-Content-Type: text/markdown
 
 # Rozklad ONTU Pareser [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 Library on [PyPi](https://pypi.org/project/rozklad-ontu-parser-MakisuKurisu/)
 
 Installation: `pip install rozklad-ontu-parser-MakisuKurisu`
```

