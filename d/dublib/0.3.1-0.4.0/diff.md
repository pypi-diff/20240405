# Comparing `tmp/dublib-0.3.1.tar.gz` & `tmp/dublib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dublib-0.3.1.tar", last modified: Sun Jan 28 22:16:05 2024, max compression
+gzip compressed data, was "dublib-0.4.0.tar", last modified: Thu Apr  4 22:46:26 2024, max compression
```

## Comparing `dublib-0.3.1.tar` & `dublib-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:16:05.749454 dublib-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-28 22:15:54.000000 dublib-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-28 22:16:05.749454 dublib-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-01-28 22:15:54.000000 dublib-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-28 22:15:54.000000 dublib-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 22:16:05.749454 dublib-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:16:05.745454 dublib-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:16:05.745454 dublib-0.3.1/src/dublib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:16:05.749454 dublib-0.3.1/src/dublib/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Exceptions/StyledPrinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Exceptions/Terminalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Exceptions/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Polyglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/StyledPrinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    42920 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/Terminalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30713 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 22:15:54.000000 dublib-0.3.1/src/dublib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:16:05.749454 dublib-0.3.1/src/dublib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-28 22:16:05.000000 dublib-0.3.1/src/dublib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-28 22:16:05.000000 dublib-0.3.1/src/dublib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 22:16:05.000000 dublib-0.3.1/src/dublib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-28 22:16:05.000000 dublib-0.3.1/src/dublib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 22:16:05.000000 dublib-0.3.1/src/dublib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-04 22:46:22.000000 dublib-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-04 22:46:26.818866 dublib-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-04 22:46:22.000000 dublib-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-04 22:46:22.000000 dublib-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:46:26.818866 dublib-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.814866 dublib-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/src/dublib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/src/dublib/Exceptions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/WebRequestor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8986 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/StyledPrinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27075 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/WebRequestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/src/dublib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/top_level.txt
```

### Comparing `dublib-0.3.1/LICENSE` & `dublib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dublib-0.3.1/PKG-INFO` & `dublib-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.3.1
+Version: 0.4.0
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -39,29 +39,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: curl_cffi>=0.6.0
 Requires-Dist: fake_useragent
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
 Requires-Dist: requests
 
 # dublib
 **dublib** – это библиотека, поставляющая компоненты, требующиеся в проектах [@DUB1401](https://github.com/DUB1401), написанных на Python.
 
 # Поставляемые компоненты
 Библиотека включает следующие модули:
-* [Methods](docs/Methods.md)
-* [Polyglot](docs/Polyglot.md)
-* [StyledPrinter](docs/StyledPrinter.md)
-* [Terminalyzer](docs/Terminalyzer.md)
-* [WebRequestor](docs/WebRequestor.md)
+* [Methods](https://github.com/DUB1401/dublib/blob/main/docs/Methods.md)
+* [Polyglot](https://github.com/DUB1401/dublib/blob/main/docs/Polyglot.md)
+* [StyledPrinter](https://github.com/DUB1401/dublib/blob/main/docs/StyledPrinter.md)
+* [Terminalyzer](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
+* [WebRequestor](https://github.com/DUB1401/dublib/blob/main/docs/WebRequestor.md)
 
 # Установка
 Библиотека поддерживает установку из двух типов репозиториев:
 * **PyPI** – стабильные выпуски (с возможностью выбора конкретной версии);
 * **GitHub** – канал разработки со всеми последними изменениями и исправлениями.
 
 _**Примечание:**_ Для установки библиотеки из репозитория GitHub на вашем устройстве должна присутствовать система контроля версий Git.
```

### Comparing `dublib-0.3.1/README.md` & `dublib-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # dublib
 **dublib** – это библиотека, поставляющая компоненты, требующиеся в проектах [@DUB1401](https://github.com/DUB1401), написанных на Python.
 
 # Поставляемые компоненты
 Библиотека включает следующие модули:
-* [Methods](docs/Methods.md)
-* [Polyglot](docs/Polyglot.md)
-* [StyledPrinter](docs/StyledPrinter.md)
-* [Terminalyzer](docs/Terminalyzer.md)
-* [WebRequestor](docs/WebRequestor.md)
+* [Methods](https://github.com/DUB1401/dublib/blob/main/docs/Methods.md)
+* [Polyglot](https://github.com/DUB1401/dublib/blob/main/docs/Polyglot.md)
+* [StyledPrinter](https://github.com/DUB1401/dublib/blob/main/docs/StyledPrinter.md)
+* [Terminalyzer](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
+* [WebRequestor](https://github.com/DUB1401/dublib/blob/main/docs/WebRequestor.md)
 
 # Установка
 Библиотека поддерживает установку из двух типов репозиториев:
 * **PyPI** – стабильные выпуски (с возможностью выбора конкретной версии);
 * **GitHub** – канал разработки со всеми последними изменениями и исправлениями.
 
 _**Примечание:**_ Для установки библиотеки из репозитория GitHub на вашем устройстве должна присутствовать система контроля версий Git.
```

### Comparing `dublib-0.3.1/pyproject.toml` & `dublib-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "cython"]
 
 [project]
 name = "dublib"
-version = "0.3.1"
+version = "0.4.0"
 description = "Коллекция модулей от DUB1401."
 authors = [
 	{name = "DUB1401", email="vlad.milosta@outlook.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
-dependencies = ["fake_useragent", "httpx", "httpx[http2]", "requests"]
+dependencies = ["curl_cffi>=0.6.0", "fake_useragent", "httpx", "httpx[http2]", "requests"]
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"License :: OSI Approved :: The Unlicense (Unlicense)",
 	"Natural Language :: Russian",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3.10",
```

### Comparing `dublib-0.3.1/src/dublib/Exceptions/StyledPrinter.py` & `dublib-0.4.0/src/dublib/Exceptions/StyledPrinter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-class DuplicatedStyles(Exception):
-	"""
-	Исключение: использованы оба способа указания стилей.
-	"""
-
-	def __init__(self):
-		"""
-		Исключение: использованы оба способа указания стилей.
-		"""
-		
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "Use only StyledGroup() or arguments styles."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message)
-			
-	def __str__(self):
+class DuplicatedStyles(Exception):
+	"""Исключение: использованы оба способа указания стилей."""
+
+	def __init__(self):
+		"""Исключение: использованы оба способа указания стилей."""
+		
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "Use only StyledGroup() or arguments styles."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message)
+			
+	def __str__(self):
 		return self.__Message
```

### Comparing `dublib-0.3.1/src/dublib/Exceptions/Terminalyzer.py` & `dublib-0.4.0/src/dublib/Exceptions/Terminalyzer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,134 @@
-class IdenticalIndicators(Exception):
-	"""
-	Исключение: попытка установки одинаковых индикаторов ключей и флагов.
-	"""
-
-	def __init__(self):
-		"""
-		Исключение: попытка установки одинаковых индикаторов ключей и флагов.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "Cannot set same indicators for keys and flags."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-			
-	def __str__(self):
-		return self.__Message
-
-class InvalidArgumentType(Exception):
-	"""
-	Исключение: неверное значение аргумента.
-	"""
-
-	def __init__(self, value: str, type_name: str):
-		"""
-		Исключение: неверное значение аргумента.
-			value – значение аргумента;
-			type_name – название ожидаемого типа.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + value + "\" isn't \"" + type_name + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-			
-	def __str__(self):
-		return self.__Message
-
-class MutuallyExclusiveFlags(Exception):
-	"""
-	Исключение: активированы взаимоисключающие флаги.
-	"""
-
-	def __init__(self, command: str):
-		"""
-		Исключение: активированы взаимоисключающие флаги.
-			command – команда, вызвавшая исключение.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + command + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-			
-	def __str__(self):
-		return self.__Message
-
-class MutuallyExclusiveKeys(Exception):
-	"""
-	Исключение: активированы взаимоисключающие ключи.
-	"""
-
-	def __init__(self, command: str):
-		"""
-		Исключение: активированы взаимоисключающие ключи.
-			command – команда, вызвавшая исключение.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + command + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-		
-			
-	def __str__(self):
-		return self.__Message
-	
-class MutuallyExclusivePositions(Exception):
-	"""
-	Исключение: активированы разные позиции на одном слое.
-	"""
-
-	def __init__(self, command: str): 
-		"""
-		Исключение: активированы разные позиции на одном слое.
-			command – команда, вызвавшая исключение.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + command + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-		
-	def __str__(self):
-		return self.__Message
-
-class NotEnoughArguments(Exception):
-	"""
-	Исключение: недостаточно аргументов.
-	"""
-
-	def __init__(self, command: str):
-		"""
-		Исключение: недостаточно аргументов.
-			command – команда, вызвавшая исключение.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + command + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-
-	def __str__(self):
-		return self.__Message
-
-class TooManyArguments(Exception):
-	"""
-	Исключение: слишком много аргументов.
-	"""
-
-	def __init__(self, command: str):
-		"""
-		Исключение: слишком много аргументов.
-			command – команда, вызвавшая исключение.
-		"""
-
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + command + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-			
-	def __str__(self):
-		return self.__Message
-
-class UnknownCommand(Exception):
-	"""
-	Исключение: неизвестная комманда.
-	"""
-
-	def __init__(self, command: str):
-		"""
-		Исключение: неизвестная комманда.
-			command – команда, вызвавшая исключение.
-		"""
-		
-		# Добавление данных в сообщение об ошибке.
-		self.__Message = "\"" + command + "\"."
-		# Обеспечение доступа к оригиналу наследованного свойства.
-		super().__init__(self.__Message) 
-		
-	def __str__(self):
+class IdenticalIndicators(Exception):
+	"""Исключение: попытка установки одинаковых индикаторов ключей и флагов."""
+
+	def __init__(self):
+		"""Исключение: попытка установки одинаковых индикаторов ключей и флагов."""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "Cannot set same indicators for keys and flags."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+			
+	def __str__(self):
+		return self.__Message
+
+class InvalidArgumentType(Exception):
+	"""Исключение: неверное значение аргумента."""
+
+	def __init__(self, value: str, type_name: str):
+		"""
+		Исключение: неверное значение аргумента.
+			value – значение аргумента;
+			type_name – название ожидаемого типа.
+		"""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + value + "\" isn't \"" + type_name + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+			
+	def __str__(self):
+		return self.__Message
+
+class MutuallyExclusiveFlags(Exception):
+	"""Исключение: активированы взаимоисключающие флаги."""
+
+	def __init__(self, command: str):
+		"""
+		Исключение: активированы взаимоисключающие флаги.
+			command – команда, вызвавшая исключение.
+		"""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + command + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+			
+	def __str__(self):
+		return self.__Message
+
+class MutuallyExclusiveKeys(Exception):
+	"""Исключение: активированы взаимоисключающие ключи."""
+
+	def __init__(self, command: str):
+		"""
+		Исключение: активированы взаимоисключающие ключи.
+			command – команда, вызвавшая исключение.
+		"""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + command + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+		
+			
+	def __str__(self):
+		return self.__Message
+	
+class MutuallyExclusivePositions(Exception):
+	"""Исключение: активированы разные позиции на одном слое."""
+
+	def __init__(self, command: str): 
+		"""
+		Исключение: активированы разные позиции на одном слое.
+			command – команда, вызвавшая исключение.
+		"""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + command + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+		
+	def __str__(self):
+		return self.__Message
+
+class NotEnoughArguments(Exception):
+	"""Исключение: недостаточно аргументов."""
+
+	def __init__(self, command: str):
+		"""
+		Исключение: недостаточно аргументов.
+			command – команда, вызвавшая исключение.
+		"""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + command + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+
+	def __str__(self):
+		return self.__Message
+
+class TooManyArguments(Exception):
+	"""Исключение: слишком много аргументов."""
+
+	def __init__(self, command: str):
+		"""
+		Исключение: слишком много аргументов.
+			command – команда, вызвавшая исключение.
+		"""
+
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + command + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+			
+	def __str__(self):
+		return self.__Message
+
+class UnknownCommand(Exception):
+	"""Исключение: неизвестная комманда."""
+
+	def __init__(self, command: str):
+		"""
+		Исключение: неизвестная комманда.
+			command – команда, вызвавшая исключение.
+		"""
+		
+		# Добавление данных в сообщение об ошибке.
+		self.__Message = "\"" + command + "\"."
+		# Обеспечение доступа к оригиналу наследованного свойства.
+		super().__init__(self.__Message) 
+		
+	def __str__(self):
 		return self.__Message
```

### Comparing `dublib-0.3.1/src/dublib/Methods.py` & `dublib-0.4.0/src/dublib/Methods.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,211 +1,221 @@
-import shutil
-import html
-import json
-import sys
-import os
-import re
-
-#==========================================================================================#
-# >>>>> ФУНКЦИИ РАБОТЫ С СИСТЕМОЙ <<<<< #
-#==========================================================================================#
-
-def CheckPythonMinimalVersion(major: int, minor: int, raise_exception: bool = True) -> bool:
-	"""
-	Проверяет, соответствует ли используемая версия Python минимальной требуемой.
-		major – идентификатор Major-версии Python;
-		minor – идентификатор Minor-версии Python;
-		raise_exception – указывает, как поступать при несоответствии версии: выбрасывать исключение или возвращать значение.
-	"""
-
-	# Состояние: корректна ли версия.
-	IsVersionCorrect = True
-	
-	# Если версия Python старше минимальной требуемой.
-	if sys.version_info < (major, minor): 
-		
-		# Если указано выбросить исключение.
-		if raise_exception == True:
-			# Выброс исключения.
-			raise RuntimeError(f"Python {major}.{minor} or newer is required.")
-
-		else: 
-			# Переключение статуса проверки.
-			IsVersionCorrect = False
-
-	return IsVersionCorrect
-
-def Cls():
-	"""
-	Очищает консоль.
-	"""
-
-	os.system("cls" if os.name == "nt" else "clear")
-
-def MakeRootDirectories(directories: list[str]):
-	"""
-	Создаёт каталоги в текущей корневой директории скрипта.
-		directories – список названий каталогов.
-	"""
-	
-	# Для каждого названия каталога.
-	for Name in directories:
-		# Если каталог не существует, то создать его.
-		if os.path.exists(Name) == False: os.makedirs(Name)
-
-def RemoveFolderContent(path: str):
-	"""
-	Удаляет всё содержимое каталога.
-		path – путь к каталогу.
-	"""
-
-	# Список содержимого в папке.
-	FolderContent = os.listdir(path)
-
-	# Для каждого элемента.
-	for Item in FolderContent:
-
-		# Если элемент является каталогом.
-		if os.path.isdir(path + "/" + Item):
-			# Удаление каталога.
-			shutil.rmtree(path + "/" + Item)
-
-		else:
-			# Удаление файла.
-			os.remove(path + "/" + Item)
-
-def Shutdown():
-	"""
-	Выключает устройство.
-	"""
-
-	# Если устройство работает под управлением ОС семейства Linux.
-	if sys.platform in ["linux", "linux2"]: os.system("sudo shutdown now")
-	# Если устройство работает под управлением ОС семейства Windows.
-	if sys.platform == "win32": os.system("shutdown /s")
-
-#==========================================================================================#
-# >>>>> ФУНКЦИИ ОБРАБОТКИ ТИПОВ ДАННЫХ <<<<< #
-#==========================================================================================#
-
-def CheckForCyrillicPresence(text: str) -> bool:
-	"""
-	Проверяет, имеются ли кирилические символы в строке.
-		text – проверяемая строка.
-	"""
-
-	# Русский алфавит в нижнем регистре.
-	Alphabet = set("абвгдеёжзийклмнопрстуфхцчшщъыьэюя")
-	# Состояние: содержит ли строка кирилические символы.
-	IsTextContainsCyrillicCharacters = not Alphabet.isdisjoint(text.lower())
-
-	return IsTextContainsCyrillicCharacters
-
-def MergeDictionaries(base_dictionary: dict, mergeable_dictionary: dict, overwrite: bool = False) -> dict:
-	"""
-	Объединяет словари.
-		base_dictionary – словарь, в который идёт копирование;
-		mergeable_dictionary – словарь, из котрого идёт копирование;
-		overwrite – указывает, нужно ли перезаписывать значения конфликтующих ключей базового словаря.
-	"""
-
-	# Для каждого ключа.
-	for Key in mergeable_dictionary.keys():
-
-		# Если перезапись отключена и ключ отсутствует в базовом словаре.
-		if overwrite == False and Key not in base_dictionary.keys():
-			# Копирование в базовый словарь ключа и его значения из объединяемого.
-			base_dictionary[Key] = mergeable_dictionary[Key]
-
-		# Если перезапись включена.
-		elif overwrite == True:
-			# Копирование в базовый словарь ключа и его значения из объединяемого.
-			base_dictionary[Key] = mergeable_dictionary[Key]
-
-	return base_dictionary
-
-def RemoveRecurringSubstrings(string: str, substring: str) -> str:
-	"""
-	Удаляет из строки подряд идущие повторяющиеся подстроки.
-		string – строка, из которой удаляются повторы;
-		Substring – удаляемая подстрока.
-	"""
-
-	# Пока в строке находятся повторы указанного символа, удалять их.
-	while substring + substring in string: string = string.replace(substring + substring, substring)
-
-	return string
-
-def ReplaceDictionaryKey(dictionary: dict, old_key: any, new_key: any) -> dict:
-	"""
-	Заменяет ключ в словаре, сохраняя исходный порядок элементов.
-		dictionary – обрабатываемый словарь;
-		old_key – старое название ключа;
-		new_key – новое название ключа.
-	"""
-	
-	# Результат выполнения.
-	Result = dict()
-	# Если ключ не найден, выбросить исключение.
-	if old_key not in dictionary.keys(): raise KeyError(str(old_key))
-
-	# Для каждого ключа.
-	for Key in dictionary.keys():
-
-		# Если текущий ключ совпадает с искомым.
-		if Key == old_key:
-			# Замена ключа новым.
-			Result[new_key] = dictionary[old_key]
-
-		else:
-			# Копирование старой пары ключ-значение.
-			Result[Key] = dictionary[Key]
-
-	return Result
-
-def ReplaceRegexSubstring(origin: str, regex: str, substring: str) -> str:
-	"""
-	Заменяет все вхождения регулярного выражения в строке на подстроку.
-		origin – обрабатываемая строка;
-		regex – регулярное выражение для поиска подстрок;
-		substring – вставляемая подстрока.
-	"""
-
-	# Список совпадений.
-	RegexSubstring = list()
-
-	while re.findall(regex, origin) != []:
-		# Буфер.
-		RegexSubstring = re.findall(regex, origin)
-		# Поиск всех совпадений.
-		RegexSubstring = RegexSubstring[0] if len(RegexSubstring) > 0 else None
-		# Удаление подстроки.
-		if RegexSubstring != None: origin = origin.replace(RegexSubstring, substring)
-
-	return origin
-
-#==========================================================================================#
-# >>>>> ФУНКЦИИ РАБОТЫ С JSON <<<<< #
-#==========================================================================================#
-
-def ReadJSON(path: str) -> dict:
-	"""
-	Читает файл JSON и конвертирует его в словарь.
-		path – путь к файлу.
-	"""
-
-	# Словарь для преобразования.
-	JSON = dict()
-	# Открытие и чтение файла JSON.
-	with open(path, encoding = "utf-8") as FileRead: JSON = json.load(FileRead)
-
-	return JSON
-
-def WriteJSON(path: str, dictionary: dict):
-	"""
-	Записывает стандартизированный JSON файл. Для отступов используются символы табуляции.
-		path – путь к файлу;
-		dictionary – словарь, конвертируемый в формат JSON.
-	"""
-
-	# Запись словаря в JSON файл.
+import shutil
+import html
+import json
+import sys
+import os
+import re
+
+#==========================================================================================#
+# >>>>> ФУНКЦИИ РАБОТЫ С СИСТЕМОЙ <<<<< #
+#==========================================================================================#
+
+def CheckPythonMinimalVersion(major: int, minor: int, raise_exception: bool = True) -> bool:
+	"""
+	Проверяет, соответствует ли используемая версия Python минимальной требуемой.
+		major – идентификатор Major-версии Python;
+		minor – идентификатор Minor-версии Python;
+		raise_exception – указывает, как поступать при несоответствии версии: выбрасывать исключение или возвращать значение.
+	"""
+
+	# Состояние: корректна ли версия.
+	IsVersionCorrect = True
+	
+	# Если версия Python старше минимальной требуемой.
+	if sys.version_info < (major, minor): 
+		
+		# Если указано выбросить исключение.
+		if raise_exception == True:
+			# Выброс исключения.
+			raise RuntimeError(f"Python {major}.{minor} or newer is required.")
+
+		else: 
+			# Переключение статуса проверки.
+			IsVersionCorrect = False
+
+	return IsVersionCorrect
+
+def Cls():
+	"""Очищает консоль."""
+
+	os.system("cls" if os.name == "nt" else "clear")
+
+def MakeRootDirectories(directories: list[str]):
+	"""
+	Создаёт каталоги в текущей корневой директории скрипта.
+		directories – список названий каталогов.
+	"""
+	
+	# Для каждого названия каталога.
+	for Name in directories:
+		# Если каталог не существует, то создать его.
+		if os.path.exists(Name) == False: os.makedirs(Name)
+
+def RemoveFolderContent(path: str):
+	"""
+	Удаляет всё содержимое каталога.
+		path – путь к каталогу.
+	"""
+
+	# Список содержимого в папке.
+	FolderContent = os.listdir(path)
+
+	# Для каждого элемента.
+	for Item in FolderContent:
+
+		# Если элемент является каталогом.
+		if os.path.isdir(path + "/" + Item):
+			# Удаление каталога.
+			shutil.rmtree(path + "/" + Item)
+
+		else:
+			# Удаление файла.
+			os.remove(path + "/" + Item)
+
+def Shutdown():
+	"""Выключает устройство."""
+
+	# Если устройство работает под управлением ОС семейства Linux.
+	if sys.platform in ["linux", "linux2"]: os.system("sudo shutdown now")
+	# Если устройство работает под управлением ОС семейства Windows.
+	if sys.platform == "win32": os.system("shutdown /s")
+
+#==========================================================================================#
+# >>>>> ФУНКЦИИ ОБРАБОТКИ ТИПОВ ДАННЫХ <<<<< #
+#==========================================================================================#
+
+def CheckForCyrillicPresence(text: str) -> bool:
+	"""
+	Проверяет, имеются ли кирилические символы в строке.
+		text – проверяемая строка.
+	"""
+
+	# Русский алфавит в нижнем регистре.
+	Alphabet = set("абвгдеёжзийклмнопрстуфхцчшщъыьэюя")
+	# Состояние: содержит ли строка кирилические символы.
+	IsTextContainsCyrillicCharacters = not Alphabet.isdisjoint(text.lower())
+
+	return IsTextContainsCyrillicCharacters
+
+def IsNotAlpha(text: str) -> bool:
+	"""
+	Проверяет, состоит ли строка целиком из небуквенных символов.
+	"""
+
+	# Результат проверки.
+	Result = True
+
+	# Для каждого символа в строке.
+	for Character in text:
+
+		# Если символ является буквой.
+		if Character.isalpha():
+			# Изменение результата.
+			Result = False
+			# Прерывание цикла.
+			break
+
+	return Result
+
+def MergeDictionaries(base_dictionary: dict, mergeable_dictionary: dict, overwrite: bool = False) -> dict:
+	"""
+	Объединяет словари.
+		base_dictionary – словарь, в который идёт копирование;
+		mergeable_dictionary – словарь, из котрого идёт копирование;
+		overwrite – указывает, нужно ли перезаписывать значения конфликтующих ключей базового словаря.
+	"""
+
+	# Для каждого ключа.
+	for Key in mergeable_dictionary.keys():
+
+		# Если перезапись отключена и ключ отсутствует в базовом словаре.
+		if overwrite == False and Key not in base_dictionary.keys():
+			# Копирование в базовый словарь ключа и его значения из объединяемого.
+			base_dictionary[Key] = mergeable_dictionary[Key]
+
+		# Если перезапись включена.
+		elif overwrite == True:
+			# Копирование в базовый словарь ключа и его значения из объединяемого.
+			base_dictionary[Key] = mergeable_dictionary[Key]
+
+	return base_dictionary
+
+def RemoveRecurringSubstrings(string: str, substring: str) -> str:
+	"""
+	Удаляет из строки подряд идущие повторяющиеся подстроки.
+		string – строка, из которой удаляются повторы;
+		Substring – удаляемая подстрока.
+	"""
+
+	# Пока в строке находятся повторы указанного символа, удалять их.
+	while substring + substring in string: string = string.replace(substring + substring, substring)
+
+	return string
+
+def ReplaceDictionaryKey(dictionary: dict, old_key: any, new_key: any) -> dict:
+	"""
+	Заменяет ключ в словаре, сохраняя исходный порядок элементов.
+		dictionary – обрабатываемый словарь;
+		old_key – старое название ключа;
+		new_key – новое название ключа.
+	"""
+	
+	# Результат выполнения.
+	Result = dict()
+	# Если ключ не найден, выбросить исключение.
+	if old_key not in dictionary.keys(): raise KeyError(str(old_key))
+
+	# Для каждого ключа.
+	for Key in dictionary.keys():
+
+		# Если текущий ключ совпадает с искомым.
+		if Key == old_key:
+			# Замена ключа новым.
+			Result[new_key] = dictionary[old_key]
+
+		else:
+			# Копирование старой пары ключ-значение.
+			Result[Key] = dictionary[Key]
+
+	return Result
+
+def StripAlpha(text: str) -> str:
+	"""
+	Удаляет из строки начальные и конечные небуквенные символы.
+		text – обрабатываемая строка.
+	"""
+
+	try:
+		# Пока по краям строки есть небуквенные символы, удалять их по одному.
+		while not text[0].isalpha(): text.pop(0)
+		while not text[-1].isalpha(): text.pop()
+
+	except:
+		# Очистка строки.
+		text = ""
+
+#==========================================================================================#
+# >>>>> ФУНКЦИИ РАБОТЫ С JSON <<<<< #
+#==========================================================================================#
+
+def ReadJSON(path: str) -> dict:
+	"""
+	Читает файл JSON и конвертирует его в словарь.
+		path – путь к файлу.
+	"""
+
+	# Словарь для преобразования.
+	JSON = dict()
+	# Открытие и чтение файла JSON.
+	with open(path, encoding = "utf-8") as FileRead: JSON = json.load(FileRead)
+
+	return JSON
+
+def WriteJSON(path: str, dictionary: dict):
+	"""
+	Записывает стандартизированный JSON файл. Для отступов используются символы табуляции.
+		path – путь к файлу;
+		dictionary – словарь, конвертируемый в формат JSON.
+	"""
+
+	# Запись словаря в JSON файл.
 	with open(path, "w", encoding = "utf-8") as FileWrite: json.dump(dictionary, FileWrite, ensure_ascii = False, indent = '\t', separators = (",", ": "))
```

### Comparing `dublib-0.3.1/src/dublib/Polyglot.py` & `dublib-0.4.0/src/dublib/Polyglot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-from dublib.Methods import ReplaceRegexSubstring
-
 import html
 import re
 
 class HTML:
-	"""
-	Объектная реализация обработчика HTML.
-	"""
+	"""Объектная реализация обработчика HTML."""
 
 	#==========================================================================================#
 	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
 	#==========================================================================================#
 
 	@property
 	def plain_text(self) -> str:
-		"""
-		Текст без тегов и спецсимволов HTML.
-		"""
+		"""Текст без тегов и спецсимволов HTML."""
 		
 		# Конвертирование спецсимволов HTML в Unicode.
 		PlainText = html.unescape(self.__Text)
 		# Удаление найденных по регулярному выражению тегов.
 		PlainText = str(re.sub(self.__AllTagsRegex, "", PlainText))
 
 		return PlainText
 
 	@property
 	def text(self) -> str:
-		"""
-		Текст.
-		"""
+		"""Текст."""
 
 		return self.__Text
 
 	#==========================================================================================#
 	# >>>>> МЕТОДЫ <<<<< #
 	#==========================================================================================#
 
@@ -49,56 +41,74 @@
 		self.__AllTagsRegex = re.compile('<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});')
 		# Обрабатываемый текст.
 		self.__Text = text	
 
 	def __str__(self) -> str:
 		return self.__Text
 
-	def remove_tags(self):
+	def remove_tags(self, tags: list[str] | None = None):
 		"""
-		Удаляет все теги HTML из текста.
+		Удаляет теги HTML из текста.
+			tags – список тегов, которые необходимо удалить.
 		"""
 
-		# Удаление найденных по регулярному выражению тегов.
-		self.__Text = str(re.sub(self.__AllTagsRegex, "", self.__Text))
+		# Если фильтр не установлен.
+		if tags == None:
+			# Удаление найденных по регулярному выражению тегов.
+			self.__Text = str(re.sub(self.__AllTagsRegex, "", self.__Text))
 
-	def unescape(self):
+		else:
+
+			# Для каждого тега.
+			for Tag in tags:
+				# Удаление открывающих и закрывающих тегов.
+				self.__Text = re.sub(f"<{Tag}[^>]*>", "", self.__Text)
+				self.__Text = re.sub(f"</{Tag}>", "", self.__Text)
+
+	def replace_tag(self, origin: str, new: str):
 		"""
-		Преобразует спецсимволы HTML в Unicode.
+		Заменяет переданный тип тега HTML другим.
+			origin – замещаемый тег;
+			new – новый тег.
 		"""
 
+		# Поиск открывающих тегов.
+		Matches = re.findall(f"<{origin}[^>]*>", self.__Text)
+		# Для каждого совпадения произвести замену.
+		for Match in Matches: self.__Text = self.__Text.replace(f"<{origin}", f"<{new}")
+		# Замена закрывающих тегов.
+		self.__Text = re.sub(f"</{origin}>", f"</{new}>", self.__Text)
+
+	def unescape(self):
+		"""Преобразует спецсимволы HTML в Unicode."""
+
 		# Конвертирование спецсимволов HTML в Unicode.
 		self.__Text = html.unescape(self.__Text)
 
 class Markdown:
-	"""
-	Объектная реализация обработчика Markdown.
-	"""
+	"""Объектная реализация обработчика Markdown."""
 
 	#==========================================================================================#
 	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
 	#==========================================================================================#
 
 	@property
 	def escaped_text(self) -> str:
-		"""
-		Текст с экранированными спецсимволами.
-		"""
+		"""Текст с экранированными спецсимволами."""
+
 		# Буфер текста.
 		Text = self.__Text
 		# Для каждого спецсимвола провести экранирование.
-		for Character in self.__SpecialCharacters: Text = ReplaceRegexSubstring(Text, f"(?<!\\\\)\\{Character}", f"\\{Character}")
+		for Character in self.__SpecialCharacters: Text = re.sub(f"(?<!\\\\)\\{Character}", f"\\{Character}", self.__Text)
 
 		return Text
 
 	@property
 	def text(self) -> str:
-		"""
-		Текст.
-		"""
+		"""Текст."""
 
 		return self.__Text
 
 	#==========================================================================================#
 	# >>>>> МЕТОДЫ <<<<< #
 	#==========================================================================================#
 
@@ -115,13 +125,11 @@
 		# Список спецсимволов.
 		self.__SpecialCharacters = ['_', '*', '[', ']', '(', ')', '~', '`', '>', '#', '+', '-', '=', '|', '{', '}', '.', '!']
 
 	def __str__(self) -> str:
 		return self.__Text
 
 	def escape(self):
-		"""
-		Экранирует спецсимволы.
-		"""
+		"""Экранирует спецсимволы."""
 
 		# Для каждого спецсимвола провести экранирование.
-		for Character in self.__SpecialCharacters: self.__Text = ReplaceRegexSubstring(self.__Text, f"(?<!\\\\)\\{Character}", f"\\{Character}")
+		for Character in self.__SpecialCharacters: self.__Text = re.sub(f"(?<!\\\\)\\{Character}", f"\\{Character}", self.__Text)
```

### Comparing `dublib-0.3.1/src/dublib/StyledPrinter.py` & `dublib-0.4.0/src/dublib/StyledPrinter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,42 @@
-from dublib.Exceptions.StyledPrinter import DuplicatedStyles
+from .Exceptions.StyledPrinter import DuplicatedStyles
 
 import enum
 
 class Styles:
-	"""
-	Содержит перечисления декораций и стилей.
-	"""
+	"""Содержит перечисления декораций и стилей."""
 
 	class Colors(enum.Enum):
-		"""
-		Перечисление цветов.
-		"""
+		"""Перечисление цветов."""
 
 		Black = "0"
 		Red = "1"
 		Green = "2"
 		Yellow = "3"
 		Blue = "4"
 		Purple = "5"
 		Cyan = "6"
 		White = "7"
 
 	class Decorations(enum.Enum):
-		"""
-		Перечисление декораций.
-		"""
+		"""Перечисление декораций."""
 
 		Bold = "1"
 		Faded = "2"
 		Italic = "3"
 		Underlined = "4"
 		Flashing = "5"
 		Throughline = "9"
 		DoubleUnderlined = "21"
 		Framed = "51"
 		Surrounded = "52"
 		Upperlined = "53"
 
 class StylesGroup:
-	"""
-	Контейнер стилей. Предоставляет возможность комбинировать стили для их однократной инициализации с последующим многократным использования.
-	"""
+	"""Контейнер стилей. Предоставляет возможность комбинировать стили для их однократной инициализации с последующим многократным использования."""
 
 	def __init__(self, decorations: list[Styles.Decorations] = list(), text_color: Styles.Colors | None = None, background_color: Styles.Colors | None = None):
 		"""
 		Контейнер стилей. Предоставляет возможность комбинировать стили для их однократной инициализации с последующим многократным использования.
 			decorations – список декораций;
 			text_color – цвет текста;
 			background_color – цвет фона.
@@ -52,15 +44,15 @@
 
 		#---> Генерация динамических свойств.
 		#==========================================================================================#
 		# Строка маркеров стилей.
 		self.__StylesMarkers = "\033["
 
 		# Добавить каждый маркер стиля к общей строке.
-		for Decoration in decorations: self.__StylesMarkers += Decoration + ";"
+		for Decoration in decorations: self.__StylesMarkers += Decoration.value + ";"
 		# Если передан цвет текста, создать соответствующий маркер.
 		if TextColor != None: self.__StylesMarkers += "3" + TextColor.value + ";"
 		# Если передан цвет фона, создать соответствующий маркер.
 		if BackgroundColor != None: self.__StylesMarkers += "4" + BackgroundColor.value + ";"
 		# Постановка завершающего символа маркировки.
 		self.__StylesMarkers = self.__StylesMarkers.rstrip(';') + "m"
 
@@ -108,15 +100,15 @@
 
 	# Если не указана группа стилей.
 	if styles == None:
 		# Инициализация маркера стилей строки.
 		StyleMarkers = "\033["
 
 		# Добавить каждую декорацию.
-		for Decoration in decorations: StyleMarkers += Decoration + ";"
+		for Decoration in decorations: StyleMarkers += Decoration.value + ";"
 		# Если передан цвет текста, создать соответствующий маркер.
 		if text_color != None: StyleMarkers += "3" + text_color.value + ";"
 		# Если передан цвет фона, создать соответствующий маркер.
 		if background_color != None: StyleMarkers += "4" + background_color.value + ";"
 		# Постановка завершающего символа маркировки.
 		StyleMarkers = StyleMarkers.rstrip(';') + "m"
```

### Comparing `dublib-0.3.1/src/dublib/Terminalyzer.py` & `dublib-0.4.0/src/dublib/Terminalyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,119 +1,96 @@
-from dublib.Exceptions.Terminalyzer import *
-from dublib.Methods import ReadJSON
+from .Exceptions.Terminalyzer import *
+from .Methods import ReadJSON
+
 from urllib.parse import urlparse
 
 import enum
 import sys
 import os
 
 #==========================================================================================#
 # >>>>> ВСПОМОГАТЕЛЬНЫЕ ТИПЫ ДАННЫХ <<<<< #
 #==========================================================================================#
 
 class ArgumentsTypes(enum.Enum):
-	"""
-	Перечисление типов аргументов.
-	"""
+	"""Перечисление типов аргументов."""
 
 	All = "all"
 	Number = "number"
 	ValidPath = "validpath"
 	Text = "text"
 	URL = "url"
 	
 class Command:
-	"""
-	Контейнер описания команды.
-	"""
+	"""Контейнер описания команды."""
 
 	#==========================================================================================#
 	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
 	#==========================================================================================#
 
 	@property
 	def arguments(self) -> list:
-		"""
-		Список аргументов.
-		"""
+		"""Список аргументов."""
 
 		return self.__Arguments
 	
 	@property
 	def description(self) -> str:
-		"""
-		Описание команды.
-		"""
+		"""Описание команды."""
 
 		return self.__Description
 
 	@property
 	def flags_indicator(self) -> str:
-		"""
-		Индикатор флагов.
-		"""
+		"""Индикатор флагов."""
 
 		return self.__FlagIndicator
 
 	@property
 	def flags_positions(self) -> list:
-		"""
-		Список позиций флагов.
-		"""
+		"""Список позиций флагов."""
 
 		return self.__FlagsPositions
 	
 	@property
 	def keys_indicator(self) -> str:
-		"""
-		Индикатор ключей.
-		"""
+		"""Индикатор ключей."""
 
 		return self.__KeyIndicator
 	
 	@property
 	def keys_positions(self) -> list:
-		"""
-		Список позиций ключей.
-		"""
+		"""Список позиций ключей."""
 
 		return self.__KeysPositions
 	
 	@property
 	def max_parameters(self) -> int:
-		"""
-		Максимальное количество параметров.
-		"""
+		"""Максимальное количество параметров."""
 
 		return self.__MaxArgc
 
 	@property
 	def min_parameters(self) -> int:
-		"""
-		Минимальное количество параметров.
-		"""
+		"""Минимальное количество параметров."""
 
 		return self.__MinArgc
  
 	@property
 	def name(self) -> str:
-		"""
-		Название команды.
-		"""
+		"""Название команды."""
 
 		return self.__Name
 
 	#==========================================================================================#
 	# >>>>> МЕТОДЫ <<<<< #
 	#==========================================================================================#
 
 	def __CalculateMaxParameters(self):
-		"""
-		Подсчитывает максимальное количество параметров.
-		"""
+		"""Подсчитывает максимальное количество параметров."""
 
 		# Обнуление максимального количества параметров.
 		self.__MaxArgc = 0
 
 		# Для каждой позиции флага.
 		for FlagsPostionIngex in range(0, len(self.__FlagsPositions)):
 
@@ -138,17 +115,15 @@
 				self.__MaxArgc += 2
 
 			else:
 				# Посчитать слой за 1 параметр.
 				self.__MaxArgc += 1
 
 	def __CalculateMinParameters(self):
-		"""
-		Подсчитывает минимальное количество параметров.
-		"""
+		"""Подсчитывает минимальное количество параметров."""
 
 		# Обнуление минимального количества параметров.
 		self.__MinArgc = 0
 		
 		# Для каждой позиции флага.
 		for FlagsPostionIngex in range(0, len(self.__FlagsPositions)):
 			
@@ -216,15 +191,16 @@
 
 			# Если аргумент лежит на важном слое, сделать его важным.
 			if self.__Arguments[ArgumentIndex]["layout-index"] == layout_index: self.__Arguments[ArgumentIndex]["important"] = True
 	
 	def __init__(self, name: str, description: str | None = None):
 		"""
 		Контейнер описания команды.
-			name – название команды.
+			name – название команды;
+			description – описание команды.
 		"""
 
 		#---> Генерация динамических свойств.
 		#==========================================================================================#
 		# Список флагов.
 		self.__FlagsPositions = list()
 		# Список ключей.
@@ -440,17 +416,15 @@
 			self.__KeyIndicator = indicator
 
 		else:
 			# Выброс исключения.
 			raise IdenticalIndicators()
 
 class CommandData:
-	"""
-	Контейнер хранения данных обработанной команды.
-	"""
+	"""Контейнер хранения данных обработанной команды."""
 
 	def __init__(self, name: str, flags: list[str] = list(), keys: list[str] = list(), values: dict[str, str] = dict(), arguments: list[str] = list()):
 		"""
 		Контейнер хранения данных обработанной команды.
 			name – название команды;
 			flags – список активированных флагов;
 			keys – список активированных ключей;
@@ -477,27 +451,23 @@
 			"flags": self.flags, 
 			"keys": self.keys, 
 			"values": self.values, 
 			"arguments": self.arguments
 		})
 
 class Config:
-	"""
-	JSON-конфигурация команд.
-	"""
+	"""JSON-конфигурация команд."""
 
 	#==========================================================================================#
 	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
 	#==========================================================================================#
 
 	@property
 	def arguments_types(self) -> dict:
-		"""
-		Словарь строковых и классовых представлений типов аргументов.
-		"""
+		"""Словарь строковых и классовых представлений типов аргументов."""
 
 		return {
 			"all": ArgumentsTypes.All,
 			"number": ArgumentsTypes.Number,
 			"validpath": ArgumentsTypes.ValidPath,
 			"text": ArgumentsTypes.Text,
 			"url": ArgumentsTypes.URL,
@@ -534,28 +504,27 @@
 		if len(Types) == 1: Types = Types[0]
 
 		return Types
 
 	def __init__(self, path: str | None = None):
 		"""
 		JSON-конфигурация команд.
+			path – путь к файлу конфигурации.
 		"""
 
 		#---> Генерация динамических свойств.
 		#==========================================================================================#
 		# Конфигурация.
 		self.__Config = None
 
 		# Если указан путь к файлу, прочитать его.
 		if path != None: self.read(path)
 
 	def build_commands(self) -> list[Command]:
-		"""
-		Строит список описаний команд из конфигурации.
-		"""
+		"""Строит список описаний команд из конфигурации."""
 
 		# Список описательных структур команд.
 		CommandsList = list()
 
 		# Для каждой команды.
 		for CommandName in self.__Config["commands"].keys():
 			# Буфер обрабатываемой команды.
@@ -642,17 +611,15 @@
 		self.__Config = ReadJSON(path)
 
 #==========================================================================================#
 # >>>>> ОСНОВНОЙ КЛАСС <<<<< #
 #==========================================================================================#
 
 class Terminalyzer:
-	"""
-	Обработчик консольных аргументов.
-	"""
+	"""Обработчик консольных аргументов."""
 
 	def __CheckArgc(self, command: Command):
 		"""
 		Проверяет соответвтсие количества аргументов.
 			command – описательная структура команды.
 		"""
 
@@ -713,15 +680,15 @@
 				# Если параметр соответствует типу.
 				if self.__CheckArgumentsTypes(FreeParameters[Index], ArgumentsDescription[Index]["type"]) == True:
 					# Сохранение параметра в качестве аргумента.
 					Values.append(FreeParameters[Index])
 
 				else:
 					# Выброс исключения.
-					raise InvalidArgumentsTypes(FreeParameters[Index], command.arguments["type"])
+					raise InvalidArgumentType(FreeParameters[Index], command.arguments["type"])
 				
 			else:
 				# Сохранение пустого значения аргумента.
 				Values.append(None)
 
 		return Values
 	
@@ -735,33 +702,33 @@
 		# Если требуется проверить специфический тип аргумента.
 		if type_name != ArgumentsTypes.All:
 			
 			# Если аргумент должен являться числом.
 			if type_name == ArgumentsTypes.Number:
 
 				# Если вся строка, без учёта отрицательного знака, не является числом, выбросить исключение.
-				if value.lstrip('-').isdigit() == False: raise InvalidArgumentsTypes(value, "Number")
+				if value.lstrip('-').isdigit() == False: raise InvalidArgumentType(value, "Number")
 				
 			# Если аргумент должен являться валидным путём к файлу или директории.
 			if type_name == ArgumentsTypes.ValidPath:
 
 				# Если строка не является валидным путём к файлу или директории, выбросить исключение.
-				if os.path.exists(value) == False: raise InvalidArgumentsTypes(value, "ValidPath")
+				if os.path.exists(value) == False: raise InvalidArgumentType(value, "ValidPath")
 
 			# Если аргумент должен являться набором букв.
 			if type_name == ArgumentsTypes.Text:
 
 				# Если строка содержит небуквенные символы, выбросить исключение.
-				if value.isalpha() == False: raise InvalidArgumentsTypes(value, "Text")
+				if value.isalpha() == False: raise InvalidArgumentType(value, "Text")
 
 			# Если аргумент должен являться URL.
 			if type_name == ArgumentsTypes.URL:
 
 				# Если строка не является URL, выбросить исключение.
-				if bool(urlparse(value).scheme) == False: raise InvalidArgumentsTypes(value, "URL")
+				if bool(urlparse(value).scheme) == False: raise InvalidArgumentType(value, "URL")
 
 		return True
 
 	def __CheckCommand(self, command: Command) -> CommandData | None:
 		"""
 		Выполняет проверку соответствия конкретной команде.
 			command – описательная структура команды.
```

### Comparing `dublib-0.3.1/src/dublib/WebRequestor.py` & `dublib-0.4.0/src/dublib/WebRequestor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,804 +1,635 @@
-from fake_useragent import UserAgent as UserAgentGenerator
-from dublib.Exceptions.WebRequestor import *
-
-import importlib
-import requests
-import logging
-import random
-import httpx
-import enum
-
-#==========================================================================================#
-# >>>>> ВСПОМОГАТЕЛЬНЫЕ ТИПЫ ДАННЫХ <<<<< #
-#==========================================================================================#
-
-class Browsers(enum.Enum):
-	"""
-	Перечисление типов поддерживаемых браузеров.
-	"""
-
-	Chrome = "Google Chrome"
-	#Firefox = "Mozilla Firefox"
-	#Edge = "Microsoft Edge"
-
-class Protocols(enum.Enum):
-	"""
-	Перечисление типов протоколов.
-	"""
-	
-	FTP = "ftp"
-	HTTP = "http"
-	HTTPS = "https"
-	SOCKS = "socks"
-
-class HttpxConfig:
-	"""
-	Конфигурация библиотеки httpx.
-	"""
-	
-	#==========================================================================================#
-	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
-	#==========================================================================================#
-	
-	@property
-	def headers(self) -> dict:
-		return self.__Headers.copy()
-	
-	@property
-	def http2(self) -> bool:
-		return self.__HTTP2
-	
-	@property
-	def redirecting(self) -> bool:
-		return self.__Redirecting
-	
-	#==========================================================================================#
-	# >>>>> МЕТОДЫ <<<<< #
-	#==========================================================================================#
-
-	def __init__(self, auto_user_agent: bool = True):
-		"""
-		Конфигурация библиотеки httpx.
-			auto_user_agent – переключает автоматическую генерацию заголовка User-Agent.
-		"""
-		
-		#---> Генерация динамических свойств.
-		#==========================================================================================#
-		# Заголовки запросов.
-		self.__Headers = dict()
-		# Состояние: выполнять ли переадресацию.
-		self.__Redirecting = True
-		# Состояние: использовать ли HTTP2.0.
-		self.__HTTP2 = True
-		
-		# Если указано, сгенерировать заголовок User-Agent.
-		if auto_user_agent == True: self.__Headers = {"User-Agent": UserAgentGenerator().chrome}
-		
-	def add_header(self, key: str, value: int | str):
-		"""
-		Добавляет пользовательский заголовок запроса.
-			key – ключ заголовка;
-			value – значение заголовка.
-		"""
-
-		# Запись заголовка.
-		self.__Headers[key] = value
-		
-	def enable_http2(self, status: bool):
-		"""
-		Переключает использование протокола HTTP2.0.
-			status – статус использования протокола.
-		"""
-		
-		self.__HTTP2 = status
-		
-	def enable_redirecting(self, status: bool):
-		"""
-		Переключает автоматическое перенаправление HTTP.
-			status – статус перенаправления.
-		"""
-		
-		self.__Redirecting = status
-		
-	def set_referer(self, referer: str):
-		"""
-		Задаёт пользовательское значение заголовка Referer.
-			referer – новое значение заголовка.
-		"""
-
-		self.__Headers["Referer"] = referer
-		
-	def set_user_agent(self, user_agent: str):
-		"""
-		Задаёт пользовательское значение заголовка User-Agent.
-			user_agent – новое значение заголовка.
-		"""
-
-		self.__Headers["User-Agent"] = user_agent
-
-class RequestsConfig:
-	"""
-	Конфигурация библиотеки requests.
-	"""
-	
-	#==========================================================================================#
-	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
-	#==========================================================================================#
-	
-	@property
-	def headers(self) -> dict:
-		return self.__Headers.copy()
-	
-	@property
-	def redirecting(self) -> bool:
-		return self.__Redirecting
-	
-	#==========================================================================================#
-	# >>>>> МЕТОДЫ <<<<< #
-	#==========================================================================================#
-
-	def __init__(self, auto_user_agent: bool = True):
-		"""
-		Конфигурация библиотеки requests.
-			auto_user_agent – переключает автоматическую генерацию заголовка User-Agent.
-		"""
-		
-		#---> Генерация динамических свойств.
-		#==========================================================================================#
-		# Заголовки запросов.
-		self.__Headers = dict()
-		# Состояние: выполнять ли переадресацию.
-		self.__Redirecting = True
-		
-		# Если указано, сгенерировать заголовок User-Agent.
-		if auto_user_agent == True: self.__Headers = {"User-Agent": UserAgentGenerator().chrome}
-		
-	def add_header(self, key: str, value: int | str):
-		"""
-		Добавляет пользовательский заголовок запроса.
-			key – ключ заголовка;
-			value – значение заголовка.
-		"""
-
-		# Запись заголовка.
-		self.__Headers[key] = Value
-		
-	def enable_redirecting(self, status: bool):
-		"""
-		Переключает автоматическое перенаправление HTTP.
-			status – статус перенаправления.
-		"""
-		
-		self.__Redirecting = status
-		
-	def set_referer(self, referer: str):
-		"""
-		Задаёт пользовательское значение заголовка Referer.
-			referer – новое значение заголовка.
-		"""
-
-		self.__Headers["Referer"] = referer
-		
-	def set_user_agent(self, user_agent: str):
-		"""
-		Задаёт пользовательское значение заголовка User-Agent.
-			user_agent – новое значение заголовка.
-		"""
-
-		self.__Headers["User-Agent"] = user_agent
-	
-class SeleniumConfig:
-	"""
-	Конфигурация библиотеки Selenium.
-	"""
-	
-	def __init__(
-			self,
-			browser_type: Browsers = Browsers.Chrome,
-			headless: bool = False,
-			page_load_timeout: int = 75,
-			script_timeout: int = 75,
-			window_width: int = 1920,
-			WindowHeight: int = 1080
-		):
-		"""
-		Конфигурация библиотеки Selenium.
-			browser_type – наименование используемого браузера;
-			headless – переключатель безоконного режима;
-			page_load_timeout – тайм-аут загрузки страницы;
-			script_timeout – тайм-аут выполнения JavaScript;
-			window_width – ширина окна;
-			window_height – высота окна.
-		"""
-		
-		#---> Генерация динамических свойств.
-		#==========================================================================================#
-		# Тип используемого браузера.
-		self.BrowserType = browser_type
-		# Состояние: активен ли безрабочный режим.
-		self.Headless = headless
-		# Тайм-аут загрузки страницы.
-		self.PageLoadTimeout = page_load_timeout
-		# Тайм-аут выполнения JavaScript.
-		self.ScriptTimeout = script_timeout
-		# Ширина окна.
-		self.WindowWidth = window_width
-		# Высота окна.
-		self.WindowHeight = window_height
-		
-	def set_browser_type(self, browser_type: Browsers):
-		"""
-		Задаёт используемый браузер.
-			BrowserType – браузер.
-		"""
-
-		self.BrowserType = browser_type
-		
-	def set_headless(self, status: bool):
-		"""
-		Переключает отображение окна браузера.
-			status – состояние отображение окна браузера.
-		"""
-
-		self.Headless = status
-		
-	def set_page_load_timeout(self, page_load_timeout: int):
-		"""
-		Задаёт тайм-аут загрузки страницы.
-			page_load_timeout – тайм-аут загрузки страницы в секундах.
-		"""
-
-		self.PageLoadTimeout = page_load_timeout
-		
-	def set_script_timeout(self, script_timeout: int):
-		"""
-		Задаёт тайм-аут выполнения JavaScript.
-			script_timeout – тайм-аут выполнения JavaScript в секундах.
-		"""
-
-		self.ScriptTimeout = script_timeout
-		
-	def set_window_size(self, width: int, height: int):
-		"""
-		Задаёт размер окна браузера.
-			width – ширина окна в пикселях;
-			height – высота окна в пикселях.
-		"""
-
-		self.WindowWidth = width
-		self.WindowHeight = height
-		
-class WebResponse:
-	"""
-	Эмуляция структуры ответа библиотеки requests.
-	"""
-
-	def __init__(self):
-		"""
-		Эмуляция структуры ответа библиотеки requests.
-		"""
-
-		#---> Генерация динамических свойств.
-		#==========================================================================================#
-		# Статус ответа.
-		self.status_code = None
-		# Бинарное представление ответа.
-		self.content = None
-		# Текстовое представление ответа.
-		self.text = None
-		
-#==========================================================================================#
-# >>>>> ОСНОВНОЙ КЛАСС <<<<< #
-#==========================================================================================#
-
-class WebRequestor:
-	"""
-	Запросчик HTML кода веб-страниц.
-	"""
-	
-	#==========================================================================================#
-	# >>>>> ВСПОМОГАТЕЛЬНЫЕ МЕТОДЫ <<<<< #
-	#==========================================================================================#
-
-	def __CheckConfig(self):
-		"""
-		Выбрасывает исключение при отсутствии конфигурации.
-		"""
-
-		# Если конфигурация не задана, выбросить исключение.
-		if self.__Config == None: raise ConfigRequired()
-		
-	def __GetProxy(self) -> dict | None:
-		"""
-		Возвращает объект прокси для запроса.
-		"""
-		
-		# Объект прокси.
-		Proxy = None
-		
-		# Если задан хотя бы один прокси..
-		if len(self.__Proxies) > 0:
-			# Случайный выбор прокси.
-			Proxy = random.choice(self.__Proxies)
-			# Данные авторизации.
-			Auth = ""
-			# Если указаны логин и пароль, составить авторизационные данные.
-			if Proxy["login"] != None and Proxy["password"] != None: Auth = Proxy["login"] + ":" + Proxy["password"] + "@"
-					
-			# Если задана конфигурация requests.		
-			if type(self.__Config) == RequestsConfig:
-				# Создание объекта прокси.
-				Proxy = {
-					Proxy["protocol"]: Proxy["protocol"].replace("https", "http") + "://" + Auth + Proxy["host"] + ":" + Proxy["port"]
-				}
-			
-			# Если задана конфигурация httpx.		
-			if type(self.__Config) == HttpxConfig:
-				# Создание объекта прокси.
-				Proxy = {
-					Proxy["protocol"] + "://": Proxy["protocol"].replace("https", "http") + "://" + Auth + Proxy["host"] + ":" + Proxy["port"]
-				}
-			
-		return Proxy
-	
-	def __InitializeChrome(self):
-		"""
-		Инициализирует браузер Google Chrome.
-		"""
-
-		# Закрытие браузера.
-		self.close()
-		# Опции веб-браузера.
-		ChromeOptions = self.Options.Options()
-		# Установка опций.
-		ChromeOptions.add_argument("--no-sandbox")
-		ChromeOptions.add_argument("--disable-dev-shm-usage")
-		ChromeOptions.add_argument("--disable-gpu")
-		ChromeOptions.add_experimental_option("excludeSwitches", ["enable-logging"])
-		# При отключённом режиме отладки скрыть окно браузера.
-		if self.__Config.Headless == True: ChromeOptions.add_argument("--headless=new")
-		# Инициализация браузера.
-		self.__Browser = self.selenium.webdriver.Chrome(service = self.Service.Service(self.ChromeDriverManager.ChromeDriverManager().install()), options = ChromeOptions)
-		# Установка размера окна браузера на FullHD для корректной работы сайтов.
-		self.__Browser.set_window_size(self.__Config.WindowWidth, self.__Config.WindowHeight)
-		# Установка максимального времени загрузки страницы и выполнения скрипта.
-		self.__Browser.set_page_load_timeout(self.__Config.PageLoadTimeout)
-		self.__Browser.set_script_timeout(self.__Config.ScriptTimeout)
-
-	def __ProcessHeaders(self, headers: dict | None) -> dict | None:
-		"""
-		Обрабатывает заголовки перед выполнением запроса.
-		"""
-
-		# Если переданы заголовки.
-		if headers != None:
-			# Объединение словарей заголовков из конфигурации и аргументов.
-			headers = self.__Config.headers | headers
-			
-		else:
-			# Установка словаря заголовков из конфигурации.
-			headers = self.__Config.headers
-
-		return headers
-		
-	#==========================================================================================#
-	# >>>>> МЕТОДЫ ЗАПРОСОВ <<<<< #
-	#==========================================================================================#
-
-	def __httpx_GET(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None) -> httpx.Response:
-		"""
-		Отправляет GET запрос через библиотеку httpx.
-			url – адрес запроса;
-			params – словарь параметров запроса;
-			headers – словарь заголовков;
-			cookies – словарь куков.
-		"""
-
-		# Обработка заголовков.
-		headers = self.__ProcessHeaders(headers)
-		# Ответ.
-		Response = self.__Client.get(url, params = params, headers = headers, cookies = cookies, follow_redirects = self.__Config.redirecting)
-		
-		return Response
-	
-	def __httpx_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> httpx.Response:
-		"""
-		Отправляет POST запрос через библиотеку httpx.
-			url – адрес запроса;
-			params – словарь параметров запроса;
-			headers – словарь заголовков;
-			cookies – словарь куков;
-			data – данные запроса;
-			json – сериализованное тело запроса.
-		"""
-		
-		# Обработка заголовков.
-		headers = self.__ProcessHeaders(headers)
-		# Ответ.
-		Response = self.__Client.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, follow_redirects = self.__Config.redirecting)
-		
-		return Response
-		
-	def __requests_GET(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None) -> requests.Response:
-		"""
-		Отправляет GET запрос через библиотеку requests.
-			url – адрес запроса;
-			params – словарь параметров запроса;
-			headers – словарь заголовков;
-			cookies – словарь куков.
-		"""
-		
-		# Обработка заголовков.
-		headers = self.__ProcessHeaders(headers)
-		# Ответ.
-		Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting)
-		
-		return Response
-	
-	def __requests_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> requests.Response:
-		"""
-		Отправляет POST запрос через библиотеку requests.
-			url – адрес запроса;
-			params – словарь параметров запроса;
-			headers – словарь заголовков;
-			cookies – словарь куков;
-			data – данные запроса;
-			json – сериализованное тело запроса.
-		"""
-		
-		# Обработка заголовков.
-		headers = self.__ProcessHeaders(headers)
-		# Ответ.
-		Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting)
-		
-		return Response
-	
-	def __selenium_LOAD(self, url: str) -> WebResponse:
-		"""
-		Загружает страницу при помощи библиотеки Selenium.
-			URL – адрес страницы.
-		"""
-
-		# Ответ.
-		Response = WebResponse()
-		
-		try:
-			# Запрос страницы.
-			self.__Browser.get(url)
-			
-		except self.TimeoutException.TimeoutException:
-			# Установка свойств ответа.
-			Response.status_code = 408
-			
-		except Exception:
-			# Установка свойств ответа.
-			Response.status_code = 499
-			
-		else:
-			# Установка свойств ответа.
-			Response.status_code = 200
-			Response.text = self.__Browser.execute_script("return document.body.innerHTML;")
-			Response.content = bytes(Response.text)
-		
-		return Response
-			
-	def __init__(self, logging: bool = False):
-		"""
-		Запросчик HTML кода веб-страниц.
-			logging – переключает ведение логов при помощи стандартного модуля.
-		"""
-
-		#---> Генерация динамических свойств.
-		#==========================================================================================#
-		# Конфигурация.
-		self.__Config = None
-		# Сессия запросов httpx.
-		self.__Session = None
-		# Клиент запросов httpx.
-		self.__Client = None
-		# Экземпляр веб-браузера Selenium.
-		self.__Browser = None
-		# Состояние: вести ли логи.
-		self.__Logging = logging
-		# Список прокси.
-		self.__Proxies = list()
-		
-	#==========================================================================================#
-	# >>>>> ОБЩИЕ МЕТОДЫ <<<<< #
-	#==========================================================================================#
-		
-	def close(self):
-		"""
-		Закрывает запросчик.
-		"""
-
-		# Если задана конфигурация Selenium.
-		if type(self.__Config) == SeleniumConfig:
-			
-			try:
-				# Закрытие браузера.
-				self.__Browser.close()
-				self.__Browser.quit()
-				# Обнуление экземпляра.
-				self.__Browser = None
-			
-			except Exception:
-				pass
-			
-		# Если задана конфигурация requests.
-		if type(self.__Config) == RequestsConfig:
-			# Закрытие сессии.
-			self.__Session.close()
-			# Обнуление сессии.
-			self.__Session = None
-			
-		# Если задана конфигурация httpx.
-		if type(self.__Config) == HttpxConfig:
-			# Закрытие клиента.
-			self.__Client.close()
-			# Обнуление клиента.
-			self.__Client = None
-			
-	def add_proxy(self, protocol: Protocols, host: str, port: int | str, login: str | None = None, password: str | None = None):
-		"""
-		Добавляет прокси для использования в запросах. Не работает с Selenium.
-			protocol – протокол прокси-соединения;
-			host – IP или адрес хоста;
-			port – порт сервера;
-			login – логин для авторизации;
-			password – пароль для авторизации.
-		"""
-		
-		# Добавление прокси.
-		self.__Proxies.append({
-			"protocol": protocol.value,
-			"host": host,
-			"port": str(port),
-			"login": login,
-			"password": password
-		})
-			
-	def initialize(self, config: HttpxConfig | RequestsConfig | SeleniumConfig = RequestsConfig()):
-		"""
-		Задаёт конфигурацию и инициализирует модуль запросов. Вызывать после всех настроек.
-			config – конфигурация.
-		"""
-
-		# Если задана конфигурация Selenium.
-		if type(config) == SeleniumConfig:
-			# Сохранение конфигурации.
-			self.__Config = config
-			
-			try:
-				# Динамический импорт пакетов.
-				self.Options = importlib.import_module("selenium.webdriver.chrome.option")
-				self.Service = importlib.import_module("selenium.webdriver.chrome.service")
-				self.ChromeDriverManager = importlib.import_module("webdriver_manager.chrome")
-				self.TimeoutException = importlib.import_module("selenium.common.exceptions")
-				
-			except:
-				raise SeleniumRequired()
-			
-			# Инициализация выбранного браузера.
-			match config.BrowserType:
-				
-				case Browsers.Chrome: self.__InitializeChrome()
-					
-		# Если задана конфигурация requests.		
-		if type(config) == RequestsConfig:
-			# Сохранение конфигурации.
-			self.__Config = config
-			# Инициализация сессии.
-			self.__Session = requests.Session()
-			
-		# Если задана конфигурация httpx.		
-		if type(config) == HttpxConfig:
-			# Сохранение конфигурации.
-			self.__Config = config
-			# Инициализация клиента.
-			self.__Client = httpx.Client(http2 = config.http2, proxies = self.__GetProxy())
-	
-	#==========================================================================================#
-	# >>>>> SELENIUM <<<<< #
-	#==========================================================================================#
-
-	def execute_script(self, script: str, use_async: bool = False, tries: int = 3) -> WebResponse:
-		"""
-		Выполняет JavaScript на текущей странице браузера. Требуется инициализация библиотеки Selenium!
-			script – исполняемый код;
-			use_async – указывает, необходимо ли выполнить скрипт асинхронно;
-			tries – количество попыток повтора при неудачном выполнении.
-		Примечание:
-			Требуется инициализация библиотеки Selenium!
-		"""
-
-		# Ответ.
-		Response = WebResponse()
-		
-		# Если веб-драйвер инициализирован.
-		if self.__Browser != None:
-			# Результат выполнения скрипта.
-			Result = None
-			# Количество повторов.
-			CurrentTry = 0
-			# Состояние: вернул ли скрипт ответ.
-			IsLoaded = False
-		
-			# Повторять, пока скрипт не вернёт ответ.
-			while IsLoaded == False:
-				
-				try:
-					# Выполнение скрипта и запись результата.
-					Result = self.__Browser.execute_async_script(script) if use_async == True else self.__Browser.execute_script(script)
-				
-				except self.TimeoutException.TimeoutException:
-					# Установка свойств ответа.
-					Response.status_code = 408
-					
-				except Exception:
-					# Инкремент количества повторов.
-					CurrentTry += 1
-					# Установка свойств ответа.
-					Response.status_code = 400
-					
-					# Если достигнуто максимальное количество повторов, остановить повторные запросы.
-					if CurrentTry == tries:
-						break
-			
-				else:
-					# Переключение статуса выполнения скрипта.
-					IsLoaded = True
-					# Установка свойств ответа.
-					Response.status_code = 200
-					Response.text = Result
-					Response.content = bytes(Result)
-					
-			else:
-				# Выброс исключения.
-				raise SeleniumRequired()
-				
-		return Response
-	
-	def get_browser_handler(self) -> any:
-		"""
-		Возвращает дескриптор экземпляра браузера.
-			URL – адрес страницы;
-			TriesCount – количество попыток повтора при неудачном выполнении.
-		Примечание:
-			Требуется инициализация библиотеки Selenium!
-		"""
-
-		# Если веб-драйвер не инициализирован, выбросить исключение.
-		if self.__Browser == None: raise SeleniumRequired()
-		
-		return self.__Browser
-	
-	def load(self, url: str, tries: int = 3) -> WebResponse:
-		"""
-		Загружает HTML код страницы через Selenium.
-			url – адрес запроса;
-			tries – количество попыток повтора при неудачном выполнении.
-		Примечание:
-			Требуется инициализация библиотеки Selenium!
-		"""
-
-		# Ответ.
-		Response = WebResponse()
-		# Индекс попытки.
-		Try = 0
-		# Проверка наличия конфигурации.
-		self.__CheckConfig()
-		
-		# Пока не превышено количество попыток.
-		while Try < tries and Response.status_code != 200:
-			# Инкремент повтора.
-			Try += 1
-			
-			try:
-				# Выполнение запроса.
-				Response = self.__selenium_LOAD(url)
-				
-			except Exception as ExceptionData:
-				# Запись в лог ошибки: не удалось выполнить запрос.
-				if self.__Logging == True: logging.error("[SELENIUM-LOAD] Description: \"" + str(ExceptionData).split("\n")[0] + "\".")
-		
-		return Response
-	
-	#==========================================================================================#
-	# >>>>> ЗАПРОСЫ <<<<< #
-	#==========================================================================================#	
-	
-	def get(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, tries: int = 1) -> requests.Response | httpx.Response:
-		"""
-		Отправляет GET запрос.
-			url – адрес запроса;
-			params – словарь параметров запроса;
-			headers – словарь заголовков;
-			cookies – словарь куков;
-			tries – количество попыток повтора при неудачном выполнении.
-		"""
-
-		# Ответ.
-		Response = WebResponse()
-		# Индекс попытки.
-		Try = 0
-		# Проверка наличия конфигурации.
-		self.__CheckConfig()
-
-		# Название библиотеки.
-		LibName = None
-		
-		# Пока не превышено количество попыток.
-		while Try < tries and Response.status_code != 200:
-			# Инкремент повтора.
-			Try += 1
-			
-			try:
-				
-				# Если установлена конфигурация библиотеки requests.
-				if type(self.__Config) == RequestsConfig:
-					# Установка имени библиотеки.
-					LibName = "REQUESTS"
-					# Выполнение запроса.
-					Response = self.__requests_GET(url, params, headers, cookies)
-					
-				# Если установлена конфигурация библиотеки httpx.
-				if type(self.__Config) == HttpxConfig:
-					# Установка имени библиотеки.
-					LibName = "HTTPX"
-					# Выполнение запроса.
-					Response = self.__httpx_GET(url, params, headers, cookies)
-				
-			except Exception as ExceptionData:
-				# Запись в лог ошибки: не удалось выполнить запрос.
-				if self.__Logging == True: logging.error(f"[{LibName}-GET] Description: \"" + str(ExceptionData).split("\n")[0] + "\".")
-		
-		return Response
-	
-	def post(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None, tries: int = 1) -> requests.Response | httpx.Response:
-		"""
-		Отправляет POST запрос.
-			url – адрес запроса;
-			params – словарь параметров запроса;
-			headers – словарь заголовков;
-			cookies – словарь куков;
-			data – отправляемые данные;
-			json – сериализованное тело запроса;
-			tries – количество попыток повтора при неудачном выполнении.
-		"""
-
-		# Ответ.
-		Response = WebResponse()
-		# Индекс попытки.
-		Try = 0
-		# Проверка наличия конфигурации.
-		self.__CheckConfig()
-		# Название библиотеки.
-		LibName = None
-		
-		# Пока не превышено количество попыток.
-		while Try < tries and Response.status_code != 200:
-			# Инкремент повтора.
-			Try += 1
-			
-			try:
-				
-				# Если установлена конфигурация библиотеки requests.
-				if type(self.__Config) == RequestsConfig:
-					# Установка имени библиотеки.
-					LibName = "REQUESTS"
-					# Выполнение запроса.
-					Response = self.__requests_POST(url, params, headers, cookies, data, json)
-					
-				# Если установлена конфигурация библиотеки httpx.
-				if type(self.__Config) == HttpxConfig:
-					# Установка имени библиотеки.
-					LibName = "HTTPX"
-					# Выполнение запроса.
-					Response = self.__httpx_POST(url, params, headers, cookies, data, json)
-				
-			except Exception as ExceptionData:
-				# Запись в лог ошибки: не удалось выполнить запрос.
-				if self.__Logging == True: logging.error(f"[{LibName}-POST] Description: \"" + str(ExceptionData).split("\n")[0] + "\".")
-		
+from .Exceptions.WebRequestor import *
+
+from curl_cffi import requests as curl_cffi_requests
+from fake_useragent import UserAgent
+
+import importlib
+import requests
+import logging
+import random
+import httpx
+import enum
+
+#==========================================================================================#
+# >>>>> ДОПОЛНИТЕЛЬНЫЕ КОНФИГУРАЦИИ БИБЛИОТЕК ЗАПРОСОВ <<<<< #
+#==========================================================================================#
+
+class _curl_cffi_config:
+	"""Дополнительная конфигурация библиотеки curl_cffi."""
+
+	#==========================================================================================#
+	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
+	#==========================================================================================#
+
+	@property
+	def fingerprint(self) -> str | None:
+		"""Отпечаток браузера."""
+
+		return self.__Fingerprint
+
+	@property
+	def http2(self) -> bool:
+		"""Состояние использования протокола HTTP/2 для запросов."""
+
+		return self.__EnableHTTP2
+
+	#==========================================================================================#
+	# >>>>> МЕТОДЫ <<<<< #
+	#==========================================================================================#
+
+	def __init__(self):
+		"""Дополнительная конфигурация библиотеки curl_cffi."""
+
+		#---> Генерация динамических свойств.
+		#==========================================================================================#
+		# Состояние использования протокола HTTP/2 для запросов.
+		self.__EnableHTTP2 = False
+		# Используемый отпечаток.
+		self.__Fingerprint = None
+	
+	def enable_http2(self, status: bool):
+		"""
+		Переключает режим использования протокола HTTP/2 для запросов.
+			status – состояние режима.
+		"""
+
+		self.__EnableHTTP2 = status
+
+	def select_fingerprint(self, fingerprint: str | None):
+		"""Выбирает используемый отпечаток браузера."""
+
+		self.__Fingerprint = fingerprint
+
+class _httpx_config:
+	"""Дополнительная конфигурация библиотеки httpx."""
+
+	#==========================================================================================#
+	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
+	#==========================================================================================#
+
+	@property
+	def http2(self) -> bool:
+		"""Состояние использования протокола HTTP/2 для запросов."""
+
+		return self.__EnableHTTP2
+
+	#==========================================================================================#
+	# >>>>> МЕТОДЫ <<<<< #
+	#==========================================================================================#
+
+	def __init__(self):
+		"""Дополнительная конфигурация библиотеки curl_cffi."""
+
+		#---> Генерация динамических свойств.
+		#==========================================================================================#
+		# Состояние использования протокола HTTP/2 для запросов.
+		self.__EnableHTTP2 = False
+	
+	def enable_http2(self, status: bool):
+		"""
+		Переключает режим использования протокола HTTP/2 для запросов.
+			status – состояние режима.
+		"""
+
+		self.__EnableHTTP2 = status
+
+#==========================================================================================#
+# >>>>> ВСПОМОГАТЕЛЬНЫЕ ТИПЫ ДАННЫХ <<<<< #
+#==========================================================================================#
+
+class Protocols(enum.Enum):
+	"""Перечисление типов протоколов."""
+	
+	SOCKS = "socks"
+	HTTPS = "https"
+	HTTP = "http"
+	FTP = "ftp"
+
+class WebLibs(enum.Enum):
+	"""Перечисление поддерживаемых библиотек запросов."""
+
+	curl_cffi = "curl_cffi"
+	requests = "requests"
+	httpx = "httpx"
+		
+class WebResponse:
+	"""Эмуляция структуры ответа библиотеки requests."""
+
+	def __init__(self):
+		"""Эмуляция структуры ответа библиотеки requests."""
+
+		#---> Генерация динамических свойств.
+		#==========================================================================================#
+		# Статус ответа.
+		self.status_code = None
+		# Бинарное представление ответа.
+		self.content = None
+		# Текстовое представление ответа.
+		self.text = None
+		
+#==========================================================================================#
+# >>>>> ОСНОВНЫЕ КЛАССЫ <<<<< #
+#==========================================================================================#
+
+class WebConfig:
+	"""Конфигурация запросчика."""
+
+	#==========================================================================================#
+	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
+	#==========================================================================================#
+
+	@property
+	def headers(self) -> dict | None:
+		"""Словарь заголвоков, приоритетно применяемых ко всем запросам."""
+
+		# Возвращаемый словарь заголовков.
+		Headers = self.__Headers
+
+		# Если установлено значение User-Agent.
+		if self.__UserAgent:
+			# Если заголовки не определены, привести их к словарному типу.
+			if not Headers: Headers = dict()
+			# Добавление заголовка User-Agent.
+			Headers["User-Agent"] = self.__UserAgent
+
+		return Headers
+
+	@property
+	def lib(self) -> WebLibs:
+		"""Тип используемой библиотеки."""
+
+		return self.__UsedLib
+
+	@property
+	def logging(self) -> bool:
+		"""Статус ведения логов при помощи стандартного модуля."""
+
+		return self.__EnableLogging
+
+	@property
+	def redirecting(self) -> bool:
+		"""Состояние режима автоматического перенаправления запросов."""
+
+		return self.__EnableRedirecting
+
+	@property
+	def user_agent(self) -> str | None:
+		"""Значение User-Agent."""
+
+		return self.__UserAgent
+
+	#==========================================================================================#
+	# >>>>> МЕТОДЫ <<<<< #
+	#==========================================================================================#
+
+	def __init__(self):
+		"""Конфигурация запросчика."""
+
+		#---> Генерация публичных динамических свойств.
+		#==========================================================================================#
+		# Дополнительные конфигурации библиотек.
+		self.curl_cffi = _curl_cffi_config()
+		self.httpx = _httpx_config()
+
+		#---> Генерация приватных динамических свойств.
+		#==========================================================================================#
+		# Тип используемой библиотеки.
+		self.__UsedLib = WebLibs.requests
+		# Состояние режима автоматического перенаправления запросов.
+		self.__EnableRedirecting = True
+		# Статус ведения логов при помощи стандартного модуля.
+		self.__EnableLogging = True
+		# Значение заголовка UserAgent.
+		self.__UserAgent = None
+		# Словарь заголвоков, приоритетно применяемых ко всем запросам.
+		self.__Headers = None
+
+	def enable_logging(self, status: bool):
+		"""
+		Переключает ведение логов при помощи стандартного модуля.
+			status – состояние режима.
+		"""
+
+		self.__EnableLogging = status
+
+	def enable_redirecting(self, status: bool):
+		"""
+		Переключает режим автоматического перенаправления запросов.
+			status – состояние режима.
+		"""
+
+		self.__EnableRedirecting = status
+
+	def generate_user_agent(self, platform: str):
+		"""
+		Генерирует случайное значение User-Agent при помощи библиотеки fake_useragent.
+			platform – тип платформы.
+		"""
+
+		self.__UserAgent = UserAgent(platforms = platform).random
+
+	def remove_header(self, key: str):
+		"""
+		Удаляет заголовок, приоритетно применяемый ко всем запросам.
+			key – название заголовка.
+		"""
+
+		# Если задаётся заголовок User-Agent, выбросить исключение.
+		if key.lower() == "user-agent": raise UserAgentRedefining()
+		# Удаление заголовка.
+		del self.__Headers[key]
+
+	def select_lib(self, lib: WebLibs):
+		"""
+		Задаёт тип используемой библиотеки.
+			lib – тип библиотеки.
+		"""
+
+		self.__UsedLib = lib
+
+	def set_header(self, key: str, value: int | bool | dict | str):
+		"""
+		Добавляет заголовок, приоритетно применяемый ко всем запросам.
+			key – название заголовка;
+			value – значение заголовка.
+		"""
+
+		# Если задаётся заголовок User-Agent, выбросить исключение.
+		if key.lower() == "user-agent": raise UserAgentRedefining()
+		# Если заголовки не объявлены, привести их к словарному типу.
+		if self.__Headers == None: self.__Headers = dict()
+		# Добавление заголовка.
+		self.__Headers[key] = value
+
+	def set_user_agent(self, user_agent: str | None):
+		"""
+		Задаёт значение заголовка UserAgent.
+			user_agent – значение заголовка.
+		"""
+
+		self.__UserAgent = user_agent
+
+class WebRequestor:
+	"""Менеджер запросов."""
+	
+	#==========================================================================================#
+	# >>>>> ВСПОМОГАТЕЛЬНЫЕ МЕТОДЫ <<<<< #
+	#==========================================================================================#
+
+	def __Initialize(self):
+		"""Инициализирует сессию."""
+
+		# Если используется библиотека curl_cffi.	
+		if self.__Config.lib == WebLibs.curl_cffi:
+			# Инициализация сессии.
+			self.__Session = curl_cffi_requests.Session(allow_redirects = self.__Config.redirecting)
+
+		# Если используется библиотека httpx.	
+		if self.__Config.lib == WebLibs.httpx:
+			# Инициализация сессии.
+			self.__Session = httpx.Client(http2 = self.__Config.httpx.http2, proxies = self.__GetProxy())
+					
+		# Если используется библиотека requests.		
+		if self.__Config.lib == WebLibs.requests:
+			# Инициализация сессии.
+			self.__Session = requests.Session()
+		
+	def __GetProxy(self) -> dict | None:
+		"""Возвращает объект прокси для использования конкретной библиотекой."""
+		
+		# Объект прокси.
+		Proxy = None
+		
+		# Если задан хотя бы один прокси..
+		if len(self.__Proxies) > 0:
+			# Случайный выбор прокси.
+			Proxy = random.choice(self.__Proxies)
+			# Данные авторизации.
+			Auth = ""
+			# Если указаны логин и пароль, составить авторизационные данные.
+			if Proxy["login"] != None and Proxy["password"] != None: Auth = Proxy["login"] + ":" + Proxy["password"] + "@"
+					
+			# Если используется библиотека curl_cffi или requests.
+			if self.__Config.lib in [WebLibs.curl_cffi, WebLibs.requests]:
+				# Создание объекта прокси.
+				Proxy = {
+					Proxy["protocol"]: Proxy["protocol"].replace("https", "http") + "://" + Auth + Proxy["host"] + ":" + Proxy["port"]
+				}
+			
+			# Если используется библиотека httpx.	
+			if self.__Config.lib == WebLibs.httpx:
+				# Создание объекта прокси.
+				Proxy = {
+					Proxy["protocol"] + "://": Proxy["protocol"].replace("https", "http") + "://" + Auth + Proxy["host"] + ":" + Proxy["port"]
+				}
+			
+		return Proxy
+
+	def __MergeHeaders(self, headers: dict | None) -> dict | None:
+		"""Объединяет заголовки конфигурации и параметров запроса."""
+
+		# Если конфигурация содержит заголовки.
+		if self.__Config.headers:
+
+			# Если переданы заголовки.
+			if headers: 
+				# Объединение заголовков с приоритетом конфигурационным.
+				headers = self.__Config.headers | headers
+				
+			else:
+				# Установка словаря заголовков из конфигурации.
+				headers = self.__Config.headers
+
+		return headers
+
+	#==========================================================================================#
+	# >>>>> МЕТОДЫ ЗАПРОСОВ БИБЛИОТЕКИ CURL_CFFI <<<<< #
+	#==========================================================================================#
+
+	def __curl_cffi_GET(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None) -> curl_cffi_requests.Response:
+		"""
+		Отправляет GET запрос через библиотеку curl_cffi.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков.
+		"""
+
+		# Обработка заголовков.
+		headers = self.__MergeHeaders(headers)
+		# Выполнение запроса.
+		Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy())
+
+		return Response
+
+	def __curl_cffi_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> curl_cffi_requests.Response:
+		"""
+		Отправляет POST запрос через библиотеку curl_cffi.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков;
+			data – данные запроса;
+			json – сериализованное тело запроса.
+		"""
+		
+		# Обработка заголовков.
+		headers = self.__MergeHeaders(headers)
+		# Выполнение запроса.
+		Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy())
+		
+		return Response
+	
+	#==========================================================================================#
+	# >>>>> МЕТОДЫ ЗАПРОСОВ БИБЛИОТЕКИ HTTPX <<<<< #
+	#==========================================================================================#
+
+	def __httpx_GET(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None) -> httpx.Response:
+		"""
+		Отправляет GET запрос через библиотеку httpx.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков.
+		"""
+
+		# Обработка заголовков.
+		headers = self.__MergeHeaders(headers)
+		# Выполнение запроса.
+		Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, follow_redirects = self.__Config.redirecting)
+
+		return Response
+
+	def __httpx_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> httpx.Response:
+		"""
+		Отправляет POST запрос через библиотеку httpx.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков;
+			data – данные запроса;
+			json – сериализованное тело запроса.
+		"""
+		
+		# Обработка заголовков.
+		headers = self.__MergeHeaders(headers)
+		# Выполнение запроса.
+		Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, follow_redirects = self.__Config.redirecting)
+		
+		return Response
+	
+	#==========================================================================================#
+	# >>>>> МЕТОДЫ ЗАПРОСОВ БИБЛИОТЕКИ REQUESTS <<<<< #
+	#==========================================================================================#
+
+	def __requests_GET(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None) -> requests.Response:
+		"""
+		Отправляет GET запрос через библиотеку requests.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков.
+		"""
+		
+		# Обработка заголовков.
+		headers = self.__MergeHeaders(headers)
+		# Эмуляция ответа.
+		Response = WebResponse()
+		
+		try:
+			# Выполнение запроса.
+			Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting)
+
+		except requests.exceptions.ProxyError as ExceptionData:
+			# Установка значений ответа.
+			Response.status_code = 407
+			Response.text = str(ExceptionData)
+			Response.content = bytes(ExceptionData)
+
+		return Response
+	
+	def __requests_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> requests.Response:
+		"""
+		Отправляет POST запрос через библиотеку requests.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков;
+			data – данные запроса;
+			json – сериализованное тело запроса.
+		"""
+		
+		# Обработка заголовков.
+		headers = self.__MergeHeaders(headers)
+		# Эмуляция ответа.
+		Response = WebResponse()
+
+		try:
+			# Выполнение запроса.
+			Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting)
+		
+		except requests.exceptions.ProxyError as ExceptionData:
+			# Установка значений ответа.
+			Response.status_code = 407
+			Response.text = str(ExceptionData)
+			Response.content = bytes(ExceptionData)
+
+		return Response
+		
+	#==========================================================================================#
+	# >>>>> ОБЩИЕ МЕТОДЫ <<<<< #
+	#==========================================================================================#
+		
+	def __init__(self, config: WebConfig):
+		"""
+		Менеджер запросов.
+			config – конфигурация библиотеки запросов.
+		"""
+
+		#---> Генерация динамических свойств.
+		#==========================================================================================#
+		# Список прокси.
+		self.__Proxies = list()
+		# Конфигурация.
+		self.__Config = config
+		# Сессия запросов.
+		self.__Session = None
+
+		# Инициализация сессии.
+		self.__Initialize()
+
+	def close(self):
+		"""Закрывает менеджер запросов."""
+			
+		# Закрытие и обнуление сессии.
+		self.__Session.close()
+		self.__Session = None
+			
+	def add_proxy(self, protocol: Protocols, host: str, port: int | str, login: str | None = None, password: str | None = None):
+		"""
+		Добавляет прокси для использования в запросах. Не работает с Selenium.
+			protocol – протокол прокси-соединения;
+			host – IP или адрес хоста;
+			port – порт сервера;
+			login – логин для авторизации;
+			password – пароль для авторизации.
+		"""
+		
+		# Добавление прокси в список.
+		self.__Proxies.append({
+			"protocol": protocol.value,
+			"host": host,
+			"port": str(port),
+			"login": login,
+			"password": password
+		})
+		# Если используется библиотека httpx, реинициализировать сессию.
+		if self.__Config.lib == WebLibs.httpx: self.__Initialize()
+	
+	#==========================================================================================#
+	# >>>>> ЗАПРОСЫ <<<<< #
+	#==========================================================================================#	
+	
+	def get(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, tries: int = 1) -> requests.Response | httpx.Response:
+		"""
+		Отправляет GET запрос.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков;
+			tries – количество попыток повтора при неудачном выполнении.
+		"""
+
+		# Ответ.
+		Response = WebResponse()
+		# Индекс попытки.
+		Try = 0
+		# Название библиотеки.
+		LibName = None
+		
+		# Пока не превышено количество попыток.
+		while Try < tries and Response.status_code != 200:
+			# Инкремент повтора.
+			Try += 1
+			
+			try:
+
+				# Если используется библиотека curl_cffi.
+				if self.__Config.lib == WebLibs.curl_cffi:
+					# Установка имени библиотеки.
+					LibName = "CURL_CFFI"
+					# Выполнение запроса.
+					Response = self.__curl_cffi_GET(url, params, headers, cookies)
+
+				# Если используется библиотека httpx.
+				if self.__Config.lib == WebLibs.httpx:
+					# Установка имени библиотеки.
+					LibName = "HTTPX"
+					# Выполнение запроса.
+					Response = self.__httpx_GET(url, params, headers, cookies)
+				
+				# Если используется библиотека requests.
+				if self.__Config.lib == WebLibs.requests:
+					# Установка имени библиотеки.
+					LibName = "REQUESTS"
+					# Выполнение запроса.
+					Response = self.__requests_GET(url, params, headers, cookies)
+
+			except Exception as ExceptionData:
+				# Запись в лог ошибки: не удалось выполнить запрос.
+				if self.__Config.logging: logging.error(f"[{LibName}-GET] Description: \"" + str(ExceptionData) + "\".")
+		
+		return Response
+	
+	def post(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None, tries: int = 1) -> requests.Response | httpx.Response:
+		"""
+		Отправляет POST запрос.
+			url – адрес запроса;
+			params – словарь параметров запроса;
+			headers – словарь заголовков;
+			cookies – словарь куков;
+			data – отправляемые данные;
+			json – сериализованное тело запроса;
+			tries – количество попыток повтора при неудачном выполнении.
+		"""
+
+		# Ответ.
+		Response = WebResponse()
+		# Индекс попытки.
+		Try = 0
+		# Название библиотеки.
+		LibName = None
+		
+		# Пока не превышено количество попыток.
+		while Try < tries and Response.status_code != 200:
+			# Инкремент повтора.
+			Try += 1
+			
+			try:
+				
+				# Если используется библиотека curl_cffi.
+				if self.__Config.lib == WebLibs.curl_cffi:
+					# Установка имени библиотеки.
+					LibName = "CURL_CFFI"
+					# Выполнение запроса.
+					Response = self.__curl_cffi_POST(url, params, headers, cookies, data, json)
+
+				# Если используется библиотека httpx.
+				if self.__Config.lib == WebLibs.httpx:
+					# Установка имени библиотеки.
+					LibName = "HTTPX"
+					# Выполнение запроса.
+					Response = self.__httpx_POST(url, params, headers, cookies, data, json)
+				
+				# Если используется библиотека requests.
+				if self.__Config.lib == WebLibs.requests:
+					# Установка имени библиотеки.
+					LibName = "REQUESTS"
+					# Выполнение запроса.
+					Response = self.__requests_POST(url, params, headers, cookies, data, json)
+				
+			except Exception as ExceptionData:
+				# Запись в лог ошибки: не удалось выполнить запрос.
+				if self.__Config.logging: logging.error(f"[{LibName}-POST] Description: \"" + str(ExceptionData) + "\".")
+		
 		return Response
```

### Comparing `dublib-0.3.1/src/dublib.egg-info/PKG-INFO` & `dublib-0.4.0/src/dublib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.3.1
+Version: 0.4.0
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -39,29 +39,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: curl_cffi>=0.6.0
 Requires-Dist: fake_useragent
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
 Requires-Dist: requests
 
 # dublib
 **dublib** – это библиотека, поставляющая компоненты, требующиеся в проектах [@DUB1401](https://github.com/DUB1401), написанных на Python.
 
 # Поставляемые компоненты
 Библиотека включает следующие модули:
-* [Methods](docs/Methods.md)
-* [Polyglot](docs/Polyglot.md)
-* [StyledPrinter](docs/StyledPrinter.md)
-* [Terminalyzer](docs/Terminalyzer.md)
-* [WebRequestor](docs/WebRequestor.md)
+* [Methods](https://github.com/DUB1401/dublib/blob/main/docs/Methods.md)
+* [Polyglot](https://github.com/DUB1401/dublib/blob/main/docs/Polyglot.md)
+* [StyledPrinter](https://github.com/DUB1401/dublib/blob/main/docs/StyledPrinter.md)
+* [Terminalyzer](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
+* [WebRequestor](https://github.com/DUB1401/dublib/blob/main/docs/WebRequestor.md)
 
 # Установка
 Библиотека поддерживает установку из двух типов репозиториев:
 * **PyPI** – стабильные выпуски (с возможностью выбора конкретной версии);
 * **GitHub** – канал разработки со всеми последними изменениями и исправлениями.
 
 _**Примечание:**_ Для установки библиотеки из репозитория GitHub на вашем устройстве должна присутствовать система контроля версий Git.
```

