# Comparing `tmp/django_login_email-0.2.0.tar.gz` & `tmp/django_login_email-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_login_email-0.2.0.tar", max compression
+gzip compressed data, was "django_login_email-0.3.0.tar", max compression
```

## Comparing `django_login_email-0.2.0.tar` & `django_login_email-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.2.0/django_login_email/__init__.py
--rw-r--r--   0        0        0       66 2024-04-04 13:03:53.315517 django_login_email-0.2.0/django_login_email/admin.py
--rw-r--r--   0        0        0      172 2024-04-04 13:48:39.145418 django_login_email-0.2.0/django_login_email/apps.py
--rw-r--r--   0        0        0     2023 2024-04-05 07:09:02.784147 django_login_email-0.2.0/django_login_email/email.py
--rw-r--r--   0        0        0       48 2024-04-04 14:10:43.064298 django_login_email-0.2.0/django_login_email/errors.py
--rw-r--r--   0        0        0      148 2024-04-04 13:39:37.730372 django_login_email-0.2.0/django_login_email/forms.py
--rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.2.0/django_login_email/migrations/__init__.py
--rw-r--r--   0        0        0      511 2024-04-05 06:58:54.154438 django_login_email-0.2.0/django_login_email/models.py
--rw-r--r--   0        0        0      262 2024-04-04 13:13:26.017612 django_login_email-0.2.0/django_login_email/templates/login_email/base.html
--rw-r--r--   0        0        0        0 2024-04-05 07:10:27.427724 django_login_email-0.2.0/django_login_email/templates/login_email/components/mail_template.html
--rw-r--r--   0        0        0      264 2024-04-04 13:28:15.565466 django_login_email-0.2.0/django_login_email/templates/login_email/error.html
--rw-r--r--   0        0        0      303 2024-04-05 02:52:27.902145 django_login_email-0.2.0/django_login_email/templates/login_email/home.html
--rw-r--r--   0        0        0      262 2024-04-04 13:14:07.688691 django_login_email-0.2.0/django_login_email/templates/login_email/login.html
--rw-r--r--   0        0        0      166 2024-04-04 13:14:54.572437 django_login_email-0.2.0/django_login_email/templates/login_email/success.html
--rw-r--r--   0        0        0        0 2024-04-05 02:35:09.498191 django_login_email-0.2.0/django_login_email/tests/__init__.py
--rw-r--r--   0        0        0       85 2024-04-05 02:38:19.911927 django_login_email-0.2.0/django_login_email/tests/test_str.py
--rw-r--r--   0        0        0      130 2024-04-05 06:52:23.110227 django_login_email-0.2.0/django_login_email/tests/test_time.py
--rw-r--r--   0        0        0       63 2024-04-04 13:03:53.315517 django_login_email-0.2.0/django_login_email/tests.py
--rw-r--r--   0        0        0     2478 2024-04-05 07:08:57.343034 django_login_email-0.2.0/django_login_email/token.py
--rw-r--r--   0        0        0     2546 2024-04-05 07:08:11.008205 django_login_email-0.2.0/django_login_email/views.py
--rw-r--r--   0        0        0     1270 2024-04-04 14:30:21.236968 django_login_email-0.2.0/LICENSE
--rw-r--r--   0        0        0      732 2024-04-05 07:10:56.127496 django_login_email-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      738 2024-04-05 07:10:41.402112 django_login_email-0.2.0/README.md
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 django_login_email-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.3.0/django_login_email/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-04 13:03:53.315517 django_login_email-0.3.0/django_login_email/admin.py
+-rw-r--r--   0        0        0      172 2024-04-04 13:48:39.145418 django_login_email-0.3.0/django_login_email/apps.py
+-rw-r--r--   0        0        0     3280 2024-04-05 09:03:42.714709 django_login_email-0.3.0/django_login_email/email.py
+-rw-r--r--   0        0        0       48 2024-04-04 14:10:43.064298 django_login_email-0.3.0/django_login_email/errors.py
+-rw-r--r--   0        0        0      148 2024-04-04 13:39:37.730372 django_login_email-0.3.0/django_login_email/forms.py
+-rw-r--r--   0        0        0      651 2024-04-05 07:43:16.485657 django_login_email-0.3.0/django_login_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:03:53.331270 django_login_email-0.3.0/django_login_email/migrations/__init__.py
+-rw-r--r--   0        0        0      644 2024-04-05 08:49:30.577058 django_login_email-0.3.0/django_login_email/models.py
+-rw-r--r--   0        0        0      262 2024-04-04 13:13:26.017612 django_login_email-0.3.0/django_login_email/templates/login_email/base.html
+-rw-r--r--   0        0        0        0 2024-04-05 07:10:27.427724 django_login_email-0.3.0/django_login_email/templates/login_email/components/mail_template.html
+-rw-r--r--   0        0        0      264 2024-04-04 13:28:15.565466 django_login_email-0.3.0/django_login_email/templates/login_email/error.html
+-rw-r--r--   0        0        0      303 2024-04-05 02:52:27.902145 django_login_email-0.3.0/django_login_email/templates/login_email/home.html
+-rw-r--r--   0        0        0      262 2024-04-04 13:14:07.688691 django_login_email-0.3.0/django_login_email/templates/login_email/login.html
+-rw-r--r--   0        0        0      166 2024-04-04 13:14:54.572437 django_login_email-0.3.0/django_login_email/templates/login_email/success.html
+-rw-r--r--   0        0        0        0 2024-04-05 02:35:09.498191 django_login_email-0.3.0/django_login_email/tests/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-05 09:03:29.344879 django_login_email-0.3.0/django_login_email/tests/test_mixin.py
+-rw-r--r--   0        0        0      455 2024-04-05 07:41:19.183970 django_login_email-0.3.0/django_login_email/tests/test_models.py
+-rw-r--r--   0        0        0       85 2024-04-05 02:38:19.911927 django_login_email-0.3.0/django_login_email/tests/test_str.py
+-rw-r--r--   0        0        0      130 2024-04-05 06:52:23.110227 django_login_email-0.3.0/django_login_email/tests/test_time.py
+-rw-r--r--   0        0        0       63 2024-04-04 13:03:53.315517 django_login_email-0.3.0/django_login_email/tests.py
+-rw-r--r--   0        0        0     2595 2024-04-05 07:28:51.167000 django_login_email-0.3.0/django_login_email/token.py
+-rw-r--r--   0        0        0     3599 2024-04-05 09:06:32.403242 django_login_email-0.3.0/django_login_email/views.py
+-rw-r--r--   0        0        0     1270 2024-04-04 14:30:21.236968 django_login_email-0.3.0/LICENSE
+-rw-r--r--   0        0        0      854 2024-04-05 09:08:51.152655 django_login_email-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      769 2024-04-05 09:07:23.790007 django_login_email-0.3.0/README.md
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 django_login_email-0.3.0/PKG-INFO
```

### Comparing `django_login_email-0.2.0/django_login_email/token.py` & `django_login_email-0.3.0/django_login_email/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 EmailAndSalt = str
 Email = str
 
 TokenDict = t.TypedDict("TokenDict", {"email": Email, "expire_time": int, "salt": str})
 
 
 class TokenGenerator(object):
-    minutes: int = 10
+    def __init__(self, minutes: int) -> None:
+        self.minutes = minutes
 
     def get_expire_time(self) -> int:
         return int((datetime.datetime.now() + datetime.timedelta(minutes=self.minutes)).timestamp())
 
     def gen(self, email, salt):
         return json.dumps(
             {
@@ -30,18 +31,19 @@
             }
         )
 
 
 class TokenManager(object):
     salt: str = "randomsalt"
     key: bytes
-    generator: TokenGenerator = TokenGenerator()
+    generator: TokenGenerator
 
-    def __init__(self) -> None:
+    def __init__(self, minutes: int) -> None:
         self.key = settings.SECRET_KEY[:32].encode("utf-8")
+        self.generator: TokenGenerator = TokenGenerator(minutes)
 
     def check_token(self, token_uncrypt: str) -> t.Optional[TokenDict]:
         """check salt and expire-time"""
         token_dict: TokenDict = json.loads(token_uncrypt)
         if token_dict["salt"] == self.salt and token_dict["expire_time"] > int(datetime.datetime.now().timestamp()):
             return token_dict
         return None
```

### Comparing `django_login_email-0.2.0/django_login_email/views.py` & `django_login_email-0.3.0/django_login_email/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,72 @@
+import datetime
 from typing import Any
 from django.http import Http404, HttpRequest, HttpResponse
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.views.generic.edit import FormView
 from django.views.generic import TemplateView
 from django.contrib.auth import get_user_model
 from . import forms
 from . import email
-from . import token
+from . import models
 
 # Create your views here.
 
-m = token.TokenManager()
 
+class TimeLimit(email.TimeLimit):
+    minutes = 10
 
-class EmailLoginView(FormView, email.EmailInfoMixin):
+
+class MailRecordModelMixin(email.EmailInfoMixin):
+    """Here is an example for MailRecord, using django model. You could implement yourself."""
+
+    def set_mail_record(self, mail: str):
+        models.EmailLogin.set_email_last_time(mail, datetime.datetime.now(tz=datetime.timezone.utc))
+
+    def reset_mail(self, mail: str):
+        # models.EmailLogin.objects.filter(email=mail).delete()
+        e = models.EmailLogin.objects.get(email=mail)
+        e.last_time = e.last_time - datetime.timedelta(minutes=self.tl.minutes)
+        e.save()
+
+    def get_mail_record(self, mail: str) -> email.MailRecord:
+        # for easy to change. use a function.
+        try:
+            e = models.EmailLogin.objects.get(email=mail)
+        except models.EmailLogin.DoesNotExist:
+            return email.MailRecord(email=mail, last_time=None)
+        return email.MailRecord(email=e.email, last_time=e.last_time)
+
+
+class EmailLoginView(FormView, MailRecordModelMixin):
     template_name = "login_email/login.html"
     form_class = forms.LoginForm
     email_info_class = email.EmailLoginInfo
+    tl = TimeLimit()
 
     def form_valid(self, form):
         """check the email"""
         User = get_user_model()
         try:
             self.send_login_mail(form.cleaned_data["email"])
         except User.DoesNotExist as e:
             # ignore user missing problem.
             print(e, form.cleaned_data["email"])
             return render(self.request, "login_email/success.html", {"form": form})
         except Exception as e:
+            # raise Exception(e)
             print(e)
             return render(self.request, "login_email/error.html", {"error": e})
         return render(self.request, "login_email/success.html", {"form": form})
 
 
 class EmailVerifyView(TemplateView, email.EmailValidateMixin):
+    tl = TimeLimit()
+
     def post(self, request: HttpRequest, *args: str, **kwargs: Any) -> HttpResponse:
         raise Http404("Invalid Request.")
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         token = request.GET.get("token", None)
         if token is None:
             raise Http404("Invalid Request")
```

### Comparing `django_login_email-0.2.0/LICENSE` & `django_login_email-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_login_email-0.2.0/pyproject.toml` & `django_login_email-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [tool.poetry]
 name = "django-login-email"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["svtter <svtter@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 django = "^5.0.4"
 pycryptodome = "^3.20.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
+pytest-django = "^4.8.0"
+psycopg2 = "^2.9.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 homepage = "https://github.com/Svtter/django-login-email"
 repository = "https://github.com/Svtter/django-login-email.git"
 changelog = "https://github.com/Svtter/django-login-email/blob/master/CHANGELOG.md"
 bugs = "https://github.com/Svtter/django-login-email/issues"
-# sponsor = "https://github.com/sponsors/svtter"
+# sponsor = "https://github.com/sponsors/svtter"
+
+[tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "settings.settings"
```

### Comparing `django_login_email-0.2.0/README.md` & `django_login_email-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - `/account/logout` for logout.
 - `/account/verify` for email verify.
 
 ## Feature
 
 - [x] The developer could define their own `User` model.
 - [x] Time-limited of login link.
-- [ ] limited of sending email.
+- [x] limited of sending email. Using TimeLimt to set minutes.
 - [ ] More easier and customizable login link.
 
 ## Future
 
 - Academically prove the safety of this method.
 
 ## Related project
```

### Comparing `django_login_email-0.2.0/PKG-INFO` & `django_login_email-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-login-email
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: svtter
 Author-email: svtter@qq.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,15 +31,15 @@
 - `/account/logout` for logout.
 - `/account/verify` for email verify.
 
 ## Feature
 
 - [x] The developer could define their own `User` model.
 - [x] Time-limited of login link.
-- [ ] limited of sending email.
+- [x] limited of sending email. Using TimeLimt to set minutes.
 - [ ] More easier and customizable login link.
 
 ## Future
 
 - Academically prove the safety of this method.
 
 ## Related project
```

