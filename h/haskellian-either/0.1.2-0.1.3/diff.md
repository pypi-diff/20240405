# Comparing `tmp/haskellian-either-0.1.2.tar.gz` & `tmp/haskellian-either-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-either-0.1.2.tar", last modified: Thu Apr  4 16:14:25 2024, max compression
+gzip compressed data, was "haskellian-either-0.1.3.tar", last modified: Fri Apr  5 06:25:30 2024, max compression
```

## Comparing `haskellian-either-0.1.2.tar` & `haskellian-either-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      492 2024-04-04 16:14:20.000000 haskellian-either-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.583188 haskellian-either-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.583188 haskellian-either-0.1.2/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-04 11:11:34.000000 haskellian-either-0.1.2/src/haskellian/either/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2190 2024-04-04 11:13:26.000000 haskellian-either-0.1.2/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2257 2024-04-03 05:57:59.000000 haskellian-either-0.1.2/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      492 2024-04-05 06:25:24.000000 haskellian-either-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      170 2024-04-05 06:18:29.000000 haskellian-either-0.1.3/src/haskellian/either/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1068 2024-04-05 06:18:26.000000 haskellian-either-0.1.3/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2121 2024-04-05 06:25:01.000000 haskellian-either-0.1.3/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 06:25:30.130847 haskellian-either-0.1.3/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-05 06:25:30.000000 haskellian-either-0.1.3/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-04-05 06:25:30.000000 haskellian-either-0.1.3/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 06:25:30.000000 haskellian-either-0.1.3/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-05 06:25:30.000000 haskellian-either-0.1.3/src/haskellian_either.egg-info/top_level.txt
```

### Comparing `haskellian-either-0.1.2/src/haskellian/either/type.py` & `haskellian-either-0.1.3/src/haskellian/either/type.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 A = TypeVar('A')
 L = TypeVar('L', covariant=True)
 R = TypeVar('R', covariant=True)
 L2 = TypeVar('L2')
 R2 = TypeVar('R2')
 
+@dataclass(eq=False)
+class IsLeft(BaseException, Generic[L]):
+  value: L
+
 @dataclass
 class Either(ABC, Generic[L, R]):
   value: L | R
   tag: Literal['left', 'right']
 
   def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
     """Unwrap an `Either` by matching both branches"""
@@ -32,47 +36,40 @@
         on_left(err)
       case Right(value):
         on_right(value)
     return self
   
   def mapl(self, f: Callable[[L], L2]) -> 'Either[L2, R]':
     """Map the left branch"""
-    return self.match(lambda x: Left(f(x)), Right)
+    return self.match(lambda x: Left(f(x)), lambda x: Right(x))
   
   def fmap(self, f: Callable[[R], R2]) -> 'Either[L, R2]':
-    return self.match(Left, lambda x: Right(f(x)))
+    return self.match(lambda x: Left(x), lambda x: Right(f(x)))
   
   __or__ = fmap
   """Alias of `fmap`"""
       
   def bind(self, f: 'Callable[[R], Either[L2, R2]]') -> 'Either[L|L2, R2]':
-    return self.match(Left, f)
+    return self.match(lambda x: Left(x), f)
   
   __and__ = bind
   """Alias of `bind`"""
 
   def unsafe(self) -> R:
-    """Unwraps the value or throws the left exception"""
+    """Unwraps the value or throws an `IsLeft` exception
+    
+    (`IsLeft.value` will contain the wrapped value)"""
     match self:
       case Left(err):
-        exc = err if isinstance(err, BaseException) else Exception(err)
-        raise exc
-      case Right(value):
-        return value
-  
-  def expect(self, exc: Callable[[], BaseException]) -> R:
-    """Unwraps the value or throws the exception"""
-    match self:
-      case Left():
-        raise exc()
+        raise IsLeft(err)
       case Right(value):
         return value
 
 @dataclass
-class Left(Either[L, R], Generic[L, R]):
+class Left(Either[L, R]):
   value: L = None
   tag: Literal['left'] = 'left'
 
 @dataclass
-class Right(Either[L, R], Generic[L, R]):
+class Right(Either[L, R]):
   value: R = None
   tag: Literal['right'] = 'right'
```

