# Comparing `tmp/ofnodes-1.0.0.tar.gz` & `tmp/ofnodes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.0.0.tar", max compression
+gzip compressed data, was "ofnodes-1.0.1.tar", max compression
```

## Comparing `ofnodes-1.0.0.tar` & `ofnodes-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-03-25 17:13:37.977755 ofnodes-1.0.0/README.md
--rw-r--r--   0        0        0      590 2024-04-04 17:47:49.284523 ofnodes-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      100 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1747 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.0.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    18327 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 ofnodes-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1691 2024-04-05 18:37:11.805026 ofnodes-1.0.1/README.md
+-rw-r--r--   0        0        0      590 2024-04-05 18:38:42.024542 ofnodes-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.0.1/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.1/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1747 2024-04-04 17:47:49.284523 ofnodes-1.0.1/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.0.1/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.1/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    17664 2024-04-05 18:26:37.004190 ofnodes-1.0.1/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 ofnodes-1.0.1/PKG-INFO
```

### Comparing `ofnodes-1.0.0/pyproject.toml` & `ofnodes-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.0.0"
+version = "1.0.1"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.0.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.0.1/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.0.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.0.1/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,45 +20,38 @@
         SinglyLinkedList(head=None, tail=None)
     """
     def __init__(self) -> None:
         self._head: Optional[SinglyNode] = None
         self._tail: Optional[SinglyNode] = None
 
     @property
-    def head(self):
+    def head(self) -> SinglyNode | None:
         """Getter property for the head of the linked list.
 
         Returns:
             SinglyNode | None: The head of the linked list, or None if the list is empty.
 
         Notes:
             The `head` property allows access to the first node in the linked list.
 
         Examples:
             >>> llist = SinglyLinkedList()
-            >>> llist
-            SinglyLinkedList(head=None, tail=None)
             >>> llist.head = "first node"
-            >>> llist.head
-            SinglyNode(data='first node')
-            >>> assert llist.head is llist.tail
-            >>> assert llist.head.next is None
+            >>> llist.head = [42.0, True, "LGRW"]
+            >>> llist.tail = "third node added to list"
             >>> llist
-            SinglyLinkedList(head=This node's data is 11 of type str., tail=This node's data is 10 of type str.)
-            >>> llist.head, llist.head.next, llist.tail
-            (SinglyNode(data='second node'), SinglyNode(data='first node'), SinglyNode(data='first node'))
-            llist.head = None
-            >>> llist.head = None
-            >>> llist.head, llist.head.next, llist.tail
-            (SinglyNode(data=None), SinglyNode(data='second node'), SinglyNode(data='first node'))
-            >>> llist.head.__dict__
-            {'_data': None, '_next': SinglyNode(data='second node')}
-            >>> llist.remove_head()
-            >>> llist.head.__dict__
-            {'_data': 'second node', '_next': SinglyNode(data='first node')}
+            SinglyLinkedList(head=This node's data is 3 of type list., tail=This node's data is 24 of type str.)
+            >>> llist.tail = None
+            >>> llist
+            SinglyLinkedList(head=This node's data is 3 of type list., tail=This node's data is of type NoneType.)
+            >>> llist.head.next.data
+            'first node'
+            >>> llist.remove_tail()
+            >>> llist.tail.data
+            'third node added to list'
         """
         return self._head
 
     @head.setter
     def head(self, value: SinglyNode | Any) -> None:
         """
         Setter property for the head of the linked list.
@@ -93,15 +86,15 @@
             AttributeError: Deleting the `head` attribute is not allowed.
         """
         raise AttributeError(
             f"{type(self).__name__}'s `head` attribute " "cannot be deleted."
         )
 
     @property
-    def tail(self):
+    def tail(self) -> SinglyNode | None:
         """
         Getter property for the tail of the linked list.
 
         Returns:
             SinglyNode | None: The tail of the linked list, or None if the list is empty.
 
         Examples:
@@ -174,15 +167,15 @@
             case SinglyLinkedList(head=None, tail=None):
                 return "This instance of SinglyLinkedList is empty."
             case SinglyLinkedList(head=head, tail=tail):
                 if head is tail:
                     return "This instance of SinglyLinkedList has a single node."
                 return "The head and tail are different nodes."
 
-    def insert_head(self, data):
+    def insert_head(self, data: Any) -> None:
         """ Inserts a new node with the provided data at the head of the linked list.
 
         Args:
             data: The data to be inserted into the new node. If the data is already a
                 `SinglyNode` object, it is inserted directly; otherwise, a new
                 `SinglyNode` object is created with the provided data.
 
@@ -220,32 +213,25 @@
             [None, None, None, None]
             >>> llist.head = "to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`'), SinglyNode(data='4 node'), SinglyNode(data='1 node'))
         """
         self.head = data  # trigger the head setter
 
-    def insert_tail(self, data):
+    def insert_tail(self, data: Any) -> None:
         """Inserts a new node with the provided data at the tail of the linked list.
 
         Args:
             data: The data to be inserted into the new node. If the data is already a
                 `SinglyNode` object, it is inserted directly; otherwise, a new
                 `SinglyNode` object is created with the provided data.
 
         Returns:
             None
 
-        Raises:
-            ~~RuntimeError: If the linked list is not properly initialized (unexpected
-                condition where `self.tail` is `None`).~~
-
-            `self.tail` can't be deleted from instance. It's data value can be written
-            over, but the attribute persists.
-
         Notes:
             If the linked list is empty, the new node becomes both the head and the
             tail of the linked list. Otherwise, the new node is appended to the end
             of the list by updating the `next` attribute of the current tail node
             to point to the new node, and then updating the instance's `tail`
             attribute to reference the new node.
 
@@ -279,15 +265,15 @@
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
-    def search(self, target):
+    def search(self, target) -> bool:
         """Searches for a target value in the linked list.
 
         Args:
             target (Any): The value to search for in the linked list.
 
         Returns:
             bool: True if the target value is found in the linked list, False otherwise.
@@ -318,15 +304,15 @@
             while current_node:
                 if current_node.data == target:
                     return True
                 current_node = current_node.next
             return False
         raise ValueError("Cannot perform search: The list is empty.")
 
-    def remove_head(self):
+    def remove_head(self) -> None:
         """Removes the head node from the linked list.
 
         Raises:
             ValueError: If the linked list is empty.
 
         Returns:
             None
@@ -357,15 +343,15 @@
             self._tail = None
             return
         if self._head and self._head is not self._tail:
             self._head = self.head.next
             return
         raise ValueError("Cannot remove head from empty list")
 
-    def remove_tail(self):
+    def remove_tail(self) -> None:
         """Removes the tail node from the linked list.
 
         Raises:
             ValueError: If the linked list is empty.
 
         Returns:
             None
@@ -417,17 +403,14 @@
                     node = getattr(node, "_next")  # keep looking
                 setattr(node, "_next", None)  # point the second to last node to None
                 setattr(self, "_tail", node)  # assign tail to the node
 
     def print_node_data(self) -> None:
         """Traverse the linked list and print the data attribute of each node.
 
-        Args:
-            None
-
         Returns:
             None
 
         Notes:
             This method iterates through the linked list starting from the head node and prints the data attribute of each node
             until the end of the list is reached.
```

