# Comparing `tmp/hogql_parser-1.0.6.tar.gz` & `tmp/hogql_parser-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hogql_parser-1.0.6.tar", last modified: Thu Mar 28 15:04:54 2024, max compression
+gzip compressed data, was "hogql_parser-1.0.7.tar", last modified: Fri Apr  5 10:50:56 2024, max compression
```

## Comparing `hogql_parser-1.0.6.tar` & `hogql_parser-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:04:54.654211 hogql_parser-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    73182 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/HogQLLexer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   319116 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/HogQLParser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/HogQLParserBaseVisitor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/HogQLParserVisitor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-28 15:04:54.654211 hogql_parser-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/error.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:04:54.654211 hogql_parser-1.0.6/hogql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-28 15:04:53.000000 hogql_parser-1.0.6/hogql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 15:04:54.000000 hogql_parser-1.0.6/hogql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:04:53.000000 hogql_parser-1.0.6/hogql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 15:04:53.000000 hogql_parser-1.0.6/hogql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    81004 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:04:54.654211 hogql_parser-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-28 15:04:41.000000 hogql_parser-1.0.6/string.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    73182 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLLexer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   319116 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLParserBaseVisitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/HogQLParserVisitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/error.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/hogql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 10:50:56.000000 hogql_parser-1.0.7/hogql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    80472 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:50:56.811019 hogql_parser-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-05 10:50:54.000000 hogql_parser-1.0.7/string.cpp
```

### Comparing `hogql_parser-1.0.6/HogQLLexer.cpp` & `hogql_parser-1.0.7/HogQLLexer.cpp`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.6/HogQLParser.cpp` & `hogql_parser-1.0.7/HogQLParser.cpp`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.6/PKG-INFO` & `hogql_parser-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hogql_parser
-Version: 1.0.6
+Version: 1.0.7
 Summary: HogQL parser for internal PostHog use
 Home-page: https://github.com/PostHog/posthog/tree/master/hogql_parser
 Author: PostHog Inc.
 Author-email: hey@posthog.com
 Maintainer: PostHog Inc.
 Maintainer-email: hey@posthog.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hogql_parser-1.0.6/error.cpp` & `hogql_parser-1.0.7/error.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #include "error.h"
 
 using namespace std;
 
-#define EXCEPTION_CLASS_IMPLEMENTATION(NAME, BASE)                                                       \
+#define ERROR_CLASS_IMPLEMENTATION(NAME, BASE)                                                           \
   NAME::NAME(const string& message, size_t start, size_t end) : BASE(message), start(start), end(end) {} \
   NAME::NAME(const char* message, size_t start, size_t end) : BASE(message), start(start), end(end) {}   \
   NAME::NAME(const string& message) : BASE(message), start(0), end(0) {}                                 \
   NAME::NAME(const char* message) : BASE(message), start(0), end(0) {}
 
-EXCEPTION_CLASS_IMPLEMENTATION(HogQLException, runtime_error)
+ERROR_CLASS_IMPLEMENTATION(HogQLError, runtime_error)
 
-EXCEPTION_CLASS_IMPLEMENTATION(SyntaxException, HogQLException)
-EXCEPTION_CLASS_IMPLEMENTATION(NotImplementedException, HogQLException)
-EXCEPTION_CLASS_IMPLEMENTATION(ParsingException, HogQLException)
+ERROR_CLASS_IMPLEMENTATION(SyntaxError, HogQLError)
+ERROR_CLASS_IMPLEMENTATION(NotImplementedError, HogQLError)
+ERROR_CLASS_IMPLEMENTATION(ParsingError, HogQLError)
 
-PyInternalException::PyInternalException() : exception() {}
+PyInternalError::PyInternalError() : exception() {}
```

### Comparing `hogql_parser-1.0.6/hogql_parser.egg-info/PKG-INFO` & `hogql_parser-1.0.7/hogql_parser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hogql-parser
-Version: 1.0.6
+Version: 1.0.7
 Summary: HogQL parser for internal PostHog use
 Home-page: https://github.com/PostHog/posthog/tree/master/hogql_parser
 Author: PostHog Inc.
 Author-email: hey@posthog.com
 Maintainer: PostHog Inc.
 Maintainer-email: hey@posthog.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hogql_parser-1.0.6/parser.cpp` & `hogql_parser-1.0.7/parser.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 #include "error.h"
 #include "parser.h"
 #include "string.h"
 
 #define VISIT(RULE) any visit##RULE(HogQLParser::RULE##Context* ctx) override
 #define VISIT_UNSUPPORTED(RULE)                                \
   VISIT(RULE) {                                                \
-    throw NotImplementedException("Unsupported rule: " #RULE); \
+    throw NotImplementedError("Unsupported rule: " #RULE); \
   }
 
-#define HANDLE_HOGQL_EXCEPTION(TYPE, OTHER_CLEANUP)                                                     \
+#define HANDLE_HOGQL_ERROR(TYPE, OTHER_CLEANUP)                                                     \
   (const TYPE& e) {                                                                                     \
     string err_what = e.what();                                                                         \
     PyObject *error_type = NULL, *py_err_args = NULL, *py_err = NULL, *py_start = NULL, *py_end = NULL; \
     int err_indicator = 0;                                                                              \
     error_type = PyObject_GetAttrString(state->errors_module, #TYPE);                                   \
     if (!error_type) goto exit##TYPE;                                                                   \
     py_err_args = Py_BuildValue("(s#)", err_what.data(), err_what.size());                              \
@@ -46,15 +46,15 @@
     return NULL;                                                                                        \
   }
 
 #define RETURN_NEW_AST_NODE(TYPE_NAME, KWARGS_FORMAT, ...)                                                    \
   PyObject* ret = build_ast_node(TYPE_NAME, KWARGS_FORMAT, __VA_ARGS__);                                      \
   /* Fortunately we don't need to care about decrementing Py_BuildValue/Py_VaBuildValue args, */              \
   /* so just throw is enough: https://github.com/python/cpython/blob/a254120f/Python/modsupport.c#L147-L148*/ \
-  if (!ret) throw PyInternalException();                                                                      \
+  if (!ret) throw PyInternalError();                                                                      \
   return ret
 
 using namespace std;
 
 // PYTHON UTILS (`X_` stands for "extension")
 
 // Extend `list` with `extension` in-place. Return 0 on success, -1 on error.
@@ -162,37 +162,37 @@
     auto token = dynamic_cast<antlr4::Token*>(tree);
     if (token) {
       start = token->getStartIndex();
       stop = token->getStopIndex();
     } else {
       auto ctx = dynamic_cast<antlr4::ParserRuleContext*>(tree);
       if (!ctx) {
-        throw ParsingException("Parse tree node is neither a Token nor a ParserRuleContext");
+        throw ParsingError("Parse tree node is neither a Token nor a ParserRuleContext");
       }
       start = ctx->getStart()->getStartIndex();
       stop = ctx->getStop()->getStopIndex();
     }
     // Visit the parse tree node (while making sure that nodes/errors have spans - except for internal expressions)
     any node;
     try {
       node = tree->accept(this);
-    } catch (const SyntaxException& e) {
+    } catch (const SyntaxError& e) {
       // If start and end are unset, rethrow with the current start and stop
       if (!is_internal && e.start == 0 && e.end == 0) {
-        throw SyntaxException(e.what(), start, stop + 1);
+        throw SyntaxError(e.what(), start, stop + 1);
       }
       throw;
     }
     if (!is_internal && node.has_value() && node.type() == typeid(PyObject*)) {
       PyObject* py_node = any_cast<PyObject*>(node);
       if (py_node) {
         int is_ast = is_ast_node_instance(py_node);
         if (is_ast == -1) {
           Py_DECREF(py_node);
-          throw PyInternalException();
+          throw PyInternalError();
         }
         if (is_ast) {
           PyObject *py_start = NULL, *py_end = NULL;
           int err_indicator = 0;
           py_start = PyLong_FromSize_t(start);
           if (!py_start) goto error;
           py_end = PyLong_FromSize_t(stop + 1);
@@ -202,47 +202,47 @@
           err_indicator = PyObject_SetAttrString(py_node, "end", py_end);
           if (err_indicator == -1) goto error;
           goto success;
         error:
           Py_XDECREF(py_start);
           Py_XDECREF(py_end);
           Py_DECREF(py_node);
-          throw PyInternalException();
+          throw PyInternalError();
         success:
           Py_XDECREF(py_start);
           Py_XDECREF(py_end);
         }
       }
     }
     return node;
   }
 
   // This is the only method that should actually be called from outside the class.
   // Convert the parse tree to an AST node result. If an error has occurred in conversion, handle it gracefully.
   PyObject* visitAsPyObjectFinal(antlr4::tree::ParseTree* tree) {
     try {
       return visitAsPyObject(tree);
-    } catch HANDLE_HOGQL_EXCEPTION(SyntaxException, ) catch HANDLE_HOGQL_EXCEPTION(
-        NotImplementedException,
-    ) catch HANDLE_HOGQL_EXCEPTION(ParsingException, ) catch (const PyInternalException& e) {
+    } catch HANDLE_HOGQL_ERROR(SyntaxError, ) catch HANDLE_HOGQL_ERROR(
+        NotImplementedError,
+    ) catch HANDLE_HOGQL_ERROR(ParsingError, ) catch (const PyInternalError& e) {
       return NULL;
     } catch (const bad_any_cast& e) {
-      PyObject* error_type = PyObject_GetAttrString(state->errors_module, "ParsingException");
+      PyObject* error_type = PyObject_GetAttrString(state->errors_module, "ParsingError");
       if (error_type) {
         PyErr_SetString(error_type, "Parsing failed due to bad type casting");
       }
       return NULL;
     }
   }
 
   PyObject* visitAsPyObject(antlr4::tree::ParseTree* tree) {
     PyObject* ret = any_cast<PyObject*>(visit(tree));
     if (!ret) {
-      throw ParsingException(
-          "Rule resulted in a null PyObject pointer. A PyInternalException should have been raised instead."
+      throw ParsingError(
+          "Rule resulted in a null PyObject pointer. A PyInternalError should have been raised instead."
       );
     }
     return ret;
   }
 
   PyObject* visitAsPyObjectOrNone(antlr4::tree::ParseTree* tree) {
     if (tree == NULL) {
@@ -250,27 +250,27 @@
     }
     return visitAsPyObject(tree);
   }
 
   PyObject* visitAsPyObjectOrEmptyList(antlr4::tree::ParseTree* tree) {
     if (tree == NULL) {
       PyObject* list = PyList_New(0);
-      if (!list) throw PyInternalException();
+      if (!list) throw PyInternalError();
       return list;
     }
     return visitAsPyObject(tree);
   }
 
   // T has to be used in place of antlr4::tree::ParseTree* here, because there's no conversion from the child class
   // to its parent within vectors
   template <typename T>
   PyObject* visitPyListOfObjects(vector<T> tree) {
     PyObject* ret = PyList_New(tree.size());
     if (!ret) {
-      throw PyInternalException();
+      throw PyInternalError();
     }
     for (size_t i = 0; i < tree.size(); i++) {
       try {
         PyList_SET_ITEM(ret, i, visitAsPyObject(tree[i]));
       } catch (...) {
         Py_DECREF(ret);
         throw;
@@ -311,15 +311,15 @@
       return visit(select_stmt_ctx);
     }
 
     auto placeholder_ctx = ctx->placeholder();
     if (placeholder_ctx) {
       return visitAsPyObject(placeholder_ctx);
     }
-    
+
     return visit(ctx->selectUnionStmt());
   }
 
   VISIT(SelectUnionStmt) {
     // Using a vector of PyObjects atypically here, because this is a precursor of flattened_queries
     vector<PyObject*> select_queries;
     auto select_stmt_with_parens_ctxs = ctx->selectStmtWithParens();
@@ -331,15 +331,15 @@
         X_Py_DECREF_ALL(select_queries);
         throw;
       }
     }
     PyObject* flattened_queries = PyList_New(0);
     if (!flattened_queries) {
       X_Py_DECREF_ALL(select_queries);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     for (auto query : select_queries) {
       int is_select_query = is_ast_node_instance(query, "SelectQuery");
       if (is_select_query == -1) goto select_queries_loop_py_error;
       if (is_ast_node_instance(query, "SelectQuery")) {
         int append_code = PyList_Append(flattened_queries, query);
         if (append_code == -1) goto select_queries_loop_py_error;
@@ -352,28 +352,28 @@
         Py_DECREF(sub_select_queries);
       } else if (is_ast_node_instance(query, "Placeholder")) {
         int append_code = PyList_Append(flattened_queries, query);
         if (append_code == -1) goto select_queries_loop_py_error;
       } else {
         Py_DECREF(flattened_queries);
         X_Py_DECREF_ALL(select_queries);
-        throw ParsingException("Unexpected query node type: " + string(Py_TYPE(query)->tp_name));
+        throw ParsingError("Unexpected query node type: " + string(Py_TYPE(query)->tp_name));
       }
     }
     goto select_queries_loop_success;
   select_queries_loop_py_error:
     X_Py_DECREF_ALL(select_queries);
     Py_DECREF(flattened_queries);
-    throw PyInternalException();
+    throw PyInternalError();
   select_queries_loop_success:
     X_Py_DECREF_ALL(select_queries);
     Py_ssize_t flattened_queries_size = PyList_Size(flattened_queries);
     if (flattened_queries_size == -1) {
       Py_DECREF(flattened_queries);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     if (flattened_queries_size == 1) {
       PyObject* query = PyList_GET_ITEM(flattened_queries, 0);
       Py_INCREF(query);
       Py_DECREF(flattened_queries);
       return query;
     }
@@ -408,31 +408,31 @@
 
     PyObject* select_query = build_ast_node(
         "SelectQuery", "{s:N,s:N,s:N,s:N,s:N,s:N,s:N,s:N,s:N}", "ctes", ctes, "select", select, "distinct",
         Py_NewRef(ctx->DISTINCT() ? Py_True : Py_None), "select_from", select_from, "where", where, "prewhere",
         prewhere, "having", having, "group_by", group_by, "order_by", order_by
     );
     if (!select_query) {
-      throw PyInternalException();
+      throw PyInternalError();
     }
 
     int err_indicator = 0;
 
     auto window_clause_ctx = ctx->windowClause();
     if (window_clause_ctx) {
       auto window_expr_ctxs = window_clause_ctx->windowExpr();
       auto identifier_ctxs = window_clause_ctx->identifier();
       if (window_expr_ctxs.size() != identifier_ctxs.size()) {
         Py_DECREF(select_query);
-        throw ParsingException("WindowClause must have a matching number of window exprs and identifiers");
+        throw ParsingError("WindowClause must have a matching number of window exprs and identifiers");
       }
       PyObject* window_exprs = PyDict_New();
       if (!window_exprs) {
         Py_DECREF(select_query);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       for (size_t i = 0; i < window_expr_ctxs.size(); i++) {
         string identifier;
         PyObject* window_expr;
         try {
           identifier = visitAsString(identifier_ctxs[i]);
           window_expr = visitAsPyObject(window_expr_ctxs[i]);
@@ -442,22 +442,22 @@
           throw;
         }
         err_indicator = PyDict_SetItemString(window_exprs, identifier.c_str(), window_expr);
         Py_DECREF(window_expr);
         if (err_indicator == -1) {
           Py_DECREF(window_exprs);
           Py_DECREF(select_query);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       }
       err_indicator = PyObject_SetAttrString(select_query, "window_exprs", window_exprs);
       Py_DECREF(window_exprs);
       if (err_indicator == -1) {
         Py_DECREF(select_query);
-        throw PyInternalException();
+        throw PyInternalError();
       }
     }
 
     auto limit_and_offset_clause_ctx = ctx->limitAndOffsetClause();
     if (limit_and_offset_clause_ctx) {
       PyObject* limit;
       try {
@@ -466,30 +466,30 @@
         Py_DECREF(select_query);
         throw;
       }
       err_indicator = PyObject_SetAttrString(select_query, "limit", limit);
       Py_DECREF(limit);
       if (err_indicator == -1) {
         Py_DECREF(select_query);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       auto offset_ctx = limit_and_offset_clause_ctx->columnExpr(1);
       if (offset_ctx) {
         PyObject* offset;
         try {
           offset = visitAsPyObject(offset_ctx);
         } catch (...) {
           Py_DECREF(select_query);
           throw;
         }
         err_indicator = PyObject_SetAttrString(select_query, "offset", offset);
         Py_DECREF(offset);
         if (err_indicator == -1) {
           Py_DECREF(select_query);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       }
       auto limit_by_exprs_ctx = limit_and_offset_clause_ctx->columnExprList();
       if (limit_by_exprs_ctx) {
         PyObject* limit_by_exprs;
         try {
           limit_by_exprs = visitAsPyObject(limit_by_exprs_ctx);
@@ -497,22 +497,22 @@
           Py_DECREF(select_query);
           throw;
         }
         err_indicator = PyObject_SetAttrString(select_query, "limit_by", limit_by_exprs);
         Py_DECREF(limit_by_exprs);
         if (err_indicator == -1) {
           Py_DECREF(select_query);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       }
       if (limit_and_offset_clause_ctx->WITH() && limit_and_offset_clause_ctx->TIES()) {
         err_indicator = PyObject_SetAttrString(select_query, "limit_with_ties", Py_True);
         if (err_indicator == -1) {
           Py_DECREF(select_query);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       }
     } else {
       auto offset_only_clause_ctx = ctx->offsetOnlyClause();
       if (offset_only_clause_ctx) {
         PyObject* offset_only_clause;
         try {
@@ -521,88 +521,88 @@
           Py_DECREF(select_query);
           throw;
         }
         err_indicator = PyObject_SetAttrString(select_query, "offset", offset_only_clause);
         Py_DECREF(offset_only_clause);
         if (err_indicator == -1) {
           Py_DECREF(select_query);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       }
     }
 
     auto array_join_clause_ctx = ctx->arrayJoinClause();
     if (array_join_clause_ctx) {
       if (Py_IsNone(select_from)) {
         Py_DECREF(select_query);
-        throw SyntaxException("Using ARRAY JOIN without a FROM clause is not permitted");
+        throw SyntaxError("Using ARRAY JOIN without a FROM clause is not permitted");
       }
       PyObject* join_op = PyUnicode_FromString(
           array_join_clause_ctx->LEFT()    ? "LEFT ARRAY JOIN"
           : array_join_clause_ctx->INNER() ? "INNER ARRAY JOIN"
                                            : "ARRAY JOIN"
       );
       if (!join_op) {
         Py_DECREF(select_query);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       err_indicator = PyObject_SetAttrString(select_query, "array_join_op", join_op);
       Py_DECREF(join_op);
       if (err_indicator == -1) {
         Py_DECREF(select_query);
-        throw PyInternalException();
+        throw PyInternalError();
       }
 
       auto array_join_arrays_ctx = array_join_clause_ctx->columnExprList();
       PyObject* array_join_list;
       try {
         array_join_list = visitAsPyObject(array_join_arrays_ctx);
       } catch (...) {
         Py_DECREF(select_query);
         throw;
       }
       Py_ssize_t array_join_list_size = PyList_Size(array_join_list);
       if (array_join_list_size == -1) {
         Py_DECREF(select_query);
         Py_DECREF(array_join_list);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       for (Py_ssize_t i = 0; i < array_join_list_size; i++) {
         PyObject* expr = PyList_GET_ITEM(array_join_list, i);
         int is_alias = is_ast_node_instance(expr, "Alias");
         if (is_alias == -1) {
           Py_DECREF(array_join_list);
           Py_DECREF(select_query);
-          throw PyInternalException();
+          throw PyInternalError();
         }
         if (!is_alias) {
           Py_DECREF(array_join_list);
           Py_DECREF(select_query);
           auto relevant_column_expr_ctx = array_join_arrays_ctx->columnExpr(i);
-          throw SyntaxException(
+          throw SyntaxError(
               "ARRAY JOIN arrays must have an alias", relevant_column_expr_ctx->getStart()->getStartIndex(),
               relevant_column_expr_ctx->getStop()->getStopIndex() + 1
           );
         }
       }
       err_indicator = PyObject_SetAttrString(select_query, "array_join_list", array_join_list);
       Py_DECREF(array_join_list);
       if (err_indicator == -1) {
         Py_DECREF(select_query);
-        throw PyInternalException();
+        throw PyInternalError();
       }
     }
 
     if (ctx->topClause()) {
       Py_DECREF(select_query);
-      throw NotImplementedException("Unsupported: SelectStmt.topClause()");
+      throw NotImplementedError("Unsupported: SelectStmt.topClause()");
     }
     if (ctx->settingsClause()) {
       Py_DECREF(select_query);
-      throw NotImplementedException("Unsupported: SelectStmt.settingsClause()");
+      throw NotImplementedError("Unsupported: SelectStmt.settingsClause()");
     }
 
     return select_query;
   }
 
   VISIT(WithClause) { return visit(ctx->withExprList()); }
 
@@ -635,79 +635,79 @@
   PyObject* next_join =                                                                                          \
       PyObject_GetAttrString(last_join, "next_join"); /* 1500 is Python's recursion limit (C_RECURSION_LIMIT) */ \
   for (size_t i = 0; i < 1500; i++) { /* We can safely decref, because a reference is anyway held by join1 */    \
     Py_XDECREF(next_join);                                                                                       \
     if (!next_join) {                                                                                            \
       Py_DECREF(join1);                                                                                          \
       Py_DECREF(join2);                                                                                          \
-      throw PyInternalException();                                                                               \
+      throw PyInternalError();                                                                               \
     }                                                                                                            \
     int reached_end_of_chain = Py_IsNone(next_join);                                                             \
     if (reached_end_of_chain == -1) {                                                                            \
       Py_DECREF(join1);                                                                                          \
       Py_DECREF(join2);                                                                                          \
-      throw PyInternalException();                                                                               \
+      throw PyInternalError();                                                                               \
     }                                                                                                            \
     if (reached_end_of_chain) {                                                                                  \
       int err_indicator = PyObject_SetAttrString(last_join, "next_join", join2);                                 \
       if (err_indicator == -1) {                                                                                 \
         Py_DECREF(join1);                                                                                        \
         Py_DECREF(join2);                                                                                        \
-        throw PyInternalException();                                                                             \
+        throw PyInternalError();                                                                             \
       }                                                                                                          \
       Py_DECREF(join2);                                                                                          \
       return join1;                                                                                              \
     }                                                                                                            \
     last_join = next_join;                                                                                       \
     next_join = PyObject_GetAttrString(last_join, "next_join");                                                  \
   }                                                                                                              \
   Py_DECREF(join1);                                                                                              \
   Py_DECREF(join2);                                                                                              \
   PyErr_SetString(PyExc_RecursionError, "maximum recursion depth exceeded during JOIN parsing");                 \
-  throw PyInternalException(); /* This should never be reached, but `while (true)`s are scary, so better to be safe */
+  throw PyInternalError(); /* This should never be reached, but `while (true)`s are scary, so better to be safe */
 
   VISIT(JoinExprOp) {
     auto join_op_ctx = ctx->joinOp();
     PyObject* py_join_op;
     if (join_op_ctx) {
       string join_op = visitAsString(join_op_ctx);
       join_op.append(" JOIN");
       py_join_op = PyUnicode_FromStringAndSize(join_op.data(), join_op.size());
     } else {
       py_join_op = PyUnicode_FromString("JOIN");
     }
-    if (!py_join_op) throw PyInternalException();
+    if (!py_join_op) throw PyInternalError();
 
     int err_indicator = 0;
 
     PyObject* join2;
     try {
       join2 = visitAsPyObject(ctx->joinExpr(1));
     } catch (...) {
       Py_DECREF(py_join_op);
       throw;
     }
     err_indicator = PyObject_SetAttrString(join2, "join_type", py_join_op);
     Py_DECREF(py_join_op);
     if (err_indicator == -1) {
       Py_DECREF(join2);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* constraint;
     try {
       constraint = visitAsPyObject(ctx->joinConstraintClause());
     } catch (...) {
       Py_DECREF(join2);
       throw;
     }
     err_indicator = PyObject_SetAttrString(join2, "constraint", constraint);
     Py_DECREF(constraint);
     if (err_indicator == -1) {
       Py_DECREF(join2);
-      throw PyInternalException();
+      throw PyInternalError();
     }
 
     PyObject* join1;
     try {
       join1 = visitAsPyObject(ctx->joinExpr(0));
     } catch (...) {
       Py_DECREF(join2);
@@ -718,15 +718,15 @@
   }
 
   VISIT(JoinExprTable) {
     PyObject* table = visitAsPyObject(ctx->tableExpr());
     int is_table_join_expr = is_ast_node_instance(table, "JoinExpr");
     if (is_table_join_expr == -1) {
       Py_DECREF(table);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* sample;
     try {
       sample = visitAsPyObjectOrNone(ctx->sampleClause());
     } catch (...) {
       Py_DECREF(table);
       throw;
@@ -734,53 +734,53 @@
     PyObject* table_final = ctx->FINAL() ? Py_True : Py_None;
     if (is_table_join_expr) {
       int err_indicator = 0;
       err_indicator = PyObject_SetAttrString(table, "sample", sample);
       Py_DECREF(sample);
       if (err_indicator == -1) {
         Py_DECREF(table);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       err_indicator = PyObject_SetAttrString(table, "table_final", table_final);
       if (err_indicator == -1) {
         Py_DECREF(table);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       return table;
     } else {
       PyObject* ret =
           build_ast_node("JoinExpr", "{s:N,s:O,s:N}", "table", table, "table_final", table_final, "sample", sample);
       if (!ret) {
         Py_DECREF(table);
         Py_DECREF(sample);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       return ret;
     }
   }
 
   VISIT(JoinExprParens) { return visit(ctx->joinExpr()); }
 
   VISIT(JoinExprCrossOp) {
     PyObject* join_type = PyUnicode_FromString("CROSS JOIN");
     if (!join_type) {
-      throw PyInternalException();
+      throw PyInternalError();
     }
 
     PyObject* join2;
     try {
       join2 = visitAsPyObject(ctx->joinExpr(1));
     } catch (...) {
       Py_DECREF(join_type);
       throw;
     }
     int err_indicator = PyObject_SetAttrString(join2, "join_type", join_type);
     if (err_indicator == -1) {
       Py_DECREF(join2);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     Py_DECREF(join_type);
 
     PyObject* join1;
     try {
       join1 = visitAsPyObject(ctx->joinExpr(0));
     } catch (...) {
@@ -854,25 +854,25 @@
     return boost::algorithm::join(tokens, " ");
   }
 
   VISIT_UNSUPPORTED(JoinOpCross)
 
   VISIT(JoinConstraintClause) {
     if (ctx->USING()) {
-      throw NotImplementedException("Unsupported: JOIN ... USING");
+      throw NotImplementedError("Unsupported: JOIN ... USING");
     }
     PyObject* column_expr_list = visitAsPyObject(ctx->columnExprList());
     Py_ssize_t column_expr_list_size = PyList_Size(column_expr_list);
     if (column_expr_list_size == -1) {
       Py_DECREF(column_expr_list);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     if (column_expr_list_size > 1) {
       Py_DECREF(column_expr_list);
-      throw NotImplementedException("Unsupported: JOIN ... ON with multiple expressions");
+      throw NotImplementedError("Unsupported: JOIN ... ON with multiple expressions");
     }
     PyObject* expr = Py_NewRef(PyList_GET_ITEM(column_expr_list, 0));
     Py_DECREF(column_expr_list);
     RETURN_NEW_AST_NODE("JoinConstraint", "{s:N}", "expr", expr);
   }
 
   VISIT(SampleClause) {
@@ -901,17 +901,17 @@
     if (placeholder_ctx) {
       return visitAsPyObject(placeholder_ctx);
     }
 
     auto number_literal_ctxs = ctx->numberLiteral();
 
     if (number_literal_ctxs.size() > 2) {
-      throw ParsingException("RatioExpr must have at most two number literals");
+      throw ParsingError("RatioExpr must have at most two number literals");
     } else if (number_literal_ctxs.size() == 0) {
-      throw ParsingException("RatioExpr must have at least one number literal");
+      throw ParsingError("RatioExpr must have at least one number literal");
     }
 
     auto left_ctx = number_literal_ctxs[0];
     auto right_ctx = ctx->SLASH() && number_literal_ctxs.size() > 1 ? number_literal_ctxs[1] : NULL;
 
     PyObject* left = visitAsPyObject(left_ctx);
     PyObject* right;
@@ -931,37 +931,37 @@
 
   VISIT(WindowExpr) {
     auto frame_ctx = ctx->winFrameClause();
     PyObject* frame = visitAsPyObjectOrNone(frame_ctx);
     int is_frame_a_tuple = PyTuple_Check(frame);
     if (is_frame_a_tuple == -1) {
       Py_DECREF(frame);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     if (is_frame_a_tuple) {
       Py_ssize_t frame_tuple_size = PyTuple_Size(frame);
       if (frame_tuple_size == -1) {
         Py_DECREF(frame);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       if (frame_tuple_size != 2) {
         Py_DECREF(frame);
-        throw ParsingException("WindowExpr frame must be a tuple of size 2");
+        throw ParsingError("WindowExpr frame must be a tuple of size 2");
       }
     }
     PyObject* frame_start = Py_NewRef(is_frame_a_tuple ? PyTuple_GET_ITEM(frame, 0) : frame);
     PyObject* frame_end = Py_NewRef(is_frame_a_tuple ? PyTuple_GET_ITEM(frame, 1) : Py_None);
     Py_DECREF(frame);
     PyObject* frame_method = frame_ctx && frame_ctx->RANGE()  ? PyUnicode_FromString("RANGE")
                              : frame_ctx && frame_ctx->ROWS() ? PyUnicode_FromString("ROWS")
                                                               : Py_NewRef(Py_None);
     if (!frame_method) {
       Py_DECREF(frame_start);
       Py_DECREF(frame_end);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* partition_by;
     try {
       partition_by = visitAsPyObjectOrNone(ctx->winPartitionByClause());
     } catch (...) {
       Py_DECREF(frame_start);
       Py_DECREF(frame_end);
@@ -1009,15 +1009,15 @@
   VISIT(WinFrameBound) {
     if (ctx->PRECEDING() || ctx->FOLLOWING()) {
       PyObject* number;
       if (ctx->numberLiteral()) {
         PyObject* constant = visitAsPyObject(ctx->numberLiteral());
         number = PyObject_GetAttrString(constant, "value");
         Py_DECREF(constant);
-        if (!number) throw PyInternalException();
+        if (!number) throw PyInternalError();
       } else {
         number = Py_NewRef(Py_None);
       }
       RETURN_NEW_AST_NODE(
           "WindowFrameExpr", "{s:s,s:N}", "frame_type", ctx->PRECEDING() ? "PRECEDING" : "FOLLOWING", "frame_value",
           number
       );
@@ -1065,34 +1065,34 @@
     if (ctx->alias()) {
       alias = visitAsString(ctx->alias());
     } else if (ctx->identifier()) {
       alias = visitAsString(ctx->identifier());
     } else if (ctx->STRING_LITERAL()) {
       alias = unquote_string_terminal(ctx->STRING_LITERAL());
     } else {
-      throw ParsingException("A ColumnExprAlias must have the alias in some form");
+      throw ParsingError("A ColumnExprAlias must have the alias in some form");
     }
     PyObject* expr = visitAsPyObject(ctx->columnExpr());
 
     if (find(RESERVED_KEYWORDS.begin(), RESERVED_KEYWORDS.end(), boost::algorithm::to_lower_copy(alias)) !=
         RESERVED_KEYWORDS.end()) {
       Py_DECREF(expr);
-      throw SyntaxException("\"" + alias + "\" cannot be an alias or identifier, as it's a reserved keyword");
+      throw SyntaxError("\"" + alias + "\" cannot be an alias or identifier, as it's a reserved keyword");
     }
 
     RETURN_NEW_AST_NODE("Alias", "{s:N,s:s#}", "expr", expr, "alias", alias.data(), alias.size());
   }
 
   VISIT(ColumnExprNegate) {
     PyObject* left = build_ast_node("Constant", "{s:i}", "value", 0);
-    if (!left) throw PyInternalException();
+    if (!left) throw PyInternalError();
     PyObject* op = get_ast_enum_member("ArithmeticOperationOp", "Sub");
     if (!op) {
       Py_DECREF(left);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* right;
     try {
       right = visitAsPyObject(ctx->columnExpr());
     } catch (...) {
       Py_DECREF(op);
       Py_DECREF(left);
@@ -1117,17 +1117,17 @@
     if (ctx->SLASH()) {
       op = get_ast_enum_member("ArithmeticOperationOp", "Div");
     } else if (ctx->ASTERISK()) {
       op = get_ast_enum_member("ArithmeticOperationOp", "Mult");
     } else if (ctx->PERCENT()) {
       op = get_ast_enum_member("ArithmeticOperationOp", "Mod");
     } else {
-      throw ParsingException("Unsupported value of rule ColumnExprPrecedence1");
+      throw ParsingError("Unsupported value of rule ColumnExprPrecedence1");
     }
-    if (!op) throw PyInternalException();
+    if (!op) throw PyInternalError();
     PyObject* left;
     try {
       left = visitAsPyObject(ctx->columnExpr(0));
     } catch (...) {
       Py_DECREF(op);
       throw;
     }
@@ -1153,110 +1153,110 @@
     }
 
     if (ctx->PLUS()) {
       PyObject* op = get_ast_enum_member("ArithmeticOperationOp", "Add");
       if (!op) {
         Py_DECREF(left);
         Py_DECREF(right);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       RETURN_NEW_AST_NODE("ArithmeticOperation", "{s:N,s:N,s:N}", "left", left, "right", right, "op", op);
     } else if (ctx->DASH()) {
       PyObject* op = get_ast_enum_member("ArithmeticOperationOp", "Sub");
       if (!op) {
         Py_DECREF(left);
         Py_DECREF(right);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       RETURN_NEW_AST_NODE("ArithmeticOperation", "{s:N,s:N,s:N}", "left", left, "right", right, "op", op);
     } else if (ctx->CONCAT()) {
 #define IS_NODE_A_CONCAT_CALL(VAR) /* This is complex because of all the error handling, hence a macro */ \
   int is_##VAR##_a_concat_call = false;                                                                   \
   int is_##VAR##_a_call = is_ast_node_instance(VAR, "Call");                                              \
   if (is_##VAR##_a_call == -1) {                                                                          \
     Py_DECREF(left);                                                                                      \
     Py_DECREF(right);                                                                                     \
-    throw PyInternalException();                                                                          \
+    throw PyInternalError();                                                                          \
   }                                                                                                       \
   if (is_##VAR##_a_call) {                                                                                \
     PyObject* VAR##_name = PyObject_GetAttrString(VAR, "name");                                           \
     if (!VAR##_name) {                                                                                    \
       Py_DECREF(left);                                                                                    \
       Py_DECREF(right);                                                                                   \
       Py_DECREF(concat_as_str);                                                                           \
-      throw PyInternalException();                                                                        \
+      throw PyInternalError();                                                                        \
     }                                                                                                     \
     PyObject* VAR##_name_lower = PyObject_CallMethod(VAR##_name, "lower", NULL);                          \
     Py_DECREF(VAR##_name);                                                                                \
     if (!VAR##_name_lower) {                                                                              \
       Py_DECREF(left);                                                                                    \
       Py_DECREF(right);                                                                                   \
       Py_DECREF(concat_as_str);                                                                           \
-      throw PyInternalException();                                                                        \
+      throw PyInternalError();                                                                        \
     }                                                                                                     \
     is_##VAR##_a_concat_call = PyObject_RichCompareBool(VAR##_name_lower, concat_as_str, Py_EQ);          \
     Py_DECREF(VAR##_name_lower);                                                                          \
     if (is_##VAR##_a_concat_call == -1) {                                                                 \
       Py_DECREF(left);                                                                                    \
       Py_DECREF(right);                                                                                   \
       Py_DECREF(concat_as_str);                                                                           \
-      throw PyInternalException();                                                                        \
+      throw PyInternalError();                                                                        \
     }                                                                                                     \
   }
 
       PyObject* concat_as_str = PyUnicode_FromString("concat");
       if (!concat_as_str) {
         Py_DECREF(left);
         Py_DECREF(right);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       IS_NODE_A_CONCAT_CALL(left);
       IS_NODE_A_CONCAT_CALL(right);
       Py_DECREF(concat_as_str);
 
 #undef IS_NODE_A_CONCAT_CALL
 
       PyObject* args = is_left_a_concat_call ? PyObject_GetAttrString(left, "args") : Py_BuildValue("[O]", left);
       if (!args) {
         Py_DECREF(left);
         Py_DECREF(right);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       if (is_right_a_concat_call) {
         PyObject* right_args = PyObject_GetAttrString(right, "args");
         if (!right_args) {
           Py_DECREF(args);
           Py_DECREF(left);
           Py_DECREF(right);
-          throw PyInternalException();
+          throw PyInternalError();
         }
         int err_indicator = X_PyList_Extend(args, right_args);
         Py_DECREF(right_args);
         if (err_indicator == -1) {
           Py_DECREF(args);
           Py_DECREF(left);
           Py_DECREF(right);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       } else {
         int err_indicator = PyList_Append(args, right);
         if (err_indicator == -1) {
           Py_DECREF(args);
           Py_DECREF(left);
           Py_DECREF(right);
-          throw PyInternalException();
+          throw PyInternalError();
         }
       }
       Py_DECREF(right);
       Py_DECREF(left);
       RETURN_NEW_AST_NODE("Call", "{s:s,s:N}", "name", "concat", "args", args);
     } else {
       Py_DECREF(right);
       Py_DECREF(left);
-      throw ParsingException("Unsupported value of rule ColumnExprPrecedence2");
+      throw ParsingError("Unsupported value of rule ColumnExprPrecedence2");
     }
   }
 
   VISIT(ColumnExprPrecedence3) {
     PyObject* op = NULL;
     if (ctx->EQ_SINGLE() || ctx->EQ_DOUBLE()) {
       op = get_ast_enum_member("CompareOperationOp", "Eq");
@@ -1301,17 +1301,17 @@
         if (ctx->NOT()) {
           op = get_ast_enum_member("CompareOperationOp", "NotIn");
         } else {
           op = get_ast_enum_member("CompareOperationOp", "In");
         }
       }
     } else {
-      throw ParsingException("Unsupported value of rule ColumnExprPrecedence3");
+      throw ParsingError("Unsupported value of rule ColumnExprPrecedence3");
     }
-    if (!op) throw PyInternalException();
+    if (!op) throw PyInternalError();
 
     PyObject* left;
     try {
       left = visitAsPyObject(ctx->left);
     } catch (...) {
       Py_DECREF(op);
       throw;
@@ -1344,27 +1344,27 @@
     } else if (interval_ctx->MONTH()) {
       name = "toIntervalMonth";
     } else if (interval_ctx->QUARTER()) {
       name = "toIntervalQuarter";
     } else if (interval_ctx->YEAR()) {
       name = "toIntervalYear";
     } else {
-      throw ParsingException("Unsupported value of rule ColumnExprInterval");
+      throw ParsingError("Unsupported value of rule ColumnExprInterval");
     }
 
     RETURN_NEW_AST_NODE("Call", "{s:s,s:[N]}", "name", name, "args", visitAsPyObject(ctx->columnExpr()));
   }
 
   VISIT(ColumnExprIsNull) {
     PyObject* null_constant = build_ast_node("Constant", "{s:O}", "value", Py_None);
-    if (!null_constant) throw PyInternalException();
+    if (!null_constant) throw PyInternalError();
     PyObject* op = get_ast_enum_member("CompareOperationOp", ctx->NOT() ? "NotEq" : "Eq");
     if (!op) {
       Py_DECREF(null_constant);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* left;
     try {
       left = visitAsPyObject(ctx->columnExpr());
     } catch (...) {
       Py_DECREF(op);
       Py_DECREF(null_constant);
@@ -1378,56 +1378,56 @@
     if (ctx->LEADING()) {
       name = "trimLeft";
     } else if (ctx->TRAILING()) {
       name = "trimRight";
     } else if (ctx->BOTH()) {
       name = "trim";
     } else {
-      throw ParsingException("Unsupported value of rule ColumnExprTrim");
+      throw ParsingError("Unsupported value of rule ColumnExprTrim");
     }
     string text = unquote_string_terminal(ctx->STRING_LITERAL());
     PyObject* expr = visitAsPyObject(ctx->columnExpr());
     PyObject* value = build_ast_node("Constant", "{s:s#}", "value", text.data(), text.size());
-    if (!value) throw PyInternalException();
+    if (!value) throw PyInternalError();
     RETURN_NEW_AST_NODE("Call", "{s:s,s:[NN]}", "name", name, "args", expr, value);
   }
 
   VISIT(ColumnExprTuple) {
     RETURN_NEW_AST_NODE("Tuple", "{s:N}", "exprs", visitAsPyObjectOrEmptyList(ctx->columnExprList()));
   }
 
   VISIT(ColumnExprArrayAccess) {
     PyObject* property = visitAsPyObject(ctx->columnExpr(1));
     int is_property_a_constant = is_ast_node_instance(property, "Constant");
     if (is_property_a_constant == -1) {
       Py_DECREF(property);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     if (is_property_a_constant) {
       PyObject* property_value = PyObject_GetAttrString(property, "value");
       if (!property_value) {
         Py_DECREF(property);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       PyObject* zero = PyLong_FromLong(0);
       if (!zero) {
         Py_DECREF(property_value);
         Py_DECREF(property);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       int is_property_zero = PyObject_RichCompareBool(property_value, zero, Py_EQ);
       Py_DECREF(zero);
       Py_DECREF(property_value);
       if (is_property_zero == -1) {
         Py_DECREF(property);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       if (is_property_zero) {
         Py_DECREF(property);
-        throw SyntaxException("SQL indexes start from one, not from zero. E.g: array[1]");
+        throw SyntaxError("SQL indexes start from one, not from zero. E.g: array[1]");
       }
     }
     PyObject* object;
     try {
       object = visitAsPyObject(ctx->columnExpr(0));
     } catch (...) {
       Py_DECREF(property);
@@ -1436,15 +1436,15 @@
     RETURN_NEW_AST_NODE("ArrayAccess", "{s:N,s:N}", "array", object, "property", property);
   }
 
   VISIT(ColumnExprPropertyAccess) {
     string identifier = visitAsString(ctx->identifier());
     PyObject* property = build_ast_node("Constant", "{s:s#}", "value", identifier.data(), identifier.size());
     if (!property) {
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* object;
     try {
       object = visitAsPyObject(ctx->columnExpr());
     } catch (...) {
       Py_DECREF(property);
       throw;
@@ -1468,15 +1468,15 @@
       throw;
     }
 
     int is_left_an_and = is_ast_node_instance(left, "And");
     if (is_left_an_and == -1) {
       Py_DECREF(left);
       Py_DECREF(right);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* exprs = is_left_an_and ? PyObject_GetAttrString(left, "exprs") : Py_BuildValue("[O]", left);
 
     int is_right_an_and = is_ast_node_instance(right, "And");
     if (is_right_an_and == -1) goto right_check_error;
     if (is_right_an_and) {
       PyObject* right_exprs = PyObject_GetAttrString(right, "exprs");
@@ -1489,15 +1489,15 @@
       if (err_indicator == -1) goto right_check_error;
     }
     goto right_check_success;
   right_check_error:
     Py_DECREF(exprs);
     Py_DECREF(left);
     Py_DECREF(right);
-    throw PyInternalException();
+    throw PyInternalError();
   right_check_success:
     Py_DECREF(right);
     Py_DECREF(left);
 
     RETURN_NEW_AST_NODE("And", "{s:N}", "exprs", exprs);
   }
 
@@ -1511,15 +1511,15 @@
       throw;
     }
 
     int is_left_an_or = is_ast_node_instance(left, "Or");
     if (is_left_an_or == -1) {
       Py_DECREF(left);
       Py_DECREF(right);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     PyObject* exprs = is_left_an_or ? PyObject_GetAttrString(left, "exprs") : Py_BuildValue("[O]", left);
 
     int is_right_an_or = is_ast_node_instance(right, "Or");
     if (is_right_an_or == -1) goto right_check_error;
     if (is_right_an_or) {
       PyObject* right_exprs = PyObject_GetAttrString(right, "exprs");
@@ -1532,39 +1532,39 @@
       if (err_indicator == -1) goto right_check_error;
     }
     goto right_check_success;
   right_check_error:
     Py_DECREF(exprs);
     Py_DECREF(left);
     Py_DECREF(right);
-    throw PyInternalException();
+    throw PyInternalError();
   right_check_success:
     Py_DECREF(right);
     Py_DECREF(left);
 
     RETURN_NEW_AST_NODE("Or", "{s:N}", "exprs", exprs);
   }
 
   VISIT(ColumnExprTupleAccess) {
     PyObject* index = PyLong_FromString(ctx->DECIMAL_LITERAL()->getText().c_str(), NULL, 10);
-    if (!index) throw PyInternalException();
+    if (!index) throw PyInternalError();
     PyObject* zero = PyLong_FromLong(0);
     if (!zero) {
       Py_DECREF(index);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     int is_index_zero = PyObject_RichCompareBool(index, zero, Py_EQ);
     Py_DECREF(zero);
     if (is_index_zero == -1) {
       Py_DECREF(index);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     if (is_index_zero) {
       Py_DECREF(index);
-      throw SyntaxException("SQL indexes start from one, not from zero. E.g: array[1]");
+      throw SyntaxError("SQL indexes start from one, not from zero. E.g: array[1]");
     }
     PyObject* tuple;
     try {
       tuple = visitAsPyObject(ctx->columnExpr());
     } catch (...) {
       Py_DECREF(index);
       throw;
@@ -1604,15 +1604,15 @@
     error:
       Py_XDECREF(temp_expr_lists[1]);
       Py_XDECREF(temp_expr_lists[0]);
       Py_XDECREF(args);
       Py_XDECREF(arg_2);
       Py_XDECREF(arg_1);
       Py_XDECREF(columns);
-      throw PyInternalException();
+      throw PyInternalError();
     success:
       RETURN_NEW_AST_NODE("Call", "{s:s,s:N}", "name", "transform", "args", args);
     } else {
       RETURN_NEW_AST_NODE("Call", "{s:s,s:N}", "name", columns_size == 3 ? "if" : "multiIf", "args", columns);
     }
   }
 
@@ -1690,35 +1690,35 @@
       throw;
     }
     RETURN_NEW_AST_NODE("Lambda", "{s:N,s:N}", "args", args, "expr", expr);
   }
 
   VISIT(WithExprList) {
     PyObject* ctes = PyDict_New();
-    if (!ctes) throw PyInternalException();
+    if (!ctes) throw PyInternalError();
     for (auto with_expr_ctx : ctx->withExpr()) {
       PyObject* cte;
       try {
         cte = visitAsPyObject(with_expr_ctx);
       } catch (...) {
         Py_DECREF(ctes);
         throw;
       }
       PyObject* name = PyObject_GetAttrString(cte, "name");
       if (!name) {
         Py_DECREF(cte);
         Py_DECREF(ctes);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       int err_indicator = PyDict_SetItem(ctes, name, cte);
       if (err_indicator == -1) {
         Py_DECREF(name);
         Py_DECREF(cte);
         Py_DECREF(ctes);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       Py_DECREF(name);
       Py_DECREF(cte);
     }
     return ctes;
   }
 
@@ -1776,56 +1776,56 @@
   VISIT(TableExprPlaceholder) { return visitAsPyObject(ctx->placeholder()); }
 
   VISIT(TableExprAlias) {
     auto alias_ctx = ctx->alias();
     string alias = any_cast<string>(alias_ctx ? visit(alias_ctx) : visit(ctx->identifier()));
     if (find(RESERVED_KEYWORDS.begin(), RESERVED_KEYWORDS.end(), boost::algorithm::to_lower_copy(alias)) !=
         RESERVED_KEYWORDS.end()) {
-      throw SyntaxException("ALIAS is a reserved keyword");
+      throw SyntaxError("ALIAS is a reserved keyword");
     }
     PyObject* py_alias = PyUnicode_FromStringAndSize(alias.data(), alias.size());
-    if (!py_alias) throw PyInternalException();
+    if (!py_alias) throw PyInternalError();
     PyObject* table;
     try {
       table = visitAsPyObject(ctx->tableExpr());
     } catch (...) {
       Py_DECREF(py_alias);
       throw;
     }
 
     int is_table_a_join_expr = is_ast_node_instance(table, "JoinExpr");
     if (is_table_a_join_expr == -1) {
       Py_DECREF(py_alias);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     if (is_table_a_join_expr) {
       int err_indicator = PyObject_SetAttrString(table, "alias", py_alias);
       Py_DECREF(py_alias);
       if (err_indicator == -1) {
         Py_DECREF(table);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       return table;
     }
     RETURN_NEW_AST_NODE("JoinExpr", "{s:N,s:N}", "table", table, "alias", py_alias);
   }
 
   VISIT(TableExprFunction) { return visit(ctx->tableFunctionExpr()); }
 
   VISIT(TableExprTag) { return visit(ctx->hogqlxTagElement()); }
 
   VISIT(TableFunctionExpr) {
     string table_name = visitAsString(ctx->identifier());
     auto table_args_ctx = ctx->tableArgList();
     PyObject* table_args = table_args_ctx ? visitAsPyObject(table_args_ctx) : PyList_New(0);
-    if (!table_args) throw PyInternalException();
+    if (!table_args) throw PyInternalError();
     PyObject* table = build_ast_node("Field", "{s:[s#]}", "chain", table_name.data(), table_name.size());
     if (!table) {
       Py_DECREF(table_args);
-      throw PyInternalException();
+      throw PyInternalError();
     }
     RETURN_NEW_AST_NODE("JoinExpr", "{s:N,s:N}", "table", table, "table_args", table_args);
   }
 
   VISIT(TableIdentifier) {
     string text = visitAsString(ctx->identifier());
     auto database_identifier_ctx = ctx->databaseIdentifier();
@@ -1843,22 +1843,22 @@
 
   VISIT(NumberLiteral) {
     string text = ctx->getText();
     boost::algorithm::to_lower(text);
     if (text.find(".") != string::npos || text.find("e") != string::npos || !text.compare("-inf") ||
         !text.compare("inf") || !text.compare("nan")) {
       PyObject* py_text = PyUnicode_FromStringAndSize(text.data(), text.size());
-      if (!py_text) throw PyInternalException();
+      if (!py_text) throw PyInternalError();
       PyObject* value = PyFloat_FromString(py_text);
       Py_DECREF(py_text);
-      if (!value) throw PyInternalException();
+      if (!value) throw PyInternalError();
       RETURN_NEW_AST_NODE("Constant", "{s:N}", "value", value);
     } else {
       PyObject* value = PyLong_FromString(text.c_str(), NULL, 10);
-      if (!value) throw PyInternalException();
+      if (!value) throw PyInternalError();
       RETURN_NEW_AST_NODE("Constant", "{s:N}", "value", value);
     }
   }
 
   VISIT(Literal) {
     if (ctx->NULL_SQL()) {
       RETURN_NEW_AST_NODE("Constant", "{s:O}", "value", Py_None);
@@ -1911,20 +1911,20 @@
       );
     }
 
     auto string_literal_ctx = ctx->STRING_LITERAL();
     if (string_literal_ctx) {
       string text = unquote_string_terminal(string_literal_ctx);
       PyObject* value = build_ast_node("Constant", "{s:s#}", "value", text.data(), text.size());
-      if (!value) throw PyInternalException();
+      if (!value) throw PyInternalError();
       RETURN_NEW_AST_NODE("HogQLXAttribute", "{s:s#,s:N}", "name", name.data(), name.size(), "value", value);
     }
 
     PyObject* value = build_ast_node("Constant", "{s:O}", "value", Py_True);
-    if (!value) throw PyInternalException();
+    if (!value) throw PyInternalError();
     RETURN_NEW_AST_NODE("HogQLXAttribute", "{s:s#,s:N}", "name", name.data(), name.size(), "value", value);
   }
 
   VISIT(HogqlxTagElementClosed) {
     string kind = visitAsString(ctx->identifier());
     RETURN_NEW_AST_NODE(
         "HogQLXTag", "{s:s#,s:N}", "kind", kind.data(), kind.size(), "attributes",
@@ -1932,66 +1932,66 @@
     );
   }
 
   VISIT(HogqlxTagElementNested) {
     string opening = visitAsString(ctx->identifier(0));
     string closing = visitAsString(ctx->identifier(1));
     if (opening != closing) {
-      throw SyntaxException("Opening and closing HogQLX tags must match. Got " + opening + " and " + closing);
+      throw SyntaxError("Opening and closing HogQLX tags must match. Got " + opening + " and " + closing);
     }
 
     auto tag_element_ctx = ctx->hogqlxTagElement();
     auto tag_attribute_ctx = ctx->hogqlxTagAttribute();
     PyObject* attributes = PyList_New(tag_attribute_ctx.size() + (tag_element_ctx ? 1 : 0));
-    if (!attributes) throw PyInternalException();
+    if (!attributes) throw PyInternalError();
     bool found_source = false;
     for (size_t i = 0; i < tag_attribute_ctx.size(); i++) {
       PyObject* object;
       try {
         object = visitAsPyObject(tag_attribute_ctx[i]);
       } catch (...) {
         Py_DECREF(attributes);
         throw;
       }
       PyList_SET_ITEM(attributes, i, object);
 
       PyObject* name = PyObject_GetAttrString(object, "name");
       if (!name) {
         Py_DECREF(attributes);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       PyObject* source_as_str = PyUnicode_FromString("source");
       if (!source_as_str) {
         Py_DECREF(name);
         Py_DECREF(attributes);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       int tentative_found_source = PyObject_RichCompareBool(name, source_as_str, Py_EQ);
       Py_DECREF(source_as_str);
       Py_DECREF(name);
       if (tentative_found_source == -1) {
         Py_DECREF(attributes);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       if (tentative_found_source) {
         found_source = true;
       }
     }
 
     if (tag_element_ctx) {
       if (found_source) {
         Py_DECREF(attributes);
-        throw SyntaxException("Nested HogQLX tags cannot have a source attribute");
+        throw SyntaxError("Nested HogQLX tags cannot have a source attribute");
       }
       PyObject* source_attribute = build_ast_node(
           "HogQLXAttribute", "{s:s#,s:N}", "name", "source", 6, "value", visitAsPyObject(ctx->hogqlxTagElement())
       );
       if (!source_attribute) {
         Py_DECREF(attributes);
-        throw PyInternalException();
+        throw PyInternalError();
       }
       PyList_SET_ITEM(attributes, tag_attribute_ctx.size(), source_attribute);
     }
 
     RETURN_NEW_AST_NODE("HogQLXTag", "{s:s#,s:N}", "kind", opening.data(), opening.size(), "attributes", attributes);
   }
 
@@ -2029,15 +2029,15 @@
       const string& msg,
       exception_ptr e
   ) override {
     size_t start = getPosition(line, charPositionInLine);
     if (start == string::npos) {
       start = 0;
     }
-    throw SyntaxException(msg, start, input.size());
+    throw SyntaxError(msg, start, input.size());
   }
 
  private:
   size_t getPosition(size_t line, size_t column) {
     size_t linePosition = 0;
     for (size_t i = 0; i < line - 1; i++) {
       size_t increment = input.find("\n", linePosition) + 1;
@@ -2073,15 +2073,15 @@
     auto parser = new HogQLParser(stream);                                                                             \
     parser->removeErrorListeners();                                                                                    \
     auto error_listener = new HogQLErrorListener(str);                                                                 \
     parser->addErrorListener(error_listener);                                                                          \
     HogQLParser::PASCAL_CASE##Context* parse_tree;                                                                     \
     try {                                                                                                              \
       parse_tree = parser->CAMEL_CASE();                                                                               \
-    } catch HANDLE_HOGQL_EXCEPTION(SyntaxException, delete error_listener; delete parser; delete stream; delete lexer; \
+    } catch HANDLE_HOGQL_ERROR(SyntaxError, delete error_listener; delete parser; delete stream; delete lexer; \
                                    delete input_stream;);                                                              \
     HogQLParseTreeConverter converter = HogQLParseTreeConverter(state, internal == 1);                                 \
     PyObject* result_node = converter.visitAsPyObjectFinal(parse_tree);                                                \
     delete error_listener;                                                                                             \
     delete parser;                                                                                                     \
     delete stream;                                                                                                     \
     delete lexer;                                                                                                      \
@@ -2100,15 +2100,15 @@
   const char* str;
   if (!PyArg_ParseTuple(args, "s", &str)) {
     return NULL;
   }
   string unquoted_string;
   try {
     unquoted_string = unquote_string(str);
-  } catch HANDLE_HOGQL_EXCEPTION(SyntaxException, );
+  } catch HANDLE_HOGQL_ERROR(SyntaxError, );
   return PyUnicode_FromStringAndSize(unquoted_string.data(), unquoted_string.size());
 }
 
 // MODULE SETUP
 
 static PyMethodDef parser_methods[] = {
     {.ml_name = "parse_expr",
```

### Comparing `hogql_parser-1.0.6/pyproject.toml` & `hogql_parser-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hogql_parser-1.0.6/setup.py` & `hogql_parser-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     library_dirs=[f"{homebrew_location}/lib/"] if is_macos else ["/usr/lib/", "/usr/lib64/"],
     libraries=["antlr4-runtime"],
     extra_compile_args=["-std=c++20"],
 )
 
 setup(
     name="hogql_parser",
-    version="1.0.6",
+    version="1.0.7",
     url="https://github.com/PostHog/posthog/tree/master/hogql_parser",
     author="PostHog Inc.",
     author_email="hey@posthog.com",
     maintainer="PostHog Inc.",
     maintainer_email="hey@posthog.com",
     description="HogQL parser for internal PostHog use",
     long_description=open("README.md").read(),
```

### Comparing `hogql_parser-1.0.6/string.cpp` & `hogql_parser-1.0.7/string.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #include "string.h"
 
 using namespace std;
 
 string unquote_string(string text) {
   size_t original_text_size = text.size();
   if (original_text_size == 0) {
-    throw ParsingException("Encountered an unexpected empty string input");
+    throw ParsingError("Encountered an unexpected empty string input");
   }
   const char first_char = text.front();
   const char last_char = text.back();
   if (first_char == '\'' && last_char == '\'') {
     text = text.substr(1, original_text_size - 2);
     boost::replace_all(text, "''", "'");
     boost::replace_all(text, "\\'", "'");
@@ -25,15 +25,15 @@
     boost::replace_all(text, "``", "`");
     boost::replace_all(text, "\\`", "`");
   } else if (first_char == '{' && last_char == '}') {
     text = text.substr(1, original_text_size - 2);
     boost::replace_all(text, "{{", "{");
     boost::replace_all(text, "\\{", "{");
   } else {
-    throw SyntaxException("Invalid string literal, must start and end with the same quote type: " + text);
+    throw SyntaxError("Invalid string literal, must start and end with the same quote type: " + text);
   }
 
   // Copied from clickhouse_driver/util/escape.py
   boost::replace_all(text, "\\a", "\a");
   boost::replace_all(text, "\\b", "\b");
   boost::replace_all(text, "\\f", "\f");
   boost::replace_all(text, "\\n", "\n");
@@ -46,13 +46,13 @@
   return text;
 }
 
 string unquote_string_terminal(antlr4::tree::TerminalNode* node) {
   string text = node->getText();
   try {
     return unquote_string(text);
-  } catch (SyntaxException& e) {
-    throw SyntaxException(e.what(), node->getSymbol()->getStartIndex(), node->getSymbol()->getStopIndex() + 1);
-  } catch (ParsingException& e) {
-    throw ParsingException(e.what(), node->getSymbol()->getStartIndex(), node->getSymbol()->getStopIndex() + 1);
+  } catch (SyntaxError& e) {
+    throw SyntaxError(e.what(), node->getSymbol()->getStartIndex(), node->getSymbol()->getStopIndex() + 1);
+  } catch (ParsingError& e) {
+    throw ParsingError(e.what(), node->getSymbol()->getStartIndex(), node->getSymbol()->getStopIndex() + 1);
   }
 }
```

