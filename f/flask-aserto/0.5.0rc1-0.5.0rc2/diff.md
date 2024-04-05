# Comparing `tmp/flask-aserto-0.5.0rc1.tar.gz` & `tmp/flask-aserto-0.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-aserto-0.5.0rc1.tar", max compression
+gzip compressed data, was "flask-aserto-0.5.0rc2.tar", max compression
```

## Comparing `flask-aserto-0.5.0rc1.tar` & `flask-aserto-0.5.0rc2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1414 2022-02-03 23:43:06.664822 flask-aserto-0.5.0rc1/README.md
--rw-r--r--   0        0        0     2354 2022-10-20 16:42:12.913626 flask-aserto-0.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7359 2022-10-19 21:20:08.057786 flask-aserto-0.5.0rc1/src/flask_aserto/__init__.py
--rw-r--r--   0        0        0     1293 2022-10-18 20:41:06.191822 flask-aserto-0.5.0rc1/src/flask_aserto/_defaults.py
--rw-r--r--   0        0        0      394 2022-02-03 23:43:06.666409 flask-aserto-0.5.0rc1/src/flask_aserto/_maybe_async.py
--rw-r--r--   0        0        0        0 2022-02-03 23:43:06.666457 flask-aserto-0.5.0rc1/src/flask_aserto/py.typed
--rw-r--r--   0        0        0     2377 2022-10-20 16:42:21.010889 flask-aserto-0.5.0rc1/setup.py
--rw-r--r--   0        0        0     2848 2022-10-20 16:42:21.011116 flask-aserto-0.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1414 2022-02-03 23:43:06.664822 flask-aserto-0.5.0rc2/README.md
+-rw-r--r--   0        0        0     2354 2022-10-20 23:25:40.038736 flask-aserto-0.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     8022 2022-10-20 23:21:27.735529 flask-aserto-0.5.0rc2/src/flask_aserto/__init__.py
+-rw-r--r--   0        0        0     1293 2022-10-18 20:41:06.191822 flask-aserto-0.5.0rc2/src/flask_aserto/_defaults.py
+-rw-r--r--   0        0        0      394 2022-02-03 23:43:06.666409 flask-aserto-0.5.0rc2/src/flask_aserto/_maybe_async.py
+-rw-r--r--   0        0        0        0 2022-02-03 23:43:06.666457 flask-aserto-0.5.0rc2/src/flask_aserto/py.typed
+-rw-r--r--   0        0        0     2377 2022-10-20 23:25:43.405313 flask-aserto-0.5.0rc2/setup.py
+-rw-r--r--   0        0        0     2848 2022-10-20 23:25:43.405553 flask-aserto-0.5.0rc2/PKG-INFO
```

### Comparing `flask-aserto-0.5.0rc1/README.md` & `flask-aserto-0.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `flask-aserto-0.5.0rc1/pyproject.toml` & `flask-aserto-0.5.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-aserto"
-version = "0.5.0.rc1"
+version = "0.5.0.rc2"
 description = "Aserto integration for Flask"
 readme = "README.md"
 authors = ["Aserto, Inc. <pypi@aserto.com>"]
 maintainers = ["authereal <authereal@aserto.com>"]
 homepage = "https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto"
 repository = "https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto"
 documentation = "https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto"
@@ -29,15 +29,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = "^3.10.0"
 Flask = {version = "^2.0.1", extras = ["async"]}
 Flask-Cors = "^3.0.10"
 grpcio = "^1.49.1"
 protobuf = "^4.21.7"
-aserto = {version = "0.3.0.rc1", allow-prereleases = true}
+aserto = {version = "0.3.0.rc3", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 black = "21.7b0"
 isort= "^5.9.3"
 mypy = "^0.910"
 pytest = "^6.2.4"
 python-dotenv = "^0.19.0"
```

### Comparing `flask-aserto-0.5.0rc1/src/flask_aserto/__init__.py` & `flask-aserto-0.5.0rc2/src/flask_aserto/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,35 +17,37 @@
 from ._maybe_async import MaybeAsyncCallback, maybe_await
 
 __all__ = ["AsertoMiddleware", "AuthorizationError"]
 
 
 @dataclass(frozen=True)
 class AuthorizationError(Exception):
-    policy_name: str
+    policy_instance_name: str
     policy_path: str
 
 
 Handler = TypeVar("Handler", bound=Callable[..., Union[Response, Awaitable[Response]]])
 
 
 class AsertoMiddleware:
     def __init__(
         self,
         *,
         authorizer_options: AuthorizerOptions,
-        policy_name: str,
         policy_path_root: str,
         identity_provider: MaybeAsyncCallback[Identity],
+        policy_instance_name: Optional[str]= None,
+        policy_instance_label: Optional[str]= None,
         policy_path_resolver: Optional[MaybeAsyncCallback[str]] = None,
         resource_context_provider: Optional[MaybeAsyncCallback[ResourceContext]] = None,
     ):
         self._authorizer_options = authorizer_options
         self._identity_provider = identity_provider
-        self._policy_name = policy_name
+        self._policy_instance_name = policy_instance_name
+        self._policy_instance_label = policy_instance_label
         self._policy_path_root = policy_path_root
 
         self._policy_path_resolver = (
             policy_path_resolver
             if policy_path_resolver is not None
             else create_default_policy_path_resolver(policy_path_root)
         )
@@ -56,27 +58,28 @@
             else DEFAULT_RESOURCE_CONTEXT_PROVIDER_FOR_ENDPOINT
         )
 
     async def _generate_client(self) -> AuthorizerClient:
         identity = await maybe_await(self._identity_provider())
 
         return AuthorizerClient(
-            authorizer=self._authorizer_options,
             identity=identity,
+            options=self._authorizer_options,
         )
 
     def _with_overrides(self, **kwargs: Any) -> "AsertoMiddleware":
         return (
             self
             if not kwargs
             else AsertoMiddleware(
                 authorizer_options=kwargs.get("authorizer", self._authorizer_options),
-                identity_provider=kwargs.get("identity_provider", self._identity_provider),
-                policy_name=kwargs.get("policy_name", self._policy_name),
                 policy_path_root=kwargs.get("policy_path_root", self._policy_path_root),
+                identity_provider=kwargs.get("identity_provider", self._identity_provider),
+                policy_instance_name=kwargs.get("policy_instance_name", self._policy_instance_name),
+                policy_instance_label=kwargs.get("policy_instance_label", self._policy_instance_label),
                 policy_path_resolver=kwargs.get("policy_path_resolver", self._policy_path_resolver),
                 resource_context_provider=kwargs.get(
                     "resource_context_provider", self._resource_context_provider
                 ),
             )
         )
 
@@ -87,15 +90,16 @@
     @overload
     async def check(
         self,
         decision: str,
         *,
         authorizer_options: AuthorizerOptions = ...,
         identity_provider: MaybeAsyncCallback[Identity] = ...,
-        policy_name: str = ...,
+        policy_instance_name: str = ...,
+        policy_instance_label: str = ...,
         policy_path_root: str = ...,
         policy_path_resolver: MaybeAsyncCallback[str] = ...,
         resource_context_provider: MaybeAsyncCallback[ResourceContext] = ...,
     ) -> bool:
         ...
 
     async def check(self, decision: str, **kwargs: Any) -> bool:
@@ -104,32 +108,34 @@
     async def _check(self, decision: str) -> bool:
         client, resource_context, policy_path = await gather(
             self._generate_client(),
             maybe_await(self._resource_context_provider()),
             maybe_await(self._policy_path_resolver()),
         )
         decisions = await client.decisions(
-            decisions=(decision,),
-            policy_name=self._policy_name,
             policy_path=policy_path,
+            decisions=(decision,),
+            policy_instance_name=self._policy_instance_name,
+            policy_instance_label=self._policy_instance_label,
             resource_context=resource_context,
         )
         return decisions[decision]
 
     @overload
     def authorize(self, handler: Handler) -> Handler:
         ...
 
     @overload
     def authorize(
         self,
         *,
         authorizer_options: AuthorizerOptions = ...,
         identity_provider: MaybeAsyncCallback[Identity] = ...,
-        policy_name: str = ...,
+        policy_instance_name: str = ...,
+        policy_instance_label: str = ...,
         policy_path_root: str = ...,
         policy_path_resolver: MaybeAsyncCallback[str] = ...,
     ) -> Callable[[Handler], Handler]:
         ...
 
     def authorize(  # type: ignore[misc]
         self,
@@ -164,22 +170,23 @@
             client, policy_path, resource_context = await gather(
                 self._generate_client(),
                 maybe_await(self._policy_path_resolver()),
                 maybe_await(self._resource_context_provider()),
             )
 
             decisions = await client.decisions(
-                decisions=("allowed",),
-                policy_name=self._policy_name,
                 policy_path=policy_path,
+                decisions=("allowed",),
+                policy_instance_name=self._policy_instance_name,
+                policy_instance_label=self._policy_instance_label,
                 resource_context=resource_context,
             )
 
             if not decisions["allowed"]:
-                raise AuthorizationError(policy_name=self._policy_name, policy_path=policy_path)
+                raise AuthorizationError(policy_instance_name=self._policy_instance_name, policy_path=policy_path)
 
             return await maybe_await(handler(*args, **kwargs))
 
         return cast(Handler, decorated)
 
     def register_display_state_map(
         self,
@@ -196,16 +203,17 @@
 
             client, resource_context = await gather(
                 self._generate_client(),
                 maybe_await(resource_context_provider()),
             )
 
             display_state_map = await client.decision_tree(
-                decisions=["visible", "enabled"],
-                policy_name=self._policy_name,
                 policy_path_root=self._policy_path_root,
+                decisions=["visible", "enabled"],
+                policy_instance_name=self._policy_instance_name,
+                policy_instance_label=self._policy_instance_label,
                 resource_context=resource_context,
                 policy_path_separator="SLASH",
             )
             return jsonify(display_state_map)
 
         return app
```

### Comparing `flask-aserto-0.5.0rc1/src/flask_aserto/_defaults.py` & `flask-aserto-0.5.0rc2/src/flask_aserto/_defaults.py`

 * *Files identical despite different names*

### Comparing `flask-aserto-0.5.0rc1/setup.py` & `flask-aserto-0.5.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Flask-Cors>=3.0.10,<4.0.0',
  'Flask[async]>=2.0.1,<3.0.0',
- 'aserto==0.3.0.rc1',
+ 'aserto==0.3.0.rc3',
  'grpcio>=1.49.1,<2.0.0',
  'protobuf>=4.21.7,<5.0.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'flask-aserto',
-    'version': '0.5.0rc1',
+    'version': '0.5.0rc2',
     'description': 'Aserto integration for Flask',
     'long_description': '# Aserto Flask middleware\nThis is the official library for integrating [Aserto](https://www.aserto.com/) authorization into your [Flask](https://github.com/pallets/flask) applications.\n\nFor a example of what this looks like in a running Flask app and guidance on connecting an identity provider, see the [PeopleFinder app example](https://github.com/aserto-dev/aserto-python/tree/main/packages/flask-aserto/peoplefinder_example).\n\n## Features\n### Add authorization checks to your routes\n```py\nfrom flask_aserto import AsertoMiddleware, AuthorizationError\n\n\napp = Flask(__name__)\naserto = AsertoMiddleware(**aserto_options)\n\n\n@app.route("/api/users/<id>", methods=["GET"])\n@aserto.authorize\ndef api_user(id: str) -> Response:\n    # Raises an AuthorizationError if the `GET.api.users.__id`\n    # policy returns a decision of "allowed = false" \n    ...\n```\n### Automatically create a route to serve a [Display State Map](https://docs.aserto.com/docs/authorizer-guide/display-state-map)\n```py\n# Defaults to creating a route at the path "/__displaystatemap" \naserto.register_display_state_map(app)\n```\n### Perform more finely controlled authorization checks\n```py\n@app.route("/api/users/<id>", methods=["GET"])\nasync def api_user(id: str) -> Response:\n    # This also automatically knows to check the `GET.api.users.__id` policy\n    if not await aserto.check("allowed"):\n        raise AuthorizationError()\n\n    ...\n```\n',
     'author': 'Aserto, Inc.',
     'author_email': 'pypi@aserto.com',
     'maintainer': 'authereal',
     'maintainer_email': 'authereal@aserto.com',
     'url': 'https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto',
```

### Comparing `flask-aserto-0.5.0rc1/PKG-INFO` & `flask-aserto-0.5.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-aserto
-Version: 0.5.0rc1
+Version: 0.5.0rc2
 Summary: Aserto integration for Flask
 Home-page: https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto
 License: Apache-2.0
 Author: Aserto, Inc.
 Author-email: pypi@aserto.com
 Maintainer: authereal
 Maintainer-email: authereal@aserto.com
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask[async] (>=2.0.1,<3.0.0)
-Requires-Dist: aserto (==0.3.0.rc1)
+Requires-Dist: aserto (==0.3.0.rc3)
 Requires-Dist: grpcio (>=1.49.1,<2.0.0)
 Requires-Dist: protobuf (>=4.21.7,<5.0.0)
 Requires-Dist: typing-extensions (>=3.10.0,<4.0.0)
 Project-URL: Documentation, https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto
 Project-URL: Repository, https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/flask-aserto
 Description-Content-Type: text/markdown
```

