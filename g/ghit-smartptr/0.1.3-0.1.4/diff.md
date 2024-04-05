# Comparing `tmp/ghit_smartptr-0.1.3.tar.gz` & `tmp/ghit_smartptr-0.1.4.tar.gz`

## Comparing `ghit_smartptr-0.1.3.tar` & `ghit_smartptr-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/requirements.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/.ghit/.gitignore
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/.ghit/stack
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/__main__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/args.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/branch_commands.py
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/common.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/error.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/gh.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/gh_formatting.py
--rw-r--r--   0        0        0    14791 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/gh_graphql.py
--rwxr-xr-x   0        0        0     3563 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/ghit.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/gitools.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/graphql.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/stack.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/stack_commands.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/styling.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/terminal.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/ghit/top_commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/tests/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/tests/test_gh_graphql.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/tests/test_graphql.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/src/tests/test_stack.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/LICENSE
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/README.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/__main__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/args.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/branch_commands.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/common.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/error.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gh.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gh_formatting.py
+-rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gh_graphql.py
+-rwxr-xr-x   0        0        0     3563 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/ghit.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/gitools.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/graphql.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/stack.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/stack_commands.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/styling.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/terminal.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/ghit/top_commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/test_gh_graphql.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/test_graphql.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/src/tests/test_stack.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 ghit_smartptr-0.1.4/PKG-INFO
```

### Comparing `ghit_smartptr-0.1.3/.github/workflows/python-app.yml` & `ghit_smartptr-0.1.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/.github/workflows/python-publish.yml` & `ghit_smartptr-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/branch_commands.py` & `ghit_smartptr-0.1.4/src/ghit/branch_commands.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/common.py` & `ghit_smartptr-0.1.4/src/ghit/common.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/gh.py` & `ghit_smartptr-0.1.4/src/ghit/gh.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,10 +247,12 @@
         return pr
 
 
 def init_gh(repo: git.Repository, stack: Stack, offline: bool) -> GH | None:
     gh = GH(repo, stack) if not offline and is_gh(repo) else None
     if gh:
         logging.debug('found gh repository %s', gh.repository)
+    elif offline:
+        logging.debug('working offline')
     else:
         logging.debug('gh not found')
     return gh
```

### Comparing `ghit_smartptr-0.1.3/src/ghit/gh_formatting.py` & `ghit_smartptr-0.1.4/src/ghit/gh_formatting.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/gh_graphql.py` & `ghit_smartptr-0.1.4/src/ghit/gh_graphql.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,14 @@
 def graphql(token: str, query: str) -> any:
     logging.debug('query GH graphql: %s', query)
     response = requests.post(
         url=os.getenv('GITHUB_API_URL', 'https://api.github.com/graphql'),
         headers={
             'Authorization': f'Bearer {token}',
             'Accept': 'application/vnd.github.v3+json',
-            'X-GitHub-Api-Version': '2022-11-28',
         },
         json={'query': query},
         timeout=30,
     )
     logging.debug('response: %s', response.status_code)
     if not response.ok:
         raise BaseException(response.text)
```

### Comparing `ghit_smartptr-0.1.3/src/ghit/ghit.py` & `ghit_smartptr-0.1.4/src/ghit/ghit.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/gitools.py` & `ghit_smartptr-0.1.4/src/ghit/gitools.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/graphql.py` & `ghit_smartptr-0.1.4/src/ghit/graphql.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/stack.py` & `ghit_smartptr-0.1.4/src/ghit/stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,31 +16,31 @@
         branch_name: str | None = None,
         enabled: bool = False,
         parent: Stack | None = None,
     ):
         self.branch_name = branch_name
         self.__parent = parent
         self._enabled = enabled
-        self.depth = parent.depth + 1 if parent else 0
+        self.depth = parent.depth + 1 if parent else -1
         self._index = parent.length() if parent else 0
         self._children = dict[str, Stack]()
 
-    def get_parent(self) -> Stack:
+    def get_parent(self, ignore_enabled: bool = False) -> Stack:
         if self.__parent is None:
             return None
         p = self.__parent
-        return p if p._enabled else p.get_parent()
+        return p if p._enabled or ignore_enabled else p.get_parent(ignore_enabled)
 
     def disable(self) -> None:
         self._enabled = False
 
     def add_child(self, branch_name: str, enabled: bool = True) -> Stack:
         if branch_name in self._children:
             raise GhitError(f"'{branch_name}' already exist in '{self.branch_name}'")
-        child = Stack(branch_name, enabled, self if self._enabled else self.get_parent())
+        child = Stack(branch_name, enabled, self)
         self._children.update({branch_name: child})
         return child
 
     def is_last_child(self) -> bool:
         return self.is_root() or self._index == self.get_parent().length() - 1
 
     def length(self) -> int:
@@ -52,19 +52,26 @@
             else:
                 length += v.length()
         return length
 
     def is_root(self) -> bool:
         return self.branch_name is None
 
-    def traverse(self, with_first_level: bool = True) -> Iterator[Stack]:
-        if not self.is_root() and self._enabled and (self.get_parent() or with_first_level):
+    def traverse(self, with_first_level: bool = True, ignored_disabled: bool = False) -> Iterator[Stack]:
+        if not self.is_root() and (self._enabled or ignored_disabled) and \
+            (self.get_parent(ignored_disabled) or with_first_level):
             yield self
         for r in self._children.values():
-            yield from r.traverse(with_first_level)
+            yield from r.traverse(with_first_level, ignored_disabled)
+
+    def find(self, branch_name: str) -> Stack:
+        for s in self.traverse(True, True):
+            if s.branch_name == branch_name:
+                return s
+        return None
 
     def _find_depth(self) -> int:
         depth = 0
         for record in self.traverse():
             depth = max(depth, record.depth)
         return depth
 
@@ -83,45 +90,48 @@
             lines.append(('' if self._enabled else '#') + '.' * depth + self.branch_name)
         for record in self._children.values():
             record.dumps(lines, depth + (not self.is_root()))
         return lines
 
 
 def parse_line(line: str, parents: list[Stack]) -> Stack:
+    line = line.strip(' \t\r\n')
     enabled = not line.startswith('#')
-
-    stack_line = line.rstrip().lstrip('#')
-    branch_name = stack_line.lstrip('.')
+    stack_line = line.lstrip('#').lstrip()
+    branch_name = stack_line.lstrip('. \t')
     if not branch_name:
         raise GhitError('no branch name')
 
-    depth = len(stack_line) - len(branch_name)
-
-    if len(parents) <= depth:
-        raise GhitError('bad indent')
-
-    for _ in range(1, len(parents) - depth):
+    depth = 0
+    while stack_line[depth] == '.':
+        depth += 1
+
+    while True:
+        parent = parents[-1] if parents else None
+        if not parent.branch_name or parent.depth < depth:
+            break
         parents.pop()
 
-    parent = parents[-1]
-    depth = min(depth, parent.depth + 1)
+    if enabled and depth - parent.depth > 1:
+        raise GhitError('bad indent')
 
     logging.debug('parsed: %s%s%s parent: %s', '' if enabled else '#', '.'*depth, branch_name, parent.branch_name)
 
-    return parent.add_child(branch_name, enabled)
+    child = parent.add_child(branch_name, enabled)
+    parents.append(child)
+    return child
 
 
 def parse(lines: Iterator[str]) -> Stack:
     stack = Stack()
     parents = [stack]
     for i, line in enumerate(lines, start=1):
         logging.debug('reading line [%s]', line)
         try:
-            child = parse_line(line, parents)
-            parents.append(child)
+            parse_line(line, parents)
         except GhitError as e:
             raise GhitError(f'line {i}: {e}') from e
     return stack
 
 
 def open_stack(filename: Path | None) -> Stack | None:
     if filename is None or not filename.is_file():
```

### Comparing `ghit_smartptr-0.1.3/src/ghit/stack_commands.py` & `ghit_smartptr-0.1.4/src/ghit/stack_commands.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/styling.py` & `ghit_smartptr-0.1.4/src/ghit/styling.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/ghit/top_commands.py` & `ghit_smartptr-0.1.4/src/ghit/top_commands.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/tests/test_gh_graphql.py` & `ghit_smartptr-0.1.4/src/tests/test_gh_graphql.py`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/src/tests/test_graphql.py` & `ghit_smartptr-0.1.4/src/tests/test_graphql.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,21 +52,21 @@
     f = func(
         'func',
         {'a': 1, 'b': '"word"'},
         obj('pageInfo', 'endCursor', 'hasNextPage'),
         obj('edges', 'cursor', obj('node', *['1', '2'])),
     )
 
-    assert 'func(a: 1, b: "word"){ pageInfo{ endCursor hasNextPage } ' + 'edges{ cursor node{ 1 2 } } }' == f
+    assert f == 'func(a: 1, b: "word"){ pageInfo{ endCursor hasNextPage } ' + 'edges{ cursor node{ 1 2 } } }'
 
 
 def test_paged():
-    assert 'object(a: 1, b: "word"){ pageInfo{ endCursor hasNextPage } ' + 'edges{ cursor node{ c d } } }' == paged(
+    assert paged(
         'object', {'a': 1, 'b': '"word"'}, 'c', 'd'
-    )
+    ) == 'object(a: 1, b: "word"){ pageInfo{ endCursor hasNextPage } ' + 'edges{ cursor node{ c d } } }'
 
 
 def test_cursor_or_null():
     assert cursor_or_null('x') == '"x"'
     assert cursor_or_null(None) == 'null'
```

### Comparing `ghit_smartptr-0.1.3/src/tests/test_stack.py` & `ghit_smartptr-0.1.4/src/tests/test_stack.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,105 +11,119 @@
     assert child.get_parent() is None
 
 
 def test_parse_line():
     stack = Stack()
     parents = [stack]
     child = parse_line('main', parents)
-    parents.append(child)
     assert child.get_parent() is None
     assert stack._children['main'].branch_name == 'main'
     assert child.branch_name == 'main'
     assert child.depth == 0
 
     child = parse_line('.a1', parents)
-    parents.append(child)
     assert child.branch_name == 'a1'
     assert child.depth == 1
     assert child.get_parent().branch_name == 'main'
 
     child = parse_line('..a2', parents)
-    parents.append(child)
     assert child.branch_name == 'a2'
     assert child.depth == 2  # noqa: PLR2004
     assert child.get_parent().branch_name == 'a1'
 
     child = parse_line('..a21', parents)
-    parents.append(child)
     assert child.branch_name == 'a21'
     assert child.depth == 2  # noqa: PLR2004
     assert child.get_parent().branch_name == 'a1'
 
     child = parse_line('.b1', parents)
-    parents.append(child)
     assert child.branch_name == 'b1'
     assert child.depth == 1
     assert child.get_parent().branch_name == 'main'
 
     child = parse_line('dev', parents)
-    parents.append(child)
     assert child.branch_name == 'dev'
     assert child.depth == 0
     assert child.get_parent() is None
 
 
 def test_disabled():
     stack = Stack()
     parents = [stack]
     child = parse_line('main', parents)
-    parents.append(child)
 
     child = parse_line('#.a1', parents)
-    parents.append(child)
     assert child.branch_name == 'a1'
     assert child.depth == 1
 
     child = parse_line('..a2', parents)
-    parents.append(child)
     assert child.branch_name == 'a2'
-    assert child.depth == 1
+    assert child.depth == 2  # noqa: PLR2004
     assert child.get_parent().branch_name == 'main'
 
     child = parse_line('..a21', parents)
-    parents.append(child)
     assert child.branch_name == 'a21'
-    assert child.depth == 1
+    assert child.depth == 2  # noqa: PLR2004
     assert child.get_parent().branch_name == 'main'
 
     child = parse_line('.b1', parents)
-    parents.append(child)
     assert child.branch_name == 'b1'
     assert child.depth == 1
     assert child.get_parent().branch_name == 'main'
 
     child = parse_line('dev', parents)
-    parents.append(child)
     assert child.branch_name == 'dev'
     assert child.depth == 0
     assert child.get_parent() is None
 
 def test_bad_indent():
-    stack = Stack()
-    parents = [stack]
-    child = parse_line('main', parents)
-    parents.append(child)
-    assert child.get_parent() is None
-    assert stack._children['main'].branch_name == 'main'
-    assert child.branch_name == 'main'
-    assert child.depth == 0
-
+    text = ['main', '..a2']
     with pytest.raises(GhitError):
-        child = parse_line('..a1', parents)
+        parse(text)
 
+    text = ['#.disabled', 'main']
+    parse(text)
 
 def test_parse():
     text = ['main', '.b1', '..b2']
     stack = parse(text)
     assert stack is not None
     assert stack.dumps() == text
 
 
 def test_parse_disabled():
-    text = ['main', '#.a1', '..a2', '..a21', '...a3', '..a22', '.b1', '..b2']
+    text = ['main', '#.disabled', '..a2', '..a21', '...a3', '..a22', '.b1', '..b2']
     stack = parse(text)
     assert stack is not None
     assert stack.dumps() == text
+
+    s = stack.find('main')
+    assert s.get_parent() is None
+    assert s.get_parent(True).branch_name is None
+
+    s = stack.find('a2')
+    assert s.get_parent().branch_name == 'main'
+    assert s.get_parent(True).branch_name == 'disabled'
+
+    s = stack.find('a21')
+    assert s.get_parent().branch_name == 'main'
+    assert s.get_parent(True).branch_name == 'disabled'
+
+    s = stack.find('a3')
+    assert s.get_parent().branch_name == 'a21'
+    assert s.get_parent(True).branch_name == 'a21'
+
+    s = stack.find('a22')
+    assert s.get_parent().branch_name == 'main'
+    assert s.get_parent(True).branch_name == 'disabled'
+
+    s = stack.find('b1')
+    assert s.get_parent().branch_name == 'main'
+    assert s.get_parent(True).branch_name == 'main'
+
+    s = stack.find('b2')
+    assert s.get_parent().branch_name == 'b1'
+    assert s.get_parent(True).branch_name == 'b1'
+
+    s = stack.find('disabled')
+    assert s.get_parent().branch_name == 'main'
+    assert s.get_parent(True).branch_name == 'main'
```

### Comparing `ghit_smartptr-0.1.3/LICENSE` & `ghit_smartptr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/README.md` & `ghit_smartptr-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ghit_smartptr-0.1.3/pyproject.toml` & `ghit_smartptr-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -27,26 +27,22 @@
 packages = ['src/ghit']
 
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [tool.ruff]
-select = ['E', 'F', 'W', 'I', 'YTT', 'FA', 'ISC', 'ICN', 'G', 'C90', 'N', 'UP', 'S', 'B', 'C4', 'DTZ', 'DJ', 'PIE', 'T20', 'PT', 'Q', 'RSE', 'RET', 'SIM', 'TID', 'TCH', 'INT', 'PTH', 'PL']
 line-length = 120
 target-version = 'py39'
 
-[tool.ruff.per-file-ignores]
-'*/tests/*' = ['S101']
-
-[tool.ruff.pylint]
-max-args = 8
-
-[tool.ruff.flake8-quotes]
-inline-quotes = 'single'
+[tool.ruff.lint]
+select = ['E', 'F', 'W', 'I', 'YTT', 'FA', 'ISC', 'ICN', 'G', 'C90', 'N', 'UP', 'S', 'B', 'C4', 'DTZ', 'DJ', 'PIE', 'T20', 'PT', 'Q', 'RSE', 'RET', 'SIM', 'TID', 'TCH', 'INT', 'PTH', 'PL']
+flake8-quotes.inline-quotes = 'single'
+per-file-ignores.'*/tests/*' = ['S101']
+pylint.max-args = 8
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
 skip-string-normalization = true
 
 [project.scripts]
```

### Comparing `ghit_smartptr-0.1.3/PKG-INFO` & `ghit_smartptr-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ghit-smartptr
-Version: 0.1.3
+Version: 0.1.4
 Summary: ghit
 Project-URL: Homepage, https://github.com/0x656b694d/ghit
 Project-URL: Issues, https://github.com/0x656b694d/ghit/issues
 Author-email: Michaël Petrov <smartptr@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Michaël
```

