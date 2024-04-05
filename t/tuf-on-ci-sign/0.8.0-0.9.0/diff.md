# Comparing `tmp/tuf_on_ci_sign-0.8.0.tar.gz` & `tmp/tuf_on_ci_sign-0.9.0.tar.gz`

## Comparing `tuf_on_ci_sign-0.8.0.tar` & `tuf_on_ci_sign-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/create-config-file.sh
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/test/test_user.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/__init__.py
--rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/_common.py
--rw-r--r--   0        0        0    27671 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/_signer_repository.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/_user.py
--rwxr-xr-x   0        0        0    13482 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/delegate.py
--rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/import_repo.py
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/sign.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/.gitignore
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/README.md
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/create-config-file.sh
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/test/test_user.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/__init__.py
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/_common.py
+-rw-r--r--   0        0        0    28053 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/_signer_repository.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/_user.py
+-rwxr-xr-x   0        0        0    13482 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/delegate.py
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/import_repo.py
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/sign.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/.gitignore
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/README.md
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 tuf_on_ci_sign-0.9.0/PKG-INFO
```

### Comparing `tuf_on_ci_sign-0.8.0/create-config-file.sh` & `tuf_on_ci_sign-0.9.0/create-config-file.sh`

 * *Files identical despite different names*

### Comparing `tuf_on_ci_sign-0.8.0/test/test_user.py` & `tuf_on_ci_sign-0.9.0/test/test_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,14 +90,17 @@
                 hsm_signer.token_filter, {"label": "YubiKey PIV #15835999"}
             )
             self.assertEqual(
                 hsm_signer.public_key.keyid,
                 "762cb22caca65de5e9b7b6baecb84ca989d337280ce6914b6440aea95769ad93",
             )
 
+            # Cache the signer
+            user.set_signer(HSM_KEY, hsm_signer)
+
             # If the signing key is not configured, we expect a generic HSM signer
             other_signer = user.get_signer(NONCONFIGURED_KEY)
             self.assertIsInstance(other_signer, HSMSigner)
             self.assertEqual(other_signer.token_filter, {})
             self.assertEqual(
                 other_signer.public_key.keyid,
                 "64eeece964e09c058ef8f9805daca546b01ba4719c80b6fe911b091a7c05124b",
```

### Comparing `tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/_common.py` & `tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/_common.py`

 * *Files identical despite different names*

### Comparing `tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/_signer_repository.py` & `tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/_signer_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,27 +239,36 @@
                 keys.append(key)
         except ValueError:
             pass  # role is not delegated or key was not found
 
         return keys
 
     def _sign(self, role: str, md: Metadata, key: Key) -> None:
-        signer = self.user.get_signer(key)
         while True:
+            signer = self.user.get_signer(key)
             try:
-                md.sign(signer, True)
+                sig = md.sign(signer, True)
+                key.verify_signature(sig, md.signed_bytes)
+                self.user.set_signer(key, signer)
                 break
             except UnsignedMetadataError as e:
                 print(f"Failed to sign {role} with {self.user.name} key.\n    {e}")
                 logger.debug("Sign traceback", exc_info=True)
-                click.prompt(
-                    "Press any key to try again (Ctrl-C to cancel)",
-                    default=True,
-                    show_default=False,
+            except UnverifiedSignatureError as e:
+                print(
+                    f"Failed to verify {self.user.name} signature "
+                    f"(is this the correct key?)\n    {e}"
                 )
+                logger.debug("Verify traceback", exc_info=True)
+
+            click.prompt(
+                "Press any key to try again (Ctrl-C to cancel)",
+                default=True,
+                show_default=False,
+            )
 
     def _write(self, role: str, md: Metadata) -> None:
         filename = self._get_filename(role)
 
         os.makedirs(os.path.join(self._dir, "root_history"), exist_ok=True)
 
         data = md.to_bytes(JSONSerializer())
```

### Comparing `tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/_user.py` & `tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         # signer cache gets populated as they are used the first time
         self._signers: dict[str, Signer] = {}
 
     def get_signer(self, key: Key) -> Signer:
         """Returns a Signer for the given public key
 
         The signer sources are (in order):
+        * signers cached via set_signer()
         * any configured signer from 'signing-keys' config section
         * for sigstore type keys, a Signer is automatically created
         * for any remaining keys, HSM is assumed and a signer is created
         """
 
         def get_secret(secret: str) -> str:
             msg = f"Enter {secret} to sign"
@@ -81,23 +82,24 @@
             # special case for tests -- prompt() will lockup trying to hide STDIN:
             if not sys.stdin.isatty():
                 return sys.stdin.readline().rstrip()
 
             return click.prompt(bold(msg), hide_input=True)
 
         if key.keyid in self._signers:
-            # signer is already cached
-            pass
-        elif key.keyid in self._signing_key_uris:
+            return self._signers[key.keyid]
+        if key.keyid in self._signing_key_uris:
             # signer is not cached yet, but config exists
             uri = self._signing_key_uris[key.keyid]
-            self._signers[key.keyid] = Signer.from_priv_key_uri(uri, key, get_secret)
-        elif key.keytype == "sigstore-oidc":
+            return Signer.from_priv_key_uri(uri, key, get_secret)
+        if key.keytype == "sigstore-oidc":
             # signer is not cached, no configuration was found, type is sigstore
-            self._signers[key.keyid] = Signer.from_priv_key_uri(
-                "sigstore:?ambient=false", key, get_secret
-            )
-        else:
-            # signer is not cached, no configuration was found: assume Yubikey
-            self._signers[key.keyid] = Signer.from_priv_key_uri("hsm:", key, get_secret)
+            return Signer.from_priv_key_uri("sigstore:?ambient=false", key, get_secret)
+        # signer is not cached, no configuration was found: assume Yubikey
+        return Signer.from_priv_key_uri("hsm:", key, get_secret)
 
-        return self._signers[key.keyid]
+    def set_signer(self, key: Key, signer: Signer) -> None:
+        """Cache a signer for a keyid
+
+        This should be called after a successful signing operation
+        """
+        self._signers[key.keyid] = signer
```

### Comparing `tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/delegate.py` & `tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/delegate.py`

 * *Files identical despite different names*

### Comparing `tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/import_repo.py` & `tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/import_repo.py`

 * *Files identical despite different names*

### Comparing `tuf_on_ci_sign-0.8.0/tuf_on_ci_sign/sign.py` & `tuf_on_ci_sign-0.9.0/tuf_on_ci_sign/sign.py`

 * *Files identical despite different names*

### Comparing `tuf_on_ci_sign-0.8.0/pyproject.toml` & `tuf_on_ci_sign-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 [project]
 name = "tuf-on-ci-sign"
 description = "Signing tools for TUF-on-CI"
 readme = "README.md"
 dependencies = [
   "packaging >= 23.2,< 25.0",
   "platformdirs ~= 4.2",
-  "securesystemslib[awskms,azurekms,gcpkms,hsm,sigstore] ~= 0.30",
+  "securesystemslib[awskms,azurekms,gcpkms,hsm,sigstore] ~= 0.31.0",
   "tuf ~= 3.0",
   "click ~= 8.1",
 ]
 requires-python = ">=3.10"
 dynamic = ["version"]
 
 [project.scripts]
 tuf-on-ci-delegate = "tuf_on_ci_sign:delegate"
 tuf-on-ci-import-repo = "tuf_on_ci_sign:import_repo"
 tuf-on-ci-sign = "tuf_on_ci_sign:sign"
 
 [project.optional-dependencies]
 lint = [
   "mypy == 1.9.0",
-  "ruff == 0.3.4",
+  "ruff == 0.3.5",
 ]
 
 [tool.hatch.version]
 path = "tuf_on_ci_sign/__init__.py"
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `tuf_on_ci_sign-0.8.0/PKG-INFO` & `tuf_on_ci_sign-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: tuf-on-ci-sign
-Version: 0.8.0
+Version: 0.9.0
 Summary: Signing tools for TUF-on-CI
 Requires-Python: >=3.10
 Requires-Dist: click~=8.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: platformdirs~=4.2
-Requires-Dist: securesystemslib[awskms,azurekms,gcpkms,hsm,sigstore]~=0.30
+Requires-Dist: securesystemslib[awskms,azurekms,gcpkms,hsm,sigstore]~=0.31.0
 Requires-Dist: tuf~=3.0
 Provides-Extra: lint
 Requires-Dist: mypy==1.9.0; extra == 'lint'
-Requires-Dist: ruff==0.3.4; extra == 'lint'
+Requires-Dist: ruff==0.3.5; extra == 'lint'
 Description-Content-Type: text/markdown
 
 ### TUF-on-CI Signing tools
 
 This package contains the signing tools for
 [TUF-on-CI](https://github.com/theupdateframework/tuf-on-ci). Please see
 TUF-on-CI README for usage.
```

