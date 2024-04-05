# Comparing `tmp/astr-0.0.6.tar.gz` & `tmp/astr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astr-0.0.6.tar", last modified: Wed Apr  3 12:01:19 2024, max compression
+gzip compressed data, was "astr-0.0.7.tar", last modified: Fri Apr  5 14:15:17 2024, max compression
```

## Comparing `astr-0.0.6.tar` & `astr-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 12:01:19.916152 astr-0.0.6/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-01-13 21:01:11.000000 astr-0.0.6/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-01-13 21:01:11.000000 astr-0.0.6/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-03 12:01:19.916017 astr-0.0.6/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1635 2024-01-13 21:09:28.000000 astr-0.0.6/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 12:01:19.914882 astr-0.0.6/astr/
--rw-r--r--   0 solst      (501) staff       (20)      322 2024-04-03 12:01:14.000000 astr-0.0.6/astr/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     4038 2024-04-03 12:01:14.000000 astr-0.0.6/astr/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      421 2024-04-03 12:01:14.000000 astr-0.0.6/astr/_tmp.py
--rw-r--r--   0 solst      (501) staff       (20)    20996 2024-04-03 12:01:14.000000 astr-0.0.6/astr/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 12:01:19.915841 astr-0.0.6/astr.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      307 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-26 19:39:48.000000 astr-0.0.6/astr.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      878 2024-03-09 19:12:22.000000 astr-0.0.6/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-03 12:01:19.916201 astr-0.0.6/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2024-01-13 21:01:11.000000 astr-0.0.6/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:15:17.748628 astr-0.0.7/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-01-13 21:01:11.000000 astr-0.0.7/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-01-13 21:01:11.000000 astr-0.0.7/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-05 14:15:17.748499 astr-0.0.7/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1635 2024-01-13 21:09:28.000000 astr-0.0.7/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:15:17.747274 astr-0.0.7/astr/
+-rw-r--r--   0 solst      (501) staff       (20)      322 2024-04-05 14:15:15.000000 astr-0.0.7/astr/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     5994 2024-04-05 14:15:15.000000 astr-0.0.7/astr/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      421 2024-04-05 14:15:15.000000 astr-0.0.7/astr/_tmp.py
+-rw-r--r--   0 solst      (501) staff       (20)    27824 2024-04-05 14:15:15.000000 astr-0.0.7/astr/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-05 14:15:17.748322 astr-0.0.7/astr.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-05 14:15:17.000000 astr-0.0.7/astr.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      307 2024-04-05 14:15:17.000000 astr-0.0.7/astr.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-05 14:15:17.000000 astr-0.0.7/astr.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-05 14:15:17.000000 astr-0.0.7/astr.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-26 19:39:48.000000 astr-0.0.7/astr.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-05 14:15:17.000000 astr-0.0.7/astr.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-05 14:15:17.000000 astr-0.0.7/astr.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      878 2024-04-03 12:02:28.000000 astr-0.0.7/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-05 14:15:17.748672 astr-0.0.7/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2024-01-13 21:01:11.000000 astr-0.0.7/setup.py
```

### Comparing `astr-0.0.6/LICENSE` & `astr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `astr-0.0.6/PKG-INFO` & `astr-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astr
-Version: 0.0.6
+Version: 0.0.7
 Summary: astr (attribute string) for defined getter / setter methods
 Home-page: https://github.com/dsm-72/astr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: attr str attribute string astr attrstr python alias type astr typ get set instance ins insattr getter setter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `astr-0.0.6/README.md` & `astr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `astr-0.0.6/astr/core.py` & `astr-0.0.7/astr/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['DOT', 'NIL', 'GET', 'ATTR', 'BASES', 'CHECK', 'GUARD', 'RETHAS', 'RETSELF', 'DEFAULT', 'CHECKOBJ', 'GUARDOBJ',
-           'NAMESPACE', 'CLASSVARS', 'ASSIGNED', 'T', 'O', 'P', 'GuardLike', 'iscall', 'isnone', 'notnone', 'isiter',
-           'isstr', 'allstrs', 'istuple', 'insattr', 'astrmeta', 'astr', 'attr', 'attrstr']
+__all__ = ['DOT', 'NIL', 'GET', 'HAS', 'RET', 'ATTR', 'SELF', 'ITEM', 'BASES', 'CHECK', 'GUARD', 'RETHAS', 'RETSELF', 'OPTION',
+           'DEFAULT', 'CHECKOBJ', 'GUARDOBJ', 'CHECK_ATTR', 'ATTR_GUARD', 'CHECK_ITEM', 'ITEM_GUARD', 'RET_OPTION',
+           'RETURN_FNC', 'ATTR_MODE', 'NAMESPACE', 'CLASSVARS', 'ASSIGNED', 'T', 'O', 'P', 'GuardLike',
+           'ReturnFunction', 'AttributeMode', 'ReturnOption', 'iscall', 'isnone', 'notnone', 'isiter', 'isstr',
+           'allstrs', 'istuple', 'make_return_fnc', 'insattr', 'inspect_attribute', 'inspect_attr', 'ins_attr',
+           'get_or_has', 'astrmeta', 'astr', 'attr', 'attrstr', 'attribute_meta', 'attribute']
 
 # %% ../nbs/00_core.ipynb 6
 from abc import abstractmethod
 from functools import wraps
+from enum import StrEnum, auto
 
 # %% ../nbs/00_core.ipynb 8
 from typing import (
     Any, Self, Type, Union, TypeVar, ParamSpec, 
     TypeAlias, TypeGuard, ClassVar, Callable, Optional, Iterable,
 )
 
@@ -28,51 +32,111 @@
 
 
 # %% ../nbs/00_core.ipynb 16
 DOT = '.'
 NIL = ''
 
 GET = 'get'
+HAS = 'has'
+RET = 'ret'
+
 ATTR = 'attr' 
+SELF = 'self'
+ITEM = 'item'
 
 BASES = 'bases' 
+
 CHECK = 'check'
 GUARD = 'guard'
 
-RETHAS = 'rethas' 
-RETSELF = 'retself'
+RETHAS = f'{RET}{HAS}' 
+RETSELF = f'{RET}{SELF}'
 
+OPTION = 'option'
 DEFAULT = 'default'
 
 CHECKOBJ = 'checkobj'
 GUARDOBJ = 'guardobj'
 
+CHECK_ATTR = f'{CHECK}_{ATTR}'
+ATTR_GUARD = f'{ATTR}_{GUARD}'
+CHECK_ITEM = f'{CHECK}_{ITEM}'
+ITEM_GUARD = f'{ITEM}_{GUARD}'
+RET_OPTION = f'{RET}_{OPTION}'
+RETURN_FNC = 'return_fnc'
+
+
+ATTR_MODE = f'{ATTR}_mode'
+
 NAMESPACE = 'namespace'
 
 __DOC__ = '__doc__' 
 __NAME__ = '__name__'
 __MODULE__ = '__module__'
 __QUALNAME__ = '__qualname__'
 __ANNOTATIONS__ = '__annotations__'
 
-
-CLASSVARS = (ATTR, CHECK, GUARD, CHECKOBJ, GUARDOBJ, RETSELF, DEFAULT)
+# CLASSVARS = (ATTR, CHECK, GUARD, CHECKOBJ, GUARDOBJ, RETSELF, DEFAULT)
+CLASSVARS = (ATTR, CHECK_ATTR, ATTR_GUARD, CHECK_ITEM, ITEM_GUARD, RET_OPTION, RETURN_FNC, ATTR_MODE, DEFAULT)
 ASSIGNED = (__MODULE__, __DOC__, __ANNOTATIONS__)
 
 # %% ../nbs/00_core.ipynb 18
+class AttributeMode(StrEnum):
+    GET = auto()
+    HAS = auto()
+    
+class ReturnOption(StrEnum):
+    '''What to return from the item when inspecting its attribute.
+    
+    Attributes
+    ----------
+    val : 'val'
+        inspect attribute will return the default value.
+    
+    bool : 'bool'
+        inspect attribute will return the boolean of `hasattr`.
+        
+    call : 'call'
+        inspect attribute will return the identity function `(*args, **kwds) --> item`
+        which returns the item it was called on.
+    
+    self : 'self'
+        inspect attribute will return the item it was called with.
+        
+    item : 'self'
+        Alias for self.
+        
+    has : 'bool'
+        Alias for bool.
+    
+    default : 'val'
+        Alias for val.
+    '''
+    val = auto()
+    bool = auto()
+    call = auto()
+    self = auto()
+    has = bool
+    item = self
+    default = val
+
+# %% ../nbs/00_core.ipynb 20
 T = TypeVar('T')
 
 O = TypeVar('O')
 
 P = ParamSpec('P')
 
 GuardLike: TypeAlias = Callable[[O], TypeGuard[T]]
 '''TypeAlias for a callable that takes an object of type O and returns a TypeGuard for type T.''';
 
-# %% ../nbs/00_core.ipynb 20
+ReturnFunction: TypeAlias = Callable[[tuple[object, str, Any]], Any]
+'''The constructor function `(item, attr, default) -> Any` for making the function returned from inspect attribute.''';
+
+# %% ../nbs/00_core.ipynb 22
 def iscall(x) -> TypeGuard[Callable]:
     '''Check if `x` is `Callable`.'''
     return isinstance(x, Callable)
 
 def isnone(x) -> TypeGuard[None]:
     '''Check if `x` is `None`.'''
     return x is None
@@ -81,167 +145,203 @@
     '''Check if `x` is not `None`.'''
     return not isnone(x)
 
 def isiter(x) -> TypeGuard[Iterable]:
     '''Check if `x` is `Iterable`.'''
     return isinstance(x, Iterable)
 
-
 def isstr(x) -> TypeGuard[str]:
     '''Check if `x` is `str`.'''
     return isinstance(x, str)
 
 def allstrs(x) -> TypeGuard[tuple[str, ...]]:
     '''Check if `x` is an iterable of `str`s.'''
     return isinstance(x, Iterable) and all(isstr(a) for a in x)
 
 def istuple(x) -> TypeGuard[tuple]:
     '''Check if `x` is a `tuple`'''
     return isinstance(x, tuple)
 
-# %% ../nbs/00_core.ipynb 22
+# %% ../nbs/00_core.ipynb 24
+def make_return_fnc(item: object, attr: str, default: Any = None) -> Callable[P, object]:
+    def identity(*args: P.args, **kwargs: P.kwargs):
+        return item
+    return identity
+
+# %% ../nbs/00_core.ipynb 25
 def insattr(
-    obj:      object, 
-    attr:     str, 
-    default:  Any = None,
-    check:    bool = True,
-    guard:    Optional[GuardLike] = notnone,
-    checkobj: Optional[GuardLike] = None, 
-    guardobj: Optional[GuardLike] = notnone, 
-    rethas:   bool = False,
-    retself:  bool = False,
-    __value:  Any = None,
+    item: object, 
+    attr: str, 
+    default: Any = None,
+    
+    check_attr: bool = True,
+    attr_guard: Optional[GuardLike] = notnone,
+    check_item: Optional[bool] = None, 
+    item_guard: Optional[GuardLike] = notnone, 
+    
+    ret_option: ReturnOption = ReturnOption.default,
+    return_fnc: Optional[ReturnFunction] = make_return_fnc,
+    **kwargs: P.kwargs
 ) -> Union[Any, bool, object]:
-    '''Get an attribute from an object and check its type.
+    '''Get an attribute from an object and check_attr its type.
     
     Parameters
     ----------
-    obj : object
+    item : object
         The object to get the attribute from.
         
     attr : str
         The name of the attribute to get.
         
     default : Any, optional
         The default value to return if the attribute is not found, by default None.
         
-    check : bool, default: True
+    check_attr : bool, default: True
         Whether to check the type of the attribute, by default True.
         
-    guard : Optional[GuardLike], default: `notnone`
-        The guard to check the type of the retrieved attribute, by default `notnone`.
+    attr_guard : Optional[GuardLike], default: `notnone`
+        The type guard to check the type of the retrieved attribute, by default `notnone`.
         
-    checkobj : Optional[GuardLike], default: None
-        The guard to check the type of the object, by default None.
+    check_item : Optional[bool], default: False
+        Whether to check the object, by default None.
         
-    guardobj : Optional[GuardLike], default: `notnone`
-        The guard to check the type of the object, by default `notnone`.
+    item_guard : Optional[GuardLike], default: `notnone`
+        The type guard to check the type of the object, by default `notnone`.
+        
+    ret_option : bool, default: ReturnOption.default
+        Specifies what to return: the value of the attribute from `item`, a boolean indicating 
+        the attribute's existence, or the input `item` itself.
+        
+    return_fnc : Optional[ReturnFunction], optional
+        A function that defines the return behavior when ret_option is set to ReturnOption.call, by default make_return_fnc.
         
-    rethas : bool, default: False
-        Whether to return the boolean result of the typeguard or the attribute, 
-        by default False.
-        
-    retself : bool, default: False
-        Whether to return the object if the attribute fails the guard, otherwise
-        the default value is returned, by default False.
     '''
-    # Step 1: Check if the object is of the correct type
-    if (checkobj and iscall(guardobj)) and not guardobj(obj): 
+    check_attr = kwargs.get('check_attr', kwargs.get('checkret', check_attr))
+    attr_guard = kwargs.get('attr_guard', kwargs.get('guardret', attr_guard))
+    
+    check_item = kwargs.get('checkobj', check_item)
+    item_guard = kwargs.get('guardobj', item_guard)
+    
+    # Step 1: Check if the item is of the correct type
+    if (check_item and iscall(item_guard)) and not item_guard(item): 
         return default
     
     # Step 2: Try and get the attribute
-    try: has = hasattr(obj, attr)
+    try: has = hasattr(item, attr)
     except: has = False
     
     if not isstr(attr):
         try: attr = getattr(attr, ATTR, attr)
         except: ...
         
-    try: val = getattr(obj, attr, default)
+    try: val = getattr(item, attr, default)
     except: val = default
     
     if isnone(val): 
         val = default
     
-    if __value is not None: 
-        val = __value
-    
-    if val is None and __value is None:
-        try: val = getattr(obj, ATTR, val)
-        except: ...
-        
+    return_has = (ret_option == ReturnOption.has)
     # Step 3: Check if the attribute is of the correct type
-    passed = (has and check and iscall(guard)) and guard(val)
+    passed = (has and check_attr and iscall(attr_guard)) and attr_guard(val)
     if passed: 
-        return has if rethas else val
+        return has if return_has else val
     
-    # Step 4: value failed the guard, check if the boolean
+    # Step 4: value failed the attr_guard, check_attr if the boolean
     # i.e. typeguard result should be returned
-    if rethas: 
+    if return_has:
         return has
     
-    # Step 5: value failed the guard, check if the object 
+    # Step 5: value failed the attr_guard, check_attr if the object 
     # should be returned
-    passed = (check and iscall(guard)) and guardobj(obj)
-    if (retself and passed): 
-        return obj
+    return_self = (ret_option == ReturnOption.self)
+    passed = (check_item and iscall(item_guard)) and item_guard(item)
+    if (return_self and (not check_item or passed)):
+        return item
+    
+    return_call = (ret_option == ReturnOption.call)
+    if return_call:
+        return return_fnc(item, attr, default)
     
     return default
 
-# %% ../nbs/00_core.ipynb 24
+# %% ../nbs/00_core.ipynb 26
+@wraps(insattr, assigned=ASSIGNED)
+def inspect_attribute(*args: P.args, **kwargs: P.kwargs):
+    '''Alias for `insattr`.'''
+    return insattr(*args, **kwargs)
+
+@wraps(insattr, assigned=ASSIGNED)
+def inspect_attr(*args: P.args, **kwargs: P.kwargs):
+    '''Alias for `insattr`.'''
+    return insattr(*args, **kwargs)
+
+@wraps(insattr, assigned=ASSIGNED)
+def ins_attr(*args: P.args, **kwargs: P.kwargs):
+    '''Alias for `insattr`.'''
+    return insattr(*args, **kwargs)
+
+@wraps(insattr, assigned=ASSIGNED)
+def get_or_has(*args: P.args, **kwargs: P.kwargs):
+    '''Alias for `insattr`.'''
+    return insattr(*args, **kwargs)
+
+# %% ../nbs/00_core.ipynb 28
 class astrmeta(type):
     '''A metaclass for attributes to extend instance checks and equality.
     
     A metaclass for dynamically generating and handling attributes with enhanced instance checks, equality, and attribute manipulation.
     This metaclass allows for the creation of attribute-centric classes (`astr` instances) that encapsulate logic for accessing, setting, 
     and checking the presence of specified attributes on objects. It supports creating attribute-specific classes directly or 
     through decoration, enabling flexible and powerful attribute manipulation and introspection.
     
     Attributes
     ----------
     attr : str
-        The name of the attribute to get, set, or check on an object.
+        The name of the attribute to get, set, or check_attr on an object.
         
-    check : bool
-        Indicates whether to check the type of the attribute upon retrieval.
+    check_attr : bool
+        Indicates whether to check_attr the type of the attribute upon retrieval.
         
-    guard : GuardLike, optional
-        A callable used as a type guard for the retrieved attribute.
+    attr_guard : GuardLike, optional
+        A callable used as a type attr_guard for the retrieved attribute.
         
-    checkobj : bool, optional
-        Indicates whether to check the type of the object before attribute manipulation.
+    check_item : bool, optional
+        Indicates whether to check_attr the type of the object before attribute manipulation.
         
-    guardobj : GuardLike, optional
-        A callable used as a type guard for the object before attribute manipulation.
+    item_guard : GuardLike, optional
+        A callable used as a type attr_guard for the object before attribute manipulation.
         
-    retself : bool
-        Determines whether to return the original object if the attribute fails the type guard check.
+    ret_option : bool
+        Determines whether to return the original object if the attribute fails the type attr_guard check_attr.
         
     default : Any
-        The default value to return if the attribute is not found or fails the type guard check.
+        The default value to return if the attribute is not found or fails the type attr_guard check_attr.
     '''
     
-    
     attr: ClassVar[str]
-    '''The name of the attribute to get / set / or check if an object has.'''
+    '''The name of the attribute to get / set / or check_attr if an object has.'''
     
-    check: ClassVar[bool] = True
+    check_attr: ClassVar[bool] = True
     '''Whether to check the type of the attribute, by default True.'''
     
-    guard: ClassVar[Optional[GuardLike]] = notnone
-    '''The guard to check the type of the retrieved attribute, by default `notnone`.'''
+    attr_guard: ClassVar[Optional[GuardLike]] = notnone
+    '''The type guard to check the type of the retrieved attribute, by default `notnone`.'''
     
-    checkobj: ClassVar[Optional[bool]] = True
-    '''The guard to check the type of the object, by default None.'''
+    check_item: ClassVar[Optional[bool]] = True
+    '''Whether to check the type of the object, by default None.'''
     
-    guardobj: ClassVar[Optional[GuardLike]] = notnone
-    '''The guard to check the type of the object, by default `notnone`.'''
+    item_guard: ClassVar[Optional[GuardLike]] = notnone
+    '''The type guard to check the type of the object, by default `notnone`.'''
     
-    retself: ClassVar[bool] = True
-    '''Whether to return the object if the attribute fails the guard, otherwise the default value is returned, by default False.'''
+    ret_option: ClassVar[ReturnOption] = ReturnOption.self
+    '''Whether to return the object if the attribute fails the attr_guard, otherwise the default value is returned, by default False.'''
+    
+    return_fnc: ClassVar[ReturnFunction] = make_return_fnc
+    
+    attr_mode: ClassVar[AttributeMode] = AttributeMode.GET
     
     default: ClassVar[Any] = None
     '''The default value to return if the attribute is not found, by default None.'''
     
     clsvars: tuple[str, ...] = CLASSVARS
     '''The tuple of class variable names.'''
     
@@ -280,15 +380,15 @@
         ... # create two classes that have a foo attribute
         ... class testa: 
         ...    foo = 1; bar = 2; hi = 'no'; qux = dict(a=2);
         ... 
         ... class testb: 
         ...    foo = None; bar = -10; hello = 'yes'; qux = dict(a=5);
         ... 
-        ... # test equality and instance check works via astrmeta __eq__ and __instancecheck__ methods
+        ... # test equality and instance check_attr works via astrmeta __eq__ and __instancecheck__ methods
         ... foo == testa, foo == testb, isinstance(testa, foo), isinstance(testb, foo)
         (True, True, True, True)
         '''
         try: sub = issubclass(__instance, cls)
         except: sub = False
         return cls.__guard__(__instance) or sub
     
@@ -304,15 +404,15 @@
         ... # create two classes that have a foo attribute
         ... class testa: 
         ...    foo = 1; bar = 2; hi = 'no'; qux = dict(a=2);
         ... 
         ... class testb: 
         ...    foo = None; bar = -10; hello = 'yes'; qux = dict(a=5);
         ... 
-        ... # test equality and instance check works via attrmeta __eq__ and __instancecheck__ methods
+        ... # test equality and instance check_attr works via attrmeta __eq__ and __instancecheck__ methods
         ... foo == testa, foo == testb, isinstance(testa, foo), isinstance(testb, foo)
         (True, True, True, True)
         '''
         if isinstance(ins, cls): 
             return True
         return super().__eq__(ins)
     
@@ -343,16 +443,14 @@
         '''Make a new attribute class with the given attribute name.'''
         # class name, bases and dct
         kwargs.setdefault(ATTR, attr or name)
         bases = kwargs.pop(BASES, (cls, ))
         ndict = kwargs.pop(NAMESPACE, {})
         ndict.update(__annotations__ = cls.__annotations__, __module__ = cls.__module__, attr = attr)
         return cls.__class__(name, bases, ndict, *args, **kwargs)
-        new.setvars(**kwargs)
-        return new
     
     def __make_astrs__(cls, attrs: tuple[str, ...] = tuple(), *args: P.args, **kwargs: P.kwargs):
         attrs = attrs or (getattr(cls, __NAME__, None), )
         return tuple(cls.__make_astr__(
             getattr(cls, __NAME__, attr), *args, **kwargs, 
             attr=attr) for attr in attrs
         )
@@ -382,104 +480,108 @@
             # args0 is a tuple of all strings (e.g. names of attributes)
             attrs = cls.__make_astrs__(attrs=arg0, *args[1:], **kwargs)
             return attrs[0] if len(attrs) == 1 else attrs
         
         else:
             # called with arguments, but not all are strings, use the classes __call__ method
             return cls.__call__(cls, *args, **kwargs)
-        return cls.__make_astrs__(*args, **kwargs)
-    
     
     def __deco__(cls, **kwargs: P.kwargs):
         def decorator(sub: type):
             return cls.__make_astr__(sub.__name__, bases=(cls, ), **kwargs)
         return decorator
     
     @wraps(insattr)
-    def get(cls, obj: object) -> Union[Any, bool, object]:
+    def get(cls, item: object) -> Union[Any, bool, object]:
         '''Get the attribute specified by the this class from the object.'''
         if DOT in cls.attr: 
-            return cls.dot(obj, rethas = False)
-        return insattr(obj, rethas = False, **cls.getvars())
+            return cls.dot(item, ret_option = ReturnOption.default)
+        kwds = {**cls.getvars(), **dict(ret_option = ReturnOption.default)}
+        return insattr(item, **kwds)
     
     @wraps(insattr)
-    def has(cls, obj: object) -> TypeGuard[bool]:
+    def has(cls, item: object) -> TypeGuard[bool]:
         '''Returns whether the object has the attribute specified by the this class.'''
-        if DOT in cls.attr: return cls.dot(obj, rethas=True)
-        return insattr(obj, rethas=True, **cls.getvars())
+        if DOT in cls.attr: return cls.dot(item, ret_option = ReturnOption.has)
+        kwds = {**cls.getvars(), **dict(ret_option = ReturnOption.has)}
+        return insattr(item, **kwds)
     
-    def set(cls, obj: object, val: Any) -> Type[Self]:
+    def set(cls, item: object, val: Any) -> Type[Self]:
         '''Set the attribute specified by the this class on the object to the value `val`.'''
-        setattr(obj, cls.attr, val)
+        setattr(item, cls.attr, val)
         return cls
     
-    def dot(cls, obj: object, **kwargs:P.kwargs):
+    def dot(cls, item: object, **kwargs:P.kwargs):
         '''Returns get(...) --> get(...) --> ... --> get / has for a dotted attribute name e.g. `attr1.attr2.attr3`.'''
         names = getattr(cls, ATTR, NIL).split(DOT)
-        return cls.chain(obj, *names, **kwargs)
+        return cls.chain(item, *names, **kwargs)
     
-    def chain(cls, obj: object, *names: P.args, **kwargs: P.kwargs):
+    def chain(cls, item: object, *names: P.args, **kwargs: P.kwargs):
         '''Returns chain cls.get until for each attribute in *names until the end, then call get / has 
         for a dotted attribute name e.g. `attr1.attr2.attr3`.'''
         kwds = cls.getvars(**kwargs)
+        retopt = kwargs.get('return_opt')
         rethas = kwargs.get(RETHAS, False)
+        if rethas: 
+            retopt = ReturnOption.has
+            
         for i, name in enumerate(names):
-            cur = dict(attr=name, rethas=False, retself=True)
-            for key in ('guard', 'guardobj'):
+            cur = dict(attr=name, rethas=False, ret_option=True)
+            for key in ('attr_guard', 'item_guard'):
                 val = kwds.get(key, None)
                 if not isiter(val):
                     kwds[key] = notnone
                 elif isiter(val) and i >= len(val):
                     kwds[key] = notnone
                 elif isiter(val) and i < len(val):
                     cur[key] = val[i]
                     
             kws = {**kwds, **cur}
             if i == len(names) - 1: 
-                kws.update(rethas = rethas)
-            obj = insattr(obj, **kws)
-        return obj
+                kws.update(return_opt = retopt)
+            item = insattr(item, **kws)
+        return item
     
     def __repr__(cls) -> str:
         return f'{cls.__name__}({cls.attr})'
     
     def __str__(cls) -> str:
         return f'{cls.__name__}({cls.attr})'
 
-# %% ../nbs/00_core.ipynb 26
+# %% ../nbs/00_core.ipynb 30
 class astr(metaclass=astrmeta):
     '''Provides a flexible and powerful interface for getting, setting, and checking if an object has a specific attribute.
     
     Instances of `astr` (or subclasses thereof) represent specific attributes and encapsulate logic for accessing, setting, and 
     verifying the presence of these attributes on objects. This enables expressive and concise attribute manipulation and 
     introspection. `astr` classes support creating attribute-specific behavior directly or through decoration, offering a 
     versatile tool for object attribute management.
 
     Attributes
     ----------
     attr : str
-        The name of the attribute to get, set, or check on an object.
+        The name of the attribute to get, set, or check_attr on an object.
         
-    check : bool
-        Indicates whether to check the type of the attribute upon retrieval.
+    check_attr : bool
+        Indicates whether to check_attr the type of the attribute upon retrieval.
         
-    guard : GuardLike, optional
-        A callable used as a type guard for the retrieved attribute.
+    attr_guard : GuardLike, optional
+        A callable used as a type attr_guard for the retrieved attribute.
         
-    checkobj : bool, optional
-        Indicates whether to check the type of the object before attribute manipulation.
+    check_item : bool, optional
+        Indicates whether to check_attr the type of the object before attribute manipulation.
         
-    guardobj : GuardLike, optional
-        A callable used as a type guard for the object before attribute manipulation.
+    item_guard : GuardLike, optional
+        A callable used as a type attr_guard for the object before attribute manipulation.
         
-    retself : bool
-        Determines whether to return the original object if the attribute fails the type guard check.
+    ret_option : bool
+        Determines whether to return the original object if the attribute fails the type attr_guard check_attr.
         
     default : Any
-        The default value to return if the attribute is not found or fails the type guard check.
+        The default value to return if the attribute is not found or fails the type attr_guard check_attr.
     
     Notes
     -----
     `astr` can be subclassed to create attribute-specific classes that include logic for getting, 
     setting, and checking attributes on objects. It supports dot notation for nested attributes and 
     can be used directly or as a decorator to enhance classes with attribute-specific logic.
     
@@ -488,49 +590,57 @@
     >>> class foo(attr):
     ...    attr = 'foo'
     
     >>> class bar(attr):
     ...    attr = 'bar'
     
     >>> # Decorator usage to enhance a class with attribute-specific logic
-    ... @attr.deco(check=False)
+    ... @attr.deco(check_attr=False)
     ... class quz: ...
     '''
     attr: ClassVar[str]
-    '''The name of the attribute to get / set / or check if an object has.'''
+    '''The name of the attribute to get / set / or check_attr if an object has.'''
     
-    check: ClassVar[bool] = True
-    '''Whether to check the type of the attribute, by default True.'''
+    check_attr: ClassVar[bool] = True
+    '''Whether to check_attr the type of the attribute, by default True.'''
     
-    guard: ClassVar[Optional[GuardLike]] = notnone
-    '''The guard to check the type of the retrieved attribute, by default `notnone`.'''
+    attr_guard: ClassVar[Optional[GuardLike]] = notnone
+    '''The attr_guard to check_attr the type of the retrieved attribute, by default `notnone`.'''
     
-    checkobj: ClassVar[Optional[bool]] = True
-    '''The guard to check the type of the object, by default None.'''
+    check_item: ClassVar[Optional[bool]] = True
+    '''The attr_guard to check_attr the type of the object, by default None.'''
     
-    guardobj: ClassVar[Optional[GuardLike]] = notnone
-    '''The guard to check the type of the object, by default `notnone`.'''
+    item_guard: ClassVar[Optional[GuardLike]] = notnone
+    '''The attr_guard to check_attr the type of the object, by default `notnone`.'''
     
-    retself: ClassVar[bool] = True
-    '''Whether to return the object if the attribute fails the guard, otherwise the default value is returned, by default False.'''
+    ret_option: ClassVar[ReturnOption] = ReturnOption.self
+    '''Whether to return the object if the attribute fails the attr_guard, otherwise the default value is returned, by default False.'''
     
     default: ClassVar[Any] = None
     '''The default value to return if the attribute is not found, by default None.'''
     
+    return_fnc: ClassVar[ReturnFunction] = make_return_fnc
+    
+    attr_mode: ClassVar[AttributeMode] = AttributeMode.GET
+    
     clsvars: tuple[str, ...] = CLASSVARS
     '''The tuple of class variable names.'''
     
     def __new__(cls, *args: P.args, **kwargs: P.kwargs):
         if args: return cls.many(*args, **kwargs)
         if kwargs: return cls.deco(**kwargs)
         new = super().__new__(cls)
         return new
     
-    def __call__(self, obj: object, *args: P.args, **kwargs: P.kwargs) -> object:
-        return self.get(obj) if kwargs.get(GET, True) else self.has(obj)
+    
+    def __call__(self, item: object, *args: P.args, **kwargs: P.kwargs) -> object:
+        rethas = kwargs.get(HAS, self.attr_mode == AttributeMode.HAS)
+        if rethas == ReturnOption.has:
+            return self.has(item)
+        return self.get(item)
     
     def __init_subclass__(cls, *args: P.args, **kwargs: P.kwargs):
         super().__init_subclass__()
         # NOTE: likely unneeded as it is called in __new__
         cls.setvars(**kwargs)
         
     @classmethod
@@ -549,15 +659,15 @@
         if istuple(attrs) and len(attrs) == 1: return attrs[0]
         return attrs
     
     @classmethod
     def deco(cls: Type[Self], **kwargs: P.kwargs) -> Type[Self]:
         return cls.__deco__(**kwargs)
 
-# %% ../nbs/00_core.ipynb 28
+# %% ../nbs/00_core.ipynb 32
 @wraps(astr, assigned=ASSIGNED, updated=()) 
 class attr(astr):
     '''An alias for the `astr` class.
     
     See Also
     --------
     astr : A class for getting, setting and checking if an object has an attribute.
@@ -567,7 +677,74 @@
 class attrstr(astr):
     '''An alias for the `astr` class.
     
     See Also
     --------
     astr : A class for getting, setting and checking if an object has an attribute.
     '''
+
+# %% ../nbs/00_core.ipynb 33
+class attribute_meta(type):
+    clsvars: tuple[str, ...] = CLASSVARS
+    '''The tuple of class variable names.'''
+    def __new__(cls, name: str, bases: tuple = tuple(), dct: dict = dict(), *args: P.args, **kwargs: P.kwargs):
+        kwargs.setdefault('__args', args)
+        new = super().__new__(cls, name, bases, dct)
+        new.setvars(**kwargs)
+        return new
+    
+    def getvars(cls, **kwargs: P.kwargs) -> dict:
+        '''Returns a dictionary of class variables using class defaults if not found in `kwargs`.'''
+        return {a: kwargs.get(a, getattr(cls, a, None)) for a in cls.clsvars}
+    
+    def setvars(cls, **kwargs: P.kwargs):
+        '''Set all class variables using their defaults values if not found in `kwargs`.'''
+        for k, v in cls.getvars(**kwargs).items(): setattr(cls, k, v)
+        clsattr = getattr(cls, ATTR, NIL)
+        clsname = getattr(cls, __NAME__, NIL).lower()
+        # no attr but class has a name, use that for the attribute
+        if not clsattr and clsname: setattr(cls, ATTR, clsname)
+        return cls
+    
+    def __init__(cls, name: str, bases: tuple = tuple(), dct: dict = dict(), *args: P.args, **kwargs: P.kwargs):
+        super().__init__(name, bases, dct)
+        # NOTE: likely unneeded as it is called in __new__
+        cls.setvars(**kwargs)
+            
+    def __init_subclass__(cls, *args: P.args, **kwargs: P.kwargs):
+        super().__init_subclass__(*args, **kwargs)
+        # NOTE: likely unneeded as it is called in __new__
+        cls.setvars(**kwargs)
+    
+    
+    
+    def inspect(cls, item: object, attr: str, **kwargs):
+        kwds = cls.getvars(attr=attr, **kwargs)
+        return insattr(item, **kwds)
+    
+    def __repr__(cls) -> str:
+        return f'{cls.__name__}({cls.attr})'
+    
+    def __str__(cls) -> str:
+        return f'{cls.__name__}({cls.attr})'
+    
+    def __call__(self, 
+        item: object,
+        default: Any = None,
+        check_attr: bool = True,
+        attr_guard: Optional[GuardLike] = notnone,
+        check_item: Optional[bool] = None, 
+        item_guard: Optional[GuardLike] = notnone, 
+        ret_option: ReturnOption = ReturnOption.default,
+        return_fnc: Optional[ReturnFunction] = make_return_fnc,
+        **kwargs: P.kwargs
+    ):
+        return self.inspect(item, self.attr,
+            default=default, check_attr=check_attr, attr_guard=attr_guard, check_item=check_item, 
+            item_guard=item_guard, ret_option=ret_option, return_fnc=return_fnc, **kwargs
+        )
+    
+class attribute(metaclass=attribute_meta):
+    ...
+    # def __new__(cls, *args: P.args, **kwargs: P.kwargs):
+    #     new = super().__new__(cls)
+    #     return new
```

### Comparing `astr-0.0.6/astr.egg-info/PKG-INFO` & `astr-0.0.7/astr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astr
-Version: 0.0.6
+Version: 0.0.7
 Summary: astr (attribute string) for defined getter / setter methods
 Home-page: https://github.com/dsm-72/astr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: attr str attribute string astr attrstr python alias type astr typ get set instance ins insattr getter setter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `astr-0.0.6/settings.ini` & `astr-0.0.7/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = astr
 lib_name = astr
-version = 0.0.6
+version = 0.0.7
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = astr
 nbs_path = nbs
 recursive = True
```

### Comparing `astr-0.0.6/setup.py` & `astr-0.0.7/setup.py`

 * *Files identical despite different names*

