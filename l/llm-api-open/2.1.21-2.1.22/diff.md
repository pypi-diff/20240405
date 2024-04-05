# Comparing `tmp/llm-api-open-2.1.21.tar.gz` & `tmp/llm-api-open-2.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-api-open-2.1.21.tar", last modified: Tue Apr  2 17:15:29 2024, max compression
+gzip compressed data, was "llm-api-open-2.1.22.tar", last modified: Fri Apr  5 16:16:56 2024, max compression
```

## Comparing `llm-api-open-2.1.21.tar` & `llm-api-open-2.1.22.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.727098 llm-api-open-2.1.21/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/configs/chatgpt.json
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/configs/ms_copilot.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.727098 llm-api-open-2.1.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/src/llm_api_open.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-02 17:15:29.000000 llm-api-open-2.1.21/src/llm_api_open.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 17:15:29.000000 llm-api-open-2.1.21/src/llm_api_open.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:15:29.000000 llm-api-open-2.1.21/src/llm_api_open.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 17:15:29.000000 llm-api-open-2.1.21/src/llm_api_open.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 17:15:29.000000 llm-api-open-2.1.21/src/llm_api_open.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 17:15:29.000000 llm-api-open-2.1.21/src/llm_api_open.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/src/lmao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/src/lmao/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/chatgpt/assistantGetLastMessage.js
--rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/chatgpt/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/chatgpt/conversationSearch.js
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/chatgpt/proxy_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/external_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/module_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:15:29.731098 llm-api-open-2.1.21/src/lmao/ms_copilot/
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/ms_copilot/conversationManage.js
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/ms_copilot/conversationParser.js
--rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/ms_copilot/ms_copilot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-02 17:15:23.000000 llm-api-open-2.1.21/src/lmao/ms_copilot/proxy_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.114415 llm-api-open-2.1.22/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.106414 llm-api-open-2.1.22/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/configs/chatgpt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/configs/ms_copilot.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:16:56.114415 llm-api-open-2.1.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.106414 llm-api-open-2.1.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/llm_api_open.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 16:16:56.000000 llm-api-open-2.1.22/src/llm_api_open.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/lmao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/lmao/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/assistantGetLastMessage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38090 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/conversationSearch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/chatgpt/proxy_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/external_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8706 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/module_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:16:56.110415 llm-api-open-2.1.22/src/lmao/ms_copilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/conversationManage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/conversationParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/ms_copilot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-05 16:16:52.000000 llm-api-open-2.1.22/src/lmao/ms_copilot/proxy_extension.py
```

### Comparing `llm-api-open-2.1.21/LICENSE` & `llm-api-open-2.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/PKG-INFO` & `llm-api-open-2.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.21
+Version: 2.1.22
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `llm-api-open-2.1.21/README.md` & `llm-api-open-2.1.22/README.md`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/configs/chatgpt.json` & `llm-api-open-2.1.22/configs/chatgpt.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/configs/ms_copilot.json` & `llm-api-open-2.1.22/configs/ms_copilot.json`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/setup.py` & `llm-api-open-2.1.22/setup.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/llm_api_open.egg-info/PKG-INFO` & `llm-api-open-2.1.22/src/llm_api_open.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-api-open
-Version: 2.1.21
+Version: 2.1.22
 Summary: Unofficial open APIs for popular LLMs with self-hosted redirect capability
 Home-page: https://github.com/F33RNI/LlM-Api-Open
 Author: Fern Lane
 License: MIT License
 Project-URL: Bug Report, https://github.com/F33RNI/LlM-Api-Open/issues/new
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `llm-api-open-2.1.21/src/llm_api_open.egg-info/SOURCES.txt` & `llm-api-open-2.1.22/src/llm_api_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/_version.py` & `llm-api-open-2.1.22/src/lmao/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = "2.1.21"
+__version__ = "2.1.22"
```

### Comparing `llm-api-open-2.1.21/src/lmao/chatgpt/assistantGetLastMessage.js` & `llm-api-open-2.1.22/src/lmao/chatgpt/assistantGetLastMessage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/chatgpt/chatgpt_api.py` & `llm-api-open-2.1.22/src/lmao/chatgpt/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/chatgpt/conversationSearch.js` & `llm-api-open-2.1.22/src/lmao/chatgpt/conversationSearch.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/chatgpt/proxy_extension.py` & `llm-api-open-2.1.22/src/lmao/chatgpt/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/external_api.py` & `llm-api-open-2.1.22/src/lmao/external_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/main.py` & `llm-api-open-2.1.22/src/lmao/main.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/module_wrapper.py` & `llm-api-open-2.1.22/src/lmao/module_wrapper.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/ms_copilot/conversationManage.js` & `llm-api-open-2.1.22/src/lmao/ms_copilot/conversationManage.js`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/ms_copilot/conversationParser.js` & `llm-api-open-2.1.22/src/lmao/ms_copilot/conversationParser.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -223,16 +223,37 @@
             // iframe inner document
             const iframeDocument = cibMessage.shadowRoot.querySelector("cib-shared > iframe").contentWindow.document;
 
             // Extract image caption from title
             try {
                 const caption = iframeDocument.querySelector("#gir_async > a").getAttribute("title");
                 result.caption = caption;
-            } catch (error) {
-                console.error(error);
+            } catch (e) {
+                try {
+                    const caption = iframeDocument.querySelector("#gir_async > div.gir_attr_lnk_container > a.gir_attr_lnk").getAttribute("title");
+                    result.caption = caption;
+                } catch (error) {
+                    console.error(error);
+                }
+            }
+
+            // Try to find error
+            let errorMessage = null;
+            try {
+                errorMessage = iframeDocument.querySelector("#girer > div > div.gil_err_sbt").innerText;
+                errorMessage = "<p>" + errorMessage.replace("\nReport", "") + "</p>";
+            } catch (error) {}
+
+            // Save error text
+            if (errorMessage !== null) {
+                if (result.text === undefined) {
+                    result.text = errorMessage;
+                } else {
+                    result.text += errorMessage;
+                }
             }
 
             // Parse image tags (extract clean links)
             result.images = [];
             const images = iframeDocument.getElementsByClassName("mimg");
             for (const image of images) {
                 if (image.tagName !== "IMG" || !image.getAttribute("src")) {
```

### Comparing `llm-api-open-2.1.21/src/lmao/ms_copilot/ms_copilot_api.py` & `llm-api-open-2.1.22/src/lmao/ms_copilot/ms_copilot_api.py`

 * *Files identical despite different names*

### Comparing `llm-api-open-2.1.21/src/lmao/ms_copilot/proxy_extension.py` & `llm-api-open-2.1.22/src/lmao/ms_copilot/proxy_extension.py`

 * *Files identical despite different names*

