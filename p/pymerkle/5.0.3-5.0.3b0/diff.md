# Comparing `tmp/pymerkle-5.0.3.tar.gz` & `tmp/pymerkle-5.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymerkle-5.0.3.tar", last modified: Sun Jun 11 21:45:06 2023, max compression
+gzip compressed data, was "dist/pymerkle-5.0.3b0.tar", last modified: Fri Nov 15 17:12:06 2019, max compression
```

## Comparing `pymerkle-5.0.3.tar` & `pymerkle-5.0.3b0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:45:06.039398 pymerkle-5.0.3/
--rw-r--r--   0 none      (1000) none      (1000)    35147 2023-02-03 09:19:28.000000 pymerkle-5.0.3/LICENSE
--rw-rw-r--   0 none      (1000) none      (1000)     6001 2023-06-11 21:45:06.039398 pymerkle-5.0.3/PKG-INFO
--rw-rw-r--   0 none      (1000) none      (1000)     5029 2023-06-11 21:02:25.000000 pymerkle-5.0.3/README.md
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:45:06.039398 pymerkle-5.0.3/pymerkle/
--rw-rw-r--   0 none      (1000) none      (1000)      464 2023-06-11 21:43:57.000000 pymerkle-5.0.3/pymerkle/__init__.py
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:45:06.039398 pymerkle-5.0.3/pymerkle/concrete/
--rw-rw-r--   0 none      (1000) none      (1000)        0 2023-06-11 21:43:57.000000 pymerkle-5.0.3/pymerkle/concrete/__init__.py
--rw-rw-r--   0 none      (1000) none      (1000)    11501 2023-06-11 21:02:25.000000 pymerkle-5.0.3/pymerkle/concrete/inmemory.py
--rw-rw-r--   0 none      (1000) none      (1000)     3408 2023-06-11 21:02:25.000000 pymerkle-5.0.3/pymerkle/concrete/sqlite.py
--rw-rw-r--   0 none      (1000) none      (1000)      173 2023-06-08 10:32:47.000000 pymerkle-5.0.3/pymerkle/constants.py
--rw-rw-r--   0 none      (1000) none      (1000)     8586 2023-06-11 21:02:25.000000 pymerkle-5.0.3/pymerkle/core.py
--rw-rw-r--   0 none      (1000) none      (1000)     2106 2023-06-08 10:32:47.000000 pymerkle-5.0.3/pymerkle/hasher.py
--rw-rw-r--   0 none      (1000) none      (1000)     4588 2023-06-08 10:32:47.000000 pymerkle-5.0.3/pymerkle/proof.py
--rw-rw-r--   0 none      (1000) none      (1000)      783 2023-06-09 10:44:21.000000 pymerkle-5.0.3/pymerkle/utils.py
-drwxrwxr-x   0 none      (1000) none      (1000)        0 2023-06-11 21:45:06.039398 pymerkle-5.0.3/pymerkle.egg-info/
--rw-rw-r--   0 none      (1000) none      (1000)     6001 2023-06-11 21:45:06.000000 pymerkle-5.0.3/pymerkle.egg-info/PKG-INFO
--rw-rw-r--   0 none      (1000) none      (1000)      388 2023-06-11 21:45:06.000000 pymerkle-5.0.3/pymerkle.egg-info/SOURCES.txt
--rw-rw-r--   0 none      (1000) none      (1000)        1 2023-06-11 21:45:06.000000 pymerkle-5.0.3/pymerkle.egg-info/dependency_links.txt
--rw-rw-r--   0 none      (1000) none      (1000)        1 2023-06-11 21:45:06.000000 pymerkle-5.0.3/pymerkle.egg-info/not-zip-safe
--rw-rw-r--   0 none      (1000) none      (1000)        9 2023-06-11 21:45:06.000000 pymerkle-5.0.3/pymerkle.egg-info/top_level.txt
--rw-rw-r--   0 none      (1000) none      (1000)       38 2023-06-11 21:45:06.039398 pymerkle-5.0.3/setup.cfg
--rw-rw-r--   0 none      (1000) none      (1000)     1832 2023-06-11 21:02:25.000000 pymerkle-5.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/validations/
+-rwxr-xr-x   0 root         (0) root         (0)     9185 2019-11-01 19:35:41.000000 pymerkle-5.0.3b0/pymerkle/validations/mechanisms.py
+-rw-r--r--   0 root         (0) root         (0)      112 2019-10-30 18:07:48.000000 pymerkle-5.0.3b0/pymerkle/validations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/core/
+-rwxr-xr-x   0 root         (0) root         (0)    12346 2019-11-01 21:52:00.000000 pymerkle-5.0.3b0/pymerkle/core/prover.py
+-rwxr-xr-x   0 root         (0) root         (0)    12228 2019-11-01 19:18:15.000000 pymerkle-5.0.3b0/pymerkle/core/nodes.py
+-rwxr-xr-x   0 root         (0) root         (0)    26038 2019-11-01 19:42:30.000000 pymerkle-5.0.3b0/pymerkle/core/tree.py
+-rw-r--r--   0 root         (0) root         (0)       91 2019-10-27 15:32:24.000000 pymerkle-5.0.3b0/pymerkle/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6031 2019-10-31 18:42:38.000000 pymerkle-5.0.3b0/pymerkle/core/encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-12 12:35:43.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      539 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9157 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/hashing/
+-rw-r--r--   0 root         (0) root         (0)      132 2019-10-21 17:45:51.000000 pymerkle-5.0.3b0/pymerkle/hashing/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5246 2019-11-01 07:12:24.000000 pymerkle-5.0.3b0/pymerkle/hashing/machine.py
+-rw-r--r--   0 root         (0) root         (0)     3921 2019-11-01 06:49:29.000000 pymerkle-5.0.3b0/pymerkle/hashing/encoding.py
+-rwxr-xr-x   0 root         (0) root         (0)     6754 2019-11-12 14:04:20.000000 pymerkle-5.0.3b0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2019-11-15 17:11:39.000000 pymerkle-5.0.3b0/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9157 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pymerkle-5.0.3/pymerkle/concrete/inmemory.py` & `pymerkle-5.0.3b0/pymerkle/core/nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,450 +1,398 @@
-from pymerkle.utils import decompose
-from pymerkle.core import BaseMerkleTree
+"""
+Provides classes for the Merkle-tree's leaves and internal nodes
+"""
 
+from abc import ABCMeta, abstractmethod
 
-class Node:
-    """
-    Merkle-tree node
+from pymerkle.serializers import NodeSerializer, LeafSerializer
+from pymerkle.exceptions import (NoChildException, NoDescendantException,
+    NoParentException, LeafConstructionError, UndecodableArgumentError,
+    UndecodableRecord)
+from pymerkle.utils import NONE
+import json
 
-    :param value: the hash to be stored by the node
-    :type value: bytes
-    :param left: [optional] left child
-    :type left: Node
-    :param right: [optional] right child
-    :type right: Node
-    :rtype: Node
-    """
 
-    __slots__ = ('value', 'left', 'right', 'parent')
+# Prefices used for node and tree printing
 
+L_BRACKET_SHORT = '\u2514' + '\u2500'           # └─
+L_BRACKET_LONG  = '\u2514' + 2 * '\u2500'       # └──
+T_BRACKET       = '\u251C' + 2 * '\u2500'       # ├──
+VERTICAL_BAR    = '\u2502'                      # │
 
-    def __init__(self, value, left=None, right=None):
-        self.value = value
 
-        self.left = left
-        if left:
-            left.parent = self
+class __Node(object, metaclass=ABCMeta):
+    """
+    Abstract base class for Merkle-tree leaves and internal nodes
+    """
 
-        self.right = right
-        if right:
-            right.parent = self
+    __slots__ = ('__encoding', '__child',)
 
-        self.parent = None
+    def __init__(self, encoding):
+        self.__encoding = encoding
 
 
-    def is_root(self):
+    @abstractmethod
+    def serialize(self):
         """
-        :rtype: bool
         """
-        return not self.parent
-
 
-    def is_leaf(self):
+    @abstractmethod
+    def toJSONString(self):
         """
-        :rtype: bool
         """
-        return not self.left and not self.right
 
+    @property
+    def encoding(self):
+        return self.__encoding
 
-    def is_left_child(self):
+
+    @property
+    def child(self):
         """
-        :rtype: bool
+        :raises NoChildException: if the node has no *.child* attribute
         """
-        parent = self.parent
-        if not parent:
-            return False
+        try:
+            return self.__child
+        except AttributeError:
+            raise NoChildException
 
-        return self == parent.left
+    def set_child(self, child):
+        self.__child = child
 
 
-    def is_right_child(self):
+    @property
+    def left(self):
         """
-        :rtype: bool
+        :raises NoChildException: if the node has no *.left* attribute
         """
-        parent = self.parent
-        if not parent:
-            return False
-
-        return self == parent.right
+        try:
+            return self.__left
+        except AttributeError:
+            raise NoParentException
 
 
-    def get_ancestor(self, degree):
+    @property
+    def right(self):
         """
-        .. note:: Ancestor of degree 0 is the node itself, ancestor of degree
-            1 is the node's parent, etc.
-
-        :type degree: int
-        :rtype: Node
+        :raises NoChildException: if the node has no *.right* attribute
         """
-        curr = self
-        while degree > 0:
-            curr = curr.parent
-            degree -= 1
-
-        return curr
+        try:
+            return self.__right
+        except AttributeError:
+            raise NoParentException
 
 
-    def expand(self, indent=2, trim=None, level=0, ignored=None):
+    def is_left_parent(self):
         """
-        Returns a string representing the subtree rooted at the current node
+        Checks if the node is a left parent.
 
-        :param indent: [optional]
-        :type indent: str
-        :param trim: [optional]
-        :type trim: str
-        :param level: [optional]
-        :type level: str
-        :param ignored: [optional]
-        :type ignored: str
-        :rtype: str
+        :returns: *True* iff the node is the *.left* attribute of some
+                other node inside the containing tree
+        :rtype: bool
         """
-        ignored = ignored or []
-
-        if level == 0:
-            out = 2 * '\n' + ' └─' if not self.parent else ''
-        else:
-            out = (indent + 1) * ' '
-
-        col = 1
-        while col < level:
-            out += ' │' if col not in ignored else 2 * ' '
-            out += indent * ' '
-            col += 1
+        try:
+            _child = self.child
+        except NoChildException:
+            return False
+        return self == _child.left
 
-        if self.is_left_child():
-            out += ' ├──'
 
-        if self.is_right_child():
-            out += ' └──'
-            ignored += [level]
+    def is_right_parent(self):
+        """
+        Checks if the node is a right parent.
 
-        checksum = self.value.hex()
-        out += (checksum[:trim] + '...') if trim else checksum
-        out += '\n'
+        :returns: *True* iff the node is the *.right* attribute of some
+                other node inside the containing tree
+        :rtype: bool
+        """
+        try:
+            _child = self.child
+        except NoChildException:
+            return False
+        return self == _child.right
 
-        if self.is_leaf():
-            return out
 
-        recursion = (indent, trim, level + 1, ignored[:])
+    def is_parent(self):
+        """
+        Checks if the node is a parent.
 
-        out += self.left.expand(*recursion)
-        out += self.right.expand(*recursion)
+        :returns: *True* iff the node is the *.right* or *.left*
+            attribute of some other node inside the containing tree
+        :rtype: bool
+        """
+        try:
+            self.child
+        except NoChildException:
+            return False
+        return True
 
-        return out
 
+    def descendant(self, degree):
+        """
+        Detects and returns the node that is *degree* steps
+        upwards within the containing Merkle-tree.
 
-class Leaf(Node):
-    """
-    Merkle-tree leaf
+        .. note:: Descendant of degree 0 is the node itself, descendant
+                of degree 1 is the node's child, etc.
 
-    :param entry: data stored by the leaf
-    :type entry: bytes
-    :param value: hash value stored by the leaf
-    :type value: bytes
-    """
+        :param degree: depth of descendancy
+        :type degree:  int
+        :returns:      the descendant corresdponding to the requested depth
+        :rtype:        __Node
 
-    def __init__(self, entry, value):
-        self.entry = entry
+        :raises NoDescendantException: if the provided degree
+            exceeds possibilities
+        """
+        if degree == 0:
+            return self
+        else:
+            try:
+                _child = self.child
+            except NoChildException:
+                raise NoDescendantException
+            return _child.descendant(degree - 1)
+
+
+    def __repr__(self):
+        """
+        Overrides the default implementation.
+
+        Sole purpose of this function is to easy display info
+        about the node by just invoking it at console.
+
+        .. warning:: Contrary to convention, the output of this implementation
+            is not insertible into the *eval()* builtin Python function
+        """
+        def memory_id(obj): return str(hex(id(obj)))
+        try:
+            child_id = memory_id(self.child)
+        except NoChildException:
+            child_id = NONE
+        try:
+            left_id  = memory_id(self.left)
+        except NoParentException:
+            left_id  = NONE
+            right_id = NONE
+        else:
+            right_id = memory_id(self.right)
 
-        super().__init__(value, None, None)
+        return '\n    memory-id    : {self_id}\
+                \n    left parent  : {left_id}\
+                \n    right parent : {right_id}\
+                \n    child        : {child_id}\
+                \n    hash         : {hash}\n'\
+                .format(self_id=memory_id(self),
+                    left_id=left_id,
+                    right_id=right_id,
+                    child_id=child_id,
+                    hash=self.digest.decode(self.encoding))
+
+
+    def __str__(self, encoding=None, level=0, indent=3, ignore=[]):
+        """
+        Overrides the default implementation.
+
+        Designed so that inserting the node as an argument to the builtin
+        *print()* Python function displays the subtree of the Merkle-tree
+        whose root is the present node.
+
+        Sole purpose of this function is to be used for printing Merkle-trees
+        in a terminal friendly way (similar to what is printed at console when
+        running the ``tree`` command of Unix based platforms)
+
+        :param encoding: [optional] encoding type to be used for decoding
+                    the digest stored by the present node
+        :type encoding: str
+        :param level: [optional] Defaults to 0. Must be left equal to the
+                default value when called externally by the user. Increased by
+                1 whenever the function is recursively called, in order for
+                track be kept of depth while printing
+        :type level: int
+        :param indent: [optional] Defaults to 3. The horizontal depth at
+                    which each level of the tree will be indented with
+                    respect to the previous one. Increase to achieve
+                    better visibility of the tree's structure.
+        :type indent: int
+        :param ignore: [optional] Defaults to the empty list. Must be left
+                    equal to the *default* value when called externally by the
+                    user. Augmented appropriately whenever the function is
+                    recursively invoked, in order for track to be kept of the
+                    positions where vertical bars should be omitted.
+        :type ignore: list of integers
+        :rtype: str
 
+        .. note:: Left parents appear above the right ones.
+        """
+        if level == 0:
+            output = '\n'
+            if not self.is_left_parent() and not self.is_right_parent(): # root case
+                output += f' {L_BRACKET_SHORT}'
+        else:
+            output = (indent + 1) * ' '
+        for _ in range(1, level):
+            if _ not in ignore:
+                output += f' {VERTICAL_BAR}'              # Include vertical bar
+            else:
+                output += 2 * ' '
+            output += indent * ' '
+        new_ignore = ignore[:]
+        del ignore
+        if self.is_left_parent():
+            output += f' {T_BRACKET}'
+        if self.is_right_parent():
+            output += f' {L_BRACKET_LONG}'
+            new_ignore.append(level)
+        encoding = encoding if encoding else self.encoding
+        output += f'{self.digest.decode(encoding)}\n'
+        if not isinstance(self, Leaf):                          # Recursive step
+            output += self.left.__str__(encoding, level + 1,
+                                indent, new_ignore)
+            output += self.right.__str__(encoding, level + 1,
+                                indent, new_ignore)
+        return output
 
-class InmemoryTree(BaseMerkleTree):
-    """
-    Non-persistent Merkle-tree with with nodes residing inside the runtime memory
 
-    .. note:: This implementation is intended for debugging and testing. Use it
-        to investigate the tree topology by means of concrete path traversals
+class Leaf(__Node):
     """
+    Class for the Merkle-tree's leaves
 
-    def __init__(self, algorithm='sha256', security=True):
-        self.root = None
-        self.leaves = []
+    By leaf is meant a parentless node storing the checksum
+    of some encrypted record
 
-        super().__init__(algorithm, security)
+    :param hash_func: hash function to be used for encryption.
+    :type hash_func: method
+    :param encoding: encoding type to be used when decoding the
+            digest stored by the leaf
+    :type encoding: str
+    :param record: [optional] the record to be encrypted within the leaf.
+            If provided, then *digest* should not be provided.
+    :type record: str or bytes
+    :param digest: [optional] The checksum to be stored by the leaf.
+                If provided, then *record* should not be provided.
+    :type digest: str
 
+    :raises LeafConstructionError: if both *record* and *digest* were
+        provided
+    """
 
-    def __str__(self, indent=2, trim=8):
-        """
-        :returns: visual representation of the tree
-        :rtype: str
-        """
-        if not self.root:
-            return '\n └─[None]\n'
-
-        return self.root.expand(indent, trim) + '\n'
+    __slots__ = ('__digest',)
 
+    def __init__(self, hash_func, encoding, record=None, digest=None):
+        if digest is None and record:
+            try:
+                digest = hash_func(record)
+            except UndecodableArgumentError:
+                raise UndecodableRecord
+            else:
+                super().__init__(encoding)
+                self.__digest = digest
+        elif record is None and digest:
+            super().__init__(encoding)
+            self.__digest = bytes(digest, encoding)
+        else:
+            err = 'Either record or digest may be provided'
+            raise LeafConstructionError(err)
 
-    def _encode_leaf(self, entry):
+    @property
+    def digest(self):
         """
-        Returns the binary format of the provided entry
+        The checksum currently stored by the leaf.
 
-        :param entry: data to encode
-        :type entry: bytes
         :rtype: bytes
         """
-        return entry
-
+        return self.__digest
 
-    def _store_leaf(self, entry, value):
+    def serialize(self):
         """
-        Creates a new leaf storing the provided entry along with its binary
-        format and corresponding hash value
+        Returns a JSON entity with the leaf's characteristics as key-value pairs.
 
-        :param entry: data to append
-        :type entry: whatever expected according to application logic
-        :param value: hashed data
-        :type value: bytes
-        :returns: index of newly appended leaf counting from one
-        :rtype: int
+        :rtype: dict
         """
-        tail = Leaf(entry, value)
-
-        if not self.leaves:
-            self.leaves += [tail]
-            self.root = tail
-            return 1
+        return LeafSerializer().default(self)
 
-        node = self.get_last_maximal_perfect_node()
-        self.leaves += [tail]
-        value = self.hash_nodes(node.value, tail.value)
 
-        if node.is_root():
-            self.root = Node(value, node, tail)
-            index = self.get_size()
-            return index
-
-        curr = node.parent
-        curr.right = Node(value, node, tail)
-        curr.right.parent = curr
-        while curr:
-            curr.value = self.hash_nodes(
-                curr.left.value, curr.right.value)
-            curr = curr.parent
-
-        index = self.get_size()
-        return index
-
-
-    def _get_leaf(self, index):
+    def toJSONString(self):
         """
-        Returns the hash stored by the leaf specified
+        Returns a JSON text with the leaf's characteristics as key-value pairs.
 
-        :param index: leaf index counting from one
-        :type index: int
-        :rtype: bytes
+        :rtype: str
         """
-        if index < 1 or index > len(self.leaves):
-            raise ValueError("%d not in leaf range" % index)
-
-        return self.leaves[index - 1].value
+        return json.dumps(self, cls=LeafSerializer, sort_keys=True, indent=4)
 
 
-    def _get_size(self):
-        """
-        :returns: current number of leaves
-        :rtype: int
-        """
-        return len(self.leaves)
-
+class Node(__Node):
+    """
+    Class for Merkle-tree's internal nodes
 
-    @classmethod
-    def init_from_entries(cls, entries, algorithm='sha256', security=True):
-        """
-        Create tree from initial data
+    By internal is meant a node with exactly two parents.
 
-        :param entries: initial data to append
-        :type entries: iterable of bytes
-        :param algorithm: [optional] hash function. Defaults to *sha256*
-        :type algorithm: str
-        :param security: [optional] resistance against second-preimage attack.
-            Defaults to *True*
-        :type security: bool
-        """
-        tree = cls(algorithm, security)
+    :param hash_func: hash function to be used for encryption
+    :type hash_func: method
+    :param encoding: encoding type to be used when decoding the digest
+            stored by the node
+    :type encoding: str
+    :param left: [optional] the node's left parent
+    :type left: __Node
+    :param right: [optional] the node's right parent
+    :type right: __Node
+    """
 
-        append = tree.append
-        for entry in entries:
-            append(entry)
+    __slots__ = ('__digest', '__left', '__right',)
 
-        return tree
+    def __init__(self, hash_func, encoding, left, right):
+        super().__init__(encoding=encoding)
 
+        digest = hash_func(left.digest, right.digest)
+        self.__digest = digest
+        self.__left   = left
+        self.__right  = right
+        left.__child  = self
+        right.__child = self
 
-    def get_state(self, subsize=None):
+    @property
+    def digest(self):
         """
-        Computes the root-hash of the subtree corresponding to the provided
-        size
-
-        .. note:: Overrides the default implementation inherited from the base
-            class
+        The checksum currently stored by the node.
 
-        :param subsize: [optional] number of leaves to consider. Defaults to
-            current tree size
-        :type subsize: int
         :rtype: bytes
         """
-        if subsize is None:
-            subsize = self.get_size()
-
-        if subsize == 0:
-            return self.consume(b'')
-
-        if subsize == self.get_size():
-            return self.root.value
-
-        principals = self.get_principal_nodes(subsize)
-        result = principals[0].value
-        i = 0
-        while i < len(principals) - 1:
-            result = self.hash_nodes(principals[i + 1].value, result)
-            i += 1
-
-        return result
-
+        return self.__digest
 
-    def inclusion_path_fallback(self, offset):
+    def set_right(self, right):
         """
-        Non-recursive utility using concrete traversals to compute the inclusion
-        path of the provided leaf hash against the current tree state
+        Sets the node's right parent.
 
-        .. warning:: This method is intended for investigating the tree
-            structure and testing. Use ``prove_inclusion`` to properly generate
-            inclusion proofs
-
-        :param offset: base leaf index counting from zero
-        :type offset: int
-        :rtype: (list[int], list[bytes])
+        :param right: the new right parent
+        :type: __Node
         """
-        base = self.leaves[offset]
-        bit = 1 if base.is_right_child() else 0
-
-        path = [base.value]
-        rule = [bit]
-
-        curr = base
-        while curr.parent:
-            parent = curr.parent
-
-            if curr.is_left_child():
-                value = parent.right.value
-                bit = 0 if parent.is_left_child() else 1
-            else:
-                value = parent.left.value
-                bit = 1 if parent.is_right_child() else 0
-
-            rule += [bit]
-            path += [value]
-            curr = parent
+        self.__right = right
 
-        # Last bit is insignificant; fix it to zero just to be fully compatible
-        # with the output of the overriden method
-        rule[-1] = 0
-
-        return rule, path
-
-
-    def inclusion_path(self, start, offset, end, bit):
+    def recalculate_hash(self, hash_func):
         """
-        Computes the inclusion path for the leaf located at the provided offset
-        against the specified leaf range
-
-        .. warning:: This method should not be called directly. Use
-            ``prove_inclusion`` instead
+        Recalculates the node's digest under account of the (possibly new)
+        digests stored by its parents.
 
-        :param start: leftmost leaf index counting from zero
-        :type start: int
-        :param offset: base leaf index counting from zero
-        :type offset: int
-        :param end: rightmost leaf index counting from zero
-        :type end: int
-        :param bit: bit indicating direction during recursive call
-        :type bit: int
-        :rtype: (list[int], list[bytes])
+        :param hash_func: hash function to be used for recalculation
+        :type hash_func: method
         """
-        if start == 0 and end == self.get_size():
-            return self.inclusion_path_fallback(offset)
+        self.__digest = hash_func(self.left.digest, self.right.digest)
 
-        return super().inclusion_path(start, offset, end, bit)
 
-
-    def get_perfect_node(self, index, height):
+    def serialize(self):
         """
-        Returns the root node of the perfect subtree of the provided height whose
-        leftmost leaf node is located at the provided position
+        Returns a JSON entity with the node's characteristics as key-value pairs.
 
-        .. note:: Returns *None* if no binary subtree exists for the provided
-            parameters
+        :rtype: dict
 
-        :param index: position of leftmost leaf node coutning from one
-        :type index: int
-        :param height: height of requested subtree
-        :type height: int
-        :rtype: Node
+        .. note:: The *.child* attribute is ommited from node serialization
+            in order for circular reference error to be avoided.
         """
-        node = self.leaves[index - 1]
-
-        if not node:
-            return
-
-        i = 0
-        while i < height:
-            curr = node.parent
-
-            if not curr:
-                return
-
-            if curr.left is not node:
-                return
-
-            node = curr
-            i += 1
-
-        # Verify existence of perfect subtree rooted at the detected node
-        curr = node
-        i = 0
-        while i < height:
-            if curr.is_leaf():
-                return
-
-            curr = curr.right
-            i += 1
-
-        return node
+        return NodeSerializer().default(self)
 
-
-    def get_last_maximal_perfect_node(self):
-        """
-        Returns the root-node of the perfect subtree of maximum possible size
-        containing the currently last leaf
-
-        :rtype: Node
-        """
-        degree = decompose(len(self.leaves))[0]
-
-        return self.leaves[-1].get_ancestor(degree)
-
-
-    def get_principal_nodes(self, subsize):
+    def toJSONString(self):
         """
-        Returns in respective order the root-nodes of the successive perfect
-        subtrees whose sizes sum up to the provided size
+        Returns a JSON text with the node's characteristics as key-value pairs.
 
-        :param subsize:
-        :type subsize: int
-        :rtype: list[Node]
+        :rtype: str
         """
-        if subsize < 0 or subsize > self.get_size():
-            return []
-
-        principals = []
-        offset = 0
-        for height in reversed(decompose(subsize)):
-            node = self.get_perfect_node(offset + 1, height)
-
-            if not node:
-                return []
-
-            principals += [node]
-            offset += 1 << height
-
-        return list(reversed(principals))
+        return json.dumps(self, cls=NodeSerializer, sort_keys=True, indent=4)
```

### Comparing `pymerkle-5.0.3/setup.py` & `pymerkle-5.0.3b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,50 +4,49 @@
 from setuptools import setup, find_packages
 import os
 import io
 
 import pymerkle
 
 
-URL = "https://github.com/fmerg/pymerkle"
+URL = "https://github.com/FoteinosMerg/pymerkle"
 
 current_dir = os.path.abspath(os.path.dirname(__file__))
 
 try:
-  with io.open(os.path.join(current_dir, "requirements.txt"),
-    encoding="utf-8") as f:
-    install_requires = [_.strip() for _ in f.readlines()]
+  with io.open(os.path.join(current_dir, "requirements.txt"), encoding="utf-8") as __file:
+    install_requires = [_.strip() for _ in __file.readlines()]
 except FileNotFoundError:
-    install_requires = []
+    install_requires = ["tqdm>=4.28.1",]
 
-with open("README.md", 'r') as f:
-    long_description = f.read()
+with open("README.md", 'r') as __file:
+    long_description = __file.read()
 
 def main():
     setup(
        name=pymerkle.__name__,
        version=pymerkle.__version__,
        description=pymerkle.__doc__.strip(),
        long_description=long_description,
        long_description_content_type='text/markdown',
-       packages=find_packages(exclude=['tests']),
-       # package_dir={'': 'pymerkle'},
+       packages=find_packages("pymerkle"),
+       package_dir={'': 'pymerkle'},
        url=URL,
        project_urls={
             "github": URL,
             "source": "%s/%s" % (URL, "tree/master/%s" % pymerkle.__name__),
             "docs": "https://%s.readthedocs.io/en/latest/" % pymerkle.__name__,
        },
-       author="fmerg",
-       author_email="fmerg@protonmail.com",
+       author="FoteinosMerg",
+       author_email="foteinosmerg@protonmail.com",
        python_requires=">=3.6",
        install_requires=install_requires,
        zip_safe=False,
        keywords=[
-           "merkle", "proof", "inclusion", "consistency",
+           "merkle", "proof", "audit", "consistency",
        ],
        classifiers=[
            "Development Status :: 4 - Beta",
            "Intended Audience :: Developers",
            "Intended Audience :: Science/Research",
            "Programming Language :: Python :: 3.6",
            "Operating System :: POSIX",
```

