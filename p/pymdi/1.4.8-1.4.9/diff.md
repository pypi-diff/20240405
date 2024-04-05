# Comparing `tmp/pymdi-1.4.8.tar.gz` & `tmp/pymdi-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymdi-1.4.8.tar", last modified: Tue Aug 30 12:35:31 2022, max compression
+gzip compressed data, was "pymdi-1.4.9.tar", last modified: Thu Sep  8 19:10:19 2022, max compression
```

## Comparing `pymdi-1.4.8.tar` & `pymdi-1.4.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 12:35:32.656960 pymdi-1.4.8/
--rw-r--r--   0 root         (0) root         (0)     2297 2022-08-30 12:30:46.000000 pymdi-1.4.8/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       52 2022-08-29 19:02:49.000000 pymdi-1.4.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 12:35:32.441200 pymdi-1.4.8/MDI_Library/
--rw-r--r--   0 root         (0) root         (0)     7428 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 12:35:32.469016 pymdi-1.4.8/MDI_Library/STUBS_MPI/
--rw-r--r--   0 root         (0) root         (0)     2250 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/STUBS_MPI/mpi.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 12:35:32.530768 pymdi-1.4.8/MDI_Library/STUBS_Python/
--rw-r--r--   0 root         (0) root         (0)      234 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/STUBS_Python/mdi_plug_py.c
--rw-r--r--   0 root         (0) root         (0)      250 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/STUBS_Python/mdi_plug_py.h
--rwxr-xr-x   0 root         (0) root         (0)     1490 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/__init__.py
--rw-r--r--   0 root         (0) root         (0)      773 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/elements.h
--rw-r--r--   0 root         (0) root         (0)    61217 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi.c
--rw-r--r--   0 root         (0) root         (0)     8264 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi.h
--rwxr-xr-x   0 root         (0) root         (0)    44454 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi.py
--rw-r--r--   0 root         (0) root         (0)    51657 2022-08-30 12:30:46.000000 pymdi-1.4.8/MDI_Library/mdi_f90.F90
--rw-r--r--   0 root         (0) root         (0)    41886 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_general.c
--rw-r--r--   0 root         (0) root         (0)     1210 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_general.h
--rw-r--r--   0 root         (0) root         (0)    38642 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_global.c
--rw-r--r--   0 root         (0) root         (0)     9353 2022-08-30 12:30:46.000000 pymdi-1.4.8/MDI_Library/mdi_global.h
--rw-r--r--   0 root         (0) root         (0)    37262 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_lib.c
--rw-r--r--   0 root         (0) root         (0)     5512 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_lib.h
--rw-r--r--   0 root         (0) root         (0)    17564 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_mpi.c
--rw-r--r--   0 root         (0) root         (0)     1327 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_mpi.h
--rw-r--r--   0 root         (0) root         (0)     4609 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_plug_py.c
--rw-r--r--   0 root         (0) root         (0)      522 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_plug_py.h
--rw-r--r--   0 root         (0) root         (0)    14923 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_tcp.c
--rw-r--r--   0 root         (0) root         (0)      925 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_tcp.h
--rw-r--r--   0 root         (0) root         (0)     4741 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_test.c
--rw-r--r--   0 root         (0) root         (0)      645 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/mdi_test.h
--rw-r--r--   0 root         (0) root         (0)    55764 2022-08-29 19:02:49.000000 pymdi-1.4.8/MDI_Library/physconst.h
--rw-r--r--   0 root         (0) root         (0)      500 2022-08-30 12:35:32.646386 pymdi-1.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3401 2022-08-29 19:02:49.000000 pymdi-1.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 12:35:32.555770 pymdi-1.4.8/cmake/
--rw-r--r--   0 root         (0) root         (0)     1856 2022-08-29 19:02:49.000000 pymdi-1.4.8/cmake/mdiConfig.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 12:35:32.633810 pymdi-1.4.8/pymdi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      500 2022-08-30 12:35:31.000000 pymdi-1.4.8/pymdi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      801 2022-08-30 12:35:31.000000 pymdi-1.4.8/pymdi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-30 12:35:31.000000 pymdi-1.4.8/pymdi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-08-30 12:35:31.000000 pymdi-1.4.8/pymdi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-30 12:35:32.658044 pymdi-1.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4073 2022-08-29 19:02:51.000000 pymdi-1.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 19:10:19.253361 pymdi-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)     2297 2022-09-08 19:08:48.000000 pymdi-1.4.9/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2022-09-02 13:45:13.000000 pymdi-1.4.9/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 19:10:19.052920 pymdi-1.4.9/MDI_Library/
+-rw-r--r--   0 root         (0) root         (0)     7428 2022-09-02 15:20:39.000000 pymdi-1.4.9/MDI_Library/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 19:10:19.076898 pymdi-1.4.9/MDI_Library/STUBS_MPI/
+-rw-r--r--   0 root         (0) root         (0)     2250 2022-09-02 13:45:13.000000 pymdi-1.4.9/MDI_Library/STUBS_MPI/mpi.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 19:10:19.128023 pymdi-1.4.9/MDI_Library/STUBS_Python/
+-rw-r--r--   0 root         (0) root         (0)      234 2022-09-02 13:45:13.000000 pymdi-1.4.9/MDI_Library/STUBS_Python/mdi_plug_py.c
+-rw-r--r--   0 root         (0) root         (0)      250 2022-09-02 13:45:13.000000 pymdi-1.4.9/MDI_Library/STUBS_Python/mdi_plug_py.h
+-rwxr-xr-x   0 root         (0) root         (0)     1490 2022-09-02 15:20:39.000000 pymdi-1.4.9/MDI_Library/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      773 2022-09-02 15:20:39.000000 pymdi-1.4.9/MDI_Library/elements.h
+-rw-r--r--   0 root         (0) root         (0)    72537 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi.c
+-rw-r--r--   0 root         (0) root         (0)     8581 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi.h
+-rwxr-xr-x   0 root         (0) root         (0)    44617 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi.py
+-rw-r--r--   0 root         (0) root         (0)    48619 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_f90.F90
+-rw-r--r--   0 root         (0) root         (0)    47650 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_general.c
+-rw-r--r--   0 root         (0) root         (0)     1137 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_general.h
+-rw-r--r--   0 root         (0) root         (0)    41094 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_global.c
+-rw-r--r--   0 root         (0) root         (0)    10265 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_global.h
+-rw-r--r--   0 root         (0) root         (0)    41015 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_lib.c
+-rw-r--r--   0 root         (0) root         (0)     6054 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_lib.h
+-rw-r--r--   0 root         (0) root         (0)    19895 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_mpi.c
+-rw-r--r--   0 root         (0) root         (0)     1327 2022-09-02 15:20:39.000000 pymdi-1.4.9/MDI_Library/mdi_mpi.h
+-rw-r--r--   0 root         (0) root         (0)     4495 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_plug_py.c
+-rw-r--r--   0 root         (0) root         (0)      265 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_plug_py.h
+-rw-r--r--   0 root         (0) root         (0)    17524 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_tcp.c
+-rw-r--r--   0 root         (0) root         (0)      766 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_tcp.h
+-rw-r--r--   0 root         (0) root         (0)     5927 2022-09-08 19:08:48.000000 pymdi-1.4.9/MDI_Library/mdi_test.c
+-rw-r--r--   0 root         (0) root         (0)      645 2022-09-02 15:20:39.000000 pymdi-1.4.9/MDI_Library/mdi_test.h
+-rw-r--r--   0 root         (0) root         (0)    55764 2022-09-02 15:20:39.000000 pymdi-1.4.9/MDI_Library/physconst.h
+-rw-r--r--   0 root         (0) root         (0)      500 2022-09-08 19:10:19.247551 pymdi-1.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3401 2022-09-02 13:45:13.000000 pymdi-1.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 19:10:19.149440 pymdi-1.4.9/cmake/
+-rw-r--r--   0 root         (0) root         (0)     1856 2022-09-02 13:45:13.000000 pymdi-1.4.9/cmake/mdiConfig.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 19:10:19.229735 pymdi-1.4.9/pymdi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      500 2022-09-08 19:10:18.000000 pymdi-1.4.9/pymdi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      801 2022-09-08 19:10:18.000000 pymdi-1.4.9/pymdi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-08 19:10:18.000000 pymdi-1.4.9/pymdi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2022-09-08 19:10:18.000000 pymdi-1.4.9/pymdi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-08 19:10:19.254602 pymdi-1.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4073 2022-09-02 13:45:15.000000 pymdi-1.4.9/setup.py
```

### Comparing `pymdi-1.4.8/CMakeLists.txt` & `pymdi-1.4.9/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
    set(use_C "C")
    set(use_Python "Python")
 else()
    message( FATAL_ERROR "Language not supported.  Supported languages: C, CXX, Fortran, Python" )
 endif()
 
 project(mdi
-        VERSION 1.4.8
+        VERSION 1.4.9
         LANGUAGES ${use_C} ${use_CXX} ${use_Fortran})
 
 
 # Check for Python developement libraries, which are used for Python plugins
 if( python_plugins )
 
    # Attempt to find a valid development version of Python
```

### Comparing `pymdi-1.4.8/MDI_Library/CMakeLists.txt` & `pymdi-1.4.9/MDI_Library/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/MDI_Library/STUBS_MPI/mpi.h` & `pymdi-1.4.9/MDI_Library/STUBS_MPI/mpi.h`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/MDI_Library/__init__.py` & `pymdi-1.4.9/MDI_Library/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/MDI_Library/elements.h` & `pymdi-1.4.9/MDI_Library/elements.h`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/MDI_Library/mdi.c` & `pymdi-1.4.9/MDI_Library/mdi.c`

 * *Files 12% similar despite different names*

```diff
@@ -110,14 +110,39 @@
  * \param [in, out]  argc
  *                   Pointer to the number of arguments.
  * \param [in, out]  argv
  *                   Pointer to the argument vector.
  */
 int MDI_Init(int* argc, char*** argv)
 {
+  int ret;
+  ret = MDI_Init_code();
+  if ( ret != 0 ) {
+    return ret;
+  }
+  ret = MDI_Init_with_argv(argc, argv);
+  if ( ret != 0 ) {
+    return ret;
+  }
+  return 0;
+}
+
+
+/*! \brief Initialize communication through the MDI library
+ *
+ * If using the "-method MPI" option, this function must be called by all ranks.
+ * The function returns \p 0 on a success.
+ *
+ * \param [in, out]  argc
+ *                   Pointer to the number of arguments.
+ * \param [in, out]  argv
+ *                   Pointer to the argument vector.
+ */
+int MDI_Init_with_argv(int* argc, char*** argv)
+{
   int argc_in = *argc;
   char** argv_in = *argv;
 
   // Extract the mdi options
   int iarg;
   int mdi_iarg = -1;
   for (iarg=0; iarg < argc_in; iarg++) {
@@ -132,18 +157,16 @@
     mdi_error("No argument to the -mdi option was provided");
     return 1;
   }
 
   if ( mdi_iarg >= 0 ) {
     // Initialize MDI
     int ret = general_init(argv_in[mdi_iarg + 1]);
-    if ( ret == 0 ) {
-      is_initialized = 1;
-    }
-    else {
+    if ( ret != 0 ) {
+      mdi_error("Error in MDI_Init during call to general_init");
       return ret;
     }
 
     // pass out argc and argv, without the mdi-related options
     *argc = argc_in - 2;
     for (iarg=mdi_iarg+2; iarg < argc_in; iarg++) {
       argv_in[iarg - 2] = argv_in[iarg];
@@ -153,44 +176,62 @@
     // The -mdi argument was not provided, so don't initialize
     return 0;
   }
   return 0;
 }
 
 
+/*! \brief Initialize a code structure for the MDI library
+ *
+ * The function returns \p 0 on a success.
+ *
+ */
+int MDI_Init_code()
+{
+  int ret = general_init_code();
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Init_code");
+    return ret;
+  }
+  return 0;
+}
+
+
 /*! \brief Initialize communication through the MDI library
  *
  * If using the "-method MPI" option, this function must be called by all ranks.
  * The function returns \p 0 on a success.
  *
  * \param [in]       options
  *                   Options describing the communication method used to connect to codes.
  * \param [in, out]  world_comm
  *                   On input, the MPI communicator that spans all of the codes.
  *                   On output, the MPI communicator that spans the single code corresponding to the calling rank.
  *                   Only used if the "-method MPI" option is provided.
  */
 int MDI_Init_with_options(const char* options)
 {
-  int ret = general_init(options);
-  if ( ret == 0 ) {
-    is_initialized = 1;
+  int ret;
+  ret = general_init(options);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Init_with_options");
+    return ret;
   }
-  return ret;
+  return 0;
 }
 
 
 /*! \brief Indicates whether MDI_Init has been called
  *
  * \param [out]  flag
  *                   Flag is true if and only if MDI_Init has been called.
  */
 int MDI_Initialized(int* flag)
 {
-  *flag = is_initialized;
+  *flag = codes.initialized;
   return 0;
 }
 
 /*! \brief Accept a new MDI communicator
  *
  * The function returns an MDI_Comm that describes a connection between two codes.
  * If no new communicators are available, the function returns \p MDI_COMM_NULL.
@@ -206,15 +247,15 @@
  *
  * The function returns an MDI_Comm that describes a connection between two codes.
  * If no new communicators are available, the function returns \p MDI_COMM_NULL.
  *
  */
 MDI_Comm MDI_Accept_communicator(MDI_Comm* comm)
 {
-  if ( is_initialized == 0 ) {
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Accept_Communicator called but MDI has not been initialized");
     return 1;
   }
   *comm = general_accept_communicator();
   return 0;
 }
 
@@ -231,15 +272,15 @@
  * \param [in]       datatype
  *                   MDI handle (MDI_INT, MDI_DOUBLE, MDI_CHAR, etc.) corresponding to the type of data to be sent.
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int MDI_Send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm)
 {
-  if ( is_initialized == 0 ) {
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Send called but MDI has not been initialized");
     return 1;
   }
   return general_send(buf, count, datatype, comm);
 }
 
 
@@ -255,15 +296,15 @@
  * \param [in]       datatype
  *                   MDI handle (MDI_INT, MDI_DOUBLE, MDI_CHAR, etc.) corresponding to the type of data to be received.
  * \param [in]       comm
  *                   MDI communicator associated with the connection to the sending code.
  */
 int MDI_Recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm)
 {
-  if ( is_initialized == 0 ) {
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Recv called but MDI has not been initialized");
     return 1;
   }
   return general_recv(buf, count, datatype, comm);
 }
 
 
@@ -291,15 +332,15 @@
  * \param [in]       buf
  *                   Pointer to the data to be sent.
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int MDI_Send_command(const char* buf, MDI_Comm comm)
 {
-  if ( is_initialized == 0 ) {
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Send_Command called but MDI has not been initialized");
     return 1;
   }
   return general_send_command(buf, comm);
 }
 
 
@@ -327,15 +368,15 @@
  * \param [in]       buf
  *                   Pointer to the buffer where the received data will be stored.
  * \param [in]       comm
  *                   MDI communicator associated with the connection to the sending code.
  */
 int MDI_Recv_command(char* buf, MDI_Comm comm)
 {
-  if ( is_initialized == 0 ) {
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Recv_Command called but MDI has not been initialized");
     return 1;
   }
   return general_recv_command(buf, comm);
 }
 
 
@@ -824,19 +865,25 @@
  *
  * \param [out]      role
  *                   Role of the code (either \p MDI_DRIVER or \p MDI_ENGINE)
  *
  */
 int MDI_Get_role(int* role)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_Role called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_role: get_current_code failed");
+    return 1;
+  }
   if (strcmp(this_code->role, "DRIVER") == 0) {
     *role = MDI_DRIVER;
   }
   else if (strcmp(this_code->role, "ENGINE") == 0) {
     *role = MDI_ENGINE;
   }
   else {
@@ -855,15 +902,21 @@
  *                   Role of the code (either \p MDI_TCP, \p MDI_MPI, \p MDI_TEST, or \p MDI_PLUGIN)
  * \param [in]       comm
  *                   MDI communicator for which the library will return the communication method.
  *
  */
 int MDI_Get_method(int* method, MDI_Comm comm)
 {
-  communicator* comm_obj = get_communicator(current_code, comm);
+  int ret;
+  communicator* comm_obj;
+  ret = get_communicator(codes.current_key, comm, &comm_obj);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_method: get_communicator failed");
+    return 1;
+  }
   *method = comm_obj->method_id;
   return 0;
 }
 
 
 /*! \brief Get the previously accepted MDI communicator at a specific index in the array of all communicators.
  *
@@ -875,20 +928,32 @@
  * \param [in]       index
  *                   Request the i'th communicator in the list of accepted and valid communicators.
  *                   The list begins at \p 0.
  *
  */
 int MDI_Get_communicator(MDI_Comm* comm, int index)
 {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_communicator: get_current_code failed");
+    return 1;
+  }
   if ( index >= this_code->comms->size || index < 0 ) {
     *comm = MDI_COMM_NULL;
   }
   else {
-    communicator* comm_obj = vector_get(this_code->comms, index);
+    communicator* comm_obj;
+    ret = vector_get( this_code->comms, index, (void**)&comm_obj );
+    if ( ret != 0 ) {
+      mdi_error("Error in MDI_Get_communicator: vector_get failed");
+      return ret;
+    }
     if ( comm_obj->is_accepted == 0 ) {
       // If the code hasn't accepted this communicator, return null
       *comm = MDI_COMM_NULL;
     }
     else {
       *comm = comm_obj->id;
     }
@@ -922,19 +987,25 @@
 /*! \brief Get the rank of this process within the MPI intra-communicator for the current code
  *
  * This function is only used by the Fortran wrapper
  *
  */
 int MDI_Get_intra_rank(int intra_rank_out)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_intra_rank called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_intra_rank: get_current_code failed");
+    return 1;
+  }
   return this_code->intra_rank;
 }
 
 
 /*! \brief Register a node
  *
  * The function returns \p 0 on a success.
@@ -953,19 +1024,25 @@
  * The function returns \p 0 on a success.
  *
  * \param [in]       node_name
  *                   Name of the node.
  */
 int MDI_Register_node(const char* node_name)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Register_Node called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Register_node: get_current_code failed");
+    return 1;
+  }
   return register_node(this_code->nodes, node_name);
 }
 
 
 /*! \brief Check whether a node is supported on a specified engine
  *
  * The function returns \p 0 on a success.
@@ -994,34 +1071,51 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      flag
  *                   On return, 1 if the node is supported and 0 otherwise.
  */
 int MDI_Check_node_exists(const char* node_name, MDI_Comm comm, int* flag)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Check_Node_Exists called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_node_exists: get_current_code failed");
+    return ret;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
     return 2;
   }
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_node_exists: get_node_vector failed"); 
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_node_exists: get_node_index failed"); 
+    return ret;
+  }
   if ( node_index == -1 ) {
     *flag = 0;
   }
   else {
     *flag = 1;
   }
   return 0;
@@ -1052,26 +1146,38 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      nnodes
  *                   On return, the number of nodes supported by the engine.
  */
 int MDI_Get_nnodes(MDI_Comm comm, int* nnodes)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_NNodes called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_nnodes: get_current_code failed");
+    return ret;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_nnodes: get_node_vector failed");
+    return ret;
+  }
+
   *nnodes = (int)node_vec->size;
 
   return 0;
 }
 
 
 /*! \brief Get the name of a node on a specified engine
@@ -1102,32 +1208,44 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      name
  *                   On return, the name of the node
  */
 int MDI_Get_node(int index, MDI_Comm comm, char* name)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_Node called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_node: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  vector* node_vec = get_node_vector(comm);
-  if ( node_vec == NULL ) {
-    mdi_error("MDI_Get_Node unable to find node vector");
-    return 1;
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_nodes: get_node_vector failed");
+    return ret;
   }
 
-  node* ret_node = vector_get(node_vec, index);
+  node* ret_node;
+  ret = vector_get( node_vec, index, (void**)&ret_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_node: vector_get failed");
+    return ret;
+  }
   if ( ret_node == NULL ) {
     mdi_error("MDI_Get_Node unable to find node");
     return 1;
   }
   snprintf(name, MDI_NAME_LENGTH, "%s", ret_node->name);
   return 0;
 }
@@ -1155,19 +1273,26 @@
  * \param [in]       node_name
  *                   Name of the node on which the command will be registered.
  * \param [in]       command_name
  *                   Name of the command.
  */
 int MDI_Register_command(const char* node_name, const char* command_name)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Register_Command called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Register_command: get_current_code failed");
+    return 1;
+  }
   return register_command(this_code->nodes, node_name, command_name);
 }
 
 
 /*! \brief Check whether a command is supported on specified node on a specified engine
  *
  * The function returns \p 0 on a success.
@@ -1200,21 +1325,27 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      flag
  *                   On return, 1 if the command is supported and 0 otherwise.
  */
 int MDI_Check_command_exists(const char* node_name, const char* command_name, MDI_Comm comm, int* flag)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Check_Command_Exists called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_command_exists: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
@@ -1223,26 +1354,46 @@
 
   // confirm that the command_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(command_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Cannot chcek command name with length greater than MDI_COMMAND_LENGTH");
     return 3;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_command_exists: get_node_vector failed");
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_command_exists: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("Could not find the node");
     return 1;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get( node_vec, node_index, (void**)&target_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_command_exists: vector_get failed");
+    return ret;
+  }
 
   // find the command
-  int command_index = get_command_index(target_node, command_name);
+  int command_index;
+  ret = get_command_index(target_node, command_name, &command_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_command_exists: get_command_index failed");
+    return ret;
+  }
   if ( command_index == -1 ) {
     *flag = 0;
   }
   else {
     *flag = 1;
   }
   return 0;
@@ -1279,40 +1430,61 @@
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      nnodes
  *                   On return, the number of commands supported on the specified engine
  *                   on the specified node.
  */
 int MDI_Get_ncommands(const char* node_name, MDI_Comm comm, int* ncommands)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_NCommands called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncommands: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
     return 2;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncommands: get_node_vector failed");
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncommands: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("Could not find the node");
     return 1;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get( node_vec, node_index, (void**)&target_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncommands: vector_get failed");
+    return ret;
+  }
 
   *ncommands = (int)target_node->commands->size;
   return 0;
 }
 
 
 /*! \brief Get the name of a command on a specified node on a specified engine
@@ -1347,41 +1519,67 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      name
  *                   On return, the name of the command
  */
 int MDI_Get_command(const char* node_name, int index, MDI_Comm comm, char* name)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_Command called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_command: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_command: get_node_vector failed");
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_command: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("MDI_Get_Command could not find the requested node");
     return 1;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get( node_vec, node_index, (void**)&target_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_command: vector_get failed for node");
+    return ret;
+  }
 
   if ( target_node->commands->size <= index ) {
     mdi_error("MDI_Get_Command failed because the command does not exist");
     return 1;
   }
 
-  char* target_command = vector_get( target_node->commands, index );
+  char* target_command;
+  ret = vector_get( target_node->commands, index, (void**)&target_command );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_command: vector_get failed for command");
+    return ret;
+  }
   snprintf(name, MDI_NAME_LENGTH, "%s", target_command);
   return 0;
 }
 
 
 /*! \brief Register a callback on a specified node
  *
@@ -1405,19 +1603,25 @@
  * \param [in]       node_name
  *                   Name of the node on which the callback will be registered.
  * \param [in]       callback_name
  *                   Name of the callback.
  */
 int MDI_Register_callback(const char* node_name, const char* callback_name)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Register_Callback called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Register_callback: get_current_code failed");
+    return 1;
+  }
   return register_callback(this_code->nodes, node_name, callback_name);
 }
 
 
 /*! \brief Check whether a callback exists on specified node on a specified engine
  *
  * The function returns \p 0 on a success.
@@ -1450,21 +1654,27 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      flag
  *                   On return, 1 if the callback is supported and 0 otherwise.
  */
 int MDI_Check_callback_exists(const char* node_name, const char* callback_name, MDI_Comm comm, int* flag)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Check_Callback_Exists called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_callback_exists: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
@@ -1473,26 +1683,46 @@
 
   // confirm that the callback_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(callback_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Cannot check callback name with length greater than MDI_COMMAND_LENGTH");
     return 3;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_callback_exists: get_node_vector failed");
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_callback_exists: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("Could not find the node");
     return 4;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get( node_vec, node_index, (void**)&target_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_callback_exists: vector_get failed");
+    return ret;
+  }
 
   // find the callback
-  int callback_index = get_callback_index(target_node, callback_name);
+  int callback_index;
+  ret = get_callback_index(target_node, callback_name, &callback_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_callback_exists: get_callback_index failed"); 
+    return 1;
+  }
   if ( callback_index == -1 ) {
     *flag = 0;
   }
   else {
     *flag = 1;
   }
   return 0;
@@ -1529,40 +1759,61 @@
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      ncallbacks
  *                   On return, the number of callbacks on the specified node
  *                   on the specified engine.
  */
 int MDI_Get_ncallbacks(const char* node_name, MDI_Comm comm, int* ncallbacks)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_NCallbacks called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncallbacks: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) > MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
     return 2;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncallbacks: get_node_vector failed");
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Check_node_exists: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("Could not find the node");
     return 3;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get( node_vec, node_index, (void**)&target_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_ncallbacks: vector_get failed");
+    return ret;
+  }
 
   *ncallbacks = (int)target_node->callbacks->size;
   return 0;
 }
 
 
 /*! \brief Get the name of a callback on a specified node on a specified engine
@@ -1597,60 +1848,92 @@
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will check for the calling engine.
  * \param [out]      name
  *                   On return, the name of the callback
  */
 int MDI_Get_callback(const char* node_name, int index, MDI_Comm comm, char* name)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_Get_Callback called but MDI has not been initialized");
     return 1;
   }
 
   // Only rank 0 should respond to this call
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_callback: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  vector* node_vec = get_node_vector(comm);
+  vector* node_vec;
+  ret = get_node_vector(comm, &node_vec);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_callback: get_node_vector failed");
+    return ret;
+  }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_callback: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("MDI_Get_Command could not find the requested node");
     return 2;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get( node_vec, node_index, (void**)&target_node );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_callback: vector_get failed for node");
+    return ret;
+  }
 
   if ( target_node->callbacks->size <= index ) {
     mdi_error("MDI_Get_Command failed because the command does not exist");
     return 3;
   }
 
-  char* target_callback = vector_get( target_node->callbacks, index );
+  char* target_callback;
+  ret = vector_get( target_node->callbacks, index, (void**)&target_callback );
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_callback: vector_get failed for callback");
+    return ret;
+  }
   snprintf(name, MDI_NAME_LENGTH, "%s", target_callback);
   return 0;
 }
 
 
 /*! \brief Obtain the MPI communicator that spans the single code corresponding to the calling rank
  *
  * The function returns \p 0 on a success.
  *
  * \param [out]  world_comm
  *                   On output, the MPI communicator that spans the single code corresponding to the calling rank.
  */
 int MDI_MPI_get_world_comm(void* world_comm)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_MPI_get_world_comm called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_MPI_get_world_comm: get_current_code failed");
+    return 1;
+  }
 
   if ( this_code->language == MDI_LANGUAGE_PYTHON ) {
     mdi_error("MDI_MPI_get_world_comm was called by a Python code");
   }
   else if ( this_code->language == MDI_LANGUAGE_FORTRAN ) {
     MPI_Comm mpi_communicator = MPI_COMM_NULL;
     mpi_update_world_comm( (void*) &mpi_communicator );
@@ -1674,19 +1957,25 @@
  * The function returns \p 0 on a success.
  *
  * \param [out]  world_comm
  *                   The MPI communicator that spans the single code corresponding to the calling rank.
  */
 int MDI_MPI_set_world_comm(void* world_comm)
 {
-  if ( is_initialized == 0 ) {
+  int ret;
+  if ( codes.initialized == 0 ) {
     mdi_error("MDI_MPI_set_world_comm called but MDI has not been initialized");
     return 1;
   }
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_MPI_set_world_comm: get_current_code failed");
+    return 1;
+  }
 
   if ( this_code->language == MDI_LANGUAGE_PYTHON ) {
     mdi_error("MDI_MPI_set_world_comm was called by a Python code");
   }
   else if ( this_code->language == MDI_LANGUAGE_FORTRAN ) {
     MPI_Fint* f_comm_ptr = (MPI_Fint*) world_comm;
     MPI_Comm c_comm = MPI_Comm_f2c( *f_comm_ptr );
@@ -1799,224 +2088,341 @@
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       execute_command
  *                   Function pointer to the generic execute_command function
  */
 int MDI_Set_execute_command_func(int (*generic_command)(const char*, MDI_Comm, void*), void* class_object) {
-  code* this_code = get_code(current_code);
-  this_code->execute_command = generic_command;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_execute_command_func: get_current_code failed");
+    return 1;
+  }
+  this_code->execute_command_wrapper = generic_command;
   this_code->execute_command_obj = class_object;
   this_code->called_set_execute_command_func = 1;
   return 0;
 }
 
 
 int MDI_Set_plugin_state(void* state) {
+  int ret = MDI_Init_code();
+  if ( ret != 0 ) {
+    return ret;
+  }
+
+  return library_set_state(state);
+}
+
+
+/*! \brief Set the language-based callback for when a code is destroyed
+ *
+ * This is only intended to be used internally by the MDI Library
+ *
+ */
+int MDI_Set_plugin_state_internal(void* state) {
   return library_set_state(state);
 }
 
 
 /*! \brief Set the language-based callback for when a code is destroyed
  *
  * This is currently only used by Fortran plugins
  *
  */
 int MDI_Set_on_destroy_code(int (*func)(int)) {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_on_destroy_code: get_current_code failed");
+    return 1;
+  }
   this_code->language_on_destroy = func;
   return 0;
 }
 
 
 /*! \brief Get the current code
  *
  */
 int MDI_Get_Current_Code() {
-  return current_code;
-}
-
-
-/*! \brief Get whether plugin mode is active
- *
- */
-int MDI_Get_plugin_mode(int* plugin_mode_ptr) {
-  *plugin_mode_ptr = plugin_mode;
-  return 0;
+  return codes.current_key;
 }
 
 
 /*! \brief Get plugin_argc
  *
  */
 int MDI_Plugin_get_argc(int* argc_ptr) {
-  if ( ! plugin_mode ) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Plugin_get_argc: get_current_code failed");
+    return 1;
+  }
+  if ( this_code->plugin_argc == -1 ) {
     mdi_error("MDI_Plugin_get_argc called, but plugin mode is not active.");
     return 1;
   }
-  *argc_ptr = plugin_argc;
+  *argc_ptr = this_code->plugin_argc;
   return 0;
 }
 
 
 /*! \brief Get plugin_argv
  *
  */
 int MDI_Plugin_get_argv(char*** argv_ptr) {
-  if ( ! plugin_mode ) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Plugin_get_argv: get_current_code failed");
+    return 1;
+  }
+  if ( this_code->plugin_argc == -1 ) {
     mdi_error("MDI_Plugin_get_argv called, but plugin mode is not active.");
     return 1;
   }
-  *argv_ptr = plugin_argv;
+  *argv_ptr = this_code->plugin_argv;
   return 0;
 }
 
 
 /*! \brief Get plugin_unedited_options
  *
  */
 int MDI_Plugin_get_args(char** args_ptr) {
-  if ( ! plugin_mode ) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Plugin_get_args: get_current_code failed");
+    return 1;
+  }
+  if ( this_code->plugin_argc == -1 ) {
     mdi_error("MDI_Plugin_get_args called, but plugin mode is not active.");
     return 1;
   }
-  *args_ptr = plugin_unedited_options;
+  *args_ptr = this_code->plugin_unedited_options;
   return 0;
 }
 
 
 /*! \brief Get a specific element from plugin_argv
  *
  */
 int MDI_Plugin_get_arg(int index, char** arg_ptr) {
-  if ( ! plugin_mode ) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Plugin_get_arg: get_current_code failed");
+    return 1;
+  }
+  if ( this_code->plugin_argc == -1 ) {
     mdi_error("MDI_Plugin_get_arg called, but plugin mode is not active.");
     return 1;
   }
   if ( index < 0 ) {
     mdi_error("MDI_Plugin_get_arg called with invalid value (<0) for index.");
     return 1;
   }
-  if ( index > plugin_argc ) {
+  if ( index > this_code->plugin_argc ) {
     mdi_error("MDI_Plugin_get_arg called with invalid value (>argc) for index.");
     return 1;
   }
-  *arg_ptr = plugin_argv[index];
+  *arg_ptr = this_code->plugin_argv[index];
   return 0;
 }
 
 
 /*! \brief Get the Python plugin MPI communicator
  *
  */
-int MDI_Get_python_plugin_mpi_world_ptr(void** python_plugin_mpi_world_ptr_ptr) {
-  *python_plugin_mpi_world_ptr_ptr = shared_state_from_driver->mpi_comm_ptr;
+int MDI_Get_python_plugin_mpi_world_ptr(void** python_plugin_mpi_world_ptr_ptr, void* state_in) {
+  plugin_shared_state* this_state = (plugin_shared_state*) state_in;
+  *python_plugin_mpi_world_ptr_ptr = this_state->mpi_comm_ptr;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for MPI_Recv when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_recv
  *                   Function pointer to the mpi4py_recv callback
  */
 int MDI_Set_Mpi4py_Recv_Callback(int (*mpi4py_recv)(void*, int, int, int, MDI_Comm)) {
-  mpi4py_recv_callback = mpi4py_recv;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Recv_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_recv_callback = mpi4py_recv;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for MPI_Send when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_send
  *                   Function pointer to the mpi4py_send callback
  */
 int MDI_Set_Mpi4py_Send_Callback(int (*mpi4py_send)(void*, int, int, int, MDI_Comm)) {
-  mpi4py_send_callback = mpi4py_send;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Send_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_send_callback = mpi4py_send;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for gathering MDI versions when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_allgather
  *                   Function pointer to the mpi4py_allgather callback
  */
 int MDI_Set_Mpi4py_Allgather_Callback(int (*mpi4py_allgather)(void*, void*)) {
-  mpi4py_allgather_callback = mpi4py_allgather;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Allgather_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_allgather_callback = mpi4py_allgather;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for gathering code names when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_gather_names
  *                   Function pointer to the mpi4py_gather_names callback
  */
 int MDI_Set_Mpi4py_Gather_Names_Callback(int (*mpi4py_gather_names)(void*, void*, int*, int*)) {
-  mpi4py_gather_names_callback = mpi4py_gather_names;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Gather_Names_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_gather_names_callback = mpi4py_gather_names;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for MPI_Split when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_split
  *                   Function pointer to the mpi4py_split callback
  */
 int MDI_Set_Mpi4py_Split_Callback(int (*mpi4py_split)(int, int, MDI_Comm, int)) {
-  mpi4py_split_callback = mpi4py_split;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Split_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_split_callback = mpi4py_split;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for MPI_Comm_rank when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_rank
  *                   Function pointer to the mpi4py_rank callback
  */
 int MDI_Set_Mpi4py_Rank_Callback(int (*mpi4py_rank)(int)) {
-  mpi4py_rank_callback = mpi4py_rank;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Rank_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_rank_callback = mpi4py_rank;
   return 0;
 }
 
 /*! \brief Set the callback MDI uses for MPI_Comm_size when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_size
  *                   Function pointer to the mpi4py_size callback
  */
 int MDI_Set_Mpi4py_Size_Callback(int (*mpi4py_size)(int)) {
-  mpi4py_size_callback = mpi4py_size;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Size_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_size_callback = mpi4py_size;
   return 0;
 }
 
 
 /*! \brief Set the callback MDI uses for MPI_Barrier when using mpi4py
  *
  * The function returns \p 0 on a success.
  *
  * \param [in]       mpi4py_barrier
  *                   Function pointer to the mpi4py_barrier callback
  */
 int MDI_Set_Mpi4py_Barrier_Callback(int (*mpi4py_barrier)(int)) {
-  mpi4py_barrier_callback = mpi4py_barrier;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_Mpi4py_Barrier_Callback: get_current_code failed");
+    return ret;
+  }
+  this_code->mpi4py_barrier_callback = mpi4py_barrier;
   return 0;
 }
 
 
 /*! \brief Set the language of an MDI plugin
  *
  * The function returns \p 0 on a success.
@@ -2024,8 +2430,52 @@
  * \param [in]       language
  *                   Language of the plugin
  */
 int MDI_Set_plugin_language(int language, void* plugin_state) {
   plugin_shared_state* this_state = (plugin_shared_state*) plugin_state;
   this_state->engine_language = language;
   return 0;
-}
+}
+
+
+/*! \brief Set the language execute_command function needed by a language wrapper
+ *
+ * The function returns \p 0 on a success.
+ *
+ * \param [in]       execute_command
+ *                   Execute command callback
+ */
+int MDI_Set_language_execute_command(int (*execute_command)(void*, MDI_Comm, void*)) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Set_language_execute_command: get_current_code failed");
+    return ret;
+  }
+  this_code->execute_command = execute_command;
+  return 0;
+}
+
+
+/*! \brief Get the language execute_command function needed by a language wrapper
+ *
+ * The function returns a function pointer to the execute_command function.
+ *
+ * \param [out]      execute_command
+ *                   Execute command callback
+ * \param [in]       comm
+ *                   MDI communicator
+ */
+int (*MDI_Get_language_execute_command(MDI_Comm comm))(void*, MDI_Comm, void*) {
+  communicator* this_comm;
+  int ret = get_communicator(codes.current_key, comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Get_language_execute_command: get_communicator failed");
+    //return ret;
+  }
+  library_data* libd = (library_data*) this_comm->method_data;
+  return libd->shared_state->execute_command;
+}
+
+
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi.h` & `pymdi-1.4.9/MDI_Library/mdi.h`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 
 // MDI role types
 DllExport extern const int MDI_DRIVER;
 DllExport extern const int MDI_ENGINE;
 
 // functions for handling MDI communication
 DllExport int MDI_Init(int* argc, char ***argv);
-DllExport int MDI_Init_with_options(const char *options);
 DllExport int MDI_Initialized(int* flag);
 DllExport int MDI_Accept_Communicator(MDI_Comm* comm);
 DllExport int MDI_Accept_communicator(MDI_Comm* comm);
 DllExport int MDI_Send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm);
 DllExport int MDI_Recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm);
 DllExport int MDI_Send_Command(const char* buf, MDI_Comm comm);
 DllExport int MDI_Send_command(const char* buf, MDI_Comm comm);
@@ -136,15 +135,15 @@
                                 MDI_Driver_node_callback_t driver_node_callback,
                                 void* driver_callback_object);
 DllExport int MDI_Open_plugin(const char* plugin_name, const char* options, void* mpi_comm_ptr, MDI_Comm* mdi_comm_ptr);
 DllExport int MDI_Close_plugin(MDI_Comm mdi_comm);
 DllExport int MDI_Set_Execute_Command_Func(int (*generic_command)(const char*, MDI_Comm, void*), void* class_object);
 DllExport int MDI_Set_execute_command_func(int (*generic_command)(const char*, MDI_Comm, void*), void* class_object);
 DllExport int MDI_Set_plugin_state(void* state);
-DllExport int MDI_Get_plugin_mode(int* plugin_mode);
+DllExport int MDI_Set_plugin_state_internal(void* state);
 DllExport int MDI_Plugin_get_argc(int* argc_ptr);
 DllExport int MDI_Plugin_get_argv(char*** argv_ptr);
 DllExport int MDI_Plugin_get_args(char** args_ptr);
 DllExport int MDI_Plugin_get_arg(int index, char** arg_ptr);
 
 // functions for managing callback functions for mpi4py
 DllExport int MDI_Set_Mpi4py_Recv_Callback(int (*mpi4py_recv)(void*, int, int, int, MDI_Comm));
@@ -153,21 +152,26 @@
 DllExport int MDI_Set_Mpi4py_Gather_Names_Callback(int (*mpi4py_gather_names)(void*, void*, int*, int*));
 DllExport int MDI_Set_Mpi4py_Split_Callback(int (*mpi4py_split)(int, int, MDI_Comm, int));
 DllExport int MDI_Set_Mpi4py_Rank_Callback(int (*mpi4py_rank)(int));
 DllExport int MDI_Set_Mpi4py_Size_Callback(int (*mpi4py_size)(int));
 DllExport int MDI_Set_Mpi4py_Barrier_Callback(int (*mpi4py_barrier)(int));
 
 // only used internally by MDI
+DllExport int MDI_Init_code();
+DllExport int MDI_Init_with_argv(int* argc, char ***argv);
+DllExport int MDI_Init_with_options(const char *options);
 DllExport void mdi_error(const char* message);
 DllExport void MDI_Set_World_Size(int world_size_in);
 DllExport void MDI_Set_World_Rank(int world_rank_in);
 DllExport int MDI_Get_intra_rank(int intra_rank_out);
 DllExport int MDI_Get_Current_Code();
-DllExport int MDI_Get_python_plugin_mpi_world_ptr(void** plugin_mode);
+DllExport int MDI_Get_python_plugin_mpi_world_ptr(void** python_plugin_mpi_world_ptr_ptr, void* state_in);
 DllExport int MDI_Set_on_destroy_code(int (*func)(int));
 DllExport int MDI_Set_plugin_language(int language, void* plugin_state);
+DllExport int MDI_Set_language_execute_command(int (*execute_command)(void*, MDI_Comm, void*));
+DllExport int (*MDI_Get_language_execute_command(MDI_Comm comm))(void*, MDI_Comm, void*);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi.py` & `pymdi-1.4.9/MDI_Library/mdi.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,37 +492,26 @@
 # define the python function that will set the callback function in c
 mpi4py_split_callback_c = mpi4py_split_func_type( mpi4py_split_callback )
 def set_mpi4py_split_callback():
     global mpi4py_split_callback_c
     mdi.MDI_Set_Mpi4py_Split_Callback( mpi4py_split_callback_c )
 
 
-# MDI_Get_plugin_mode
-mdi.MDI_Get_plugin_mode.argtypes = [ctypes.POINTER(ctypes.c_int)]
-mdi.MDI_Get_plugin_mode.restype = ctypes.c_int
-def MDI_Get_plugin_mode():
-    plugin_mode = ctypes.c_int()
-    ret = mdi.MDI_Get_plugin_mode(ctypes.byref(plugin_mode))
-    if ret != 0:
-        raise Exception("MDI Error: MDI_Get_plugin_mode failed")
-    return plugin_mode.value
-
-
-# MDI_Get_plugin_mode
-mdi.MDI_Get_python_plugin_mpi_world_ptr.argtypes = [ctypes.POINTER(ctypes.c_void_p)]
+# MDI_Get_python_plugin_mpi_world_ptr
+mdi.MDI_Get_python_plugin_mpi_world_ptr.argtypes = [ctypes.POINTER(ctypes.c_void_p), ctypes.c_void_p]
 mdi.MDI_Get_python_plugin_mpi_world_ptr.restype = ctypes.c_int
-def MDI_Get_python_plugin_mpi_world_ptr():
+def MDI_Get_python_plugin_mpi_world_ptr( plugin_state ):
     python_plugin_mpi_world_ptr = ctypes.c_void_p()
-    ret = mdi.MDI_Get_python_plugin_mpi_world_ptr(ctypes.byref(python_plugin_mpi_world_ptr))
+    ret = mdi.MDI_Get_python_plugin_mpi_world_ptr(ctypes.byref(python_plugin_mpi_world_ptr), plugin_state)
     if ret != 0:
         raise Exception("MDI Error: MDI_Get_python_plugin_mpi_world_ptr failed")
     return python_plugin_mpi_world_ptr.value
 
 
-def MDI_MPI_initialization():
+def MDI_MPI_initialization(plugin_state = None):
     global world_comm
     global intra_code_comm
     global use_mpi4py
     global MPI
 
     # attempt to import mpi4py
     try:
@@ -536,18 +525,17 @@
         pass
 
     comm = None
     if use_mpi4py:
         comm = MPI.COMM_WORLD
 
     # if this is a plugin code, get the plugin's MPI communicator
-    plugin_mode = MDI_Get_plugin_mode()
-    if ( plugin_mode == 1  and use_mpi4py ):
+    if ( plugin_state is not None and use_mpi4py ):
         # Get a pointer to the C MPI communicator
-        python_plugin_mpi_world_ptr = MDI_Get_python_plugin_mpi_world_ptr()
+        python_plugin_mpi_world_ptr = MDI_Get_python_plugin_mpi_world_ptr(plugin_state)
 
         # Convert the C MPI communicator to an MPI4Py communicator
         c_mpi_communicator = ctypes.cast(python_plugin_mpi_world_ptr, ctypes.POINTER(ctypes.c_void_p)).contents.value
         handle_t = ctypes.c_void_p
         newobj = type(MPI.COMM_WORLD)()
         handle_new = handle_t.from_address(MPI._addressof(newobj))
         handle_new.value = c_mpi_communicator
@@ -576,14 +564,16 @@
     set_mpi4py_allgather_callback()
     set_mpi4py_gather_names_callback()
     set_mpi4py_barrier_callback()
     set_mpi4py_split_callback()
 
 
 # MDI_Init
+mdi.MDI_Init_code.argtypes = []
+mdi.MDI_Init_code.restype = ctypes.c_int
 mdi.MDI_Init_with_options.argtypes = [ctypes.POINTER(ctypes.c_char)]
 mdi.MDI_Init_with_options.restype = ctypes.c_int
 def MDI_Init(arg1, arg2 = None):
     # prepend the _language option, so that MDI knows this is a Python code
     arg1 = "_language Python " + arg1
 
     # determine the communication method
@@ -601,19 +591,24 @@
         #    raise Exception("MDI Error: When using the MPI communication method, mpi4py must be available")
 
         # ensure that numpy is available
         if use_mpi4py:
             if not found_numpy:
                 raise Exception("MDI Error: When using the MPI communication method, numpy must be available")
 
+    # Initialize the MDI codes vector
+    ret = mdi.MDI_Init_code()
+    if ret != 0:
+        raise Exception("MDI Error: MDI_Init during call to MDI_Init_code failed")
+
     MDI_MPI_initialization()
 
     # call MDI_Init
     command = arg1.encode('utf-8')
-    ret = mdi.MDI_Init_with_options(ctypes.c_char_p(command) )
+    ret = mdi.MDI_Init_with_options( ctypes.c_char_p(command) )
     if ret != 0:
         raise Exception("MDI Error: MDI_Init failed")
 
     return ret
 
 def MDI_MPI_get_world_comm():
     global intra_code_comm
@@ -1175,18 +1170,24 @@
     if ret != 0:
         raise Exception("MDI Error: MDI_Launch_plugin failed")
 
     return ret
 
 
 # MDI_Set_plugin_state
-mdi.MDI_Set_plugin_state.argtypes = [ctypes.c_void_p]
-mdi.MDI_Set_plugin_state.restye = ctypes.c_int
+mdi.MDI_Set_plugin_state_internal.argtypes = [ctypes.c_void_p]
+mdi.MDI_Set_plugin_state_internal.restye = ctypes.c_int
 def MDI_Set_plugin_state(plugin_state):
-    ret = mdi.MDI_Set_plugin_state( plugin_state )
 
-    MDI_MPI_initialization()
+    # Initialize a new MDI code
+    ret = mdi.MDI_Init_code()
+    if ret != 0:
+        raise Exception("MDI Error: MDI_Set_plugin_state failed during call to MDI_Init_code")
+
+    MDI_MPI_initialization( plugin_state=plugin_state )
+
+    ret = mdi.MDI_Set_plugin_state_internal( plugin_state )
 
     if ret != 0:
         raise Exception("MDI Error: MDI_Set_plugin_state failed")
 
     return ret
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_f90.F90` & `pymdi-1.4.9/MDI_Library/mdi_f90.F90`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,49 @@
 
 MODULE MDI_INTERNAL
   USE ISO_C_BINDING
   USE MDI_GLOBAL
 
   IMPLICIT NONE
 
-  ! The execute_command callbacks are implemented in a pseudo-dictionary
-  ! Each key corresponds to the handle of one of the codes that has called MDI_Init
-  ! The values are the actual procedure pointers
-  TYPE command_func_ptr
-     INTEGER                                     :: key
-     PROCEDURE(execute_command), POINTER, NOPASS :: value => null()
-  END TYPE command_func_ptr
-  TYPE(command_func_ptr), ALLOCATABLE :: execute_commands(:)
-
   ABSTRACT INTERFACE
     SUBROUTINE execute_command(buf, comm, ierr)
       CHARACTER(LEN=*), INTENT(IN) :: buf
       INTEGER, INTENT(IN)          :: comm
       INTEGER, INTENT(OUT)         :: ierr
     END SUBROUTINE execute_command
   END INTERFACE
 
+  ABSTRACT INTERFACE
+    FUNCTION execute_command_correct(buf, comm, class_obj)
+      USE ISO_C_BINDING
+      USE MDI_GLOBAL
+!      CHARACTER(LEN=1, KIND=C_CHAR), TARGET    :: buf(COMMAND_LENGTH)
+!      INTEGER(KIND=C_INT), VALUE               :: comm
+      CHARACTER(LEN=*), INTENT(IN) :: buf
+!      CHARACTER(LEN=1), INTENT(IN) :: buf(COMMAND_LENGTH)
+      INTEGER, INTENT(IN)          :: comm
+      TYPE(C_PTR), VALUE                       :: class_obj
+      INTEGER(KIND=C_INT)       :: execute_command_correct
+    END FUNCTION execute_command_correct
+  END INTERFACE
+
+  ABSTRACT INTERFACE
+    FUNCTION execute_command_write(buf, comm, class_obj)
+      USE ISO_C_BINDING
+      USE MDI_GLOBAL
+!      CHARACTER(LEN=1, KIND=C_CHAR), TARGET    :: buf(COMMAND_LENGTH)
+!      CHARACTER(LEN=*), INTENT(IN) :: buf
+      CHARACTER(LEN=1), INTENT(IN) :: buf(COMMAND_LENGTH)
+      INTEGER, INTENT(IN)          :: comm
+      TYPE(C_PTR), VALUE                       :: class_obj
+      INTEGER(KIND=C_INT)       :: execute_command_write
+    END FUNCTION execute_command_write
+  END INTERFACE
+
   INTERFACE
 
      FUNCTION MDI_Set_Execute_Command_Func_c(command_func, class_obj) bind(c, name="MDI_Set_Execute_Command_Func")
        USE ISO_C_BINDING
        TYPE(C_FUNPTR), VALUE, INTENT(IN)        :: command_func
        TYPE(C_PTR), VALUE                       :: class_obj
        INTEGER(KIND=C_INT)                      :: MDI_Set_Execute_Command_Func_c
@@ -52,14 +70,29 @@
      END FUNCTION MDI_Get_Current_Code_
 
      FUNCTION MDI_Get_intra_rank_() bind(c, name="MDI_Get_intra_rank")
        USE, INTRINSIC :: iso_c_binding
        INTEGER(KIND=C_INT)                      :: MDI_Get_intra_rank_
      END FUNCTION MDI_Get_intra_rank_
 
+     FUNCTION MDI_Set_language_execute_command_(func_ptr) bind(c, name="MDI_Set_language_execute_command")
+       USE, INTRINSIC :: iso_c_binding
+       TYPE(C_FUNPTR), VALUE                    :: func_ptr
+       INTEGER(KIND=C_INT)                      :: MDI_Set_language_execute_command_
+     END FUNCTION MDI_Set_language_execute_command_
+
+     FUNCTION MDI_Get_language_execute_command_(comm) bind(c, name="MDI_Get_language_execute_command")
+       USE, INTRINSIC :: iso_c_binding
+       INTEGER(KIND=C_INT), VALUE               :: comm
+       !TYPE(C_FUNPTR), VALUE                       :: execute_command_ptr
+       !INTEGER(KIND=C_INT)                      :: MDI_Get_language_execute_command_
+       TYPE(C_FUNPTR)                           :: MDI_Get_language_execute_command_
+     END FUNCTION MDI_Get_language_execute_command_
+
+
   END INTERFACE
 
 CONTAINS
 
   FUNCTION MDI_Get_intra_rank()
     INTEGER                                  :: MDI_Get_intra_rank
     MDI_Get_intra_rank = MDI_Get_intra_rank_()
@@ -102,157 +135,70 @@
     DO i = 1, LEN_TRIM(fbuf)
        cbuf(i) = fbuf(i:i)
     END DO
     cbuf( LEN_TRIM(fbuf) + 1 ) = c_null_char
     str_f_to_c = cbuf
   END FUNCTION str_f_to_c
 
-  ! Return the index in execute_commands that corresponds to the key argument
-  FUNCTION find_execute_command(key)
-    INTEGER, INTENT(IN)                      :: key
-    INTEGER                                  :: find_execute_command
-    INTEGER                                  :: index
-
-    ! Check if the execute_commands dictionary has been allocated
-    IF ( .not. ALLOCATED(execute_commands) ) THEN
-      find_execute_command = -1
-      RETURN
-    END IF
-
-    index = 1
-    DO WHILE( (index .le. SIZE(execute_commands)) .and. (execute_commands(index)%key .ne. key) )
-      index = index + 1
-    END DO
+  FUNCTION MDI_On_destroy_code_f(code_id) bind(c)
+    INTEGER(KIND=C_INT)                      :: MDI_On_destroy_code_f
+    INTEGER                                  :: ierr
+    INTEGER(KIND=C_INT), VALUE               :: code_id
 
-    IF ( index .gt. SIZE(execute_commands) ) THEN
-      find_execute_command = -1
-      RETURN
-    END IF
-
-    find_execute_command = index
-  END FUNCTION find_execute_command
-
-  ! Add a value to the execute_command dictionary
-  SUBROUTINE add_execute_command(key, value)
-    INTEGER, INTENT(IN)                      :: key
-    PROCEDURE(execute_command), POINTER      :: value
-    INTEGER                                  :: index
-    TYPE(command_func_ptr), ALLOCATABLE      :: temp_dict(:)
-
-    IF ( .not. ALLOCATED( execute_commands ) ) THEN
-       ! Just allocate the key-value arrays with a size of one
-       ALLOCATE( execute_commands(1) )
-    ELSE
-      ! Confirm that this key does not already exist
-      index = find_execute_command( key )
-      IF ( index .ne. -1 ) THEN
-        WRITE(6,*)'MDI ERROR: Value already exists in execute_command dictionary'
-      END IF
+    !INTEGER                                  :: i, current_code
+    LOGICAL                                  :: end_string
 
-      ! Store the execute_commands data in a temporary array
-      ALLOCATE( temp_dict( SIZE(execute_commands) ) )
-      temp_dict = execute_commands
-      
-      ! Reallocate execute_commands to the correct size
-      DEALLOCATE( execute_commands )
-      ALLOCATE( execute_commands( SIZE(temp_dict) + 1 ) )
-      execute_commands(1:SIZE(temp_dict)) = temp_dict
-      DEALLOCATE( temp_dict )
-    END IF
-
-    ! Add the key-value pair
-    execute_commands( SIZE(execute_commands) )%key = key
-    execute_commands( SIZE(execute_commands) )%value => value
-
-  END SUBROUTINE add_execute_command
-
-  ! Remove a value from the execute_command dictionary
-  SUBROUTINE remove_execute_command(key, ierr)
-    INTEGER, INTENT(IN)                      :: key
-    INTEGER, INTENT(OUT)                     :: ierr
-    INTEGER                                  :: index
-    TYPE(command_func_ptr), ALLOCATABLE      :: temp_dict(:)
-
-    index = find_execute_command( key )
-
-    ! Ensure that this key was actually found in the execute_command dictionary
-    IF ( index .eq. -1 ) THEN
-      ierr = 1
-      RETURN
-    END IF
-
-    ! Store the execute_commands data in a temporary array
-    ALLOCATE( temp_dict( SIZE(execute_commands) ) )
-    temp_dict = execute_commands
-
-    ! Replace the deleted element with the last element
-    temp_dict(index) = temp_dict( SIZE(temp_dict) )
-
-    ! Reallocate execute_commands to the correct size
-    DEALLOCATE( execute_commands )
-    IF ( size(temp_dict) .gt. 1 ) THEN
-      ALLOCATE( execute_commands( SIZE(temp_dict) - 1 ) )
-      execute_commands(1:SIZE(execute_commands)) = temp_dict
-    END IF
-    DEALLOCATE( temp_dict )
-    
+    !current_code = MDI_Get_Current_Code_()
+
+    ! Perform memory cleanup for this code's language-specific data
+    !CALL remove_execute_command( code_id, ierr )
     ierr = 0
 
-  END SUBROUTINE remove_execute_command
+    MDI_On_destroy_code_f = ierr
+
+  END FUNCTION MDI_On_destroy_code_f
+
+  FUNCTION MDI_Execute_Command_f(buf, comm, class_obj) bind(c)
 
-  FUNCTION MDI_Execute_Command_f(buf, comm) bind(c)
     CHARACTER(LEN=1, KIND=C_CHAR), TARGET    :: buf(COMMAND_LENGTH)
     INTEGER(KIND=C_INT), VALUE               :: comm
     INTEGER(KIND=C_INT)                      :: MDI_Execute_Command_f
+    TYPE(C_PTR), VALUE                       :: class_obj
 
     CHARACTER(LEN=COMMAND_LENGTH)        :: fbuf
     INTEGER                                  :: commf
     INTEGER                                  :: ierr
 
     INTEGER                                  :: i, current_code
     LOGICAL                                  :: end_string
 
+    !PROCEDURE(execute_command), POINTER :: this_func => null()
+    PROCEDURE(execute_command_correct), POINTER :: this_func => null()
+    !TYPE(C_FUNPTR), TARGET                      :: this_func_ptr
+    TYPE(C_FUNPTR)                      :: this_func_ptr
+
     commf = comm
 
     ! convert from C string to Fortran string
     fbuf = str_c_to_f(buf, COMMAND_LENGTH)
 
     ! Get the correct execute_command callback
     current_code = MDI_Get_Current_Code_()
-    i = find_execute_command( current_code )
-    IF ( i .eq. -1 ) THEN
-      WRITE(6,*)'MDI Error: Could not locate correct execute_command callback'
-    END IF
-    call execute_commands(i)%value(fbuf, commf, ierr)
-
-    ! If this is the EXIT command, delete all Fortran state associated with the code
-    !IF ( TRIM(fbuf) .eq. "EXIT" ) THEN
-    !  CALL remove_execute_command( current_code )
-    !END IF
 
-    MDI_Execute_Command_f = ierr
+    !ierr = MDI_Get_language_execute_command_(c_loc(this_func_ptr), comm)
+    this_func_ptr = MDI_Get_language_execute_command_(comm)
 
-  END FUNCTION MDI_Execute_Command_f
+    CALL c_f_procpointer(this_func_ptr, this_func)
 
-  FUNCTION MDI_On_destroy_code_f(code_id) bind(c)
-    INTEGER(KIND=C_INT)                      :: MDI_On_destroy_code_f
-    INTEGER                                  :: ierr
-    INTEGER(KIND=C_INT), VALUE               :: code_id
-
-    !INTEGER                                  :: i, current_code
-    LOGICAL                                  :: end_string
+    ierr = this_func(fbuf, commf, class_obj)
 
-    !current_code = MDI_Get_Current_Code_()
-
-    ! Perform memory cleanup for this code's language-specific data
-    CALL remove_execute_command( code_id, ierr )
+    MDI_Execute_Command_f = ierr
 
-    MDI_On_destroy_code_f = ierr
+  END FUNCTION MDI_Execute_Command_f
 
-  END FUNCTION MDI_On_destroy_code_f
 
 END MODULE
 
 
 
 
 
@@ -310,14 +256,19 @@
       MODULE PROCEDURE MDI_Recv_s, &
                        MDI_Recv_d, MDI_Recv_dv, &
                        MDI_Recv_i, MDI_Recv_iv
   END INTERFACE 
 
   INTERFACE
 
+     FUNCTION MDI_Init_code_() bind(c, name="MDI_Init_code")
+       USE, INTRINSIC :: iso_c_binding
+       INTEGER(KIND=C_INT)                      :: MDI_Init_code_
+     END FUNCTION MDI_Init_code_
+
      FUNCTION MDI_Init_with_options_(options) bind(c, name="MDI_Init_with_options")
        USE, INTRINSIC :: iso_c_binding
        CHARACTER(C_CHAR)                        :: options(*)
        INTEGER(KIND=C_INT)                      :: MDI_Init_with_options_
      END FUNCTION MDI_Init_with_options_
 
      FUNCTION MDI_Accept_Communicator_(comm) bind(c, name="MDI_Accept_Communicator")
@@ -496,20 +447,14 @@
 
      FUNCTION MDI_MPI_set_world_comm_(world_comm) bind(c, name="MDI_MPI_set_world_comm")
        USE, INTRINSIC :: iso_c_binding
        TYPE(C_PTR), VALUE                       :: world_comm
        INTEGER(KIND=C_INT)                      :: MDI_MPI_set_world_comm_
      END FUNCTION MDI_MPI_set_world_comm_
 
-     FUNCTION MDI_Get_plugin_mode_(plugin_mode_ptr) bind(c, name="MDI_Get_plugin_mode")
-       USE, INTRINSIC :: iso_c_binding
-       TYPE(C_PTR), VALUE                       :: plugin_mode_ptr
-       INTEGER(KIND=C_INT)                      :: MDI_Get_plugin_mode_
-     END FUNCTION MDI_Get_plugin_mode_
-
      FUNCTION MDI_Plugin_get_argc_(argc_ptr) bind(c, name="MDI_Plugin_get_argc")
        USE, INTRINSIC :: iso_c_binding
        TYPE(C_PTR), VALUE                       :: argc_ptr
        INTEGER(KIND=C_INT)                      :: MDI_Plugin_get_argc_
      END FUNCTION MDI_Plugin_get_argc_
 
      FUNCTION MDI_Plugin_get_args_(args_ptr) bind(c, name="MDI_Plugin_get_args")
@@ -528,51 +473,38 @@
      FUNCTION MDI_Set_plugin_language_(language, state_ptr) bind(c, name="MDI_Set_plugin_language")
        USE, INTRINSIC :: iso_c_binding
        INTEGER(KIND=C_INT), VALUE               :: language
        TYPE(C_PTR), VALUE                       :: state_ptr
        INTEGER(KIND=C_INT)                      :: MDI_Set_plugin_language_
      END FUNCTION MDI_Set_plugin_language_
 
-     FUNCTION MDI_Set_plugin_state_(state_ptr) bind(c, name="MDI_Set_plugin_state")
+     FUNCTION MDI_Set_plugin_state_internal_(state_ptr) bind(c, name="MDI_Set_plugin_state_internal")
        USE, INTRINSIC :: iso_c_binding
        TYPE(C_PTR), VALUE                       :: state_ptr
-       INTEGER(KIND=C_INT)                      :: MDI_Set_plugin_state_
-     END FUNCTION MDI_Set_plugin_state_
+       INTEGER(KIND=C_INT)                      :: MDI_Set_plugin_state_internal_
+     END FUNCTION MDI_Set_plugin_state_internal_
 
   END INTERFACE
 
-
-
 CONTAINS
 
     SUBROUTINE MDI_Init(foptions, ierr)
       USE MDI_INTERNAL
       IMPLICIT NONE
 #if MDI_WINDOWS
       !GCC$ ATTRIBUTES DLLEXPORT :: MDI_Init
       !DEC$ ATTRIBUTES DLLEXPORT :: MDI_Init
 #endif
       CHARACTER(LEN=*), INTENT(IN) :: foptions
       INTEGER, INTENT(OUT) :: ierr
 
-      ierr = MDI_Init_with_options_( TRIM(foptions)//" _language Fortran"//c_null_char )
-
-      ! determine if plugin mode is active
-      ! if this rank has previously run a Fortran plugin, need to remove its state now
-      ! NOTE: Should consider whether the C code can call these at end of MDI_Launch_plugin
-      !ierr2 = MDI_Get_plugin_mode_( c_loc(cplugin_mode) )
-      !plugin_mode = cplugin_mode
-      !IF ( plugin_mode .eq. 1 ) THEN
-      !   current_code = MDI_Get_Current_Code_()
-      !   index = find_execute_command( current_code )
-      !   IF ( index .ne. -1 ) THEN
-      !      CALL remove_execute_command( current_code )
-      !   END IF
-      !ENDIF
+      ierr = MDI_Init_code_()
+      IF ( ierr .ne. 0 ) RETURN
 
+      ierr = MDI_Init_with_options_( TRIM(foptions)//" _language Fortran"//c_null_char )
 
     END SUBROUTINE MDI_Init
 
     SUBROUTINE MDI_Accept_Communicator(communicator, ierr)
       IMPLICIT NONE
 #if MDI_WINDOWS
       !GCC$ ATTRIBUTES DLLEXPORT :: MDI_Accept_Communicator
@@ -770,48 +702,32 @@
       !END IF
 
       ierr = MDI_Send_Command_( c_loc(cbuf), comm)
     END SUBROUTINE MDI_Send_Command
 
     SUBROUTINE MDI_Recv_Command(fbuf, comm, ierr)
       USE ISO_C_BINDING
-      USE MDI_INTERNAL, ONLY : MDI_Get_Current_Code_, remove_execute_command, str_c_to_f, MDI_Get_intra_rank
+      USE MDI_INTERNAL, ONLY : MDI_Get_Current_Code_, str_c_to_f, MDI_Get_intra_rank
 #if MDI_WINDOWS
       !GCC$ ATTRIBUTES DLLEXPORT :: MDI_Recv_Command
       !DEC$ ATTRIBUTES DLLEXPORT :: MDI_Recv_Command
 #endif
       CHARACTER(LEN=*), INTENT(OUT)            :: fbuf
       INTEGER, INTENT(IN)                      :: comm
       INTEGER, INTENT(OUT)                     :: ierr
 
-      INTEGER                                  :: i, current_code
-      LOGICAL                                  :: end_string
       CHARACTER(LEN=1, KIND=C_CHAR), TARGET    :: cbuf(MDI_COMMAND_LENGTH)
 
-      INTEGER                                  :: plugin_mode, ierr2
-      INTEGER(KIND=C_INT), TARGET              :: cplugin_mode
-
       ierr = MDI_Recv_Command_(c_loc(cbuf(1)), comm)
 
-      ! get whether this is code is running in plugin mode
-      ierr2 = MDI_Get_plugin_mode_( c_loc(cplugin_mode) )
-      plugin_mode = cplugin_mode
-
       ! convert from C string to Fortran string
       IF ( MDI_Get_intra_rank() .eq. 0 ) THEN
          fbuf = str_c_to_f(cbuf, MDI_COMMAND_LENGTH)
       END IF
 
-      ! If this is the EXIT command, delete all Fortran state associated with the code
-      !IF ( plugin_mode .eq. 1 ) THEN
-      !  IF ( TRIM(fbuf) .eq. "EXIT" ) THEN
-      !    current_code = MDI_Get_Current_Code_()
-      !    CALL remove_execute_command( current_code )
-      !  END IF
-      !END IF
     END SUBROUTINE MDI_Recv_Command
 
     SUBROUTINE MDI_Conversion_Factor(fin_unit, fout_unit, factor, ierr)
       USE ISO_C_BINDING
 #if MDI_WINDOWS
       !GCC$ ATTRIBUTES DLLEXPORT :: MDI_Conversion_Factor
       !DEC$ ATTRIBUTES DLLEXPORT :: MDI_Conversion_Factor
@@ -1278,56 +1194,55 @@
       END DO
 
       ! convert from C string to Fortran string
       arg = str_c_to_f(carg, LEN(arg))
 
     END SUBROUTINE MDI_Plugin_get_arg
 
-    SUBROUTINE MDI_Set_Execute_Command_Func(command_func, class_obj, ierr)
+    SUBROUTINE MDI_Set_Execute_Command_Func(funptr, class_obj, ierr)
       USE MDI_INTERNAL
 
 #if MDI_WINDOWS
       !GCC$ ATTRIBUTES DLLEXPORT :: MDI_Set_Execute_Command_Func
       !DEC$ ATTRIBUTES DLLEXPORT :: MDI_Set_Execute_Command_Func
 #endif
-      PROCEDURE(execute_command), POINTER        :: command_func
-      TYPE(C_PTR), VALUE                         :: class_obj
-      INTEGER, INTENT(OUT)                       :: ierr
-      INTEGER                                    :: current_code
+      TYPE(C_FUNPTR), VALUE                       :: funptr
+      TYPE(C_PTR), VALUE                          :: class_obj
+      INTEGER, INTENT(OUT)                        :: ierr
+      INTEGER                                     :: current_code
+
 
       current_code = MDI_Get_Current_Code_()
 
-      CALL add_execute_command(current_code, command_func)
+      ierr = MDI_Set_language_execute_command_( funptr )
       ierr = MDI_Set_Execute_Command_Func_c( c_funloc(MDI_Execute_Command_f), class_obj )
 
     END SUBROUTINE MDI_Set_Execute_Command_Func
 
     SUBROUTINE MDI_Set_plugin_state(state_ptr, ierr)
       USE MDI_INTERNAL, ONLY : MDI_On_destroy_code_f, MDI_Set_on_destroy_code_c
 
 #if MDI_WINDOWS
       !GCC$ ATTRIBUTES DLLEXPORT :: MDI_Set_plugin_state
       !DEC$ ATTRIBUTES DLLEXPORT :: MDI_Set_plugin_state
 #endif
       TYPE(C_PTR), VALUE                       :: state_ptr
       INTEGER, INTENT(OUT)                     :: ierr
 
-      INTEGER                                  :: plugin_mode
-      INTEGER(KIND=C_INT), TARGET              :: cplugin_mode
-      INTEGER                                  :: ierr2
-
       INTEGER(KIND=C_INT)                      :: language
 
       language = MDI_LANGUAGE_FORTRAN
-      ierr2 = MDI_Set_plugin_language_(language, state_ptr)
+      ierr = MDI_Set_plugin_language_(language, state_ptr)
+      IF ( ierr .ne. 0 ) RETURN
 
-      ierr = MDI_Set_plugin_state_(state_ptr)
+      ierr = MDI_Init_code_()
+      IF ( ierr .ne. 0 ) RETURN
 
-      ierr2 = MDI_Get_plugin_mode_( c_loc(cplugin_mode) )
-      plugin_mode = cplugin_mode
-      IF ( plugin_mode .eq. 1 ) THEN
-        ierr = MDI_Set_on_destroy_code_c( c_funloc(MDI_On_destroy_code_f) )
-      END IF
+      ierr = MDI_Set_plugin_state_internal_(state_ptr)
+      IF ( ierr .ne. 0 ) RETURN
+
+      ierr = MDI_Set_on_destroy_code_c( c_funloc(MDI_On_destroy_code_f) )
+      IF ( ierr .ne. 0 ) RETURN
 
     END SUBROUTINE MDI_Set_plugin_state
 
 END MODULE
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_general.c` & `pymdi-1.4.9/MDI_Library/mdi_general.c`

 * *Files 8% similar despite different names*

```diff
@@ -10,63 +10,80 @@
 #include "mdi.h"
 #include "mdi_general.h"
 #include "mdi_mpi.h"
 #include "mdi_tcp.h"
 #include "mdi_lib.h"
 #include "mdi_test.h"
 
-/*! \brief Initialize communication through the MDI library
+
+/*! \brief Initialize a new code
  *
- * If using the "-method MPI" option, this function must be called by all ranks.
  * The function returns \p 0 on a success.
  *
- * \param [in]       options
- *                   Options describing the communication method used to connect to codes.
  */
-int general_init(const char* options) {
+int general_init_code() {
+  int ret;
 
   // If this is the first time MDI has initialized, initialize the code vector
-  if ( ! is_initialized ) {
+  if ( ! codes.initialized ) {
     vector_init(&codes, sizeof(code));
   }
 
   // MDI assumes that each call to general_init corresponds to a new code, so create a new code now
   // Note that unless using the LINK communication method, general_init should only be called once
-  current_code = new_code();
-  code* this_code = get_code(current_code);
+  ret = new_code(&codes.current_key);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_init_code: new_code failed");
+    return ret;
+  }
 
-  // If this is the first time MDI has initialized, initialize the method vector
-  //if ( ! is_initialized ) {
+  return 0;
+}
 
-    //vector_init(&methods, sizeof(method));
+
+/*! \brief Initialize communication through the MDI library
+ *
+ * If using the "-method MPI" option, this function must be called by all ranks.
+ * The function returns \p 0 on a success.
+ *
+ * \param [in]       options
+ *                   Options describing the communication method used to connect to codes.
+ */
+int general_init(const char* options) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_init: get_current_code failed");
+    return 1;
+  }
 
   // Create method objects for each supported method
-  if ( enable_tcp_support(current_code) ) {
+  if ( enable_tcp_support(codes.current_key) ) {
     mdi_error("Unable to enable TCP support");
     return 1;
   }
-  if ( enable_mpi_support(current_code) ) {
+  if ( enable_mpi_support(codes.current_key) ) {
     mdi_error("Unable to enable MPI support");
     return 1;
   }
 #if _MDI_PLUGIN_SUPPORT == 1
-  if ( enable_plug_support(current_code) ) {
+  if ( enable_plug_support(codes.current_key) ) {
     mdi_error("Unable to enable plugin support");
     return 1;
   }
 #endif
-  if ( enable_test_support(current_code) ) {
+  if ( enable_test_support(codes.current_key) ) {
     mdi_error("Unable to enable TEST support");
     return 1;
   }
 
-  //}
-
   char* strtol_ptr;
-  int i, ret;
+  int i;
 
   // values acquired from the input options
   char* role;
   char* method_str;
   char* output_file;
   char* language_argument = ((char*)"");
   int has_role = 0;
@@ -139,29 +156,29 @@
     }
     //-hostname
     else if (strcmp(argv[iarg],"-hostname") == 0){
       if (iarg+2 > argc) {
         mdi_error("Error in MDI_Init: Argument missing from -hostname option");
         return 1;
       }
-      hostname = argv[iarg+1];
+      this_code->hostname = argv[iarg+1];
       iarg += 2;
     }
     //-port
     else if (strcmp(argv[iarg],"-port") == 0) {
       if (iarg+2 > argc) {
         mdi_error("Error in MDI_Init: Argument missing from -port option");
         return 1;
       }
-      port = strtol( argv[iarg+1], &strtol_ptr, 10 );
+      this_code->port = strtol( argv[iarg+1], &strtol_ptr, 10 );
       iarg += 2;
     }
     //-ipi
     else if (strcmp(argv[iarg],"-ipi") == 0) {
-      ipi_compatibility = 1;
+      this_code->ipi_compatibility = 1;
       iarg += 1;
     }
     //-out
     else if (strcmp(argv[iarg],"-out") == 0) {
       if (iarg+2 > argc) {
         mdi_error("Error in MDI_Init: Argument missing from -out option");
         return 1;
@@ -225,36 +242,42 @@
     mdi_error("Error in MDI_Init: -method option not provided");
     return 1;
   }
 
   // if this is a plugin, get the langauge from the shared value
   if ( strcmp(method_str, "LINK") == 0 || strcmp(method_str, "PLUG") == 0 ) {
     if ( strcmp(this_code->role, "ENGINE") == 0 ) {
-      this_code->language = shared_state_from_driver->engine_language;
+      plugin_shared_state* shared_state = (plugin_shared_state*) this_code->shared_state_from_driver;
+      this_code->language = shared_state->engine_language;
     }
   }
 
   // determine the method id of the method selected by the user
   if ( strcmp(method_str, "TCP") == 0 ) {
-    selected_method_id = MDI_TCP;
+    this_code->selected_method_id = MDI_TCP;
   }
   else if ( strcmp(method_str, "MPI") == 0 ) {
-    selected_method_id = MDI_MPI;
+    this_code->selected_method_id = MDI_MPI;
   }
   else if ( strcmp(method_str, "LINK") == 0 || strcmp(method_str, "PLUG") == 0 ) {
-    selected_method_id = MDI_LINK;
+    this_code->selected_method_id = MDI_LINK;
   }
   else if ( strcmp(method_str, "TEST") == 0 ) {
-    selected_method_id = MDI_TEST;
+    this_code->selected_method_id = MDI_TEST;
   }
   else {
     mdi_error("Error in MDI_Init: Method not recognized");
     return 1;
   }
-  method* selected_method = get_method(current_code, selected_method_id);
+  method* selected_method;
+  ret = get_method(codes.current_key, this_code->selected_method_id, &selected_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_init: get_method failed");
+    return ret;
+  }
 
   // ensure that a valid role has been provided
   if ( strcmp(this_code->role, "DRIVER") != 0 &&
        strcmp(this_code->role, "ENGINE") != 0 ) {
     mdi_error("Error in MDI_Init: Role not recognized");
     return 1;
   }
@@ -262,47 +285,49 @@
   // redirect the standard output
   if ( has_output_file == 1 ) {
     freopen(output_file, "w", stdout);
   }
 
   // ensure that the name of this code is not the same as the name of any of the other codes
   for (i = 0; i < codes.size; i++) {
-    if ( i != current_code ) {
-      code* other_code = vector_get(&codes, i);
+    if ( i != codes.current_key ) {
+      code* other_code;
+      ret = vector_get(&codes, i, (void**)&other_code);
       if (strcmp(this_code->name, other_code->name) == 0) {
-	mdi_error("MDI_Init found multiple codes with the same name");
-	return 1;
+        mdi_error("MDI_Init found multiple codes with the same name");
+        return 1;
       }
     }
   }
 
   // ensure that at most one driver has been initialized
   if ( strcmp(this_code->role, "DRIVER") == 0 ) {
     for (i = 0; i < codes.size; i++) {
-      if ( i != current_code ) {
-	code* other_code = vector_get(&codes, i);
-	if (strcmp(this_code->role, other_code->role) == 0) {
-	  mdi_error("MDI_Init found multiple drivers");
-	  return 1;
-	}
+      if ( i != codes.current_key ) {
+        code* other_code;
+        ret = vector_get(&codes, i, (void**)&other_code);
+        if (strcmp(this_code->role, other_code->role) == 0) {
+          mdi_error("MDI_Init found multiple drivers");
+          return 1;
+        }
       }
     }
   }
 
   // Initialize this code's intra-rank
   // If using the MPI method, this value may change
   int mpi_init_flag;
   if ( MPI_Initialized(&mpi_init_flag) ) {
     mdi_error("Error in MDI_Init: MPI_Initialized failed");
     return 1;
   }
   if ( mpi_init_flag == 1 && this_code->language != MDI_LANGUAGE_PYTHON ) {
-    MPI_Comm_rank(MPI_COMM_WORLD, &world_rank);
-    MPI_Comm_size(MPI_COMM_WORLD, &world_size);
-    this_code->intra_rank = world_rank;
+    MPI_Comm_rank(MPI_COMM_WORLD, &this_code->world_rank);
+    MPI_Comm_size(MPI_COMM_WORLD, &this_code->world_size);
+    this_code->intra_rank = this_code->world_rank;
   }
 
   // Execute the on_selection() function for the user-selected method
   if ( selected_method->on_selection() ) {
     mdi_error("MDI method on_selection function failed");
     return 1;
   }
@@ -317,15 +342,28 @@
 /*! \brief Accept a new MDI communicator
  *
  * The function returns an MDI_Comm that describes a connection between two codes.
  * If no new communicators are available, the function returns \p MDI_COMM_NULL.
  *
  */
 int general_accept_communicator() {
-  method* selected_method = get_method(current_code, selected_method_id);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_accept_communicator: get_current_code failed");
+    return 1;
+  }
+  method* selected_method;
+  ret = get_method(codes.current_key, this_code->selected_method_id, &selected_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_accept_communicator: get_method failed");
+    return ret;
+  }
   return selected_method->on_accept_communicator();
 }
 
 
 /*! \brief Send a message through the MDI connection
  *
  * If running with MPI, this function must be called only by rank \p 0.
@@ -337,23 +375,34 @@
  *                   Number of values (integers, double precision floats, characters, etc.) to be sent.
  * \param [in]       datatype
  *                   MDI handle (MDI_INT, MDI_DOUBLE, MDI_CHAR, etc.) corresponding to the type of data to be sent.
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int general_send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm) {
-  int ret = 0;
+  int ret;
 
-  communicator* this = get_communicator(current_code, comm);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_send: get_current_code failed");
+    return 1;
+  }
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_send: get_communicator failed");
+    return ret;
+  }
 
   // send message header information
   // only do this if communicating with MDI version 1.1 or higher
   if ( ( this->mdi_version[0] > 1 ||
          ( this->mdi_version[0] == 1 && this->mdi_version[1] >= 1 ) )
-       && ipi_compatibility != 1 ) {
+       && this_code->ipi_compatibility != 1 ) {
 
     // prepare the header information
     size_t nheader = 4;
     int* header = (int*) malloc( nheader * sizeof(int) );
     header[0] = 0;        // error flag
     header[1] = 0;        // header type
     header[2] = datatype; // datatype
@@ -392,21 +441,32 @@
   int ret = 0;
 
   // Actual datatype of data sent to this code
   // This will be read from the message header, and might be different from datatype
   int send_datatype = datatype;
   size_t send_datasize;
 
-  communicator* this = get_communicator(current_code, comm);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_recv: get_current_code failed");
+    return 1;
+  }
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_recv: get_communicator failed");
+    return ret;
+  }
 
   // receive message header information
   // only do this if communicating with MDI version 1.1 or higher
   if ( ( this->mdi_version[0] > 1 ||
          ( this->mdi_version[0] == 1 && this->mdi_version[1] >= 1 ) )
-       && ipi_compatibility != 1 ) {
+       && this_code->ipi_compatibility != 1 ) {
 
     // prepare buffer to hold header information
     size_t nheader = 4;
     int* header = (int*) malloc( nheader * sizeof(int) );
 
     // initialize the header with the expected data
     // this is important when ranks other than 0 call this function
@@ -490,26 +550,41 @@
  *
  * \param [in]       buf
  *                   Pointer to the data to be sent.
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int general_send_command(const char* buf, MDI_Comm comm) {
-  code* this_code = get_code(current_code);
-  method* selected_method = get_method(current_code, selected_method_id);
-  communicator* this = get_communicator(current_code, comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_send_command: get_current_code failed");
+    return 1;
+  }
+  method* selected_method;
+  ret = get_method(codes.current_key, this_code->selected_method_id, &selected_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_send_command: get_method failed");
+    return ret;
+  }
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_send_command: get_communicator failed");
+    return ret;
+  }
 
   // For the count, use the smaller of MDI_COMMAND_LENGTH between the two codes
   int count = MDI_COMMAND_LENGTH_;
   if ( this->command_length < MDI_COMMAND_LENGTH_ ) {
     count = this->command_length;
   }
 
-  //const char* command = buf;
-  int ret = 0;
   int skip_flag = 0;
 
   // Copy the command
   char* command = malloc( count * sizeof(char) );
   int ichar;
   for ( ichar=0; ichar < count; ichar++) {
     command[ichar] = '\0';
@@ -543,77 +618,91 @@
   return ret;
 }
 
 
 /*! \brief Respond to a general built-in command
  *
  * If running with MPI, this function must be called only by rank \p 0.
- * The function returns \p 1 if the command is a built-in command and \p 0 otherwise.
+ * The function returns \p 0 on success.
  *
  * \param [in]       buf
  *                   Pointer to the buffer for the command name.
  * \param [in]       comm
  *                   MDI communicator associated with the connection to the sending code.
+ * \param [in]       flag
+ *                   Returns \p 1 if the command is a built-in command and \p 0 otherwise.
  */
-int general_builtin_command(const char* buf, MDI_Comm comm) {
+int general_builtin_command(const char* buf, MDI_Comm comm, int* flag) {
   int ret = 0;
+  *flag = 0;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_builtin_command: get_current_code failed");
+    return 1;
+  }
 
   // check if this command corresponds to one of MDI's standard built-in commands
   if ( strcmp( buf, "<NAME" ) == 0 ) {
-    code* this_code = get_code(current_code);
-    communicator* this_comm = get_communicator(current_code, comm);
+    communicator* this_comm;
+    ret = get_communicator(codes.current_key, comm, &this_comm);
+    if ( ret != 0 ) {
+      mdi_error("Error in general_builtin_command: get_communicator failed");
+      return ret;
+    }
 
     // For the count, use the smaller of MDI_NAME_LENGTH between the two codes
     int count = MDI_NAME_LENGTH_;
     if ( this_comm->name_length < MDI_NAME_LENGTH_ ) {
       count = this_comm->name_length;
     }
 
     MDI_Send(this_code->name, count, MDI_CHAR, comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<VERSION" ) == 0 ) {
     int version[3];
     version[0] = MDI_MAJOR_VERSION;
     version[1] = MDI_MINOR_VERSION;
     version[2] = MDI_PATCH_VERSION;
     MDI_Send(&version[0], 3, MDI_INT, comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<COMMANDS" ) == 0 ) {
     send_command_list(comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<CALLBACKS" ) == 0 ) {
     send_callback_list(comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<NODES" ) == 0 ) {
     send_node_list(comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<NCOMMANDS" ) == 0 ) {
     send_ncommands(comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<NCALLBACKS" ) == 0 ) {
     send_ncallbacks(comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "<NNODES" ) == 0 ) {
     send_nnodes(comm);
-    ret = 1;
+    *flag = 1;
   }
   else if ( strcmp( buf, "EXIT" ) == 0 ) {
     // if the MDI Library called MPI_Init, call MPI_Finalize now
-    if ( initialized_mpi == 1 ) {
+    if ( this_code->initialized_mpi == 1 ) {
       MPI_Finalize();
     }
   }
-  return ret;
+  return 0;
 }
 
 
 /*! \brief Receive a command of length \p MDI_COMMAND_LENGTH through the MDI connection
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
@@ -621,17 +710,33 @@
  * \param [in]       buf
  *                   Pointer to the buffer where the received data will be stored.
  * \param [in]       comm
  *                   MDI communicator associated with the connection to the sending code.
  */
 int general_recv_command(char* buf, MDI_Comm comm) {
   int ret;
-  code* this_code = get_code(current_code);
-  communicator* this = get_communicator(current_code, comm);
-  method* selected_method = get_method(current_code, selected_method_id);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_recv_command: get_current_code failed");
+    return 1;
+  }
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_recv_command: get_communicator failed");
+    return ret;
+  }
+  method* selected_method;
+  ret = get_method(codes.current_key, this_code->selected_method_id, &selected_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in general_recv_command: get_method failed");
+    return ret;
+  }
 
   ret = selected_method->on_recv_command(comm);
   if ( ret != 0 ) {
     mdi_error("MDI Recv Command error: method-specific on_recv_command() function failed");
     return ret;
   }
 
@@ -651,15 +756,20 @@
   ret = general_recv( buf, count, datatype, comm );
   if ( ret != 0 ) {
     mdi_error("Error in MDI_Recv_Command: Unable to receive command");
     return ret;
   }
 
   // check if this command corresponds to one of MDI's standard built-in commands
-  int builtin_flag = general_builtin_command(buf, comm);
+  int builtin_flag;
+  ret = general_builtin_command(buf, comm, &builtin_flag);
+  if ( ret != 0 ) {
+    mdi_error("Error in MDI_Recv_Command: Built-in command failed");
+    return ret;
+  }
   if ( builtin_flag == 1 ) {
     return general_recv_command(buf, comm);
   }
   else if ( builtin_flag != 0 ) {
     mdi_error("Error in MDI_Recv_Command: Unable to respond to builtin command");
     return builtin_flag;
   }
@@ -675,28 +785,40 @@
  * \param [in]       node_vec
  *                   Vector of nodes, into which the new node will be added.
  * \param [in]       node_name
  *                   Name of the node.
  */
 int register_node(vector* node_vec, const char* node_name)
 {
+  int ret;
+
   // only register on rank 0
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_node: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) >= MDI_COMMAND_LENGTH_ ) {
     mdi_error("Cannot register node name with length greater than MDI_COMMAND_LENGTH");
     return 1;
   }
 
   // confirm that this node is not already registered
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_node: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index != -1 ) {
     mdi_error("This node is already registered"); 
     return 1;
   }
 
   node new_node;
   vector* command_vec = malloc(sizeof(vector));
@@ -724,16 +846,23 @@
  * \param [in]       node_name
  *                   Name of the node on which the command will be registered.
  * \param [in]       command_name
  *                   Name of the command.
  */
 int register_command(vector* node_vec, const char* node_name, const char* command_name)
 {
+  int ret;
+
   // only register on rank 0
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_command: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) >= MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
@@ -743,23 +872,34 @@
   // confirm that the command_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(command_name) >= MDI_COMMAND_LENGTH_ ) {
     mdi_error("Cannot register command name with length greater than MDI_COMMAND_LENGTH");
     return 1;
   }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_command: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("Attempting to register a command on an unregistered node");
     return 1;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get(node_vec, node_index, (void**)&target_node);
 
   // confirm that this command is not already registered
-  int command_index = get_command_index(target_node, command_name);
+  int command_index;
+  ret = get_command_index(target_node, command_name, &command_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_command: get_command_index failed"); 
+    return 1;
+  }
   if ( command_index != -1 ) {
     mdi_error("This command is already registered for this node");
     return 1;
   }
 
   // register this command
   char new_command[MDI_COMMAND_LENGTH_];
@@ -783,16 +923,23 @@
  * \param [in]       node_name
  *                   Name of the node on which the callback will be registered.
  * \param [in]       callback_name
  *                   Name of the callback.
  */
 int register_callback(vector* node_vec, const char* node_name, const char* callback_name)
 {
+  int ret;
+
   // only register on rank 0
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_callback: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
   // confirm that the node_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(node_name) >= MDI_COMMAND_LENGTH_ ) {
     mdi_error("Node name is greater than MDI_COMMAND_LENGTH");
@@ -802,23 +949,34 @@
   // confirm that the callback_name size is not greater than MDI_COMMAND_LENGTH
   if ( strlen(callback_name) >= MDI_COMMAND_LENGTH_ ) {
     mdi_error("Cannot register callback name with length greater than MDI_COMMAND_LENGTH");
     return 1;
   }
 
   // find the node
-  int node_index = get_node_index(node_vec, node_name);
+  int node_index;
+  ret = get_node_index(node_vec, node_name, &node_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_callback: get_node_index failed"); 
+    return 1;
+  }
   if ( node_index == -1 ) {
     mdi_error("Attempting to register a callback on an unregistered node");
     return 1;
   }
-  node* target_node = vector_get(node_vec, node_index);
+  node* target_node;
+  ret = vector_get(node_vec, node_index, (void**)&target_node);
 
   // confirm that this callback is not already registered
-  int callback_index = get_callback_index(target_node, callback_name);
+  int callback_index;
+  ret = get_callback_index(target_node, callback_name, &callback_index);
+  if ( ret != 0 ) {
+    mdi_error("Error in register_callback: get_callback_index failed"); 
+    return 1;
+  }
   if ( callback_index != -1 ) {
     mdi_error("This callback is already registered for this node");
     return 1;
   }
 
   // register this callback
   char new_callback[MDI_COMMAND_LENGTH_];
@@ -838,16 +996,28 @@
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int send_command_list(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
-  communicator* this_comm = get_communicator(current_code, comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_command_list: get_current_code failed");
+    return 1;
+  }
+  communicator* this_comm;
+  ret = get_communicator(codes.current_key, comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_command_list: get_communicator failed");
+    return ret;
+  }
 
   if ( this_code->intra_rank != 0 ) {
     mdi_error("Attempting to send command information from the incorrect rank");
     return 1;
   }
   
   // Use the smaller of MDI_COMMAND_LENGTH between the two codes
@@ -859,27 +1029,29 @@
   int ncommands = 0;
   int nnodes = (int)this_code->nodes->size;
   int inode, icommand;
   int stride = clength + 1;
 
   // determine the number of commands
   for (inode = 0; inode < nnodes; inode++) {
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     ncommands += (int)this_node->commands->size;
   }
 
   // allocate memory for the commands list
   int count = ( ncommands + nnodes ) * stride;
   char* commands = malloc( count * sizeof(char) );
 
   // form the list of commands
   int islot = 0;
   for (inode = 0; inode < nnodes; inode++) {
     // add the name of this node to the list
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     int length = (int)strlen(this_node->name);
     snprintf(&commands[ islot * stride ], clength, "%s", this_node->name);
     int ichar;
     for (ichar = length; ichar < stride-1; ichar++) {
       commands[ islot * stride + ichar ] = ' ';
     }
     if ( this_node->commands->size > 0 ) {
@@ -888,15 +1060,16 @@
     else {
       commands[ islot * stride + stride - 1 ] = ';';
     }
     islot++;
 
     // add the commands for this node
     for (icommand = 0; icommand < this_node->commands->size; icommand++) {
-      char* command = vector_get(this_node->commands, icommand);
+      char* command;
+      ret = vector_get(this_node->commands, icommand, (void**)&command);
       length = (int)strlen(command);
       snprintf(&commands[ islot * stride ], clength, "%s", command);
       for (ichar = length; ichar < stride-1; ichar++) {
 	commands[ islot * stride + ichar ] = ' ';
       }
       if ( icommand == this_node->commands->size - 1 ) {
 	commands[ islot * stride + stride - 1 ] = ';';
@@ -904,31 +1077,43 @@
       else {
 	commands[ islot * stride + stride - 1 ] = ',';
       }
       islot++;
     }
   }
 
-  int ret = general_send( commands, count, MDI_CHAR, comm );
+  ret = general_send( commands, count, MDI_CHAR, comm );
   free( commands );
   return ret;
 }
 
 
 /*! \brief Send the list of callbacks
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int send_callback_list(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
-  communicator* this_comm = get_communicator(current_code, comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_callback_list: get_current_code failed");
+    return ret;
+  }
+  communicator* this_comm;
+  ret = get_communicator(codes.current_key, comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_callback_list: get_communicator failed");
+    return ret;
+  }
 
   if ( this_code->intra_rank != 0 ) {
     mdi_error("Attempting to send callback information from the incorrect rank");
     return 1;
   }
   int ncallbacks = 0;
   int nnodes = (int)this_code->nodes->size;
@@ -940,15 +1125,16 @@
     clength = this_comm->command_length;
   }
   
   int stride = clength + 1;
 
   // determine the number of callbakcs
   for (inode = 0; inode < nnodes; inode++) {
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     ncallbacks += (int)this_node->callbacks->size;
   }
 
   // allocate memory for the callbacks list
   int count = ( ncallbacks + nnodes ) * stride;
   char* callbacks = malloc( count * sizeof(char) );
   int ichar;
@@ -956,15 +1142,16 @@
     callbacks[ichar] = '\0';
   }
 
   // form the list of callbacks
   int islot = 0;
   for (inode = 0; inode < nnodes; inode++) {
     // add the name of this node to the list
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     int length = (int)strlen(this_node->name);
     snprintf(&callbacks[ islot * stride ], clength, "%s", this_node->name);
     int ichar;
     for (ichar = length; ichar < stride-1; ichar++) {
       callbacks[ islot * stride + ichar ] = ' ';
     }
     if ( this_node->callbacks->size > 0 ) {
@@ -973,15 +1160,16 @@
     else {
       callbacks[ islot * stride + stride - 1 ] = ';';
     }
     islot++;
 
     // add the callbacks for this node
     for (icallback = 0; icallback < this_node->callbacks->size; icallback++) {
-      char* callback = vector_get(this_node->callbacks, icallback);
+      char* callback;
+      ret = vector_get(this_node->callbacks, icallback, (void**)&callback);
       length = (int)strlen(callback);
       snprintf(&callbacks[ islot * stride ], clength, "%s", callback);
       for (ichar = length; ichar < stride-1; ichar++) {
 	callbacks[ islot * stride + ichar ] = ' ';
       }
       if ( icallback == this_node->callbacks->size - 1 ) {
 	callbacks[ islot * stride + stride - 1 ] = ';';
@@ -989,31 +1177,43 @@
       else {
 	callbacks[ islot * stride + stride - 1 ] = ',';
       }
       islot++;
     }
   }
 
-  int ret = general_send( callbacks, count, MDI_CHAR, comm );
+  ret = general_send( callbacks, count, MDI_CHAR, comm );
   free( callbacks );
   return ret;
 }
 
 
 /*! \brief Send the list of nodes
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int send_node_list(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
-  communicator* this_comm = get_communicator(current_code, comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_node_list: get_current_code failed");
+    return 1;
+  }
+  communicator* this_comm;
+  ret = get_communicator(codes.current_key, comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_node_list: get_communicator failed");
+    return ret;
+  }
 
   if ( this_code->intra_rank != 0 ) {
     mdi_error("Attempting to send node information from the incorrect rank");
     return 1;
   }
   int nnodes = (int)this_code->nodes->size;
   int inode;
@@ -1029,122 +1229,153 @@
   // allocate memory for the node list
   int count = nnodes * stride;
   char* node_list = malloc( count * sizeof(char) );
 
   // form the list of nodes
   for (inode = 0; inode < nnodes; inode++) {
     // add the name of this node to the list
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     int length = (int)strlen(this_node->name);
     if ( strlen(this_node->name) >= MDI_COMMAND_LENGTH_ ) {
       mdi_error("Error in send_node_list: Node name is larger than MDI_COMMAND_LENGTH");
       return 1;
     }
     snprintf(&node_list[ inode * stride ], clength, "%s", this_node->name);
     int ichar;
     for (ichar = length; ichar < stride-1; ichar++) {
       node_list[ inode * stride + ichar ] = ' ';
     }
     node_list[ inode * stride + stride - 1 ] = ',';
   }
 
-  int ret = general_send( node_list, count, MDI_CHAR, comm );
+  ret = general_send( node_list, count, MDI_CHAR, comm );
   free( node_list );
   return ret;
 }
 
 
 /*! \brief Send the number of supported commands
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int send_ncommands(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_ncommands: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     mdi_error("Attempting to send command information from the incorrect rank");
     return 1;
   }
   int ncommands = 0;
   int nnodes = (int)this_code->nodes->size;
   int inode;
 
   // determine the number of commands
   for (inode = 0; inode < nnodes; inode++) {
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     ncommands += (int)this_node->commands->size;
   }
 
-  int ret = general_send( &ncommands, 1, MDI_INT, comm );
+  ret = general_send( &ncommands, 1, MDI_INT, comm );
   return ret;
 }
 
 
 /*! \brief Send the number of supported callbacks
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int send_ncallbacks(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_ncallbacks: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     mdi_error("Attempting to send callback information from the incorrect rank");
     return 1;
   }
   int ncallbacks = 0;
   int nnodes = (int)this_code->nodes->size;
   int inode;
 
   // determine the number of callbacks
   for (inode = 0; inode < nnodes; inode++) {
-    node* this_node = vector_get(this_code->nodes, inode);
+    node* this_node;
+    ret = vector_get(this_code->nodes, inode, (void**)&this_node);
     ncallbacks += (int)this_node->callbacks->size;
   }
 
-  int ret = general_send( &ncallbacks, 1, MDI_INT, comm );
+  ret = general_send( &ncallbacks, 1, MDI_INT, comm );
   return ret;
 }
 
 
 /*! \brief Send the number of supported nodes
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int send_nnodes(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in send_nnodes: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     mdi_error("Attempting to send callback information from the incorrect rank");
     return 1;
   }
   int nnodes = (int)this_code->nodes->size;
-  int ret = general_send( &nnodes, 1, MDI_INT, comm );
+  ret = general_send( &nnodes, 1, MDI_INT, comm );
   return ret;
 }
 
 
 /*! \brief Get information about the nodes of a particular code
  *
  * If running with MPI, this function must be called only by rank \p 0.
  * The function returns \p 0 on a success.
  *
  * \param [in]       comm
  *                   MDI communicator associated with the connection to the sending code.
  */
 int get_node_info(MDI_Comm comm) {
-  communicator* this = get_communicator(current_code, comm);
+  int ret;
+
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in get_node_info: get_communicator failed");
+    return ret;
+  }
 
   // Use the smaller of MDI_COMMAND_LENGTH between the two codes
   int clength = MDI_COMMAND_LENGTH_;
   if ( this->command_length < MDI_COMMAND_LENGTH_ ) {
     clength = this->command_length;
   }
 
@@ -1341,33 +1572,44 @@
  *
  * The function returns the node vector for the communicator.
  *
  * \param [in]       comm
  *                   MDI communicator of the engine.  If comm is set to 
  *                   MDI_COMM_NULL, the function will return the node vector for the calling engine.
  */
-vector* get_node_vector(MDI_Comm comm) {
+int get_node_vector(MDI_Comm comm, vector** vector_ptr) {
+  int ret;
+
   // get the vector of nodes associated with the communicator
   vector* node_vec;
-  code* this_code = get_code(current_code);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in get_node_vector: get_current_code failed");
+    return ret;
+  }
   if ( comm == MDI_COMM_NULL ) {
     node_vec = this_code->nodes;
   }
   else {
-    communicator* this = get_communicator(current_code, comm);
+    communicator* this;
+    ret = get_communicator(codes.current_key, comm, &this);
+    if ( ret != 0 ) {
+      mdi_error("Error in get_node_vector: get_communicator failed");
+      return ret;
+    }
     if ( this->method_id == MDI_LINK ) {
-      // get the engine code to which this communicator connects
       library_data* libd = (library_data*) this->method_data;
-      int iengine = libd->connected_code;
-      code* engine_code = get_code(iengine);
-      node_vec = engine_code->nodes;
+      node_vec = (vector*)libd->shared_state->engine_nodes;
     }
     else {
       if ( this->nodes->size == 0 ) {
         // acquire node information for this communicator
         get_node_info(comm);
       }
       node_vec = this->nodes;
     }
   }
-  return node_vec;
+  *vector_ptr = node_vec;
+  return 0;
 }
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_general.h` & `pymdi-1.4.9/MDI_Library/mdi_general.h`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,30 @@
 
 #ifndef MDI_GENERAL
 #define MDI_GENERAL
 
 #include "mdi.h"
 #include "mdi_global.h"
 
-/*! \brief Function pointer to the generic execute_command function */
-extern int (*execute_command)(const char*, MDI_Comm);
-
+int general_init_code();
 int general_init(const char* options);
 int general_accept_communicator();
 int general_send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm);
 int general_recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm);
 int general_send_command(const char* buf, MDI_Comm comm);
 int general_recv_command(char* buf, MDI_Comm comm);
-int general_builtin_command(const char* buf, MDI_Comm comm);
+int general_builtin_command(const char* buf, MDI_Comm comm, int* flag);
 
 int register_node(vector* node_vec, const char* node_name);
 int register_command(vector* node_vec, const char* node_name, const char* command_name);
 int register_callback(vector* node_vec, const char* node_name, const char* callback_name);
 
 int send_command_list(MDI_Comm comm);
 int send_callback_list(MDI_Comm comm);
 int send_node_list(MDI_Comm comm);
 int send_ncommands(MDI_Comm comm);
 int send_ncallbacks(MDI_Comm comm);
 int send_nnodes(MDI_Comm comm);
 int get_node_info(MDI_Comm comm);
-vector* get_node_vector(MDI_Comm comm);
+int get_node_vector(MDI_Comm comm, vector** vector_ptr);
 
 #endif
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_global.c` & `pymdi-1.4.9/MDI_Library/mdi_global.c`

 * *Files 7% similar despite different names*

```diff
@@ -14,103 +14,47 @@
   #include <unistd.h>
 #endif
 #include <stdint.h>
 #include "mdi_global.h"
 
 /*! \brief Vector containing all codes that have been initiailized on this rank
  * Typically, this will only include a single code, unless the communication method is LIBRARY */
-vector codes;
+vector codes = { .initialized = 0 };
 
-/*! \brief Vector containing all supported methods */
-vector methods;
-
-/*! \brief ID of the method being used for inter-code communication */
-int selected_method_id = 0;
-
-/*! \brief Index of the active code */
-int current_code = 0;
-
-/*! \brief Flag for whether MDI is running in i-PI compatibility mode */
-int ipi_compatibility = 0;
-
-/*! \brief Flag for whether MDI has been previously initialized */
-int is_initialized = 0;
-
-/*! \brief Flag for whether MDI called MPI_Init */
-int initialized_mpi = 0;
-
-/*! \brief Flag for whether MDI is currently operating in plugin mode */
-int plugin_mode = 0;
-
-/*! \brief Internal copy of MPI_COMM_WORLD, used when MDI initializes MPI */
-MPI_Comm mdi_mpi_comm_world;
-
-/*! \brief Unedited command-line options for currently running plugin */
-char* plugin_unedited_options = NULL;
-
-/*! \brief Argument count for plugin command-line options */
-int plugin_argc = 0;
-
-/*! \brief Argument vector for plugin command-line options */
-char** plugin_argv = NULL;
-
-/*! \brief Python callback pointer for MPI_Recv */
-int (*mpi4py_recv_callback)(void*, int, int, int, MDI_Comm_Type);
-
-/*! \brief Python callback pointer for MPI_Send */
-int (*mpi4py_send_callback)(void*, int, int, int, MDI_Comm_Type);
-
-/*! \brief Python callback pointer for initial MPI allgather */
-int (*mpi4py_allgather_callback)(void*, void*);
-
-/*! \brief Python callback pointer for gathering names */
-int (*mpi4py_gather_names_callback)(void*, void*, int*, int*);
-
-/*! \brief Python callback pointer for MPI_Comm_split */
-int (*mpi4py_split_callback)(int, int, MDI_Comm_Type, int);
-
-/*! \brief Python callback pointer for MPI_Comm_rank */
-int (*mpi4py_rank_callback)(int);
-
-/*! \brief Python callback pointer for MPI_Comm_size */
-int (*mpi4py_size_callback)(int);
-
-/*! \brief Python callback pointer for MPI_Comm_barrier */
-int (*mpi4py_barrier_callback)(int);
-
-/*! \brief Size of MPI_COMM_WORLD */
-int world_size = -1;
-
-/*! \brief Rank of this process within MPI_COMM_WORLD */
-int world_rank = -1;
 
 /*! \brief Initialize memory allocation for a vector structure
  *
+ * The function returns \p 0 on a success.
+ *
  * \param [in]       v
  *                   Pointer to the vector structure for which the memory will be allocated
  * \param [in]       stride
  *                   Stride of the vector
  */
 int vector_init(vector* v, size_t stride) {
   //initialize the vector with the given stride
   v->data = malloc(0);
   if (!v->data) {
-    perror("Could not initialize vector");
-    exit(-1);
+    mdi_error("Could not initialize vector");
+    return 1;
   }
 
   v->size = 0;
   v->capacity = 0;
   v->stride = stride;
+  v->current_key = -1;
+  v->initialized = 1;
 
   return 0;
 }
 
 /*! \brief Append a new element to the end of the vector
  *
+ * The function returns \p 0 on a success.
+ *
  * \param [in]       v
  *                   Pointer to the vector to which the element will be appended
  * \param [in]       element
  *                   Pointer to the element that will be appended to the vector
  */
 int vector_push_back(vector* v, void* element) {
   //grow the vector
@@ -134,14 +78,16 @@
   v->size++;
 
   return 0;
 }
 
 /*! \brief Remove an element from a vector
  *
+ * The function returns \p 0 on a success.
+ *
  * \param [in]       v
  *                   Pointer to the vector from which the element will be removed
  * \param [in]       index
  *                   Index of the element that will be removed from the vector
  */
 int vector_delete(vector* v, int index) {
   // copy the data from the last element to the element that is being deleted
@@ -162,101 +108,138 @@
   }
 
   return 0;
 }
 
 /*! \brief Free all data associated with a vector
  *
+ * The function returns \p 0 on a success.
+ *
  * \param [in]       v
  *                   Pointer to the vector that will be freed
  */
 int vector_free(vector* v) {
   free(v->data);
   free(v);
   return 0;
 }
 
 /*! \brief Return a pointer to an element of a vector
  *
+ * The function returns \p 0 on a success.
+ *
  * \param [in]       v
  *                   Pointer to the vector
  * \param [in]       index
  *                   Index of the element within the vector
  */
-void* vector_get(vector* v, int index) {
+int vector_get(vector* v, int index, void** element) {
   if (index < 0 || index >= v->size) {
     mdi_error("Vector accessed out-of-bounds");
-    return NULL;
+    return 1;
   }
-  return ( void* )( v->data + (index * v->stride) );
+  *element = ( void* )( v->data + (index * v->stride) );
+  return 0;
 }
 
 /*! \brief Determine the index of a node within a vector of nodes
  *
  * \param [in]       v
  *                   Pointer to the vector
  * \param [in]       node_name
  *                   Name of the node
  */
-int get_node_index(vector* v, const char* node_name) {
+int get_node_index(vector* v, const char* node_name, int* node_index) {
+  int ret;
   int inode;
-  int node_index = -1;
+  int correct_node = -1;
   for ( inode = 0; inode < v->size; inode++ ) {
-    node* this_node = vector_get(v, inode);
+    node* this_node;
+    ret = vector_get(v, inode, (void**)&this_node);
+    if ( ret != 0 ) {
+      mdi_error("Error in get_node_index: vector_get failed");
+      return 1;
+    }
     if ( strcmp( node_name, this_node->name ) == 0 ) {
-      node_index = inode;
+      correct_node = inode;
     }
   }
-  return node_index;
+  *node_index = correct_node;
+  return 0;
 }
 
 /*! \brief Determine the index of a command within a node
  *
  * \param [in]       node
  *                   Pointer to the node
  * \param [in]       command_name
  *                   Name of the command
  */
-int get_command_index(node* n, const char* command_name) {
+int get_command_index(node* n, const char* command_name, int* command_index) {
+  int ret;
   int icommand;
-  int command_index = -1;
+  int correct_command = -1;
+  char* this_command;
+
   for ( icommand = 0; icommand < n->commands->size; icommand++ ) {
-    if ( strcmp( command_name, vector_get( n->commands, icommand ) ) == 0 ) {
-      command_index = icommand;
+    ret = vector_get( n->commands, icommand, (void**)&this_command );
+    if ( ret != 0 ) {
+      mdi_error("Error in get_node_index: vector_get failed");
+      return 1;
+    }
+    if ( strcmp( command_name, this_command ) == 0 ) {
+      correct_command = icommand;
     }
   }
-  return command_index;
+  *command_index = correct_command;
+  return 0;
 }
 
 /*! \brief Determine the index of a callback within a node
  *
  * \param [in]       node
  *                   Pointer to the node
  * \param [in]       callback_name
  *                   Name of the callback
  */
-int get_callback_index(node* n, const char* callback_name) {
+int get_callback_index(node* n, const char* callback_name, int* callback_index) {
+  int ret;
   int icallback;
-  int callback_index = -1;
+  int correct_callback = -1;
+  char* this_callback;
+
   for ( icallback = 0; icallback < n->callbacks->size; icallback++ ) {
-    if ( strcmp( callback_name, vector_get( n->callbacks, icallback ) ) == 0 ) {
-      callback_index = icallback;
+    ret = vector_get( n->callbacks, icallback, (void**)&this_callback );
+    if ( ret != 0 ) {
+      mdi_error("Error in get_node_index: vector_get failed");
+      return 1;
+    }
+    if ( strcmp( callback_name, this_callback ) == 0 ) {
+      correct_callback = icallback;
     }
   }
-  return callback_index;
+  *callback_index = correct_callback;
+  return 0;
 }
 
 
 /*! \brief Determine the index of a callback within a node
  */
 int free_node_vector(vector* v) {
+  int ret;
   int inode = 0;
   size_t nnodes = v->size;
+
   for ( inode = 0; inode < nnodes; inode++ ) {
-    node* this_node = vector_get(v, inode);
+    node* this_node;
+    ret = vector_get(v, inode, (void**)&this_node );
+    if ( ret != 0 ) {
+      mdi_error("Error in free_node_vector: vector_get failed");
+      return ret;
+    }
 
     // free the "commands" and "callbacks" vectors for this node
     vector_free(this_node->commands);
     vector_free(this_node->callbacks);
   }
 
   // free this node vector
@@ -265,21 +248,35 @@
   return 0;
 }
 
 
 /*! \brief Create a new code structure and add it to the list of codes
  * Returns the index of the new code
  */
-int new_code() {
+int new_code(size_t* code_id) {
+  int ret;
+
   code new_code;
   new_code.returned_comms = 0;
   new_code.next_comm = 1;
   new_code.intra_MPI_comm = MPI_COMM_WORLD;
   new_code.language = MDI_LANGUAGE_C;
   new_code.language_on_destroy = NULL;
+  new_code.selected_method_id = 0;
+  new_code.initialized_mpi = 0;
+  new_code.ipi_compatibility = 0;
+  new_code.plugin_argc = -1;
+  new_code.plugin_argv = NULL;
+  new_code.tcp_initialized = 0;
+  new_code.mpi_initialized = 0;
+  new_code.test_initialized = 0;
+  new_code.shared_state_from_driver = NULL;
+  new_code.tcp_socket = -1;
+  new_code.port = -1;
+  new_code.hostname = NULL;
 
   // initialize the name and role strings
   int ichar;
   for (ichar=0; ichar < MDI_NAME_LENGTH_; ichar++) {
     new_code.name[ichar] = '\0';
     new_code.role[ichar] = '\0';
   }
@@ -290,102 +287,133 @@
     new_code.plugin_path[ichar] = '\0';
   }
 
   new_code.is_library = 0;
   new_code.id = (int)codes.size;
   new_code.called_set_execute_command_func = 0;
   new_code.intra_rank = 0;
-  if (world_rank != -1) {
-    // The Python wrapper has called MDI_Set_World_Rank to set this value
-    new_code.intra_rank = world_rank;
-  }
+  new_code.world_rank = -1;
+  new_code.world_size = -1;
 
   // initialize the node vector
   vector* node_vec = malloc(sizeof(vector));
-  vector_init(node_vec, sizeof(node));
+  ret = vector_init(node_vec, sizeof(node));
+  if ( ret != 0 ) {
+    mdi_error("Error in new_code: could not initialize node vector");
+    return ret;
+  }
   new_code.nodes = node_vec;
 
   // initialize the comms vector
   vector* comms_vec = malloc(sizeof(vector));
   vector_init(comms_vec, sizeof(communicator));
+  if ( ret != 0 ) {
+    mdi_error("Error in new_code: could not initialize comms vector");
+    return ret;
+  }
   new_code.comms = comms_vec;
 
   // initialize the methods vector
   vector* methods_vec = malloc(sizeof(vector));
   vector_init(methods_vec, sizeof(method));
+  if ( ret != 0 ) {
+    mdi_error("Error in new_code: could not initialize methods vector");
+    return ret;
+  }
   new_code.methods = methods_vec;
 
-  // Set the MPI callbacks
-  //new_code.mdi_mpi_recv = MPI_Recv;
-  //int (*mpi4py_recv_callback)(void*, int, int, MDI_Comm_Type);
-
   // add the new code to the global vector of codes
-  vector_push_back( &codes, &new_code );
-
-  // Create method objects for each supported method
-  /*
-  if ( enable_tcp_support( new_code.id ) ) {
-    mdi_error("Unable to enable TCP support");
-  }
-  if ( enable_mpi_support( new_code.id ) ) {
-    mdi_error("Unable to enable MPI support");
-  }
-#if _MDI_PLUGIN_SUPPORT == 1
-  if ( enable_plug_support( new_code.id ) ) {
-    mdi_error("Unable to enable plugin support");
+  ret = vector_push_back( &codes, &new_code );
+  if ( ret != 0 ) {
+    mdi_error("Error in new_code: could not add code to global codes vector");
+    return ret;
   }
-#endif
-  if ( enable_test_support( new_code.id ) ) {
-    mdi_error("Unable to enable TEST support");
-  }
-  */
 
   // return the index of the new code
-  return (int)codes.size - 1;
+  *code_id = codes.size - 1;
+  
+  return 0;
 }
 
 
 /*! \brief Get a code from a code handle
  * Returns a pointer to the code
  */
-code* get_code(int code_id) {
+int get_code(size_t code_id, code** ret_code) {
+  int ret;
+
   // Search through all of the codes for the one that matches code_id
   int icode;
   for (icode = 0; icode < codes.size; icode++ ) {
-    code* this_code = vector_get(&codes, icode);
+
+    code* this_code;
+
+    ret = vector_get( &codes, icode, (void**)&this_code );
+    if ( ret != 0 ) {
+      mdi_error("Error in get_code: vector_get failed");
+      return ret;
+    }
     if ( this_code->id == code_id ) {
-      return this_code;
+      *ret_code = this_code;
+      return 0;
     }
+
   }
   mdi_error("Code not found");
-  return NULL;
+  return 1;
+}
+
+
+/*! \brief Get the currently active code
+ * Returns a pointer to the code
+ */
+int get_current_code(code** this_code_ptr) {
+  int ret;
+  ret = get_code(codes.current_key, this_code_ptr);
+  if ( ret != 0 ) {
+    mdi_error("Error in get_current_code: get_code failed");
+    return ret;
+  }
+  return 0;
 }
 
 
 /*! \brief Delete a code
  * Returns 0 on success
  */
-int delete_code(int code_id) {
-  code* this_code = get_code(code_id);
+int delete_code(size_t code_id) {
+  int ret;
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
 
   // Call the langauge-specific destructor
   if ( this_code->language_on_destroy != NULL ) {
     if ( this_code->language_on_destroy(code_id) != 0 ) {
       mdi_error("Language-specific code deletion function failed");
       return 1;
     }
   }
 
   // Search through all of the codes for the one that matches code_id
   int icode;
   int code_index;
   int code_found = 0;
   for (icode = 0; icode < codes.size; icode++ ) {
-    code* code = vector_get(&codes, icode);
-    if ( code->id == code_id ) {
+    code* check_code;
+      
+    ret = vector_get( &codes, icode, (void**)&check_code );
+    if ( ret != 0 ) {
+      mdi_error("Error in delete_code: vector_get failed");
+      return ret;
+    }
+    if ( check_code->id == code_id ) {
       code_found = 1;
       code_index = icode;
 
       // stop searching
       icode = (int)codes.size;
     }
   }
@@ -403,88 +431,136 @@
   // delete the methods vector
   free_methods_vector(this_code->methods);
 
   // delete the comms vector
   int icomm;
   size_t ncomms = this_code->comms->size;
   for (icomm = 0; icomm < ncomms; icomm++) {
-    communicator* this_comm = vector_get( this_code->comms, (int)this_code->comms->size - 1 );
+    communicator* this_comm;
+    ret = vector_get( this_code->comms, (int)this_code->comms->size - 1, (void**)&this_comm );
+    if ( ret != 0 ) {
+      mdi_error("Error in delete_code: vector_get for comms vector failed");
+      return ret;
+    }
     delete_communicator(code_id, this_comm->id);
   }
   vector_free( this_code->comms );
 
   // delete the data for this code from the global vector of codes
   vector_delete(&codes, code_index);
 
   return 0;
 }
 
 
 /*! \brief Create a new method structure and add it to the vector of methods
  * Returns the handle of the new method
  */
-int new_method(int code_id, int method_id) {
-  code* this_code = get_code(code_id);
+int new_method(size_t code_id, int method_id, int* id_ptr) {
+  int ret;
+
+  // get the code
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
+
   method new_method;
-  new_method.id = (int)methods.size;
+  new_method.id = (int)this_code->methods->size;
   new_method.method_id = method_id;
 
   vector_push_back( this_code->methods, &new_method );
 
-  return new_method.id;
+  *id_ptr = new_method.id;
+  return 0;
 }
 
 
 /*! \brief Get a method from a method handle
  * Returns a pointer to the method
  */
-method* get_method(int code_id, int method_id) {
-  code* this_code = get_code(code_id);
+int get_method(size_t code_id, int method_id, method** method_ptr) {
+  int ret;
+
+  // get the code
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
 
   // Search through all of the codes for the one that matches code_id
   int imethod;
   for (imethod = 0; imethod < this_code->methods->size; imethod++ ) {
-    method* this_method = vector_get(this_code->methods, imethod);
+    method* this_method;
+    ret = vector_get( this_code->methods, imethod, (void**)&this_method );
+    if ( ret != 0 ) {
+      mdi_error("Error in get_method: vector_get failed");
+      return ret;
+    }
     if ( this_method->method_id == method_id ) {
-      return this_method;
+      *method_ptr = this_method;
+      return 0;
     }
   }
   mdi_error("Method not supported for this build of the MDI Library");
-  return NULL;
+  return 1;
 }
 
 
 /*! \brief Delete a method
  * Returns 0 on success
  */
-int delete_method(int code_id, int method_id) {
-  code* this_code = get_code(code_id);
-  method* this_method = get_method(code_id, method_id);
+int delete_method(size_t code_id, int method_id) {
+  int ret;
+
+  // get the code
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
+
+  method* this_method;
+  ret = get_method(code_id, method_id, &this_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_plug_support: delete_method failed");
+    return ret;
+  }
 
   // Search through all of the methods for the one that matches method
   int imethod;
   int method_index;
   int method_found = 0;
-  for (imethod = 0; imethod < methods.size; imethod++ ) {
-    method* method = vector_get(&methods, imethod);
-    if ( method->method_id == method_id ) {
+  for (imethod = 0; imethod < this_code->methods->size; imethod++ ) {
+    method* check_method;
+    ret = vector_get(this_code->methods, imethod, (void**)&check_method );
+    if ( ret != 0 ) {
+      mdi_error("Error in delete_method: vector_get failed");
+      return ret;
+    }
+    if ( check_method->method_id == method_id ) {
       method_found = 1;
       method_index = imethod;
 
       // stop searching
-      imethod = (int)methods.size;
+      imethod = (int)this_code->methods->size;
     }
   }
   if ( method_found != 1 ) {
     mdi_error("Method not found during delete");
     return 1;
   }
 
   // delete the data for this method from the global vector of methods
-  vector_delete(&methods, method_index);
+  vector_delete(this_code->methods, method_index);
 
   return 0;
 }
 
 
 
 /*! \brief Free the memory associated with a methods vector
@@ -509,16 +585,24 @@
 }
 
 
 
 /*! \brief Create a new communicator structure and add it to the list of communicators
  * Returns the handle of the new communicator
  */
-int new_communicator(int code_id, int method) {
-  code* this_code = get_code(code_id);
+int new_communicator(size_t code_id, int method, MDI_Comm_Type* comm_id_ptr) {
+  int ret;
+
+  // get the code
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
 
   communicator new_comm;
   new_comm.method_id = method;
   new_comm.is_accepted = 0;
   vector* node_vec = malloc(sizeof(vector));
   vector_init(node_vec, sizeof(node));
   new_comm.nodes = node_vec;
@@ -534,50 +618,85 @@
   new_comm.mdi_version[2] = 0;
   this_code->next_comm++;
 
   new_comm.delete = communicator_delete;
 
   vector_push_back( this_code->comms, &new_comm );
 
-  return new_comm.id;
+  *comm_id_ptr = new_comm.id;
+  return 0;
 }
 
 
 /*! \brief Get a communicator from a communicator handle
  * Returns a pointer to the communicator
  */
-communicator* get_communicator(int code_id, MDI_Comm_Type comm_id) {
-  code* this_code = get_code(code_id);
+int get_communicator(size_t code_id, MDI_Comm_Type comm_id, communicator** comm_ptr) {
+  int ret;
+
+  // get the code
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
 
   // Search through all of the communicators for the one that matches comm_id
   int icomm;
   for (icomm = 0; icomm < this_code->comms->size; icomm++ ) {
-    communicator* comm = vector_get(this_code->comms, icomm);
+    communicator* comm;
+    ret = vector_get( this_code->comms, icomm, (void**)&comm );
+    if ( ret != 0 ) {
+      mdi_error("Error in get_communicator: vector_get failed");
+      return ret;
+    }
     if ( comm->id == comm_id ) {
-      return comm;
+      *comm_ptr = comm;
+      return 0;
     }
   }
   mdi_error("Communicator not found");
-  return NULL;
+  return 1;
 }
 
 
 /*! \brief Delete a communicator
- * Returns 0 on success
+ *
+ * The function returns \p 0 on a success.
  */
-int delete_communicator(int code_id, MDI_Comm_Type comm_id) {
-  code* this_code = get_code(code_id);
-  communicator* this_comm = get_communicator(code_id, comm_id);
+int delete_communicator(size_t code_id, MDI_Comm_Type comm_id) {
+  int ret;
+
+  // get the code
+  code* this_code;
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code failed");
+    return ret;
+  }
+
+  communicator* this_comm;
+  ret = get_communicator(code_id, comm_id, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_communicator failed");
+    return ret;
+  }
 
   // Search through all of the communicators for the one that matches comm_id
   size_t icomm;
   size_t comm_index;
   int comm_found = 0;
   for (icomm = 0; icomm < this_code->comms->size; icomm++ ) {
-    communicator* comm = vector_get(this_code->comms, (int)icomm);
+    communicator* comm;
+    ret = vector_get( this_code->comms, (int)icomm, (void**)&comm );
+    if ( ret != 0 ) {
+      mdi_error("Error in delete_communicator: vector_get failed");
+      return ret;
+    }
     if ( comm->id == comm_id ) {
       comm_found = 1;
       comm_index = icomm;
 
       // stop searching
       icomm = this_code->comms->size;
     }
@@ -587,16 +706,24 @@
     return 1;
   }
 
   // do any method-specific deletion operations
   this_comm->delete(this_comm);
 
   // in case this communicator's delete function modified the code / comms vectors, update the pointers
-  this_code = get_code(code_id);
-  this_comm = get_communicator(code_id, comm_id);
+  ret = get_code(code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: get_code after delete failed");
+    return ret;
+  }
+  ret = get_communicator(code_id, comm_id, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in delete_code: second get_communicator failed");
+    return ret;
+  }
 
   // delete the node vector
   free_node_vector(this_comm->nodes);
 
   // delete the data for this communicator from the code's vector of communicators
   vector_delete(this_code->comms, (int)comm_index);
 
@@ -612,31 +739,32 @@
 
 
 /*! \brief Print error message and exit
  *
  * \param [in]       message
  *                   Message printed before exiting.
  */
-int file_exists(const char* file_name) {
+int file_exists(const char* file_name, int* flag) {
 #ifdef _WIN32
   DWORD dwAttrib = GetFileAttributes(file_name);
   if ( dwAttrib != INVALID_FILE_ATTRIBUTES && !(dwAttrib & FILE_ATTRIBUTE_DIRECTORY) ) {
-    return 1;
+    *flag = 1;
   }
   else {
-    return 0;
+    *flag = 0;
   }
 #else
   if ( access( file_name, F_OK ) == 0 ) {
-    return 1;
+    *flag = 1;
   }
   else {
-    return 0;
+    *flag = 0;
   }
 #endif
+  return 0;
 }
 
 
 /*! \brief Print error message
  *
  * \param [in]       message
  *                   Message printed before exiting.
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_global.h` & `pymdi-1.4.9/MDI_Library/mdi_global.h`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #define MDI_LANGUAGE_C 1
 #define MDI_LANGUAGE_FORTRAN 2
 #define MDI_LANGUAGE_PYTHON 3
 
 // MDI version numbers
 #define MDI_MAJOR_VERSION_ 1
 #define MDI_MINOR_VERSION_ 4
-#define MDI_PATCH_VERSION_ 8
+#define MDI_PATCH_VERSION_ 9
 
 // length of an MDI command in characters
 #define MDI_COMMAND_LENGTH_ 256
 
 // length of an MDI name in characters
 #define MDI_NAME_LENGTH_ 256
 
@@ -70,66 +70,71 @@
 // MDI role types
 #define MDI_DRIVER_ 1
 #define MDI_ENGINE_ 2
 
 // MDI Typedefs
 typedef int MDI_Comm_Type;
 typedef int MDI_Datatype_Type;
+typedef int (*MDI_execute_command_type)(void*, MDI_Comm_Type, void*);
 
 typedef struct dynamic_array_struct {
   /*! \brief The elements stored by this vector */
   unsigned char* data;
   /*! \brief Size of each element */
   size_t stride;
   /*! \brief Total number of elements that can be stored by this vector */
   size_t capacity;
   /*! \brief Number of elements actually stored */
   size_t size; //number of elements actually stored
+  /*! \brief If the array has a currently active component, this is that value */
+  size_t current_key; //number of elements actually stored
+  /*! \brief Flag whether the vector has been initialized */
+  int initialized;
 } vector;
 
 typedef struct method_struct {
-  /*! \brief ID of this method */
-  int id;
-  /*! \brief Communication method */
-  int method_id;
   /*! \brief Function pointer for method initialization work */
   int (*on_selection)();
   int (*on_accept_communicator)();
   int (*on_send_command)(const char*, MDI_Comm_Type, int* skip_flag);
   int (*after_send_command)(const char*, MDI_Comm_Type);
   int (*on_recv_command)(MDI_Comm_Type);
+  /*! \brief ID of this method */
+  int id;
+  /*! \brief Communication method */
+  int method_id;
 } method;
 
 typedef struct communicator_struct {
-  /*! \brief Communication method used by this communicator */
-  int method_id;
-  /*! \brief MDI_Comm handle that corresponds to this communicator */
-  MDI_Comm_Type id;
-  /*! \brief Indicate whether this communicator has been accepted yet */
-  int is_accepted;
-  /*! \brief Handle for the id of the associated code */
-  int code_id;
-  /*! \brief For communicators using the TCP communicatiom method, the socket descriptor (WINDOWS) */
-  sock_t sockfd;
-  /*! \brief The value of MDI_NAME_LENGTH for the connected code */
-  int name_length;
-  /*! \brief The value of MDI_COMMAND_LENGTH for the connected code */
-  int command_length;
   /*! \brief The MDI version of the connected code */
   int mdi_version[3];
   /*! \brief The nodes supported by the connected code */
   vector* nodes;
   /*! \brief Method-specific information for this communicator */
   void* method_data;
   /*! \brief Function pointer for method-specific send operations */
   int (*send)(const void*, int, MDI_Datatype_Type, MDI_Comm_Type, int);
   /*! \brief Function pointer for method-specific receive operations */
   int (*recv)(void*, int, MDI_Datatype_Type, MDI_Comm_Type, int);
   /*! \brief Function pointer for method-specific deletion operations */
   int (*delete)(void*);
+  /*! \brief Handle for the id of the associated code */
+  size_t code_id;
+  /*! \brief For communicators using the TCP communicatiom method, the socket descriptor (WINDOWS) */
+  sock_t sockfd;
+  /*! \brief Communication method used by this communicator */
+  int method_id;
+  /*! \brief MDI_Comm handle that corresponds to this communicator */
+  MDI_Comm_Type id;
+  /*! \brief Indicate whether this communicator has been accepted yet */
+  int is_accepted;
+  /*! \brief The value of MDI_NAME_LENGTH for the connected code */
+  int name_length;
+  /*! \brief The value of MDI_COMMAND_LENGTH for the connected code */
+  int command_length;
 } communicator;
 
 typedef struct node_struct {
   /*! \brief Name of the node */
   char name[MDI_COMMAND_LENGTH_];
   /*! \brief Vector containing all the commands supported at this node */
   vector* commands;
@@ -138,139 +143,133 @@
 } node;
 
 typedef struct code_struct {
   /*! \brief Name of the driver/engine */
   char name[MDI_NAME_LENGTH_];
   /*! \brief Role of the driver/engine */
   char role[MDI_NAME_LENGTH_];
-  /*! \brief Function pointer to the generic execute_command_function */
-  int (*execute_command)(const char*, MDI_Comm_Type, void*);
   /*! \brief Pointer to the class object that is passed to any call to execute_command */
   void* execute_command_obj;
-  /*! \brief Handle for this code */
-  int id;
-  /*! \brief The number of communicator handles that have been returned by MDI_Accept_Connection() */
-  int returned_comms;
-  /*! \brief The handle of the next communicator */
-  int next_comm;
-  /*! \brief Native language of this code */
-  int language;
-  /*! \brief Rank of this process within its associated code */
-  int intra_rank;
-  /*! \brief Flag whether this code has called set_execute_command_func */
-  int called_set_execute_command_func;
-  /*! \brief MPI intra-communicator that spans all ranks associated with this code */
-  MPI_Comm intra_MPI_comm;
   /*! \brief Vector containing all nodes supported by this code */
   vector* nodes;
   /*! \brief Vector containing all communicators associated with this code */
   vector* comms;
   /*! \brief Vector containing all supported methods */
   vector* methods;
   /*! \brief Path to the plugins available to this code */
   char* plugin_path;
+  /*! \brief Argument vector for plugin command-line options */
+  char** plugin_argv;
+  /*! \brief Unedited command-line options for currently running plugin */
+  char* plugin_unedited_options;
+  /*! \brief Shared plugin state, received from the driver during plugin calculations */
+  void* shared_state_from_driver;
+  /*! \brief Hostname of the driver */
+  char* hostname;
+  /*! \brief Function pointer to the language-specific wrapper for the execute_command function */
+  int (*execute_command_wrapper)(const char*, MDI_Comm_Type, void*);
+  /*! \brief Function pointer to the generic execute_command_function */
+  MDI_execute_command_type execute_command;
   /*! \brief Function pointer to the language-specific destructor function */
   int (*language_on_destroy)(int);
+  /*! \brief Python callback pointer for MPI_Recv */
+  int (*mpi4py_recv_callback)(void*, int, int, int, MDI_Comm_Type);
+  /*! \brief Python callback pointer for MPI_Send */
+  int (*mpi4py_send_callback)(void*, int, int, int, MDI_Comm_Type);
+  /*! \brief Python callback pointer for the initial MPI allgather */
+  int (*mpi4py_allgather_callback)(void*, void*);
+  /*! \brief Python callback pointer for gathering names */
+  int (*mpi4py_gather_names_callback)(void*, void*, int*, int*);
+  /*! \brief Python callback pointer for MPI_Comm_split */
+  int (*mpi4py_split_callback)(int, int, MDI_Comm_Type, int);
+  /*! \brief Python callback pointer for MPI_Comm_rank */
+  int (*mpi4py_rank_callback)(int);
+  /*! \brief Python callback pointer for MPI_Comm_size */
+  int (*mpi4py_size_callback)(int);
+  /*! \brief Python callback pointer for MPI_Comm_barrier */
+  int (*mpi4py_barrier_callback)(int);
+  /*! \brief MPI intra-communicator that spans all ranks associated with this code */
+  MPI_Comm intra_MPI_comm;
+  /*! \brief Socket for TCP connections */
+  sock_t tcp_socket;
   /*! \brief Flag whether this code is being used as a library
   0: Not a library
   1: Is an ENGINE library, but has not connected to the driver
   2: Is an ENGINE library that has connected to the driver */
   int is_library;
+  /*! \brief Size of MPI_COMM_WORLD */
+  int world_size;
+  /*! \brief Rank of this process within MPI_COMM_WORLD */
+  int world_rank;
+  /*! \brief Handle for this code */
+  size_t id;
+  /*! \brief The number of communicator handles that have been returned by MDI_Accept_Connection() */
+  int returned_comms;
+  /*! \brief The handle of the next communicator */
+  int next_comm;
+  /*! \brief Native language of this code */
+  int language;
+  /*! \brief Rank of this process within its associated code */
+  int intra_rank;
+  /*! \brief Flag whether this code has called set_execute_command_func */
+  int called_set_execute_command_func;
+  /*! \brief ID of the method being used for inter-code communication */
+  int selected_method_id;
+  /*! \brief Flag for whether MDI is running in i-PI compatibility mode */
+  int ipi_compatibility;
+  /*! \brief Flag for whether MDI called MPI_Init */
+  int initialized_mpi;
+  /*! \brief Argument count for plugin command-line options */
+  int plugin_argc;
+  /*! \brief Flag whether this code has previously initialized TCP */
+  int tcp_initialized;
+  /*! \brief Flag whether this code has previously initialized MPI */
+  int mpi_initialized;
+  /*! \brief Flag whether this code has previously initialized TEST */
+  int test_initialized;
+  /*! \brief Port over which the driver will listen */
+  int port;
 } code;
 
-/*! \brief Vector containing all codes that have been initiailized on this rank. Typically, 
-this will only include a single code, unless the communication method is LINK */
-extern vector codes;
-
-/*! \brief ID of the method being used for inter-code communication */
-extern int selected_method_id;
-
-/*! \brief Index of the active code */
-extern int current_code;
-
-/*! \brief Flag for whether MDI is running in i-PI compatibility mode */
-extern int ipi_compatibility;
-
-/*! \brief Flag for whether MDI has been previously initialized */
-extern int is_initialized;
-
-/*! \brief Flag for whether MDI called MPI_Init */
-extern int initialized_mpi;
-
-/*! \brief Flag for whether MDI is currently operating in plugin mode */
-extern int plugin_mode;
-
-/*! \brief Internal copy of MPI_COMM_WORLD, used when MDI initializes MPI */
-extern MPI_Comm mdi_mpi_comm_world;
-
-/*! \brief Unedited command-line options for currently running plugin */
-extern char* plugin_unedited_options;
 
-/*! \brief Argument count for plugin command-line options */
-extern int plugin_argc;
 
-/*! \brief Argument vector for plugin command-line options */
-extern char** plugin_argv;
-
-/*! \brief Python callback pointer for MPI_Recv */
-extern int (*mpi4py_recv_callback)(void*, int, int, int, MDI_Comm_Type);
-
-/*! \brief Python callback pointer for MPI_Send */
-extern int (*mpi4py_send_callback)(void*, int, int, int, MDI_Comm_Type);
-
-/*! \brief Python callback pointer for the initial MPI allgather */
-extern int (*mpi4py_allgather_callback)(void*, void*);
-
-/*! \brief Python callback pointer for gathering names */
-extern int (*mpi4py_gather_names_callback)(void*, void*, int*, int*);
-
-/*! \brief Python callback pointer for MPI_Comm_split */
-extern int (*mpi4py_split_callback)(int, int, MDI_Comm_Type, int);
-
-/*! \brief Python callback pointer for MPI_Comm_rank */
-extern int (*mpi4py_rank_callback)(int);
-
-/*! \brief Python callback pointer for MPI_Comm_size */
-extern int (*mpi4py_size_callback)(int);
-
-/*! \brief Python callback pointer for MPI_Comm_barrier */
-extern int (*mpi4py_barrier_callback)(int);
+/*! \brief Vector containing all codes that have been initiailized on this rank. Typically, 
+this will only include a single code, unless the communication method is LINK.
+ALL global MDI data is stored within this vector */
+extern vector codes;
 
-/*! \brief Size of MPI_COMM_WORLD */
-extern int world_size;
 
-/*! \brief Rank of this process within MPI_COMM_WORLD */
-extern int world_rank;
 
 int vector_init(vector* v, size_t stride);
 int vector_push_back(vector* v, void* element);
-void* vector_get(vector* v, int index);
+int vector_get(vector* v, int index, void** element);
 int vector_delete(vector* v, int index);
 int vector_free(vector* v);
 
-int get_node_index(vector* v, const char* node_name);
-int get_command_index(node* n, const char* command_name);
-int get_callback_index(node* n, const char* callback_name);
+int get_node_index(vector* v, const char* node_name, int* node_index);
+int get_command_index(node* n, const char* command_name, int* command_index);
+int get_callback_index(node* n, const char* callback_name, int* callback_index);
 int free_node_vector(vector* v);
 
-int new_communicator(int code_id, int method);
-communicator* get_communicator(int code_id, MDI_Comm_Type comm_id);
-int delete_communicator(int code_id, MDI_Comm_Type comm_id);
-
-int new_code();
-code* get_code(int code_id);
-int delete_code(int code_id);
-
-int new_method(int code_id, int method_id);
-method* get_method(int code_id, int method_id);
-int delete_method(int code_id, int method_id);
+int new_communicator(size_t code_id, int method, MDI_Comm_Type* comm_id_ptr);
+int get_communicator(size_t code_id, MDI_Comm_Type comm_id, communicator** comm_ptr);
+int delete_communicator(size_t code_id, MDI_Comm_Type comm_id);
+
+int new_code(size_t* code_id);
+int get_code(size_t code_id, code** ret_code);
+int delete_code(size_t code_id);
+int get_current_code(code** this_code_ptr);
+
+int new_method(size_t code_id, int method_id, int* id_ptr);
+int get_method(size_t code_id, int method_id, method** method_ptr);
+int delete_method(size_t code_id, int method_id);
 int free_methods_vector(vector* v);
 
 /*! \brief Check whether a file exists */
-int file_exists(const char* file_name);
+int file_exists(const char* file_name, int* flag);
 
 /*! \brief Dummy function for method-specific deletion operations for communicator deletion */
 int communicator_delete(void* comm);
 
 void mdi_error(const char* message);
 void mdi_warning(const char* message);
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_lib.c` & `pymdi-1.4.9/MDI_Library/mdi_lib.c`

 * *Files 8% similar despite different names*

```diff
@@ -16,75 +16,112 @@
 
 #ifdef _WIN32
 #include <windows.h>
 #else
 #include <dlfcn.h>
 #endif
 
-/*! \brief Shared state received from the driver */
-plugin_shared_state* shared_state_from_driver = NULL;
 
 /*! \brief Enable support for the PLUG method */
 int enable_plug_support( int code_id ) {
-  new_method(code_id, MDI_LINK);
-  method* this_method = get_method(code_id, MDI_LINK);
+  int ret;
+  int method_id;
+  ret = new_method(code_id, MDI_LINK, &method_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_plug_support: new_method failed");
+    return ret;
+  }
+  method* this_method;
+  ret = get_method(code_id, MDI_LINK, &this_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_plug_support: get_method failed");
+    return ret;
+  }
   this_method->on_selection = plug_on_selection;
   this_method->on_accept_communicator = plug_on_accept_communicator;
   this_method->on_send_command = plug_on_send_command;
   this_method->after_send_command = plug_after_send_command;
   this_method->on_recv_command = plug_on_recv_command;
   return 0;
 }
 
 
 
 /*! \brief Callback when the end-user selects PLUG as the method */
 int plug_on_selection() {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in plug_on_selection: get_current_code failed");
+    return ret;
+  }
 
   // Check if this is an engine being used as a library
   if (strcmp(this_code->role, "ENGINE") == 0) {
     this_code->is_library = 1;
     library_initialize();
   }
 
   return 0;
 }
 
 
 
 /*! \brief Callback when the PLUG method must accept a communicator */
 int plug_on_accept_communicator() {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in plug_on_accept_communicator: get_current_code failed");
+    return 1;
+  }
 
   // Give the library method an opportunity to update the current code
-  library_accept_communicator();
+  //library_accept_communicator();
 
   // If MDI hasn't returned some connections, do that now
   if ( this_code->returned_comms < this_code->next_comm - 1 ) {
     this_code->returned_comms++;
-    communicator* comm_obj = get_communicator(current_code, this_code->returned_comms);
+    communicator* comm_obj;
+    ret = get_communicator(codes.current_key, this_code->returned_comms, &comm_obj);
+    if ( ret != 0 ) {
+      mdi_error("Error in plug_on_accept_communicator: get_communicator failed");
+      return ret;
+    }
     comm_obj->is_accepted = 1;
     return this_code->returned_comms;
   }
 
   // unable to accept any connections
   return MDI_COMM_NULL;
 }
 
 
 
 /*! \brief Callback when the PLUG method must send a command */
 int plug_on_send_command(const char* command, MDI_Comm comm, int* skip_flag) {
-  code* this_code = get_code(current_code);
-  communicator* this_comm = get_communicator(current_code, comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in plug_on_send_command: get_current_code failed");
+    return 1;
+  }
+  communicator* this_comm;
+  ret = get_communicator(codes.current_key, comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in plug_on_send_command: get_communicator failed");
+    return ret;
+  }
   library_data* libd = (library_data*) this_comm->method_data;
-  //int iengine = libd->connected_code;
-  //code* engine_code = get_code(iengine);
-  int ret = 0;
 
   // Check whether MPI has been initialized
   int mpi_init_flag;
   if ( MPI_Initialized(&mpi_init_flag) ) {
     mdi_error("Error in MDI_plug_on_send_command: MPI_Initialized failed");
     return 1;
   }
@@ -113,51 +150,56 @@
   // set the command for the engine to execute
   library_set_command(command_bcast, comm);
 
   if ( command_bcast[0] == '<' ) {
     // execute the command, so that the data from the engine can be received later by the driver
     //ret = library_execute_command(comm);
 
-    libd->shared_state->engine_activate_code( libd->shared_state->engine_code_id );
+    libd->shared_state->engine_activate_code( libd->shared_state->engine_codes_ptr, libd->shared_state->engine_code_id );
 
     libd->shared_state->lib_execute_command(libd->shared_state->engine_mdi_comm);
     if ( ret != 0 ) {
       mdi_error("Error in MDI_Send_Command: Unable to execute receive command through library");
       free( command_bcast );
       return ret;
     }
 
-    libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+    libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr, libd->shared_state->driver_code_id );
 
     *skip_flag = 1;
   }
   else if ( command_bcast[0] == '>' ) {
     // flag the command to be executed after the next call to MDI_Send
-    communicator* this = get_communicator(current_code, comm);
+    communicator* this;
+    ret = get_communicator(codes.current_key, comm, &this);
+    if ( ret != 0 ) {
+      mdi_error("Error in plug_on_send_command: second get_communicator failed");
+      return ret;
+    }
     library_data* libd = (library_data*) this->method_data;
     libd->execute_on_send = 1;
     *skip_flag = 1;
   }
-  else if ( plugin_mode && ( strcmp( command_bcast, "EXIT" ) == 0 || command_bcast[0] == '@' ) ) {
+  else if ( strcmp( command_bcast, "EXIT" ) == 0 || command_bcast[0] == '@' ) {
     // this command should be received by MDI_Recv_command, rather than through the execute_command callback
   }
   else {
     // this is a command that neither sends nor receives data, so execute it now
     //ret = library_execute_command(comm);
 
-    libd->shared_state->engine_activate_code( libd->shared_state->engine_code_id );
+    libd->shared_state->engine_activate_code( libd->shared_state->engine_codes_ptr, libd->shared_state->engine_code_id );
 
     libd->shared_state->lib_execute_command(libd->shared_state->engine_mdi_comm);
     if ( ret != 0 ) {
       mdi_error("Error in MDI_Send_Command: Unable to execute command through library");
       free( command_bcast );
       return ret;
     }
 
-    libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+    libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr, libd->shared_state->driver_code_id );
 
     *skip_flag = 1;
   }
 
   free( command_bcast );
   return ret;
 }
@@ -169,61 +211,75 @@
   return 0;
 }
 
 
 
 /*! \brief Callback when the PLUG method must receive a command */
 int plug_on_recv_command(MDI_Comm comm) {
-  int ret = 0;
-  int iengine = current_code;
-  code* this_code = get_code(current_code);
-  communicator* engine_comm = get_communicator(current_code, comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in plug_on_recv_command: get_current_code failed");
+    return 1;
+  }
+  communicator* engine_comm;
+  ret = get_communicator(codes.current_key, comm, &engine_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in plug_on_recv_command: get_communicator failed");
+    return ret;
+  }
 
   // get the driver code to which this communicator connects
   library_data* libd = (library_data*) engine_comm->method_data;
   int idriver = libd->connected_code;
 
   //MDI_Comm driver_comm_handle = library_get_matching_handle(comm);
   //communicator* driver_comm = get_communicator(idriver, driver_comm_handle);
   //library_data* driver_lib = (library_data*) driver_comm->method_data;
 
   // Copy the execute_command function to a shared location
+  libd->shared_state->execute_command_wrapper = this_code->execute_command_wrapper;
   libd->shared_state->execute_command = this_code->execute_command;
   libd->shared_state->execute_command_obj = this_code->execute_command_obj;
 
   // set the current code to the driver
-//  current_code = idriver;
-//  current_code = libd->shared_state->driver_code_id;
-  libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+  libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr, 
+                                            libd->shared_state->driver_code_id );
 
   //void* class_obj = driver_lib->driver_callback_obj;
   ret = libd->shared_state->driver_node_callback(libd->shared_state->mpi_comm_ptr, libd->shared_state->driver_mdi_comm, libd->shared_state->driver_callback_obj);
   if ( ret != 0 ) {
     mdi_error("PLUG error in on_recv_command: driver_node_callback failed");
     return ret;
   }
 
   // set the current code to the engine
-//  current_code = iengine;
-//  current_code = libd->shared_state->engine_code_id;
-  libd->shared_state->engine_activate_code( libd->shared_state->engine_code_id );
+  libd->shared_state->engine_activate_code( libd->shared_state->engine_codes_ptr,
+                                            libd->shared_state->engine_code_id );
 
   return 0;
 }
 
 
 
 /*! \brief Load the initialization function for a plugin
  *
  */
 int library_load_init(const char* plugin_name, void* mpi_comm_ptr,
                       library_data* libd, int mode) {
   int ret;
-  int driver_code_id = current_code;
-  code* this_code = get_code(driver_code_id);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_load_init: get_current_code failed");
+    return ret;
+  }
   MPI_Comm mpi_comm = *(MPI_Comm*) mpi_comm_ptr;
 
   //
   // Get the path to the plugin
   // Note: Eventually, should probably replace this code with libltdl
   //
   char* plugin_path = malloc( PLUGIN_PATH_LENGTH * sizeof(char) );
@@ -235,15 +291,21 @@
   }
   else { // Load MDI_Plugin_open
     snprintf(plugin_init_name, PLUGIN_PATH_LENGTH, "MDI_Plugin_open_%s", plugin_name);
   }
 
   // Attempt to load a python script
   snprintf(plugin_path, PLUGIN_PATH_LENGTH, "%s/%s.py", this_code->plugin_path, plugin_name);
-  if ( file_exists(plugin_path) ) {
+  int exists_flag;
+  ret = file_exists( plugin_path, &exists_flag );
+  if ( ret != 0 ) {
+    mdi_error("Error in library_load_init: file_exists failed");
+    return ret;
+  }
+  if ( exists_flag ) {
     libd->is_python = 1;
     libd->shared_state->engine_language = MDI_LANGUAGE_PYTHON;
     ret = python_plugin_init( plugin_name, plugin_path, mpi_comm_ptr, libd->shared_state );
     if ( ret != 0 ) {
       mdi_error("Error in python_plugin_init");
       return -1;
     }
@@ -324,74 +386,80 @@
  */
 int library_parse_options(const char* options, library_data* libd) {
 
   // Begin parsing the options char array into an argv-style array of char arrays
 
   // copy the input options array
   int options_len = strlen(options) + 1;
-  libd->plugin_options = malloc( options_len * sizeof(char) );
-  snprintf(libd->plugin_options, options_len, "%s", options);
-  libd->plugin_unedited_options = malloc( options_len * sizeof(char) );
-  snprintf(libd->plugin_unedited_options, options_len, "%s", options);
-  libd->plugin_options_allocated = 1;
+  libd->shared_state->plugin_options = malloc( options_len * sizeof(char) );
+  libd->shared_state->plugin_unedited_options = malloc( options_len * sizeof(char) );
+
+  // zero both of the new arrays
+  int ichar;
+  for (ichar=0; ichar < options_len; ichar++) {
+    libd->shared_state->plugin_options[ichar] = '\0';
+    libd->shared_state->plugin_unedited_options[ichar] = '\0';
+  }
+
+  snprintf(libd->shared_state->plugin_options, options_len, "%s", options);
+  snprintf(libd->shared_state->plugin_unedited_options, options_len, "%s", options);
 
   // determine the number of arguments
   libd->shared_state->plugin_argc = 0;
-  int ichar;
   int in_argument = 0; // was the previous character part of an argument, or just whitespace?
   int in_single_quotes = 0; // was the previous character part of a single quote?
   int in_double_quotes = 0; // was the previous character part of a double quote?
   for (ichar=0; ichar < options_len; ichar++) {
-    if ( libd->plugin_options[ichar] == '\0' ) {
+    if ( libd->shared_state->plugin_options[ichar] == '\0' ) {
       if ( in_double_quotes ) {
         mdi_error("Unterminated double quotes received in MDI_Launch_plugin \"options\" argument.");
       }
       if ( in_argument ) {
         libd->shared_state->plugin_argc++;
       }
       in_argument = 0;
     }
-    else if (libd->plugin_options[ichar] == ' ') {
+    else if (libd->shared_state->plugin_options[ichar] == ' ') {
       if ( ! in_double_quotes && ! in_single_quotes ) {
         if ( in_argument ) {
           libd->shared_state->plugin_argc++;
         }
         in_argument = 0;
-        libd->plugin_options[ichar] = '\0';
+        libd->shared_state->plugin_options[ichar] = '\0';
       }
     }
-    else if (libd->plugin_options[ichar] == '\"') {
+    else if (libd->shared_state->plugin_options[ichar] == '\"') {
       if ( in_single_quotes ) {
         mdi_error("Nested quotes not supported by MDI_Launch_plugin \"options\" argument.");
       }
       in_argument = 1;
       in_double_quotes = (in_double_quotes + 1) % 2;
-      libd->plugin_options[ichar] = '\0';
+      libd->shared_state->plugin_options[ichar] = '\0';
     }
-    else if (libd->plugin_options[ichar] == '\'') { 
+    else if (libd->shared_state->plugin_options[ichar] == '\'') { 
       if ( in_double_quotes ) {
         mdi_error("Nested quotes not supported by MDI_Launch_plugin \"options\" argument.");
       }
       in_argument = 1;
       in_single_quotes = (in_single_quotes + 1) % 2;
-      libd->plugin_options[ichar] = '\0';
+      libd->shared_state->plugin_options[ichar] = '\0';
     }
     else {
       in_argument = 1;
     }
   }
 
   // construct pointers to all of the arguments
   libd->shared_state->plugin_argv = malloc( libd->shared_state->plugin_argc * sizeof(char*) );
   libd->shared_state->plugin_argv_allocated = 1;
   int iarg = 0;
   for (ichar=0; ichar < options_len; ichar++) {
-    if ( libd->plugin_options[ichar] != '\0' ) {
-      if ( ichar == 0 || libd->plugin_options[ichar-1] == '\0' ) {
-        libd->shared_state->plugin_argv[iarg] = &libd->plugin_options[ichar];
+    if ( libd->shared_state->plugin_options[ichar] != '\0' ) {
+      if ( ichar == 0 || libd->shared_state->plugin_options[ichar-1] == '\0' ) {
+        libd->shared_state->plugin_argv[iarg] = &libd->shared_state->plugin_options[ichar];
         iarg++;
       }
     }
   }
   if ( iarg != libd->shared_state->plugin_argc ) {
     mdi_error("Programming error: unable to correctly parse the MDI_Launch_plugin \"options\" argument.");
   }
@@ -404,30 +472,43 @@
 /*! \brief Launch an MDI plugin
  *
  */
 int library_launch_plugin(const char* plugin_name, const char* options, void* mpi_comm_ptr,
                           MDI_Driver_node_callback_t driver_node_callback,
                           void* driver_callback_object) {
   int ret;
-  code* this_code = get_code(current_code);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_launch_plugin: get_current_code failed");
+    return 1;
+  }
   MPI_Comm mpi_comm = *(MPI_Comm*) mpi_comm_ptr;
 
   // initialize a communicator for the driver
   int icomm = library_initialize();
-  communicator* driver_comm = get_communicator(current_code, icomm);
+  communicator* driver_comm;
+  ret = get_communicator(codes.current_key, icomm, &driver_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_launch_plugin: get_communicator failed");
+    return ret;
+  }
   library_data* libd = (library_data*) driver_comm->method_data;
   libd->connected_code = (int)codes.size;
 
   // allocate data that is shared between the driver and the plugin
   libd->shared_state = malloc(sizeof(plugin_shared_state));
   libd->shared_state->plugin_argc = 0;
   libd->shared_state->plugin_argv_allocated = 0;
   libd->shared_state->buf_allocated = 0;
-  libd->shared_state->driver_code_id = current_code;
+  libd->shared_state->driver_code_id = codes.current_key;
   libd->shared_state->engine_language = MDI_LANGUAGE_C;
+  libd->shared_state->python_interpreter_initialized = 0;
+  libd->shared_state->driver_codes_ptr = &codes;
 
   MDI_Comm comm;
   ret = MDI_Accept_Communicator(&comm);
   if ( ret != 0 || comm == MDI_COMM_NULL ) {
     mdi_error("MDI unable to create communicator for plugin");
     return -1;
   }
@@ -439,16 +520,16 @@
   // Set the mpi communicator associated with this plugin instance
   libd->mpi_comm = mpi_comm;
 
   // Parse plugin command-line options
   library_parse_options(options, libd);
 
   // Assign the global command-line options variables to the values for this plugin  
-  plugin_argc = libd->shared_state->plugin_argc;
-  plugin_argv = libd->shared_state->plugin_argv;
+  //plugin_argc = libd->shared_state->plugin_argc;
+  //plugin_argv = libd->shared_state->plugin_argv;
 
 
   libd->shared_state->mpi_comm_ptr = &libd->mpi_comm;
   libd->shared_state->driver_node_callback = libd->driver_node_callback;
   libd->shared_state->driver_mdi_comm = driver_comm->id;
   libd->shared_state->driver_activate_code = library_activate_code;
   libd->shared_state->driver_callback_obj = libd->driver_callback_obj;
@@ -465,15 +546,14 @@
 
 
 
 
   /*************************************************/
   /*************** BEGIN PLUGIN MODE ***************/
   /*************************************************/
-  plugin_mode = 1;
 
   ret = library_load_init(plugin_name, mpi_comm_ptr, libd, 0);
   if ( ret != 0 ) {
     free( plugin_path );
     free( plugin_init_name );
     return ret;
   }
@@ -482,18 +562,17 @@
   int is_python = libd->is_python;
 #ifdef _WIN32
   HINSTANCE plugin_handle = libd->plugin_handle;
 #else
   void* plugin_handle = libd->plugin_handle;
 #endif
 
-  plugin_mode = 0;
 //  current_code = libd->shared_state->driver_code_id;
 //  current_code = libd->shared_state->driver_code_id;
-  libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+  libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr, libd->shared_state->driver_code_id );
 
   // Delete the driver's communicator to the engine
   // This will also delete the engine code and its communicator
   delete_communicator(libd->shared_state->driver_code_id, comm);
 
   if (is_python == 0 ) {
   // Close the plugin library
@@ -520,21 +599,31 @@
 
 /*! \brief Open an MDI plugin in the background
  *
  */
 int library_open_plugin(const char* plugin_name, const char* options, void* mpi_comm_ptr,
                           MDI_Comm* mdi_comm_ptr) {
   int ret;
-  int driver_code_id = current_code;
-  code* this_code = get_code(driver_code_id);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_open_plugin: get_current_code failed");
+    return 1;
+  }
   MPI_Comm mpi_comm = *(MPI_Comm*) mpi_comm_ptr;
 
   // initialize a communicator for the driver
   int icomm = library_initialize();
-  communicator* driver_comm = get_communicator(current_code, icomm);
+  communicator* driver_comm;
+  ret = get_communicator(codes.current_key, icomm, &driver_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_open_plugin: get_communicator failed");
+    return ret;
+  }
   library_data* libd = (library_data*) driver_comm->method_data;
   libd->connected_code = (int)codes.size;
 
   MDI_Comm comm;
   ret = MDI_Accept_Communicator(&comm);
   if ( ret != 0 || comm == MDI_COMM_NULL ) {
     mdi_error("MDI unable to create communicator for plugin");
@@ -544,228 +633,203 @@
   // Set the mpi communicator associated with this plugin instance
   libd->mpi_comm = mpi_comm;
 
   // Parse plugin command-line options
   library_parse_options(options, libd);
 
   // Assign the global command-line options variables to the values for this plugin  
-  plugin_argc = libd->shared_state->plugin_argc;
-  plugin_argv = libd->shared_state->plugin_argv;
-  plugin_unedited_options = libd->plugin_unedited_options;
+  //plugin_argc = libd->shared_state->plugin_argc;
+  //plugin_argv = libd->shared_state->plugin_argv;
+  //plugin_unedited_options = libd->plugin_unedited_options;
 
   //
   // Get the path to the plugin
   // Note: Eventually, should probably replace this code with libltdl
   //
   char* plugin_path = malloc( PLUGIN_PATH_LENGTH * sizeof(char) );
 
   // Get the name of the plugin's init function
   char* plugin_init_name = malloc( PLUGIN_PATH_LENGTH * sizeof(char) );
   snprintf(plugin_init_name, PLUGIN_PATH_LENGTH, "MDI_Plugin_open_%s", plugin_name);
 
   /*************************************************/
   /*************** BEGIN PLUGIN MODE ***************/
   /*************************************************/
-  plugin_mode = 1;
 
   library_load_init(plugin_name, mpi_comm_ptr, libd, 1);
   if ( ret != 0 ) {
     free( plugin_path );
     free( plugin_init_name );
     return ret;
   }
 
   /*************************************************/
   /**************** END PLUGIN MODE ****************/
   /*************************************************/
-  plugin_mode = 0;
-//  current_code = driver_code_id;
-//  current_code = libd->shared_state->driver_code_id;
-  libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+
+  // Set the driver as the active code
+  libd->shared_state->driver_activate_code(
+                  libd->shared_state->driver_codes_ptr,
+                  libd->shared_state->driver_code_id );
 
   // Delete the driver's communicator to the engine
   // This will also delete the engine code and its communicator
   //delete_communicator(driver_code_id, comm);
 
   // free memory from loading the plugin's initialization function
   free( plugin_path );
   free( plugin_init_name );
 
   *mdi_comm_ptr = comm;
   return 0;
 }
 
 int library_close_plugin(MDI_Comm mdi_comm) {
-  code* this_code = get_code(current_code);
-  communicator* this_comm = get_communicator(this_code->id, mdi_comm);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_close_plugin: get_current_code failed");
+    return 1;
+  }
+  communicator* this_comm;
+  ret = get_communicator(this_code->id, mdi_comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_close_plugin: get_communicator failed");
+    return ret;
+  }
   library_data* libd = (library_data*) this_comm->method_data;
 
   if (libd->is_python == 0 ) {
   // Close the plugin library
 #ifdef _WIN32
     FreeLibrary( libd->plugin_handle );
 #else
     dlclose( libd->plugin_handle );
 #endif
   }
 
   // Delete the driver's communicator to the engine
   // This will also delete the engine code and its communicator
-  delete_communicator(current_code, mdi_comm);
+  delete_communicator(codes.current_key, mdi_comm);
   
   return 0;
 }
 
 
 /*! \brief Perform initialization of a communicator for library-based communication
  *
  */
 int library_initialize() {
-  code* this_code = get_code(current_code);
+  int ret;
 
-  MDI_Comm comm_id = new_communicator(this_code->id, MDI_LINK);
-  communicator* new_comm = get_communicator(this_code->id, comm_id);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_initialize: get_current_code failed");
+    return 1;
+  }
+
+  MDI_Comm comm_id;
+  ret = new_communicator(this_code->id, MDI_LINK, &comm_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_initialize: new_communicator failed");
+    return 1;
+  }
+  communicator* new_comm;
+  ret = get_communicator(this_code->id, comm_id, &new_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_initialize: get_communicator failed");
+    return ret;
+  }
   new_comm->delete = communicator_delete_lib;
   new_comm->send = library_send;
   new_comm->recv = library_recv;
 
   // set the MDI version number of the new communicator
   new_comm->mdi_version[0] = MDI_MAJOR_VERSION;
   new_comm->mdi_version[1] = MDI_MINOR_VERSION;
   new_comm->mdi_version[2] = MDI_PATCH_VERSION;
   new_comm->name_length = MDI_NAME_LENGTH;
   new_comm->command_length = MDI_COMMAND_LENGTH;
 
   // allocate the method data
   library_data* libd = malloc(sizeof(library_data));
-  //libd->connected_code = -1;
-  //libd->buf_allocated = 0;
   libd->execute_on_send = 0;
   libd->mpi_comm = MPI_COMM_NULL;
-  libd->plugin_options_allocated = 0;
-  libd->plugin_options = NULL;
-  libd->plugin_unedited_options = NULL;
 
   new_comm->method_data = libd;
 
   // if this is an engine, go ahead and set the driver as the connected code
   if ( strcmp(this_code->role, "ENGINE") == 0 ) {
-    //int engine_code = current_code;
-    //library_set_driver_current();
-    //int driver_code_id = current_code;
-    //libd->connected_code = driver_code_id;
-    //current_code = engine_code;
-    libd->shared_state = shared_state_from_driver;
+
+    libd->shared_state = (plugin_shared_state*) this_code->shared_state_from_driver;
     libd->shared_state->engine_mdi_comm = new_comm->id;
     libd->shared_state->delete_engine = library_delete_engine;
     libd->shared_state->engine_activate_code = library_activate_code;
     libd->shared_state->lib_execute_command = library_execute_command;
-    libd->shared_state->engine_code_id = current_code;
-//    current_code = libd->shared_state->engine_code_id;
+    libd->shared_state->engine_code_id = codes.current_key;
+    libd->shared_state->engine_codes_ptr = &codes;
+    libd->shared_state->execute_builtin = general_builtin_command;
+    libd->shared_state->engine_nodes = (void*)this_code->nodes;
+    this_code->plugin_argc = libd->shared_state->plugin_argc;
+    this_code->plugin_argv = libd->shared_state->plugin_argv;
+    this_code->plugin_unedited_options = libd->shared_state->plugin_unedited_options;
 
     // set the engine's mpi communicator
-    //if ( plugin_mode ) {
-      // get the driver's library data
-      //code* driver_code = get_code(driver_code_id);
-      //MDI_Comm matching_handle = library_get_matching_handle(comm_id);
-      //communicator* driver_comm = get_communicator(driver_code->id, matching_handle);
-      //library_data* driver_libd = (library_data*) driver_comm->method_data;
+    libd->mpi_comm = *(MPI_Comm*)libd->shared_state->mpi_comm_ptr;
+    this_code->intra_MPI_comm = libd->mpi_comm;
 
+    // check whether MPI has been initialized
+    int mpi_init_flag;
+    if ( MPI_Initialized(&mpi_init_flag) ) {
+      mdi_error("Error in MDI_Init: MPI_Initialized failed");
+      return 1;
+    }
 
-
-      //libd->mpi_comm = driver_libd->mpi_comm;
-      libd->mpi_comm = *(MPI_Comm*)libd->shared_state->mpi_comm_ptr;
-      this_code->intra_MPI_comm = libd->mpi_comm;
-
-      // check whether MPI has been initialized
-      int mpi_init_flag;
-      if ( MPI_Initialized(&mpi_init_flag) ) {
-        mdi_error("Error in MDI_Init: MPI_Initialized failed");
-        return 1;
-      }
-
-      // Set the engine's MPI rank
-      if ( mpi_init_flag == 1 ) {
-        MPI_Comm_rank( this_code->intra_MPI_comm, &this_code->intra_rank );
-      }
-      else {
-        this_code->intra_rank = 0;
-      }
+    // Set the engine's MPI rank
+    if ( mpi_init_flag == 1 ) {
+      MPI_Comm_rank( this_code->intra_MPI_comm, &this_code->intra_rank );
+    }
+    else {
+      this_code->intra_rank = 0;
+    }
       
-      libd->shared_state->intra_rank = this_code->intra_rank;
-    //}
+    libd->shared_state->intra_rank = this_code->intra_rank;
 
   }
 
   return new_comm->id;
 }
 
 
 /*! \brief Set the driver as the current code
  *
  */
 int library_set_driver_current(MDI_Comm comm) {
-  code* this_code = get_code(current_code);
-  communicator* this_comm = get_communicator(current_code, comm);
-  library_data* libd = (library_data*) this_comm->method_data;
-
-  //current_code = libd->shared_state->driver_code_id;
-  libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
-
-  return 0;
-}
-
+  int ret;
 
-/*! \brief Perform LIBRARY method operations upon a call to MDI_Accept_Communicator
- *
- */
-int library_accept_communicator() {
-  code* this_code = get_code(current_code);
-  /*
-  if ( this_code->called_set_execute_command_func && (! plugin_mode) ) {
-    // library codes are not permitted to call MDI_Accept_communicator after calling
-    // MDI_Set_execute_command_func, so assume that this call is being made by the driver
-    library_set_driver_current();
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_set_driver_current: get_current_code failed");
+    return 1;
   }
-  */
-  this_code = get_code(current_code);
-
-  // if this is a DRIVER, check if there are any ENGINES that are linked to it
-  if ( strcmp(this_code->role, "DRIVER") == 0 ) {
-
-    int icode;
-    int found_engine = 0;
-    int iengine = 0;
-    for ( icode = 0; icode < codes.size; icode++ ) {
-      code* other_code = vector_get(&codes, icode);
-      if ( strcmp(other_code->role, "ENGINE") == 0 ) {
-	if ( other_code->is_library == 1 ) {
-	  // flag that this library has connected to the driver
-	  other_code->is_library = 2;
-
-	  //iengine = icode;
-	  iengine = other_code->id;
-	  found_engine = 1;
-	  break;
-	}
-      }
-    }
-
-    // create a new communicator for this engine
-    if ( found_engine == 1 ) {
-      int icomm = library_initialize();
-
-      // set the connected code for the driver
-      code* engine_code = get_code(iengine);
-      communicator* this_comm = get_communicator(current_code, icomm);
-      library_data* libd = (library_data*) this_comm->method_data;
-      libd->connected_code = engine_code->id;
-    }
-
+  communicator* this_comm;
+  ret = get_communicator(codes.current_key, comm, &this_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_set_driver_current: get_communicator failed");
+    return ret;
   }
+  library_data* libd = (library_data*) this_comm->method_data;
+
+  // set the driver as the active code
+  libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr,
+                                            libd->shared_state->driver_code_id );
 
   return 0;
 }
 
 
 
 /*! \brief Set the next command that will be executed through the library communicator
@@ -775,15 +839,22 @@
  *
  * \param [in]       command
  *                   Pointer to the command to be executed.
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int library_set_command(const char* command, MDI_Comm comm) {
-  communicator* this = get_communicator(current_code, comm);
+  int ret;
+
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_set_command: get_communicator failed");
+    return ret;
+  }
 
   // get the engine code to which this communicator connects
   library_data* libd = (library_data*) this->method_data;
   //int iengine = libd->connected_code;
 
   // get the matching engine communicator
   //MDI_Comm engine_comm_handle = library_get_matching_handle(comm);
@@ -806,50 +877,54 @@
  * \param [in]       command
  *                   Pointer to the command to be executed.
  * \param [in]       comm
  *                   MDI communicator associated with the intended recipient code.
  */
 int library_execute_command(MDI_Comm comm) {
   int ret = 0;
-
-  int idriver = current_code;
-  communicator* this = get_communicator(current_code, comm);
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_execute_command: get_communicator failed");
+    return ret;
+  }
 
   // get the engine code to which this communicator connects
   library_data* libd = (library_data*) this->method_data;
   //int iengine = libd->connected_code;
-  //code* engine_code = get_code(iengine);
 
   //MDI_Comm engine_comm_handle = library_get_matching_handle(comm);
   MDI_Comm engine_comm_handle = libd->shared_state->engine_mdi_comm;
   //communicator* engine_comm = get_communicator(iengine, engine_comm_handle);
   //library_data* engine_lib = (library_data*) engine_comm->method_data;
 
   // set the current code to the engine
-//  current_code = iengine;
-//  current_code = libd->shared_state->engine_code_id;
-  libd->shared_state->engine_activate_code( libd->shared_state->engine_code_id );
+  libd->shared_state->engine_activate_code( libd->shared_state->engine_codes_ptr,
+                                            libd->shared_state->engine_code_id );
 
   // check if this command corresponds to one of MDI's standard built-in commands
   //int builtin_flag = general_builtin_command(engine_lib->command, engine_comm_handle);
-  int builtin_flag = general_builtin_command(libd->shared_state->command, engine_comm_handle);
+  int builtin_flag;
+  //ret = general_builtin_command(libd->shared_state->command, engine_comm_handle, &builtin_flag);
+  ret = libd->shared_state->execute_builtin(libd->shared_state->command,
+                                            engine_comm_handle,
+                                            &builtin_flag);
   //int builtin_flag = 0;
 
   if ( builtin_flag == 0 ) {
     // call execute_command now
     //void* class_obj = engine_code->execute_command_obj;
     void* class_obj = libd->shared_state->execute_command_obj;
     //ret = engine_code->execute_command(engine_lib->command,engine_comm_handle,class_obj);
-    ret = libd->shared_state->execute_command(libd->shared_state->command, engine_comm_handle, class_obj);
+    ret = libd->shared_state->execute_command_wrapper(libd->shared_state->command, engine_comm_handle, class_obj);
   }
 
   // set the current code to the driver
-//  current_code = idriver;
-//  current_code = libd->shared_state->driver_code_id;
-  libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+  libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr,
+                                            libd->shared_state->driver_code_id );
 
   return ret;
 }
 
 
 
 /*! \brief Function to handle sending data through an MDI connection, using library-based communication
@@ -867,20 +942,28 @@
  *                   0: Not part of a message.
  *                   1: The header of a message.
  *                   2: The body (data) of a message.
  */
 int library_send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag) {
   int ret;
 
-  code* this_code = get_code(current_code);
-  communicator* this = get_communicator(current_code, comm);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_send: get_current_code failed");
+    return 1;
+  }
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_send: get_communicator failed");
+    return ret;
+  }
   library_data* libd = (library_data*) this->method_data;
 
-  //code* other_code = get_code(libd->connected_code);
-
   // get the rank of this process on the engine
   /*
   int engine_rank = 0;
   if ( this_code->is_library ) {
     engine_rank = this_code->intra_rank;
   }
   else {
@@ -964,19 +1047,19 @@
   }
 
   // check whether the recipient code should now execute its command
   if ( msg_flag == 2 && libd->execute_on_send ) {
     // have the recipient code execute its command
     //library_execute_command(comm);
 
-    libd->shared_state->engine_activate_code( libd->shared_state->engine_code_id );
+    libd->shared_state->engine_activate_code( libd->shared_state->engine_codes_ptr, libd->shared_state->engine_code_id );
 
     libd->shared_state->lib_execute_command(libd->shared_state->engine_mdi_comm);
 
-    libd->shared_state->driver_activate_code( libd->shared_state->driver_code_id );
+    libd->shared_state->driver_activate_code( libd->shared_state->driver_codes_ptr, libd->shared_state->driver_code_id );
 
     // turn off the execute_on_send flag
     libd->execute_on_send = 0;
   }
 
   return 0;
 }
@@ -998,19 +1081,28 @@
  *                   0: Not part of a message.
  *                   1: The header of a message.
  *                   2: The body (data) of a message.
  */
 int library_recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag) {
   int ret;
 
-  code* this_code = get_code(current_code);
-  communicator* this = get_communicator(current_code, comm);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_recv: get_current_code failed");
+    return 1;
+  }
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_recv: get_communicator failed");
+    return ret;
+  }
   library_data* libd = (library_data*) this->method_data;
 
-  //code* other_code = get_code(libd->connected_code);
   //MDI_Comm other_comm_handle = library_get_matching_handle(comm);
   //communicator* other_comm = get_communicator(libd->connected_code, other_comm_handle);
   //library_data* other_lib = (library_data*) other_comm->method_data;
 
   // only recv from rank 0 of the engine
   /*
   int engine_rank = 0;
@@ -1041,15 +1133,15 @@
     return 1;
   }
 
   // receive message header information
   // only do this if communicating with MDI version 1.1 or higher
   if ( ( this->mdi_version[0] > 1 ||
 	 ( this->mdi_version[0] == 1 && this->mdi_version[1] >= 1 ) )
-       && ipi_compatibility != 1 ) {
+       && this_code->ipi_compatibility != 1 ) {
 
     if ( msg_flag == 1 ) { // message header
 
       memcpy(buf, libd->shared_state->buf, count * datasize);
 
     }
     else if ( msg_flag == 2 ) { // message body
@@ -1076,78 +1168,113 @@
 }
 
 
 
 /*! \brief Function for LIBRARY-specific deletion operations for communicator deletion
  */
 int communicator_delete_lib(void* comm) {
+  int ret;
   communicator* this_comm = (communicator*) comm;
-  code* this_code = get_code(this_comm->code_id);
+  code* this_code;
+  ret = get_code(this_comm->code_id, &this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in communicator_delete_lib: get_code failed");
+    return ret;
+  }
   library_data* libd = (library_data*) this_comm->method_data;
 
-  // if this is the driver, delete the engine code
+  // if this is the driver, delete the engine code and shared state
   if ( this_code->is_library == 0 ) {
-    //delete_code(libd->connected_code);
-    libd->shared_state->delete_engine( libd->shared_state->engine_code_id );
+
+    // set the engine as the active code
+    ret = libd->shared_state->engine_activate_code(
+                    libd->shared_state->engine_codes_ptr,
+                    libd->shared_state->engine_code_id );
+    if ( ret != 0 ) {
+      mdi_error("Error in communicator_delete_lib: engine_activate_code failed");
+      return ret;
+    }
+
+    // delete the engine code
+    ret = libd->shared_state->delete_engine(
+                    libd->shared_state->engine_code_id );
+    if ( ret != 0 ) {
+      mdi_error("Error in communicator_delete_lib: delete_engine failed");
+      return ret;
+    }
+
+    // set the driver as the active code
+    ret = libd->shared_state->driver_activate_code(
+                    libd->shared_state->driver_codes_ptr,
+                    libd->shared_state->driver_code_id );
+    if ( ret != 0 ) {
+      mdi_error("Error in communicator_delete_lib: driver_activate_code failed");
+      return ret;
+    }
 
     if ( libd->shared_state->plugin_argv_allocated ) {
       free( libd->shared_state->plugin_argv );
+      free( libd->shared_state->plugin_options );
+      free( libd->shared_state->plugin_unedited_options );
     }
 
     // delete the method-specific information
     if ( libd->shared_state->buf_allocated ) {
       free( libd->shared_state->buf );
     }
 
     // delete the shared state, but only on the driver side
     free( libd->shared_state );
 
   }
 
-  if ( libd->plugin_options_allocated ) {
-    free( libd->plugin_options );
-    free( libd->plugin_unedited_options );
-  }
-
   free( libd );
 
   return 0;
 }
 
 
 /*! \brief Function to delete all of the engine's state
  */
-int library_delete_engine(int code_id) {
+int library_delete_engine(size_t code_id) {
   delete_code(code_id);
   if ( codes.size == 0 ) {
     free(codes.data);
   }
-  //free(methods.data);
   return 0;
 }
 
 
-
 /*! \brief Function to set the plugin's state
  */
 int library_set_state(void* state) {
-  shared_state_from_driver = (plugin_shared_state*) state;
+  int ret;
 
-  // activate plugin mode
-  plugin_mode = 1;
-  //is_initialized = 1;
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in library_set_state: get_current_code failed");
+    return 1;
+  }
+  this_code->shared_state_from_driver = state;
 
-  
+  plugin_shared_state* shared_state = (plugin_shared_state*) state;
 
-  MDI_Init(&shared_state_from_driver->plugin_argc, &shared_state_from_driver->plugin_argv);
+  ret = MDI_Init_with_argv(&shared_state->plugin_argc, 
+                           &shared_state->plugin_argv);
+  if ( ret != 0 ) {
+    return ret;
+  }
 
   return 0;
 }
 
 
 /*! \brief Function to set the active code
  */
-int library_activate_code(int code_id) {
-  current_code = code_id;
+int library_activate_code(void* codes_in, int code_id) {
+
+  vector* codes_vec = (vector*) codes_in;
+  codes_vec->current_key = code_id;
 
   return 0;
 }
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_lib.h` & `pymdi-1.4.9/MDI_Library/mdi_lib.h`

 * *Files 8% similar despite different names*

```diff
@@ -13,65 +13,76 @@
 
 typedef struct plugin_shared_state_struct {
   /*! \brief Name of the next command to be executed on this code.
   This is only used by engines. */
   char command[MDI_COMMAND_LENGTH_];
   /*! \brief Buffer used for communication of data */
   void* buf;
-  /*! \brief Function pointer to the driver node's callback function */
-  MDI_Driver_node_callback_t driver_node_callback;
   /*! \brief Argument vector for plugin command-line options */
   char** plugin_argv;
+  /*! \brief Command-line options for currently running plugin */
+  char* plugin_options;
+  /*! \brief Unedited command-line options for currently running plugin */
+  char* plugin_unedited_options;
   /*! \brief Pointer to the intra-communicator for the plugin */
   void* mpi_comm_ptr;
   /*! \brief Pointer to the class object that is used for the driver_node_callback function */
   void* driver_callback_obj;
+  /*! \brief Pointer to the class object that is passed to any call to execute_command */
+  void* execute_command_obj;
+  /*! \brief Pointer to the original Python interpreter's dictionary.
+   * Only used for Python plugins */
+  void* python_interpreter_dict;
+  /*! \brief Pointer to the driver's codes vector */
+  void* driver_codes_ptr;
+  /*! \brief Pointer to the engine's codes vector */
+  void* engine_codes_ptr;
+  /*! \brief Pointer to the engine's nodes vector */
+  void* engine_nodes;
   /*! \brief Function pointer to the driver's library_activate_code function */
-  int (*driver_activate_code)(int);
+  int (*driver_activate_code)(void*, int);
   /*! \brief Function pointer to the engine's library_activate_code function */
-  int (*engine_activate_code)(int);
+  int (*engine_activate_code)(void*, int);
   /*! \brief Function pointer to the library execute command function */
   int (*lib_execute_command)(MDI_Comm);
-  /*! \brief Function pointer to the generic execute command function */
-  int (*execute_command)(const char*, MDI_Comm_Type, void*);
+  /*! \brief Function pointer to a wrapper for the language-specific execute command function */
+  int (*execute_command_wrapper)(const char*, MDI_Comm_Type, void*);
+  /*! \brief Function pointer to the engine's function for responding to built-in commands */
+  int (*execute_builtin)(const char*, MDI_Comm_Type, int*);
   /*! \brief Function pointer to the engine's function to delete everything */
-  int (*delete_engine)(int);
-  /*! \brief Pointer to the class object that is passed to any call to execute_command */
-  void* execute_command_obj;
+  int (*delete_engine)(size_t);
+  /*! \brief Engine-side ID of the engine code */
+  size_t engine_code_id;
+  /*! \brief Driver-side ID of the driver code */
+  size_t driver_code_id;
+  /*! \brief Pointer to engine's execute_command function */
+  MDI_execute_command_type execute_command;
+  /*! \brief Function pointer to the driver node's callback function */
+  MDI_Driver_node_callback_t driver_node_callback;
   /*! \brief Driver-side MDI communicator */
   MDI_Comm driver_mdi_comm;
   /*! \brief Engine-side MDI communicator */
   MDI_Comm engine_mdi_comm;
   /*! \brief Flag whether buf is allocated */
   int buf_allocated;
   /*! \brief Argument count for plugin command-line options */
   int plugin_argc;
   /*! \brief Flag whether plugin_argv is allocted for this code */
   int plugin_argv_allocated;
   /*! \brief MPI rank of this process within the plugin  */
   int intra_rank;
-  /////////////////////////////////////////////////////////////
-  /*! \brief Engine-side ID of the engine code */
-  int engine_code_id;
-  /*! \brief Driver-side ID of the driver code */
-  int driver_code_id;
   /*! \brief Flag whether the engine is a Python code */
   int engine_language;
-  //////////////////////////////////////////////////////////////
+  /*! \brief Flag whether the Python interpreter has been initialized */
+  int python_interpreter_initialized;
 } plugin_shared_state;
 
 typedef struct library_data_struct {
   /*! \brief State shared between the driver and the plugin */
   plugin_shared_state* shared_state;
-  /*! \brief Command-line options for currently running plugin */
-  char* plugin_options;
-  /*! \brief Unedited command-line options for currently running plugin */
-  char* plugin_unedited_options;
-  /*! \brief Flag whether plugin_options is allocted for this code */
-  int plugin_options_allocated;
   /*! \brief Handle of the code to which this communicator connects */
   int connected_code;
   /*! \brief Flag whether the next MDI_Send call should trigger execution of the engine's command */
   int execute_on_send;
   /*! \brief MPI intra-communicator for the engine */
   MPI_Comm mpi_comm;
   /*! \brief Pointer to the class object that is used for the driver_node_callback function */
@@ -87,17 +98,14 @@
 #endif
   /*! \brief Initialization function for the plugin library */
   MDI_Plugin_init_t plugin_init;
   /*! \brief Flag whether this communicator connects to a Python library */
   int is_python;
 } library_data;
 
-/*! \brief Shared state received from the driver */
-extern plugin_shared_state* shared_state_from_driver;
-
 int enable_plug_support(int code_id);
 int plug_on_selection();
 int plug_on_accept_communicator();
 int plug_on_send_command(const char* command, MDI_Comm comm, int* skip_flag);
 int plug_after_send_command(const char* command, MDI_Comm comm);
 int plug_on_recv_command(MDI_Comm comm);
 
@@ -107,23 +115,24 @@
 int library_launch_plugin(const char* plugin_name, const char* options, void* mpi_comm_ptr,
                           MDI_Driver_node_callback_t driver_node_callback,
                           void* driver_callback_object);
 int library_open_plugin(const char* plugin_name, const char* options, void* mpi_comm_ptr,
                           MDI_Comm* mdi_comm_ptr);
 int library_close_plugin(MDI_Comm mdi_comm);
 int library_initialize();
-int library_accept_communicator();
 int library_set_driver_current();
 int library_set_command(const char* command, MDI_Comm comm);
 int library_execute_command(MDI_Comm comm);
 int library_send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag);
 int library_recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag);
 int library_send_msg(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm);
 int library_recv_msg(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm);
 
 int library_set_state(void* state);
-int library_activate_code(int code_id);
+int library_activate_code(void* codes_in, int code_id);
+int library_activate_driver(library_data* libd);
+int library_activate_engine(library_data* libd);
 
 int communicator_delete_lib(void* comm);
-int library_delete_engine(int code_id);
+int library_delete_engine(size_t code_id);
 
 #endif
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_mpi.c` & `pymdi-1.4.9/MDI_Library/mdi_mpi.c`

 * *Files 22% similar despite different names*

```diff
@@ -15,53 +15,91 @@
 
 /*! \brief Set the size of MPI_COMM_WORLD
  *
  * \param [in]       world_size_in
  *                   Size of MPI_COMM_WORLD
  */
 int set_world_size(int world_size_in) {
-  world_size = world_size_in;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in set_world_size: get_current_code failed");
+    return 1;
+  }
+
+  this_code->world_size = world_size_in;
   return 0;
 }
 
 
 /*! \brief Set the rank of this process in MPI_COMM_WORLD
  *
  * \param [in]       world_rank_in
  *                   Rank of this process within MPI_COMM_WORLD
  */
 int set_world_rank(int world_rank_in) {
-  world_rank = world_rank_in;
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in set_world_rank: get_current_code failed");
+    return 1;
+  }
+
+  this_code->world_rank = world_rank_in;
+  this_code->intra_rank = world_rank_in;
   return 0;
 }
 
 
 /*! \brief Enable support for the TCP method */
 int enable_mpi_support(int code_id) {
-  new_method(code_id, MDI_MPI);
-  method* this_method = get_method(code_id, MDI_MPI);
+  int ret;
+  int method_id;
+  ret = new_method(code_id, MDI_MPI, &method_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_mpi_support: new_method failed");
+    return ret;
+  }
+  method* this_method;
+  ret = get_method(code_id, MDI_MPI, &this_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_mpi_support: get_method failed");
+    return ret;
+  }
   this_method->on_selection = mpi_on_selection;
   this_method->on_accept_communicator = mpi_on_accept_communicator;
   this_method->on_send_command = mpi_on_send_command;
   this_method->after_send_command = mpi_after_send_command;
   this_method->on_recv_command = mpi_on_recv_command;
   return 0;
 }
 
 
 /*! \brief Callback when the end-user selects MPI as the method */
 int mpi_on_selection() {
   int ret;
-  code* this_code = get_code(current_code);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_on_selection: get_current_code failed");
+    return 1;
+  }
+
   int mpi_initialized = 0;
 
-  if ( is_initialized == 1 ) {
-    mdi_error("MDI_Init called after MDI was already initialized");
+  if ( this_code->mpi_initialized == 1 ) {
+    mdi_error("MDI_Init called after MPI was already initialized");
     return 1;
   }
+  this_code->mpi_initialized = 1;
 
   // ensure MPI has been initialized
   int mpi_init_flag = 0;
 
   ret = MPI_Initialized(&mpi_init_flag);
   if ( ret != 0 ) {
     mdi_error("Error in MDI_Init: MPI_Initialized failed");
@@ -87,52 +125,51 @@
       return ret;
     }
     if ( mpi_init_flag == 0 ) {
       mdi_error("Error in MDI_Init: Failed to initialize MPI. Check that the MDI Library is linked to an MPI library.");
       return 1;
     }
 
-    initialized_mpi = 1;
+    this_code->initialized_mpi = 1;
   }
 
   // get the appropriate MPI communicator to use
   MPI_Comm mpi_communicator;
   ret = MPI_Initialized(&mpi_init_flag);
   if ( ret != 0 ) {
     mdi_error("Error in MDI_Init: MPI_Initialized failed");
     return ret;
   }
   if ( mpi_init_flag == 0 ) {
     mpi_communicator = 0;
   }
   else {
-    if ( this_code->language == MDI_LANGUAGE_PYTHON && ( ! initialized_mpi ) ) {
+    if ( this_code->language == MDI_LANGUAGE_PYTHON && ( ! this_code->initialized_mpi ) ) {
       mpi_communicator = 0;
     }
     else {
       mpi_communicator = MPI_COMM_WORLD;
-      MPI_Comm_rank(mpi_communicator, &world_rank);
-      MPI_Comm_size(mpi_communicator, &world_size);
-      this_code->intra_rank = world_rank;
+      MPI_Comm_rank(mpi_communicator, &this_code->world_rank);
+      MPI_Comm_size(mpi_communicator, &this_code->world_size);
+      this_code->intra_rank = this_code->world_rank;
     }
   }
 
   // determine whether the intra-code MPI communicator should be split
   int use_mpi4py = 0;
-  if ( this_code->language == MDI_LANGUAGE_PYTHON && ( ! initialized_mpi ) ) {
+  if ( this_code->language == MDI_LANGUAGE_PYTHON && ( ! this_code->initialized_mpi ) ) {
     use_mpi4py = 1;
   }
 
   // split intra-communicators for each code
   if ( strcmp(this_code->role, "DRIVER") == 0 ) {
     mpi_identify_codes("", use_mpi4py, mpi_communicator);
     mpi_initialized = 1;
   }
   else if ( strcmp(this_code->role,"ENGINE") == 0 ) {
-    code* this_code = get_code(current_code);
     mpi_identify_codes(this_code->name, use_mpi4py, mpi_communicator);
     mpi_initialized = 1;
   }
   else {
     mdi_error("Error in MDI_Init: Role not recognized");
     return 1;
   }
@@ -140,20 +177,32 @@
   return 0;
 }
 
 
 
 /*! \brief Callback when the MPI method must accept a communicator */
 int mpi_on_accept_communicator() {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_on_accept_communicator: get_current_code failed");
+    return 1;
+  }
 
   // If MDI hasn't returned some connections, do that now
   if ( this_code->returned_comms < this_code->next_comm - 1 ) {
     this_code->returned_comms++;
-    communicator* comm_obj = get_communicator(current_code, this_code->returned_comms);
+    communicator* comm_obj;
+    ret = get_communicator(codes.current_key, this_code->returned_comms, &comm_obj);
+    if ( ret != 0 ) {
+      mdi_error("Error in mpi_on_accept_communicator: get_communicator failed");
+      return ret;
+    }
     comm_obj->is_accepted = 1;
     return this_code->returned_comms;
   }
 
   // unable to accept any connections
   return MDI_COMM_NULL;
 }
@@ -165,23 +214,30 @@
   return 0;
 }
 
 
 
 /*! \brief Callback after the MPI method has received a command */
 int mpi_after_send_command(const char* command, MDI_Comm comm) {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_after_send_command: get_current_code failed");
+    return 1;
+  }
 
   // if the command was "EXIT", delete this communicator
   if ( strcmp( command, "EXIT" ) == 0 ) {
-    delete_communicator(current_code, comm);
+    delete_communicator(codes.current_key, comm);
   }
 
   // if MDI called MPI_Init, and there are no more communicators, call MPI_Finalize now
-  if ( initialized_mpi == 1 ) {
+  if ( this_code->initialized_mpi == 1 ) {
     if ( this_code->comms->size == 0 ) {
       MPI_Finalize();
     }
   }
   
   return 0;
 }
@@ -209,65 +265,71 @@
  *                   Should normally be set to 0, unless the code associated with this process is a Python code.
  *                   In that case, the Python wrapper code will do the split instead.
  */
 int mpi_identify_codes(const char* code_name, int use_mpi4py, MPI_Comm world_comm) {
   int i, j, ret;
   int driver_rank;
   int nunique_names = 0;
-  code* this_code = get_code(current_code);
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_identify_codes: get_current_code failed");
+    return 1;
+  }
 
   // get the number of processes
   if ( use_mpi4py == 0 ) {
-    MPI_Comm_size(world_comm, &world_size);
+    MPI_Comm_size(world_comm, &this_code->world_size);
   }
   else {
     int comm_flag = 0;
-    world_size = mpi4py_size_callback(comm_flag);
+    this_code->world_size = this_code->mpi4py_size_callback(comm_flag);
   }
 
   // get the rank of this process
   if ( use_mpi4py == 0 ) {
-    MPI_Comm_rank(world_comm, &world_rank);
+    MPI_Comm_rank(world_comm, &this_code->world_rank);
   }
   else {
     int comm_flag = 0;
-    world_rank = mpi4py_rank_callback(comm_flag);
+    this_code->world_rank = this_code->mpi4py_rank_callback(comm_flag);
   }
 
   // determine the MDI version of each code
   int* my_version = malloc( sizeof(int) * 5 );
-  int* all_versions = malloc( sizeof(int) * 5 * world_size );
+  int* all_versions = malloc( sizeof(int) * 5 * this_code->world_size );
   my_version[0] = MDI_MAJOR_VERSION;
   my_version[1] = MDI_MINOR_VERSION;
   my_version[2] = MDI_PATCH_VERSION;
   my_version[3] = MDI_COMMAND_LENGTH;
   my_version[4] = MDI_NAME_LENGTH;
   if ( use_mpi4py == 0 ) {
     MPI_Allgather(my_version, 5, MPI_INT, all_versions, 5, 
         MPI_INT, world_comm);
   }
   else {
-    ret = mpi4py_allgather_callback(my_version, all_versions);
+    ret = this_code->mpi4py_allgather_callback(my_version, all_versions);
     if ( ret != 0 ) {
       mdi_error("Error in mpi4py_allgather_callback");
       return ret;
     }
   }
 
   // create a list of the name lengths of each rank
-  int* name_lengths = malloc( sizeof(int) * world_size );
-  int* name_displs = malloc( sizeof(int) * world_size );
+  int* name_lengths = malloc( sizeof(int) * this_code->world_size );
+  int* name_displs = malloc( sizeof(int) * this_code->world_size );
   name_displs[0] = 0;
-  for (i=0; i < world_size; i++) {
+  for (i=0; i < this_code->world_size; i++) {
       name_lengths[i] = all_versions[i*5 + 4];
       if ( i > 0 ) {
           name_displs[i] = name_displs[i-1] + name_lengths[i-1];
       }
   }
-  int name_array_length = name_displs[world_size-1] + name_lengths[world_size-1];
+  int name_array_length = name_displs[this_code->world_size-1] + name_lengths[this_code->world_size-1];
 
   // create the name of this process
   char* buffer = malloc( sizeof(char) * MDI_NAME_LENGTH );
   int ichar;
   for (ichar=0; ichar < MDI_NAME_LENGTH; ichar++) {
     buffer[ichar] = '\0';
   }
@@ -277,39 +339,39 @@
 
   char* names = malloc(sizeof(char) * name_array_length);
   for (ichar=0; ichar < name_array_length; ichar++) {
     names[ichar] = '\0';
   }
 
   char* unique_names = NULL;
-  unique_names = (char*)malloc(sizeof(char) * world_size*MDI_NAME_LENGTH);
-  for (ichar=0; ichar < world_size*MDI_NAME_LENGTH; ichar++) {
+  unique_names = (char*)malloc(sizeof(char) * this_code->world_size*MDI_NAME_LENGTH);
+  for (ichar=0; ichar < this_code->world_size*MDI_NAME_LENGTH; ichar++) {
     unique_names[ichar] = '\0';
   }
 
   // gather the name of the code associated with each rank
   if ( use_mpi4py == 0 ) {
     //MPI_Allgather(buffer, MDI_NAME_LENGTH, MPI_CHAR, names, MDI_NAME_LENGTH,
 	//	  MPI_CHAR, world_comm);
     MPI_Allgatherv(buffer, MDI_NAME_LENGTH, MPI_CHAR, names,
         name_lengths, name_displs,
         MPI_CHAR, world_comm);
   }
   else {
-    ret = mpi4py_gather_names_callback(buffer, names, name_lengths, name_displs);
+    ret = this_code->mpi4py_gather_names_callback(buffer, names, name_lengths, name_displs);
     if ( ret != 0 ) {
       mdi_error("Error in mpi4py_gather_names_callback");
       return ret;
     }
   }
 
   // determine which rank corresponds to rank 0 of the driver
   char* name = malloc( sizeof(char) * MDI_NAME_LENGTH );
   driver_rank = -1;
-  for (i=0; i<world_size; i++) {
+  for (i=0; i<this_code->world_size; i++) {
     if ( driver_rank == -1 ) {
       memcpy( name, &names[i*MDI_NAME_LENGTH], MDI_NAME_LENGTH );
       if ( strcmp(name, "") == 0 ) {
 	driver_rank = i;
       }
     }
   }
@@ -318,15 +380,15 @@
     return 1;
   }
 
   //create communicators
   char* prev_name = malloc( sizeof(char) * MDI_NAME_LENGTH );
   char* my_name = malloc( sizeof(char) * MDI_NAME_LENGTH );
   int mpi_code_rank = 0;
-  for (i=0; i<world_size; i++) {
+  for (i=0; i<this_code->world_size; i++) {
     memcpy( name, &names[i*MDI_NAME_LENGTH], MDI_NAME_LENGTH );
 
     int found = 0;
     for (j=0; j<i; j++) {
       memcpy( prev_name, &names[j*MDI_NAME_LENGTH], MDI_NAME_LENGTH );
       if ( strcmp(name, prev_name) == 0 ) {
 	found = 1;
@@ -334,115 +396,110 @@
     }
 
     // check if this rank is the first instance of a new production code
     if ( found == 0 && strcmp(name,"") != 0 ) {
       // add this code's name to the list of unique names
       memcpy( &unique_names[nunique_names*MDI_NAME_LENGTH], name, MDI_NAME_LENGTH );
       nunique_names++;
-      memcpy( my_name, &names[world_rank*MDI_NAME_LENGTH], MDI_NAME_LENGTH );
+      memcpy( my_name, &names[this_code->world_rank*MDI_NAME_LENGTH], MDI_NAME_LENGTH );
       if ( strcmp(my_name, name) == 0 ) {
-	mpi_code_rank = nunique_names;
+        mpi_code_rank = nunique_names;
       }
 
       // if this rank is a member of either the driver or the engine, create a new communicator
       MDI_Comm comm_id = MDI_COMM_NULL;
       if ( strcmp(my_name, "") == 0 || strcmp(my_name, name) == 0 ) {
-        comm_id = new_communicator(this_code->id, MDI_MPI);
-        communicator* new_comm = get_communicator(this_code->id, comm_id);
+        ret = new_communicator(this_code->id, MDI_MPI, &comm_id);
+        if ( ret != 0 ) {
+          mdi_error("Error in mpi_identify_codes: new_communicator failed");
+          return 1;
+        }
+        communicator* new_comm;
+        ret = get_communicator(this_code->id, comm_id, &new_comm);
+        if ( ret != 0 ) {
+          mdi_error("Error in mpi_identify_codes: get_communicator failed");
+          return ret;
+        }
 
         // set the communicator's version numbers
 
         new_comm->mdi_version[0] = all_versions[0]; // MDI_MAJOR_VERSION
         new_comm->mdi_version[1] = all_versions[1]; // MDI_MINOR_VERSION
         new_comm->mdi_version[2] = all_versions[2]; // MDI_PATCH_VERSION
         new_comm->command_length = all_versions[3]; // MDI_COMMAND_LENGTH
         new_comm->name_length = all_versions[4]; // MDI_NAME_LENGTH
       }
 
       // create an MPI communicator for inter-code communication
       MPI_Comm new_mpi_comm;
       int color = 0;
       int key = 0;
-      if ( world_rank == driver_rank ) {
-	color = 1;
+      if ( this_code->world_rank == driver_rank ) {
+        color = 1;
       }
-      else if ( world_rank == i ) {
-	color = 1;
-	key = 1;
+      else if ( this_code->world_rank == i ) {
+        color = 1;
+        key = 1;
       }
       if ( use_mpi4py == 0 ) {
-	MPI_Comm_split(world_comm, color, key, &new_mpi_comm);
+        MPI_Comm_split(world_comm, color, key, &new_mpi_comm);
       }
       else {
-	int comm_flag = 0; // indicates that this is for creating the inter-code communicator
-	mpi4py_split_callback(color, key, comm_id, comm_flag);
+        int comm_flag = 0; // indicates that this is for creating the inter-code communicator
+        this_code->mpi4py_split_callback(color, key, comm_id, comm_flag);
       }
 
       // create an MDI communicator for communication between the driver and engine
       // only done if this is a rank on either the driver or the engine
       if ( strcmp(my_name, "") == 0 || strcmp(my_name, name) == 0 ) {
-	communicator* new_comm = get_communicator(this_code->id, comm_id);
-	new_comm->delete = communicator_delete_mpi;
-	new_comm->send = mpi_send;
-	new_comm->recv = mpi_recv;
-
-	// allocate the method data
-	mpi_method_data* method_data = malloc(sizeof(mpi_method_data));
-	method_data->mpi_comm = new_mpi_comm;
-	method_data->mpi_rank = key;
-	method_data->use_mpi4py = use_mpi4py;
-	new_comm->method_data = method_data;
+        communicator* new_comm;
+        ret = get_communicator(this_code->id, comm_id, &new_comm);
+        if ( ret != 0 ) {
+          mdi_error("Error in mpi_identify_codes: second get_communicator failed");
+          return ret;
+        }
+        new_comm->delete = communicator_delete_mpi;
+        new_comm->send = mpi_send;
+        new_comm->recv = mpi_recv;
+
+        // allocate the method data
+        mpi_method_data* method_data = malloc(sizeof(mpi_method_data));
+        method_data->mpi_comm = new_mpi_comm;
+        method_data->mpi_rank = key;
+        method_data->use_mpi4py = use_mpi4py;
+        new_comm->method_data = method_data;
       }
     }
 
   }
 
   // create the intra-code communicators
   if ( use_mpi4py == 0 ) {
-    MPI_Comm_split(world_comm, mpi_code_rank, world_rank, &this_code->intra_MPI_comm);
+    MPI_Comm_split(world_comm, mpi_code_rank, this_code->world_rank, &this_code->intra_MPI_comm);
   }
   else {
-    mpi4py_split_callback(mpi_code_rank, world_rank, 0, 1);
+    this_code->mpi4py_split_callback(mpi_code_rank, this_code->world_rank, 0, 1);
   }
 
   // get the intra-code rank
   if ( use_mpi4py == 0 ) {
     MPI_Comm_rank(this_code->intra_MPI_comm, &this_code->intra_rank);
   }
   else {
-    this_code->intra_rank = mpi4py_rank_callback(1);
+    this_code->intra_rank = this_code->mpi4py_rank_callback(1);
   }
 
   // Barrier
   if ( use_mpi4py == 0 ) {
     MPI_Barrier(world_comm);
   }
   else {
-    mpi4py_barrier_callback(0);
+    this_code->mpi4py_barrier_callback(0);
   }
 
-  // communicate the version number between codes
-  /*
-  int icomm;
-  for ( icomm = 0; icomm < this_code->comms->size; icomm++ ) {
-    communicator* this_comm = vector_get(this_code->comms, icomm);
-    if (this_comm->method_id == MDI_MPI) {
-      // only communicate the version number if not using i-PI compatibility mode
-      if ( ipi_compatibility != 1 ) {
-	int version[3];
-	version[0] = MDI_MAJOR_VERSION;
-	version[1] = MDI_MINOR_VERSION;
-	version[2] = MDI_PATCH_VERSION;
-	mpi_send(&version[0], 3, MDI_INT, this_comm->id, 0);
-	mpi_recv(&this_comm->mdi_version[0], 3, MDI_INT, this_comm->id, 0);
-      }
-    }
-  }
-  */
-
   free( buffer );
   free( names );
   free( unique_names );
   free( name );
   free( prev_name );
   free( my_name );
   free( my_version );
@@ -457,15 +514,23 @@
 /*! \brief Update a pointer to MPI_COMM_WORLD to instead point to the intra-code MPI communicator
  *
  * \param [in, out]  world_comm
  *                   On input, the MPI communicator that spans all of the codes.
  *                   On output, the MPI communicator that spans the single code corresponding to the calling rank.
  */
 int mpi_update_world_comm(void* world_comm) {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_update_world_comm: get_current_code failed");
+    return 1;
+  }
+
   MPI_Comm* world_comm_ptr = (MPI_Comm*) world_comm;
   *world_comm_ptr = this_code->intra_MPI_comm;
   return 0;
 }
 
 
 /*! \brief Send data through an MDI connection, using MPI
@@ -483,34 +548,45 @@
  *                   0: Not part of a message.
  *                   1: The header of a message.
  *                   2: The body (data) of a message.
  */
 int mpi_send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag) {
   int ret;
 
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_send: get_current_code failed");
+    return 1;
+  }
+
   // only send from rank 0
-  code* this_code = get_code(current_code);
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  communicator* this = get_communicator(current_code, comm);
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_send: get_communicator failed");
+    return ret;
+  }
   mpi_method_data* method_data = (mpi_method_data*) this->method_data;
 
   // determine the byte size of the data type being sent
   MPI_Datatype mpi_type;
   ret = datatype_mpitype(datatype, &mpi_type);
   if ( ret != 0 ) { return ret; }
 
   // send the data
   if ( method_data->use_mpi4py == 0 ) {
     MPI_Send((void*)buf, count, mpi_type, (method_data->mpi_rank+1)%2, 0, method_data->mpi_comm);
   }
   else {
-    mpi4py_send_callback( (void*)buf, count, datatype, (method_data->mpi_rank+1)%2, this->id );
+    this_code->mpi4py_send_callback( (void*)buf, count, datatype, (method_data->mpi_rank+1)%2, this->id );
   }
 
   return 0;
 }
 
 
 /*! \brief Receive data through an MDI connection, using MPI
@@ -528,34 +604,45 @@
  *                   0: Not part of a message.
  *                   1: The header of a message.
  *                   2: The body (data) of a message.
  */
 int mpi_recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag) {
   int ret;
 
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_recv: get_current_code failed");
+    return 1;
+  }
+
   // only recv from rank 0
-  code* this_code = get_code(current_code);
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  communicator* this = get_communicator(current_code, comm);
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in mpi_recv: get_communicator failed");
+    return ret;
+  }
   mpi_method_data* method_data = (mpi_method_data*) this->method_data;
 
   // determine the byte size of the data type being sent
   MPI_Datatype mpi_type;
   ret = datatype_mpitype(datatype, &mpi_type);
   if ( ret != 0 ) { return ret; }
 
   // receive the data
   if ( method_data->use_mpi4py == 0 ) {
     MPI_Recv(buf, count, mpi_type, (method_data->mpi_rank+1)%2, 0, method_data->mpi_comm, MPI_STATUS_IGNORE);
   }
   else {
-    mpi4py_recv_callback( buf, count, datatype, (method_data->mpi_rank+1)%2, this->id );
+    this_code->mpi4py_recv_callback( buf, count, datatype, (method_data->mpi_rank+1)%2, this->id );
   }
 
   return 0;
 }
 
 
 /*! \brief Function for MPI-specific deletion operations for communicator deletion
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_mpi.h` & `pymdi-1.4.9/MDI_Library/mdi_mpi.h`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/MDI_Library/mdi_plug_py.c` & `pymdi-1.4.9/MDI_Library/mdi_plug_py.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 #include <mpi.h>
 #include <string.h>
 #include "mdi.h"
 #include "mdi_global.h"
+#include "mdi_lib.h"
 #include "mdi_plug_py.h"
 #include <Python.h>
 #include <stdint.h>
 
-/*! \brief Flag whether the Python interpreter has been initialized */
-int python_interpreter_initialized = 0;
-
-/*! \brief Pointer to the original Python interpreter's dictionary.
- * Only used for Python plugins */
-void* python_interpreter_dict;
-
 int print_traceback()
 {
   // Function to print the Python traceback
   
   PyObject *ptype, *pvalue, *ptraceback;
   PyObject *traceback_module;
   char *c_traceback;
@@ -66,28 +60,30 @@
   printf("%s\n", c_traceback);
   free(c_traceback);
 
   return 0;
 }
 
 int python_plugin_init( const char* engine_name, const char* engine_path, void* engine_comm_ptr, void* shared_state ) {
+  plugin_shared_state* my_state = (plugin_shared_state*) shared_state;
+
   // Initialize the Python interpreter
   // Because Python has problems with reinitialization, only initialize Python once
-  if ( ! python_interpreter_initialized ) {
+  if ( ! my_state->python_interpreter_initialized ) {
     Py_Initialize();
     if ( ! Py_IsInitialized() ) {
       mdi_error("Unable to initialize Python interpreter");
       return 1;
     }
     PyObject* main_module = PyImport_AddModule("__main__");
     PyObject* original_dict = PyModule_GetDict(main_module);
-    python_interpreter_dict = PyDict_Copy(original_dict);
-    python_interpreter_initialized = 1;
+    my_state->python_interpreter_dict = PyDict_Copy(original_dict);
+    my_state->python_interpreter_initialized = 1;
   }
-  PyObject* main_dict = PyDict_Copy(python_interpreter_dict);
+  PyObject* main_dict = PyDict_Copy(my_state->python_interpreter_dict);
 
   // Open the Python script for the Engine
   FILE* engine_script = fopen(engine_path, "r");
 
   if( engine_script ) {
 
     // Get the pointer to the plugin state
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_tcp.c` & `pymdi-1.4.9/MDI_Library/mdi_tcp.c`

 * *Files 20% similar despite different names*

```diff
@@ -18,90 +18,102 @@
 #include <errno.h>
 #include "mdi.h"
 #include "mdi_tcp.h"
 #include "mdi_global.h"
 
 static sock_t sigint_sockfd;
 
-/*! \brief Hostname of the driver */
-char* hostname = NULL;
 
-/*! \brief Port over which the driver will listen */
-int port = -1;
 
 /*! \brief SIGINT handler to ensure the socket is closed on termination
  *
  * \param [in]       dummy
  *                   Dummy argument.
  */
 void sigint_handler(int dummy) {
 #ifdef _WIN32
   closesocket(sigint_sockfd);
 #else
   close(sigint_sockfd);
 #endif
 }
 
-/*! \brief Socket over which a driver will listen for incoming connections */
-sock_t tcp_socket = -1;
-
 
 
 /*! \brief Enable support for the TCP method */
 int enable_tcp_support(int code_id) {
-  new_method(code_id, MDI_TCP);
-  method* this_method = get_method(code_id, MDI_TCP);
+  int ret;
+  int method_id;
+  ret = new_method(code_id, MDI_TCP, &method_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_tcp_support: new_method failed");
+    return ret;
+  }
+  method* this_method;
+  ret = get_method(code_id, MDI_TCP, &this_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_tcp_support: get_method failed");
+    return ret;
+  }
   this_method->on_selection = tcp_on_selection;
   this_method->on_accept_communicator = tcp_on_accept_communicator;
   this_method->on_send_command = tcp_on_send_command;
   this_method->after_send_command = tcp_after_send_command;
   this_method->on_recv_command = tcp_on_recv_command;
   return 0;
 }
 
 
 
 /*! \brief Callback when the end-user selects TCP as the method */
 int tcp_on_selection() {
-  if ( is_initialized == 1 ) {
-    mdi_error("MDI_Init called after MDI was already initialized");
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_on_selection: get_current_code failed");
     return 1;
   }
 
-  code* this_code = get_code(current_code);
+  if ( this_code->tcp_initialized == 1 ) {
+    mdi_error("MDI_Init called after TCP was already initialized");
+    return 1;
+  }
+  this_code->tcp_initialized = 1;
 
   if ( strcmp(this_code->role, "DRIVER") == 0 ) {
-    if ( port == -1 ) {
+    if ( this_code->port == -1 ) {
       mdi_error("Error in MDI_Init: -port option not provided");
       return 1;
     }
     if ( this_code->intra_rank == 0 ) {
-      tcp_listen(port);
+      tcp_listen(this_code->port);
     }
     else {
       // If this isn't rank 0, just set tcp_socket to > 0 so that accept_communicator knows we are using TCP
-      tcp_socket = 1;
+      this_code->tcp_socket = 1;
     }
   }
   else if ( strcmp(this_code->role,"ENGINE") == 0 ) {
-    if ( hostname == NULL ) {
+    if ( this_code->hostname == NULL ) {
       mdi_error("Error in MDI_Init: -hostname option not provided");
       return 1;
     }
-    if ( port == -1 ) {
+    if ( this_code->port == -1 ) {
       mdi_error("Error in MDI_Init: -port option not provided");
       return 1;
     }
     if ( this_code->intra_rank == 0 ) {
-      tcp_request_connection(port, hostname);
+      tcp_request_connection(this_code->port, this_code->hostname);
     }
     else {
       // If this isn't rank 0, just set tcp_socket to > 0 so that accept_communicator knows we are using TCP
       if ( this_code->intra_rank != 0 ) {
-	tcp_socket = 1;
+        this_code->tcp_socket = 1;
       }
     }
   }
   else {
     mdi_error("Error in MDI_Init: Role not recognized");
     return 1;
   }
@@ -109,36 +121,53 @@
   return 0;
 }
 
 
 
 /*! \brief Callback when the TCP method must accept a communicator */
 int tcp_on_accept_communicator() {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_on_accept_communicator: get_current_code failed");
+    return 1;
+  }
 
   // If MDI hasn't returned some connections, do that now
   if ( this_code->returned_comms < this_code->next_comm - 1 ) {
     this_code->returned_comms++;
-    communicator* comm_obj = get_communicator(current_code, this_code->returned_comms);
+    communicator* comm_obj;
+    ret = get_communicator(codes.current_key, this_code->returned_comms, &comm_obj);
+    if ( ret != 0 ) {
+      mdi_error("Error in tcp_on_accept_communicator: get_communicator failed");
+      return ret;
+    }
     comm_obj->is_accepted = 1;
     return this_code->returned_comms;
   }
 
   // Check for any production codes connecting via TCP
-  if ( tcp_socket > 0 ) {
+  if ( this_code->tcp_socket > 0 ) {
     // Accept a connection via TCP
     // NOTE: If this is not intra_rank==0, this will always create a dummy communicator
     int size_before = this_code->comms->size;
     tcp_accept_connection();
     int size_after = this_code->comms->size;
 
     // if MDI hasn't returned some connections, do that now
     if ( size_before < size_after ) {
       this_code->returned_comms++;
-      communicator* comm_obj = get_communicator(current_code, this_code->returned_comms);
+      communicator* comm_obj;
+      ret = get_communicator(codes.current_key, this_code->returned_comms, &comm_obj);
+      if ( ret != 0 ) {
+        mdi_error("Error in tcp_on_accept_communicator: second get_communicator failed");
+        return ret;
+      }
       comm_obj->is_accepted = 1;
       return (MDI_Comm)this_code->returned_comms;
     }
   }
 
   // unable to accept any connections
   return MDI_COMM_NULL;
@@ -152,16 +181,16 @@
 }
 
 
 
 /*! \brief Callback after the TCP method has received a command */
 int tcp_after_send_command(const char* command, MDI_Comm comm) {
   // if the command was "EXIT", delete this communicator
-  if ( ! plugin_mode && strcmp( command, "EXIT" ) == 0 ) {
-    delete_communicator(current_code, comm);
+  if ( strcmp( command, "EXIT" ) == 0 ) {
+    delete_communicator(codes.current_key, comm);
   }
 
   return 0;
 }
 
 
 
@@ -174,17 +203,23 @@
 
 /*! \brief Begin listening for incoming TCP connections
  *
  * \param [in]       port
  *                   Port to listen over
  */
 int tcp_listen(int port_in) {
-  code* this_code = get_code(current_code);
-
   int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_listen: get_current_code failed");
+    return 1;
+  }
+
   struct sockaddr_in serv_addr;
   int reuse_value = 1;
   sock_t sockfd;
 
 #ifdef _WIN32
   // initialize Winsock
   WSADATA wsa_data;
@@ -227,15 +262,15 @@
   ret = listen(sockfd, 20);
   if (ret < 0) {
     mdi_error("Could not listen");
     return 1;
   }
 
   //return sockfd;
-  tcp_socket = sockfd;
+  this_code->tcp_socket = sockfd;
 
   return 0;
 }
 
 
 /*! \brief Request a connection over TCP
  *
@@ -250,15 +285,20 @@
 
 #ifdef _WIN32
   // initialize Winsock
   WSADATA wsa_data;
   ret = WSAStartup(MAKEWORD(2,2), &wsa_data);
 #endif
 
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_request_connection: get_current_code failed");
+    return 1;
+  }
 
   struct sockaddr_in driver_address;
   struct hostent* host_ptr;
 
   // get the address of the host
   host_ptr = gethostbyname((char*) hostname_ptr);
   if (host_ptr == NULL) {
@@ -291,54 +331,64 @@
     }
 
     ret = connect(sockfd, (const struct sockaddr *) &driver_address, sizeof(struct sockaddr));
     if (ret < 0 ) {
 #ifdef _WIN32
       int sock_error = WSAGetLastError();
       if ( sock_error == WSAECONNREFUSED ) {
-	// close the socket, so that a new one can be created
-	ret = closesocket(sockfd);
+        // close the socket, so that a new one can be created
+        ret = closesocket(sockfd);
 
-	// wait a short period before attempting to connect again
-	Sleep(1000);
+        // wait a short period before attempting to connect again
+        Sleep(1000);
 #else
       if ( errno == ECONNREFUSED ) {
-	// close the socket, so that a new one can be created
-	ret = close(sockfd);
+        // close the socket, so that a new one can be created
+        ret = close(sockfd);
 
-	// wait a short period before attempting to connect again
-	sleep(1);
+        // wait a short period before attempting to connect again
+        sleep(1);
 #endif
-	if (ret != 0) {
-	  mdi_error("Could not close socket");
-	  return 1;
-	}
+        if (ret != 0) {
+          mdi_error("Could not close socket");
+          return 1;
+        }
 
       }
       else { // only error out for errors other than "connection refused"
-	mdi_error("Could not connect to the driver");
-	return 1;
+        mdi_error("Could not connect to the driver");
+        return 1;
       }
 
     }
     else {
       try_connect = 0;
     }
   }
 
-  MDI_Comm comm_id = new_communicator(this_code->id, MDI_TCP);
-  communicator* new_comm = get_communicator(this_code->id, comm_id);
+  MDI_Comm comm_id;
+  ret = new_communicator(this_code->id, MDI_TCP, &comm_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_request_connection: new_communicator failed");
+    return 1;
+  }
+  communicator* new_comm;
+  ret = get_communicator(this_code->id, comm_id, &new_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_request_connection: get_communicator failed");
+    return ret;
+  }
   new_comm->sockfd = sockfd;
   new_comm->send = tcp_send;
   new_comm->recv = tcp_recv;
 
 
   // communicate the version number between codes
   // only do this if not in i-PI compatibility mode
-  if ( ipi_compatibility != 1 ) {
+  if ( this_code->ipi_compatibility != 1 ) {
     int version[3];
     int length_send[2];
     int length_recv[2];
     version[0] = MDI_MAJOR_VERSION;
     version[1] = MDI_MINOR_VERSION;
     version[2] = MDI_PATCH_VERSION;
     tcp_send(&version[0], 3, MDI_INT, new_comm->id, 0);
@@ -358,33 +408,50 @@
 }
 
 
 /*! \brief Accept a TCP connection request
  */
 int tcp_accept_connection() {
   sock_t connection;
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_accept_connection: get_current_code failed");
+    return 1;
+  }
 
   if ( this_code->intra_rank == 0 ) { // Running on rank 0
 
-    connection = accept(tcp_socket, NULL, NULL);
+    connection = accept(this_code->tcp_socket, NULL, NULL);
     if (connection < 0) {
       mdi_error("Could not accept connection");
       return 1;
     }
 
-    MDI_Comm comm_id = new_communicator(this_code->id, MDI_TCP);
-    communicator* new_comm = get_communicator(this_code->id, comm_id);
+    MDI_Comm comm_id;
+    ret = new_communicator(this_code->id, MDI_TCP, &comm_id);
+    if ( ret != 0 ) {
+      mdi_error("Error in tcp_accept_connection: new_communicator failed");
+      return 1;
+    }
+    communicator* new_comm;
+    ret = get_communicator(this_code->id, comm_id, &new_comm);
+    if ( ret != 0 ) {
+      mdi_error("Error in tcp_accept_connection: get_communicator failed");
+      return ret;
+    }
     new_comm->sockfd = connection;
     new_comm->send = tcp_send;
     new_comm->recv = tcp_recv;
 
     // communicate the version number between codes
     // only do this if not in i-PI compatibility mode
-    if ( ipi_compatibility != 1 ) {
+    if ( this_code->ipi_compatibility != 1 ) {
       int version[3];
       int length_send[2];
       int length_recv[2];
       version[0] = MDI_MAJOR_VERSION;
       version[1] = MDI_MINOR_VERSION;
       version[2] = MDI_PATCH_VERSION;
       tcp_send(&version[0], 3, MDI_INT, new_comm->id, 0);
@@ -400,16 +467,26 @@
       }
     }
 
   }
   else { // Not running on rank 0
 
     // Simply create a dummy communicator
-    MDI_Comm comm_id = new_communicator(this_code->id, MDI_TCP);
-    communicator* new_comm = get_communicator(this_code->id, comm_id);
+    MDI_Comm comm_id;
+    ret = new_communicator(this_code->id, MDI_TCP, &comm_id);
+    if ( ret != 0 ) {
+      mdi_error("Error in dummy tcp_accept_connection: new_communicator failed");
+      return 1;
+    }
+    communicator* new_comm;
+    ret = get_communicator(this_code->id, comm_id, &new_comm);
+    if ( ret != 0 ) {
+      mdi_error("Error in tcp_accept_connection: second get_communicator failed");
+      return ret;
+    }
     new_comm->sockfd = connection;
     new_comm->send = tcp_send;
     new_comm->recv = tcp_recv;
 
   }
 
   return 0;
@@ -431,22 +508,32 @@
  *                   Type of role this data has within a message.
  *                   0: Not part of a message.
  *                   1: The header of a message.
  *                   2: The body (data) of a message.
  */
 int tcp_send(const void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag) {
   int ret;
-  
+
   // only send from rank 0
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_send: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
-  communicator* this = get_communicator(current_code, comm);
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_send: get_communicator failed");
+    return ret;
+  }
   size_t count_t = count;
 #ifdef _WIN32
   int n = 0;
 #else
   ssize_t n = 0;
 #endif
 
@@ -492,25 +579,35 @@
  *                   1: The header of a message.
  *                   2: The body (data) of a message.
  */
 int tcp_recv(void* buf, int count, MDI_Datatype datatype, MDI_Comm comm, int msg_flag) {
   int ret;
   
   // only recv from rank 0
-  code* this_code = get_code(current_code);
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_recv: get_current_code failed");
+    return 1;
+  }
   if ( this_code->intra_rank != 0 ) {
     return 0;
   }
 
 #ifdef _WIN32
   int n, nr;
 #else
   ssize_t n, nr;
 #endif
-  communicator* this = get_communicator(current_code, comm);
+  communicator* this;
+  ret = get_communicator(codes.current_key, comm, &this);
+  if ( ret != 0 ) {
+    mdi_error("Error in tcp_recv: get_communicator failed");
+    return ret;
+  }
   size_t count_t = count;
 
   // determine the byte size of the data type being sent
   size_t datasize;
   MDI_Datatype basetype;
   ret = datatype_info(datatype, &datasize, &basetype);
   if ( ret != 0 ) { return ret; }
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_test.c` & `pymdi-1.4.9/MDI_Library/mdi_test.c`

 * *Files 26% similar despite different names*

```diff
@@ -10,48 +10,81 @@
 #include "mdi.h"
 #include "mdi_test.h"
 #include "mdi_global.h"
 
 
 /*! \brief Enable support for the TEST method */
 int enable_test_support(int code_id) {
-  new_method(code_id, MDI_TEST);
-  method* this_method = get_method(code_id, MDI_TEST);
+  int ret;
+  int method_id;
+  ret = new_method(code_id, MDI_TEST, &method_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_test_support: new_method failed");
+    return ret;
+  }
+  method* this_method;
+  ret = get_method(code_id, MDI_TEST, &this_method);
+  if ( ret != 0 ) {
+    mdi_error("Error in enable_test_support: get_method failed");
+    return ret;
+  }
   this_method->on_selection = test_on_selection;
   this_method->on_accept_communicator = test_on_accept_communicator;
   this_method->on_send_command = test_on_send_command;
   this_method->after_send_command = test_after_send_command;
   this_method->on_recv_command = test_on_recv_command;
   return 0;
 }
 
 
 
 /*! \brief Callback when the end-user selects TCP as the method */
 int test_on_selection() {
-  if ( is_initialized == 1 ) {
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in test_on_selection: get_current_code failed");
+    return 1;
+  }
+
+  if ( this_code->test_initialized == 1 ) {
     mdi_error("MDI_Init called after MDI was already initialized");
     return 1;
   }
+  this_code->test_initialized = 1;
 
   test_initialize();
 
   return 0;
 }
 
 
 
 /*! \brief Callback when the TEST method must accept a communicator */
 int test_on_accept_communicator() {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in test_on_accept_communicator: get_current_code failed");
+    return 1;
+  }
 
   // If MDI hasn't returned some connections, do that now
   if ( this_code->returned_comms < this_code->next_comm - 1 ) {
     this_code->returned_comms++;
-    communicator* comm_obj = get_communicator(current_code, this_code->returned_comms);
+    communicator* comm_obj;
+    ret = get_communicator(codes.current_key, this_code->returned_comms, &comm_obj);
+    if ( ret != 0 ) {
+      mdi_error("Error in test_on_accept_communicator: get_communicator failed");
+      return ret;
+    }
     comm_obj->is_accepted = 1;
     return this_code->returned_comms;
   }
 
   // unable to accept any connections
   return MDI_COMM_NULL;
 }
@@ -65,15 +98,15 @@
 
 
 
 /*! \brief Callback after the TEST method has received a command */
 int test_after_send_command(const char* command, MDI_Comm comm) {
   // if the command was "EXIT", delete this communicator
   if ( strcmp( command, "EXIT" ) == 0 ) {
-    delete_communicator(current_code, comm);
+    delete_communicator(codes.current_key, comm);
   }
   
   return 0;
 }
 
 
 
@@ -84,18 +117,35 @@
 
 
 
 /*! \brief Perform initialization of a dummy communicator for testing purposes
  *
  */
 int test_initialize() {
-  code* this_code = get_code(current_code);
+  int ret;
+
+  code* this_code;
+  ret = get_current_code(&this_code);
+  if ( ret != 0 ) {
+    mdi_error("Error in test_initialize: get_current_code failed");
+    return 1;
+  }
 
-  MDI_Comm comm_id = new_communicator(this_code->id, MDI_TEST);
-  communicator* new_comm = get_communicator(this_code->id, comm_id);
+  MDI_Comm comm_id;
+  ret = new_communicator(this_code->id, MDI_TEST, &comm_id);
+  if ( ret != 0 ) {
+    mdi_error("Error in test_initialize: new_communicator failed");
+    return 1;
+  }
+  communicator* new_comm;
+  ret = get_communicator(this_code->id, comm_id, &new_comm);
+  if ( ret != 0 ) {
+    mdi_error("Error in test_initialize: get_communicator failed");
+    return ret;
+  }
   new_comm->send = test_send;
   new_comm->recv = test_recv;
 
   return 0;
 }
 
 /*! \brief Dummy function to handle sending data through an MDI connection, for testing purposes
```

### Comparing `pymdi-1.4.8/MDI_Library/mdi_test.h` & `pymdi-1.4.9/MDI_Library/mdi_test.h`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/MDI_Library/physconst.h` & `pymdi-1.4.9/MDI_Library/physconst.h`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/README.md` & `pymdi-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/cmake/mdiConfig.cmake.in` & `pymdi-1.4.9/cmake/mdiConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/pymdi.egg-info/SOURCES.txt` & `pymdi-1.4.9/pymdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymdi-1.4.8/setup.py` & `pymdi-1.4.9/setup.py`

 * *Files identical despite different names*

