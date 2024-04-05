# Comparing `tmp/nestpython-0.3.6.tar.gz` & `tmp/nestpython-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestpython-0.3.6.tar", last modified: Tue Apr  2 20:06:36 2024, max compression
+gzip compressed data, was "nestpython-0.3.7.tar", last modified: Fri Apr  5 18:34:22 2024, max compression
```

## Comparing `nestpython-0.3.6.tar` & `nestpython-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:06:36.890846 nestpython-0.3.6/
--rw-rw-rw-   0        0        0     1346 2024-04-02 20:06:36.888850 nestpython-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-02 20:06:36.000000 nestpython-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 20:06:36.881871 nestpython-0.3.6/nestpy/
--rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.6/nestpy/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.6/nestpy/files.py
--rw-rw-rw-   0        0        0    14122 2024-04-02 20:06:20.000000 nestpython-0.3.6/nestpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:06:36.887853 nestpython-0.3.6/nestpython.egg-info/
--rw-rw-rw-   0        0        0     1346 2024-04-02 20:06:36.000000 nestpython-0.3.6/nestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-02 20:06:36.000000 nestpython-0.3.6/nestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:06:36.000000 nestpython-0.3.6/nestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 20:06:36.000000 nestpython-0.3.6/nestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 20:06:36.891843 nestpython-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:34:22.769569 nestpython-0.3.7/
+-rw-rw-rw-   0        0        0     1346 2024-04-05 18:34:22.767555 nestpython-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 18:34:21.000000 nestpython-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 18:34:22.761571 nestpython-0.3.7/nestpy/
+-rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.7/nestpy/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.7/nestpy/files.py
+-rw-rw-rw-   0        0        0    14327 2024-04-05 18:10:38.000000 nestpython-0.3.7/nestpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:34:22.766558 nestpython-0.3.7/nestpython.egg-info/
+-rw-rw-rw-   0        0        0     1346 2024-04-05 18:34:22.000000 nestpython-0.3.7/nestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-05 18:34:22.000000 nestpython-0.3.7/nestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:34:22.000000 nestpython-0.3.7/nestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 18:34:22.000000 nestpython-0.3.7/nestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:34:22.770547 nestpython-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.7/setup.py
```

### Comparing `nestpython-0.3.6/PKG-INFO` & `nestpython-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.6
+Version: 0.3.7
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.6/nestpy/files.py` & `nestpython-0.3.7/nestpy/files.py`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.6/nestpy/main.py` & `nestpython-0.3.7/nestpy/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         case Iterable():
           out += unpack(arg)
         case _:
           out.append(arg)
     return out
 
   TokenTypes = Enum('TokenTypes', [
-      'SYNTACTICAL', 'MISS', 'INDENTED', 
+      'SYNTACTICAL', 'MULTILINE', 'INDENTED',
     'MAP', 'CTYPES', 'STRING', 
     'APPENDSUB', 'SHORTHAND', 'MACROS', 'ESCAPEMENT'
   ])
 
   id = 0
 
   class Token:
@@ -49,18 +49,17 @@
   def tokenize(string, tokens: list[Token], buffer):
     tokenized = []
     i = 0
     j = 0
     while i + j < len(string):
       for token in tokens:
         F = (i + j - buffer >= 0)
-        match = re.match(
+        if match := re.match(
             fr'[\s\S]{{{buffer}}}{token.symb}' if F else token.symb,
-            string[i + j - buffer:] if F else string, re.M)
-        if match:
+            string[i + j - buffer:] if F else string, re.M):
           match_string = match.group()[buffer:] if F else match.group()
           if string[i:i + j] != '':
             tokenized.append(anonToken(string[i:i + j]))
           tokenized.append(Token(match_string, token.types, setID=token.id))
           i += j + len(match_string)
           j = -1
           break
@@ -87,18 +86,20 @@
     dictIndentRight = Token(r'}-', TokenTypes.MAP)
     indentLeftNoColon = Token(r'~{', TokenTypes.INDENTED,
       TokenTypes.SYNTACTICAL)
     indentLeftDouble = Token(r'{{')
     indentSelfClose = Token(r'{\s*}', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
     indentLeft = Token(r'{', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
     indentRight = Token(r'}', TokenTypes.INDENTED, TokenTypes.SYNTACTICAL)
-    newline = Token(r'\n', TokenTypes.INDENTED, TokenTypes.MISS)
+    newline = Token(r'\n', TokenTypes.INDENTED, TokenTypes.MULTILINE)
     returnShorthand = Token(r'=>', TokenTypes.SHORTHAND)
     nativeSemicolon = Token(r',,', TokenTypes.MAP)
     nativeAssignment = Token(r'<-', TokenTypes.MAP)
+    incrementOperator = Token(r'\+\+', TokenTypes.MAP)
+    decrementOperator = Token(r'--', TokenTypes.MAP)
     andShorthand = Token(r'&&', TokenTypes.SHORTHAND)
     orShorthand = Token(r'\|\|', TokenTypes.SHORTHAND)
     isShorthand = Token(r'=&', TokenTypes.SHORTHAND)
     isNotShorthand = Token(r'!=&', TokenTypes.SHORTHAND)
     defShorthand = Token(r':=', TokenTypes.SHORTHAND)
     inShorthand = Token(r'->', TokenTypes.SHORTHAND)
     notInShorthand = Token(r'!>', TokenTypes.SHORTHAND)
@@ -143,14 +144,16 @@
       Tokens.defShorthand.value.id: 'def',
       Tokens.inShorthand.value.id: 'in',
       Tokens.caseShorthand.value.id: 'case',
       Tokens.notInShorthand.value.id: 'not in',
       Tokens.returnShorthand.value.id: 'return',
       Tokens.lambdaShorthand.value.id: 'lambda',
       Tokens.delShorthand.value.id: 'del',
+      Tokens.incrementOperator.value.id: '+=1',
+      Tokens.decrementOperator.value.id: '-=1',
       Tokens.intDiv.value.id: '//'
   }
 
   def isF(token, ptoken):
     with contextlib.suppress(TypeError):
       return (TokenTypes.STRING in token.types) and (ptoken.symb[~0].lower() == 'f' or
                                                      ptoken.symb[~1:].lower() == 'fr')
@@ -336,15 +339,15 @@
             compiled_code += token.symb
           case Tokens.indentRight.value.id:
             if tokens[n+1].id == token.id:
               compiled_code += token.symb * 2
               tokens = tokens[n+2:]
               raise breakout
       if (not (TokenTypes.SYNTACTICAL in token.types and compilable())
-          and not (TokenTypes.MISS in token.types and not in_multilineString())):
+          and not (TokenTypes.MULTILINE in token.types and not in_multilineString())):
         
         mtoken = tokenMap[token.id] if (TokenTypes.MAP in token.types
                                         and compilable()) else token.symb
         if compilable():
           if TokenTypes.APPENDSUB in token.types:
             mtoken += '_'
           if TokenTypes.SHORTHAND in token.types:
```

### Comparing `nestpython-0.3.6/nestpython.egg-info/PKG-INFO` & `nestpython-0.3.7/nestpython.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.6
+Version: 0.3.7
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.6/setup.py` & `nestpython-0.3.7/setup.py`

 * *Files identical despite different names*

