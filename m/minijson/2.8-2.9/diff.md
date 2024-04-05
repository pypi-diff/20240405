# Comparing `tmp/minijson-2.8.tar.gz` & `tmp/minijson-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minijson-2.8.tar", last modified: Fri Aug  6 16:09:25 2021, max compression
+gzip compressed data, was "dist/minijson-2.9.tar", last modified: Fri Aug  6 16:57:23 2021, max compression
```

## Comparing `minijson-2.8.tar` & `minijson-2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-06 16:09:25.000000 minijson-2.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2984 2021-08-06 16:09:25.000000 minijson-2.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2021-08-06 16:08:58.000000 minijson-2.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-06 16:09:25.000000 minijson-2.8/minijson.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2984 2021-08-06 16:09:25.000000 minijson-2.8/minijson.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-06 16:09:25.000000 minijson-2.8/minijson.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-08-06 16:09:25.000000 minijson-2.8/minijson.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2021-08-06 16:09:25.000000 minijson-2.8/minijson.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   834603 2021-08-06 16:09:19.000000 minijson-2.8/minijson.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1239 2021-08-06 16:09:25.000000 minijson-2.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2021-08-06 16:08:58.000000 minijson-2.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      622 2021-08-06 16:08:58.000000 minijson-2.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-06 16:57:23.000000 minijson-2.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2021-08-06 16:57:23.000000 minijson-2.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2021-08-06 16:56:57.000000 minijson-2.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-06 16:57:23.000000 minijson-2.9/minijson.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      175 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   803310 2021-08-06 16:57:17.000000 minijson-2.9/minijson.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1239 2021-08-06 16:57:23.000000 minijson-2.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2021-08-06 16:56:57.000000 minijson-2.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      622 2021-08-06 16:56:57.000000 minijson-2.9/setup.py
```

### Comparing `minijson-2.8/PKG-INFO` & `minijson-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minijson
-Version: 2.8
+Version: 2.9
 Summary: A library for serializing JSON in a small binary format
 Home-page: https://github.com/Dronehub/minijson
 Author: Piotr Maślanka
 Author-email: piotr.maslanka@dronehub.ai
 License: UNKNOWN
 Project-URL: Documentation, https://minijson.readthedocs.io/
 Project-URL: Code, https://github.com/Dronehub/minijson
@@ -36,14 +36,16 @@
         compile it yourself.
         Alternatively, you can
         [file an issue](https://github.com/Dronehub/minijson/issues/new)
         and I'll do my best to compile a wheel for you.
         
         In order to do that you must have `Cython` installed.
         
+        Run the Dockerfile to launch unit tests locally.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `minijson-2.8/README.md` & `minijson-2.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 If there are no binary wheels precompiled for this platform, you will need to
 compile it yourself.
 Alternatively, you can
 [file an issue](https://github.com/Dronehub/minijson/issues/new)
 and I'll do my best to compile a wheel for you.
 
 In order to do that you must have `Cython` installed.
+
+Run the Dockerfile to launch unit tests locally.
```

### Comparing `minijson-2.8/minijson.egg-info/PKG-INFO` & `minijson-2.9/minijson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minijson
-Version: 2.8
+Version: 2.9
 Summary: A library for serializing JSON in a small binary format
 Home-page: https://github.com/Dronehub/minijson
 Author: Piotr Maślanka
 Author-email: piotr.maslanka@dronehub.ai
 License: UNKNOWN
 Project-URL: Documentation, https://minijson.readthedocs.io/
 Project-URL: Code, https://github.com/Dronehub/minijson
@@ -36,14 +36,16 @@
         compile it yourself.
         Alternatively, you can
         [file an issue](https://github.com/Dronehub/minijson/issues/new)
         and I'll do my best to compile a wheel for you.
         
         In order to do that you must have `Cython` installed.
         
+        Run the Dockerfile to launch unit tests locally.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `minijson-2.8/minijson.c` & `minijson-2.9/minijson.c`

 * *Files 5% similar despite different names*

```diff
@@ -841,51 +841,51 @@
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8minijson_MiniJSONEncoder;
 struct __pyx_opt_args_8minijson_dump;
 struct __pyx_opt_args_8minijson_dumps;
 struct __pyx_opt_args_8minijson_dumps_object;
 
-/* "minijson.pyx":563
+/* "minijson.pyx":550
  * 
  * 
  * cpdef int dump(object data, cio: io.BytesIO, default: tp.Optional[tp.Callable] = None) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Write an object to a stream.
  */
 struct __pyx_opt_args_8minijson_dump {
   int __pyx_n;
   PyObject *__pyx_default;
 };
 
-/* "minijson.pyx":584
+/* "minijson.pyx":571
  * 
  * 
  * cpdef bytes dumps(object data, default: tp.Optional[tp.Callable] = None):             # <<<<<<<<<<<<<<
  *     """
  *     Serialize given data to a MiniJSON representation.
  */
 struct __pyx_opt_args_8minijson_dumps {
   int __pyx_n;
   PyObject *__pyx_default;
 };
 
-/* "minijson.pyx":604
+/* "minijson.pyx":591
  * 
  * 
  * cpdef bytes dumps_object(object data, default: tp.Optional[tp.Callable] = None):             # <<<<<<<<<<<<<<
  *     """
  *     Dump an object's :code:`__dict__`.
  */
 struct __pyx_opt_args_8minijson_dumps_object {
   int __pyx_n;
   PyObject *__pyx_default;
 };
 
-/* "minijson.pyx":317
+/* "minijson.pyx":308
  * 
  * 
  * cdef class MiniJSONEncoder:             # <<<<<<<<<<<<<<
  *     """
  *     A base class for encoders.
  */
 struct __pyx_obj_8minijson_MiniJSONEncoder {
@@ -1292,38 +1292,35 @@
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* JoinPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       Py_UCS4 max_char);
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_LshiftObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_LshiftObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceLshift(op1, op2) : PyNumber_Lshift(op1, op2))
-#endif
-
-/* bytes_index.proto */
-static CYTHON_INLINE char __Pyx_PyBytes_GetItemInt(PyObject* bytes, Py_ssize_t index, int check_bounds);
-
 /* ListExtend.proto */
 static CYTHON_INLINE int __Pyx_PyList_Extend(PyObject* L, PyObject* v) {
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject* none = _PyList_Extend((PyListObject*)L, v);
     if (unlikely(!none))
         return -1;
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* PyIntBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_LshiftObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
+#else
+#define __Pyx_PyInt_LshiftObjC(op1, op2, intval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceLshift(op1, op2) : PyNumber_Lshift(op1, op2))
+#endif
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
@@ -1445,32 +1442,14 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE unsigned short __Pyx_PyInt_As_unsigned_short(PyObject *);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_short(unsigned short value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value);
-
-/* CIntFromPy.proto */
-static CYTHON_INLINE unsigned char __Pyx_PyInt_As_unsigned_char(PyObject *);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_char(unsigned char value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
-
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static int __pyx_f_8minijson_15MiniJSONEncoder_dump(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_cio, int __pyx_skip_dispatch); /* proto*/
@@ -1550,14 +1529,15 @@
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_dump[] = "dump";
 static const char __pyx_k_keys[] = "keys";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_pack[] = "pack";
+static const char __pyx_k_sort[] = "sort";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_write[] = "write";
 static const char __pyx_k_Struct[] = "Struct";
@@ -1719,14 +1699,15 @@
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_should_double_be_used;
 static PyObject *__pyx_n_s_signed;
+static PyObject *__pyx_n_s_sort;
 static PyObject *__pyx_n_s_starting_position;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_to_bytes;
 static PyObject *__pyx_n_s_tp;
 static PyObject *__pyx_n_s_typing;
@@ -1737,15 +1718,15 @@
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_write;
 static PyObject *__pyx_pf_8minijson_switch_default_float(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8minijson_2switch_default_double(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8minijson_4parse(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, int __pyx_v_starting_position); /* proto */
 static PyObject *__pyx_pf_8minijson_6loads(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
 static int __pyx_pf_8minijson_15MiniJSONEncoder___init__(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_default, int __pyx_v_use_double, int __pyx_v_use_strict_order); /* proto */
-static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_2should_double_be_used(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_y); /* proto */
+static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_2should_double_be_used(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, CYTHON_UNUSED double __pyx_v_y); /* proto */
 static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_4default(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_6encode(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_8dump(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_cio); /* proto */
 static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_10use_double___get__(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self); /* proto */
 static int __pyx_pf_8minijson_15MiniJSONEncoder_10use_double_2__set__(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_16use_strict_order___get__(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self); /* proto */
 static int __pyx_pf_8minijson_15MiniJSONEncoder_16use_strict_order_2__set__(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
@@ -2965,19 +2946,14 @@
 static PyObject *__pyx_f_8minijson_parse_bytes(PyObject *__pyx_v_data, int __pyx_v_starting_position) {
   int __pyx_v_value_type;
   int __pyx_v_string_length;
   int __pyx_v_elements;
   int __pyx_v_offset;
   unsigned int __pyx_v_uint32;
   unsigned int __pyx_v_length;
-  int __pyx_v_sint32;
-  unsigned short __pyx_v_uint16;
-  short __pyx_v_sint16;
-  unsigned char __pyx_v_uint8;
-  char __pyx_v_sint8;
   PyObject *__pyx_v_e_list = 0;
   PyObject *__pyx_v_e_dict = 0;
   PyObject *__pyx_v_b_field_name = 0;
   PyObject *__pyx_v_byte_data = 0;
   PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -3004,20 +2980,17 @@
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   PyObject *__pyx_t_23 = NULL;
   PyObject *__pyx_t_24 = NULL;
   PyObject *__pyx_t_25 = NULL;
   long __pyx_t_26;
   char const *__pyx_t_27;
-  int __pyx_t_28;
-  unsigned int __pyx_t_29;
-  unsigned short __pyx_t_30;
-  char __pyx_t_31;
-  PyObject *(*__pyx_t_32)(PyObject *);
-  char const *__pyx_t_33;
+  unsigned int __pyx_t_28;
+  PyObject *(*__pyx_t_29)(PyObject *);
+  char const *__pyx_t_30;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_bytes", 0);
 
   /* "minijson.pyx":146
  *         bytes b_field_name, byte_data
@@ -3830,15 +3803,15 @@
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
           /* "minijson.pyx":177
  *             try:
  *                 return offset+1, b_field_name.decode('utf-8')
  *             except UnicodeDecodeError as e:             # <<<<<<<<<<<<<<
  *                 raise DecodingError('Invalid UTF-8') from e
- *         elif value_type in (1, 4):
+ *         elif value_type == 1:
  */
           __pyx_t_18 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_UnicodeDecodeError);
           if (__pyx_t_18) {
             __Pyx_AddTraceback("minijson.parse_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
             if (__Pyx_GetException(&__pyx_t_12, &__pyx_t_14, &__pyx_t_4) < 0) __PYX_ERR(0, 177, __pyx_L31_except_error)
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_GOTREF(__pyx_t_14);
@@ -3847,16 +3820,16 @@
             __pyx_v_e = __pyx_t_14;
             /*try:*/ {
 
               /* "minijson.pyx":178
  *                 return offset+1, b_field_name.decode('utf-8')
  *             except UnicodeDecodeError as e:
  *                 raise DecodingError('Invalid UTF-8') from e             # <<<<<<<<<<<<<<
- *         elif value_type in (1, 4):
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]
+ *         elif value_type == 1:
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])
  */
               __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 178, __pyx_L40_error)
               __Pyx_GOTREF(__pyx_t_16);
               __pyx_t_17 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_16))) {
                 __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_16);
                 if (likely(__pyx_t_17)) {
@@ -3877,15 +3850,15 @@
             }
 
             /* "minijson.pyx":177
  *             try:
  *                 return offset+1, b_field_name.decode('utf-8')
  *             except UnicodeDecodeError as e:             # <<<<<<<<<<<<<<
  *                 raise DecodingError('Invalid UTF-8') from e
- *         elif value_type in (1, 4):
+ *         elif value_type == 1:
  */
             /*finally:*/ {
               __pyx_L40_error:;
               /*exception exit:*/{
                 __Pyx_PyThreadState_declare
                 __Pyx_PyThreadState_assign
                 __pyx_t_25 = 0; __pyx_t_24 = 0; __pyx_t_23 = 0; __pyx_t_22 = 0; __pyx_t_21 = 0; __pyx_t_20 = 0;
@@ -3952,2838 +3925,2841 @@
  *             offset, b_field_name = parse_cstring(data, starting_position+1)
  */
       }
 
       /* "minijson.pyx":179
  *             except UnicodeDecodeError as e:
  *                 raise DecodingError('Invalid UTF-8') from e
- *         elif value_type in (1, 4):             # <<<<<<<<<<<<<<
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]
- *             if value_type == 4:
- */
-      switch (__pyx_v_value_type) {
-        case 1:
-        case 4:
-        __pyx_t_6 = 1;
-        break;
-        default:
-        __pyx_t_6 = 0;
-        break;
-      }
-      __pyx_t_28 = (__pyx_t_6 != 0);
-      if (__pyx_t_28) {
+ *         elif value_type == 1:             # <<<<<<<<<<<<<<
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 4:
+ */
+      __pyx_t_6 = ((__pyx_v_value_type == 1) != 0);
+      if (__pyx_t_6) {
 
         /* "minijson.pyx":180
  *                 raise DecodingError('Invalid UTF-8') from e
- *         elif value_type in (1, 4):
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]             # <<<<<<<<<<<<<<
- *             if value_type == 4:
- *                 return 5, uint32
+ *         elif value_type == 1:
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
+ *         elif value_type == 4:
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  */
-        __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_14 = __Pyx_PyInt_LshiftObjC(__pyx_t_4, __pyx_int_24, 24, 0, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_26 = (__pyx_v_starting_position + 2);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_12 = __Pyx_PyInt_LshiftObjC(__pyx_t_4, __pyx_int_16, 16, 0, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = PyNumber_Or(__pyx_t_14, __pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_26 = (__pyx_v_starting_position + 3);
-        __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_14 = __Pyx_PyInt_LshiftObjC(__pyx_t_12, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 180, __pyx_L3_error)
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 180, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_12 = PyNumber_Or(__pyx_t_4, __pyx_t_14); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L3_error)
+        __Pyx_INCREF(__pyx_int_5);
+        __Pyx_GIVEREF(__pyx_int_5);
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_5);
+        __pyx_t_4 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_l, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_t_26 = (__pyx_v_starting_position + 4);
-        __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 180, __pyx_L3_error)
+        if (unlikely(__pyx_v_data == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+          __PYX_ERR(0, 180, __pyx_L3_error)
+        }
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 180, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_12);
+          if (likely(__pyx_t_16)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+            __Pyx_INCREF(__pyx_t_16);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
+          }
+        }
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 180, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_4 = PyNumber_Or(__pyx_t_12, __pyx_t_14); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_t_14) < 0) __PYX_ERR(0, 180, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_t_29 = __Pyx_PyInt_As_unsigned_int(__pyx_t_4); if (unlikely((__pyx_t_29 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_v_uint32 = __pyx_t_29;
-
-        /* "minijson.pyx":181
- *         elif value_type in (1, 4):
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]
- *             if value_type == 4:             # <<<<<<<<<<<<<<
- *                 return 5, uint32
- *             else:
- */
-        __pyx_t_28 = ((__pyx_v_value_type == 4) != 0);
-        if (__pyx_t_28) {
-
-          /* "minijson.pyx":182
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]
- *             if value_type == 4:
- *                 return 5, uint32             # <<<<<<<<<<<<<<
- *             else:
- *                 sint32 = uint32
- */
-          __Pyx_XDECREF(__pyx_r);
-          __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_uint32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 182, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 182, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
-          __Pyx_INCREF(__pyx_int_5);
-          __Pyx_GIVEREF(__pyx_int_5);
-          PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_int_5);
-          __Pyx_GIVEREF(__pyx_t_4);
-          PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_4);
-          __pyx_t_4 = 0;
-          __pyx_r = ((PyObject*)__pyx_t_14);
-          __pyx_t_14 = 0;
-          goto __pyx_L7_try_return;
-
-          /* "minijson.pyx":181
- *         elif value_type in (1, 4):
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]
- *             if value_type == 4:             # <<<<<<<<<<<<<<
- *                 return 5, uint32
- *             else:
- */
-        }
-
-        /* "minijson.pyx":184
- *                 return 5, uint32
- *             else:
- *                 sint32 = uint32             # <<<<<<<<<<<<<<
- *                 return 5, sint32
- *         elif value_type in (2, 5):
- */
-        /*else*/ {
-          __pyx_v_sint32 = __pyx_v_uint32;
-
-          /* "minijson.pyx":185
- *             else:
- *                 sint32 = uint32
- *                 return 5, sint32             # <<<<<<<<<<<<<<
- *         elif value_type in (2, 5):
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]
- */
-          __Pyx_XDECREF(__pyx_r);
-          __pyx_t_14 = __Pyx_PyInt_From_int(__pyx_v_sint32); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 185, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
-          __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L3_error)
+        {
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_4);
+          __pyx_t_4 = __pyx_temp; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_INCREF(__pyx_int_5);
-          __Pyx_GIVEREF(__pyx_int_5);
-          PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_5);
-          __Pyx_GIVEREF(__pyx_t_14);
-          PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_14);
-          __pyx_t_14 = 0;
-          __pyx_r = ((PyObject*)__pyx_t_4);
-          __pyx_t_4 = 0;
-          goto __pyx_L7_try_return;
         }
+        __pyx_r = ((PyObject*)__pyx_t_4);
+        __pyx_t_4 = 0;
+        goto __pyx_L7_try_return;
 
         /* "minijson.pyx":179
  *             except UnicodeDecodeError as e:
  *                 raise DecodingError('Invalid UTF-8') from e
- *         elif value_type in (1, 4):             # <<<<<<<<<<<<<<
- *             uint32 = (data[starting_position+1] << 24) | (data[starting_position+2] << 16) | (data[starting_position+3] << 8) | data[starting_position+4]
- *             if value_type == 4:
+ *         elif value_type == 1:             # <<<<<<<<<<<<<<
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 4:
  */
       }
 
-      /* "minijson.pyx":186
- *                 sint32 = uint32
- *                 return 5, sint32
- *         elif value_type in (2, 5):             # <<<<<<<<<<<<<<
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]
- *             if value_type == 5:
- */
-      switch (__pyx_v_value_type) {
-        case 2:
-        case 5:
-        __pyx_t_28 = 1;
-        break;
-        default:
-        __pyx_t_28 = 0;
-        break;
-      }
-      __pyx_t_6 = (__pyx_t_28 != 0);
+      /* "minijson.pyx":181
+ *         elif value_type == 1:
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 4:             # <<<<<<<<<<<<<<
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 2:
+ */
+      __pyx_t_6 = ((__pyx_v_value_type == 4) != 0);
       if (__pyx_t_6) {
 
-        /* "minijson.pyx":187
- *                 return 5, sint32
- *         elif value_type in (2, 5):
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]             # <<<<<<<<<<<<<<
- *             if value_type == 5:
- *                 return 3, uint16
+        /* "minijson.pyx":182
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 4:
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
+ *         elif value_type == 2:
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])
  */
-        __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_14 = __Pyx_PyInt_LshiftObjC(__pyx_t_4, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 187, __pyx_L3_error)
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 182, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_26 = (__pyx_v_starting_position + 2);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_12 = PyNumber_Or(__pyx_t_14, __pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 187, __pyx_L3_error)
+        __Pyx_INCREF(__pyx_int_5);
+        __Pyx_GIVEREF(__pyx_int_5);
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_5);
+        __pyx_t_4 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 182, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_30 = __Pyx_PyInt_As_unsigned_short(__pyx_t_12); if (unlikely((__pyx_t_30 == (unsigned short)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
+        if (unlikely(__pyx_v_data == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+          __PYX_ERR(0, 182, __pyx_L3_error)
+        }
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 182, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_12);
+          if (likely(__pyx_t_16)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+            __Pyx_INCREF(__pyx_t_16);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
+          }
+        }
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 182, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_v_uint16 = __pyx_t_30;
-
-        /* "minijson.pyx":188
- *         elif value_type in (2, 5):
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]
- *             if value_type == 5:             # <<<<<<<<<<<<<<
- *                 return 3, uint16
- *             else:
- */
-        __pyx_t_6 = ((__pyx_v_value_type == 5) != 0);
-        if (__pyx_t_6) {
-
-          /* "minijson.pyx":189
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]
- *             if value_type == 5:
- *                 return 3, uint16             # <<<<<<<<<<<<<<
- *             else:
- *                 sint16 = uint16
- */
-          __Pyx_XDECREF(__pyx_r);
-          __pyx_t_12 = __Pyx_PyInt_From_unsigned_short(__pyx_v_uint16); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 189, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L3_error)
+        if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_t_14) < 0) __PYX_ERR(0, 182, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        {
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_4);
+          __pyx_t_4 = __pyx_temp; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 182, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_INCREF(__pyx_int_3);
-          __Pyx_GIVEREF(__pyx_int_3);
-          PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_3);
-          __Pyx_GIVEREF(__pyx_t_12);
-          PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_12);
-          __pyx_t_12 = 0;
-          __pyx_r = ((PyObject*)__pyx_t_4);
-          __pyx_t_4 = 0;
-          goto __pyx_L7_try_return;
+        }
+        __pyx_r = ((PyObject*)__pyx_t_4);
+        __pyx_t_4 = 0;
+        goto __pyx_L7_try_return;
 
-          /* "minijson.pyx":188
- *         elif value_type in (2, 5):
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]
- *             if value_type == 5:             # <<<<<<<<<<<<<<
- *                 return 3, uint16
- *             else:
+        /* "minijson.pyx":181
+ *         elif value_type == 1:
+ *             return 5, *STRUCT_l.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 4:             # <<<<<<<<<<<<<<
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 2:
  */
-        }
+      }
 
-        /* "minijson.pyx":191
- *                 return 3, uint16
- *             else:
- *                 sint16 = uint16             # <<<<<<<<<<<<<<
- *                 return 3, sint16
- *         elif value_type in (3, 6):
+      /* "minijson.pyx":183
+ *         elif value_type == 4:
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 2:             # <<<<<<<<<<<<<<
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 5:
  */
-        /*else*/ {
-          __pyx_v_sint16 = __pyx_v_uint16;
+      __pyx_t_6 = ((__pyx_v_value_type == 2) != 0);
+      if (__pyx_t_6) {
 
-          /* "minijson.pyx":192
- *             else:
- *                 sint16 = uint16
- *                 return 3, sint16             # <<<<<<<<<<<<<<
- *         elif value_type in (3, 6):
- *             uint8 = data[starting_position+1]
+        /* "minijson.pyx":184
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 2:
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
+ *         elif value_type == 5:
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  */
-          __Pyx_XDECREF(__pyx_r);
-          __pyx_t_4 = __Pyx_PyInt_From_short(__pyx_v_sint16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L3_error)
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 184, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_INCREF(__pyx_int_3);
+        __Pyx_GIVEREF(__pyx_int_3);
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_3);
+        __pyx_t_4 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_h, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 184, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(__pyx_v_data == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+          __PYX_ERR(0, 184, __pyx_L3_error)
+        }
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 184, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_12);
+          if (likely(__pyx_t_16)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+            __Pyx_INCREF(__pyx_t_16);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
+          }
+        }
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 184, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_t_14) < 0) __PYX_ERR(0, 184, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        {
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_4);
+          __pyx_t_4 = __pyx_temp; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 192, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __Pyx_INCREF(__pyx_int_3);
-          __Pyx_GIVEREF(__pyx_int_3);
-          PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_int_3);
-          __Pyx_GIVEREF(__pyx_t_4);
-          PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_4);
-          __pyx_t_4 = 0;
-          __pyx_r = ((PyObject*)__pyx_t_12);
-          __pyx_t_12 = 0;
-          goto __pyx_L7_try_return;
         }
+        __pyx_r = ((PyObject*)__pyx_t_4);
+        __pyx_t_4 = 0;
+        goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":186
- *                 sint32 = uint32
- *                 return 5, sint32
- *         elif value_type in (2, 5):             # <<<<<<<<<<<<<<
- *             uint16 = (data[starting_position+1] << 8) | data[starting_position+2]
- *             if value_type == 5:
+        /* "minijson.pyx":183
+ *         elif value_type == 4:
+ *             return 5, *STRUCT_L.unpack(data[starting_position+1:starting_position+5])
+ *         elif value_type == 2:             # <<<<<<<<<<<<<<
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 5:
  */
       }
 
-      /* "minijson.pyx":193
- *                 sint16 = uint16
- *                 return 3, sint16
- *         elif value_type in (3, 6):             # <<<<<<<<<<<<<<
- *             uint8 = data[starting_position+1]
- *             if value_type == 6:
- */
-      switch (__pyx_v_value_type) {
-        case 3:
-        case 6:
-        __pyx_t_6 = 1;
-        break;
-        default:
-        __pyx_t_6 = 0;
-        break;
-      }
-      __pyx_t_28 = (__pyx_t_6 != 0);
-      if (__pyx_t_28) {
+      /* "minijson.pyx":185
+ *         elif value_type == 2:
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 5:             # <<<<<<<<<<<<<<
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 3:
+ */
+      __pyx_t_6 = ((__pyx_v_value_type == 5) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":194
- *                 return 3, sint16
- *         elif value_type in (3, 6):
- *             uint8 = data[starting_position+1]             # <<<<<<<<<<<<<<
- *             if value_type == 6:
- *                 return 2, uint8
+        /* "minijson.pyx":186
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 5:
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
+ *         elif value_type == 3:
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])
  */
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 186, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_INCREF(__pyx_int_3);
+        __Pyx_GIVEREF(__pyx_int_3);
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_3);
+        __pyx_t_4 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 186, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 194, __pyx_L3_error)
+          __PYX_ERR(0, 186, __pyx_L3_error)
         }
-        __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_31 = __Pyx_PyBytes_GetItemInt(__pyx_v_data, __pyx_t_26, 1); if (unlikely(__pyx_t_31 == ((char)((char)-1)) && PyErr_Occurred())) __PYX_ERR(0, 194, __pyx_L3_error)
-        __pyx_v_uint8 = __pyx_t_31;
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 186, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_12);
+          if (likely(__pyx_t_16)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+            __Pyx_INCREF(__pyx_t_16);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
+          }
+        }
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 186, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_t_14) < 0) __PYX_ERR(0, 186, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        {
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_4);
+          __pyx_t_4 = __pyx_temp; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_4);
+        }
+        __pyx_r = ((PyObject*)__pyx_t_4);
+        __pyx_t_4 = 0;
+        goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":195
- *         elif value_type in (3, 6):
- *             uint8 = data[starting_position+1]
- *             if value_type == 6:             # <<<<<<<<<<<<<<
- *                 return 2, uint8
- *             else:
+        /* "minijson.pyx":185
+ *         elif value_type == 2:
+ *             return 3, *STRUCT_h.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 5:             # <<<<<<<<<<<<<<
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 3:
  */
-        __pyx_t_28 = ((__pyx_v_value_type == 6) != 0);
-        if (__pyx_t_28) {
+      }
 
-          /* "minijson.pyx":196
- *             uint8 = data[starting_position+1]
- *             if value_type == 6:
- *                 return 2, uint8             # <<<<<<<<<<<<<<
- *             else:
- *                 sint8 = uint8
+      /* "minijson.pyx":187
+ *         elif value_type == 5:
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 3:             # <<<<<<<<<<<<<<
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])
+ *         elif value_type == 6:
  */
-          __Pyx_XDECREF(__pyx_r);
-          __pyx_t_12 = __Pyx_PyInt_From_unsigned_char(__pyx_v_uint8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 196, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_INCREF(__pyx_int_2);
-          __Pyx_GIVEREF(__pyx_int_2);
-          PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_2);
-          __Pyx_GIVEREF(__pyx_t_12);
-          PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_12);
-          __pyx_t_12 = 0;
-          __pyx_r = ((PyObject*)__pyx_t_4);
-          __pyx_t_4 = 0;
-          goto __pyx_L7_try_return;
+      __pyx_t_6 = ((__pyx_v_value_type == 3) != 0);
+      if (__pyx_t_6) {
 
-          /* "minijson.pyx":195
- *         elif value_type in (3, 6):
- *             uint8 = data[starting_position+1]
- *             if value_type == 6:             # <<<<<<<<<<<<<<
- *                 return 2, uint8
- *             else:
+        /* "minijson.pyx":188
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 3:
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])             # <<<<<<<<<<<<<<
+ *         elif value_type == 6:
+ *             return 2, data[starting_position+1]
  */
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 188, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_INCREF(__pyx_int_2);
+        __Pyx_GIVEREF(__pyx_int_2);
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_2);
+        __pyx_t_4 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_b, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 188, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(__pyx_v_data == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+          __PYX_ERR(0, 188, __pyx_L3_error)
+        }
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 188, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_12);
+          if (likely(__pyx_t_16)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+            __Pyx_INCREF(__pyx_t_16);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
+          }
         }
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 188, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_t_14) < 0) __PYX_ERR(0, 188, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        {
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_4);
+          __pyx_t_4 = __pyx_temp; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_4);
+        }
+        __pyx_r = ((PyObject*)__pyx_t_4);
+        __pyx_t_4 = 0;
+        goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":198
- *                 return 2, uint8
- *             else:
- *                 sint8 = uint8             # <<<<<<<<<<<<<<
- *                 return 2, sint8
+        /* "minijson.pyx":187
+ *         elif value_type == 5:
+ *             return 3, *STRUCT_H.unpack(data[starting_position+1:starting_position+3])
+ *         elif value_type == 3:             # <<<<<<<<<<<<<<
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])
+ *         elif value_type == 6:
+ */
+      }
+
+      /* "minijson.pyx":189
+ *         elif value_type == 3:
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])
+ *         elif value_type == 6:             # <<<<<<<<<<<<<<
+ *             return 2, data[starting_position+1]
  *         elif value_type == 7:
  */
-        /*else*/ {
-          __pyx_v_sint8 = __pyx_v_uint8;
+      __pyx_t_6 = ((__pyx_v_value_type == 6) != 0);
+      if (__pyx_t_6) {
 
-          /* "minijson.pyx":199
- *             else:
- *                 sint8 = uint8
- *                 return 2, sint8             # <<<<<<<<<<<<<<
+        /* "minijson.pyx":190
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])
+ *         elif value_type == 6:
+ *             return 2, data[starting_position+1]             # <<<<<<<<<<<<<<
  *         elif value_type == 7:
  *             elements = data[starting_position+1]
  */
-          __Pyx_XDECREF(__pyx_r);
-          __pyx_t_4 = __Pyx_PyInt_From_char(__pyx_v_sint8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 199, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __Pyx_INCREF(__pyx_int_2);
-          __Pyx_GIVEREF(__pyx_int_2);
-          PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_int_2);
-          __Pyx_GIVEREF(__pyx_t_4);
-          PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_4);
-          __pyx_t_4 = 0;
-          __pyx_r = ((PyObject*)__pyx_t_12);
-          __pyx_t_12 = 0;
-          goto __pyx_L7_try_return;
-        }
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_26 = (__pyx_v_starting_position + 1);
+        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 190, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_INCREF(__pyx_int_2);
+        __Pyx_GIVEREF(__pyx_int_2);
+        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_int_2);
+        __Pyx_GIVEREF(__pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_4);
+        __pyx_t_4 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_14);
+        __pyx_t_14 = 0;
+        goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":193
- *                 sint16 = uint16
- *                 return 3, sint16
- *         elif value_type in (3, 6):             # <<<<<<<<<<<<<<
- *             uint8 = data[starting_position+1]
- *             if value_type == 6:
+        /* "minijson.pyx":189
+ *         elif value_type == 3:
+ *             return 2, *STRUCT_b.unpack(data[starting_position+1:starting_position+2])
+ *         elif value_type == 6:             # <<<<<<<<<<<<<<
+ *             return 2, data[starting_position+1]
+ *         elif value_type == 7:
  */
       }
 
-      /* "minijson.pyx":200
- *                 sint8 = uint8
- *                 return 2, sint8
+      /* "minijson.pyx":191
+ *         elif value_type == 6:
+ *             return 2, data[starting_position+1]
  *         elif value_type == 7:             # <<<<<<<<<<<<<<
  *             elements = data[starting_position+1]
  *             offset, e_list = parse_list(data, elements, starting_position+2)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 7) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 7) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":201
- *                 return 2, sint8
+        /* "minijson.pyx":192
+ *             return 2, data[starting_position+1]
  *         elif value_type == 7:
  *             elements = data[starting_position+1]             # <<<<<<<<<<<<<<
  *             offset, e_list = parse_list(data, elements, starting_position+2)
  *             return offset+2, e_list
  */
         __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 201, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_12); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 192, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_14); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 192, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":202
+        /* "minijson.pyx":193
  *         elif value_type == 7:
  *             elements = data[starting_position+1]
  *             offset, e_list = parse_list(data, elements, starting_position+2)             # <<<<<<<<<<<<<<
  *             return offset+2, e_list
  *         elif value_type == 8:
  */
-        __pyx_t_12 = __pyx_f_8minijson_parse_list(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 202, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        if (likely(__pyx_t_12 != Py_None)) {
-          PyObject* sequence = __pyx_t_12;
+        __pyx_t_14 = __pyx_f_8minijson_parse_list(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 193, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        if (likely(__pyx_t_14 != Py_None)) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 202, __pyx_L3_error)
+            __PYX_ERR(0, 193, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 1); 
+          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_14);
+          __Pyx_INCREF(__pyx_t_12);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_14 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 202, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 193, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 202, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 193, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (!(likely(PyList_CheckExact(__pyx_t_14))||((__pyx_t_14) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_14)->tp_name), 0))) __PYX_ERR(0, 202, __pyx_L3_error)
+        if (!(likely(PyList_CheckExact(__pyx_t_12))||((__pyx_t_12) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_12)->tp_name), 0))) __PYX_ERR(0, 193, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
-        __pyx_v_e_list = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_v_e_list = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
 
-        /* "minijson.pyx":203
+        /* "minijson.pyx":194
  *             elements = data[starting_position+1]
  *             offset, e_list = parse_list(data, elements, starting_position+2)
  *             return offset+2, e_list             # <<<<<<<<<<<<<<
  *         elif value_type == 8:
  *             return 1, None
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = __Pyx_PyInt_From_long((__pyx_v_offset + 2)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 203, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 203, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyInt_From_long((__pyx_v_offset + 2)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 194, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_14);
-        __Pyx_GIVEREF(__pyx_t_12);
-        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_12);
+        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 194, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __Pyx_GIVEREF(__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_14);
         __Pyx_INCREF(__pyx_v_e_list);
         __Pyx_GIVEREF(__pyx_v_e_list);
-        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_v_e_list);
-        __pyx_t_12 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_e_list);
         __pyx_t_14 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":200
- *                 sint8 = uint8
- *                 return 2, sint8
+        /* "minijson.pyx":191
+ *         elif value_type == 6:
+ *             return 2, data[starting_position+1]
  *         elif value_type == 7:             # <<<<<<<<<<<<<<
  *             elements = data[starting_position+1]
  *             offset, e_list = parse_list(data, elements, starting_position+2)
  */
       }
 
-      /* "minijson.pyx":204
+      /* "minijson.pyx":195
  *             offset, e_list = parse_list(data, elements, starting_position+2)
  *             return offset+2, e_list
  *         elif value_type == 8:             # <<<<<<<<<<<<<<
  *             return 1, None
  *         elif value_type == 9:
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 8) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 8) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":205
+        /* "minijson.pyx":196
  *             return offset+2, e_list
  *         elif value_type == 8:
  *             return 1, None             # <<<<<<<<<<<<<<
  *         elif value_type == 9:
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_tuple_);
         __pyx_r = __pyx_tuple_;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":204
+        /* "minijson.pyx":195
  *             offset, e_list = parse_list(data, elements, starting_position+2)
  *             return offset+2, e_list
  *         elif value_type == 8:             # <<<<<<<<<<<<<<
  *             return 1, None
  *         elif value_type == 9:
  */
       }
 
-      /* "minijson.pyx":206
+      /* "minijson.pyx":197
  *         elif value_type == 8:
  *             return 1, None
  *         elif value_type == 9:             # <<<<<<<<<<<<<<
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  *         elif value_type == 10:
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 9) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 9) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":207
+        /* "minijson.pyx":198
  *             return 1, None
  *         elif value_type == 9:
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
  *         elif value_type == 10:
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = PyList_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 207, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 198, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_INCREF(__pyx_int_5);
         __Pyx_GIVEREF(__pyx_int_5);
-        PyList_SET_ITEM(__pyx_t_12, 0, __pyx_int_5);
-        __pyx_t_14 = __pyx_t_12;
-        __pyx_t_12 = 0;
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_f, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L3_error)
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_5);
+        __pyx_t_12 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_f, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 207, __pyx_L3_error)
+          __PYX_ERR(0, 198, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 207, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 198, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_16 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_16)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_16);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_12 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
         __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 207, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 198, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (__Pyx_PyList_Extend(__pyx_t_14, __pyx_t_12) < 0) __PYX_ERR(0, 207, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (__Pyx_PyList_Extend(__pyx_t_12, __pyx_t_14) < 0) __PYX_ERR(0, 198, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         {
-          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_14);
-          __Pyx_DECREF(__pyx_t_14);
-          __pyx_t_14 = __pyx_temp; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 207, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_12);
+          __pyx_t_12 = __pyx_temp; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 198, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
         }
-        __pyx_r = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":206
+        /* "minijson.pyx":197
  *         elif value_type == 8:
  *             return 1, None
  *         elif value_type == 9:             # <<<<<<<<<<<<<<
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  *         elif value_type == 10:
  */
       }
 
-      /* "minijson.pyx":208
+      /* "minijson.pyx":199
  *         elif value_type == 9:
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  *         elif value_type == 10:             # <<<<<<<<<<<<<<
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])
  *         elif value_type == 12:
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 10) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 10) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":209
+        /* "minijson.pyx":200
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  *         elif value_type == 10:
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])             # <<<<<<<<<<<<<<
  *         elif value_type == 12:
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = PyList_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 209, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = PyList_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 200, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_INCREF(__pyx_int_9);
         __Pyx_GIVEREF(__pyx_int_9);
-        PyList_SET_ITEM(__pyx_t_12, 0, __pyx_int_9);
-        __pyx_t_14 = __pyx_t_12;
-        __pyx_t_12 = 0;
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_d, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L3_error)
+        PyList_SET_ITEM(__pyx_t_14, 0, __pyx_int_9);
+        __pyx_t_12 = __pyx_t_14;
+        __pyx_t_14 = 0;
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_d, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 209, __pyx_L3_error)
+          __PYX_ERR(0, 200, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 9)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 209, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 9)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 200, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_16 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_16)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_16);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_12 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+        __pyx_t_14 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
         __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 209, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 200, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (__Pyx_PyList_Extend(__pyx_t_14, __pyx_t_12) < 0) __PYX_ERR(0, 209, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (__Pyx_PyList_Extend(__pyx_t_12, __pyx_t_14) < 0) __PYX_ERR(0, 200, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         {
-          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_14);
-          __Pyx_DECREF(__pyx_t_14);
-          __pyx_t_14 = __pyx_temp; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 209, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_12);
+          __pyx_t_12 = __pyx_temp; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 200, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
         }
-        __pyx_r = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":208
+        /* "minijson.pyx":199
  *         elif value_type == 9:
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  *         elif value_type == 10:             # <<<<<<<<<<<<<<
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])
  *         elif value_type == 12:
  */
       }
 
-      /* "minijson.pyx":210
+      /* "minijson.pyx":201
  *         elif value_type == 10:
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])
  *         elif value_type == 12:             # <<<<<<<<<<<<<<
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]
  *             return 4, uint32
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 12) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 12) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":211
+        /* "minijson.pyx":202
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])
  *         elif value_type == 12:
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]             # <<<<<<<<<<<<<<
  *             return 4, uint32
  *         elif value_type == 11:
  */
         __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 211, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_12 = __Pyx_PyInt_LshiftObjC(__pyx_t_14, __pyx_int_16, 16, 0, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 211, __pyx_L3_error)
+        __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 202, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_t_26 = (__pyx_v_starting_position + 2);
-        __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 211, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_4 = __Pyx_PyInt_LshiftObjC(__pyx_t_14, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_t_14 = PyNumber_Or(__pyx_t_12, __pyx_t_4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 211, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyInt_LshiftObjC(__pyx_t_12, __pyx_int_16, 16, 0, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 202, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_26 = (__pyx_v_starting_position + 3);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L3_error)
+        __pyx_t_26 = (__pyx_v_starting_position + 2);
+        __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 202, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_4 = __Pyx_PyInt_LshiftObjC(__pyx_t_12, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_12 = PyNumber_Or(__pyx_t_14, __pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 211, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_t_12 = PyNumber_Or(__pyx_t_14, __pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 202, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_29 = __Pyx_PyInt_As_unsigned_int(__pyx_t_12); if (unlikely((__pyx_t_29 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L3_error)
+        __pyx_t_26 = (__pyx_v_starting_position + 3);
+        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_14 = PyNumber_Or(__pyx_t_12, __pyx_t_4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 202, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_v_uint32 = __pyx_t_29;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_28 = __Pyx_PyInt_As_unsigned_int(__pyx_t_14); if (unlikely((__pyx_t_28 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __pyx_v_uint32 = __pyx_t_28;
 
-        /* "minijson.pyx":212
+        /* "minijson.pyx":203
  *         elif value_type == 12:
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]
  *             return 4, uint32             # <<<<<<<<<<<<<<
  *         elif value_type == 11:
  *             elements = data[starting_position+1]
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = __Pyx_PyInt_From_unsigned_int(__pyx_v_uint32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 212, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyInt_From_unsigned_int(__pyx_v_uint32); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 203, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 203, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_int_4);
         __Pyx_GIVEREF(__pyx_int_4);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_4);
-        __Pyx_GIVEREF(__pyx_t_12);
-        PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_12);
-        __pyx_t_12 = 0;
+        __Pyx_GIVEREF(__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_14);
+        __pyx_t_14 = 0;
         __pyx_r = ((PyObject*)__pyx_t_4);
         __pyx_t_4 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":210
+        /* "minijson.pyx":201
  *         elif value_type == 10:
  *             return 9, *STRUCT_d.unpack(data[starting_position+1:starting_position+9])
  *         elif value_type == 12:             # <<<<<<<<<<<<<<
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]
  *             return 4, uint32
  */
       }
 
-      /* "minijson.pyx":213
+      /* "minijson.pyx":204
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]
  *             return 4, uint32
  *         elif value_type == 11:             # <<<<<<<<<<<<<<
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 11) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 11) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":214
+        /* "minijson.pyx":205
  *             return 4, uint32
  *         elif value_type == 11:
  *             elements = data[starting_position+1]             # <<<<<<<<<<<<<<
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)
  *             return offset+2, e_dict
  */
         __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 205, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":215
+        /* "minijson.pyx":206
  *         elif value_type == 11:
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)             # <<<<<<<<<<<<<<
  *             return offset+2, e_dict
  *         elif value_type == 13:
  */
-        __pyx_t_4 = __pyx_f_8minijson_parse_dict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L3_error)
+        __pyx_t_4 = __pyx_f_8minijson_parse_dict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (likely(__pyx_t_4 != Py_None)) {
           PyObject* sequence = __pyx_t_4;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 215, __pyx_L3_error)
+            __PYX_ERR(0, 206, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 1); 
-          __Pyx_INCREF(__pyx_t_12);
+          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 0); 
+          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_14);
+          __Pyx_INCREF(__pyx_t_12);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 215, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_14 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 215, __pyx_L3_error)
+          __pyx_t_14 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 206, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 206, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
           #endif
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 215, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 206, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_12); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (!(likely(PyDict_CheckExact(__pyx_t_14))||((__pyx_t_14) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_14)->tp_name), 0))) __PYX_ERR(0, 215, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_14); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        if (!(likely(PyDict_CheckExact(__pyx_t_12))||((__pyx_t_12) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_12)->tp_name), 0))) __PYX_ERR(0, 206, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
-        __pyx_v_e_dict = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_v_e_dict = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
 
-        /* "minijson.pyx":216
+        /* "minijson.pyx":207
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)
  *             return offset+2, e_dict             # <<<<<<<<<<<<<<
  *         elif value_type == 13:
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_offset + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_offset + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 216, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 207, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_4);
         __Pyx_INCREF(__pyx_v_e_dict);
         __Pyx_GIVEREF(__pyx_v_e_dict);
-        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_v_e_dict);
+        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_e_dict);
         __pyx_t_4 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":213
+        /* "minijson.pyx":204
  *             uint32 = (data[starting_position+1] << 16) | (data[starting_position+2] << 8) | data[starting_position+3]
  *             return 4, uint32
  *         elif value_type == 11:             # <<<<<<<<<<<<<<
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)
  */
       }
 
-      /* "minijson.pyx":217
+      /* "minijson.pyx":208
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)
  *             return offset+2, e_dict
  *         elif value_type == 13:             # <<<<<<<<<<<<<<
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 13) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 13) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":218
+        /* "minijson.pyx":209
  *             return offset+2, e_dict
  *         elif value_type == 13:
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  *             if len(byte_data) != string_length:
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 218, __pyx_L3_error)
+          __PYX_ERR(0, 209, __pyx_L3_error)
         }
-        __pyx_t_12 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 218, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 209, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __pyx_t_11 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_11)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_11);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_14 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_11, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_12);
+        __pyx_t_12 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_11, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_14);
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 218, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 209, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if ((likely(PyTuple_CheckExact(__pyx_t_14))) || (PyList_CheckExact(__pyx_t_14))) {
-          PyObject* sequence = __pyx_t_14;
+        if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
+          PyObject* sequence = __pyx_t_12;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 218, __pyx_L3_error)
+            __PYX_ERR(0, 209, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_12 = PyObject_GetIter(__pyx_t_14); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 218, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_12)->tp_iternext;
-          index = 0; __pyx_t_4 = __pyx_t_32(__pyx_t_12); if (unlikely(!__pyx_t_4)) goto __pyx_L49_unpacking_failed;
-          __Pyx_GOTREF(__pyx_t_4);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_12), 1) < 0) __PYX_ERR(0, 218, __pyx_L3_error)
-          __pyx_t_32 = NULL;
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          goto __pyx_L50_unpacking_done;
-          __pyx_L49_unpacking_failed:;
+          __pyx_t_14 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 209, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = Py_TYPE(__pyx_t_14)->tp_iternext;
+          index = 0; __pyx_t_4 = __pyx_t_29(__pyx_t_14); if (unlikely(!__pyx_t_4)) goto __pyx_L46_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_4);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_14), 1) < 0) __PYX_ERR(0, 209, __pyx_L3_error)
+          __pyx_t_29 = NULL;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          goto __pyx_L47_unpacking_done;
+          __pyx_L46_unpacking_failed:;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 218, __pyx_L3_error)
-          __pyx_L50_unpacking_done:;
+          __PYX_ERR(0, 209, __pyx_L3_error)
+          __pyx_L47_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 209, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_string_length = __pyx_t_5;
 
-        /* "minijson.pyx":219
+        /* "minijson.pyx":210
  *         elif value_type == 13:
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+string_length+3]             # <<<<<<<<<<<<<<
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  */
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 219, __pyx_L3_error)
+          __PYX_ERR(0, 210, __pyx_L3_error)
         }
-        __pyx_t_14 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 3), ((__pyx_v_starting_position + __pyx_v_string_length) + 3)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 219, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_v_byte_data = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_t_12 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 3), ((__pyx_v_starting_position + __pyx_v_string_length) + 3)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 210, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_v_byte_data = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
 
-        /* "minijson.pyx":220
+        /* "minijson.pyx":211
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  *             if len(byte_data) != string_length:             # <<<<<<<<<<<<<<
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))
  */
-        __pyx_t_10 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L3_error)
-        __pyx_t_28 = ((__pyx_t_10 != __pyx_v_string_length) != 0);
-        if (unlikely(__pyx_t_28)) {
+        __pyx_t_10 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 211, __pyx_L3_error)
+        __pyx_t_6 = ((__pyx_t_10 != __pyx_v_string_length) != 0);
+        if (unlikely(__pyx_t_6)) {
 
-          /* "minijson.pyx":221
+          /* "minijson.pyx":212
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,             # <<<<<<<<<<<<<<
  *                                                                                      len(byte_data)))
  *             return 3+string_length, byte_data.decode('utf-8')
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L3_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_12 = PyTuple_New(4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 221, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PyTuple_New(4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 212, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           __pyx_t_10 = 0;
           __pyx_t_13 = 127;
           __Pyx_INCREF(__pyx_kp_u_Too_short_a_frame_expected);
           __pyx_t_10 += 28;
           __Pyx_GIVEREF(__pyx_kp_u_Too_short_a_frame_expected);
-          PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_kp_u_Too_short_a_frame_expected);
-          __pyx_t_11 = __Pyx_PyUnicode_From_int(__pyx_v_string_length, 0, ' ', 'd'); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 221, __pyx_L3_error)
+          PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_kp_u_Too_short_a_frame_expected);
+          __pyx_t_11 = __Pyx_PyUnicode_From_int(__pyx_v_string_length, 0, ' ', 'd'); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 212, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_11);
-          PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_11);
+          PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_11);
           __pyx_t_11 = 0;
           __Pyx_INCREF(__pyx_kp_u_bytes_got);
           __pyx_t_10 += 11;
           __Pyx_GIVEREF(__pyx_kp_u_bytes_got);
-          PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_u_bytes_got);
+          PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_u_bytes_got);
 
-          /* "minijson.pyx":222
+          /* "minijson.pyx":213
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))             # <<<<<<<<<<<<<<
  *             return 3+string_length, byte_data.decode('utf-8')
  *         elif value_type == 14:
  */
-          __pyx_t_15 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 222, __pyx_L3_error)
-          __pyx_t_11 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_15, 0, ' ', 'd'); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 222, __pyx_L3_error)
+          __pyx_t_15 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 213, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_15, 0, ' ', 'd'); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 213, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_11);
           __Pyx_GIVEREF(__pyx_t_11);
-          PyTuple_SET_ITEM(__pyx_t_12, 3, __pyx_t_11);
+          PyTuple_SET_ITEM(__pyx_t_14, 3, __pyx_t_11);
           __pyx_t_11 = 0;
 
-          /* "minijson.pyx":221
+          /* "minijson.pyx":212
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,             # <<<<<<<<<<<<<<
  *                                                                                      len(byte_data)))
  *             return 3+string_length, byte_data.decode('utf-8')
  */
-          __pyx_t_11 = __Pyx_PyUnicode_Join(__pyx_t_12, 4, __pyx_t_10, __pyx_t_13); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 221, __pyx_L3_error)
+          __pyx_t_11 = __Pyx_PyUnicode_Join(__pyx_t_14, 4, __pyx_t_10, __pyx_t_13); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 212, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_12 = NULL;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __pyx_t_14 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-            __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
-            if (likely(__pyx_t_12)) {
+            __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
+            if (likely(__pyx_t_14)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-              __Pyx_INCREF(__pyx_t_12);
+              __Pyx_INCREF(__pyx_t_14);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_4, function);
             }
           }
-          __pyx_t_14 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
-          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_14, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 221, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 212, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_Raise(__pyx_t_14, 0, 0, 0);
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          __PYX_ERR(0, 221, __pyx_L3_error)
+          __Pyx_Raise(__pyx_t_12, 0, 0, 0);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __PYX_ERR(0, 212, __pyx_L3_error)
 
-          /* "minijson.pyx":220
+          /* "minijson.pyx":211
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  *             if len(byte_data) != string_length:             # <<<<<<<<<<<<<<
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))
  */
         }
 
-        /* "minijson.pyx":223
+        /* "minijson.pyx":214
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))
  *             return 3+string_length, byte_data.decode('utf-8')             # <<<<<<<<<<<<<<
  *         elif value_type == 14:
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_14 = __Pyx_PyInt_From_long((3 + __pyx_v_string_length)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 223, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_4 = __Pyx_decode_bytes(__pyx_v_byte_data, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __pyx_t_12 = __Pyx_PyInt_From_long((3 + __pyx_v_string_length)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 214, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_4 = __Pyx_decode_bytes(__pyx_v_byte_data, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 214, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_GIVEREF(__pyx_t_14);
-        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_14);
+        __Pyx_GIVEREF(__pyx_t_12);
+        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
-        __pyx_t_14 = 0;
+        __pyx_t_12 = 0;
         __pyx_t_4 = 0;
         __pyx_r = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":217
+        /* "minijson.pyx":208
  *             offset, e_dict = parse_dict(data, elements, starting_position+2)
  *             return offset+2, e_dict
  *         elif value_type == 13:             # <<<<<<<<<<<<<<
  *             string_length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+string_length+3]
  */
       }
 
-      /* "minijson.pyx":224
+      /* "minijson.pyx":215
  *                                                                                      len(byte_data)))
  *             return 3+string_length, byte_data.decode('utf-8')
  *         elif value_type == 14:             # <<<<<<<<<<<<<<
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 14) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 14) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":225
+        /* "minijson.pyx":216
  *             return 3+string_length, byte_data.decode('utf-8')
  *         elif value_type == 14:
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  *             if len(byte_data) != string_length:
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 225, __pyx_L3_error)
+          __PYX_ERR(0, 216, __pyx_L3_error)
         }
-        __pyx_t_14 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 225, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_12 = NULL;
+        __pyx_t_12 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 216, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
-          if (likely(__pyx_t_12)) {
+          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
+          if (likely(__pyx_t_14)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-            __Pyx_INCREF(__pyx_t_12);
+            __Pyx_INCREF(__pyx_t_14);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_14);
-        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 225, __pyx_L3_error)
+        __pyx_t_11 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_14, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_12);
+        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 216, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_11))) || (PyList_CheckExact(__pyx_t_11))) {
           PyObject* sequence = __pyx_t_11;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 225, __pyx_L3_error)
+            __PYX_ERR(0, 216, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_14 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 225, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_12 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 216, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_14)->tp_iternext;
-          index = 0; __pyx_t_4 = __pyx_t_32(__pyx_t_14); if (unlikely(!__pyx_t_4)) goto __pyx_L52_unpacking_failed;
+          __pyx_t_29 = Py_TYPE(__pyx_t_12)->tp_iternext;
+          index = 0; __pyx_t_4 = __pyx_t_29(__pyx_t_12); if (unlikely(!__pyx_t_4)) goto __pyx_L49_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_14), 1) < 0) __PYX_ERR(0, 225, __pyx_L3_error)
-          __pyx_t_32 = NULL;
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          goto __pyx_L53_unpacking_done;
-          __pyx_L52_unpacking_failed:;
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          __pyx_t_32 = NULL;
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_12), 1) < 0) __PYX_ERR(0, 216, __pyx_L3_error)
+          __pyx_t_29 = NULL;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          goto __pyx_L50_unpacking_done;
+          __pyx_L49_unpacking_failed:;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 225, __pyx_L3_error)
-          __pyx_L53_unpacking_done:;
+          __PYX_ERR(0, 216, __pyx_L3_error)
+          __pyx_L50_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_string_length = __pyx_t_5;
 
-        /* "minijson.pyx":226
+        /* "minijson.pyx":217
  *         elif value_type == 14:
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+string_length+5]             # <<<<<<<<<<<<<<
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  */
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 226, __pyx_L3_error)
+          __PYX_ERR(0, 217, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 5), ((__pyx_v_starting_position + __pyx_v_string_length) + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 226, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 5), ((__pyx_v_starting_position + __pyx_v_string_length) + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 217, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_v_byte_data = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
 
-        /* "minijson.pyx":227
+        /* "minijson.pyx":218
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  *             if len(byte_data) != string_length:             # <<<<<<<<<<<<<<
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))
  */
-        __pyx_t_10 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 227, __pyx_L3_error)
-        __pyx_t_28 = ((__pyx_t_10 != __pyx_v_string_length) != 0);
-        if (unlikely(__pyx_t_28)) {
+        __pyx_t_10 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 218, __pyx_L3_error)
+        __pyx_t_6 = ((__pyx_t_10 != __pyx_v_string_length) != 0);
+        if (unlikely(__pyx_t_6)) {
 
-          /* "minijson.pyx":228
+          /* "minijson.pyx":219
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,             # <<<<<<<<<<<<<<
  *                                                                                      len(byte_data)))
  *             return 5+string_length, byte_data.decode('utf-8')
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L3_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_14 = PyTuple_New(4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 228, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_12 = PyTuple_New(4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 219, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
           __pyx_t_10 = 0;
           __pyx_t_13 = 127;
           __Pyx_INCREF(__pyx_kp_u_Too_short_a_frame_expected);
           __pyx_t_10 += 28;
           __Pyx_GIVEREF(__pyx_kp_u_Too_short_a_frame_expected);
-          PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_kp_u_Too_short_a_frame_expected);
-          __pyx_t_12 = __Pyx_PyUnicode_From_int(__pyx_v_string_length, 0, ' ', 'd'); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 228, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_12);
-          __Pyx_GIVEREF(__pyx_t_12);
-          PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_12);
-          __pyx_t_12 = 0;
+          PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_kp_u_Too_short_a_frame_expected);
+          __pyx_t_14 = __Pyx_PyUnicode_From_int(__pyx_v_string_length, 0, ' ', 'd'); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 219, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_14);
+          __Pyx_GIVEREF(__pyx_t_14);
+          PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_14);
+          __pyx_t_14 = 0;
           __Pyx_INCREF(__pyx_kp_u_bytes_got);
           __pyx_t_10 += 11;
           __Pyx_GIVEREF(__pyx_kp_u_bytes_got);
-          PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_u_bytes_got);
+          PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_u_bytes_got);
 
-          /* "minijson.pyx":229
+          /* "minijson.pyx":220
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))             # <<<<<<<<<<<<<<
  *             return 5+string_length, byte_data.decode('utf-8')
  *         elif value_type == 15:
  */
-          __pyx_t_15 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 229, __pyx_L3_error)
-          __pyx_t_12 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_15, 0, ' ', 'd'); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 229, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_12);
-          __Pyx_GIVEREF(__pyx_t_12);
-          PyTuple_SET_ITEM(__pyx_t_14, 3, __pyx_t_12);
-          __pyx_t_12 = 0;
+          __pyx_t_15 = PyBytes_GET_SIZE(__pyx_v_byte_data); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L3_error)
+          __pyx_t_14 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_15, 0, ' ', 'd'); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 220, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_14);
+          __Pyx_GIVEREF(__pyx_t_14);
+          PyTuple_SET_ITEM(__pyx_t_12, 3, __pyx_t_14);
+          __pyx_t_14 = 0;
 
-          /* "minijson.pyx":228
+          /* "minijson.pyx":219
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  *             if len(byte_data) != string_length:
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,             # <<<<<<<<<<<<<<
  *                                                                                      len(byte_data)))
  *             return 5+string_length, byte_data.decode('utf-8')
  */
-          __pyx_t_12 = __Pyx_PyUnicode_Join(__pyx_t_14, 4, __pyx_t_10, __pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 228, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          __pyx_t_14 = NULL;
+          __pyx_t_14 = __Pyx_PyUnicode_Join(__pyx_t_12, 4, __pyx_t_10, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 219, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_12 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-            __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
-            if (likely(__pyx_t_14)) {
+            __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
+            if (likely(__pyx_t_12)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-              __Pyx_INCREF(__pyx_t_14);
+              __Pyx_INCREF(__pyx_t_12);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_4, function);
             }
           }
-          __pyx_t_11 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_14, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_12);
-          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 228, __pyx_L3_error)
+          __pyx_t_11 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_14);
+          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 219, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_Raise(__pyx_t_11, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __PYX_ERR(0, 228, __pyx_L3_error)
+          __PYX_ERR(0, 219, __pyx_L3_error)
 
-          /* "minijson.pyx":227
+          /* "minijson.pyx":218
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  *             if len(byte_data) != string_length:             # <<<<<<<<<<<<<<
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))
  */
         }
 
-        /* "minijson.pyx":230
+        /* "minijson.pyx":221
  *                 raise DecodingError('Too short a frame, expected %s bytes got %s' % (string_length,
  *                                                                                      len(byte_data)))
  *             return 5+string_length, byte_data.decode('utf-8')             # <<<<<<<<<<<<<<
  *         elif value_type == 15:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyInt_From_long((5 + __pyx_v_string_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 230, __pyx_L3_error)
+        __pyx_t_11 = __Pyx_PyInt_From_long((5 + __pyx_v_string_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 221, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_4 = __Pyx_decode_bytes(__pyx_v_byte_data, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_decode_bytes(__pyx_v_byte_data, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 230, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 221, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_11);
-        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11);
+        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_11);
         __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_4);
         __pyx_t_11 = 0;
         __pyx_t_4 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_12);
-        __pyx_t_12 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_14);
+        __pyx_t_14 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":224
+        /* "minijson.pyx":215
  *                                                                                      len(byte_data)))
  *             return 3+string_length, byte_data.decode('utf-8')
  *         elif value_type == 14:             # <<<<<<<<<<<<<<
  *             string_length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+string_length+5]
  */
       }
 
-      /* "minijson.pyx":231
+      /* "minijson.pyx":222
  *                                                                                      len(byte_data)))
  *             return 5+string_length, byte_data.decode('utf-8')
  *         elif value_type == 15:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_list = parse_list(data, elements, starting_position+3)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 15) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 15) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":232
+        /* "minijson.pyx":223
  *             return 5+string_length, byte_data.decode('utf-8')
  *         elif value_type == 15:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
  *             offset, e_list = parse_list(data, elements, starting_position+3)
  *             return 3+offset, e_list
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 232, __pyx_L3_error)
+          __PYX_ERR(0, 223, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 232, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 223, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_14 = NULL;
+        __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
-          if (likely(__pyx_t_14)) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
+          if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-            __Pyx_INCREF(__pyx_t_14);
+            __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_14, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __pyx_t_14 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 232, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 223, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
-          PyObject* sequence = __pyx_t_12;
+        if ((likely(PyTuple_CheckExact(__pyx_t_14))) || (PyList_CheckExact(__pyx_t_14))) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 232, __pyx_L3_error)
+            __PYX_ERR(0, 223, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_11 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 232, __pyx_L3_error)
+          __pyx_t_11 = PyObject_GetIter(__pyx_t_14); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 223, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_11)->tp_iternext;
-          index = 0; __pyx_t_4 = __pyx_t_32(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L55_unpacking_failed;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __pyx_t_29 = Py_TYPE(__pyx_t_11)->tp_iternext;
+          index = 0; __pyx_t_4 = __pyx_t_29(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L52_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_11), 1) < 0) __PYX_ERR(0, 232, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_11), 1) < 0) __PYX_ERR(0, 223, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          goto __pyx_L56_unpacking_done;
-          __pyx_L55_unpacking_failed:;
+          goto __pyx_L53_unpacking_done;
+          __pyx_L52_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 232, __pyx_L3_error)
-          __pyx_L56_unpacking_done:;
+          __PYX_ERR(0, 223, __pyx_L3_error)
+          __pyx_L53_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 232, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 223, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":233
+        /* "minijson.pyx":224
  *         elif value_type == 15:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_list = parse_list(data, elements, starting_position+3)             # <<<<<<<<<<<<<<
  *             return 3+offset, e_list
  *         elif value_type == 16:
  */
-        __pyx_t_12 = __pyx_f_8minijson_parse_list(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 233, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        if (likely(__pyx_t_12 != Py_None)) {
-          PyObject* sequence = __pyx_t_12;
+        __pyx_t_14 = __pyx_f_8minijson_parse_list(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 224, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        if (likely(__pyx_t_14 != Py_None)) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 233, __pyx_L3_error)
+            __PYX_ERR(0, 224, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_11);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 233, __pyx_L3_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 224, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 233, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 224, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (!(likely(PyList_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 233, __pyx_L3_error)
+        if (!(likely(PyList_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 224, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
         __pyx_v_e_list = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
 
-        /* "minijson.pyx":234
+        /* "minijson.pyx":225
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_list = parse_list(data, elements, starting_position+3)
  *             return 3+offset, e_list             # <<<<<<<<<<<<<<
  *         elif value_type == 16:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = __Pyx_PyInt_From_long((3 + __pyx_v_offset)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 234, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 234, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyInt_From_long((3 + __pyx_v_offset)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 225, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 225, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_GIVEREF(__pyx_t_12);
-        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_12);
+        __Pyx_GIVEREF(__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_14);
         __Pyx_INCREF(__pyx_v_e_list);
         __Pyx_GIVEREF(__pyx_v_e_list);
         PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_e_list);
-        __pyx_t_12 = 0;
+        __pyx_t_14 = 0;
         __pyx_r = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":231
+        /* "minijson.pyx":222
  *                                                                                      len(byte_data)))
  *             return 5+string_length, byte_data.decode('utf-8')
  *         elif value_type == 15:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_list = parse_list(data, elements, starting_position+3)
  */
       }
 
-      /* "minijson.pyx":235
+      /* "minijson.pyx":226
  *             offset, e_list = parse_list(data, elements, starting_position+3)
  *             return 3+offset, e_list
  *         elif value_type == 16:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_list = parse_list(data, elements, starting_position+5)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 16) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 16) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":236
+        /* "minijson.pyx":227
  *             return 3+offset, e_list
  *         elif value_type == 16:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
  *             offset, e_list = parse_list(data, elements, starting_position+5)
  *             return 5+offset, e_list
  */
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 236, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 227, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 236, __pyx_L3_error)
+          __PYX_ERR(0, 227, __pyx_L3_error)
         }
-        __pyx_t_4 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L3_error)
+        __pyx_t_4 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_14 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_12);
-          if (likely(__pyx_t_14)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-            __Pyx_INCREF(__pyx_t_14);
+        __pyx_t_12 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_14);
+          if (likely(__pyx_t_12)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+            __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_12, function);
+            __Pyx_DECREF_SET(__pyx_t_14, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_14, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_4);
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __pyx_t_11 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_12, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 236, __pyx_L3_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 227, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_11))) || (PyList_CheckExact(__pyx_t_11))) {
           PyObject* sequence = __pyx_t_11;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 236, __pyx_L3_error)
+            __PYX_ERR(0, 227, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
-            __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_14 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
-            __pyx_t_12 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_14 = PyList_GET_ITEM(sequence, 0); 
           }
-          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(__pyx_t_14);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 236, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 227, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           #endif
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_4 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L3_error)
+          __pyx_t_4 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_4)->tp_iternext;
-          index = 0; __pyx_t_12 = __pyx_t_32(__pyx_t_4); if (unlikely(!__pyx_t_12)) goto __pyx_L57_unpacking_failed;
-          __Pyx_GOTREF(__pyx_t_12);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_4), 1) < 0) __PYX_ERR(0, 236, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = Py_TYPE(__pyx_t_4)->tp_iternext;
+          index = 0; __pyx_t_14 = __pyx_t_29(__pyx_t_4); if (unlikely(!__pyx_t_14)) goto __pyx_L54_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_14);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_4), 1) < 0) __PYX_ERR(0, 227, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          goto __pyx_L58_unpacking_done;
-          __pyx_L57_unpacking_failed:;
+          goto __pyx_L55_unpacking_done;
+          __pyx_L54_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 236, __pyx_L3_error)
-          __pyx_L58_unpacking_done:;
+          __PYX_ERR(0, 227, __pyx_L3_error)
+          __pyx_L55_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_12); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_14); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":237
+        /* "minijson.pyx":228
  *         elif value_type == 16:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_list = parse_list(data, elements, starting_position+5)             # <<<<<<<<<<<<<<
  *             return 5+offset, e_list
  *         elif value_type == 17:
  */
-        __pyx_t_11 = __pyx_f_8minijson_parse_list(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 237, __pyx_L3_error)
+        __pyx_t_11 = __pyx_f_8minijson_parse_list(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 228, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         if (likely(__pyx_t_11 != Py_None)) {
           PyObject* sequence = __pyx_t_11;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 237, __pyx_L3_error)
+            __PYX_ERR(0, 228, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
+          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 237, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L3_error)
+          __pyx_t_14 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 228, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 237, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 228, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_12); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (!(likely(PyList_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 237, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_14); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        if (!(likely(PyList_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 228, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
         __pyx_v_e_list = ((PyObject*)__pyx_t_4);
         __pyx_t_4 = 0;
 
-        /* "minijson.pyx":238
+        /* "minijson.pyx":229
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_list = parse_list(data, elements, starting_position+5)
  *             return 5+offset, e_list             # <<<<<<<<<<<<<<
  *         elif value_type == 17:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyInt_From_long((5 + __pyx_v_offset)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 238, __pyx_L3_error)
+        __pyx_t_11 = __Pyx_PyInt_From_long((5 + __pyx_v_offset)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 229, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L3_error)
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_11);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_11);
         __Pyx_INCREF(__pyx_v_e_list);
         __Pyx_GIVEREF(__pyx_v_e_list);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_e_list);
         __pyx_t_11 = 0;
         __pyx_r = ((PyObject*)__pyx_t_4);
         __pyx_t_4 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":235
+        /* "minijson.pyx":226
  *             offset, e_list = parse_list(data, elements, starting_position+3)
  *             return 3+offset, e_list
  *         elif value_type == 16:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_list = parse_list(data, elements, starting_position+5)
  */
       }
 
-      /* "minijson.pyx":239
+      /* "minijson.pyx":230
  *             offset, e_list = parse_list(data, elements, starting_position+5)
  *             return 5+offset, e_list
  *         elif value_type == 17:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 17) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 17) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":240
+        /* "minijson.pyx":231
  *             return 5+offset, e_list
  *         elif value_type == 17:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)
  *             return offset+3, e_dict
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 240, __pyx_L3_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 231, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 240, __pyx_L3_error)
+          __PYX_ERR(0, 231, __pyx_L3_error)
         }
-        __pyx_t_12 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 240, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_14 = NULL;
+        __pyx_t_14 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 231, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
-          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_11);
-          if (likely(__pyx_t_14)) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+          if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-            __Pyx_INCREF(__pyx_t_14);
+            __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
-        __pyx_t_4 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_14, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_12);
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L3_error)
+        __pyx_t_4 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_14);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
           PyObject* sequence = __pyx_t_4;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 240, __pyx_L3_error)
+            __PYX_ERR(0, 231, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_11 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_11 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_11);
           #else
-          __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 240, __pyx_L3_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 231, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_12 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 240, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 231, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_12)->tp_iternext;
-          index = 0; __pyx_t_11 = __pyx_t_32(__pyx_t_12); if (unlikely(!__pyx_t_11)) goto __pyx_L59_unpacking_failed;
+          __pyx_t_29 = Py_TYPE(__pyx_t_14)->tp_iternext;
+          index = 0; __pyx_t_11 = __pyx_t_29(__pyx_t_14); if (unlikely(!__pyx_t_11)) goto __pyx_L56_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_11);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_12), 1) < 0) __PYX_ERR(0, 240, __pyx_L3_error)
-          __pyx_t_32 = NULL;
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          goto __pyx_L60_unpacking_done;
-          __pyx_L59_unpacking_failed:;
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_32 = NULL;
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_14), 1) < 0) __PYX_ERR(0, 231, __pyx_L3_error)
+          __pyx_t_29 = NULL;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          goto __pyx_L57_unpacking_done;
+          __pyx_L56_unpacking_failed:;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 240, __pyx_L3_error)
-          __pyx_L60_unpacking_done:;
+          __PYX_ERR(0, 231, __pyx_L3_error)
+          __pyx_L57_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_11); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 240, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_11); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 231, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":241
+        /* "minijson.pyx":232
  *         elif value_type == 17:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)             # <<<<<<<<<<<<<<
  *             return offset+3, e_dict
  *         elif value_type == 18:
  */
-        __pyx_t_4 = __pyx_f_8minijson_parse_dict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L3_error)
+        __pyx_t_4 = __pyx_f_8minijson_parse_dict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (likely(__pyx_t_4 != Py_None)) {
           PyObject* sequence = __pyx_t_4;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 241, __pyx_L3_error)
+            __PYX_ERR(0, 232, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 1); 
+          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_11);
-          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(__pyx_t_14);
           #else
-          __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 241, __pyx_L3_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 232, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 241, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 232, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           #endif
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 241, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 232, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_11); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_11); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 232, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (!(likely(PyDict_CheckExact(__pyx_t_12))||((__pyx_t_12) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_12)->tp_name), 0))) __PYX_ERR(0, 241, __pyx_L3_error)
+        if (!(likely(PyDict_CheckExact(__pyx_t_14))||((__pyx_t_14) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_14)->tp_name), 0))) __PYX_ERR(0, 232, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
-        __pyx_v_e_dict = ((PyObject*)__pyx_t_12);
-        __pyx_t_12 = 0;
+        __pyx_v_e_dict = ((PyObject*)__pyx_t_14);
+        __pyx_t_14 = 0;
 
-        /* "minijson.pyx":242
+        /* "minijson.pyx":233
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)
  *             return offset+3, e_dict             # <<<<<<<<<<<<<<
  *         elif value_type == 18:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_offset + 3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_offset + 3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 242, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 233, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_4);
         __Pyx_INCREF(__pyx_v_e_dict);
         __Pyx_GIVEREF(__pyx_v_e_dict);
-        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_e_dict);
+        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_v_e_dict);
         __pyx_t_4 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_12);
-        __pyx_t_12 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_14);
+        __pyx_t_14 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":239
+        /* "minijson.pyx":230
  *             offset, e_list = parse_list(data, elements, starting_position+5)
  *             return 5+offset, e_list
  *         elif value_type == 17:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)
  */
       }
 
-      /* "minijson.pyx":243
+      /* "minijson.pyx":234
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)
  *             return offset+3, e_dict
  *         elif value_type == 18:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 18) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 18) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":244
+        /* "minijson.pyx":235
  *             return offset+3, e_dict
  *         elif value_type == 18:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)
  *             return offset+5, e_dict
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 244, __pyx_L3_error)
+          __PYX_ERR(0, 235, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 244, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 235, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_14 = NULL;
+        __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
-          if (likely(__pyx_t_14)) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
+          if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-            __Pyx_INCREF(__pyx_t_14);
+            __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_14, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __pyx_t_14 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 244, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 235, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
-          PyObject* sequence = __pyx_t_12;
+        if ((likely(PyTuple_CheckExact(__pyx_t_14))) || (PyList_CheckExact(__pyx_t_14))) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 244, __pyx_L3_error)
+            __PYX_ERR(0, 235, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_11 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 244, __pyx_L3_error)
+          __pyx_t_11 = PyObject_GetIter(__pyx_t_14); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 235, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_11)->tp_iternext;
-          index = 0; __pyx_t_4 = __pyx_t_32(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L61_unpacking_failed;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __pyx_t_29 = Py_TYPE(__pyx_t_11)->tp_iternext;
+          index = 0; __pyx_t_4 = __pyx_t_29(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L58_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_11), 1) < 0) __PYX_ERR(0, 244, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_11), 1) < 0) __PYX_ERR(0, 235, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          goto __pyx_L62_unpacking_done;
-          __pyx_L61_unpacking_failed:;
+          goto __pyx_L59_unpacking_done;
+          __pyx_L58_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 244, __pyx_L3_error)
-          __pyx_L62_unpacking_done:;
+          __PYX_ERR(0, 235, __pyx_L3_error)
+          __pyx_L59_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 244, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 235, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":245
+        /* "minijson.pyx":236
  *         elif value_type == 18:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)             # <<<<<<<<<<<<<<
  *             return offset+5, e_dict
  *         elif value_type == 19:
  */
-        __pyx_t_12 = __pyx_f_8minijson_parse_dict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 245, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        if (likely(__pyx_t_12 != Py_None)) {
-          PyObject* sequence = __pyx_t_12;
+        __pyx_t_14 = __pyx_f_8minijson_parse_dict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 236, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        if (likely(__pyx_t_14 != Py_None)) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 245, __pyx_L3_error)
+            __PYX_ERR(0, 236, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_11);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 245, __pyx_L3_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 236, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 245, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 236, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 245, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (!(likely(PyDict_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 245, __pyx_L3_error)
+        if (!(likely(PyDict_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 236, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
         __pyx_v_e_dict = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
 
-        /* "minijson.pyx":246
+        /* "minijson.pyx":237
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)
  *             return offset+5, e_dict             # <<<<<<<<<<<<<<
  *         elif value_type == 19:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = __Pyx_PyInt_From_long((__pyx_v_offset + 5)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 246, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 246, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyInt_From_long((__pyx_v_offset + 5)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 237, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 237, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_GIVEREF(__pyx_t_12);
-        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_12);
+        __Pyx_GIVEREF(__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_14);
         __Pyx_INCREF(__pyx_v_e_dict);
         __Pyx_GIVEREF(__pyx_v_e_dict);
         PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_e_dict);
-        __pyx_t_12 = 0;
+        __pyx_t_14 = 0;
         __pyx_r = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":243
+        /* "minijson.pyx":234
  *             offset, e_dict = parse_dict(data, elements, starting_position+3)
  *             return offset+3, e_dict
  *         elif value_type == 18:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)
  */
       }
 
-      /* "minijson.pyx":247
+      /* "minijson.pyx":238
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)
  *             return offset+5, e_dict
  *         elif value_type == 19:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 19) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 19) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":248
+        /* "minijson.pyx":239
  *             return offset+5, e_dict
  *         elif value_type == 19:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)
  *             return offset+5, e_dict
  */
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 248, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 239, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 248, __pyx_L3_error)
+          __PYX_ERR(0, 239, __pyx_L3_error)
         }
-        __pyx_t_4 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L3_error)
+        __pyx_t_4 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_14 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_12);
-          if (likely(__pyx_t_14)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-            __Pyx_INCREF(__pyx_t_14);
+        __pyx_t_12 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_14);
+          if (likely(__pyx_t_12)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+            __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_12, function);
+            __Pyx_DECREF_SET(__pyx_t_14, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_14, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_4);
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __pyx_t_11 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_12, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 248, __pyx_L3_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 239, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_11))) || (PyList_CheckExact(__pyx_t_11))) {
           PyObject* sequence = __pyx_t_11;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 248, __pyx_L3_error)
+            __PYX_ERR(0, 239, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
-            __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_14 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
-            __pyx_t_12 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_14 = PyList_GET_ITEM(sequence, 0); 
           }
-          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(__pyx_t_14);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 248, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 239, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           #endif
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_4 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L3_error)
+          __pyx_t_4 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_4)->tp_iternext;
-          index = 0; __pyx_t_12 = __pyx_t_32(__pyx_t_4); if (unlikely(!__pyx_t_12)) goto __pyx_L63_unpacking_failed;
-          __Pyx_GOTREF(__pyx_t_12);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_4), 1) < 0) __PYX_ERR(0, 248, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = Py_TYPE(__pyx_t_4)->tp_iternext;
+          index = 0; __pyx_t_14 = __pyx_t_29(__pyx_t_4); if (unlikely(!__pyx_t_14)) goto __pyx_L60_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_14);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_4), 1) < 0) __PYX_ERR(0, 239, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          goto __pyx_L64_unpacking_done;
-          __pyx_L63_unpacking_failed:;
+          goto __pyx_L61_unpacking_done;
+          __pyx_L60_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 248, __pyx_L3_error)
-          __pyx_L64_unpacking_done:;
+          __PYX_ERR(0, 239, __pyx_L3_error)
+          __pyx_L61_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_12); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_14); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":249
+        /* "minijson.pyx":240
  *         elif value_type == 19:
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)             # <<<<<<<<<<<<<<
  *             return offset+5, e_dict
  *         elif value_type == 20:
  */
-        __pyx_t_11 = __pyx_f_8minijson_parse_sdict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 249, __pyx_L3_error)
+        __pyx_t_11 = __pyx_f_8minijson_parse_sdict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 240, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         if (likely(__pyx_t_11 != Py_None)) {
           PyObject* sequence = __pyx_t_11;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 249, __pyx_L3_error)
+            __PYX_ERR(0, 240, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
+          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 249, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L3_error)
+          __pyx_t_14 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 240, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 249, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 240, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_12); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 249, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (!(likely(PyDict_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 249, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_14); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 240, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        if (!(likely(PyDict_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 240, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
         __pyx_v_e_dict = ((PyObject*)__pyx_t_4);
         __pyx_t_4 = 0;
 
-        /* "minijson.pyx":250
+        /* "minijson.pyx":241
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)
  *             return offset+5, e_dict             # <<<<<<<<<<<<<<
  *         elif value_type == 20:
  *             elements = data[starting_position+1]
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyInt_From_long((__pyx_v_offset + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 250, __pyx_L3_error)
+        __pyx_t_11 = __Pyx_PyInt_From_long((__pyx_v_offset + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 241, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L3_error)
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 241, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_11);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_11);
         __Pyx_INCREF(__pyx_v_e_dict);
         __Pyx_GIVEREF(__pyx_v_e_dict);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_e_dict);
         __pyx_t_11 = 0;
         __pyx_r = ((PyObject*)__pyx_t_4);
         __pyx_t_4 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":247
+        /* "minijson.pyx":238
  *             offset, e_dict = parse_dict(data, elements, starting_position+5)
  *             return offset+5, e_dict
  *         elif value_type == 19:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)
  */
       }
 
-      /* "minijson.pyx":251
+      /* "minijson.pyx":242
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)
  *             return offset+5, e_dict
  *         elif value_type == 20:             # <<<<<<<<<<<<<<
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 20) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 20) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":252
+        /* "minijson.pyx":243
  *             return offset+5, e_dict
  *         elif value_type == 20:
  *             elements = data[starting_position+1]             # <<<<<<<<<<<<<<
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)
  *             return offset+2, e_dict
  */
         __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 252, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 243, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":253
+        /* "minijson.pyx":244
  *         elif value_type == 20:
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)             # <<<<<<<<<<<<<<
  *             return offset+2, e_dict
  *         elif value_type == 21:
  */
-        __pyx_t_4 = __pyx_f_8minijson_parse_sdict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L3_error)
+        __pyx_t_4 = __pyx_f_8minijson_parse_sdict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (likely(__pyx_t_4 != Py_None)) {
           PyObject* sequence = __pyx_t_4;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 253, __pyx_L3_error)
+            __PYX_ERR(0, 244, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_12 = PyTuple_GET_ITEM(sequence, 1); 
+          __pyx_t_14 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_11);
-          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(__pyx_t_14);
           #else
-          __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 253, __pyx_L3_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 244, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 253, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 244, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_14);
           #endif
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 253, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 244, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_11); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_11); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 244, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (!(likely(PyDict_CheckExact(__pyx_t_12))||((__pyx_t_12) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_12)->tp_name), 0))) __PYX_ERR(0, 253, __pyx_L3_error)
+        if (!(likely(PyDict_CheckExact(__pyx_t_14))||((__pyx_t_14) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_14)->tp_name), 0))) __PYX_ERR(0, 244, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
-        __pyx_v_e_dict = ((PyObject*)__pyx_t_12);
-        __pyx_t_12 = 0;
+        __pyx_v_e_dict = ((PyObject*)__pyx_t_14);
+        __pyx_t_14 = 0;
 
-        /* "minijson.pyx":254
+        /* "minijson.pyx":245
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)
  *             return offset+2, e_dict             # <<<<<<<<<<<<<<
  *         elif value_type == 21:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_offset + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_offset + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 245, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 254, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 245, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_4);
         __Pyx_INCREF(__pyx_v_e_dict);
         __Pyx_GIVEREF(__pyx_v_e_dict);
-        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_e_dict);
+        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_v_e_dict);
         __pyx_t_4 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_12);
-        __pyx_t_12 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_14);
+        __pyx_t_14 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":251
+        /* "minijson.pyx":242
  *             offset, e_dict = parse_sdict(data, elements, starting_position+5)
  *             return offset+5, e_dict
  *         elif value_type == 20:             # <<<<<<<<<<<<<<
  *             elements = data[starting_position+1]
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)
  */
       }
 
-      /* "minijson.pyx":255
+      /* "minijson.pyx":246
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)
  *             return offset+2, e_dict
  *         elif value_type == 21:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 21) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 21) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":256
+        /* "minijson.pyx":247
  *             return offset+2, e_dict
  *         elif value_type == 21:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)
  *             return offset+3, e_dict
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 247, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 256, __pyx_L3_error)
+          __PYX_ERR(0, 247, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 256, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 247, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_14 = NULL;
+        __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-          __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_4);
-          if (likely(__pyx_t_14)) {
+          __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
+          if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-            __Pyx_INCREF(__pyx_t_14);
+            __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_14, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
-        __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __pyx_t_14 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 256, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 247, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
-          PyObject* sequence = __pyx_t_12;
+        if ((likely(PyTuple_CheckExact(__pyx_t_14))) || (PyList_CheckExact(__pyx_t_14))) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 256, __pyx_L3_error)
+            __PYX_ERR(0, 247, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_4);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 247, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_11 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 256, __pyx_L3_error)
+          __pyx_t_11 = PyObject_GetIter(__pyx_t_14); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 247, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_11)->tp_iternext;
-          index = 0; __pyx_t_4 = __pyx_t_32(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L65_unpacking_failed;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __pyx_t_29 = Py_TYPE(__pyx_t_11)->tp_iternext;
+          index = 0; __pyx_t_4 = __pyx_t_29(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L62_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_11), 1) < 0) __PYX_ERR(0, 256, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_11), 1) < 0) __PYX_ERR(0, 247, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          goto __pyx_L66_unpacking_done;
-          __pyx_L65_unpacking_failed:;
+          goto __pyx_L63_unpacking_done;
+          __pyx_L62_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 256, __pyx_L3_error)
-          __pyx_L66_unpacking_done:;
+          __PYX_ERR(0, 247, __pyx_L3_error)
+          __pyx_L63_unpacking_done:;
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 256, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_elements = __pyx_t_5;
 
-        /* "minijson.pyx":257
+        /* "minijson.pyx":248
  *         elif value_type == 21:
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)             # <<<<<<<<<<<<<<
  *             return offset+3, e_dict
  *         elif value_type == 22:
  */
-        __pyx_t_12 = __pyx_f_8minijson_parse_sdict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 257, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        if (likely(__pyx_t_12 != Py_None)) {
-          PyObject* sequence = __pyx_t_12;
+        __pyx_t_14 = __pyx_f_8minijson_parse_sdict(__pyx_v_data, __pyx_v_elements, (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 248, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        if (likely(__pyx_t_14 != Py_None)) {
+          PyObject* sequence = __pyx_t_14;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 257, __pyx_L3_error)
+            __PYX_ERR(0, 248, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_11);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L3_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 257, __pyx_L3_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 248, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else {
-          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 257, __pyx_L3_error)
+          __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 248, __pyx_L3_error)
         }
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (!(likely(PyDict_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 257, __pyx_L3_error)
+        if (!(likely(PyDict_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 248, __pyx_L3_error)
         __pyx_v_offset = __pyx_t_5;
         __pyx_v_e_dict = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
 
-        /* "minijson.pyx":258
+        /* "minijson.pyx":249
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)
  *             return offset+3, e_dict             # <<<<<<<<<<<<<<
  *         elif value_type == 22:
  *             return 1, True
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_12 = __Pyx_PyInt_From_long((__pyx_v_offset + 3)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 258, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 258, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyInt_From_long((__pyx_v_offset + 3)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 249, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 249, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_GIVEREF(__pyx_t_12);
-        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_12);
+        __Pyx_GIVEREF(__pyx_t_14);
+        PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_14);
         __Pyx_INCREF(__pyx_v_e_dict);
         __Pyx_GIVEREF(__pyx_v_e_dict);
         PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_e_dict);
-        __pyx_t_12 = 0;
+        __pyx_t_14 = 0;
         __pyx_r = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":255
+        /* "minijson.pyx":246
  *             offset, e_dict = parse_sdict(data, elements, starting_position+2)
  *             return offset+2, e_dict
  *         elif value_type == 21:             # <<<<<<<<<<<<<<
  *             elements, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)
  */
       }
 
-      /* "minijson.pyx":259
+      /* "minijson.pyx":250
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)
  *             return offset+3, e_dict
  *         elif value_type == 22:             # <<<<<<<<<<<<<<
  *             return 1, True
  *         elif value_type == 23:
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 22) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 22) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":260
+        /* "minijson.pyx":251
  *             return offset+3, e_dict
  *         elif value_type == 22:
  *             return 1, True             # <<<<<<<<<<<<<<
  *         elif value_type == 23:
  *             return 1, False
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_tuple__2);
         __pyx_r = __pyx_tuple__2;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":259
+        /* "minijson.pyx":250
  *             offset, e_dict = parse_sdict(data, elements, starting_position+3)
  *             return offset+3, e_dict
  *         elif value_type == 22:             # <<<<<<<<<<<<<<
  *             return 1, True
  *         elif value_type == 23:
  */
       }
 
-      /* "minijson.pyx":261
+      /* "minijson.pyx":252
  *         elif value_type == 22:
  *             return 1, True
  *         elif value_type == 23:             # <<<<<<<<<<<<<<
  *             return 1, False
  *         elif value_type == 24:
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 23) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 23) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":262
+        /* "minijson.pyx":253
  *             return 1, True
  *         elif value_type == 23:
  *             return 1, False             # <<<<<<<<<<<<<<
  *         elif value_type == 24:
  *             length = data[starting_position+1]
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_tuple__3);
         __pyx_r = __pyx_tuple__3;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":261
+        /* "minijson.pyx":252
  *         elif value_type == 22:
  *             return 1, True
  *         elif value_type == 23:             # <<<<<<<<<<<<<<
  *             return 1, False
  *         elif value_type == 24:
  */
       }
 
-      /* "minijson.pyx":263
+      /* "minijson.pyx":254
  *         elif value_type == 23:
  *             return 1, False
  *         elif value_type == 24:             # <<<<<<<<<<<<<<
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 24) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 24) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":264
+        /* "minijson.pyx":255
  *             return 1, False
  *         elif value_type == 24:
  *             length = data[starting_position+1]             # <<<<<<<<<<<<<<
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, int.from_bytes(byte_data, 'big', signed=True)
  */
         __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_11 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 264, __pyx_L3_error)
+        __pyx_t_11 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 255, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_29 = __Pyx_PyInt_As_unsigned_int(__pyx_t_11); if (unlikely((__pyx_t_29 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 264, __pyx_L3_error)
+        __pyx_t_28 = __Pyx_PyInt_As_unsigned_int(__pyx_t_11); if (unlikely((__pyx_t_28 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __pyx_v_length = __pyx_t_29;
+        __pyx_v_length = __pyx_t_28;
 
-        /* "minijson.pyx":265
+        /* "minijson.pyx":256
  *         elif value_type == 24:
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]             # <<<<<<<<<<<<<<
  *             return length+2, int.from_bytes(byte_data, 'big', signed=True)
  *         elif value_type == 25:
  */
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 265, __pyx_L3_error)
+          __PYX_ERR(0, 256, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 2), ((__pyx_v_starting_position + 2) + __pyx_v_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 265, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 2), ((__pyx_v_starting_position + 2) + __pyx_v_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 256, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_v_byte_data = ((PyObject*)__pyx_t_11);
         __pyx_t_11 = 0;
 
-        /* "minijson.pyx":266
+        /* "minijson.pyx":257
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, int.from_bytes(byte_data, 'big', signed=True)             # <<<<<<<<<<<<<<
  *         elif value_type == 25:
  *             length = data[starting_position+1]
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyInt_From_long((__pyx_v_length + 2)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 266, __pyx_L3_error)
+        __pyx_t_11 = __Pyx_PyInt_From_long((__pyx_v_length + 2)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 257, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 266, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L3_error)
+        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 257, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_v_byte_data);
         __Pyx_GIVEREF(__pyx_v_byte_data);
         PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_byte_data);
         __Pyx_INCREF(__pyx_n_u_big);
         __Pyx_GIVEREF(__pyx_n_u_big);
         PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u_big);
-        __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 266, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_signed, Py_True) < 0) __PYX_ERR(0, 266, __pyx_L3_error)
-        __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_4, __pyx_t_14); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 266, __pyx_L3_error)
+        __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 257, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_signed, Py_True) < 0) __PYX_ERR(0, 257, __pyx_L3_error)
+        __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_4, __pyx_t_12); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 257, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 266, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 257, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_11);
-        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_11);
+        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11);
         __Pyx_GIVEREF(__pyx_t_16);
-        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_16);
+        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_16);
         __pyx_t_11 = 0;
         __pyx_t_16 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":263
+        /* "minijson.pyx":254
  *         elif value_type == 23:
  *             return 1, False
  *         elif value_type == 24:             # <<<<<<<<<<<<<<
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]
  */
       }
 
-      /* "minijson.pyx":267
+      /* "minijson.pyx":258
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, int.from_bytes(byte_data, 'big', signed=True)
  *         elif value_type == 25:             # <<<<<<<<<<<<<<
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 25) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 25) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":268
+        /* "minijson.pyx":259
  *             return length+2, int.from_bytes(byte_data, 'big', signed=True)
  *         elif value_type == 25:
  *             length = data[starting_position+1]             # <<<<<<<<<<<<<<
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, byte_data
  */
         __pyx_t_26 = (__pyx_v_starting_position + 1);
-        __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 268, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_29 = __Pyx_PyInt_As_unsigned_int(__pyx_t_14); if (unlikely((__pyx_t_29 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 268, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_v_length = __pyx_t_29;
+        __pyx_t_12 = __Pyx_GetItemInt(__pyx_v_data, __pyx_t_26, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 259, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_28 = __Pyx_PyInt_As_unsigned_int(__pyx_t_12); if (unlikely((__pyx_t_28 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_v_length = __pyx_t_28;
 
-        /* "minijson.pyx":269
+        /* "minijson.pyx":260
  *         elif value_type == 25:
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]             # <<<<<<<<<<<<<<
  *             return length+2, byte_data
  *         elif value_type == 26:
  */
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 269, __pyx_L3_error)
+          __PYX_ERR(0, 260, __pyx_L3_error)
         }
-        __pyx_t_14 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 2), ((__pyx_v_starting_position + 2) + __pyx_v_length)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 269, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_v_byte_data = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_t_12 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 2), ((__pyx_v_starting_position + 2) + __pyx_v_length)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 260, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_v_byte_data = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
 
-        /* "minijson.pyx":270
+        /* "minijson.pyx":261
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, byte_data             # <<<<<<<<<<<<<<
  *         elif value_type == 26:
  *             length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_14 = __Pyx_PyInt_From_long((__pyx_v_length + 2)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 270, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 270, __pyx_L3_error)
+        __pyx_t_12 = __Pyx_PyInt_From_long((__pyx_v_length + 2)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 261, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 261, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
-        __Pyx_GIVEREF(__pyx_t_14);
-        PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_14);
+        __Pyx_GIVEREF(__pyx_t_12);
+        PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_12);
         __Pyx_INCREF(__pyx_v_byte_data);
         __Pyx_GIVEREF(__pyx_v_byte_data);
         PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_v_byte_data);
-        __pyx_t_14 = 0;
+        __pyx_t_12 = 0;
         __pyx_r = ((PyObject*)__pyx_t_16);
         __pyx_t_16 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":267
+        /* "minijson.pyx":258
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, int.from_bytes(byte_data, 'big', signed=True)
  *         elif value_type == 25:             # <<<<<<<<<<<<<<
  *             length = data[starting_position+1]
  *             byte_data = data[starting_position+2:starting_position+2+length]
  */
       }
 
-      /* "minijson.pyx":271
+      /* "minijson.pyx":262
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, byte_data
  *         elif value_type == 26:             # <<<<<<<<<<<<<<
  *             length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+3+length]
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 26) != 0);
-      if (__pyx_t_28) {
+      __pyx_t_6 = ((__pyx_v_value_type == 26) != 0);
+      if (__pyx_t_6) {
 
-        /* "minijson.pyx":272
+        /* "minijson.pyx":263
  *             return length+2, byte_data
  *         elif value_type == 26:
  *             length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])             # <<<<<<<<<<<<<<
  *             byte_data = data[starting_position+3:starting_position+3+length]
  *             return length+3, byte_data
  */
-        __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 272, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_unpack); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 263, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 272, __pyx_L3_error)
+          __PYX_ERR(0, 263, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 272, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 263, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_4 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_14);
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_12);
           if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_14, function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
           }
         }
-        __pyx_t_16 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_11);
+        __pyx_t_16 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 272, __pyx_L3_error)
+        if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 263, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_16))) || (PyList_CheckExact(__pyx_t_16))) {
           PyObject* sequence = __pyx_t_16;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 272, __pyx_L3_error)
+            __PYX_ERR(0, 263, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
-            __pyx_t_14 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
-            __pyx_t_14 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_12 = PyList_GET_ITEM(sequence, 0); 
           }
-          __Pyx_INCREF(__pyx_t_14);
+          __Pyx_INCREF(__pyx_t_12);
           #else
-          __pyx_t_14 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 272, __pyx_L3_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 263, __pyx_L3_error)
+          __Pyx_GOTREF(__pyx_t_12);
           #endif
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_11 = PyObject_GetIter(__pyx_t_16); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 272, __pyx_L3_error)
+          __pyx_t_11 = PyObject_GetIter(__pyx_t_16); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 263, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_11)->tp_iternext;
-          index = 0; __pyx_t_14 = __pyx_t_32(__pyx_t_11); if (unlikely(!__pyx_t_14)) goto __pyx_L67_unpacking_failed;
-          __Pyx_GOTREF(__pyx_t_14);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_11), 1) < 0) __PYX_ERR(0, 272, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = Py_TYPE(__pyx_t_11)->tp_iternext;
+          index = 0; __pyx_t_12 = __pyx_t_29(__pyx_t_11); if (unlikely(!__pyx_t_12)) goto __pyx_L64_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_12);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_11), 1) < 0) __PYX_ERR(0, 263, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          goto __pyx_L68_unpacking_done;
-          __pyx_L67_unpacking_failed:;
+          goto __pyx_L65_unpacking_done;
+          __pyx_L64_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 272, __pyx_L3_error)
-          __pyx_L68_unpacking_done:;
+          __PYX_ERR(0, 263, __pyx_L3_error)
+          __pyx_L65_unpacking_done:;
         }
-        __pyx_t_29 = __Pyx_PyInt_As_unsigned_int(__pyx_t_14); if (unlikely((__pyx_t_29 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 272, __pyx_L3_error)
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        __pyx_v_length = __pyx_t_29;
+        __pyx_t_28 = __Pyx_PyInt_As_unsigned_int(__pyx_t_12); if (unlikely((__pyx_t_28 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 263, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+        __pyx_v_length = __pyx_t_28;
 
-        /* "minijson.pyx":273
+        /* "minijson.pyx":264
  *         elif value_type == 26:
  *             length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+3+length]             # <<<<<<<<<<<<<<
  *             return length+3, byte_data
  *         elif value_type == 27:
  */
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 273, __pyx_L3_error)
+          __PYX_ERR(0, 264, __pyx_L3_error)
         }
-        __pyx_t_16 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 3), ((__pyx_v_starting_position + 3) + __pyx_v_length)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 273, __pyx_L3_error)
+        __pyx_t_16 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 3), ((__pyx_v_starting_position + 3) + __pyx_v_length)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 264, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_v_byte_data = ((PyObject*)__pyx_t_16);
         __pyx_t_16 = 0;
 
-        /* "minijson.pyx":274
+        /* "minijson.pyx":265
  *             length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+3+length]
  *             return length+3, byte_data             # <<<<<<<<<<<<<<
  *         elif value_type == 27:
  *             length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_16 = __Pyx_PyInt_From_long((__pyx_v_length + 3)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 274, __pyx_L3_error)
+        __pyx_t_16 = __Pyx_PyInt_From_long((__pyx_v_length + 3)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 265, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
-        __pyx_t_14 = PyTuple_New(2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 274, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 265, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_16);
-        PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_16);
+        PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_16);
         __Pyx_INCREF(__pyx_v_byte_data);
         __Pyx_GIVEREF(__pyx_v_byte_data);
-        PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_v_byte_data);
+        PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_byte_data);
         __pyx_t_16 = 0;
-        __pyx_r = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_r = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":271
+        /* "minijson.pyx":262
  *             byte_data = data[starting_position+2:starting_position+2+length]
  *             return length+2, byte_data
  *         elif value_type == 26:             # <<<<<<<<<<<<<<
  *             length, = STRUCT_H.unpack(data[starting_position+1:starting_position+3])
  *             byte_data = data[starting_position+3:starting_position+3+length]
  */
       }
 
-      /* "minijson.pyx":275
+      /* "minijson.pyx":266
  *             byte_data = data[starting_position+3:starting_position+3+length]
  *             return length+3, byte_data
  *         elif value_type == 27:             # <<<<<<<<<<<<<<
  *             length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+5+length]
  */
-      __pyx_t_28 = ((__pyx_v_value_type == 27) != 0);
-      if (likely(__pyx_t_28)) {
+      __pyx_t_6 = ((__pyx_v_value_type == 27) != 0);
+      if (likely(__pyx_t_6)) {
 
-        /* "minijson.pyx":276
+        /* "minijson.pyx":267
  *             return length+3, byte_data
  *         elif value_type == 27:
  *             length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])             # <<<<<<<<<<<<<<
  *             byte_data = data[starting_position+5:starting_position+5+length]
  *             return length+5, byte_data
  */
-        __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 276, __pyx_L3_error)
+        __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_unpack); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 267, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 276, __pyx_L3_error)
+          __PYX_ERR(0, 267, __pyx_L3_error)
         }
-        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 276, __pyx_L3_error)
+        __pyx_t_11 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 1), (__pyx_v_starting_position + 5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 267, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_16))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_16);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_16);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_16, function);
           }
         }
-        __pyx_t_14 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_16, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_16, __pyx_t_11);
+        __pyx_t_12 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_16, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_16, __pyx_t_11);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 276, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
+        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 267, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        if ((likely(PyTuple_CheckExact(__pyx_t_14))) || (PyList_CheckExact(__pyx_t_14))) {
-          PyObject* sequence = __pyx_t_14;
+        if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
+          PyObject* sequence = __pyx_t_12;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 1)) {
             if (size > 1) __Pyx_RaiseTooManyValuesError(1);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 276, __pyx_L3_error)
+            __PYX_ERR(0, 267, __pyx_L3_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_16 = PyTuple_GET_ITEM(sequence, 0); 
           } else {
             __pyx_t_16 = PyList_GET_ITEM(sequence, 0); 
           }
           __Pyx_INCREF(__pyx_t_16);
           #else
-          __pyx_t_16 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 276, __pyx_L3_error)
+          __pyx_t_16 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 267, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_16);
           #endif
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_11 = PyObject_GetIter(__pyx_t_14); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 276, __pyx_L3_error)
+          __pyx_t_11 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 267, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-          __pyx_t_32 = Py_TYPE(__pyx_t_11)->tp_iternext;
-          index = 0; __pyx_t_16 = __pyx_t_32(__pyx_t_11); if (unlikely(!__pyx_t_16)) goto __pyx_L69_unpacking_failed;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_29 = Py_TYPE(__pyx_t_11)->tp_iternext;
+          index = 0; __pyx_t_16 = __pyx_t_29(__pyx_t_11); if (unlikely(!__pyx_t_16)) goto __pyx_L66_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_16);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_32(__pyx_t_11), 1) < 0) __PYX_ERR(0, 276, __pyx_L3_error)
-          __pyx_t_32 = NULL;
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_29(__pyx_t_11), 1) < 0) __PYX_ERR(0, 267, __pyx_L3_error)
+          __pyx_t_29 = NULL;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          goto __pyx_L70_unpacking_done;
-          __pyx_L69_unpacking_failed:;
+          goto __pyx_L67_unpacking_done;
+          __pyx_L66_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_32 = NULL;
+          __pyx_t_29 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 276, __pyx_L3_error)
-          __pyx_L70_unpacking_done:;
+          __PYX_ERR(0, 267, __pyx_L3_error)
+          __pyx_L67_unpacking_done:;
         }
-        __pyx_t_29 = __Pyx_PyInt_As_unsigned_int(__pyx_t_16); if (unlikely((__pyx_t_29 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L3_error)
+        __pyx_t_28 = __Pyx_PyInt_As_unsigned_int(__pyx_t_16); if (unlikely((__pyx_t_28 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 267, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __pyx_v_length = __pyx_t_29;
+        __pyx_v_length = __pyx_t_28;
 
-        /* "minijson.pyx":277
+        /* "minijson.pyx":268
  *         elif value_type == 27:
  *             length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+5+length]             # <<<<<<<<<<<<<<
  *             return length+5, byte_data
  *         else:
  */
         if (unlikely(__pyx_v_data == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 277, __pyx_L3_error)
+          __PYX_ERR(0, 268, __pyx_L3_error)
         }
-        __pyx_t_14 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 5), ((__pyx_v_starting_position + 5) + __pyx_v_length)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 277, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_v_byte_data = ((PyObject*)__pyx_t_14);
-        __pyx_t_14 = 0;
+        __pyx_t_12 = PySequence_GetSlice(__pyx_v_data, (__pyx_v_starting_position + 5), ((__pyx_v_starting_position + 5) + __pyx_v_length)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 268, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_v_byte_data = ((PyObject*)__pyx_t_12);
+        __pyx_t_12 = 0;
 
-        /* "minijson.pyx":278
+        /* "minijson.pyx":269
  *             length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+5+length]
  *             return length+5, byte_data             # <<<<<<<<<<<<<<
  *         else:
  *             raise DecodingError('Unknown sequence type %s!' % (value_type, ))
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_14 = __Pyx_PyInt_From_long((__pyx_v_length + 5)); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 278, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 278, __pyx_L3_error)
+        __pyx_t_12 = __Pyx_PyInt_From_long((__pyx_v_length + 5)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 269, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 269, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
-        __Pyx_GIVEREF(__pyx_t_14);
-        PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_14);
+        __Pyx_GIVEREF(__pyx_t_12);
+        PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_12);
         __Pyx_INCREF(__pyx_v_byte_data);
         __Pyx_GIVEREF(__pyx_v_byte_data);
         PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_v_byte_data);
-        __pyx_t_14 = 0;
+        __pyx_t_12 = 0;
         __pyx_r = ((PyObject*)__pyx_t_16);
         __pyx_t_16 = 0;
         goto __pyx_L7_try_return;
 
-        /* "minijson.pyx":275
+        /* "minijson.pyx":266
  *             byte_data = data[starting_position+3:starting_position+3+length]
  *             return length+3, byte_data
  *         elif value_type == 27:             # <<<<<<<<<<<<<<
  *             length, = STRUCT_L.unpack(data[starting_position+1:starting_position+5])
  *             byte_data = data[starting_position+5:starting_position+5+length]
  */
       }
 
-      /* "minijson.pyx":280
+      /* "minijson.pyx":271
  *             return length+5, byte_data
  *         else:
  *             raise DecodingError('Unknown sequence type %s!' % (value_type, ))             # <<<<<<<<<<<<<<
  *     except (IndexError, struct.error) as e:
  *         raise DecodingError('String too short!') from e
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 280, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_14);
-        __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 280, __pyx_L3_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 271, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 271, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_10 = 0;
         __pyx_t_13 = 127;
         __Pyx_INCREF(__pyx_kp_u_Unknown_sequence_type);
         __pyx_t_10 += 22;
         __Pyx_GIVEREF(__pyx_kp_u_Unknown_sequence_type);
         PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_kp_u_Unknown_sequence_type);
-        __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_value_type, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_value_type, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
         __pyx_t_4 = 0;
         __Pyx_INCREF(__pyx_kp_u__4);
         __pyx_t_10 += 1;
         __Pyx_GIVEREF(__pyx_kp_u__4);
         PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_u__4);
-        __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_11, 3, __pyx_t_10, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_11, 3, __pyx_t_10, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_t_11 = NULL;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
-          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_14);
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_12);
           if (likely(__pyx_t_11)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
             __Pyx_INCREF(__pyx_t_11);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_14, function);
+            __Pyx_DECREF_SET(__pyx_t_12, function);
           }
         }
-        __pyx_t_16 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_4);
+        __pyx_t_16 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 280, __pyx_L3_error)
+        if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 271, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_16);
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_Raise(__pyx_t_16, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __PYX_ERR(0, 280, __pyx_L3_error)
+        __PYX_ERR(0, 271, __pyx_L3_error)
       }
 
       /* "minijson.pyx":146
  *         bytes b_field_name, byte_data
  *         str s_field_name
  *     try:             # <<<<<<<<<<<<<<
  *         value_type = data[starting_position]
@@ -6794,95 +6770,95 @@
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "minijson.pyx":281
+    /* "minijson.pyx":272
  *         else:
  *             raise DecodingError('Unknown sequence type %s!' % (value_type, ))
  *     except (IndexError, struct.error) as e:             # <<<<<<<<<<<<<<
  *         raise DecodingError('String too short!') from e
  * 
  */
-    __Pyx_ErrFetch(&__pyx_t_16, &__pyx_t_14, &__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_struct); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 281, __pyx_L5_except_error)
+    __Pyx_ErrFetch(&__pyx_t_16, &__pyx_t_12, &__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_struct); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 272, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_error); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 281, __pyx_L5_except_error)
-    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_error); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 272, __pyx_L5_except_error)
+    __Pyx_GOTREF(__pyx_t_14);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_5 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_16, __pyx_builtin_IndexError) || __Pyx_PyErr_GivenExceptionMatches(__pyx_t_16, __pyx_t_12);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_ErrRestore(__pyx_t_16, __pyx_t_14, __pyx_t_4);
-    __pyx_t_16 = 0; __pyx_t_14 = 0; __pyx_t_4 = 0;
+    __pyx_t_5 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_16, __pyx_builtin_IndexError) || __Pyx_PyErr_GivenExceptionMatches(__pyx_t_16, __pyx_t_14);
+    __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+    __Pyx_ErrRestore(__pyx_t_16, __pyx_t_12, __pyx_t_4);
+    __pyx_t_16 = 0; __pyx_t_12 = 0; __pyx_t_4 = 0;
     if (__pyx_t_5) {
       __Pyx_AddTraceback("minijson.parse_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_14, &__pyx_t_16) < 0) __PYX_ERR(0, 281, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_12, &__pyx_t_16) < 0) __PYX_ERR(0, 272, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GOTREF(__pyx_t_14);
+      __Pyx_GOTREF(__pyx_t_12);
       __Pyx_GOTREF(__pyx_t_16);
-      __Pyx_INCREF(__pyx_t_14);
-      __Pyx_XDECREF_SET(__pyx_v_e, __pyx_t_14);
+      __Pyx_INCREF(__pyx_t_12);
+      __Pyx_XDECREF_SET(__pyx_v_e, __pyx_t_12);
       /*try:*/ {
 
-        /* "minijson.pyx":282
+        /* "minijson.pyx":273
  *             raise DecodingError('Unknown sequence type %s!' % (value_type, ))
  *     except (IndexError, struct.error) as e:
  *         raise DecodingError('String too short!') from e             # <<<<<<<<<<<<<<
  * 
  * 
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 282, __pyx_L76_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 273, __pyx_L73_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_17 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_17)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_17);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
-        __pyx_t_12 = (__pyx_t_17) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_17, __pyx_kp_u_String_too_short) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_String_too_short);
+        __pyx_t_14 = (__pyx_t_17) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_17, __pyx_kp_u_String_too_short) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_String_too_short);
         __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 282, __pyx_L76_error)
-        __Pyx_GOTREF(__pyx_t_12);
+        if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 273, __pyx_L73_error)
+        __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __Pyx_Raise(__pyx_t_12, 0, 0, __pyx_v_e);
-        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __PYX_ERR(0, 282, __pyx_L76_error)
+        __Pyx_Raise(__pyx_t_14, 0, 0, __pyx_v_e);
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __PYX_ERR(0, 273, __pyx_L73_error)
       }
 
-      /* "minijson.pyx":281
+      /* "minijson.pyx":272
  *         else:
  *             raise DecodingError('Unknown sequence type %s!' % (value_type, ))
  *     except (IndexError, struct.error) as e:             # <<<<<<<<<<<<<<
  *         raise DecodingError('String too short!') from e
  * 
  */
       /*finally:*/ {
-        __pyx_L76_error:;
+        __pyx_L73_error:;
         /*exception exit:*/{
           __Pyx_PyThreadState_declare
           __Pyx_PyThreadState_assign
           __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
           if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_20, &__pyx_t_21, &__pyx_t_22);
           if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9) < 0)) __Pyx_ErrFetch(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
           __Pyx_XGOTREF(__pyx_t_7);
           __Pyx_XGOTREF(__pyx_t_8);
           __Pyx_XGOTREF(__pyx_t_9);
           __Pyx_XGOTREF(__pyx_t_20);
           __Pyx_XGOTREF(__pyx_t_21);
           __Pyx_XGOTREF(__pyx_t_22);
-          __pyx_t_5 = __pyx_lineno; __pyx_t_18 = __pyx_clineno; __pyx_t_33 = __pyx_filename;
+          __pyx_t_5 = __pyx_lineno; __pyx_t_18 = __pyx_clineno; __pyx_t_30 = __pyx_filename;
           {
             __Pyx_DECREF(__pyx_v_e);
             __pyx_v_e = NULL;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_20);
             __Pyx_XGIVEREF(__pyx_t_21);
@@ -6890,15 +6866,15 @@
             __Pyx_ExceptionReset(__pyx_t_20, __pyx_t_21, __pyx_t_22);
           }
           __Pyx_XGIVEREF(__pyx_t_7);
           __Pyx_XGIVEREF(__pyx_t_8);
           __Pyx_XGIVEREF(__pyx_t_9);
           __Pyx_ErrRestore(__pyx_t_7, __pyx_t_8, __pyx_t_9);
           __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0;
-          __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_18; __pyx_filename = __pyx_t_33;
+          __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_18; __pyx_filename = __pyx_t_30;
           goto __pyx_L5_except_error;
         }
       }
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
@@ -6947,15 +6923,15 @@
   __Pyx_XDECREF(__pyx_v_byte_data);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":285
+/* "minijson.pyx":276
  * 
  * 
  * cpdef tuple parse(object data, int starting_position):             # <<<<<<<<<<<<<<
  *     """
  *     Parse given stream of data starting at a position
  */
 
@@ -6966,41 +6942,41 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 0);
 
-  /* "minijson.pyx":297
+  /* "minijson.pyx":288
  *     :raises DecodingError: invalid stream
  *     """
  *     cdef bytes b_data = bytes(data)             # <<<<<<<<<<<<<<
  *     return parse_bytes(b_data, starting_position)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_b_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "minijson.pyx":298
+  /* "minijson.pyx":289
  *     """
  *     cdef bytes b_data = bytes(data)
  *     return parse_bytes(b_data, starting_position)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8minijson_parse_bytes(__pyx_v_b_data, __pyx_v_starting_position); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_parse_bytes(__pyx_v_b_data, __pyx_v_starting_position); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":285
+  /* "minijson.pyx":276
  * 
  * 
  * cpdef tuple parse(object data, int starting_position):             # <<<<<<<<<<<<<<
  *     """
  *     Parse given stream of data starting at a position
  */
 
@@ -7047,32 +7023,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_starting_position)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("parse", 1, 2, 2, 1); __PYX_ERR(0, 285, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("parse", 1, 2, 2, 1); __PYX_ERR(0, 276, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse") < 0)) __PYX_ERR(0, 285, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse") < 0)) __PYX_ERR(0, 276, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_data = values[0];
-    __pyx_v_starting_position = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_starting_position == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L3_error)
+    __pyx_v_starting_position = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_starting_position == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("parse", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 285, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("parse", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 276, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.parse", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_4parse(__pyx_self, __pyx_v_data, __pyx_v_starting_position);
 
@@ -7086,15 +7062,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8minijson_parse(__pyx_v_data, __pyx_v_starting_position, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_parse(__pyx_v_data, __pyx_v_starting_position, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7103,15 +7079,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":301
+/* "minijson.pyx":292
  * 
  * 
  * cpdef object loads(object data):             # <<<<<<<<<<<<<<
  *     """
  *     Reconstruct given JSON from a given value
  */
 
@@ -7122,36 +7098,36 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("loads", 0);
 
-  /* "minijson.pyx":310
+  /* "minijson.pyx":301
  *     :raises DecodingError: something was wrong with the stream
  *     """
  *     return parse(data, 0)[1]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8minijson_parse(__pyx_v_data, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_parse(__pyx_v_data, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 310, __pyx_L1_error)
+    __PYX_ERR(0, 301, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_GetItemInt_Tuple(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt_Tuple(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":301
+  /* "minijson.pyx":292
  * 
  * 
  * cpdef object loads(object data):             # <<<<<<<<<<<<<<
  *     """
  *     Reconstruct given JSON from a given value
  */
 
@@ -7186,15 +7162,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("loads", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8minijson_loads(__pyx_v_data, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_loads(__pyx_v_data, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7203,15 +7179,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":313
+/* "minijson.pyx":304
  * 
  * 
  * cdef inline bint is_jsonable(y):             # <<<<<<<<<<<<<<
  *     return y is None or isinstance(y, (int, float, str, dict, list, tuple))
  * 
  */
 
@@ -7220,15 +7196,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("is_jsonable", 0);
 
-  /* "minijson.pyx":314
+  /* "minijson.pyx":305
  * 
  * cdef inline bint is_jsonable(y):
  *     return y is None or isinstance(y, (int, float, str, dict, list, tuple))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_y == Py_None);
@@ -7279,29 +7255,29 @@
   __pyx_L5_bool_binop_done:;
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "minijson.pyx":313
+  /* "minijson.pyx":304
  * 
  * 
  * cdef inline bint is_jsonable(y):             # <<<<<<<<<<<<<<
  *     return y is None or isinstance(y, (int, float, str, dict, list, tuple))
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":337
+/* "minijson.pyx":328
  *         public bint use_strict_order
  * 
  *     def __init__(self, default: tp.Optional[None] = None,             # <<<<<<<<<<<<<<
  *                  bint use_double = False,
  *                  bint use_strict_order = False):
  */
 
@@ -7351,15 +7327,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_use_strict_order);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 337, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 328, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7367,51 +7343,51 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_default = values[0];
     if (values[1]) {
-      __pyx_v_use_double = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_use_double == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 338, __pyx_L3_error)
+      __pyx_v_use_double = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_use_double == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L3_error)
     } else {
 
-      /* "minijson.pyx":338
+      /* "minijson.pyx":329
  * 
  *     def __init__(self, default: tp.Optional[None] = None,
  *                  bint use_double = False,             # <<<<<<<<<<<<<<
  *                  bint use_strict_order = False):
  *         self._default = default
  */
       __pyx_v_use_double = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_use_strict_order = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_use_strict_order == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L3_error)
+      __pyx_v_use_strict_order = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_use_strict_order == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L3_error)
     } else {
 
-      /* "minijson.pyx":339
+      /* "minijson.pyx":330
  *     def __init__(self, default: tp.Optional[None] = None,
  *                  bint use_double = False,
  *                  bint use_strict_order = False):             # <<<<<<<<<<<<<<
  *         self._default = default
  *         self.use_double = use_double
  */
       __pyx_v_use_strict_order = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 337, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 328, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.MiniJSONEncoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_15MiniJSONEncoder___init__(((struct __pyx_obj_8minijson_MiniJSONEncoder *)__pyx_v_self), __pyx_v_default, __pyx_v_use_double, __pyx_v_use_strict_order);
 
-  /* "minijson.pyx":337
+  /* "minijson.pyx":328
  *         public bint use_strict_order
  * 
  *     def __init__(self, default: tp.Optional[None] = None,             # <<<<<<<<<<<<<<
  *                  bint use_double = False,
  *                  bint use_strict_order = False):
  */
 
@@ -7421,108 +7397,121 @@
 }
 
 static int __pyx_pf_8minijson_15MiniJSONEncoder___init__(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_default, int __pyx_v_use_double, int __pyx_v_use_strict_order) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "minijson.pyx":340
+  /* "minijson.pyx":331
  *                  bint use_double = False,
  *                  bint use_strict_order = False):
  *         self._default = default             # <<<<<<<<<<<<<<
  *         self.use_double = use_double
  *         self.use_strict_order = use_strict_order
  */
   __Pyx_INCREF(__pyx_v_default);
   __Pyx_GIVEREF(__pyx_v_default);
   __Pyx_GOTREF(__pyx_v_self->_default);
   __Pyx_DECREF(__pyx_v_self->_default);
   __pyx_v_self->_default = __pyx_v_default;
 
-  /* "minijson.pyx":341
+  /* "minijson.pyx":332
  *                  bint use_strict_order = False):
  *         self._default = default
  *         self.use_double = use_double             # <<<<<<<<<<<<<<
  *         self.use_strict_order = use_strict_order
  * 
  */
   __pyx_v_self->use_double = __pyx_v_use_double;
 
-  /* "minijson.pyx":342
+  /* "minijson.pyx":333
  *         self._default = default
  *         self.use_double = use_double
  *         self.use_strict_order = use_strict_order             # <<<<<<<<<<<<<<
  * 
- *     def should_double_be_used(self, y) -> bool:
+ *     def should_double_be_used(self, y: float) -> bool:
  */
   __pyx_v_self->use_strict_order = __pyx_v_use_strict_order;
 
-  /* "minijson.pyx":337
+  /* "minijson.pyx":328
  *         public bint use_strict_order
  * 
  *     def __init__(self, default: tp.Optional[None] = None,             # <<<<<<<<<<<<<<
  *                  bint use_double = False,
  *                  bint use_strict_order = False):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":344
+/* "minijson.pyx":335
  *         self.use_strict_order = use_strict_order
  * 
- *     def should_double_be_used(self, y) -> bool:             # <<<<<<<<<<<<<<
+ *     def should_double_be_used(self, y: float) -> bool:             # <<<<<<<<<<<<<<
  *         """
  *         A function that you are meant to overload that will decide on a per-case basis
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8minijson_15MiniJSONEncoder_3should_double_be_used(PyObject *__pyx_v_self, PyObject *__pyx_v_y); /*proto*/
+static PyObject *__pyx_pw_8minijson_15MiniJSONEncoder_3should_double_be_used(PyObject *__pyx_v_self, PyObject *__pyx_arg_y); /*proto*/
 static char __pyx_doc_8minijson_15MiniJSONEncoder_2should_double_be_used[] = "\n        A function that you are meant to overload that will decide on a per-case basis\n        which representation should be used for given number.\n\n        :param y: number to check\n        :return: True if double should be used, else False\n        ";
-static PyObject *__pyx_pw_8minijson_15MiniJSONEncoder_3should_double_be_used(PyObject *__pyx_v_self, PyObject *__pyx_v_y) {
+static PyObject *__pyx_pw_8minijson_15MiniJSONEncoder_3should_double_be_used(PyObject *__pyx_v_self, PyObject *__pyx_arg_y) {
+  CYTHON_UNUSED double __pyx_v_y;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("should_double_be_used (wrapper)", 0);
-  __pyx_r = __pyx_pf_8minijson_15MiniJSONEncoder_2should_double_be_used(((struct __pyx_obj_8minijson_MiniJSONEncoder *)__pyx_v_self), ((PyObject *)__pyx_v_y));
+  assert(__pyx_arg_y); {
+    __pyx_v_y = __pyx_PyFloat_AsDouble(__pyx_arg_y); if (unlikely((__pyx_v_y == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("minijson.MiniJSONEncoder.should_double_be_used", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8minijson_15MiniJSONEncoder_2should_double_be_used(((struct __pyx_obj_8minijson_MiniJSONEncoder *)__pyx_v_self), ((double)__pyx_v_y));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_2should_double_be_used(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_y) {
+static PyObject *__pyx_pf_8minijson_15MiniJSONEncoder_2should_double_be_used(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, CYTHON_UNUSED double __pyx_v_y) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("should_double_be_used", 0);
 
-  /* "minijson.pyx":352
+  /* "minijson.pyx":343
  *         :return: True if double should be used, else False
  *         """
  *         return self.use_double             # <<<<<<<<<<<<<<
  * 
  *     def default(self, v):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->use_double); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->use_double); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":344
+  /* "minijson.pyx":335
  *         self.use_strict_order = use_strict_order
  * 
- *     def should_double_be_used(self, y) -> bool:             # <<<<<<<<<<<<<<
+ *     def should_double_be_used(self, y: float) -> bool:             # <<<<<<<<<<<<<<
  *         """
  *         A function that you are meant to overload that will decide on a per-case basis
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -7530,15 +7519,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":354
+/* "minijson.pyx":345
  *         return self.use_double
  * 
  *     def default(self, v):             # <<<<<<<<<<<<<<
  *         """
  *         Convert an object to a JSON-able representation.
  */
 
@@ -7566,37 +7555,37 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("default", 0);
 
-  /* "minijson.pyx":364
+  /* "minijson.pyx":355
  *         :return: a JSONable representation
  *         """
  *         if self._default is None:             # <<<<<<<<<<<<<<
  *             raise EncodingError('Unknown value type %s' % (v, ))
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_default == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "minijson.pyx":365
+    /* "minijson.pyx":356
  *         """
  *         if self._default is None:
  *             raise EncodingError('Unknown value type %s' % (v, ))             # <<<<<<<<<<<<<<
  *         else:
  *             return self._default(v)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_EncodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_EncodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_v), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_v), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unknown_value_type, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Unknown_value_type, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7604,31 +7593,31 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 365, __pyx_L1_error)
+    __PYX_ERR(0, 356, __pyx_L1_error)
 
-    /* "minijson.pyx":364
+    /* "minijson.pyx":355
  *         :return: a JSONable representation
  *         """
  *         if self._default is None:             # <<<<<<<<<<<<<<
  *             raise EncodingError('Unknown value type %s' % (v, ))
  *         else:
  */
   }
 
-  /* "minijson.pyx":367
+  /* "minijson.pyx":358
  *             raise EncodingError('Unknown value type %s' % (v, ))
  *         else:
  *             return self._default(v)             # <<<<<<<<<<<<<<
  * 
  *     def encode(self, v) -> bytes:
  */
   /*else*/ {
@@ -7642,23 +7631,23 @@
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_v_v) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_v);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "minijson.pyx":354
+  /* "minijson.pyx":345
  *         return self.use_double
  * 
  *     def default(self, v):             # <<<<<<<<<<<<<<
  *         """
  *         Convert an object to a JSON-able representation.
  */
 
@@ -7672,15 +7661,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":369
+/* "minijson.pyx":360
  *             return self._default(v)
  * 
  *     def encode(self, v) -> bytes:             # <<<<<<<<<<<<<<
  *         """
  *         Encode a provided object
  */
 
@@ -7707,84 +7696,84 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 0);
 
-  /* "minijson.pyx":376
+  /* "minijson.pyx":367
  *         :return: returned bytes
  *         """
  *         cio = io.BytesIO()             # <<<<<<<<<<<<<<
  *         self.dump(v, cio)
  *         return cio.getvalue()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_io); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_io); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cio = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "minijson.pyx":377
+  /* "minijson.pyx":368
  *         """
  *         cio = io.BytesIO()
  *         self.dump(v, cio)             # <<<<<<<<<<<<<<
  *         return cio.getvalue()
  * 
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_v, __pyx_v_cio, 0); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_v, __pyx_v_cio, 0); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 368, __pyx_L1_error)
 
-  /* "minijson.pyx":378
+  /* "minijson.pyx":369
  *         cio = io.BytesIO()
  *         self.dump(v, cio)
  *         return cio.getvalue()             # <<<<<<<<<<<<<<
  * 
  *     cpdef int dump(self, object data, cio: io.BytesIO) except -1:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_getvalue); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_getvalue); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 369, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":369
+  /* "minijson.pyx":360
  *             return self._default(v)
  * 
  *     def encode(self, v) -> bytes:             # <<<<<<<<<<<<<<
  *         """
  *         Encode a provided object
  */
 
@@ -7798,28 +7787,27 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_cio);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":380
+/* "minijson.pyx":371
  *         return cio.getvalue()
  * 
  *     cpdef int dump(self, object data, cio: io.BytesIO) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Write an object to a stream
  */
 
 static PyObject *__pyx_pw_8minijson_15MiniJSONEncoder_9dump(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_f_8minijson_15MiniJSONEncoder_dump(struct __pyx_obj_8minijson_MiniJSONEncoder *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_cio, int __pyx_skip_dispatch) {
   PyObject *__pyx_v_field_name = 0;
   unsigned int __pyx_v_length;
   PyObject *__pyx_v_b_data = 0;
-  PyObject *__pyx_v_items = 0;
   PyObject *__pyx_v_elem = NULL;
   PyObject *__pyx_v_offset = NULL;
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_value = NULL;
   PyObject *__pyx_v_v = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -7835,33 +7823,31 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   int __pyx_t_15;
   PyObject *(*__pyx_t_16)(PyObject *);
-  int __pyx_t_17;
-  PyObject *(*__pyx_t_18)(PyObject *);
-  Py_ssize_t __pyx_t_19;
-  int __pyx_t_20;
-  Py_ssize_t __pyx_t_21;
+  PyObject *(*__pyx_t_17)(PyObject *);
+  Py_ssize_t __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dump", 0);
+  __Pyx_INCREF(__pyx_v_data);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dump); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_dump); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_8minijson_15MiniJSONEncoder_9dump)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         __pyx_t_5 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -7872,45 +7858,45 @@
             __Pyx_DECREF_SET(__pyx_t_3, function);
             __pyx_t_5 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_data, __pyx_v_cio};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
           PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_data, __pyx_v_cio};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_2);
         } else
         #endif
         {
-          __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 380, __pyx_L1_error)
+          __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           if (__pyx_t_4) {
             __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
           }
           __Pyx_INCREF(__pyx_v_data);
           __Pyx_GIVEREF(__pyx_v_data);
           PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_data);
           __Pyx_INCREF(__pyx_v_cio);
           __Pyx_GIVEREF(__pyx_v_cio);
           PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_cio);
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -7921,233 +7907,233 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "minijson.pyx":394
+  /* "minijson.pyx":385
  *             bytes b_data
  *             list items
  *         if data is None:             # <<<<<<<<<<<<<<
  *             cio.write(b'\x08')
  *             return 1
  */
   __pyx_t_7 = (__pyx_v_data == Py_None);
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "minijson.pyx":395
+    /* "minijson.pyx":386
  *             list items
  *         if data is None:
  *             cio.write(b'\x08')             # <<<<<<<<<<<<<<
  *             return 1
  *         elif data is True:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 395, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_b__5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 395, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "minijson.pyx":396
+    /* "minijson.pyx":387
  *         if data is None:
  *             cio.write(b'\x08')
  *             return 1             # <<<<<<<<<<<<<<
  *         elif data is True:
  *             cio.write(b'\x16')
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "minijson.pyx":394
+    /* "minijson.pyx":385
  *             bytes b_data
  *             list items
  *         if data is None:             # <<<<<<<<<<<<<<
  *             cio.write(b'\x08')
  *             return 1
  */
   }
 
-  /* "minijson.pyx":397
+  /* "minijson.pyx":388
  *             cio.write(b'\x08')
  *             return 1
  *         elif data is True:             # <<<<<<<<<<<<<<
  *             cio.write(b'\x16')
  *             return 1
  */
   __pyx_t_8 = (__pyx_v_data == Py_True);
   __pyx_t_7 = (__pyx_t_8 != 0);
   if (__pyx_t_7) {
 
-    /* "minijson.pyx":398
+    /* "minijson.pyx":389
  *             return 1
  *         elif data is True:
  *             cio.write(b'\x16')             # <<<<<<<<<<<<<<
  *             return 1
  *         elif data is False:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_b__6) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__6);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "minijson.pyx":399
+    /* "minijson.pyx":390
  *         elif data is True:
  *             cio.write(b'\x16')
  *             return 1             # <<<<<<<<<<<<<<
  *         elif data is False:
  *             cio.write(b'\x17')
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "minijson.pyx":397
+    /* "minijson.pyx":388
  *             cio.write(b'\x08')
  *             return 1
  *         elif data is True:             # <<<<<<<<<<<<<<
  *             cio.write(b'\x16')
  *             return 1
  */
   }
 
-  /* "minijson.pyx":400
+  /* "minijson.pyx":391
  *             cio.write(b'\x16')
  *             return 1
  *         elif data is False:             # <<<<<<<<<<<<<<
  *             cio.write(b'\x17')
  *             return 1
  */
   __pyx_t_7 = (__pyx_v_data == Py_False);
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "minijson.pyx":401
+    /* "minijson.pyx":392
  *             return 1
  *         elif data is False:
  *             cio.write(b'\x17')             # <<<<<<<<<<<<<<
  *             return 1
  *         elif isinstance(data, bytes):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_b__7) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__7);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "minijson.pyx":402
+    /* "minijson.pyx":393
  *         elif data is False:
  *             cio.write(b'\x17')
  *             return 1             # <<<<<<<<<<<<<<
  *         elif isinstance(data, bytes):
  *             length = len(data)
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "minijson.pyx":400
+    /* "minijson.pyx":391
  *             cio.write(b'\x16')
  *             return 1
  *         elif data is False:             # <<<<<<<<<<<<<<
  *             cio.write(b'\x17')
  *             return 1
  */
   }
 
-  /* "minijson.pyx":403
+  /* "minijson.pyx":394
  *             cio.write(b'\x17')
  *             return 1
  *         elif isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if length < 256:
  */
   __pyx_t_8 = PyBytes_Check(__pyx_v_data); 
   __pyx_t_7 = (__pyx_t_8 != 0);
   if (__pyx_t_7) {
 
-    /* "minijson.pyx":404
+    /* "minijson.pyx":395
  *             return 1
  *         elif isinstance(data, bytes):
  *             length = len(data)             # <<<<<<<<<<<<<<
  *             if length < 256:
  *                 cio.write(bytearray([0x19, length]))
  */
-    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 404, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 395, __pyx_L1_error)
     __pyx_v_length = __pyx_t_9;
 
-    /* "minijson.pyx":405
+    /* "minijson.pyx":396
  *         elif isinstance(data, bytes):
  *             length = len(data)
  *             if length < 256:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0x19, length]))
  *                 cio.write(data)
  */
     __pyx_t_7 = ((__pyx_v_length < 0x100) != 0);
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":406
+      /* "minijson.pyx":397
  *             length = len(data)
  *             if length < 256:
  *                 cio.write(bytearray([0x19, length]))             # <<<<<<<<<<<<<<
  *                 cio.write(data)
  *             elif length < 65536:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
+      __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_int_25);
       __Pyx_GIVEREF(__pyx_int_25);
       PyList_SET_ITEM(__pyx_t_6, 0, __pyx_int_25);
       __Pyx_GIVEREF(__pyx_t_3);
       PyList_SET_ITEM(__pyx_t_6, 1, __pyx_t_3);
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8155,80 +8141,80 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":407
+      /* "minijson.pyx":398
  *             if length < 256:
  *                 cio.write(bytearray([0x19, length]))
  *                 cio.write(data)             # <<<<<<<<<<<<<<
  *             elif length < 65536:
  *                 cio.write(b'\x1A' + struct.pack('>H', length))
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":405
+      /* "minijson.pyx":396
  *         elif isinstance(data, bytes):
  *             length = len(data)
  *             if length < 256:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0x19, length]))
  *                 cio.write(data)
  */
       goto __pyx_L4;
     }
 
-    /* "minijson.pyx":408
+    /* "minijson.pyx":399
  *                 cio.write(bytearray([0x19, length]))
  *                 cio.write(data)
  *             elif length < 65536:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x1A' + struct.pack('>H', length))
  *                 cio.write(data)
  */
     __pyx_t_7 = ((__pyx_v_length < 0x10000) != 0);
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":409
+      /* "minijson.pyx":400
  *                 cio.write(data)
  *             elif length < 65536:
  *                 cio.write(b'\x1A' + struct.pack('>H', length))             # <<<<<<<<<<<<<<
  *                 cio.write(data)
  *             else:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_struct); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_struct); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_10 = NULL;
       __pyx_t_5 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8237,47 +8223,47 @@
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_5 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_H, __pyx_t_6};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_H, __pyx_t_6};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_11 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 409, __pyx_L1_error)
+        __pyx_t_11 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         if (__pyx_t_10) {
           __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_10); __pyx_t_10 = NULL;
         }
         __Pyx_INCREF(__pyx_kp_u_H);
         __Pyx_GIVEREF(__pyx_kp_u_H);
         PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_5, __pyx_kp_u_H);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_5, __pyx_t_6);
         __pyx_t_6 = 0;
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyNumber_Add(__pyx_kp_b__8, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+      __pyx_t_4 = PyNumber_Add(__pyx_kp_b__8, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8285,71 +8271,71 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":410
+      /* "minijson.pyx":401
  *             elif length < 65536:
  *                 cio.write(b'\x1A' + struct.pack('>H', length))
  *                 cio.write(data)             # <<<<<<<<<<<<<<
  *             else:
  *                 cio.write(b'\x1B' + struct.pack('>L', length))
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 410, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":408
+      /* "minijson.pyx":399
  *                 cio.write(bytearray([0x19, length]))
  *                 cio.write(data)
  *             elif length < 65536:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x1A' + struct.pack('>H', length))
  *                 cio.write(data)
  */
       goto __pyx_L4;
     }
 
-    /* "minijson.pyx":412
+    /* "minijson.pyx":403
  *                 cio.write(data)
  *             else:
  *                 cio.write(b'\x1B' + struct.pack('>L', length))             # <<<<<<<<<<<<<<
  *                 cio.write(data)
  *         elif isinstance(data, str):
  */
     /*else*/ {
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_struct); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_struct); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_6 = NULL;
       __pyx_t_5 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -8358,47 +8344,47 @@
           __Pyx_DECREF_SET(__pyx_t_11, function);
           __pyx_t_5 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_11)) {
         PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_kp_u_L, __pyx_t_3};
-        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
         PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_kp_u_L, __pyx_t_3};
-        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_6) {
           __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_INCREF(__pyx_kp_u_L);
         __Pyx_GIVEREF(__pyx_kp_u_L);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_5, __pyx_kp_u_L);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_5, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = PyNumber_Add(__pyx_kp_b__9, __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __pyx_t_11 = PyNumber_Add(__pyx_kp_b__9, __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8406,105 +8392,105 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":413
+      /* "minijson.pyx":404
  *             else:
  *                 cio.write(b'\x1B' + struct.pack('>L', length))
  *                 cio.write(data)             # <<<<<<<<<<<<<<
  *         elif isinstance(data, str):
  *             length = len(data)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __pyx_L4:;
 
-    /* "minijson.pyx":403
+    /* "minijson.pyx":394
  *             cio.write(b'\x17')
  *             return 1
  *         elif isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if length < 256:
  */
     goto __pyx_L3;
   }
 
-  /* "minijson.pyx":414
+  /* "minijson.pyx":405
  *                 cio.write(b'\x1B' + struct.pack('>L', length))
  *                 cio.write(data)
  *         elif isinstance(data, str):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if length < 128:
  */
   __pyx_t_7 = PyUnicode_Check(__pyx_v_data); 
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "minijson.pyx":415
+    /* "minijson.pyx":406
  *                 cio.write(data)
  *         elif isinstance(data, str):
  *             length = len(data)             # <<<<<<<<<<<<<<
  *             if length < 128:
  *                 cio.write(bytearray([0x80 | length]))
  */
-    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 406, __pyx_L1_error)
     __pyx_v_length = __pyx_t_9;
 
-    /* "minijson.pyx":416
+    /* "minijson.pyx":407
  *         elif isinstance(data, str):
  *             length = len(data)
  *             if length < 128:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0x80 | length]))
  *                 cio.write(data.encode('utf-8'))
  */
     __pyx_t_8 = ((__pyx_v_length < 0x80) != 0);
     if (__pyx_t_8) {
 
-      /* "minijson.pyx":417
+      /* "minijson.pyx":408
  *             length = len(data)
  *             if length < 128:
  *                 cio.write(bytearray([0x80 | length]))             # <<<<<<<<<<<<<<
  *                 cio.write(data.encode('utf-8'))
  *                 return 1+length
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyInt_From_long((0x80 | __pyx_v_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 417, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_From_long((0x80 | __pyx_v_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
+      __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_11);
       PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_11);
       __pyx_t_11 = 0;
-      __pyx_t_11 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 417, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8512,43 +8498,43 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":418
+      /* "minijson.pyx":409
  *             if length < 128:
  *                 cio.write(bytearray([0x80 | length]))
  *                 cio.write(data.encode('utf-8'))             # <<<<<<<<<<<<<<
  *                 return 1+length
  *             elif length <= 0xFF:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 418, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8556,68 +8542,68 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":419
+      /* "minijson.pyx":410
  *                 cio.write(bytearray([0x80 | length]))
  *                 cio.write(data.encode('utf-8'))
  *                 return 1+length             # <<<<<<<<<<<<<<
  *             elif length <= 0xFF:
  *                 cio.write(bytearray([0, length]))
  */
       __pyx_r = (1 + __pyx_v_length);
       goto __pyx_L0;
 
-      /* "minijson.pyx":416
+      /* "minijson.pyx":407
  *         elif isinstance(data, str):
  *             length = len(data)
  *             if length < 128:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0x80 | length]))
  *                 cio.write(data.encode('utf-8'))
  */
     }
 
-    /* "minijson.pyx":420
+    /* "minijson.pyx":411
  *                 cio.write(data.encode('utf-8'))
  *                 return 1+length
  *             elif length <= 0xFF:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0, length]))
  *                 cio.write(data.encode('utf-8'))
  */
     __pyx_t_8 = ((__pyx_v_length <= 0xFF) != 0);
     if (__pyx_t_8) {
 
-      /* "minijson.pyx":421
+      /* "minijson.pyx":412
  *                 return 1+length
  *             elif length <= 0xFF:
  *                 cio.write(bytearray([0, length]))             # <<<<<<<<<<<<<<
  *                 cio.write(data.encode('utf-8'))
  *                 return 2+length
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
       PyList_SET_ITEM(__pyx_t_4, 0, __pyx_int_0);
       __Pyx_GIVEREF(__pyx_t_11);
       PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_11);
       __pyx_t_11 = 0;
-      __pyx_t_11 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8625,43 +8611,43 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":422
+      /* "minijson.pyx":413
  *             elif length <= 0xFF:
  *                 cio.write(bytearray([0, length]))
  *                 cio.write(data.encode('utf-8'))             # <<<<<<<<<<<<<<
  *                 return 2+length
  *             elif length <= 0xFFFF:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 422, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8669,101 +8655,101 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":423
+      /* "minijson.pyx":414
  *                 cio.write(bytearray([0, length]))
  *                 cio.write(data.encode('utf-8'))
  *                 return 2+length             # <<<<<<<<<<<<<<
  *             elif length <= 0xFFFF:
  *                 cio.write(b'\x0D')
  */
       __pyx_r = (2 + __pyx_v_length);
       goto __pyx_L0;
 
-      /* "minijson.pyx":420
+      /* "minijson.pyx":411
  *                 cio.write(data.encode('utf-8'))
  *                 return 1+length
  *             elif length <= 0xFF:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0, length]))
  *                 cio.write(data.encode('utf-8'))
  */
     }
 
-    /* "minijson.pyx":424
+    /* "minijson.pyx":415
  *                 cio.write(data.encode('utf-8'))
  *                 return 2+length
  *             elif length <= 0xFFFF:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0D')
  *                 cio.write(STRUCT_H.pack(length))
  */
     __pyx_t_8 = ((__pyx_v_length <= 0xFFFF) != 0);
     if (__pyx_t_8) {
 
-      /* "minijson.pyx":425
+      /* "minijson.pyx":416
  *                 return 2+length
  *             elif length <= 0xFFFF:
  *                 cio.write(b'\x0D')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_H.pack(length))
  *                 cio.write(data.encode('utf-8'))
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_kp_b__10) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__10);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":426
+      /* "minijson.pyx":417
  *             elif length <= 0xFFFF:
  *                 cio.write(b'\x0D')
  *                 cio.write(STRUCT_H.pack(length))             # <<<<<<<<<<<<<<
  *                 cio.write(data.encode('utf-8'))
  *                 return 3+length
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8771,43 +8757,43 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":427
+      /* "minijson.pyx":418
  *                 cio.write(b'\x0D')
  *                 cio.write(STRUCT_H.pack(length))
  *                 cio.write(data.encode('utf-8'))             # <<<<<<<<<<<<<<
  *                 return 3+length
  *             else:       # Python strings cannot grow past 0xFFFFFFFF characters
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 427, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8815,92 +8801,92 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":428
+      /* "minijson.pyx":419
  *                 cio.write(STRUCT_H.pack(length))
  *                 cio.write(data.encode('utf-8'))
  *                 return 3+length             # <<<<<<<<<<<<<<
  *             else:       # Python strings cannot grow past 0xFFFFFFFF characters
  *                 cio.write(b'\x0E')
  */
       __pyx_r = (3 + __pyx_v_length);
       goto __pyx_L0;
 
-      /* "minijson.pyx":424
+      /* "minijson.pyx":415
  *                 cio.write(data.encode('utf-8'))
  *                 return 2+length
  *             elif length <= 0xFFFF:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0D')
  *                 cio.write(STRUCT_H.pack(length))
  */
     }
 
-    /* "minijson.pyx":430
+    /* "minijson.pyx":421
  *                 return 3+length
  *             else:       # Python strings cannot grow past 0xFFFFFFFF characters
  *                 cio.write(b'\x0E')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_L.pack(length))
  *                 cio.write(data.encode('utf-8'))
  */
     /*else*/ {
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_kp_b__11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__11);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":431
+      /* "minijson.pyx":422
  *             else:       # Python strings cannot grow past 0xFFFFFFFF characters
  *                 cio.write(b'\x0E')
  *                 cio.write(STRUCT_L.pack(length))             # <<<<<<<<<<<<<<
  *                 cio.write(data.encode('utf-8'))
  *                 return 5+length
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 431, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 431, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8908,43 +8894,43 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":432
+      /* "minijson.pyx":423
  *                 cio.write(b'\x0E')
  *                 cio.write(STRUCT_L.pack(length))
  *                 cio.write(data.encode('utf-8'))             # <<<<<<<<<<<<<<
  *                 return 5+length
  *         elif isinstance(data, int):
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 432, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8952,116 +8938,116 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":433
+      /* "minijson.pyx":424
  *                 cio.write(STRUCT_L.pack(length))
  *                 cio.write(data.encode('utf-8'))
  *                 return 5+length             # <<<<<<<<<<<<<<
  *         elif isinstance(data, int):
  *             if -128 <= data <= 127: # signed char, type 3
  */
       __pyx_r = (5 + __pyx_v_length);
       goto __pyx_L0;
     }
 
-    /* "minijson.pyx":414
+    /* "minijson.pyx":405
  *                 cio.write(b'\x1B' + struct.pack('>L', length))
  *                 cio.write(data)
  *         elif isinstance(data, str):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if length < 128:
  */
   }
 
-  /* "minijson.pyx":434
+  /* "minijson.pyx":425
  *                 cio.write(data.encode('utf-8'))
  *                 return 5+length
  *         elif isinstance(data, int):             # <<<<<<<<<<<<<<
  *             if -128 <= data <= 127: # signed char, type 3
  *                 cio.write(b'\x03')
  */
   __pyx_t_8 = PyInt_Check(__pyx_v_data); 
   __pyx_t_7 = (__pyx_t_8 != 0);
   if (__pyx_t_7) {
 
-    /* "minijson.pyx":435
+    /* "minijson.pyx":426
  *                 return 5+length
  *         elif isinstance(data, int):
  *             if -128 <= data <= 127: # signed char, type 3             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x03')
  *                 cio.write(STRUCT_b.pack(data))
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_neg_128, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_neg_128, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_127, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_127, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 435, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":436
+      /* "minijson.pyx":427
  *         elif isinstance(data, int):
  *             if -128 <= data <= 127: # signed char, type 3
  *                 cio.write(b'\x03')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_b.pack(data))
  *                 return 2
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_kp_b__12) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__12);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":437
+      /* "minijson.pyx":428
  *             if -128 <= data <= 127: # signed char, type 3
  *                 cio.write(b'\x03')
  *                 cio.write(STRUCT_b.pack(data))             # <<<<<<<<<<<<<<
  *                 return 2
  *             elif 0 <= data <= 255:  # unsigned char, type 6
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_b, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_b, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 437, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9069,72 +9055,72 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":438
+      /* "minijson.pyx":429
  *                 cio.write(b'\x03')
  *                 cio.write(STRUCT_b.pack(data))
  *                 return 2             # <<<<<<<<<<<<<<
  *             elif 0 <= data <= 255:  # unsigned char, type 6
  *                 cio.write(bytearray([6, data]))
  */
       __pyx_r = 2;
       goto __pyx_L0;
 
-      /* "minijson.pyx":435
+      /* "minijson.pyx":426
  *                 return 5+length
  *         elif isinstance(data, int):
  *             if -128 <= data <= 127: # signed char, type 3             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x03')
  *                 cio.write(STRUCT_b.pack(data))
  */
     }
 
-    /* "minijson.pyx":439
+    /* "minijson.pyx":430
  *                 cio.write(STRUCT_b.pack(data))
  *                 return 2
  *             elif 0 <= data <= 255:  # unsigned char, type 6             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([6, data]))
  *                 return 2
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_255, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_255, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 430, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":440
+      /* "minijson.pyx":431
  *                 return 2
  *             elif 0 <= data <= 255:  # unsigned char, type 6
  *                 cio.write(bytearray([6, data]))             # <<<<<<<<<<<<<<
  *                 return 2
  *             elif -32768 <= data <= 32767:   # signed short, type 2
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = PyList_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_11 = PyList_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 431, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_INCREF(__pyx_int_6);
       __Pyx_GIVEREF(__pyx_int_6);
       PyList_SET_ITEM(__pyx_t_11, 0, __pyx_int_6);
       __Pyx_INCREF(__pyx_v_data);
       __Pyx_GIVEREF(__pyx_v_data);
       PyList_SET_ITEM(__pyx_t_11, 1, __pyx_v_data);
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 431, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9142,104 +9128,104 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":441
+      /* "minijson.pyx":432
  *             elif 0 <= data <= 255:  # unsigned char, type 6
  *                 cio.write(bytearray([6, data]))
  *                 return 2             # <<<<<<<<<<<<<<
  *             elif -32768 <= data <= 32767:   # signed short, type 2
  *                 cio.write(b'\x02')
  */
       __pyx_r = 2;
       goto __pyx_L0;
 
-      /* "minijson.pyx":439
+      /* "minijson.pyx":430
  *                 cio.write(STRUCT_b.pack(data))
  *                 return 2
  *             elif 0 <= data <= 255:  # unsigned char, type 6             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([6, data]))
  *                 return 2
  */
     }
 
-    /* "minijson.pyx":442
+    /* "minijson.pyx":433
  *                 cio.write(bytearray([6, data]))
  *                 return 2
  *             elif -32768 <= data <= 32767:   # signed short, type 2             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x02')
  *                 cio.write(STRUCT_h.pack(data))
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_neg_32768, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_neg_32768, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_32767, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_32767, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":443
+      /* "minijson.pyx":434
  *                 return 2
  *             elif -32768 <= data <= 32767:   # signed short, type 2
  *                 cio.write(b'\x02')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_h.pack(data))
  *                 return 3
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 434, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__13) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__13);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 434, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":444
+      /* "minijson.pyx":435
  *             elif -32768 <= data <= 32767:   # signed short, type 2
  *                 cio.write(b'\x02')
  *                 cio.write(STRUCT_h.pack(data))             # <<<<<<<<<<<<<<
  *                 return 3
  *             elif 0 <= data <= 65535:        # unsigned short, type 5
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 435, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_h, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 444, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_h, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 435, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
         }
       }
       __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9247,104 +9233,104 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 444, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":445
+      /* "minijson.pyx":436
  *                 cio.write(b'\x02')
  *                 cio.write(STRUCT_h.pack(data))
  *                 return 3             # <<<<<<<<<<<<<<
  *             elif 0 <= data <= 65535:        # unsigned short, type 5
  *                 cio.write(b'\x05')
  */
       __pyx_r = 3;
       goto __pyx_L0;
 
-      /* "minijson.pyx":442
+      /* "minijson.pyx":433
  *                 cio.write(bytearray([6, data]))
  *                 return 2
  *             elif -32768 <= data <= 32767:   # signed short, type 2             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x02')
  *                 cio.write(STRUCT_h.pack(data))
  */
     }
 
-    /* "minijson.pyx":446
+    /* "minijson.pyx":437
  *                 cio.write(STRUCT_h.pack(data))
  *                 return 3
  *             elif 0 <= data <= 65535:        # unsigned short, type 5             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x05')
  *                 cio.write(STRUCT_H.pack(data))
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_65535, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_65535, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":447
+      /* "minijson.pyx":438
  *                 return 3
  *             elif 0 <= data <= 65535:        # unsigned short, type 5
  *                 cio.write(b'\x05')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_H.pack(data))
  *                 return 3
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 438, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__14) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__14);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":448
+      /* "minijson.pyx":439
  *             elif 0 <= data <= 65535:        # unsigned short, type 5
  *                 cio.write(b'\x05')
  *                 cio.write(STRUCT_H.pack(data))             # <<<<<<<<<<<<<<
  *                 return 3
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 448, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 448, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
         }
       }
       __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9352,107 +9338,107 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":449
+      /* "minijson.pyx":440
  *                 cio.write(b'\x05')
  *                 cio.write(STRUCT_H.pack(data))
  *                 return 3             # <<<<<<<<<<<<<<
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12
  *                 cio.write(b'\x0C')
  */
       __pyx_r = 3;
       goto __pyx_L0;
 
-      /* "minijson.pyx":446
+      /* "minijson.pyx":437
  *                 cio.write(STRUCT_h.pack(data))
  *                 return 3
  *             elif 0 <= data <= 65535:        # unsigned short, type 5             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x05')
  *                 cio.write(STRUCT_H.pack(data))
  */
     }
 
-    /* "minijson.pyx":450
+    /* "minijson.pyx":441
  *                 cio.write(STRUCT_H.pack(data))
  *                 return 3
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0C')
  *                 cio.write(STRUCT_L.pack(data)[1:])
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_16777215, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_16777215, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 450, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 441, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":451
+      /* "minijson.pyx":442
  *                 return 3
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12
  *                 cio.write(b'\x0C')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_L.pack(data)[1:])
  *                 return 4
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__15) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__15);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":452
+      /* "minijson.pyx":443
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12
  *                 cio.write(b'\x0C')
  *                 cio.write(STRUCT_L.pack(data)[1:])             # <<<<<<<<<<<<<<
  *                 return 4
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 443, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
         }
       }
       __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 452, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 443, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_t_4, 1, 0, NULL, NULL, &__pyx_slice__16, 1, 0, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 452, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_t_4, 1, 0, NULL, NULL, &__pyx_slice__16, 1, 0, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 443, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9460,104 +9446,104 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":453
+      /* "minijson.pyx":444
  *                 cio.write(b'\x0C')
  *                 cio.write(STRUCT_L.pack(data)[1:])
  *                 return 4             # <<<<<<<<<<<<<<
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1
  *                 cio.write(b'\x01')
  */
       __pyx_r = 4;
       goto __pyx_L0;
 
-      /* "minijson.pyx":450
+      /* "minijson.pyx":441
  *                 cio.write(STRUCT_H.pack(data))
  *                 return 3
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0C')
  *                 cio.write(STRUCT_L.pack(data)[1:])
  */
     }
 
-    /* "minijson.pyx":454
+    /* "minijson.pyx":445
  *                 cio.write(STRUCT_L.pack(data)[1:])
  *                 return 4
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x01')
  *                 cio.write(STRUCT_l.pack(data))
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_neg_2147483648, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_neg_2147483648, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_2147483647, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_2147483647, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 454, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":455
+      /* "minijson.pyx":446
  *                 return 4
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1
  *                 cio.write(b'\x01')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_l.pack(data))
  *                 return 5
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_kp_b__17) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__17);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":456
+      /* "minijson.pyx":447
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1
  *                 cio.write(b'\x01')
  *                 cio.write(STRUCT_l.pack(data))             # <<<<<<<<<<<<<<
  *                 return 5
  *             elif 0 <= data <= 0xFFFFFFFF:       # unsigned int, type 4
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_l, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 456, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_l, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 456, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9565,104 +9551,104 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 456, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":457
+      /* "minijson.pyx":448
  *                 cio.write(b'\x01')
  *                 cio.write(STRUCT_l.pack(data))
  *                 return 5             # <<<<<<<<<<<<<<
  *             elif 0 <= data <= 0xFFFFFFFF:       # unsigned int, type 4
  *                 cio.write(b'\x04')
  */
       __pyx_r = 5;
       goto __pyx_L0;
 
-      /* "minijson.pyx":454
+      /* "minijson.pyx":445
  *                 cio.write(STRUCT_L.pack(data)[1:])
  *                 return 4
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x01')
  *                 cio.write(STRUCT_l.pack(data))
  */
     }
 
-    /* "minijson.pyx":458
+    /* "minijson.pyx":449
  *                 cio.write(STRUCT_l.pack(data))
  *                 return 5
  *             elif 0 <= data <= 0xFFFFFFFF:       # unsigned int, type 4             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x04')
  *                 cio.write(STRUCT_L.pack(data))
  */
-    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_int_0, __pyx_v_data, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 449, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
       __Pyx_DECREF(__pyx_t_1);
-      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_data, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 449, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 458, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":459
+      /* "minijson.pyx":450
  *                 return 5
  *             elif 0 <= data <= 0xFFFFFFFF:       # unsigned int, type 4
  *                 cio.write(b'\x04')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_L.pack(data))
  *                 return 5
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_kp_b__18) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__18);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":460
+      /* "minijson.pyx":451
  *             elif 0 <= data <= 0xFFFFFFFF:       # unsigned int, type 4
  *                 cio.write(b'\x04')
  *                 cio.write(STRUCT_L.pack(data))             # <<<<<<<<<<<<<<
  *                 return 5
  *             else:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 460, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 460, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 460, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9670,58 +9656,58 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "minijson.pyx":461
+      /* "minijson.pyx":452
  *                 cio.write(b'\x04')
  *                 cio.write(STRUCT_L.pack(data))
  *                 return 5             # <<<<<<<<<<<<<<
  *             else:
  *                 length = 5
  */
       __pyx_r = 5;
       goto __pyx_L0;
 
-      /* "minijson.pyx":458
+      /* "minijson.pyx":449
  *                 cio.write(STRUCT_l.pack(data))
  *                 return 5
  *             elif 0 <= data <= 0xFFFFFFFF:       # unsigned int, type 4             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x04')
  *                 cio.write(STRUCT_L.pack(data))
  */
     }
 
-    /* "minijson.pyx":463
+    /* "minijson.pyx":454
  *                 return 5
  *             else:
  *                 length = 5             # <<<<<<<<<<<<<<
  *                 while True:
  *                     try:
  */
     /*else*/ {
       __pyx_v_length = 5;
 
-      /* "minijson.pyx":464
+      /* "minijson.pyx":455
  *             else:
  *                 length = 5
  *                 while True:             # <<<<<<<<<<<<<<
  *                     try:
  *                         b_data = data.to_bytes(length, 'big', signed=True)
  */
       while (1) {
 
-        /* "minijson.pyx":465
+        /* "minijson.pyx":456
  *                 length = 5
  *                 while True:
  *                     try:             # <<<<<<<<<<<<<<
  *                         b_data = data.to_bytes(length, 'big', signed=True)
  *                         break
  */
         {
@@ -9729,55 +9715,55 @@
           __Pyx_PyThreadState_assign
           __Pyx_ExceptionSave(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           /*try:*/ {
 
-            /* "minijson.pyx":466
+            /* "minijson.pyx":457
  *                 while True:
  *                     try:
  *                         b_data = data.to_bytes(length, 'big', signed=True)             # <<<<<<<<<<<<<<
  *                         break
  *                     except OverflowError:
  */
-            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L9_error)
+            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L9_error)
+            __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 466, __pyx_L9_error)
+            __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 457, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_GIVEREF(__pyx_t_2);
             PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_2);
             __Pyx_INCREF(__pyx_n_u_big);
             __Pyx_GIVEREF(__pyx_n_u_big);
             PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_n_u_big);
             __pyx_t_2 = 0;
-            __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L9_error)
+            __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_2);
-            if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_signed, Py_True) < 0) __PYX_ERR(0, 466, __pyx_L9_error)
-            __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_11, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 466, __pyx_L9_error)
+            if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_signed, Py_True) < 0) __PYX_ERR(0, 457, __pyx_L9_error)
+            __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_11, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L9_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 466, __pyx_L9_error)
+            if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 457, __pyx_L9_error)
             __Pyx_XDECREF_SET(__pyx_v_b_data, ((PyObject*)__pyx_t_4));
             __pyx_t_4 = 0;
 
-            /* "minijson.pyx":467
+            /* "minijson.pyx":458
  *                     try:
  *                         b_data = data.to_bytes(length, 'big', signed=True)
  *                         break             # <<<<<<<<<<<<<<
  *                     except OverflowError:
  *                         length += 1
  */
             goto __pyx_L14_try_break;
 
-            /* "minijson.pyx":465
+            /* "minijson.pyx":456
  *                 length = 5
  *                 while True:
  *                     try:             # <<<<<<<<<<<<<<
  *                         b_data = data.to_bytes(length, 'big', signed=True)
  *                         break
  */
           }
@@ -9786,30 +9772,30 @@
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-          /* "minijson.pyx":468
+          /* "minijson.pyx":459
  *                         b_data = data.to_bytes(length, 'big', signed=True)
  *                         break
  *                     except OverflowError:             # <<<<<<<<<<<<<<
  *                         length += 1
  *                 cio.write(bytearray([0x18, length]))
  */
           __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_OverflowError);
           if (__pyx_t_5) {
             __Pyx_AddTraceback("minijson.MiniJSONEncoder.dump", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_11) < 0) __PYX_ERR(0, 468, __pyx_L11_except_error)
+            if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_11) < 0) __PYX_ERR(0, 459, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_GOTREF(__pyx_t_11);
 
-            /* "minijson.pyx":469
+            /* "minijson.pyx":460
  *                         break
  *                     except OverflowError:
  *                         length += 1             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0x18, length]))
  *                 cio.write(b_data)
  */
             __pyx_v_length = (__pyx_v_length + 1);
@@ -9817,15 +9803,15 @@
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             goto __pyx_L10_exception_handled;
           }
           goto __pyx_L11_except_error;
           __pyx_L11_except_error:;
 
-          /* "minijson.pyx":465
+          /* "minijson.pyx":456
  *                 length = 5
  *                 while True:
  *                     try:             # <<<<<<<<<<<<<<
  *                         b_data = data.to_bytes(length, 'big', signed=True)
  *                         break
  */
           __Pyx_XGIVEREF(__pyx_t_12);
@@ -9844,34 +9830,34 @@
           __Pyx_XGIVEREF(__pyx_t_13);
           __Pyx_XGIVEREF(__pyx_t_14);
           __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_13, __pyx_t_14);
         }
       }
       __pyx_L8_break:;
 
-      /* "minijson.pyx":470
+      /* "minijson.pyx":461
  *                     except OverflowError:
  *                         length += 1
  *                 cio.write(bytearray([0x18, length]))             # <<<<<<<<<<<<<<
  *                 cio.write(b_data)
  *         elif isinstance(data, float):
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_int_24);
       __Pyx_GIVEREF(__pyx_int_24);
       PyList_SET_ITEM(__pyx_t_1, 0, __pyx_int_24);
       __Pyx_GIVEREF(__pyx_t_4);
       PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9879,146 +9865,146 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 470, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":471
+      /* "minijson.pyx":462
  *                         length += 1
  *                 cio.write(bytearray([0x18, length]))
  *                 cio.write(b_data)             # <<<<<<<<<<<<<<
  *         elif isinstance(data, float):
  *             if self.should_double_be_used(data):
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 471, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 462, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(!__pyx_v_b_data)) { __Pyx_RaiseUnboundLocalError("b_data"); __PYX_ERR(0, 471, __pyx_L1_error) }
+      if (unlikely(!__pyx_v_b_data)) { __Pyx_RaiseUnboundLocalError("b_data"); __PYX_ERR(0, 462, __pyx_L1_error) }
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_b_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_b_data);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 471, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 462, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
 
-    /* "minijson.pyx":434
+    /* "minijson.pyx":425
  *                 cio.write(data.encode('utf-8'))
  *                 return 5+length
  *         elif isinstance(data, int):             # <<<<<<<<<<<<<<
  *             if -128 <= data <= 127: # signed char, type 3
  *                 cio.write(b'\x03')
  */
     goto __pyx_L3;
   }
 
-  /* "minijson.pyx":472
+  /* "minijson.pyx":463
  *                 cio.write(bytearray([0x18, length]))
  *                 cio.write(b_data)
  *         elif isinstance(data, float):             # <<<<<<<<<<<<<<
  *             if self.should_double_be_used(data):
  *                 cio.write(b'\x0A')
  */
   __pyx_t_7 = PyFloat_Check(__pyx_v_data); 
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "minijson.pyx":473
+    /* "minijson.pyx":464
  *                 cio.write(b_data)
  *         elif isinstance(data, float):
  *             if self.should_double_be_used(data):             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0A')
  *                 cio.write(STRUCT_d.pack(data))
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_should_double_be_used); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_should_double_be_used); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 473, __pyx_L1_error)
+    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 464, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     if (__pyx_t_8) {
 
-      /* "minijson.pyx":474
+      /* "minijson.pyx":465
  *         elif isinstance(data, float):
  *             if self.should_double_be_used(data):
  *                 cio.write(b'\x0A')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_d.pack(data))
  *                 return 9
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 474, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__19) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__19);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 474, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 465, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":475
+      /* "minijson.pyx":466
  *             if self.should_double_be_used(data):
  *                 cio.write(b'\x0A')
  *                 cio.write(STRUCT_d.pack(data))             # <<<<<<<<<<<<<<
  *                 return 9
  *             else:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 475, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_d, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_d, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 475, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 466, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10026,89 +10012,89 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 475, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 466, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":476
+      /* "minijson.pyx":467
  *                 cio.write(b'\x0A')
  *                 cio.write(STRUCT_d.pack(data))
  *                 return 9             # <<<<<<<<<<<<<<
  *             else:
  *                 cio.write(b'\x09')
  */
       __pyx_r = 9;
       goto __pyx_L0;
 
-      /* "minijson.pyx":473
+      /* "minijson.pyx":464
  *                 cio.write(b_data)
  *         elif isinstance(data, float):
  *             if self.should_double_be_used(data):             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0A')
  *                 cio.write(STRUCT_d.pack(data))
  */
     }
 
-    /* "minijson.pyx":478
+    /* "minijson.pyx":469
  *                 return 9
  *             else:
  *                 cio.write(b'\x09')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_f.pack(data))
  *                 return 5
  */
     /*else*/ {
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__20) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__20);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 478, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 469, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":479
+      /* "minijson.pyx":470
  *             else:
  *                 cio.write(b'\x09')
  *                 cio.write(STRUCT_f.pack(data))             # <<<<<<<<<<<<<<
  *                 return 5
  *         elif isinstance(data, (tuple, list)):
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 479, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_f, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_f, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_data);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 479, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10116,40 +10102,40 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 479, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 470, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":480
+      /* "minijson.pyx":471
  *                 cio.write(b'\x09')
  *                 cio.write(STRUCT_f.pack(data))
  *                 return 5             # <<<<<<<<<<<<<<
  *         elif isinstance(data, (tuple, list)):
  *             length = len(data)
  */
       __pyx_r = 5;
       goto __pyx_L0;
     }
 
-    /* "minijson.pyx":472
+    /* "minijson.pyx":463
  *                 cio.write(bytearray([0x18, length]))
  *                 cio.write(b_data)
  *         elif isinstance(data, float):             # <<<<<<<<<<<<<<
  *             if self.should_double_be_used(data):
  *                 cio.write(b'\x0A')
  */
   }
 
-  /* "minijson.pyx":481
+  /* "minijson.pyx":472
  *                 cio.write(STRUCT_f.pack(data))
  *                 return 5
  *         elif isinstance(data, (tuple, list)):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if length < 16:
  */
   __pyx_t_7 = PyTuple_Check(__pyx_v_data); 
@@ -10162,51 +10148,51 @@
   __pyx_t_15 = PyList_Check(__pyx_v_data); 
   __pyx_t_7 = (__pyx_t_15 != 0);
   __pyx_t_8 = __pyx_t_7;
   __pyx_L20_bool_binop_done:;
   __pyx_t_7 = (__pyx_t_8 != 0);
   if (__pyx_t_7) {
 
-    /* "minijson.pyx":482
+    /* "minijson.pyx":473
  *                 return 5
  *         elif isinstance(data, (tuple, list)):
  *             length = len(data)             # <<<<<<<<<<<<<<
  *             if length < 16:
  *                 cio.write(bytearray([0b01000000 | length]))
  */
-    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 482, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 473, __pyx_L1_error)
     __pyx_v_length = __pyx_t_9;
 
-    /* "minijson.pyx":483
+    /* "minijson.pyx":474
  *         elif isinstance(data, (tuple, list)):
  *             length = len(data)
  *             if length < 16:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0b01000000 | length]))
  *                 length = 1
  */
     __pyx_t_7 = ((__pyx_v_length < 16) != 0);
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":484
+      /* "minijson.pyx":475
  *             length = len(data)
  *             if length < 16:
  *                 cio.write(bytearray([0b01000000 | length]))             # <<<<<<<<<<<<<<
  *                 length = 1
  *             elif length < 256:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 475, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyInt_From_long((64 | __pyx_v_length)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_long((64 | __pyx_v_length)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 475, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 475, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10214,68 +10200,68 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 484, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 475, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":485
+      /* "minijson.pyx":476
  *             if length < 16:
  *                 cio.write(bytearray([0b01000000 | length]))
  *                 length = 1             # <<<<<<<<<<<<<<
  *             elif length < 256:
  *                 cio.write(bytearray([7, length]))
  */
       __pyx_v_length = 1;
 
-      /* "minijson.pyx":483
+      /* "minijson.pyx":474
  *         elif isinstance(data, (tuple, list)):
  *             length = len(data)
  *             if length < 16:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([0b01000000 | length]))
  *                 length = 1
  */
       goto __pyx_L22;
     }
 
-    /* "minijson.pyx":486
+    /* "minijson.pyx":477
  *                 cio.write(bytearray([0b01000000 | length]))
  *                 length = 1
  *             elif length < 256:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([7, length]))
  *                 length = 2
  */
     __pyx_t_7 = ((__pyx_v_length < 0x100) != 0);
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":487
+      /* "minijson.pyx":478
  *                 length = 1
  *             elif length < 256:
  *                 cio.write(bytearray([7, length]))             # <<<<<<<<<<<<<<
  *                 length = 2
  *             elif length < 65536:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 487, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_int_7);
       __Pyx_GIVEREF(__pyx_int_7);
       PyList_SET_ITEM(__pyx_t_1, 0, __pyx_int_7);
       __Pyx_GIVEREF(__pyx_t_4);
       PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10283,101 +10269,101 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 487, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 478, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":488
+      /* "minijson.pyx":479
  *             elif length < 256:
  *                 cio.write(bytearray([7, length]))
  *                 length = 2             # <<<<<<<<<<<<<<
  *             elif length < 65536:
  *                 cio.write(b'\x0F')
  */
       __pyx_v_length = 2;
 
-      /* "minijson.pyx":486
+      /* "minijson.pyx":477
  *                 cio.write(bytearray([0b01000000 | length]))
  *                 length = 1
  *             elif length < 256:             # <<<<<<<<<<<<<<
  *                 cio.write(bytearray([7, length]))
  *                 length = 2
  */
       goto __pyx_L22;
     }
 
-    /* "minijson.pyx":489
+    /* "minijson.pyx":480
  *                 cio.write(bytearray([7, length]))
  *                 length = 2
  *             elif length < 65536:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0F')
  *                 cio.write(STRUCT_H.pack(length))
  */
     __pyx_t_7 = ((__pyx_v_length < 0x10000) != 0);
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":490
+      /* "minijson.pyx":481
  *                 length = 2
  *             elif length < 65536:
  *                 cio.write(b'\x0F')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_H.pack(length))
  *                 length = 3
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 490, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 481, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__21) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__21);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 490, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 481, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":491
+      /* "minijson.pyx":482
  *             elif length < 65536:
  *                 cio.write(b'\x0F')
  *                 cio.write(STRUCT_H.pack(length))             # <<<<<<<<<<<<<<
  *                 length = 3
  *             elif length <= 0xFFFFFFFF:
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 491, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_10);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10385,106 +10371,106 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 491, __pyx_L1_error)
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 482, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":492
+      /* "minijson.pyx":483
  *                 cio.write(b'\x0F')
  *                 cio.write(STRUCT_H.pack(length))
  *                 length = 3             # <<<<<<<<<<<<<<
  *             elif length <= 0xFFFFFFFF:
  *                 cio.write(b'\x10')
  */
       __pyx_v_length = 3;
 
-      /* "minijson.pyx":489
+      /* "minijson.pyx":480
  *                 cio.write(bytearray([7, length]))
  *                 length = 2
  *             elif length < 65536:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x0F')
  *                 cio.write(STRUCT_H.pack(length))
  */
       goto __pyx_L22;
     }
 
-    /* "minijson.pyx":493
+    /* "minijson.pyx":484
  *                 cio.write(STRUCT_H.pack(length))
  *                 length = 3
  *             elif length <= 0xFFFFFFFF:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x10')
  *                 cio.write(STRUCT_L.pack(length))
  */
-    __pyx_t_11 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_t_11, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_t_11, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_7) {
 
-      /* "minijson.pyx":494
+      /* "minijson.pyx":485
  *                 length = 3
  *             elif length <= 0xFFFFFFFF:
  *                 cio.write(b'\x10')             # <<<<<<<<<<<<<<
  *                 cio.write(STRUCT_L.pack(length))
  *                 length = 5
  */
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 494, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 485, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
         }
       }
       __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_4, __pyx_kp_b__22) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_b__22);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 485, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "minijson.pyx":495
+      /* "minijson.pyx":486
  *             elif length <= 0xFFFFFFFF:
  *                 cio.write(b'\x10')
  *                 cio.write(STRUCT_L.pack(length))             # <<<<<<<<<<<<<<
  *                 length = 5
  *             for elem in data:
  */
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 495, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 495, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_10);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -10492,184 +10478,184 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
         }
       }
       __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "minijson.pyx":496
+      /* "minijson.pyx":487
  *                 cio.write(b'\x10')
  *                 cio.write(STRUCT_L.pack(length))
  *                 length = 5             # <<<<<<<<<<<<<<
  *             for elem in data:
  *                 length += self.dump(elem, cio)
  */
       __pyx_v_length = 5;
 
-      /* "minijson.pyx":493
+      /* "minijson.pyx":484
  *                 cio.write(STRUCT_H.pack(length))
  *                 length = 3
  *             elif length <= 0xFFFFFFFF:             # <<<<<<<<<<<<<<
  *                 cio.write(b'\x10')
  *                 cio.write(STRUCT_L.pack(length))
  */
     }
     __pyx_L22:;
 
-    /* "minijson.pyx":497
+    /* "minijson.pyx":488
  *                 cio.write(STRUCT_L.pack(length))
  *                 length = 5
  *             for elem in data:             # <<<<<<<<<<<<<<
  *                 length += self.dump(elem, cio)
  *             return length
  */
     if (likely(PyList_CheckExact(__pyx_v_data)) || PyTuple_CheckExact(__pyx_v_data)) {
       __pyx_t_2 = __pyx_v_data; __Pyx_INCREF(__pyx_t_2); __pyx_t_9 = 0;
       __pyx_t_16 = NULL;
     } else {
-      __pyx_t_9 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
+      __pyx_t_9 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 488, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_16 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 497, __pyx_L1_error)
+      __pyx_t_16 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 488, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_16)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_11 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_11); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 497, __pyx_L1_error)
+          __pyx_t_11 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_11); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 488, __pyx_L1_error)
           #else
-          __pyx_t_11 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 497, __pyx_L1_error)
+          __pyx_t_11 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 488, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
         } else {
           if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_11 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_11); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 497, __pyx_L1_error)
+          __pyx_t_11 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_11); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 488, __pyx_L1_error)
           #else
-          __pyx_t_11 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 497, __pyx_L1_error)
+          __pyx_t_11 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 488, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
         }
       } else {
         __pyx_t_11 = __pyx_t_16(__pyx_t_2);
         if (unlikely(!__pyx_t_11)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 497, __pyx_L1_error)
+            else __PYX_ERR(0, 488, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_11);
       }
       __Pyx_XDECREF_SET(__pyx_v_elem, __pyx_t_11);
       __pyx_t_11 = 0;
 
-      /* "minijson.pyx":498
+      /* "minijson.pyx":489
  *                 length = 5
  *             for elem in data:
  *                 length += self.dump(elem, cio)             # <<<<<<<<<<<<<<
  *             return length
  *         elif isinstance(data, dict):
  */
-      __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_elem, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 498, __pyx_L1_error)
+      __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_elem, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 489, __pyx_L1_error)
       __pyx_v_length = (__pyx_v_length + __pyx_t_5);
 
-      /* "minijson.pyx":497
+      /* "minijson.pyx":488
  *                 cio.write(STRUCT_L.pack(length))
  *                 length = 5
  *             for elem in data:             # <<<<<<<<<<<<<<
  *                 length += self.dump(elem, cio)
  *             return length
  */
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "minijson.pyx":499
+    /* "minijson.pyx":490
  *             for elem in data:
  *                 length += self.dump(elem, cio)
  *             return length             # <<<<<<<<<<<<<<
  *         elif isinstance(data, dict):
  *             length = len(data)
  */
     __pyx_r = __pyx_v_length;
     goto __pyx_L0;
 
-    /* "minijson.pyx":481
+    /* "minijson.pyx":472
  *                 cio.write(STRUCT_f.pack(data))
  *                 return 5
  *         elif isinstance(data, (tuple, list)):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if length < 16:
  */
   }
 
-  /* "minijson.pyx":500
+  /* "minijson.pyx":491
  *                 length += self.dump(elem, cio)
  *             return length
  *         elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if can_be_encoded_as_a_dict(data):
  */
   __pyx_t_7 = PyDict_Check(__pyx_v_data); 
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "minijson.pyx":501
+    /* "minijson.pyx":492
  *             return length
  *         elif isinstance(data, dict):
  *             length = len(data)             # <<<<<<<<<<<<<<
  *             if can_be_encoded_as_a_dict(data):
  *                 if length < 16:
  */
-    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 501, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 492, __pyx_L1_error)
     __pyx_v_length = __pyx_t_9;
 
-    /* "minijson.pyx":502
+    /* "minijson.pyx":493
  *         elif isinstance(data, dict):
  *             length = len(data)
  *             if can_be_encoded_as_a_dict(data):             # <<<<<<<<<<<<<<
  *                 if length < 16:
  *                     cio.write(bytearray([0b01010000 | length]))
  */
     __pyx_t_8 = (__pyx_f_8minijson_can_be_encoded_as_a_dict(__pyx_v_data) != 0);
     if (__pyx_t_8) {
 
-      /* "minijson.pyx":503
+      /* "minijson.pyx":494
  *             length = len(data)
  *             if can_be_encoded_as_a_dict(data):
  *                 if length < 16:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([0b01010000 | length]))
  *                     length = 1
  */
       __pyx_t_8 = ((__pyx_v_length < 16) != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":504
+        /* "minijson.pyx":495
  *             if can_be_encoded_as_a_dict(data):
  *                 if length < 16:
  *                     cio.write(bytearray([0b01010000 | length]))             # <<<<<<<<<<<<<<
  *                     length = 1
  *                 elif length < 256:
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 504, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_4 = __Pyx_PyInt_From_long((80 | __pyx_v_length)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_long((80 | __pyx_v_length)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 504, __pyx_L1_error)
+        __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GIVEREF(__pyx_t_4);
         PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
         __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -10677,69 +10663,69 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "minijson.pyx":505
+        /* "minijson.pyx":496
  *                 if length < 16:
  *                     cio.write(bytearray([0b01010000 | length]))
  *                     length = 1             # <<<<<<<<<<<<<<
  *                 elif length < 256:
  *                     cio.write(bytearray([11, len(data)]))
  */
         __pyx_v_length = 1;
 
-        /* "minijson.pyx":503
+        /* "minijson.pyx":494
  *             length = len(data)
  *             if can_be_encoded_as_a_dict(data):
  *                 if length < 16:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([0b01010000 | length]))
  *                     length = 1
  */
         goto __pyx_L26;
       }
 
-      /* "minijson.pyx":506
+      /* "minijson.pyx":497
  *                     cio.write(bytearray([0b01010000 | length]))
  *                     length = 1
  *                 elif length < 256:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([11, len(data)]))
  *                     length = 2
  */
       __pyx_t_8 = ((__pyx_v_length < 0x100) != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":507
+        /* "minijson.pyx":498
  *                     length = 1
  *                 elif length < 256:
  *                     cio.write(bytearray([11, len(data)]))             # <<<<<<<<<<<<<<
  *                     length = 2
  *                 elif length < 65536:
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 507, __pyx_L1_error)
-        __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 498, __pyx_L1_error)
+        __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_INCREF(__pyx_int_11);
         __Pyx_GIVEREF(__pyx_int_11);
         PyList_SET_ITEM(__pyx_t_1, 0, __pyx_int_11);
         __Pyx_GIVEREF(__pyx_t_4);
         PyList_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
         __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -10747,101 +10733,101 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 507, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "minijson.pyx":508
+        /* "minijson.pyx":499
  *                 elif length < 256:
  *                     cio.write(bytearray([11, len(data)]))
  *                     length = 2             # <<<<<<<<<<<<<<
  *                 elif length < 65536:
  *                     cio.write(b'\x11')
  */
         __pyx_v_length = 2;
 
-        /* "minijson.pyx":506
+        /* "minijson.pyx":497
  *                     cio.write(bytearray([0b01010000 | length]))
  *                     length = 1
  *                 elif length < 256:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([11, len(data)]))
  *                     length = 2
  */
         goto __pyx_L26;
       }
 
-      /* "minijson.pyx":509
+      /* "minijson.pyx":500
  *                     cio.write(bytearray([11, len(data)]))
  *                     length = 2
  *                 elif length < 65536:             # <<<<<<<<<<<<<<
  *                     cio.write(b'\x11')
  *                     cio.write(STRUCT_H.pack(length))
  */
       __pyx_t_8 = ((__pyx_v_length < 0x10000) != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":510
+        /* "minijson.pyx":501
  *                     length = 2
  *                 elif length < 65536:
  *                     cio.write(b'\x11')             # <<<<<<<<<<<<<<
  *                     cio.write(STRUCT_H.pack(length))
  *                     length = 3
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 510, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 501, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_4, __pyx_kp_b__23) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_b__23);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "minijson.pyx":511
+        /* "minijson.pyx":502
  *                 elif length < 65536:
  *                     cio.write(b'\x11')
  *                     cio.write(STRUCT_H.pack(length))             # <<<<<<<<<<<<<<
  *                     length = 3
  *                 elif length <= 0xFFFFFFFF:
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 511, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 502, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 502, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 511, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 502, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -10849,106 +10835,106 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "minijson.pyx":512
+        /* "minijson.pyx":503
  *                     cio.write(b'\x11')
  *                     cio.write(STRUCT_H.pack(length))
  *                     length = 3             # <<<<<<<<<<<<<<
  *                 elif length <= 0xFFFFFFFF:
  *                     cio.write(b'\x12')
  */
         __pyx_v_length = 3;
 
-        /* "minijson.pyx":509
+        /* "minijson.pyx":500
  *                     cio.write(bytearray([11, len(data)]))
  *                     length = 2
  *                 elif length < 65536:             # <<<<<<<<<<<<<<
  *                     cio.write(b'\x11')
  *                     cio.write(STRUCT_H.pack(length))
  */
         goto __pyx_L26;
       }
 
-      /* "minijson.pyx":513
+      /* "minijson.pyx":504
  *                     cio.write(STRUCT_H.pack(length))
  *                     length = 3
  *                 elif length <= 0xFFFFFFFF:             # <<<<<<<<<<<<<<
  *                     cio.write(b'\x12')
  *                     cio.write(STRUCT_L.pack(length))
  */
-      __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = PyObject_RichCompare(__pyx_t_2, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 513, __pyx_L1_error)
+      __pyx_t_11 = PyObject_RichCompare(__pyx_t_2, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 504, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 513, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 504, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":514
+        /* "minijson.pyx":505
  *                     length = 3
  *                 elif length <= 0xFFFFFFFF:
  *                     cio.write(b'\x12')             # <<<<<<<<<<<<<<
  *                     cio.write(STRUCT_L.pack(length))
  *                     length = 5
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 514, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_b__24) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__24);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 514, __pyx_L1_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 505, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":515
+        /* "minijson.pyx":506
  *                 elif length <= 0xFFFFFFFF:
  *                     cio.write(b'\x12')
  *                     cio.write(STRUCT_L.pack(length))             # <<<<<<<<<<<<<<
  *                     length = 5
- *                 if self.use_strict_order:
+ * 
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 515, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_1 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10956,1068 +10942,994 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 515, __pyx_L1_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":516
+        /* "minijson.pyx":507
  *                     cio.write(b'\x12')
  *                     cio.write(STRUCT_L.pack(length))
  *                     length = 5             # <<<<<<<<<<<<<<
- *                 if self.use_strict_order:
- *                     items = list(data.items())
+ * 
+ *                 data = data.items()
  */
         __pyx_v_length = 5;
 
-        /* "minijson.pyx":513
+        /* "minijson.pyx":504
  *                     cio.write(STRUCT_H.pack(length))
  *                     length = 3
  *                 elif length <= 0xFFFFFFFF:             # <<<<<<<<<<<<<<
  *                     cio.write(b'\x12')
  *                     cio.write(STRUCT_L.pack(length))
  */
       }
       __pyx_L26:;
 
-      /* "minijson.pyx":517
- *                     cio.write(STRUCT_L.pack(length))
+      /* "minijson.pyx":509
  *                     length = 5
+ * 
+ *                 data = data.items()             # <<<<<<<<<<<<<<
+ * 
+ *                 if self.use_strict_order:
+ */
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_items); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 509, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_4);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
+        }
+      }
+      __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 509, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_11);
+      __pyx_t_11 = 0;
+
+      /* "minijson.pyx":511
+ *                 data = data.items()
+ * 
  *                 if self.use_strict_order:             # <<<<<<<<<<<<<<
- *                     items = list(data.items())
- *                     items.sort()
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
  */
       __pyx_t_8 = (__pyx_v_self->use_strict_order != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":518
- *                     length = 5
+        /* "minijson.pyx":512
+ * 
+ *                 if self.use_strict_order:
+ *                     data = list(data)             # <<<<<<<<<<<<<<
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ * 
+ */
+        __pyx_t_11 = PySequence_List(__pyx_v_data); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 512, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_11);
+        __pyx_t_11 = 0;
+
+        /* "minijson.pyx":513
  *                 if self.use_strict_order:
- *                     items = list(data.items())             # <<<<<<<<<<<<<<
- *                     items.sort()
- *                     for field_name, elem in items:
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key             # <<<<<<<<<<<<<<
+ * 
+ *                 for field_name, elem in data:
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_items); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_sort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 513, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 518, __pyx_L1_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 513, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = PySequence_List(__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 518, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __pyx_v_items = ((PyObject*)__pyx_t_2);
-        __pyx_t_2 = 0;
 
-        /* "minijson.pyx":519
- *                 if self.use_strict_order:
- *                     items = list(data.items())
- *                     items.sort()             # <<<<<<<<<<<<<<
- *                     for field_name, elem in items:
- *                         cio.write(bytearray([len(field_name)]))
- */
-        __pyx_t_17 = PyList_Sort(__pyx_v_items); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 519, __pyx_L1_error)
-
-        /* "minijson.pyx":520
- *                     items = list(data.items())
- *                     items.sort()
- *                     for field_name, elem in items:             # <<<<<<<<<<<<<<
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))
+        /* "minijson.pyx":511
+ *                 data = data.items()
+ * 
+ *                 if self.use_strict_order:             # <<<<<<<<<<<<<<
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
  */
-        __pyx_t_2 = __pyx_v_items; __Pyx_INCREF(__pyx_t_2); __pyx_t_9 = 0;
-        for (;;) {
-          if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_2)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_11 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_11); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
-          #else
-          __pyx_t_11 = PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 520, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          #endif
-          if ((likely(PyTuple_CheckExact(__pyx_t_11))) || (PyList_CheckExact(__pyx_t_11))) {
-            PyObject* sequence = __pyx_t_11;
-            Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-            if (unlikely(size != 2)) {
-              if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-              else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-              __PYX_ERR(0, 520, __pyx_L1_error)
-            }
+      }
+
+      /* "minijson.pyx":515
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ * 
+ *                 for field_name, elem in data:             # <<<<<<<<<<<<<<
+ *                     cio.write(bytearray([len(field_name)]))
+ *                     cio.write(field_name.encode('utf-8'))
+ */
+      if (likely(PyList_CheckExact(__pyx_v_data)) || PyTuple_CheckExact(__pyx_v_data)) {
+        __pyx_t_11 = __pyx_v_data; __Pyx_INCREF(__pyx_t_11); __pyx_t_9 = 0;
+        __pyx_t_16 = NULL;
+      } else {
+        __pyx_t_9 = -1; __pyx_t_11 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = Py_TYPE(__pyx_t_11)->tp_iternext; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 515, __pyx_L1_error)
+      }
+      for (;;) {
+        if (likely(!__pyx_t_16)) {
+          if (likely(PyList_CheckExact(__pyx_t_11))) {
+            if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_11)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            if (likely(PyTuple_CheckExact(sequence))) {
-              __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
-              __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
-            } else {
-              __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
-              __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
-            }
-            __Pyx_INCREF(__pyx_t_4);
-            __Pyx_INCREF(__pyx_t_1);
+            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_11, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 515, __pyx_L1_error)
             #else
-            __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 520, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_11, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
             #endif
-            __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           } else {
-            Py_ssize_t index = -1;
-            __pyx_t_10 = PyObject_GetIter(__pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 520, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_10);
-            __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            __pyx_t_18 = Py_TYPE(__pyx_t_10)->tp_iternext;
-            index = 0; __pyx_t_4 = __pyx_t_18(__pyx_t_10); if (unlikely(!__pyx_t_4)) goto __pyx_L30_unpacking_failed;
-            __Pyx_GOTREF(__pyx_t_4);
-            index = 1; __pyx_t_1 = __pyx_t_18(__pyx_t_10); if (unlikely(!__pyx_t_1)) goto __pyx_L30_unpacking_failed;
-            __Pyx_GOTREF(__pyx_t_1);
-            if (__Pyx_IternextUnpackEndCheck(__pyx_t_18(__pyx_t_10), 2) < 0) __PYX_ERR(0, 520, __pyx_L1_error)
-            __pyx_t_18 = NULL;
-            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-            goto __pyx_L31_unpacking_done;
-            __pyx_L30_unpacking_failed:;
-            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-            __pyx_t_18 = NULL;
-            if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-            __PYX_ERR(0, 520, __pyx_L1_error)
-            __pyx_L31_unpacking_done:;
-          }
-          if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 520, __pyx_L1_error)
-          __Pyx_XDECREF_SET(__pyx_v_field_name, ((PyObject*)__pyx_t_4));
-          __pyx_t_4 = 0;
-          __Pyx_XDECREF_SET(__pyx_v_elem, __pyx_t_1);
-          __pyx_t_1 = 0;
-
-          /* "minijson.pyx":521
- *                     items.sort()
- *                     for field_name, elem in items:
- *                         cio.write(bytearray([len(field_name)]))             # <<<<<<<<<<<<<<
- *                         cio.write(field_name.encode('utf-8'))
- *                         length += self.dump(elem, cio)
- */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (unlikely(__pyx_v_field_name == Py_None)) {
-            PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-            __PYX_ERR(0, 521, __pyx_L1_error)
+            if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_11)) break;
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_11, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 515, __pyx_L1_error)
+            #else
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_11, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            #endif
+          }
+        } else {
+          __pyx_t_2 = __pyx_t_16(__pyx_t_11);
+          if (unlikely(!__pyx_t_2)) {
+            PyObject* exc_type = PyErr_Occurred();
+            if (exc_type) {
+              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+              else __PYX_ERR(0, 515, __pyx_L1_error)
+            }
+            break;
+          }
+          __Pyx_GOTREF(__pyx_t_2);
+        }
+        if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
+          PyObject* sequence = __pyx_t_2;
+          Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+          if (unlikely(size != 2)) {
+            if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+            else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+            __PYX_ERR(0, 515, __pyx_L1_error)
+          }
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          if (likely(PyTuple_CheckExact(sequence))) {
+            __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
+          } else {
+            __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
           }
-          __pyx_t_19 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_field_name); if (unlikely(__pyx_t_19 == ((Py_ssize_t)-1))) __PYX_ERR(0, 521, __pyx_L1_error)
-          __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_19); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __Pyx_INCREF(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_1);
+          #else
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 515, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_10 = PyList_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 515, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          #endif
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        } else {
+          Py_ssize_t index = -1;
+          __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 515, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
-          __Pyx_GIVEREF(__pyx_t_4);
-          PyList_SET_ITEM(__pyx_t_10, 0, __pyx_t_4);
-          __pyx_t_4 = 0;
-          __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 521, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __pyx_t_17 = Py_TYPE(__pyx_t_10)->tp_iternext;
+          index = 0; __pyx_t_4 = __pyx_t_17(__pyx_t_10); if (unlikely(!__pyx_t_4)) goto __pyx_L30_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
+          index = 1; __pyx_t_1 = __pyx_t_17(__pyx_t_10); if (unlikely(!__pyx_t_1)) goto __pyx_L30_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_1);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_17(__pyx_t_10), 2) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+          __pyx_t_17 = NULL;
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __pyx_t_10 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-              __Pyx_INCREF(__pyx_t_10);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_1, function);
-            }
-          }
-          __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 521, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          goto __pyx_L31_unpacking_done;
+          __pyx_L30_unpacking_failed:;
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __pyx_t_17 = NULL;
+          if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+          __PYX_ERR(0, 515, __pyx_L1_error)
+          __pyx_L31_unpacking_done:;
+        }
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 515, __pyx_L1_error)
+        __Pyx_XDECREF_SET(__pyx_v_field_name, ((PyObject*)__pyx_t_4));
+        __pyx_t_4 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_elem, __pyx_t_1);
+        __pyx_t_1 = 0;
 
-          /* "minijson.pyx":522
- *                     for field_name, elem in items:
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))             # <<<<<<<<<<<<<<
- *                         length += self.dump(elem, cio)
- *                 else:
+        /* "minijson.pyx":516
+ * 
+ *                 for field_name, elem in data:
+ *                     cio.write(bytearray([len(field_name)]))             # <<<<<<<<<<<<<<
+ *                     cio.write(field_name.encode('utf-8'))
+ *                     length += self.dump(elem, cio)
  */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (unlikely(__pyx_v_field_name == Py_None)) {
-            PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-            __PYX_ERR(0, 522, __pyx_L1_error)
-          }
-          __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_field_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 522, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_10 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-              __Pyx_INCREF(__pyx_t_10);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_1, function);
-            }
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(__pyx_v_field_name == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+          __PYX_ERR(0, 516, __pyx_L1_error)
+        }
+        __pyx_t_18 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_field_name); if (unlikely(__pyx_t_18 == ((Py_ssize_t)-1))) __PYX_ERR(0, 516, __pyx_L1_error)
+        __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_10 = PyList_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_GIVEREF(__pyx_t_4);
+        PyList_SET_ITEM(__pyx_t_10, 0, __pyx_t_4);
+        __pyx_t_4 = 0;
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_10 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+          __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_10)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            __Pyx_INCREF(__pyx_t_10);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_1, function);
           }
-          __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 522, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-
-          /* "minijson.pyx":523
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))
- *                         length += self.dump(elem, cio)             # <<<<<<<<<<<<<<
- *                 else:
- *                     for field_name, elem in data.items():
- */
-          __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_elem, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 523, __pyx_L1_error)
-          __pyx_v_length = (__pyx_v_length + __pyx_t_5);
-
-          /* "minijson.pyx":520
- *                     items = list(data.items())
- *                     items.sort()
- *                     for field_name, elem in items:             # <<<<<<<<<<<<<<
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))
- */
         }
+        __pyx_t_2 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
         /* "minijson.pyx":517
- *                     cio.write(STRUCT_L.pack(length))
- *                     length = 5
- *                 if self.use_strict_order:             # <<<<<<<<<<<<<<
- *                     items = list(data.items())
- *                     items.sort()
- */
-        goto __pyx_L27;
-      }
-
-      /* "minijson.pyx":525
- *                         length += self.dump(elem, cio)
- *                 else:
- *                     for field_name, elem in data.items():             # <<<<<<<<<<<<<<
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))
+ *                 for field_name, elem in data:
+ *                     cio.write(bytearray([len(field_name)]))
+ *                     cio.write(field_name.encode('utf-8'))             # <<<<<<<<<<<<<<
+ *                     length += self.dump(elem, cio)
+ *                 return length
  */
-      /*else*/ {
-        __pyx_t_9 = 0;
-        if (unlikely(__pyx_v_data == Py_None)) {
-          PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-          __PYX_ERR(0, 525, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 517, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(__pyx_v_field_name == Py_None)) {
+          PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
+          __PYX_ERR(0, 517, __pyx_L1_error)
         }
-        __pyx_t_11 = __Pyx_dict_iterator(__pyx_v_data, 0, __pyx_n_s_items, (&__pyx_t_19), (&__pyx_t_5)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 525, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_XDECREF(__pyx_t_2);
-        __pyx_t_2 = __pyx_t_11;
-        __pyx_t_11 = 0;
-        while (1) {
-          __pyx_t_20 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_19, &__pyx_t_9, &__pyx_t_11, &__pyx_t_1, NULL, __pyx_t_5);
-          if (unlikely(__pyx_t_20 == 0)) break;
-          if (unlikely(__pyx_t_20 == -1)) __PYX_ERR(0, 525, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_GOTREF(__pyx_t_1);
-          if (!(likely(PyUnicode_CheckExact(__pyx_t_11))||((__pyx_t_11) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_11)->tp_name), 0))) __PYX_ERR(0, 525, __pyx_L1_error)
-          __Pyx_XDECREF_SET(__pyx_v_field_name, ((PyObject*)__pyx_t_11));
-          __pyx_t_11 = 0;
-          __Pyx_XDECREF_SET(__pyx_v_elem, __pyx_t_1);
-          __pyx_t_1 = 0;
-
-          /* "minijson.pyx":526
- *                 else:
- *                     for field_name, elem in data.items():
- *                         cio.write(bytearray([len(field_name)]))             # <<<<<<<<<<<<<<
- *                         cio.write(field_name.encode('utf-8'))
- *                         length += self.dump(elem, cio)
- */
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 526, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          if (unlikely(__pyx_v_field_name == Py_None)) {
-            PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-            __PYX_ERR(0, 526, __pyx_L1_error)
-          }
-          __pyx_t_21 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_field_name); if (unlikely(__pyx_t_21 == ((Py_ssize_t)-1))) __PYX_ERR(0, 526, __pyx_L1_error)
-          __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_21); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 526, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_10 = PyList_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 526, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __Pyx_GIVEREF(__pyx_t_4);
-          PyList_SET_ITEM(__pyx_t_10, 0, __pyx_t_4);
-          __pyx_t_4 = 0;
-          __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 526, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __pyx_t_10 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-              __Pyx_INCREF(__pyx_t_10);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_11, function);
-            }
+        __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_field_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 517, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_10 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+          __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_10)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            __Pyx_INCREF(__pyx_t_10);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_1, function);
           }
-          __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 526, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        }
+        __pyx_t_2 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 517, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "minijson.pyx":527
- *                     for field_name, elem in data.items():
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))             # <<<<<<<<<<<<<<
- *                         length += self.dump(elem, cio)
+        /* "minijson.pyx":518
+ *                     cio.write(bytearray([len(field_name)]))
+ *                     cio.write(field_name.encode('utf-8'))
+ *                     length += self.dump(elem, cio)             # <<<<<<<<<<<<<<
  *                 return length
+ *             else:
  */
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 527, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          if (unlikely(__pyx_v_field_name == Py_None)) {
-            PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-            __PYX_ERR(0, 527, __pyx_L1_error)
-          }
-          __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_field_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 527, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_10 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-              __Pyx_INCREF(__pyx_t_10);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_11, function);
-            }
-          }
-          __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_4);
-          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 527, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_elem, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 518, __pyx_L1_error)
+        __pyx_v_length = (__pyx_v_length + __pyx_t_5);
 
-          /* "minijson.pyx":528
- *                         cio.write(bytearray([len(field_name)]))
- *                         cio.write(field_name.encode('utf-8'))
- *                         length += self.dump(elem, cio)             # <<<<<<<<<<<<<<
- *                 return length
- *             else:
+        /* "minijson.pyx":515
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ * 
+ *                 for field_name, elem in data:             # <<<<<<<<<<<<<<
+ *                     cio.write(bytearray([len(field_name)]))
+ *                     cio.write(field_name.encode('utf-8'))
  */
-          __pyx_t_20 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_elem, __pyx_v_cio, 0); if (unlikely(__pyx_t_20 == ((int)-1))) __PYX_ERR(0, 528, __pyx_L1_error)
-          __pyx_v_length = (__pyx_v_length + __pyx_t_20);
-        }
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
-      __pyx_L27:;
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":529
- *                         cio.write(field_name.encode('utf-8'))
- *                         length += self.dump(elem, cio)
+      /* "minijson.pyx":519
+ *                     cio.write(field_name.encode('utf-8'))
+ *                     length += self.dump(elem, cio)
  *                 return length             # <<<<<<<<<<<<<<
  *             else:
  *                 if length <= 0xF:
  */
       __pyx_r = __pyx_v_length;
       goto __pyx_L0;
 
-      /* "minijson.pyx":502
+      /* "minijson.pyx":493
  *         elif isinstance(data, dict):
  *             length = len(data)
  *             if can_be_encoded_as_a_dict(data):             # <<<<<<<<<<<<<<
  *                 if length < 16:
  *                     cio.write(bytearray([0b01010000 | length]))
  */
     }
 
-    /* "minijson.pyx":531
+    /* "minijson.pyx":521
  *                 return length
  *             else:
  *                 if length <= 0xF:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([0b01100000 | length]))
  *                     offset = 1
  */
     /*else*/ {
       __pyx_t_8 = ((__pyx_v_length <= 0xF) != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":532
+        /* "minijson.pyx":522
  *             else:
  *                 if length <= 0xF:
  *                     cio.write(bytearray([0b01100000 | length]))             # <<<<<<<<<<<<<<
  *                     offset = 1
  *                 elif length <= 0xFF:
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = __Pyx_PyInt_From_long((96 | __pyx_v_length)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_11 = __Pyx_PyInt_From_long((96 | __pyx_v_length)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 532, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 532, __pyx_L1_error)
+        __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 522, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_GIVEREF(__pyx_t_11);
-        PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_11);
-        __pyx_t_11 = 0;
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 532, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_GIVEREF(__pyx_t_1);
+        PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+        __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_4 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_11);
+        __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 532, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 522, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":533
+        /* "minijson.pyx":523
  *                 if length <= 0xF:
  *                     cio.write(bytearray([0b01100000 | length]))
  *                     offset = 1             # <<<<<<<<<<<<<<
  *                 elif length <= 0xFF:
  *                     cio.write(bytearray([20, length]))
  */
         __Pyx_INCREF(__pyx_int_1);
         __pyx_v_offset = __pyx_int_1;
 
-        /* "minijson.pyx":531
+        /* "minijson.pyx":521
  *                 return length
  *             else:
  *                 if length <= 0xF:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([0b01100000 | length]))
  *                     offset = 1
  */
-        goto __pyx_L34;
+        goto __pyx_L32;
       }
 
-      /* "minijson.pyx":534
+      /* "minijson.pyx":524
  *                     cio.write(bytearray([0b01100000 | length]))
  *                     offset = 1
  *                 elif length <= 0xFF:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([20, length]))
  *                     offset = 2
  */
       __pyx_t_8 = ((__pyx_v_length <= 0xFF) != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":535
+        /* "minijson.pyx":525
  *                     offset = 1
  *                 elif length <= 0xFF:
  *                     cio.write(bytearray([20, length]))             # <<<<<<<<<<<<<<
  *                     offset = 2
  *                 elif length <= 0xFFFF:
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_11 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 535, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 535, __pyx_L1_error)
+        __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_int_20);
         __Pyx_GIVEREF(__pyx_int_20);
         PyList_SET_ITEM(__pyx_t_4, 0, __pyx_int_20);
-        __Pyx_GIVEREF(__pyx_t_11);
-        PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_11);
-        __pyx_t_11 = 0;
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 535, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_GIVEREF(__pyx_t_1);
+        PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+        __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_4 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_11);
+        __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 525, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":536
+        /* "minijson.pyx":526
  *                 elif length <= 0xFF:
  *                     cio.write(bytearray([20, length]))
  *                     offset = 2             # <<<<<<<<<<<<<<
  *                 elif length <= 0xFFFF:
  *                     cio.write(b'\x15')
  */
         __Pyx_INCREF(__pyx_int_2);
         __pyx_v_offset = __pyx_int_2;
 
-        /* "minijson.pyx":534
+        /* "minijson.pyx":524
  *                     cio.write(bytearray([0b01100000 | length]))
  *                     offset = 1
  *                 elif length <= 0xFF:             # <<<<<<<<<<<<<<
  *                     cio.write(bytearray([20, length]))
  *                     offset = 2
  */
-        goto __pyx_L34;
+        goto __pyx_L32;
       }
 
-      /* "minijson.pyx":537
+      /* "minijson.pyx":527
  *                     cio.write(bytearray([20, length]))
  *                     offset = 2
  *                 elif length <= 0xFFFF:             # <<<<<<<<<<<<<<
  *                     cio.write(b'\x15')
  *                     cio.write(STRUCT_H.pack(length))
  */
       __pyx_t_8 = ((__pyx_v_length <= 0xFFFF) != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":538
+        /* "minijson.pyx":528
  *                     offset = 2
  *                 elif length <= 0xFFFF:
  *                     cio.write(b'\x15')             # <<<<<<<<<<<<<<
  *                     cio.write(STRUCT_H.pack(length))
  *                     offset = 3
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_11 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_11)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_11);
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 528, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+          if (likely(__pyx_t_1)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_11, __pyx_kp_b__25) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_b__25);
-        __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_kp_b__25) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__25);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 528, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":539
+        /* "minijson.pyx":529
  *                 elif length <= 0xFFFF:
  *                     cio.write(b'\x15')
  *                     cio.write(STRUCT_H.pack(length))             # <<<<<<<<<<<<<<
  *                     offset = 3
  *                 else:       # Python objects cannot grow to have more than 0xFFFFFFFF members
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 539, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 529, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_H, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 539, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 529, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
+        __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 539, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 529, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_4 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_11);
+        __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 529, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":540
+        /* "minijson.pyx":530
  *                     cio.write(b'\x15')
  *                     cio.write(STRUCT_H.pack(length))
  *                     offset = 3             # <<<<<<<<<<<<<<
  *                 else:       # Python objects cannot grow to have more than 0xFFFFFFFF members
  *                     cio.write(b'\x13')
  */
         __Pyx_INCREF(__pyx_int_3);
         __pyx_v_offset = __pyx_int_3;
 
-        /* "minijson.pyx":537
+        /* "minijson.pyx":527
  *                     cio.write(bytearray([20, length]))
  *                     offset = 2
  *                 elif length <= 0xFFFF:             # <<<<<<<<<<<<<<
  *                     cio.write(b'\x15')
  *                     cio.write(STRUCT_H.pack(length))
  */
-        goto __pyx_L34;
+        goto __pyx_L32;
       }
 
-      /* "minijson.pyx":542
+      /* "minijson.pyx":532
  *                     offset = 3
  *                 else:       # Python objects cannot grow to have more than 0xFFFFFFFF members
  *                     cio.write(b'\x13')             # <<<<<<<<<<<<<<
  *                     cio.write(STRUCT_L.pack(length))
  *                     offset = 5
  */
       /*else*/ {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_11 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_11)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_11);
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 532, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+          if (likely(__pyx_t_1)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_11, __pyx_kp_b__26) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_b__26);
-        __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_kp_b__26) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_b__26);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 532, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":543
+        /* "minijson.pyx":533
  *                 else:       # Python objects cannot grow to have more than 0xFFFFFFFF members
  *                     cio.write(b'\x13')
  *                     cio.write(STRUCT_L.pack(length))             # <<<<<<<<<<<<<<
  *                     offset = 5
- *                 if self.use_strict_order:
+ *                 data = data.items()
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_write); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 533, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_8minijson_STRUCT_L, __pyx_n_s_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 533, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 543, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyInt_From_unsigned_int(__pyx_v_length); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 533, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
+        __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 543, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 533, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_4 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_11);
+        __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 533, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":544
+        /* "minijson.pyx":534
  *                     cio.write(b'\x13')
  *                     cio.write(STRUCT_L.pack(length))
  *                     offset = 5             # <<<<<<<<<<<<<<
+ *                 data = data.items()
  *                 if self.use_strict_order:
- *                     items = list(data.items())
  */
         __Pyx_INCREF(__pyx_int_5);
         __pyx_v_offset = __pyx_int_5;
       }
-      __pyx_L34:;
+      __pyx_L32:;
 
-      /* "minijson.pyx":545
+      /* "minijson.pyx":535
  *                     cio.write(STRUCT_L.pack(length))
  *                     offset = 5
+ *                 data = data.items()             # <<<<<<<<<<<<<<
+ *                 if self.use_strict_order:
+ *                     data = list(data)
+ */
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_items); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_1)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_1);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
+        }
+      }
+      __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 535, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_11);
+      __pyx_t_11 = 0;
+
+      /* "minijson.pyx":536
+ *                     offset = 5
+ *                 data = data.items()
  *                 if self.use_strict_order:             # <<<<<<<<<<<<<<
- *                     items = list(data.items())
- *                     items.sort()
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
  */
       __pyx_t_8 = (__pyx_v_self->use_strict_order != 0);
       if (__pyx_t_8) {
 
-        /* "minijson.pyx":546
- *                     offset = 5
+        /* "minijson.pyx":537
+ *                 data = data.items()
  *                 if self.use_strict_order:
- *                     items = list(data.items())             # <<<<<<<<<<<<<<
- *                     items.sort()
- *                     for key, value in items:
+ *                     data = list(data)             # <<<<<<<<<<<<<<
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ *                 for key, value in data:
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_items); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 546, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_11 = NULL;
-        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
-          if (likely(__pyx_t_11)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-            __Pyx_INCREF(__pyx_t_11);
+        __pyx_t_11 = PySequence_List(__pyx_v_data); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 537, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_11);
+        __pyx_t_11 = 0;
+
+        /* "minijson.pyx":538
+ *                 if self.use_strict_order:
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key             # <<<<<<<<<<<<<<
+ *                 for key, value in data:
+ *                     offset += self.dump(key, cio)
+ */
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_sort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+          if (likely(__pyx_t_1)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+            __Pyx_INCREF(__pyx_t_1);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_1, function);
+            __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
-        __pyx_t_2 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
-        __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 546, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_11 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 538, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_v_items = ((PyObject*)__pyx_t_1);
-        __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "minijson.pyx":547
- *                 if self.use_strict_order:
- *                     items = list(data.items())
- *                     items.sort()             # <<<<<<<<<<<<<<
- *                     for key, value in items:
- *                         offset += self.dump(key, cio)
- */
-        __pyx_t_17 = PyList_Sort(__pyx_v_items); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 547, __pyx_L1_error)
-
-        /* "minijson.pyx":548
- *                     items = list(data.items())
- *                     items.sort()
- *                     for key, value in items:             # <<<<<<<<<<<<<<
- *                         offset += self.dump(key, cio)
- *                         offset += self.dump(value, cio)
- */
-        __pyx_t_1 = __pyx_v_items; __Pyx_INCREF(__pyx_t_1); __pyx_t_19 = 0;
-        for (;;) {
-          if (__pyx_t_19 >= PyList_GET_SIZE(__pyx_t_1)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_19); __Pyx_INCREF(__pyx_t_2); __pyx_t_19++; if (unlikely(0 < 0)) __PYX_ERR(0, 548, __pyx_L1_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_19); __pyx_t_19++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-          if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-            PyObject* sequence = __pyx_t_2;
-            Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-            if (unlikely(size != 2)) {
-              if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-              else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-              __PYX_ERR(0, 548, __pyx_L1_error)
-            }
+        /* "minijson.pyx":536
+ *                     offset = 5
+ *                 data = data.items()
+ *                 if self.use_strict_order:             # <<<<<<<<<<<<<<
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ */
+      }
+
+      /* "minijson.pyx":539
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ *                 for key, value in data:             # <<<<<<<<<<<<<<
+ *                     offset += self.dump(key, cio)
+ *                     offset += self.dump(value, cio)
+ */
+      if (likely(PyList_CheckExact(__pyx_v_data)) || PyTuple_CheckExact(__pyx_v_data)) {
+        __pyx_t_11 = __pyx_v_data; __Pyx_INCREF(__pyx_t_11); __pyx_t_9 = 0;
+        __pyx_t_16 = NULL;
+      } else {
+        __pyx_t_9 = -1; __pyx_t_11 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 539, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_16 = Py_TYPE(__pyx_t_11)->tp_iternext; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 539, __pyx_L1_error)
+      }
+      for (;;) {
+        if (likely(!__pyx_t_16)) {
+          if (likely(PyList_CheckExact(__pyx_t_11))) {
+            if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_11)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            if (likely(PyTuple_CheckExact(sequence))) {
-              __pyx_t_11 = PyTuple_GET_ITEM(sequence, 0); 
-              __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-            } else {
-              __pyx_t_11 = PyList_GET_ITEM(sequence, 0); 
-              __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
-            }
-            __Pyx_INCREF(__pyx_t_11);
-            __Pyx_INCREF(__pyx_t_4);
+            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_11, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 539, __pyx_L1_error)
             #else
-            __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 548, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_11);
-            __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 548, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_4);
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_11, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
             #endif
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           } else {
-            Py_ssize_t index = -1;
-            __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 548, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_10);
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __pyx_t_18 = Py_TYPE(__pyx_t_10)->tp_iternext;
-            index = 0; __pyx_t_11 = __pyx_t_18(__pyx_t_10); if (unlikely(!__pyx_t_11)) goto __pyx_L38_unpacking_failed;
-            __Pyx_GOTREF(__pyx_t_11);
-            index = 1; __pyx_t_4 = __pyx_t_18(__pyx_t_10); if (unlikely(!__pyx_t_4)) goto __pyx_L38_unpacking_failed;
-            __Pyx_GOTREF(__pyx_t_4);
-            if (__Pyx_IternextUnpackEndCheck(__pyx_t_18(__pyx_t_10), 2) < 0) __PYX_ERR(0, 548, __pyx_L1_error)
-            __pyx_t_18 = NULL;
-            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-            goto __pyx_L39_unpacking_done;
-            __pyx_L38_unpacking_failed:;
-            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-            __pyx_t_18 = NULL;
-            if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-            __PYX_ERR(0, 548, __pyx_L1_error)
-            __pyx_L39_unpacking_done:;
+            if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_11)) break;
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_11, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 539, __pyx_L1_error)
+            #else
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_11, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            #endif
+          }
+        } else {
+          __pyx_t_2 = __pyx_t_16(__pyx_t_11);
+          if (unlikely(!__pyx_t_2)) {
+            PyObject* exc_type = PyErr_Occurred();
+            if (exc_type) {
+              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+              else __PYX_ERR(0, 539, __pyx_L1_error)
+            }
+            break;
           }
-          __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_11);
-          __pyx_t_11 = 0;
-          __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_4);
-          __pyx_t_4 = 0;
-
-          /* "minijson.pyx":549
- *                     items.sort()
- *                     for key, value in items:
- *                         offset += self.dump(key, cio)             # <<<<<<<<<<<<<<
- *                         offset += self.dump(value, cio)
- *                 else:
- */
-          __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_key, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 549, __pyx_L1_error)
-          __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 549, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_offset, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 549, __pyx_L1_error)
+        }
+        if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
+          PyObject* sequence = __pyx_t_2;
+          Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+          if (unlikely(size != 2)) {
+            if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+            else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+            __PYX_ERR(0, 539, __pyx_L1_error)
+          }
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          if (likely(PyTuple_CheckExact(sequence))) {
+            __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
+          } else {
+            __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
+          }
+          __Pyx_INCREF(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_4);
+          #else
+          __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 539, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
+          #endif
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __Pyx_DECREF_SET(__pyx_v_offset, __pyx_t_4);
-          __pyx_t_4 = 0;
-
-          /* "minijson.pyx":550
- *                     for key, value in items:
- *                         offset += self.dump(key, cio)
- *                         offset += self.dump(value, cio)             # <<<<<<<<<<<<<<
- *                 else:
- *                     for key, value in data.items():
- */
-          __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_value, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 550, __pyx_L1_error)
-          __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
+        } else {
+          Py_ssize_t index = -1;
+          __pyx_t_10 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 539, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_10);
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __pyx_t_17 = Py_TYPE(__pyx_t_10)->tp_iternext;
+          index = 0; __pyx_t_1 = __pyx_t_17(__pyx_t_10); if (unlikely(!__pyx_t_1)) goto __pyx_L36_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_1);
+          index = 1; __pyx_t_4 = __pyx_t_17(__pyx_t_10); if (unlikely(!__pyx_t_4)) goto __pyx_L36_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_offset, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_DECREF_SET(__pyx_v_offset, __pyx_t_2);
-          __pyx_t_2 = 0;
-
-          /* "minijson.pyx":548
- *                     items = list(data.items())
- *                     items.sort()
- *                     for key, value in items:             # <<<<<<<<<<<<<<
- *                         offset += self.dump(key, cio)
- *                         offset += self.dump(value, cio)
- */
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_17(__pyx_t_10), 2) < 0) __PYX_ERR(0, 539, __pyx_L1_error)
+          __pyx_t_17 = NULL;
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          goto __pyx_L37_unpacking_done;
+          __pyx_L36_unpacking_failed:;
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __pyx_t_17 = NULL;
+          if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+          __PYX_ERR(0, 539, __pyx_L1_error)
+          __pyx_L37_unpacking_done:;
         }
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
+        __pyx_t_1 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_4);
+        __pyx_t_4 = 0;
 
-        /* "minijson.pyx":545
- *                     cio.write(STRUCT_L.pack(length))
- *                     offset = 5
- *                 if self.use_strict_order:             # <<<<<<<<<<<<<<
- *                     items = list(data.items())
- *                     items.sort()
+        /* "minijson.pyx":540
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ *                 for key, value in data:
+ *                     offset += self.dump(key, cio)             # <<<<<<<<<<<<<<
+ *                     offset += self.dump(value, cio)
+ *                 return offset
  */
-        goto __pyx_L35;
-      }
+        __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_key, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 540, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_offset, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 540, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF_SET(__pyx_v_offset, __pyx_t_4);
+        __pyx_t_4 = 0;
 
-      /* "minijson.pyx":552
- *                         offset += self.dump(value, cio)
- *                 else:
- *                     for key, value in data.items():             # <<<<<<<<<<<<<<
- *                         offset += self.dump(key, cio)
- *                         offset += self.dump(value, cio)
+        /* "minijson.pyx":541
+ *                 for key, value in data:
+ *                     offset += self.dump(key, cio)
+ *                     offset += self.dump(value, cio)             # <<<<<<<<<<<<<<
+ *                 return offset
+ *         else:
  */
-      /*else*/ {
-        __pyx_t_19 = 0;
-        if (unlikely(__pyx_v_data == Py_None)) {
-          PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-          __PYX_ERR(0, 552, __pyx_L1_error)
-        }
-        __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_data, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_value, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 541, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 541, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_offset, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 541, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_XDECREF(__pyx_t_1);
-        __pyx_t_1 = __pyx_t_2;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF_SET(__pyx_v_offset, __pyx_t_2);
         __pyx_t_2 = 0;
-        while (1) {
-          __pyx_t_20 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_9, &__pyx_t_19, &__pyx_t_2, &__pyx_t_4, NULL, __pyx_t_5);
-          if (unlikely(__pyx_t_20 == 0)) break;
-          if (unlikely(__pyx_t_20 == -1)) __PYX_ERR(0, 552, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_2);
-          __pyx_t_2 = 0;
-          __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_4);
-          __pyx_t_4 = 0;
-
-          /* "minijson.pyx":553
- *                 else:
- *                     for key, value in data.items():
- *                         offset += self.dump(key, cio)             # <<<<<<<<<<<<<<
- *                         offset += self.dump(value, cio)
- *                 return offset
- */
-          __pyx_t_20 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_key, __pyx_v_cio, 0); if (unlikely(__pyx_t_20 == ((int)-1))) __PYX_ERR(0, 553, __pyx_L1_error)
-          __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_offset, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_DECREF_SET(__pyx_v_offset, __pyx_t_2);
-          __pyx_t_2 = 0;
 
-          /* "minijson.pyx":554
- *                     for key, value in data.items():
- *                         offset += self.dump(key, cio)
- *                         offset += self.dump(value, cio)             # <<<<<<<<<<<<<<
- *                 return offset
- *         else:
+        /* "minijson.pyx":539
+ *                     data = list(data)
+ *                     data.sort()  # sort implicitly will sort it by first value, which is the key
+ *                 for key, value in data:             # <<<<<<<<<<<<<<
+ *                     offset += self.dump(key, cio)
+ *                     offset += self.dump(value, cio)
  */
-          __pyx_t_20 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_value, __pyx_v_cio, 0); if (unlikely(__pyx_t_20 == ((int)-1))) __PYX_ERR(0, 554, __pyx_L1_error)
-          __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 554, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_v_offset, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 554, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __Pyx_DECREF_SET(__pyx_v_offset, __pyx_t_4);
-          __pyx_t_4 = 0;
-        }
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __pyx_L35:;
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "minijson.pyx":555
- *                         offset += self.dump(key, cio)
- *                         offset += self.dump(value, cio)
+      /* "minijson.pyx":542
+ *                     offset += self.dump(key, cio)
+ *                     offset += self.dump(value, cio)
  *                 return offset             # <<<<<<<<<<<<<<
  *         else:
  *             v = self.default(data)
  */
-      __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_offset); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_offset); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 542, __pyx_L1_error)
       __pyx_r = __pyx_t_5;
       goto __pyx_L0;
     }
 
-    /* "minijson.pyx":500
+    /* "minijson.pyx":491
  *                 length += self.dump(elem, cio)
  *             return length
  *         elif isinstance(data, dict):             # <<<<<<<<<<<<<<
  *             length = len(data)
  *             if can_be_encoded_as_a_dict(data):
  */
   }
 
-  /* "minijson.pyx":557
+  /* "minijson.pyx":544
  *                 return offset
  *         else:
  *             v = self.default(data)             # <<<<<<<<<<<<<<
  *             if not is_jsonable(v):
  *                 raise EncodingError('default returned a non-JSONable value!')
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_default); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_v_v = __pyx_t_1;
-    __pyx_t_1 = 0;
+    __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 544, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_v_v = __pyx_t_11;
+    __pyx_t_11 = 0;
 
-    /* "minijson.pyx":558
+    /* "minijson.pyx":545
  *         else:
  *             v = self.default(data)
  *             if not is_jsonable(v):             # <<<<<<<<<<<<<<
  *                 raise EncodingError('default returned a non-JSONable value!')
  *             return self.dump(v, cio)
  */
     __pyx_t_8 = ((!(__pyx_f_8minijson_is_jsonable(__pyx_v_v) != 0)) != 0);
     if (unlikely(__pyx_t_8)) {
 
-      /* "minijson.pyx":559
+      /* "minijson.pyx":546
  *             v = self.default(data)
  *             if not is_jsonable(v):
  *                 raise EncodingError('default returned a non-JSONable value!')             # <<<<<<<<<<<<<<
  *             return self.dump(v, cio)
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_EncodingError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 559, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_2)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_2);
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_EncodingError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
-      __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_kp_u_default_returned_a_non_JSONable) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_default_returned_a_non_JSONable);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 559, __pyx_L1_error)
+      __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_default_returned_a_non_JSONable) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_default_returned_a_non_JSONable);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 546, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_Raise(__pyx_t_11, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __PYX_ERR(0, 546, __pyx_L1_error)
 
-      /* "minijson.pyx":558
+      /* "minijson.pyx":545
  *         else:
  *             v = self.default(data)
  *             if not is_jsonable(v):             # <<<<<<<<<<<<<<
  *                 raise EncodingError('default returned a non-JSONable value!')
  *             return self.dump(v, cio)
  */
     }
 
-    /* "minijson.pyx":560
+    /* "minijson.pyx":547
  *             if not is_jsonable(v):
  *                 raise EncodingError('default returned a non-JSONable value!')
  *             return self.dump(v, cio)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_v, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_5 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_self->__pyx_vtab)->dump(__pyx_v_self, __pyx_v_v, __pyx_v_cio, 0); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 547, __pyx_L1_error)
     __pyx_r = __pyx_t_5;
     goto __pyx_L0;
   }
   __pyx_L3:;
 
-  /* "minijson.pyx":380
+  /* "minijson.pyx":371
  *         return cio.getvalue()
  * 
  *     cpdef int dump(self, object data, cio: io.BytesIO) except -1:             # <<<<<<<<<<<<<<
  *         """
  *         Write an object to a stream
  */
 
@@ -12033,20 +11945,20 @@
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_AddTraceback("minijson.MiniJSONEncoder.dump", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_field_name);
   __Pyx_XDECREF(__pyx_v_b_data);
-  __Pyx_XDECREF(__pyx_v_items);
   __Pyx_XDECREF(__pyx_v_elem);
   __Pyx_XDECREF(__pyx_v_offset);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF(__pyx_v_v);
+  __Pyx_XDECREF(__pyx_v_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8minijson_15MiniJSONEncoder_9dump(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_8minijson_15MiniJSONEncoder_8dump[] = "\n        Write an object to a stream\n    \n        :param data: object to write\n        :param cio: stream to write to\n        :return: amount of bytes written\n        :raises EncodingError: invalid data\n        ";
@@ -12078,32 +11990,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cio)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dump", 1, 2, 2, 1); __PYX_ERR(0, 380, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dump", 1, 2, 2, 1); __PYX_ERR(0, 371, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dump") < 0)) __PYX_ERR(0, 380, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dump") < 0)) __PYX_ERR(0, 371, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_data = values[0];
     __pyx_v_cio = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dump", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 380, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dump", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 371, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.MiniJSONEncoder.dump", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_15MiniJSONEncoder_8dump(((struct __pyx_obj_8minijson_MiniJSONEncoder *)__pyx_v_self), __pyx_v_data, __pyx_v_cio);
 
@@ -12118,16 +12030,16 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dump", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8minijson_15MiniJSONEncoder_dump(__pyx_v_self, __pyx_v_data, __pyx_v_cio, 1); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 380, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_15MiniJSONEncoder_dump(__pyx_v_self, __pyx_v_data, __pyx_v_cio, 1); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12136,15 +12048,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":334
+/* "minijson.pyx":325
  *     cdef:
  *         object _default
  *         public bint use_double             # <<<<<<<<<<<<<<
  *         public bint use_strict_order
  * 
  */
 
@@ -12166,15 +12078,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->use_double); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->use_double); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12204,29 +12116,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L1_error)
   __pyx_v_self->use_double = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("minijson.MiniJSONEncoder.use_double.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":335
+/* "minijson.pyx":326
  *         object _default
  *         public bint use_double
  *         public bint use_strict_order             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, default: tp.Optional[None] = None,
  */
 
@@ -12248,15 +12160,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->use_strict_order); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->use_strict_order); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12286,15 +12198,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
   __pyx_v_self->use_strict_order = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("minijson.MiniJSONEncoder.use_strict_order.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -12603,15 +12515,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":563
+/* "minijson.pyx":550
  * 
  * 
  * cpdef int dump(object data, cio: io.BytesIO, default: tp.Optional[tp.Callable] = None) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Write an object to a stream.
  */
 
@@ -12630,49 +12542,49 @@
   __Pyx_RefNannySetupContext("dump", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default = __pyx_optional_args->__pyx_default;
     }
   }
 
-  /* "minijson.pyx":580
+  /* "minijson.pyx":567
  *     """
  *     global float_encoding_mode
  *     cdef MiniJSONEncoder mje = MiniJSONEncoder(default, float_encoding_mode == 1)             # <<<<<<<<<<<<<<
  *     return mje.dump(data, cio)
  * 
  */
-  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_8minijson_float_encoding_mode == 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_8minijson_float_encoding_mode == 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_default);
   __Pyx_GIVEREF(__pyx_v_default);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_default);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8minijson_MiniJSONEncoder), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8minijson_MiniJSONEncoder), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_mje = ((struct __pyx_obj_8minijson_MiniJSONEncoder *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "minijson.pyx":581
+  /* "minijson.pyx":568
  *     global float_encoding_mode
  *     cdef MiniJSONEncoder mje = MiniJSONEncoder(default, float_encoding_mode == 1)
  *     return mje.dump(data, cio)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_mje->__pyx_vtab)->dump(__pyx_v_mje, __pyx_v_data, __pyx_v_cio, 0); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_8minijson_MiniJSONEncoder *)__pyx_v_mje->__pyx_vtab)->dump(__pyx_v_mje, __pyx_v_data, __pyx_v_cio, 0); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 568, __pyx_L1_error)
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "minijson.pyx":563
+  /* "minijson.pyx":550
  * 
  * 
  * cpdef int dump(object data, cio: io.BytesIO, default: tp.Optional[tp.Callable] = None) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Write an object to a stream.
  */
 
@@ -12723,25 +12635,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cio)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dump", 0, 2, 3, 1); __PYX_ERR(0, 563, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dump", 0, 2, 3, 1); __PYX_ERR(0, 550, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_default);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dump") < 0)) __PYX_ERR(0, 563, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dump") < 0)) __PYX_ERR(0, 550, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -12751,15 +12663,15 @@
     }
     __pyx_v_data = values[0];
     __pyx_v_cio = values[1];
     __pyx_v_default = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dump", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 563, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dump", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 550, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.dump", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_8dump(__pyx_self, __pyx_v_data, __pyx_v_cio, __pyx_v_default);
 
@@ -12777,16 +12689,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dump", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.__pyx_default = __pyx_v_default;
-  __pyx_t_1 = __pyx_f_8minijson_dump(__pyx_v_data, __pyx_v_cio, 0, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 563, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_dump(__pyx_v_data, __pyx_v_cio, 0, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12795,15 +12707,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":584
+/* "minijson.pyx":571
  * 
  * 
  * cpdef bytes dumps(object data, default: tp.Optional[tp.Callable] = None):             # <<<<<<<<<<<<<<
  *     """
  *     Serialize given data to a MiniJSON representation.
  */
 
@@ -12824,86 +12736,86 @@
   __Pyx_RefNannySetupContext("dumps", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default = __pyx_optional_args->__pyx_default;
     }
   }
 
-  /* "minijson.pyx":599
+  /* "minijson.pyx":586
  *     :raises EncodingError: object not serializable
  *     """
  *     cio = io.BytesIO()             # <<<<<<<<<<<<<<
  *     dump(data, cio, default)
  *     return cio.getvalue()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_io); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_io); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_BytesIO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cio = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "minijson.pyx":600
+  /* "minijson.pyx":587
  *     """
  *     cio = io.BytesIO()
  *     dump(data, cio, default)             # <<<<<<<<<<<<<<
  *     return cio.getvalue()
  * 
  */
   __pyx_t_5.__pyx_n = 1;
   __pyx_t_5.__pyx_default = __pyx_v_default;
-  __pyx_t_4 = __pyx_f_8minijson_dump(__pyx_v_data, __pyx_v_cio, 0, &__pyx_t_5); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_8minijson_dump(__pyx_v_data, __pyx_v_cio, 0, &__pyx_t_5); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 587, __pyx_L1_error)
 
-  /* "minijson.pyx":601
+  /* "minijson.pyx":588
  *     cio = io.BytesIO()
  *     dump(data, cio, default)
  *     return cio.getvalue()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_getvalue); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cio, __pyx_n_s_getvalue); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 588, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":584
+  /* "minijson.pyx":571
  * 
  * 
  * cpdef bytes dumps(object data, default: tp.Optional[tp.Callable] = None):             # <<<<<<<<<<<<<<
  *     """
  *     Serialize given data to a MiniJSON representation.
  */
 
@@ -12957,15 +12869,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_default);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dumps") < 0)) __PYX_ERR(0, 584, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dumps") < 0)) __PYX_ERR(0, 571, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -12973,15 +12885,15 @@
       }
     }
     __pyx_v_data = values[0];
     __pyx_v_default = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dumps", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 584, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dumps", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 571, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.dumps", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_10dumps(__pyx_self, __pyx_v_data, __pyx_v_default);
 
@@ -12998,15 +12910,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dumps", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.__pyx_default = __pyx_v_default;
-  __pyx_t_1 = __pyx_f_8minijson_dumps(__pyx_v_data, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 584, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_dumps(__pyx_v_data, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 571, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13015,15 +12927,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":604
+/* "minijson.pyx":591
  * 
  * 
  * cpdef bytes dumps_object(object data, default: tp.Optional[tp.Callable] = None):             # <<<<<<<<<<<<<<
  *     """
  *     Dump an object's :code:`__dict__`.
  */
 
@@ -13041,34 +12953,34 @@
   __Pyx_RefNannySetupContext("dumps_object", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default = __pyx_optional_args->__pyx_default;
     }
   }
 
-  /* "minijson.pyx":621
+  /* "minijson.pyx":608
  *     :raises EncodingError: encoding error
  *     """
  *     return dumps(data.__dict__, default)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3.__pyx_n = 1;
   __pyx_t_3.__pyx_default = __pyx_v_default;
-  __pyx_t_2 = __pyx_f_8minijson_dumps(__pyx_t_1, 0, &__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8minijson_dumps(__pyx_t_1, 0, &__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":604
+  /* "minijson.pyx":591
  * 
  * 
  * cpdef bytes dumps_object(object data, default: tp.Optional[tp.Callable] = None):             # <<<<<<<<<<<<<<
  *     """
  *     Dump an object's :code:`__dict__`.
  */
 
@@ -13120,15 +13032,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_default);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dumps_object") < 0)) __PYX_ERR(0, 604, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dumps_object") < 0)) __PYX_ERR(0, 591, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -13136,15 +13048,15 @@
       }
     }
     __pyx_v_data = values[0];
     __pyx_v_default = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dumps_object", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 604, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dumps_object", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 591, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.dumps_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_12dumps_object(__pyx_self, __pyx_v_data, __pyx_v_default);
 
@@ -13161,15 +13073,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dumps_object", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.__pyx_default = __pyx_v_default;
-  __pyx_t_1 = __pyx_f_8minijson_dumps_object(__pyx_v_data, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_dumps_object(__pyx_v_data, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13178,15 +13090,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "minijson.pyx":624
+/* "minijson.pyx":611
  * 
  * 
  * cpdef object loads_object(data, object obj_class):             # <<<<<<<<<<<<<<
  *     """
  *     Load a dict from a bytestream, unserialize it and use it as a kwargs to instantiate
  */
 
@@ -13206,15 +13118,15 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("loads_object", 0);
 
-  /* "minijson.pyx":636
+  /* "minijson.pyx":623
  *     """
  *     cdef dict kwargs
  *     try:             # <<<<<<<<<<<<<<
  *          kwargs = loads(data)
  *     except TypeError:
  */
   {
@@ -13222,122 +13134,122 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "minijson.pyx":637
+      /* "minijson.pyx":624
  *     cdef dict kwargs
  *     try:
  *          kwargs = loads(data)             # <<<<<<<<<<<<<<
  *     except TypeError:
  *         raise DecodingError('Expected an object to be of type dict!')
  */
-      __pyx_t_4 = __pyx_f_8minijson_loads(__pyx_v_data, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 637, __pyx_L3_error)
+      __pyx_t_4 = __pyx_f_8minijson_loads(__pyx_v_data, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 624, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(PyDict_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 637, __pyx_L3_error)
+      if (!(likely(PyDict_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 624, __pyx_L3_error)
       __pyx_v_kwargs = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "minijson.pyx":636
+      /* "minijson.pyx":623
  *     """
  *     cdef dict kwargs
  *     try:             # <<<<<<<<<<<<<<
  *          kwargs = loads(data)
  *     except TypeError:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "minijson.pyx":638
+    /* "minijson.pyx":625
  *     try:
  *          kwargs = loads(data)
  *     except TypeError:             # <<<<<<<<<<<<<<
  *         raise DecodingError('Expected an object to be of type dict!')
  *     return obj_class(**kwargs)
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
     if (__pyx_t_5) {
       __Pyx_AddTraceback("minijson.loads_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 638, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 625, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "minijson.pyx":639
+      /* "minijson.pyx":626
  *          kwargs = loads(data)
  *     except TypeError:
  *         raise DecodingError('Expected an object to be of type dict!')             # <<<<<<<<<<<<<<
  *     return obj_class(**kwargs)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 639, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_DecodingError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 626, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_kp_u_Expected_an_object_to_be_of_type) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_kp_u_Expected_an_object_to_be_of_type);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 639, __pyx_L5_except_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 626, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 639, __pyx_L5_except_error)
+      __PYX_ERR(0, 626, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "minijson.pyx":636
+    /* "minijson.pyx":623
  *     """
  *     cdef dict kwargs
  *     try:             # <<<<<<<<<<<<<<
  *          kwargs = loads(data)
  *     except TypeError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "minijson.pyx":640
+  /* "minijson.pyx":627
  *     except TypeError:
  *         raise DecodingError('Expected an object to be of type dict!')
  *     return obj_class(**kwargs)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-    __PYX_ERR(0, 640, __pyx_L1_error)
+    __PYX_ERR(0, 627, __pyx_L1_error)
   }
-  __pyx_t_7 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_7 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_v_obj_class, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_v_obj_class, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "minijson.pyx":624
+  /* "minijson.pyx":611
  * 
  * 
  * cpdef object loads_object(data, object obj_class):             # <<<<<<<<<<<<<<
  *     """
  *     Load a dict from a bytestream, unserialize it and use it as a kwargs to instantiate
  */
 
@@ -13389,32 +13301,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj_class)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("loads_object", 1, 2, 2, 1); __PYX_ERR(0, 624, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("loads_object", 1, 2, 2, 1); __PYX_ERR(0, 611, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "loads_object") < 0)) __PYX_ERR(0, 624, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "loads_object") < 0)) __PYX_ERR(0, 611, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_data = values[0];
     __pyx_v_obj_class = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("loads_object", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 624, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("loads_object", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 611, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("minijson.loads_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8minijson_14loads_object(__pyx_self, __pyx_v_data, __pyx_v_obj_class);
 
@@ -13428,15 +13340,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("loads_object", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8minijson_loads_object(__pyx_v_data, __pyx_v_obj_class, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 624, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8minijson_loads_object(__pyx_v_data, __pyx_v_obj_class, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14172,14 +14084,15 @@
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_should_double_be_used, __pyx_k_should_double_be_used, sizeof(__pyx_k_should_double_be_used), 0, 0, 1, 1},
   {&__pyx_n_s_signed, __pyx_k_signed, sizeof(__pyx_k_signed), 0, 0, 1, 1},
+  {&__pyx_n_s_sort, __pyx_k_sort, sizeof(__pyx_k_sort), 0, 0, 1, 1},
   {&__pyx_n_s_starting_position, __pyx_k_starting_position, sizeof(__pyx_k_starting_position), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_to_bytes, __pyx_k_to_bytes, sizeof(__pyx_k_to_bytes), 0, 0, 1, 1},
   {&__pyx_n_s_tp, __pyx_k_tp, sizeof(__pyx_k_tp), 0, 0, 1, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
@@ -14191,67 +14104,67 @@
   {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 6, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 66, __pyx_L1_error)
   __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(0, 91, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 281, __pyx_L1_error)
-  __pyx_builtin_OverflowError = __Pyx_GetBuiltinName(__pyx_n_s_OverflowError); if (!__pyx_builtin_OverflowError) __PYX_ERR(0, 468, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_builtin_OverflowError = __Pyx_GetBuiltinName(__pyx_n_s_OverflowError); if (!__pyx_builtin_OverflowError) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 625, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "minijson.pyx":205
+  /* "minijson.pyx":196
  *             return offset+2, e_list
  *         elif value_type == 8:
  *             return 1, None             # <<<<<<<<<<<<<<
  *         elif value_type == 9:
  *             return 5, *STRUCT_f.unpack(data[starting_position+1:starting_position+5])
  */
-  __pyx_tuple_ = PyTuple_Pack(2, __pyx_int_1, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 205, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(2, __pyx_int_1, Py_None); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "minijson.pyx":260
+  /* "minijson.pyx":251
  *             return offset+3, e_dict
  *         elif value_type == 22:
  *             return 1, True             # <<<<<<<<<<<<<<
  *         elif value_type == 23:
  *             return 1, False
  */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_int_1, Py_True); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_int_1, Py_True); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "minijson.pyx":262
+  /* "minijson.pyx":253
  *             return 1, True
  *         elif value_type == 23:
  *             return 1, False             # <<<<<<<<<<<<<<
  *         elif value_type == 24:
  *             length = data[starting_position+1]
  */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_int_1, Py_False); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_int_1, Py_False); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "minijson.pyx":452
+  /* "minijson.pyx":443
  *             elif 0 <= data <= 0xFFFFFF:         # unsigned 3byte, type 12
  *                 cio.write(b'\x0C')
  *                 cio.write(STRUCT_L.pack(data)[1:])             # <<<<<<<<<<<<<<
  *                 return 4
  *             elif -2147483648 <= data <= 2147483647:     # signed int, type 1
  */
-  __pyx_slice__16 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__16)) __PYX_ERR(0, 452, __pyx_L1_error)
+  __pyx_slice__16 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__16)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__16);
   __Pyx_GIVEREF(__pyx_slice__16);
 
   /* "minijson.pyx":6
  * 
  * 
  * class MiniJSONError(ValueError):             # <<<<<<<<<<<<<<
@@ -14432,24 +14345,24 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_8minijson_MiniJSONEncoder = &__pyx_vtable_8minijson_MiniJSONEncoder;
   __pyx_vtable_8minijson_MiniJSONEncoder.dump = (int (*)(struct __pyx_obj_8minijson_MiniJSONEncoder *, PyObject *, PyObject *, int __pyx_skip_dispatch))__pyx_f_8minijson_15MiniJSONEncoder_dump;
-  if (PyType_Ready(&__pyx_type_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8minijson_MiniJSONEncoder.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8minijson_MiniJSONEncoder.tp_dictoffset && __pyx_type_8minijson_MiniJSONEncoder.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8minijson_MiniJSONEncoder.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_8minijson_MiniJSONEncoder.tp_dict, __pyx_vtabptr_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MiniJSONEncoder, (PyObject *)&__pyx_type_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_8minijson_MiniJSONEncoder.tp_dict, __pyx_vtabptr_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MiniJSONEncoder, (PyObject *)&__pyx_type_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8minijson_MiniJSONEncoder) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
   __pyx_ptype_8minijson_MiniJSONEncoder = &__pyx_type_8minijson_MiniJSONEncoder;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -16696,28 +16609,14 @@
         
     }
     #endif
     return (inplace ? PyNumber_InPlaceLshift : PyNumber_Lshift)(op1, op2);
 }
 #endif
 
-/* bytes_index */
-static CYTHON_INLINE char __Pyx_PyBytes_GetItemInt(PyObject* bytes, Py_ssize_t index, int check_bounds) {
-    if (index < 0)
-        index += PyBytes_GET_SIZE(bytes);
-    if (check_bounds) {
-        Py_ssize_t size = PyBytes_GET_SIZE(bytes);
-        if (unlikely(!__Pyx_is_valid_index(index, size))) {
-            PyErr_SetString(PyExc_IndexError, "string index out of range");
-            return (char) -1;
-        }
-    }
-    return PyBytes_AS_STRING(bytes)[index];
-}
-
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
@@ -18409,558 +18308,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
                                      little, !is_unsigned);
     }
 }
 
-/* CIntFromPy */
-static CYTHON_INLINE unsigned short __Pyx_PyInt_As_unsigned_short(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned short neg_one = (unsigned short) -1, const_zero = (unsigned short) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(unsigned short) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(unsigned short, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (unsigned short) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned short) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned short, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(unsigned short) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) >= 2 * PyLong_SHIFT) {
-                            return (unsigned short) (((((unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(unsigned short) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) >= 3 * PyLong_SHIFT) {
-                            return (unsigned short) (((((((unsigned short)digits[2]) << PyLong_SHIFT) | (unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(unsigned short) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) >= 4 * PyLong_SHIFT) {
-                            return (unsigned short) (((((((((unsigned short)digits[3]) << PyLong_SHIFT) | (unsigned short)digits[2]) << PyLong_SHIFT) | (unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (unsigned short) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(unsigned short) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned short, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(unsigned short) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned short, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned short) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(unsigned short, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned short,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(unsigned short) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) - 1 > 2 * PyLong_SHIFT) {
-                            return (unsigned short) (((unsigned short)-1)*(((((unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(unsigned short) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) - 1 > 2 * PyLong_SHIFT) {
-                            return (unsigned short) ((((((unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(unsigned short) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) - 1 > 3 * PyLong_SHIFT) {
-                            return (unsigned short) (((unsigned short)-1)*(((((((unsigned short)digits[2]) << PyLong_SHIFT) | (unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(unsigned short) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) - 1 > 3 * PyLong_SHIFT) {
-                            return (unsigned short) ((((((((unsigned short)digits[2]) << PyLong_SHIFT) | (unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(unsigned short) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) - 1 > 4 * PyLong_SHIFT) {
-                            return (unsigned short) (((unsigned short)-1)*(((((((((unsigned short)digits[3]) << PyLong_SHIFT) | (unsigned short)digits[2]) << PyLong_SHIFT) | (unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(unsigned short) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned short, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned short) - 1 > 4 * PyLong_SHIFT) {
-                            return (unsigned short) ((((((((((unsigned short)digits[3]) << PyLong_SHIFT) | (unsigned short)digits[2]) << PyLong_SHIFT) | (unsigned short)digits[1]) << PyLong_SHIFT) | (unsigned short)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(unsigned short) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned short, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(unsigned short) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned short, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            unsigned short val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (unsigned short) -1;
-        }
-    } else {
-        unsigned short val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (unsigned short) -1;
-        val = __Pyx_PyInt_As_unsigned_short(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to unsigned short");
-    return (unsigned short) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to unsigned short");
-    return (unsigned short) -1;
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_short(unsigned short value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned short neg_one = (unsigned short) -1, const_zero = (unsigned short) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(unsigned short) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(unsigned short) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned short) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(unsigned short) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned short) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(unsigned short),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const short neg_one = (short) -1, const_zero = (short) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(short) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(short) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(short) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(short) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(short) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(short),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntFromPy */
-static CYTHON_INLINE unsigned char __Pyx_PyInt_As_unsigned_char(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned char neg_one = (unsigned char) -1, const_zero = (unsigned char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(unsigned char) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(unsigned char, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (unsigned char) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned char) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned char, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(unsigned char) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) >= 2 * PyLong_SHIFT) {
-                            return (unsigned char) (((((unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(unsigned char) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) >= 3 * PyLong_SHIFT) {
-                            return (unsigned char) (((((((unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(unsigned char) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) >= 4 * PyLong_SHIFT) {
-                            return (unsigned char) (((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (unsigned char) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(unsigned char) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned char, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(unsigned char) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned char, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned char) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(unsigned char, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned char,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(unsigned char) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) - 1 > 2 * PyLong_SHIFT) {
-                            return (unsigned char) (((unsigned char)-1)*(((((unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(unsigned char) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) - 1 > 2 * PyLong_SHIFT) {
-                            return (unsigned char) ((((((unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(unsigned char) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) - 1 > 3 * PyLong_SHIFT) {
-                            return (unsigned char) (((unsigned char)-1)*(((((((unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(unsigned char) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) - 1 > 3 * PyLong_SHIFT) {
-                            return (unsigned char) ((((((((unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(unsigned char) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) - 1 > 4 * PyLong_SHIFT) {
-                            return (unsigned char) (((unsigned char)-1)*(((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(unsigned char) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned char) - 1 > 4 * PyLong_SHIFT) {
-                            return (unsigned char) ((((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(unsigned char) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned char, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(unsigned char) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(unsigned char, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            unsigned char val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (unsigned char) -1;
-        }
-    } else {
-        unsigned char val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (unsigned char) -1;
-        val = __Pyx_PyInt_As_unsigned_char(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to unsigned char");
-    return (unsigned char) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to unsigned char");
-    return (unsigned char) -1;
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_char(unsigned char value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned char neg_one = (unsigned char) -1, const_zero = (unsigned char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(unsigned char) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(unsigned char) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned char) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(unsigned char) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned char) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(unsigned char),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(char) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(char) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(char) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(char),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
     char ctversion[4], rtversion[4];
     PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
     if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
```

### Comparing `minijson-2.8/setup.cfg` & `minijson-2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.8
+version = 2.9
 name = minijson
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 author = Piotr Maślanka
 license_files = 
 	LICENSE
 author_email = piotr.maslanka@dronehub.ai
```

### Comparing `minijson-2.8/LICENSE` & `minijson-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `minijson-2.8/setup.py` & `minijson-2.9/setup.py`

 * *Files identical despite different names*

