# Comparing `tmp/zhixuewang-1.2.5-py3-none-any.whl.zip` & `tmp/zhixuewang-1.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 22004 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      618 b- defN 23-Dec-09 15:06 zhixuewang/__init__.py
+Zip file size: 22042 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat      617 b- defN 24-Apr-05 14:07 zhixuewang/__init__.py
 -rw-rw-rw-  2.0 fat     5015 b- defN 23-Oct-05 01:21 zhixuewang/account.py
 -rw-rw-rw-  2.0 fat      941 b- defN 23-Oct-05 01:21 zhixuewang/exceptions.py
 -rw-rw-rw-  2.0 fat     8837 b- defN 23-Oct-06 11:45 zhixuewang/models.py
 -rw-rw-rw-  2.0 fat     4578 b- defN 23-Dec-09 15:07 zhixuewang/session.py
 -rw-rw-rw-  2.0 fat      377 b- defN 23-Oct-05 01:21 zhixuewang/urls.py
 -rw-rw-rw-  2.0 fat       87 b- defN 23-Jul-06 13:22 zhixuewang/student/__init__.py
--rw-rw-rw-  2.0 fat    26022 b- defN 23-Oct-08 14:27 zhixuewang/student/student.py
+-rw-rw-rw-  2.0 fat    26124 b- defN 24-Apr-05 14:06 zhixuewang/student/student.py
 -rw-rw-rw-  2.0 fat     2056 b- defN 23-Oct-08 14:27 zhixuewang/student/urls.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Oct-05 01:21 zhixuewang/teacher/__init__.py
 -rw-rw-rw-  2.0 fat     1390 b- defN 23-Oct-06 11:43 zhixuewang/teacher/models.py
--rw-rw-rw-  2.0 fat    13573 b- defN 23-Oct-06 11:47 zhixuewang/teacher/teacher.py
+-rw-rw-rw-  2.0 fat    13633 b- defN 24-Apr-05 14:06 zhixuewang/teacher/teacher.py
 -rw-rw-rw-  2.0 fat     1357 b- defN 23-Oct-05 02:06 zhixuewang/teacher/urls.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Oct-05 01:21 zhixuewang/tools/__init__.py
 -rw-rw-rw-  2.0 fat      433 b- defN 20-Aug-05 14:04 zhixuewang/tools/datetime_tool.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Dec-09 15:07 zhixuewang-1.2.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      280 b- defN 23-Dec-09 15:07 zhixuewang-1.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-09 15:07 zhixuewang-1.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Dec-09 15:07 zhixuewang-1.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1632 b- defN 23-Dec-09 15:07 zhixuewang-1.2.5.dist-info/RECORD
-20 files, 68578 bytes uncompressed, 19344 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      280 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1632 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/RECORD
+20 files, 68739 bytes uncompressed, 19382 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: zhixuewang/tools/__init__.py
 Comment: 
 
 Filename: zhixuewang/tools/datetime_tool.py
 Comment: 
 
-Filename: zhixuewang-1.2.5.dist-info/LICENSE
+Filename: zhixuewang-1.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: zhixuewang-1.2.5.dist-info/METADATA
+Filename: zhixuewang-1.2.6.dist-info/METADATA
 Comment: 
 
-Filename: zhixuewang-1.2.5.dist-info/WHEEL
+Filename: zhixuewang-1.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: zhixuewang-1.2.5.dist-info/top_level.txt
+Filename: zhixuewang-1.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: zhixuewang-1.2.5.dist-info/RECORD
+Filename: zhixuewang-1.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhixuewang/__init__.py

```diff
@@ -1,10 +1,10 @@
 __author__ = "anwenhu,MasterYuan418,immoses648"
-__date__ = "2023/12/9 23:10"
-__version__ = "1.2.5"
+__date__ = "2024/4/5 22:10"
+__version__ = "1.2.6"
 
 from zhixuewang.account import (login, login_id, rewrite_str, login_student, login_teacher,
                                 login_student_id, login_teacher_id, load_account)
 from zhixuewang.session import get_session, get_session_id
 
 VERSION = tuple(map(int, __version__.split('.')))
 __all__ = [
```

## zhixuewang/student/student.py

```diff
@@ -52,14 +52,18 @@
         # self._token_timestamp = ["", 0]
         self._auth = {
             "token": "",
             "timestamp": 0.0
         }
         self.exams: ExtendedList[Exam] = ExtendedList()
 
+    def get_session(self):
+        '''获得学生端Session'''
+        return self._session
+    
     def get_auth_header(self) -> dict:
         """获取header"""
         self.update_login_status()
         auth_guid = str(uuid.uuid4())
         auth_time_stamp = str(int(time.time() * 1000))
         auth_token = _md5_encode(auth_guid + auth_time_stamp + "iflytek!@#123student")
         token, cur_time = self._auth["token"], self._auth["timestamp"]
```

## zhixuewang/teacher/teacher.py

```diff
@@ -37,16 +37,16 @@
             headers={
                 "referer": "https://www.zhixue.com/paperfresh/dist/assets/expertPaper.html"
             },
         )
         if r.status_code != 200:
             return self
         data = r.json()["result"]
-        self.province = data["province"]["name"]
-        self.city = data["city"]["name"]
+        self.province = data["province"]["name"] if data["province"] else None
+        self.city = data["city"]["name"] if data["city"] else None
         if data["school"]:
             self.school = School(
                 name=data["school"]["name"], id=data["school"]["id"]
             )
         if data["curSubject"]:
             self.subject = Subject(
                 data["curSubject"]["name"], code=data["curSubject"]["code"]
@@ -86,15 +86,15 @@
                 "referer": "https://www.zhixue.com/container/container/teacher/index/"
             },
         )
         json_data = r.json()["teacher"]
         self.id = json_data.get("id")
         self.mobile = json_data.get("mobile")
         self.name = json_data.get("name")
-        self.roles = json_data["roles"]
+        self.roles = json_data.get("roles")
         return self
 
     def get_school_exam_classes(
         self, school_id: str, topic_set_id: str
     ) -> List[StuClass]:
         self.update_login_status()
         r = self._session.get(
```

## Comparing `zhixuewang-1.2.5.dist-info/LICENSE` & `zhixuewang-1.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zhixuewang-1.2.5.dist-info/RECORD` & `zhixuewang-1.2.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-zhixuewang/__init__.py,sha256=3XWyyM4DdZ1V19uJ8OMLl8zg6fETtLTnfRkrEvBMM2o,618
+zhixuewang/__init__.py,sha256=z-zYJ5qQQrB8xDpnIK2K1tCHiR9163xNUFe9L6CpXZA,617
 zhixuewang/account.py,sha256=3VKn7kYy5Ytw2JGWp8Bapaic-W8qCJY_5gDUTmLkNbQ,5015
 zhixuewang/exceptions.py,sha256=p_mnjq_FIZIwzks3QZsk5xKdGL7Dbbcsdf-OtvoRbVk,941
 zhixuewang/models.py,sha256=gneTnzGhUsUX1WIuDKD1rFgYjT81x4K-oGwwNx-1eb4,8837
 zhixuewang/session.py,sha256=Jp5qX379TqFCCSZvRrNN1ZUOub8cGTojzVgQ006hb_M,4578
 zhixuewang/urls.py,sha256=JzGiCpbgnLximLXPFBeoTJgCcZoNbceZcyPVv4_-I_o,377
 zhixuewang/student/__init__.py,sha256=1hZ_-EeFM4l7wF8D56jIMigTQ5b7o7sCCTR9_YRjsj0,87
-zhixuewang/student/student.py,sha256=elcI0v9tdcIPBBvV0dNXDwv9YMXfMUVkhgBup_iWxos,26022
+zhixuewang/student/student.py,sha256=QVyHb5iHZV9_fCoOqMu2tbbbPlE3WliQ5CanAOsc-f8,26124
 zhixuewang/student/urls.py,sha256=92qXQSUzVC-IZSs1-I7eCdjjJnBgTPgzEdwon0ybyy8,2056
 zhixuewang/teacher/__init__.py,sha256=HQ02UJM7lhCgtamRCYcSuFOUTA_cWXNV2jyc9a_q4Sc,98
 zhixuewang/teacher/models.py,sha256=R8c7zljypjGOTYW60A6zss0h01xVslkoMHhk5SW_UJo,1390
-zhixuewang/teacher/teacher.py,sha256=Dy8Jl2YWHlpHKwCx2B0ouP2A8DjUjsA7e1Blo7gbb7o,13573
+zhixuewang/teacher/teacher.py,sha256=Uso50QkKDUd7vNX35supGXheOPlshs4lpmBUeobNxJg,13633
 zhixuewang/teacher/urls.py,sha256=sAZpTI4ajOoTdvimVEq0OyiHuf80D-EJi_-09YzzmuQ,1357
 zhixuewang/tools/__init__.py,sha256=apzJbuBykdNmJaeellyr4NRPtAqCtSjMFuevsMEudkM,96
 zhixuewang/tools/datetime_tool.py,sha256=mCsCA0TK27ku4GCQY7ghyruhAeIeN6360jSZZ3XQNqw,433
-zhixuewang-1.2.5.dist-info/LICENSE,sha256=xfB-JOtu13adc_d9NLglK9fKvZZlHEDoKKpYliTvaQA,1085
-zhixuewang-1.2.5.dist-info/METADATA,sha256=H0AecEgltxxiGsUTgC7X8inbgSQP0qUTB_H-1qDtxYM,280
-zhixuewang-1.2.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zhixuewang-1.2.5.dist-info/top_level.txt,sha256=ufrDrdhelpFTIliZw7eEvOtIK_zyIv4UssZNpQqV-Jw,11
-zhixuewang-1.2.5.dist-info/RECORD,,
+zhixuewang-1.2.6.dist-info/LICENSE,sha256=xfB-JOtu13adc_d9NLglK9fKvZZlHEDoKKpYliTvaQA,1085
+zhixuewang-1.2.6.dist-info/METADATA,sha256=4FbJMvYqr8gVW2N092e-jSk5oEuG2f9y-6eK2cvgHQ8,280
+zhixuewang-1.2.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zhixuewang-1.2.6.dist-info/top_level.txt,sha256=ufrDrdhelpFTIliZw7eEvOtIK_zyIv4UssZNpQqV-Jw,11
+zhixuewang-1.2.6.dist-info/RECORD,,
```

