# Comparing `tmp/relyonai-0.1.1.tar.gz` & `tmp/relyonai-0.1.2.tar.gz`

## Comparing `relyonai-0.1.1.tar` & `relyonai-0.1.2.tar`

### file list

```diff
@@ -1,1603 +1,1603 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 relyonai-0.1.1/Makefile
--rw-r--r--   0        0        0   223622 2020-02-02 00:00:00.000000 relyonai-0.1.1/showcase.png
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/@plugins_snapshot.json
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/__future__.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/__future__.meta.json
--rw-r--r--   0        0        0   111641 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_ast.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_ast.meta.json
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_bisect.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_bisect.meta.json
--rw-r--r--   0        0        0    51709 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_codecs.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_codecs.meta.json
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_collections_abc.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_collections_abc.meta.json
--rw-r--r--   0        0        0    19643 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_csv.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_csv.meta.json
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_ctypes.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_ctypes.meta.json
--rw-r--r--   0        0        0   211936 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_curses.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_curses.meta.json
--rw-r--r--   0        0        0   170347 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_decimal.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_decimal.meta.json
--rw-r--r--   0        0        0   111349 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_operator.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_operator.meta.json
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_random.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_random.meta.json
--rw-r--r--   0        0        0    88273 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_socket.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_socket.meta.json
--rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_stat.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_stat.meta.json
--rw-r--r--   0        0        0    22782 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_thread.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_thread.meta.json
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_tracemalloc.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_tracemalloc.meta.json
--rw-r--r--   0        0        0    13080 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_warnings.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_warnings.meta.json
--rw-r--r--   0        0        0    26187 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_weakref.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_weakref.meta.json
--rw-r--r--   0        0        0    49319 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_weakrefset.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_weakrefset.meta.json
--rw-r--r--   0        0        0    22313 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/abc.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/abc.meta.json
--rw-r--r--   0        0        0   145984 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/argparse.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/argparse.meta.json
--rw-r--r--   0        0        0    62446 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/array.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/array.meta.json
--rw-r--r--   0        0        0   124316 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/ast.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/ast.meta.json
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/atexit.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/atexit.meta.json
--rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/base64.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/base64.meta.json
--rw-r--r--   0        0        0    49254 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/bdb.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/bdb.meta.json
--rw-r--r--   0        0        0    14061 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/binascii.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/binascii.meta.json
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/bisect.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/bisect.meta.json
--rw-r--r--   0        0        0  1002205 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/builtins.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/builtins.meta.json
--rw-r--r--   0        0        0    20266 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/cmd.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/cmd.meta.json
--rw-r--r--   0        0        0   123219 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/codecs.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/codecs.meta.json
--rw-r--r--   0        0        0   124143 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/configparser.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/configparser.meta.json
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/conftest.data.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/conftest.meta.json
--rw-r--r--   0        0        0    92076 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/contextlib.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/contextlib.meta.json
--rw-r--r--   0        0        0    35653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/contextvars.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/contextvars.meta.json
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/copy.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/copy.meta.json
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/copyreg.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/copyreg.meta.json
--rw-r--r--   0        0        0    29661 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/csv.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/csv.meta.json
--rw-r--r--   0        0        0    51547 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/dataclasses.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/dataclasses.meta.json
--rw-r--r--   0        0        0   127876 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/datetime.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/datetime.meta.json
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/decimal.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/decimal.meta.json
--rw-r--r--   0        0        0    56438 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/difflib.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/difflib.meta.json
--rw-r--r--   0        0        0    39405 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/dis.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/dis.meta.json
--rw-r--r--   0        0        0    69288 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/doctest.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/doctest.meta.json
--rw-r--r--   0        0        0    60742 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/enum.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/enum.meta.json
--rw-r--r--   0        0        0    19385 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/errno.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/errno.meta.json
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/fnmatch.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/fnmatch.meta.json
--rw-r--r--   0        0        0    92293 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/fractions.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/fractions.meta.json
--rw-r--r--   0        0        0   126780 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/functools.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/functools.meta.json
--rw-r--r--   0        0        0    15324 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/gc.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/gc.meta.json
--rw-r--r--   0        0        0    22401 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/genericpath.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/genericpath.meta.json
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/getpass.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/getpass.meta.json
--rw-r--r--   0        0        0    53393 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/gettext.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/gettext.meta.json
--rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/glob.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/glob.meta.json
--rw-r--r--   0        0        0    27021 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/hashlib.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/hashlib.meta.json
--rw-r--r--   0        0        0   334703 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/inspect.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/inspect.meta.json
--rw-r--r--   0        0        0    85350 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/io.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/io.meta.json
--rw-r--r--   0        0        0   259435 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/itertools.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/itertools.meta.json
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/keyword.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/keyword.meta.json
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/marshal.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/marshal.meta.json
--rw-r--r--   0        0        0    49415 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/math.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/math.meta.json
--rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/mimetypes.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/mimetypes.meta.json
--rw-r--r--   0        0        0    26427 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/mmap.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/mmap.meta.json
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/netrc.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/netrc.meta.json
--rw-r--r--   0        0        0    78984 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numbers.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numbers.meta.json
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/opcode.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/opcode.meta.json
--rw-r--r--   0        0        0    46574 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/operator.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/operator.meta.json
--rw-r--r--   0        0        0    83681 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pathlib.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pathlib.meta.json
--rw-r--r--   0        0        0    93344 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pdb.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pdb.meta.json
--rw-r--r--   0        0        0    44406 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pickle.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pickle.meta.json
--rw-r--r--   0        0        0    30187 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pkgutil.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pkgutil.meta.json
--rw-r--r--   0        0        0    33444 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/platform.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/platform.meta.json
--rw-r--r--   0        0        0    75080 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/posixpath.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/posixpath.meta.json
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pprint.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pprint.meta.json
--rw-r--r--   0        0        0   103495 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pydoc.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pydoc.meta.json
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/queue.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/queue.meta.json
--rw-r--r--   0        0        0    39655 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/random.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/random.meta.json
--rw-r--r--   0        0        0   165070 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/re.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/re.meta.json
--rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/reprlib.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/reprlib.meta.json
--rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/select.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/select.meta.json
--rw-r--r--   0        0        0    54878 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/selectors.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/selectors.meta.json
--rw-r--r--   0        0        0    16509 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/shlex.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/shlex.meta.json
--rw-r--r--   0        0        0    70356 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/shutil.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/shutil.meta.json
--rw-r--r--   0        0        0    31620 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/signal.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/signal.meta.json
--rw-r--r--   0        0        0    77705 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/socket.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/socket.meta.json
--rw-r--r--   0        0        0    58033 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/socketserver.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/socketserver.meta.json
--rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sre_compile.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sre_compile.meta.json
--rw-r--r--   0        0        0    28015 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sre_constants.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sre_constants.meta.json
--rw-r--r--   0        0        0    49455 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sre_parse.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sre_parse.meta.json
--rw-r--r--   0        0        0   188211 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/ssl.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/ssl.meta.json
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/stat.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/stat.meta.json
--rw-r--r--   0        0        0    28134 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/string.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/string.meta.json
--rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/struct.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/struct.meta.json
--rw-r--r--   0        0        0   137954 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/subprocess.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/subprocess.meta.json
--rw-r--r--   0        0        0   145382 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sys.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sys.meta.json
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sysconfig.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sysconfig.meta.json
--rw-r--r--   0        0        0   133938 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tempfile.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tempfile.meta.json
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_ai.data.json
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_ai.meta.json
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_args.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_args.meta.json
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_consts.data.json
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_consts.meta.json
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_files.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_files.meta.json
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_funcs.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_funcs.meta.json
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_gpt.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_gpt.meta.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_igpt.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_igpt.meta.json
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_imports.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/test_imports.meta.json
--rw-r--r--   0        0        0    19555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/textwrap.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/textwrap.meta.json
--rw-r--r--   0        0        0    63952 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/threading.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/threading.meta.json
--rw-r--r--   0        0        0    41028 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/time.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/time.meta.json
--rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/token.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/token.meta.json
--rw-r--r--   0        0        0    48440 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tokenize.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tokenize.meta.json
--rw-r--r--   0        0        0    46133 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traceback.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traceback.meta.json
--rw-r--r--   0        0        0    47456 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tracemalloc.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tracemalloc.meta.json
--rw-r--r--   0        0        0   205398 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/types.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/types.meta.json
--rw-r--r--   0        0        0   392815 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/typing.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/typing.meta.json
--rw-r--r--   0        0        0    70277 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/typing_extensions.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/typing_extensions.meta.json
--rw-r--r--   0        0        0    42225 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unicodedata.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unicodedata.meta.json
--rw-r--r--   0        0        0    33636 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/uuid.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/uuid.meta.json
--rw-r--r--   0        0        0    22158 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/warnings.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/warnings.meta.json
--rw-r--r--   0        0        0   111375 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/weakref.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/weakref.meta.json
--rw-r--r--   0        0        0    68197 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/zipfile.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/zipfile.meta.json
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/zipimport.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/zipimport.meta.json
--rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/zlib.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/zlib.meta.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_version.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_version.meta.json
--rw-r--r--   0        0        0    41440 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   158288 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/capture.data.json
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/capture.meta.json
--rw-r--r--   0        0        0    24432 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/compat.data.json
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/compat.meta.json
--rw-r--r--   0        0        0    30451 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0    49551 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/doctest.data.json
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/doctest.meta.json
--rw-r--r--   0        0        0   146234 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    56847 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    60447 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    74402 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/logging.data.json
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/logging.meta.json
--rw-r--r--   0        0        0    44515 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/main.data.json
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/main.meta.json
--rw-r--r--   0        0        0    24892 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    55864 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/nodes.data.json
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   128637 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   110800 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/python.data.json
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/python.meta.json
--rw-r--r--   0        0        0    49915 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/python_api.data.json
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    29598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    49418 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/reports.data.json
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/reports.meta.json
--rw-r--r--   0        0        0    38342 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/runner.data.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/scope.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/scope.meta.json
--rw-r--r--   0        0        0    13836 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/stash.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/stash.meta.json
--rw-r--r--   0        0        0    90377 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/timing.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/timing.meta.json
--rw-r--r--   0        0        0    21112 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    25827 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/warnings.data.json
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/warnings.meta.json
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   154497 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    18059 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    15772 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    58844 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    22262 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0    97039 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    39844 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    22270 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    29097 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   107269 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0    90306 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/__init__.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/__init__.meta.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/_helpers.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/_helpers.meta.json
--rw-r--r--   0        0        0    54933 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/abc.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/abc.meta.json
--rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/base_protocol.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/base_protocol.meta.json
--rw-r--r--   0        0        0   114110 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client.data.json
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client.meta.json
--rw-r--r--   0        0        0    60919 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_exceptions.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_exceptions.meta.json
--rw-r--r--   0        0        0    20514 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_proto.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_proto.meta.json
--rw-r--r--   0        0        0   134406 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_reqrep.data.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_reqrep.meta.json
--rw-r--r--   0        0        0    35159 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_ws.data.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_ws.meta.json
--rw-r--r--   0        0        0   101185 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/connector.data.json
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/connector.meta.json
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/cookiejar.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/cookiejar.meta.json
--rw-r--r--   0        0        0    11434 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/formdata.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/formdata.meta.json
--rw-r--r--   0        0        0    21353 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/hdrs.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/hdrs.meta.json
--rw-r--r--   0        0        0   129839 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/helpers.data.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/helpers.meta.json
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http.meta.json
--rw-r--r--   0        0        0    19942 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_exceptions.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_exceptions.meta.json
--rw-r--r--   0        0        0   108296 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_parser.data.json
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_parser.meta.json
--rw-r--r--   0        0        0    75626 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_websocket.data.json
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_websocket.meta.json
--rw-r--r--   0        0        0    33316 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_writer.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_writer.meta.json
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/locks.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/locks.meta.json
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/log.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/log.meta.json
--rw-r--r--   0        0        0    81476 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/multipart.data.json
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/multipart.meta.json
--rw-r--r--   0        0        0    58649 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload.data.json
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload.meta.json
--rw-r--r--   0        0        0    15753 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload_streamer.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload_streamer.meta.json
--rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/resolver.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/resolver.meta.json
--rw-r--r--   0        0        0    72323 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/streams.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/streams.meta.json
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tcp_helpers.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tcp_helpers.meta.json
--rw-r--r--   0        0        0   216782 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tracing.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tracing.meta.json
--rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/typedefs.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/typedefs.meta.json
--rw-r--r--   0        0        0    25449 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web.data.json
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web.meta.json
--rw-r--r--   0        0        0    63171 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_app.data.json
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_app.meta.json
--rw-r--r--   0        0        0    92924 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_exceptions.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_exceptions.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_fileresponse.data.json
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_fileresponse.meta.json
--rw-r--r--   0        0        0    41534 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_log.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_log.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_middlewares.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_middlewares.meta.json
--rw-r--r--   0        0        0    49073 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_protocol.data.json
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_protocol.meta.json
--rw-r--r--   0        0        0    93980 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_request.data.json
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_request.meta.json
--rw-r--r--   0        0        0    82826 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_response.data.json
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_response.meta.json
--rw-r--r--   0        0        0    57693 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_routedef.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_routedef.meta.json
--rw-r--r--   0        0        0    58927 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_runner.data.json
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_runner.meta.json
--rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_server.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_server.meta.json
--rw-r--r--   0        0        0   180562 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_urldispatcher.data.json
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_urldispatcher.meta.json
--rw-r--r--   0        0        0    52501 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_ws.data.json
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_ws.meta.json
--rw-r--r--   0        0        0    19267 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/worker.data.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiohttp/worker.meta.json
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiosignal/__init__.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/aiosignal/__init__.meta.json
--rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/async_timeout/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/async_timeout/__init__.meta.json
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/__init__.meta.json
--rw-r--r--   0        0        0    98750 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    25243 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   188237 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/events.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/events.meta.json
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    35534 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/futures.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/futures.meta.json
--rw-r--r--   0        0        0    31660 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/locks.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/locks.meta.json
--rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    22078 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/queues.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/queues.meta.json
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/runners.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    35291 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/streams.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0   106509 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/tasks.meta.json
--rw-r--r--   0        0        0    27488 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/transports.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/transports.meta.json
--rw-r--r--   0        0        0    51737 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0   210184 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/__init__.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/__init__.meta.json
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/_cmp.data.json
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/_cmp.meta.json
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/_typing_compat.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/_typing_compat.meta.json
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/_version_info.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/_version_info.meta.json
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/converters.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/converters.meta.json
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/exceptions.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/exceptions.meta.json
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/filters.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/filters.meta.json
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/setters.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/setters.meta.json
--rw-r--r--   0        0        0    42073 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/validators.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/attr/validators.meta.json
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/__init__.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/__init__.meta.json
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/api.data.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/api.meta.json
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/cd.data.json
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/cd.meta.json
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/constant.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/constant.meta.json
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/legacy.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/legacy.meta.json
--rw-r--r--   0        0        0    59341 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/md.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/md.meta.json
--rw-r--r--   0        0        0    50507 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/models.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/models.meta.json
--rw-r--r--   0        0        0    28046 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/utils.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/utils.meta.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/version.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/version.meta.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/assets/__init__.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/assets/__init__.meta.json
--rw-r--r--   0        0        0   367796 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/collections/__init__.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/collections/__init__.meta.json
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/collections/abc.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/collections/abc.meta.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    70910 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    20711 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   126917 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    34692 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/curses/__init__.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/curses/__init__.meta.json
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/__init__.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/__init__.meta.json
--rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/charset.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/charset.meta.json
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/contentmanager.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/errors.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/errors.meta.json
--rw-r--r--   0        0        0    17249 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/feedparser.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/feedparser.meta.json
--rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/header.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/header.meta.json
--rw-r--r--   0        0        0    79294 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/message.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/message.meta.json
--rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/parser.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/parser.meta.json
--rw-r--r--   0        0        0    30859 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/policy.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/policy.meta.json
--rw-r--r--   0        0        0    20503 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/utils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/email/utils.meta.json
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/__init__.meta.json
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_catch.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_catch.meta.json
--rw-r--r--   0        0        0    66814 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_exceptions.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_exceptions.meta.json
--rw-r--r--   0        0        0    21945 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_formatting.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_formatting.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_version.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_version.meta.json
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/frozenlist/__init__.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/frozenlist/__init__.meta.json
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/html/__init__.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/html/__init__.meta.json
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/html/entities.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/html/entities.meta.json
--rw-r--r--   0        0        0    18711 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/__init__.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/__init__.meta.json
--rw-r--r--   0        0        0    66298 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/client.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/client.meta.json
--rw-r--r--   0        0        0    58156 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/cookiejar.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/cookiejar.meta.json
--rw-r--r--   0        0        0    38912 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/cookies.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/cookies.meta.json
--rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/server.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/http/server.meta.json
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/__init__.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/__init__.meta.json
--rw-r--r--   0        0        0    41053 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/abc.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/abc.meta.json
--rw-r--r--   0        0        0    65333 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/machinery.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/util.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/util.meta.json
--rw-r--r--   0        0        0    64663 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    93642 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    22217 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    22663 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    44366 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0    21926 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/iniconfig/_parse.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/iniconfig/_parse.meta.json
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/iniconfig/exceptions.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/iniconfig/exceptions.meta.json
--rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/__init__.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/__init__.meta.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/_identifier.data.json
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/_identifier.meta.json
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/async_utils.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/async_utils.meta.json
--rw-r--r--   0        0        0    26219 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/bccache.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/bccache.meta.json
--rw-r--r--   0        0        0   155139 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/compiler.data.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/compiler.meta.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/constants.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/constants.meta.json
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/debug.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/debug.meta.json
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/defaults.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/defaults.meta.json
--rw-r--r--   0        0        0   116065 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/environment.data.json
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/environment.meta.json
--rw-r--r--   0        0        0    17712 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/exceptions.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/exceptions.meta.json
--rw-r--r--   0        0        0    49856 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/ext.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/ext.meta.json
--rw-r--r--   0        0        0   149382 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/filters.data.json
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/filters.meta.json
--rw-r--r--   0        0        0    42314 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/idtracking.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/idtracking.meta.json
--rw-r--r--   0        0        0    88022 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/lexer.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/lexer.meta.json
--rw-r--r--   0        0        0    47837 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/loaders.data.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/loaders.meta.json
--rw-r--r--   0        0        0   146988 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/nodes.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/nodes.meta.json
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/optimizer.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/optimizer.meta.json
--rw-r--r--   0        0        0    47362 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/parser.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/parser.meta.json
--rw-r--r--   0        0        0   148084 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/runtime.data.json
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/runtime.meta.json
--rw-r--r--   0        0        0    32271 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/sandbox.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/sandbox.meta.json
--rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/tests.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/tests.meta.json
--rw-r--r--   0        0        0    61362 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/utils.data.json
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/utils.meta.json
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/visitor.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/jinja2/visitor.meta.json
--rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/json/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/json/__init__.meta.json
--rw-r--r--   0        0        0    14506 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/json/decoder.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/json/decoder.meta.json
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/json/encoder.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/json/encoder.meta.json
--rw-r--r--   0        0        0   140127 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/logging/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/logging/__init__.meta.json
--rw-r--r--   0        0        0    14100 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/logging/config.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/logging/config.meta.json
--rw-r--r--   0        0        0    74406 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/logging/handlers.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/logging/handlers.meta.json
--rw-r--r--   0        0        0    34443 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/markupsafe/__init__.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/markupsafe/__init__.meta.json
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_native.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_native.meta.json
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_speedups.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_speedups.meta.json
--rw-r--r--   0        0        0   133573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multidict/__init__.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multidict/__init__.meta.json
--rw-r--r--   0        0        0    31384 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30665 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95606 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   146899 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    50247 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17688 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    17677 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28883 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    28132 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67379 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25560 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23554 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/util.meta.json
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/__init__.data.json
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/__init__.meta.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/_imports.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/_imports.meta.json
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/_struct.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/_struct.meta.json
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/_version.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/_version.meta.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/converter.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/converter.meta.json
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/json_compat.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/json_compat.meta.json
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/notebooknode.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/notebooknode.meta.json
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/reader.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/reader.meta.json
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/sentinel.data.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/sentinel.meta.json
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/validator.data.json
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/validator.meta.json
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/warnings.data.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/warnings.meta.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/__init__.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/__init__.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/words.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/words.meta.json
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/__init__.meta.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/convert.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/convert.meta.json
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbbase.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbbase.meta.json
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbjson.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbjson.meta.json
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/rwbase.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/rwbase.meta.json
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/__init__.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/__init__.meta.json
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/convert.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/convert.meta.json
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbbase.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbbase.meta.json
--rw-r--r--   0        0        0     9806 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbjson.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbjson.meta.json
--rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbpy.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbpy.meta.json
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbxml.data.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbxml.meta.json
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/rwbase.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/rwbase.meta.json
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/__init__.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/__init__.meta.json
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/convert.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/convert.meta.json
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbbase.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbbase.meta.json
--rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbjson.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbjson.meta.json
--rw-r--r--   0        0        0    10991 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbpy.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbpy.meta.json
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/rwbase.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/rwbase.meta.json
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/__init__.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/__init__.meta.json
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/convert.data.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/convert.meta.json
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbbase.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbbase.meta.json
--rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbjson.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbjson.meta.json
--rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/rwbase.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/rwbase.meta.json
--rw-r--r--   0        0        0  2216519 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/__init__.data.json
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_version.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_version.meta.json
--rw-r--r--   0        0        0   112501 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/version.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/version.meta.json
--rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25394 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   260468 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41708 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30688 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    33297 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16755 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261349 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13641 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21869 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169656 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36045 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330685 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49546 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301742 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196438 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    45650 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    24433 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52611 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/records.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52744 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21709 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    24000 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    18058 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   154533 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    25919 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   223847 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    63614 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    47359 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    89078 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    96612 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    96739 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    62213 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    89041 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    23493 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    76988 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    97310 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    24846 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26118 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107773 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27663 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136748 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    26985 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16462 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14238 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   253014 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     8966 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    66834 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323845 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114195 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/__init__.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/__init__.meta.json
--rw-r--r--   0        0        0    63039 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_requestor.data.json
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_requestor.meta.json
--rw-r--r--   0        0        0    17891 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/error.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/error.meta.json
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/object_classes.data.json
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/object_classes.meta.json
--rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/openai_object.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/openai_object.meta.json
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/openai_response.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/openai_response.meta.json
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/util.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/util.meta.json
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/version.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/version.meta.json
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/__init__.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/__init__.meta.json
--rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/audio.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/audio.meta.json
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/chat_completion.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/chat_completion.meta.json
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/completion.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/completion.meta.json
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/customer.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/customer.meta.json
--rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/deployment.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/deployment.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/edit.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/edit.meta.json
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/embedding.data.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/embedding.meta.json
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/engine.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/engine.meta.json
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/error_object.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/error_object.meta.json
--rw-r--r--   0        0        0    20017 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/file.data.json
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/file.meta.json
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/fine_tune.data.json
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/fine_tune.meta.json
--rw-r--r--   0        0        0    18573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/image.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/image.meta.json
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/model.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/model.meta.json
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/moderation.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/moderation.meta.json
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/__init__.data.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/__init__.meta.json
--rw-r--r--   0        0        0    15484 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.meta.json
--rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.meta.json
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.meta.json
--rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.data.json
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.meta.json
--rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.meta.json
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.meta.json
--rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.meta.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/__init__.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/__init__.meta.json
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.meta.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/__init__.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/__init__.meta.json
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/common.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/common.meta.json
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/numpy_helper.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/numpy_helper.meta.json
--rw-r--r--   0        0        0   302162 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/os/__init__.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/os/__init__.meta.json
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/os/path.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/os/path.meta.json
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/__init__.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/__init__.meta.json
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    26006 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    43260 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_parser.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_parser.meta.json
--rw-r--r--   0        0        0    13942 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_structures.data.json
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_structures.meta.json
--rw-r--r--   0        0        0    16957 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_tokenizer.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/_tokenizer.meta.json
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/markers.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/markers.meta.json
--rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/requirements.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/requirements.meta.json
--rw-r--r--   0        0        0    55965 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    27782 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/tags.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/tags.meta.json
--rw-r--r--   0        0        0     9823 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/utils.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/utils.meta.json
--rw-r--r--   0        0        0    64770 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/version.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/packaging/version.meta.json
--rw-r--r--   0        0        0    13421 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/__init__.data.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/__init__.meta.json
--rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_typing.data.json
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_typing.meta.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/testing.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/testing.meta.json
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/__init__.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/__init__.meta.json
--rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/config.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/config.meta.json
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/__init__.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/__init__.meta.json
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/indexing.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/indexing.meta.json
--rw-r--r--   0        0        0   175917 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/interval.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/interval.meta.json
--rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/lib.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/lib.meta.json
--rw-r--r--   0        0        0    31716 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/missing.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/missing.meta.json
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/ops_dispatch.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/ops_dispatch.meta.json
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/properties.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/properties.meta.json
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.meta.json
--rw-r--r--   0        0        0    58549 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.meta.json
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.meta.json
--rw-r--r--   0        0        0   125179 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.data.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.meta.json
--rw-r--r--   0        0        0    92308 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/period.data.json
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/period.meta.json
--rw-r--r--   0        0        0   189107 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.data.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.meta.json
--rw-r--r--   0        0        0   148757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.data.json
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.meta.json
--rw-r--r--   0        0        0    30667 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_testing/__init__.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/_testing/__init__.meta.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/__init__.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/extensions/__init__.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/extensions/__init__.meta.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/indexers/__init__.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/indexers/__init__.meta.json
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/types/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/api/types/__init__.meta.json
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/arrays/__init__.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/arrays/__init__.meta.json
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/__init__.data.json
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/__init__.meta.json
--rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/accessor.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/accessor.meta.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/algorithms.data.json
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/algorithms.meta.json
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/api.data.json
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/api.meta.json
--rw-r--r--   0        0        0    37388 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arraylike.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arraylike.meta.json
--rw-r--r--   0        0        0    36591 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/base.data.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/base.meta.json
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/construction.data.json
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/construction.meta.json
--rw-r--r--   0        0        0   636452 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/frame.data.json
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/frame.meta.json
--rw-r--r--   0        0        0   125166 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/generic.data.json
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/generic.meta.json
--rw-r--r--   0        0        0    18184 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexers.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexers.meta.json
--rw-r--r--   0        0        0    26374 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexing.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexing.meta.json
--rw-r--r--   0        0        0    90473 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/resample.data.json
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/resample.meta.json
--rw-r--r--   0        0        0  1275803 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/series.data.json
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/series.meta.json
--rw-r--r--   0        0        0   130171 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/strings.data.json
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/strings.meta.json
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/__init__.data.json
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/__init__.meta.json
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow.data.json
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow.meta.json
--rw-r--r--   0        0        0    32987 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/base.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/base.meta.json
--rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/boolean.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/boolean.meta.json
--rw-r--r--   0        0        0   102656 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/categorical.data.json
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/categorical.meta.json
--rw-r--r--   0        0        0    39589 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimelike.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimelike.meta.json
--rw-r--r--   0        0        0    27598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimes.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimes.meta.json
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/floating.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/floating.meta.json
--rw-r--r--   0        0        0    17764 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/integer.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/integer.meta.json
--rw-r--r--   0        0        0    39144 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/interval.data.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/interval.meta.json
--rw-r--r--   0        0        0    10795 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/masked.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/masked.meta.json
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numeric.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numeric.meta.json
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numpy_.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numpy_.meta.json
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/period.data.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/period.meta.json
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/string_.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/string_.meta.json
--rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/timedeltas.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/timedeltas.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.meta.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.meta.json
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.meta.json
--rw-r--r--   0        0        0    32211 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/array.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/array.meta.json
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.meta.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/__init__.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/__init__.meta.json
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/api.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/api.meta.json
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/eval.data.json
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/eval.meta.json
--rw-r--r--   0        0        0    23567 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/expr.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/expr.meta.json
--rw-r--r--   0        0        0    44759 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/ops.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/ops.meta.json
--rw-r--r--   0        0        0    43657 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/pytables.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/pytables.meta.json
--rw-r--r--   0        0        0    11640 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/scope.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/scope.meta.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/__init__.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/__init__.meta.json
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/api.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/api.meta.json
--rw-r--r--   0        0        0    14757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/base.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/base.meta.json
--rw-r--r--   0        0        0    21491 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/common.data.json
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/common.meta.json
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/concat.data.json
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/concat.meta.json
--rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/dtypes.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/dtypes.meta.json
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/generic.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/generic.meta.json
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/inference.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/inference.meta.json
--rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/missing.data.json
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/missing.meta.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/__init__.meta.json
--rw-r--r--   0        0        0   244906 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/generic.data.json
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/generic.meta.json
--rw-r--r--   0        0        0    59210 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/groupby.data.json
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/groupby.meta.json
--rw-r--r--   0        0        0    20931 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/grouper.data.json
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/grouper.meta.json
--rw-r--r--   0        0        0    41306 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/ops.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/ops.meta.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/__init__.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/__init__.meta.json
--rw-r--r--   0        0        0   252631 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/accessors.data.json
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/accessors.meta.json
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/api.data.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/api.meta.json
--rw-r--r--   0        0        0   145199 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/base.data.json
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/base.meta.json
--rw-r--r--   0        0        0    20184 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/category.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/category.meta.json
--rw-r--r--   0        0        0    13589 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimelike.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimelike.meta.json
--rw-r--r--   0        0        0    39465 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimes.data.json
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimes.meta.json
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/extension.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/extension.meta.json
--rw-r--r--   0        0        0   201189 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/interval.data.json
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/interval.meta.json
--rw-r--r--   0        0        0    64757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/multi.data.json
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/multi.meta.json
--rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/period.data.json
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/period.meta.json
--rw-r--r--   0        0        0    33976 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/range.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/range.meta.json
--rw-r--r--   0        0        0    21832 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/timedeltas.data.json
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/timedeltas.meta.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/__init__.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/__init__.meta.json
--rw-r--r--   0        0        0    56017 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.meta.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/__init__.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/__init__.meta.json
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/api.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/api.meta.json
--rw-r--r--   0        0        0    22852 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/concat.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/concat.meta.json
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/encoding.data.json
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/encoding.meta.json
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/melt.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/melt.meta.json
--rw-r--r--   0        0        0    32377 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/merge.data.json
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/merge.meta.json
--rw-r--r--   0        0        0    40821 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/pivot.data.json
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/pivot.meta.json
--rw-r--r--   0        0        0    79005 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/tile.data.json
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/tile.meta.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/__init__.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/__init__.meta.json
--rw-r--r--   0        0        0    19799 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/datetimes.data.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/datetimes.meta.json
--rw-r--r--   0        0        0    13501 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/numeric.data.json
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/numeric.meta.json
--rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/timedeltas.data.json
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/timedeltas.meta.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/__init__.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/__init__.meta.json
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/hashing.data.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/hashing.meta.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/__init__.meta.json
--rw-r--r--   0        0        0    22703 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/ewm.data.json
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/ewm.meta.json
--rw-r--r--   0        0        0    35020 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/expanding.data.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/expanding.meta.json
--rw-r--r--   0        0        0    66448 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/rolling.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/rolling.meta.json
--rw-r--r--   0        0        0    29360 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/errors/__init__.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/errors/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/__init__.meta.json
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/api.data.json
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/api.meta.json
--rw-r--r--   0        0        0    51797 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/clipboards.data.json
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/clipboards.meta.json
--rw-r--r--   0        0        0     8436 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/common.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/common.meta.json
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/feather_format.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/feather_format.meta.json
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/gbq.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/gbq.meta.json
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/html.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/html.meta.json
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/orc.data.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/orc.meta.json
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parquet.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parquet.meta.json
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pickle.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pickle.meta.json
--rw-r--r--   0        0        0    57813 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pytables.data.json
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pytables.meta.json
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/spss.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/spss.meta.json
--rw-r--r--   0        0        0    43548 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sql.data.json
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sql.meta.json
--rw-r--r--   0        0        0    32872 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/stata.data.json
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/stata.meta.json
--rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/xml.data.json
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/xml.meta.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/__init__.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/__init__.meta.json
--rw-r--r--   0        0        0    79612 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/_base.data.json
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/_base.meta.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/__init__.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/__init__.meta.json
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/format.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/format.meta.json
--rw-r--r--   0        0        0    80709 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style.data.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style.meta.json
--rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style_render.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style_render.meta.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/__init__.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/__init__.meta.json
--rw-r--r--   0        0        0    39658 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_json.data.json
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_json.meta.json
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_normalize.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_normalize.meta.json
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_table_schema.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_table_schema.meta.json
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/__init__.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/__init__.meta.json
--rw-r--r--   0        0        0   135743 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/readers.data.json
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/readers.meta.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/__init__.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/__init__.meta.json
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas7bdat.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas7bdat.meta.json
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas_xport.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas_xport.meta.json
--rw-r--r--   0        0        0    26676 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sasreader.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sasreader.meta.json
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/__init__.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/__init__.meta.json
--rw-r--r--   0        0        0   150357 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_core.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_core.meta.json
--rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_misc.data.json
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_misc.meta.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/__init__.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/__init__.meta.json
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/api.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/api.meta.json
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/frequencies.data.json
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/frequencies.meta.json
--rw-r--r--   0        0        0    36662 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/holiday.data.json
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/holiday.meta.json
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/offsets.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/offsets.meta.json
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/__init__.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/__init__.meta.json
--rw-r--r--   0        0        0    18309 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_decorators.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_decorators.meta.json
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_print_versions.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_print_versions.meta.json
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_tester.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_tester.meta.json
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pytest/__init__.data.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/pytest/__init__.meta.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/__init__.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/__init__.meta.json
--rw-r--r--   0        0        0    16218 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/_config.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/_config.meta.json
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/ai.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/ai.meta.json
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/explain.data.json
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/explain.meta.json
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/llm.data.json
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/llm.meta.json
--rw-r--r--   0        0        0    27581 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/runtime.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/runtime.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/utils.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/utils.meta.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/__init__.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/__init__.meta.json
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples.data.json
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples.meta.json
--rw-r--r--   0        0        0    21302 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/prompt.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/prompt.meta.json
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.meta.json
--rw-r--r--   0        0        0     9569 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sqlite3/__init__.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sqlite3/__init__.meta.json
--rw-r--r--   0        0        0   122692 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sqlite3/dbapi2.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/sqlite3/dbapi2.meta.json
--rw-r--r--   0        0        0    78723 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/__init__.data.json
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/__init__.meta.json
--rw-r--r--   0        0        0    13989 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/_asyncio.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/_asyncio.meta.json
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/_utils.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/_utils.meta.json
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/after.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/after.meta.json
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/before.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/before.meta.json
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/before_sleep.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/before_sleep.meta.json
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/nap.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/nap.meta.json
--rw-r--r--   0        0        0    37328 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/retry.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/retry.meta.json
--rw-r--r--   0        0        0    19083 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/stop.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/stop.meta.json
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/tornadoweb.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/tornadoweb.meta.json
--rw-r--r--   0        0        0    28054 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/wait.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tenacity/wait.meta.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/__init__.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/__init__.meta.json
--rw-r--r--   0        0        0    26693 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/core.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/core.meta.json
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/model.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/model.meta.json
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/registry.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tiktoken/registry.meta.json
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/__init__.meta.json
--rw-r--r--   0        0        0    51399 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/_parser.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/_parser.meta.json
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/_re.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/_re.meta.json
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/_types.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tomli/_types.meta.json
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/__init__.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/__init__.meta.json
--rw-r--r--   0        0        0    25418 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/concurrent.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/concurrent.meta.json
--rw-r--r--   0        0        0    30222 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/escape.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/escape.meta.json
--rw-r--r--   0        0        0    55073 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/gen.data.json
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/gen.meta.json
--rw-r--r--   0        0        0    66117 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/ioloop.data.json
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/ioloop.meta.json
--rw-r--r--   0        0        0    76115 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/iostream.data.json
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/iostream.meta.json
--rw-r--r--   0        0        0     9443 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/log.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/log.meta.json
--rw-r--r--   0        0        0    34372 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/netutil.data.json
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/netutil.meta.json
--rw-r--r--   0        0        0    40280 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/options.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/options.meta.json
--rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/process.data.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/process.meta.json
--rw-r--r--   0        0        0    40167 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/util.data.json
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/util.meta.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/__init__.meta.json
--rw-r--r--   0        0        0    53792 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/asyncio.data.json
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/asyncio.meta.json
--rw-r--r--   0        0        0    10750 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/__init__.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/__init__.meta.json
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/_version.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/_version.meta.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/log.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/log.meta.json
--rw-r--r--   0        0        0   169650 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/traitlets.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/traitlets.meta.json
--rw-r--r--   0        0        0     9747 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/__init__.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/__init__.meta.json
--rw-r--r--   0        0        0    52360 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/application.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/application.meta.json
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/argcomplete_config.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/argcomplete_config.meta.json
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/configurable.data.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/configurable.meta.json
--rw-r--r--   0        0        0    59589 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/loader.data.json
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/loader.meta.json
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/__init__.meta.json
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/bunch.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/bunch.meta.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/decorators.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/decorators.meta.json
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/descriptions.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/descriptions.meta.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/getargspec.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/getargspec.meta.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/importstring.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/importstring.meta.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/nested_update.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/nested_update.meta.json
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/sentinel.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/sentinel.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/text.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/text.meta.json
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/__init__.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/__init__.meta.json
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/async_case.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/async_case.meta.json
--rw-r--r--   0        0        0   224041 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/case.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/case.meta.json
--rw-r--r--   0        0        0    14631 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/loader.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/loader.meta.json
--rw-r--r--   0        0        0    11728 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/main.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/main.meta.json
--rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/result.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/result.meta.json
--rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/runner.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/runner.meta.json
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/signals.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/signals.meta.json
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/suite.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/unittest/suite.meta.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/__init__.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/__init__.meta.json
--rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/error.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/error.meta.json
--rw-r--r--   0        0        0   172181 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/parse.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/parse.meta.json
--rw-r--r--   0        0        0   152233 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/request.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/request.meta.json
--rw-r--r--   0        0        0    27167 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/response.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/urllib/response.meta.json
--rw-r--r--   0        0        0    45137 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/yarl/__init__.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 relyonai-0.1.1/.mypy_cache/3.8/yarl/__init__.meta.json
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 relyonai-0.1.1/.vscode/extensions.list
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relyonai-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 relyonai-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0   338435 2020-02-02 00:00:00.000000 relyonai-0.1.1/nbs/test.ipynb
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/__init__.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/_config.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/ai.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/explain.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/llm.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/runtime.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/utils.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/README.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/__init__.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/prompt.json
--rw-r--r--   0        0        0    10303 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/prompt.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/README.md
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/consts.ipynb
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/env.ipynb
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/error_fixing.ipynb
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/errors.ipynb
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/exploration.ipynb
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/filename.txt
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/files.ipynb
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/format.ipynb
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/funcs1.ipynb
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/funcs2.ipynb
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/funcs3.ipynb
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/gpt.ipynb
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/imports.ipynb
--rw-r--r--   0        0        0     8465 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/lambdas.ipynb
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/make_prompt.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/other.txt
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/plt.ipynb
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/run_all.sh
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/session.ipynb
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/examples/template.ipynb
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/schemas/NEW_SCHEMA.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/schemas/SCHEMA.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/schemas/SIMPLER_SCHEMA.md
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/system/default.md
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/system/gpt4-refined.md
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/system/gpt4.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/system/simpler.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 relyonai-0.1.1/relyonai/prompt/system/simpler2.md
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/test_gpt.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/multi/test_ai.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/single/test_args.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/single/test_consts.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/single/test_files.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/single/test_funcs.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/single/test_igpt.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/ai/single/test_imports.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/data/cities.csv
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 relyonai-0.1.1/tests/data/test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relyonai-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 relyonai-0.1.1/LICENSE
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 relyonai-0.1.1/README.md
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 relyonai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 relyonai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 relyonai-0.1.2/Makefile
+-rw-r--r--   0        0        0   223622 2020-02-02 00:00:00.000000 relyonai-0.1.2/showcase.png
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/__future__.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/__future__.meta.json
+-rw-r--r--   0        0        0   111641 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_ast.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_ast.meta.json
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_bisect.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_bisect.meta.json
+-rw-r--r--   0        0        0    51709 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_codecs.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_codecs.meta.json
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_collections_abc.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19643 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_csv.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_csv.meta.json
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_ctypes.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_ctypes.meta.json
+-rw-r--r--   0        0        0   211936 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_curses.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_curses.meta.json
+-rw-r--r--   0        0        0   170347 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_decimal.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_decimal.meta.json
+-rw-r--r--   0        0        0   111349 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_operator.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_operator.meta.json
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_random.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_random.meta.json
+-rw-r--r--   0        0        0    88273 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_socket.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_socket.meta.json
+-rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_stat.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_stat.meta.json
+-rw-r--r--   0        0        0    22782 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_thread.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_thread.meta.json
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_tracemalloc.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_tracemalloc.meta.json
+-rw-r--r--   0        0        0    13080 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_warnings.data.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_warnings.meta.json
+-rw-r--r--   0        0        0    26187 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_weakref.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_weakref.meta.json
+-rw-r--r--   0        0        0    49319 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_weakrefset.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_weakrefset.meta.json
+-rw-r--r--   0        0        0    22313 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/abc.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/abc.meta.json
+-rw-r--r--   0        0        0   145984 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/argparse.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/argparse.meta.json
+-rw-r--r--   0        0        0    62446 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/array.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/array.meta.json
+-rw-r--r--   0        0        0   124316 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/ast.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/ast.meta.json
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/atexit.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/atexit.meta.json
+-rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/base64.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/base64.meta.json
+-rw-r--r--   0        0        0    49254 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/bdb.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/bdb.meta.json
+-rw-r--r--   0        0        0    14061 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/binascii.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/binascii.meta.json
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/bisect.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/bisect.meta.json
+-rw-r--r--   0        0        0  1002205 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/builtins.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/builtins.meta.json
+-rw-r--r--   0        0        0    20266 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/cmd.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/cmd.meta.json
+-rw-r--r--   0        0        0   123219 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/codecs.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/codecs.meta.json
+-rw-r--r--   0        0        0   124143 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/configparser.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/configparser.meta.json
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/conftest.data.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/conftest.meta.json
+-rw-r--r--   0        0        0    92076 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/contextlib.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/contextlib.meta.json
+-rw-r--r--   0        0        0    35653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/contextvars.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/contextvars.meta.json
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/copy.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/copy.meta.json
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/copyreg.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/copyreg.meta.json
+-rw-r--r--   0        0        0    29661 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/csv.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/csv.meta.json
+-rw-r--r--   0        0        0    51547 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/dataclasses.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/dataclasses.meta.json
+-rw-r--r--   0        0        0   127876 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/datetime.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/datetime.meta.json
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/decimal.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/decimal.meta.json
+-rw-r--r--   0        0        0    56438 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/difflib.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/difflib.meta.json
+-rw-r--r--   0        0        0    39405 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/dis.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/dis.meta.json
+-rw-r--r--   0        0        0    69288 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/doctest.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/doctest.meta.json
+-rw-r--r--   0        0        0    60742 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/enum.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/enum.meta.json
+-rw-r--r--   0        0        0    19385 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/errno.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/errno.meta.json
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/fnmatch.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/fnmatch.meta.json
+-rw-r--r--   0        0        0    92293 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/fractions.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/fractions.meta.json
+-rw-r--r--   0        0        0   126780 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/functools.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/functools.meta.json
+-rw-r--r--   0        0        0    15324 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/gc.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/gc.meta.json
+-rw-r--r--   0        0        0    22401 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/genericpath.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/genericpath.meta.json
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/getpass.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/getpass.meta.json
+-rw-r--r--   0        0        0    53393 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/gettext.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/gettext.meta.json
+-rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/glob.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/glob.meta.json
+-rw-r--r--   0        0        0    27021 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/hashlib.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/hashlib.meta.json
+-rw-r--r--   0        0        0   334703 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/inspect.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/inspect.meta.json
+-rw-r--r--   0        0        0    85350 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/io.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/io.meta.json
+-rw-r--r--   0        0        0   259435 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/itertools.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/itertools.meta.json
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/keyword.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/keyword.meta.json
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/marshal.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/marshal.meta.json
+-rw-r--r--   0        0        0    49415 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/math.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/math.meta.json
+-rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/mimetypes.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/mimetypes.meta.json
+-rw-r--r--   0        0        0    26427 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/mmap.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/mmap.meta.json
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/netrc.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/netrc.meta.json
+-rw-r--r--   0        0        0    78984 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numbers.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numbers.meta.json
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/opcode.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/opcode.meta.json
+-rw-r--r--   0        0        0    46574 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/operator.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/operator.meta.json
+-rw-r--r--   0        0        0    83681 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pathlib.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pathlib.meta.json
+-rw-r--r--   0        0        0    93344 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pdb.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pdb.meta.json
+-rw-r--r--   0        0        0    44406 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pickle.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pickle.meta.json
+-rw-r--r--   0        0        0    30187 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pkgutil.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pkgutil.meta.json
+-rw-r--r--   0        0        0    33444 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/platform.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/platform.meta.json
+-rw-r--r--   0        0        0    75080 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/posixpath.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/posixpath.meta.json
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pprint.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pprint.meta.json
+-rw-r--r--   0        0        0   103495 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pydoc.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pydoc.meta.json
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/queue.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/queue.meta.json
+-rw-r--r--   0        0        0    39655 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/random.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/random.meta.json
+-rw-r--r--   0        0        0   165070 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/re.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/re.meta.json
+-rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/reprlib.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/reprlib.meta.json
+-rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/select.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/select.meta.json
+-rw-r--r--   0        0        0    54878 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/selectors.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/selectors.meta.json
+-rw-r--r--   0        0        0    16509 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/shlex.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/shlex.meta.json
+-rw-r--r--   0        0        0    70356 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/shutil.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/shutil.meta.json
+-rw-r--r--   0        0        0    31620 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/signal.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/signal.meta.json
+-rw-r--r--   0        0        0    77705 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/socket.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/socket.meta.json
+-rw-r--r--   0        0        0    58033 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/socketserver.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/socketserver.meta.json
+-rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sre_compile.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sre_compile.meta.json
+-rw-r--r--   0        0        0    28015 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sre_constants.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sre_constants.meta.json
+-rw-r--r--   0        0        0    49455 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sre_parse.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sre_parse.meta.json
+-rw-r--r--   0        0        0   188211 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/ssl.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/ssl.meta.json
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/stat.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/stat.meta.json
+-rw-r--r--   0        0        0    28134 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/string.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/string.meta.json
+-rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/struct.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/struct.meta.json
+-rw-r--r--   0        0        0   137954 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/subprocess.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/subprocess.meta.json
+-rw-r--r--   0        0        0   145382 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sys.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sys.meta.json
+-rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sysconfig.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sysconfig.meta.json
+-rw-r--r--   0        0        0   133938 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tempfile.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tempfile.meta.json
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_ai.data.json
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_ai.meta.json
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_args.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_args.meta.json
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_consts.data.json
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_consts.meta.json
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_files.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_files.meta.json
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_funcs.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_funcs.meta.json
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_gpt.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_gpt.meta.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_igpt.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_igpt.meta.json
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_imports.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/test_imports.meta.json
+-rw-r--r--   0        0        0    19555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/textwrap.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/textwrap.meta.json
+-rw-r--r--   0        0        0    63952 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/threading.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/threading.meta.json
+-rw-r--r--   0        0        0    41028 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/time.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/time.meta.json
+-rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/token.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/token.meta.json
+-rw-r--r--   0        0        0    48440 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tokenize.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tokenize.meta.json
+-rw-r--r--   0        0        0    46133 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traceback.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traceback.meta.json
+-rw-r--r--   0        0        0    47456 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tracemalloc.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tracemalloc.meta.json
+-rw-r--r--   0        0        0   205398 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/types.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/types.meta.json
+-rw-r--r--   0        0        0   392815 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/typing.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/typing.meta.json
+-rw-r--r--   0        0        0    70277 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/typing_extensions.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/typing_extensions.meta.json
+-rw-r--r--   0        0        0    42225 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unicodedata.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unicodedata.meta.json
+-rw-r--r--   0        0        0    33636 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/uuid.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/uuid.meta.json
+-rw-r--r--   0        0        0    22158 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/warnings.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/warnings.meta.json
+-rw-r--r--   0        0        0   111375 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/weakref.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/weakref.meta.json
+-rw-r--r--   0        0        0    68197 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/zipfile.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/zipfile.meta.json
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/zipimport.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/zipimport.meta.json
+-rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/zlib.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/zlib.meta.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/__init__.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/__init__.meta.json
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_argcomplete.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_argcomplete.meta.json
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_version.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_version.meta.json
+-rw-r--r--   0        0        0    41440 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/cacheprovider.data.json
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/cacheprovider.meta.json
+-rw-r--r--   0        0        0   158288 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/capture.data.json
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/capture.meta.json
+-rw-r--r--   0        0        0    24432 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/compat.data.json
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/compat.meta.json
+-rw-r--r--   0        0        0    30451 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/debugging.data.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/debugging.meta.json
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/deprecated.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/deprecated.meta.json
+-rw-r--r--   0        0        0    49551 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/doctest.data.json
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/doctest.meta.json
+-rw-r--r--   0        0        0   146234 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/fixtures.data.json
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/fixtures.meta.json
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/freeze_support.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/freeze_support.meta.json
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/helpconfig.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/helpconfig.meta.json
+-rw-r--r--   0        0        0    56847 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/hookspec.data.json
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/hookspec.meta.json
+-rw-r--r--   0        0        0    60447 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/legacypath.data.json
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/legacypath.meta.json
+-rw-r--r--   0        0        0    74402 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/logging.data.json
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/logging.meta.json
+-rw-r--r--   0        0        0    44515 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/main.data.json
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/main.meta.json
+-rw-r--r--   0        0        0    24892 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/monkeypatch.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/monkeypatch.meta.json
+-rw-r--r--   0        0        0    55864 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/nodes.data.json
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/nodes.meta.json
+-rw-r--r--   0        0        0    29277 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/outcomes.data.json
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/outcomes.meta.json
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/pathlib.data.json
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/pathlib.meta.json
+-rw-r--r--   0        0        0   128637 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester.data.json
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester.meta.json
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester_assertions.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester_assertions.meta.json
+-rw-r--r--   0        0        0   110800 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/python.data.json
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/python.meta.json
+-rw-r--r--   0        0        0    49915 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/python_api.data.json
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/python_api.meta.json
+-rw-r--r--   0        0        0    29598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/recwarn.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/recwarn.meta.json
+-rw-r--r--   0        0        0    49418 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/reports.data.json
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/reports.meta.json
+-rw-r--r--   0        0        0    38342 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/runner.data.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/runner.meta.json
+-rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/scope.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/scope.meta.json
+-rw-r--r--   0        0        0    13836 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/stash.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/stash.meta.json
+-rw-r--r--   0        0        0    90377 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/terminal.data.json
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/terminal.meta.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/timing.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/timing.meta.json
+-rw-r--r--   0        0        0    21112 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/tmpdir.data.json
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/tmpdir.meta.json
+-rw-r--r--   0        0        0    25827 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/warning_types.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/warning_types.meta.json
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/warnings.data.json
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/warnings.meta.json
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/__init__.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/__init__.meta.json
+-rw-r--r--   0        0        0   154497 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/code.data.json
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/code.meta.json
+-rw-r--r--   0        0        0    18059 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/source.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/source.meta.json
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/__init__.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/__init__.meta.json
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/saferepr.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/saferepr.meta.json
+-rw-r--r--   0        0        0    15772 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/terminalwriter.data.json
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/terminalwriter.meta.json
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/wcwidth.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/wcwidth.meta.json
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/__init__.data.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/__init__.meta.json
+-rw-r--r--   0        0        0    58844 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/rewrite.data.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/rewrite.meta.json
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/truncate.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/truncate.meta.json
+-rw-r--r--   0        0        0    22262 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/util.data.json
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/util.meta.json
+-rw-r--r--   0        0        0    97039 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/__init__.data.json
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/__init__.meta.json
+-rw-r--r--   0        0        0    39844 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/argparsing.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/argparsing.meta.json
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/compat.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/compat.meta.json
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/exceptions.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/exceptions.meta.json
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/findpaths.data.json
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/findpaths.meta.json
+-rw-r--r--   0        0        0    22270 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/__init__.data.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/__init__.meta.json
+-rw-r--r--   0        0        0    29097 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/expression.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/expression.meta.json
+-rw-r--r--   0        0        0   107269 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/structures.data.json
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/structures.meta.json
+-rw-r--r--   0        0        0    90306 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/__init__.data.json
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/__init__.meta.json
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/_helpers.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/_helpers.meta.json
+-rw-r--r--   0        0        0    54933 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/abc.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/abc.meta.json
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/base_protocol.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/base_protocol.meta.json
+-rw-r--r--   0        0        0   114110 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client.data.json
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client.meta.json
+-rw-r--r--   0        0        0    60919 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_exceptions.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_exceptions.meta.json
+-rw-r--r--   0        0        0    20514 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_proto.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_proto.meta.json
+-rw-r--r--   0        0        0   134406 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_reqrep.data.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_reqrep.meta.json
+-rw-r--r--   0        0        0    35159 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_ws.data.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_ws.meta.json
+-rw-r--r--   0        0        0   101185 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/connector.data.json
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/connector.meta.json
+-rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/cookiejar.data.json
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/cookiejar.meta.json
+-rw-r--r--   0        0        0    11434 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/formdata.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/formdata.meta.json
+-rw-r--r--   0        0        0    21353 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/hdrs.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/hdrs.meta.json
+-rw-r--r--   0        0        0   129839 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/helpers.data.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/helpers.meta.json
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http.meta.json
+-rw-r--r--   0        0        0    19942 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_exceptions.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_exceptions.meta.json
+-rw-r--r--   0        0        0   108296 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_parser.data.json
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_parser.meta.json
+-rw-r--r--   0        0        0    75626 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_websocket.data.json
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_websocket.meta.json
+-rw-r--r--   0        0        0    33316 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_writer.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_writer.meta.json
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/locks.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/locks.meta.json
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/log.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/log.meta.json
+-rw-r--r--   0        0        0    81476 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/multipart.data.json
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/multipart.meta.json
+-rw-r--r--   0        0        0    58649 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload.data.json
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload.meta.json
+-rw-r--r--   0        0        0    15753 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload_streamer.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload_streamer.meta.json
+-rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/resolver.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/resolver.meta.json
+-rw-r--r--   0        0        0    72323 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/streams.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/streams.meta.json
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tcp_helpers.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tcp_helpers.meta.json
+-rw-r--r--   0        0        0   216782 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tracing.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tracing.meta.json
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/typedefs.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/typedefs.meta.json
+-rw-r--r--   0        0        0    25449 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web.data.json
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web.meta.json
+-rw-r--r--   0        0        0    63171 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_app.data.json
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_app.meta.json
+-rw-r--r--   0        0        0    92924 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_exceptions.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_exceptions.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_fileresponse.data.json
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_fileresponse.meta.json
+-rw-r--r--   0        0        0    41534 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_log.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_log.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_middlewares.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_middlewares.meta.json
+-rw-r--r--   0        0        0    49073 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_protocol.data.json
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_protocol.meta.json
+-rw-r--r--   0        0        0    93980 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_request.data.json
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_request.meta.json
+-rw-r--r--   0        0        0    82826 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_response.data.json
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_response.meta.json
+-rw-r--r--   0        0        0    57693 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_routedef.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_routedef.meta.json
+-rw-r--r--   0        0        0    58927 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_runner.data.json
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_runner.meta.json
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_server.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_server.meta.json
+-rw-r--r--   0        0        0   180562 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_urldispatcher.data.json
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_urldispatcher.meta.json
+-rw-r--r--   0        0        0    52501 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_ws.data.json
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_ws.meta.json
+-rw-r--r--   0        0        0    19267 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/worker.data.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiohttp/worker.meta.json
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiosignal/__init__.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/aiosignal/__init__.meta.json
+-rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/async_timeout/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/async_timeout/__init__.meta.json
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0    98750 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    25243 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   188237 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/events.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    35534 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    31660 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/locks.meta.json
+-rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    22078 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/queues.meta.json
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    35291 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0   106509 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0    27488 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    51737 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0   210184 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/__init__.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/__init__.meta.json
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/_cmp.data.json
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/_cmp.meta.json
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/_typing_compat.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/_typing_compat.meta.json
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/_version_info.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/_version_info.meta.json
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/converters.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/converters.meta.json
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/exceptions.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/exceptions.meta.json
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/filters.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/filters.meta.json
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/setters.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/setters.meta.json
+-rw-r--r--   0        0        0    42073 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/validators.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/attr/validators.meta.json
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/__init__.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/__init__.meta.json
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/api.data.json
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/api.meta.json
+-rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/cd.data.json
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/cd.meta.json
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/constant.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/constant.meta.json
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/legacy.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/legacy.meta.json
+-rw-r--r--   0        0        0    59341 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/md.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/md.meta.json
+-rw-r--r--   0        0        0    50507 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/models.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/models.meta.json
+-rw-r--r--   0        0        0    28046 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/utils.data.json
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/utils.meta.json
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/version.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/version.meta.json
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/assets/__init__.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/assets/__init__.meta.json
+-rw-r--r--   0        0        0   367796 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/collections/__init__.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/collections/abc.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/collections/abc.meta.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    70910 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    20711 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   126917 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    34692 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/curses/__init__.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/curses/__init__.meta.json
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/__init__.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/__init__.meta.json
+-rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/charset.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/charset.meta.json
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/errors.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/errors.meta.json
+-rw-r--r--   0        0        0    17249 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/feedparser.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/feedparser.meta.json
+-rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/header.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/header.meta.json
+-rw-r--r--   0        0        0    79294 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/message.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/message.meta.json
+-rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/parser.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/parser.meta.json
+-rw-r--r--   0        0        0    30859 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/policy.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/policy.meta.json
+-rw-r--r--   0        0        0    20503 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/utils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/email/utils.meta.json
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/__init__.meta.json
+-rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_catch.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_catch.meta.json
+-rw-r--r--   0        0        0    66814 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_exceptions.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_exceptions.meta.json
+-rw-r--r--   0        0        0    21945 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_formatting.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_formatting.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_version.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_version.meta.json
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/frozenlist/__init__.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/frozenlist/__init__.meta.json
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/html/__init__.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/html/__init__.meta.json
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/html/entities.data.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/html/entities.meta.json
+-rw-r--r--   0        0        0    18711 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/__init__.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/__init__.meta.json
+-rw-r--r--   0        0        0    66298 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/client.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/client.meta.json
+-rw-r--r--   0        0        0    58156 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/cookiejar.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/cookiejar.meta.json
+-rw-r--r--   0        0        0    38912 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/cookies.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/cookies.meta.json
+-rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/server.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/http/server.meta.json
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    41053 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/abc.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/abc.meta.json
+-rw-r--r--   0        0        0    65333 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/util.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/util.meta.json
+-rw-r--r--   0        0        0    64663 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    93642 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    22217 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    22663 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    44366 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/iniconfig/__init__.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/iniconfig/__init__.meta.json
+-rw-r--r--   0        0        0    21926 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/iniconfig/_parse.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/iniconfig/_parse.meta.json
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/iniconfig/exceptions.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/iniconfig/exceptions.meta.json
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/__init__.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/__init__.meta.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/_identifier.data.json
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/_identifier.meta.json
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/async_utils.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/async_utils.meta.json
+-rw-r--r--   0        0        0    26219 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/bccache.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/bccache.meta.json
+-rw-r--r--   0        0        0   155139 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/compiler.data.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/compiler.meta.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/constants.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/constants.meta.json
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/debug.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/debug.meta.json
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/defaults.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/defaults.meta.json
+-rw-r--r--   0        0        0   116065 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/environment.data.json
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/environment.meta.json
+-rw-r--r--   0        0        0    17712 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/exceptions.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/exceptions.meta.json
+-rw-r--r--   0        0        0    49856 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/ext.data.json
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/ext.meta.json
+-rw-r--r--   0        0        0   149382 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/filters.data.json
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/filters.meta.json
+-rw-r--r--   0        0        0    42314 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/idtracking.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/idtracking.meta.json
+-rw-r--r--   0        0        0    88022 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/lexer.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/lexer.meta.json
+-rw-r--r--   0        0        0    47837 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/loaders.data.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/loaders.meta.json
+-rw-r--r--   0        0        0   146988 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/nodes.data.json
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/nodes.meta.json
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/optimizer.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/optimizer.meta.json
+-rw-r--r--   0        0        0    47362 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/parser.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/parser.meta.json
+-rw-r--r--   0        0        0   148084 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/runtime.data.json
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/runtime.meta.json
+-rw-r--r--   0        0        0    32271 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/sandbox.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/sandbox.meta.json
+-rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/tests.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/tests.meta.json
+-rw-r--r--   0        0        0    61362 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/utils.data.json
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/utils.meta.json
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/visitor.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/jinja2/visitor.meta.json
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/json/__init__.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/json/__init__.meta.json
+-rw-r--r--   0        0        0    14506 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/json/decoder.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/json/decoder.meta.json
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/json/encoder.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/json/encoder.meta.json
+-rw-r--r--   0        0        0   140127 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/logging/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/logging/__init__.meta.json
+-rw-r--r--   0        0        0    14100 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/logging/config.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/logging/config.meta.json
+-rw-r--r--   0        0        0    74406 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/logging/handlers.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/logging/handlers.meta.json
+-rw-r--r--   0        0        0    34443 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/markupsafe/__init__.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/markupsafe/__init__.meta.json
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_native.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_native.meta.json
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_speedups.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_speedups.meta.json
+-rw-r--r--   0        0        0   133573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multidict/__init__.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multidict/__init__.meta.json
+-rw-r--r--   0        0        0    31384 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30665 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95606 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   146899 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    50247 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9020 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17688 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    17677 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28883 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    28132 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67379 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25560 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23554 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/__init__.data.json
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/__init__.meta.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/_imports.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/_imports.meta.json
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/_struct.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/_struct.meta.json
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/_version.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/_version.meta.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/converter.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/converter.meta.json
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/json_compat.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/json_compat.meta.json
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/notebooknode.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/notebooknode.meta.json
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/reader.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/reader.meta.json
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/sentinel.data.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/sentinel.meta.json
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/validator.data.json
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/validator.meta.json
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/warnings.data.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/warnings.meta.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/__init__.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/__init__.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/words.data.json
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/words.meta.json
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/__init__.meta.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/convert.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/convert.meta.json
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbbase.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbbase.meta.json
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbjson.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbjson.meta.json
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/rwbase.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/rwbase.meta.json
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/__init__.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/__init__.meta.json
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/convert.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/convert.meta.json
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbbase.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbbase.meta.json
+-rw-r--r--   0        0        0     9806 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbjson.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbjson.meta.json
+-rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbpy.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbpy.meta.json
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbxml.data.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbxml.meta.json
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/rwbase.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/rwbase.meta.json
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/__init__.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/__init__.meta.json
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/convert.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/convert.meta.json
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbbase.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbbase.meta.json
+-rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbjson.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbjson.meta.json
+-rw-r--r--   0        0        0    10991 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbpy.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbpy.meta.json
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/rwbase.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/rwbase.meta.json
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/__init__.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/__init__.meta.json
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/convert.data.json
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/convert.meta.json
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbbase.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbbase.meta.json
+-rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbjson.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbjson.meta.json
+-rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/rwbase.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/rwbase.meta.json
+-rw-r--r--   0        0        0  2216519 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_version.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112501 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/version.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/version.meta.json
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25394 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   260468 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41708 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30688 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    33297 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16755 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261349 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13641 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21869 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169656 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36045 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330685 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49546 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301742 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196438 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    45650 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    24433 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52611 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52744 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18738 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21709 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24000 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    18058 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   154533 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    25919 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   223847 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    63614 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47359 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    89078 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    96612 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    96739 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62213 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    89041 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    23493 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    76988 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0    97310 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    24846 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    26118 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107773 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27663 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136748 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    26985 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16462 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14238 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14013 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253014 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8966 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    66834 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323845 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114195 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/__init__.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/__init__.meta.json
+-rw-r--r--   0        0        0    63039 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_requestor.data.json
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_requestor.meta.json
+-rw-r--r--   0        0        0    17891 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/error.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/error.meta.json
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/object_classes.data.json
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/object_classes.meta.json
+-rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/openai_object.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/openai_object.meta.json
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/openai_response.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/openai_response.meta.json
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/util.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/util.meta.json
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/version.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/version.meta.json
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/__init__.data.json
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/__init__.meta.json
+-rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/audio.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/audio.meta.json
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/chat_completion.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/chat_completion.meta.json
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/completion.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/completion.meta.json
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/customer.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/customer.meta.json
+-rw-r--r--   0        0        0    18539 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/deployment.data.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/deployment.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/edit.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/edit.meta.json
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/embedding.data.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/embedding.meta.json
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/engine.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/engine.meta.json
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/error_object.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/error_object.meta.json
+-rw-r--r--   0        0        0    20017 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/file.data.json
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/file.meta.json
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/fine_tune.data.json
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/fine_tune.meta.json
+-rw-r--r--   0        0        0    18573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/image.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/image.meta.json
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/model.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/model.meta.json
+-rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/moderation.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/moderation.meta.json
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/__init__.data.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/__init__.meta.json
+-rw-r--r--   0        0        0    15484 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.meta.json
+-rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.meta.json
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.meta.json
+-rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.data.json
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.meta.json
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.meta.json
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.meta.json
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.meta.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/__init__.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/__init__.meta.json
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.meta.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/__init__.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/__init__.meta.json
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/common.data.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/common.meta.json
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/numpy_helper.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/numpy_helper.meta.json
+-rw-r--r--   0        0        0   302162 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/os/__init__.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/os/__init__.meta.json
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/os/path.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/os/path.meta.json
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    26006 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    43260 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_parser.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_parser.meta.json
+-rw-r--r--   0        0        0    13942 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    16957 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_tokenizer.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/_tokenizer.meta.json
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/markers.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/markers.meta.json
+-rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/requirements.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/requirements.meta.json
+-rw-r--r--   0        0        0    55965 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    27782 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/tags.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/tags.meta.json
+-rw-r--r--   0        0        0     9823 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/utils.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/utils.meta.json
+-rw-r--r--   0        0        0    64770 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/version.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/packaging/version.meta.json
+-rw-r--r--   0        0        0    13421 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/__init__.data.json
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/__init__.meta.json
+-rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_typing.data.json
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_typing.meta.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/testing.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/testing.meta.json
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/__init__.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/__init__.meta.json
+-rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/config.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/config.meta.json
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/__init__.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/__init__.meta.json
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/indexing.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/indexing.meta.json
+-rw-r--r--   0        0        0   175917 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/interval.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/interval.meta.json
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/lib.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/lib.meta.json
+-rw-r--r--   0        0        0    31716 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/missing.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/missing.meta.json
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/ops_dispatch.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/ops_dispatch.meta.json
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/properties.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/properties.meta.json
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.meta.json
+-rw-r--r--   0        0        0    58549 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.meta.json
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.meta.json
+-rw-r--r--   0        0        0   125179 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.data.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.meta.json
+-rw-r--r--   0        0        0    92308 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/period.data.json
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/period.meta.json
+-rw-r--r--   0        0        0   189107 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.data.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.meta.json
+-rw-r--r--   0        0        0   148757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.data.json
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.meta.json
+-rw-r--r--   0        0        0    30667 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_testing/__init__.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/_testing/__init__.meta.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/__init__.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/__init__.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/extensions/__init__.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/extensions/__init__.meta.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/indexers/__init__.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/indexers/__init__.meta.json
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/types/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/api/types/__init__.meta.json
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/arrays/__init__.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/arrays/__init__.meta.json
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/__init__.data.json
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/__init__.meta.json
+-rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/accessor.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/accessor.meta.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/algorithms.data.json
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/algorithms.meta.json
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/api.data.json
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/api.meta.json
+-rw-r--r--   0        0        0    37388 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arraylike.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arraylike.meta.json
+-rw-r--r--   0        0        0    36591 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/base.data.json
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/base.meta.json
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/construction.data.json
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/construction.meta.json
+-rw-r--r--   0        0        0   636452 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/frame.data.json
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/frame.meta.json
+-rw-r--r--   0        0        0   125166 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/generic.data.json
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/generic.meta.json
+-rw-r--r--   0        0        0    18184 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexers.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexers.meta.json
+-rw-r--r--   0        0        0    26374 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexing.data.json
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexing.meta.json
+-rw-r--r--   0        0        0    90473 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/resample.data.json
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/resample.meta.json
+-rw-r--r--   0        0        0  1275803 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/series.data.json
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/series.meta.json
+-rw-r--r--   0        0        0   130171 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/strings.data.json
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/strings.meta.json
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/__init__.data.json
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/__init__.meta.json
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow.data.json
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow.meta.json
+-rw-r--r--   0        0        0    32987 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/base.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/base.meta.json
+-rw-r--r--   0        0        0    12359 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/boolean.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/boolean.meta.json
+-rw-r--r--   0        0        0   102656 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/categorical.data.json
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/categorical.meta.json
+-rw-r--r--   0        0        0    39589 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimelike.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimelike.meta.json
+-rw-r--r--   0        0        0    27598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimes.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimes.meta.json
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/floating.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/floating.meta.json
+-rw-r--r--   0        0        0    17764 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/integer.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/integer.meta.json
+-rw-r--r--   0        0        0    39144 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/interval.data.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/interval.meta.json
+-rw-r--r--   0        0        0    10795 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/masked.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/masked.meta.json
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numeric.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numeric.meta.json
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numpy_.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numpy_.meta.json
+-rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/period.data.json
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/period.meta.json
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/string_.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/string_.meta.json
+-rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/timedeltas.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/timedeltas.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.meta.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.meta.json
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.meta.json
+-rw-r--r--   0        0        0    32211 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/array.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/array.meta.json
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.meta.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/__init__.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/__init__.meta.json
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/api.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/api.meta.json
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/eval.data.json
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/eval.meta.json
+-rw-r--r--   0        0        0    23567 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/expr.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/expr.meta.json
+-rw-r--r--   0        0        0    44759 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/ops.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/ops.meta.json
+-rw-r--r--   0        0        0    43657 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/pytables.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/pytables.meta.json
+-rw-r--r--   0        0        0    11640 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/scope.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/scope.meta.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/__init__.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/__init__.meta.json
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/api.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/api.meta.json
+-rw-r--r--   0        0        0    14757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/base.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/base.meta.json
+-rw-r--r--   0        0        0    21491 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/common.data.json
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/common.meta.json
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/concat.data.json
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/concat.meta.json
+-rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/dtypes.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/dtypes.meta.json
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/generic.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/generic.meta.json
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/inference.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/inference.meta.json
+-rw-r--r--   0        0        0    22548 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/missing.data.json
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/missing.meta.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/__init__.meta.json
+-rw-r--r--   0        0        0   244906 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/generic.data.json
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/generic.meta.json
+-rw-r--r--   0        0        0    59210 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/groupby.data.json
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/groupby.meta.json
+-rw-r--r--   0        0        0    20931 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/grouper.data.json
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/grouper.meta.json
+-rw-r--r--   0        0        0    41306 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/ops.data.json
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/ops.meta.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/__init__.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/__init__.meta.json
+-rw-r--r--   0        0        0   252631 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/accessors.data.json
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/accessors.meta.json
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/api.data.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/api.meta.json
+-rw-r--r--   0        0        0   145199 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/base.data.json
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/base.meta.json
+-rw-r--r--   0        0        0    20184 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/category.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/category.meta.json
+-rw-r--r--   0        0        0    13589 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimelike.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimelike.meta.json
+-rw-r--r--   0        0        0    39465 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimes.data.json
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimes.meta.json
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/extension.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/extension.meta.json
+-rw-r--r--   0        0        0   201189 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/interval.data.json
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/interval.meta.json
+-rw-r--r--   0        0        0    64757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/multi.data.json
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/multi.meta.json
+-rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/period.data.json
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/period.meta.json
+-rw-r--r--   0        0        0    33976 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/range.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/range.meta.json
+-rw-r--r--   0        0        0    21832 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/timedeltas.data.json
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/timedeltas.meta.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/__init__.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/__init__.meta.json
+-rw-r--r--   0        0        0    56017 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.meta.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/__init__.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/__init__.meta.json
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/api.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/api.meta.json
+-rw-r--r--   0        0        0    22852 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/concat.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/concat.meta.json
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/encoding.data.json
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/encoding.meta.json
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/melt.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/melt.meta.json
+-rw-r--r--   0        0        0    32377 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/merge.data.json
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/merge.meta.json
+-rw-r--r--   0        0        0    40821 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/pivot.data.json
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/pivot.meta.json
+-rw-r--r--   0        0        0    79005 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/tile.data.json
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/tile.meta.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/__init__.data.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/__init__.meta.json
+-rw-r--r--   0        0        0    19799 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/datetimes.data.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/datetimes.meta.json
+-rw-r--r--   0        0        0    13501 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/numeric.data.json
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/numeric.meta.json
+-rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/timedeltas.data.json
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/timedeltas.meta.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/__init__.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/__init__.meta.json
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/hashing.data.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/hashing.meta.json
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/__init__.meta.json
+-rw-r--r--   0        0        0    22703 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/ewm.data.json
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/ewm.meta.json
+-rw-r--r--   0        0        0    35020 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/expanding.data.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/expanding.meta.json
+-rw-r--r--   0        0        0    66448 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/rolling.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/rolling.meta.json
+-rw-r--r--   0        0        0    29360 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/errors/__init__.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/errors/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/__init__.meta.json
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/api.data.json
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/api.meta.json
+-rw-r--r--   0        0        0    51797 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/clipboards.data.json
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/clipboards.meta.json
+-rw-r--r--   0        0        0     8436 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/common.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/common.meta.json
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/feather_format.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/feather_format.meta.json
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/gbq.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/gbq.meta.json
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/html.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/html.meta.json
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/orc.data.json
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/orc.meta.json
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parquet.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parquet.meta.json
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pickle.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pickle.meta.json
+-rw-r--r--   0        0        0    57813 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pytables.data.json
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pytables.meta.json
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/spss.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/spss.meta.json
+-rw-r--r--   0        0        0    43548 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sql.data.json
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sql.meta.json
+-rw-r--r--   0        0        0    32872 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/stata.data.json
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/stata.meta.json
+-rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/xml.data.json
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/xml.meta.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/__init__.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/__init__.meta.json
+-rw-r--r--   0        0        0    79612 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/_base.data.json
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/_base.meta.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/__init__.data.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/__init__.meta.json
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/format.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/format.meta.json
+-rw-r--r--   0        0        0    80709 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style.data.json
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style.meta.json
+-rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style_render.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style_render.meta.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/__init__.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/__init__.meta.json
+-rw-r--r--   0        0        0    39658 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_json.data.json
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_json.meta.json
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_normalize.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_normalize.meta.json
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_table_schema.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_table_schema.meta.json
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/__init__.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/__init__.meta.json
+-rw-r--r--   0        0        0   135743 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/readers.data.json
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/readers.meta.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/__init__.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/__init__.meta.json
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas7bdat.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas7bdat.meta.json
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas_xport.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas_xport.meta.json
+-rw-r--r--   0        0        0    26676 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sasreader.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sasreader.meta.json
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/__init__.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/__init__.meta.json
+-rw-r--r--   0        0        0   150357 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_core.data.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_core.meta.json
+-rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_misc.data.json
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_misc.meta.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/__init__.data.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/__init__.meta.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/api.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/api.meta.json
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/frequencies.data.json
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/frequencies.meta.json
+-rw-r--r--   0        0        0    36662 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/holiday.data.json
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/holiday.meta.json
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/offsets.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/offsets.meta.json
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/__init__.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/__init__.meta.json
+-rw-r--r--   0        0        0    18309 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_decorators.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_decorators.meta.json
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_print_versions.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_print_versions.meta.json
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_tester.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_tester.meta.json
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pytest/__init__.data.json
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/pytest/__init__.meta.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/__init__.data.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/__init__.meta.json
+-rw-r--r--   0        0        0    16218 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/_config.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/_config.meta.json
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/ai.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/ai.meta.json
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/explain.data.json
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/explain.meta.json
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/llm.data.json
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/llm.meta.json
+-rw-r--r--   0        0        0    27581 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/runtime.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/runtime.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/utils.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/utils.meta.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/__init__.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/__init__.meta.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples.data.json
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples.meta.json
+-rw-r--r--   0        0        0    21302 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/prompt.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/prompt.meta.json
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.meta.json
+-rw-r--r--   0        0        0     9569 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sqlite3/__init__.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sqlite3/__init__.meta.json
+-rw-r--r--   0        0        0   122692 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sqlite3/dbapi2.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/sqlite3/dbapi2.meta.json
+-rw-r--r--   0        0        0    78723 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/__init__.data.json
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/__init__.meta.json
+-rw-r--r--   0        0        0    13989 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/_asyncio.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/_asyncio.meta.json
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/_utils.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/_utils.meta.json
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/after.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/after.meta.json
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/before.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/before.meta.json
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/before_sleep.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/before_sleep.meta.json
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/nap.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/nap.meta.json
+-rw-r--r--   0        0        0    37328 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/retry.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/retry.meta.json
+-rw-r--r--   0        0        0    19083 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/stop.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/stop.meta.json
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/tornadoweb.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/tornadoweb.meta.json
+-rw-r--r--   0        0        0    28054 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/wait.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tenacity/wait.meta.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/__init__.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/__init__.meta.json
+-rw-r--r--   0        0        0    26693 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/core.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/core.meta.json
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/model.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/model.meta.json
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/registry.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tiktoken/registry.meta.json
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/__init__.meta.json
+-rw-r--r--   0        0        0    51399 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/_parser.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/_parser.meta.json
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/_re.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/_re.meta.json
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/_types.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tomli/_types.meta.json
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/__init__.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/__init__.meta.json
+-rw-r--r--   0        0        0    25418 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/concurrent.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/concurrent.meta.json
+-rw-r--r--   0        0        0    30222 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/escape.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/escape.meta.json
+-rw-r--r--   0        0        0    55073 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/gen.data.json
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/gen.meta.json
+-rw-r--r--   0        0        0    66117 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/ioloop.data.json
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/ioloop.meta.json
+-rw-r--r--   0        0        0    76115 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/iostream.data.json
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/iostream.meta.json
+-rw-r--r--   0        0        0     9443 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/log.data.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/log.meta.json
+-rw-r--r--   0        0        0    34372 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/netutil.data.json
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/netutil.meta.json
+-rw-r--r--   0        0        0    40280 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/options.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/options.meta.json
+-rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/process.data.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/process.meta.json
+-rw-r--r--   0        0        0    40167 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/util.data.json
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/util.meta.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/__init__.meta.json
+-rw-r--r--   0        0        0    53792 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/asyncio.data.json
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/asyncio.meta.json
+-rw-r--r--   0        0        0    10750 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/__init__.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/__init__.meta.json
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/_version.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/_version.meta.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/log.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/log.meta.json
+-rw-r--r--   0        0        0   169650 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/traitlets.data.json
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/traitlets.meta.json
+-rw-r--r--   0        0        0     9747 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/__init__.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/__init__.meta.json
+-rw-r--r--   0        0        0    52360 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/application.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/application.meta.json
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/argcomplete_config.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/argcomplete_config.meta.json
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/configurable.data.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/configurable.meta.json
+-rw-r--r--   0        0        0    59589 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/loader.data.json
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/loader.meta.json
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/__init__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/bunch.data.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/bunch.meta.json
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/decorators.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/decorators.meta.json
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/descriptions.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/descriptions.meta.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/getargspec.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/getargspec.meta.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/importstring.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/importstring.meta.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/nested_update.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/nested_update.meta.json
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/sentinel.data.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/sentinel.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/text.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/text.meta.json
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/__init__.meta.json
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   224041 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/case.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/case.meta.json
+-rw-r--r--   0        0        0    14631 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/loader.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11728 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/main.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/main.meta.json
+-rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/result.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/result.meta.json
+-rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/runner.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/signals.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/suite.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/__init__.meta.json
+-rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/error.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/error.meta.json
+-rw-r--r--   0        0        0   172181 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/parse.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/parse.meta.json
+-rw-r--r--   0        0        0   152233 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/request.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/request.meta.json
+-rw-r--r--   0        0        0    27167 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/response.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/urllib/response.meta.json
+-rw-r--r--   0        0        0    45137 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/yarl/__init__.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 relyonai-0.1.2/.mypy_cache/3.8/yarl/__init__.meta.json
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 relyonai-0.1.2/.vscode/extensions.list
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relyonai-0.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 relyonai-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0   338435 2020-02-02 00:00:00.000000 relyonai-0.1.2/nbs/test.ipynb
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/__init__.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/_config.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/ai.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/explain.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/llm.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/runtime.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/utils.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/README.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/__init__.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/prompt.json
+-rw-r--r--   0        0        0    10303 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/prompt.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/README.md
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/consts.ipynb
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/env.ipynb
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/error_fixing.ipynb
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/errors.ipynb
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/exploration.ipynb
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/filename.txt
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/files.ipynb
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/format.ipynb
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/funcs1.ipynb
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/funcs2.ipynb
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/funcs3.ipynb
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/gpt.ipynb
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/imports.ipynb
+-rw-r--r--   0        0        0     8465 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/lambdas.ipynb
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/make_prompt.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/other.txt
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/plt.ipynb
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/run_all.sh
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/session.ipynb
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/examples/template.ipynb
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/schemas/NEW_SCHEMA.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/schemas/SCHEMA.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/schemas/SIMPLER_SCHEMA.md
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/system/default.md
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/system/gpt4-refined.md
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/system/gpt4.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/system/simpler.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 relyonai-0.1.2/relyonai/prompt/system/simpler2.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/test_gpt.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/multi/test_ai.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/single/test_args.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/single/test_consts.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/single/test_files.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/single/test_funcs.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/single/test_igpt.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/ai/single/test_imports.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/data/cities.csv
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 relyonai-0.1.2/tests/data/test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relyonai-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 relyonai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 relyonai-0.1.2/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relyonai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 relyonai-0.1.2/PKG-INFO
```

### Comparing `relyonai-0.1.1/showcase.png` & `relyonai-0.1.2/showcase.png`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/__future__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/__future__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/__future__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_ast.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_ast.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_ast.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_bisect.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_bisect.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_codecs.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_codecs.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_collections_abc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_collections_abc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_csv.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_csv.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_csv.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_ctypes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_ctypes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_curses.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_curses.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_curses.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_curses.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_decimal.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_decimal.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_operator.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_operator.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_operator.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_random.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_random.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_random.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_random.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_socket.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_socket.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_socket.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_stat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_stat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_stat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_thread.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_thread.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_thread.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_tracemalloc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_tracemalloc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_warnings.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_warnings.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_weakref.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_weakref.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_weakrefset.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_weakrefset.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/abc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/abc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/abc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/abc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/argparse.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/argparse.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/argparse.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/array.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/array.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/array.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/array.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/ast.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/ast.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/ast.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/ast.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/atexit.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/atexit.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/atexit.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/atexit.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/base64.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/base64.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/base64.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/base64.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/bdb.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/bdb.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/bdb.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/bdb.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/binascii.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/binascii.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/binascii.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/binascii.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/bisect.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/bisect.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/bisect.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/builtins.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/builtins.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/builtins.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/cmd.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/cmd.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/cmd.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/codecs.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/codecs.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/codecs.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/configparser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/configparser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/configparser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/conftest.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/conftest.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/conftest.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/conftest.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/contextlib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/contextlib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/contextvars.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/contextvars.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/copy.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/copy.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/copy.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/copy.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/copyreg.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/copyreg.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/csv.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/csv.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/csv.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/csv.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/dataclasses.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/dataclasses.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/datetime.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/datetime.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/datetime.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/decimal.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/decimal.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/decimal.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/difflib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/difflib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/difflib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/dis.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/dis.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/dis.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/dis.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/doctest.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/doctest.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/doctest.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/enum.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/enum.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/enum.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/enum.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/errno.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/errno.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/errno.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/errno.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/fnmatch.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/fnmatch.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/fnmatch.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/fnmatch.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/fractions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/fractions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/fractions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/functools.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/functools.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/functools.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/functools.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/gc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/gc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/gc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/gc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/genericpath.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/genericpath.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/getpass.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/getpass.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/getpass.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/gettext.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/gettext.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/gettext.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/glob.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/glob.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/glob.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/glob.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/hashlib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/hashlib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/inspect.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/inspect.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/inspect.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/io.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/io.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/io.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/io.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/itertools.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/itertools.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/itertools.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/keyword.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/keyword.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/keyword.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/keyword.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/marshal.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/marshal.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/marshal.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/math.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/math.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/math.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/math.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/mimetypes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/mimetypes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/mimetypes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/mimetypes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/mmap.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/mmap.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/mmap.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/netrc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/netrc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/netrc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/netrc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numbers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numbers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numbers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/opcode.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/opcode.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/opcode.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/operator.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/operator.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/operator.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/operator.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pathlib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pathlib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pdb.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pdb.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pdb.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pdb.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pickle.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pickle.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pickle.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pkgutil.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pkgutil.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/platform.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/platform.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/platform.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/platform.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/posixpath.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/posixpath.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pprint.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pprint.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pprint.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pydoc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pydoc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/queue.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/queue.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/queue.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/queue.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/random.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/random.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/random.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/random.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/re.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/re.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/re.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/re.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/reprlib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/reprlib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/select.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/select.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/select.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/select.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/selectors.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/selectors.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/selectors.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/shlex.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/shlex.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/shlex.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/shutil.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/shutil.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/shutil.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/signal.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/signal.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/signal.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/signal.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/socket.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/socket.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/socket.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/socket.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/socketserver.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/socketserver.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/socketserver.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/socketserver.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sre_compile.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sre_compile.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sre_constants.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sre_constants.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sre_parse.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sre_parse.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/ssl.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/ssl.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/ssl.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/stat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/stat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/stat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/stat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/string.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/string.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/string.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/string.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/struct.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/struct.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/struct.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/struct.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/subprocess.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/subprocess.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sys.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sys.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sys.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sys.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sysconfig.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sysconfig.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tempfile.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tempfile.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_ai.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_ai.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_ai.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_ai.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_args.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_args.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_args.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_args.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_consts.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_consts.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_consts.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_consts.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_files.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_files.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_files.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_files.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_funcs.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_funcs.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_funcs.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_funcs.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_gpt.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_gpt.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_gpt.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_gpt.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_igpt.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_igpt.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_igpt.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_igpt.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_imports.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_imports.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/test_imports.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/test_imports.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/textwrap.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/textwrap.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/threading.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/threading.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/threading.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/threading.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/time.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/time.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/time.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/time.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/token.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/token.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/token.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/token.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tokenize.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tokenize.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traceback.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traceback.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traceback.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tracemalloc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tracemalloc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/types.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/types.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/types.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/types.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/typing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/typing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/typing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/typing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/typing_extensions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/typing_extensions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unicodedata.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unicodedata.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/uuid.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/uuid.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/uuid.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/warnings.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/warnings.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/warnings.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/weakref.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/weakref.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/weakref.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/zipfile.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/zipfile.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/zipimport.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/zipimport.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/zipimport.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/zipimport.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/zlib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/zlib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/zlib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_argcomplete.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_argcomplete.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_argcomplete.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_argcomplete.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/cacheprovider.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/cacheprovider.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/cacheprovider.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/cacheprovider.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/capture.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/capture.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/capture.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/capture.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/compat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/compat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/compat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/compat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/debugging.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/debugging.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/debugging.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/debugging.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/deprecated.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/deprecated.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/deprecated.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/deprecated.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/doctest.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/doctest.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/doctest.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/fixtures.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/fixtures.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/fixtures.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/fixtures.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/freeze_support.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/freeze_support.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/freeze_support.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/freeze_support.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/helpconfig.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/helpconfig.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/helpconfig.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/helpconfig.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/hookspec.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/hookspec.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/hookspec.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/hookspec.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/legacypath.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/legacypath.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/legacypath.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/legacypath.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/logging.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/logging.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/logging.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/logging.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/main.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/main.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/main.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/main.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/monkeypatch.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/monkeypatch.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/monkeypatch.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/monkeypatch.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/nodes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/nodes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/nodes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/outcomes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/outcomes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/outcomes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/outcomes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/pathlib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/pathlib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester_assertions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester_assertions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/pytester_assertions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/pytester_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/python.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/python.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/python.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/python.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/python_api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/python_api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/python_api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/python_api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/recwarn.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/recwarn.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/recwarn.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/recwarn.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/reports.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/reports.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/reports.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/reports.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/runner.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/runner.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/runner.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/scope.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/scope.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/scope.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/scope.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/stash.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/stash.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/stash.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/stash.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/terminal.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/terminal.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/terminal.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/timing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/timing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/timing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/timing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/tmpdir.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/tmpdir.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/tmpdir.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/tmpdir.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/warning_types.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/warning_types.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/warning_types.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/warning_types.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/warnings.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/warnings.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/warnings.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/code.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/code.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/code.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/code.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/source.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/source.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_code/source.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_code/source.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/saferepr.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/saferepr.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/saferepr.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/saferepr.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/terminalwriter.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/terminalwriter.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/terminalwriter.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/terminalwriter.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/wcwidth.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/wcwidth.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/_io/wcwidth.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/_io/wcwidth.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/rewrite.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/rewrite.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/rewrite.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/rewrite.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/truncate.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/truncate.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/truncate.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/truncate.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/util.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/util.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/assertion/util.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/assertion/util.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/argparsing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/argparsing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/argparsing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/argparsing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/compat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/compat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/compat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/compat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/findpaths.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/findpaths.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/config/findpaths.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/config/findpaths.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/expression.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/expression.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/expression.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/expression.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/structures.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/structures.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_pytest/mark/structures.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_pytest/mark/structures.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_typeshed/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/_typeshed/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/_helpers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/_helpers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/_helpers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/_helpers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/abc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/abc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/abc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/abc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/base_protocol.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/base_protocol.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/base_protocol.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/base_protocol.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_proto.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_proto.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_proto.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_proto.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_reqrep.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_reqrep.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_reqrep.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_reqrep.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_ws.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_ws.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/client_ws.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/client_ws.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/connector.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/connector.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/connector.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/connector.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/cookiejar.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/cookiejar.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/cookiejar.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/cookiejar.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/formdata.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/formdata.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/formdata.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/formdata.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/hdrs.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/hdrs.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/hdrs.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/hdrs.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/helpers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/helpers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/helpers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/helpers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_parser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_parser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_parser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_parser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_websocket.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_websocket.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_websocket.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_websocket.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_writer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_writer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/http_writer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/http_writer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/locks.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/locks.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/locks.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/locks.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/log.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/log.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/log.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/log.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/multipart.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/multipart.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/multipart.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/multipart.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload_streamer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload_streamer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/payload_streamer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/payload_streamer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/resolver.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/resolver.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/resolver.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/resolver.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/streams.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/streams.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/streams.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/streams.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tcp_helpers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tcp_helpers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tcp_helpers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tcp_helpers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tracing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tracing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/tracing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/tracing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/typedefs.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/typedefs.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/typedefs.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/typedefs.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_app.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_app.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_app.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_app.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_fileresponse.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_fileresponse.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_fileresponse.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_fileresponse.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_log.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_log.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_log.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_log.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_middlewares.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_middlewares.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_middlewares.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_middlewares.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_protocol.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_protocol.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_protocol.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_protocol.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_request.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_request.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_request.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_request.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_response.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_response.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_response.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_response.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_routedef.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_routedef.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_routedef.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_routedef.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_runner.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_runner.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_runner.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_runner.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_server.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_server.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_server.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_server.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_urldispatcher.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_urldispatcher.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_urldispatcher.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_urldispatcher.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_ws.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_ws.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/web_ws.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/web_ws.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/worker.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/worker.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiohttp/worker.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiohttp/worker.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiosignal/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiosignal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/aiosignal/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/aiosignal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/async_timeout/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/async_timeout/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/async_timeout/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/async_timeout/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/base_events.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/base_events.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/coroutines.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/coroutines.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/events.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/events.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/futures.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/futures.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/locks.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/locks.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/protocols.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/protocols.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/queues.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/queues.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/runners.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/runners.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/selector_events.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/selector_events.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/streams.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/streams.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/subprocess.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/subprocess.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/tasks.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/tasks.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/transports.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/transports.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/unix_events.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/asyncio/unix_events.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/_cmp.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/_cmp.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/_cmp.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/_cmp.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/_typing_compat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/_typing_compat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/_typing_compat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/_typing_compat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/_version_info.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/_version_info.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/_version_info.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/_version_info.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/converters.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/converters.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/converters.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/converters.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/filters.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/filters.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/filters.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/filters.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/setters.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/setters.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/setters.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/setters.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/validators.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/validators.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/attr/validators.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/attr/validators.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/cd.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/cd.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/cd.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/cd.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/constant.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/constant.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/constant.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/constant.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/legacy.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/legacy.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/legacy.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/legacy.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/md.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/md.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/md.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/md.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/models.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/models.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/models.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/models.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/assets/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/assets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/charset_normalizer/assets/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/charset_normalizer/assets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/collections/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/collections/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/collections/abc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/collections/abc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/process.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/process.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/thread.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/concurrent/futures/thread.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/ctypes/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/ctypes/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/curses/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/curses/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/curses/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/curses/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/charset.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/charset.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/contentmanager.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/contentmanager.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/errors.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/errors.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/feedparser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/feedparser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/feedparser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/feedparser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/header.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/header.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/header.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/message.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/message.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/message.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/parser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/parser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/parser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/parser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/policy.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/policy.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/email/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/email/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_catch.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_catch.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_catch.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_catch.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_formatting.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_formatting.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_formatting.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_formatting.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/exceptiongroup/_version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/exceptiongroup/_version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/frozenlist/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/frozenlist/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/frozenlist/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/frozenlist/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/html/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/html/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/html/entities.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/html/entities.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/client.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/client.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/client.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/client.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/cookiejar.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/cookiejar.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/cookiejar.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/cookiejar.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/cookies.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/cookies.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/cookies.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/cookies.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/server.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/server.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/http/server.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/http/server.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/abc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/abc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/machinery.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/machinery.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/util.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/util.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/metadata/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib/metadata/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_adapters.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_adapters.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_collections.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_collections.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_compat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_compat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_functools.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_functools.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_itertools.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_itertools.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_meta.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_meta.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_py39compat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_py39compat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_text.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/importlib_metadata/_text.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/iniconfig/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/iniconfig/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/iniconfig/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/iniconfig/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/iniconfig/_parse.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/iniconfig/_parse.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/iniconfig/_parse.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/iniconfig/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/iniconfig/exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/iniconfig/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/iniconfig/exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/iniconfig/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/_identifier.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/_identifier.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/_identifier.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/_identifier.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/async_utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/async_utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/async_utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/async_utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/bccache.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/bccache.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/bccache.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/bccache.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/compiler.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/compiler.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/compiler.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/compiler.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/constants.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/constants.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/constants.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/constants.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/debug.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/debug.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/debug.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/debug.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/defaults.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/defaults.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/defaults.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/defaults.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/environment.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/environment.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/environment.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/environment.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/exceptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/exceptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/ext.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/ext.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/ext.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/ext.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/filters.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/filters.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/filters.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/filters.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/idtracking.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/idtracking.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/idtracking.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/idtracking.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/lexer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/lexer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/lexer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/lexer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/loaders.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/loaders.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/loaders.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/loaders.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/nodes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/nodes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/nodes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/optimizer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/optimizer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/optimizer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/optimizer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/parser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/parser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/parser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/parser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/runtime.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/runtime.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/runtime.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/runtime.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/sandbox.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/sandbox.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/sandbox.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/sandbox.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/tests.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/tests.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/tests.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/tests.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/visitor.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/visitor.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/jinja2/visitor.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/jinja2/visitor.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/json/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/json/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/json/decoder.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/json/decoder.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/json/encoder.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/json/encoder.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/logging/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/logging/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/logging/config.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/logging/config.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/logging/config.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/logging/config.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/logging/handlers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/logging/handlers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/logging/handlers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/logging/handlers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/markupsafe/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/markupsafe/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/markupsafe/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/markupsafe/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_native.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_native.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_native.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_native.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_speedups.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_speedups.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/markupsafe/_speedups.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/markupsafe/_speedups.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multidict/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multidict/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multidict/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multidict/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/connection.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/connection.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/context.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/context.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/managers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/managers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/pool.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/pool.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_fork.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_fork.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_forkserver.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_forkserver.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/process.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/process.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/queues.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/queues.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/reduction.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/reduction.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/shared_memory.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/shared_memory.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/sharedctypes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/sharedctypes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/spawn.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/spawn.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/synchronize.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/synchronize.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/util.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/multiprocessing/util.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/_imports.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/_imports.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/_imports.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/_imports.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/_struct.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/_struct.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/_struct.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/_struct.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/_version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/_version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/_version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/_version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/converter.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/converter.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/converter.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/converter.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/json_compat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/json_compat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/json_compat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/json_compat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/notebooknode.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/notebooknode.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/notebooknode.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/notebooknode.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/reader.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/reader.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/reader.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/reader.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/sentinel.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/sentinel.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/sentinel.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/sentinel.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/validator.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/validator.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/validator.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/validator.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/warnings.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/warnings.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/warnings.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/words.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/words.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/corpus/words.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/corpus/words.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/convert.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/convert.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/convert.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/convert.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbjson.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbjson.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/nbjson.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/nbjson.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/rwbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/rwbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v1/rwbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v1/rwbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/convert.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/convert.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/convert.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/convert.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbjson.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbjson.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbjson.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbjson.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbpy.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbpy.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbpy.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbpy.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbxml.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbxml.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/nbxml.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/nbxml.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/rwbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/rwbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v2/rwbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v2/rwbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/convert.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/convert.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/convert.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/convert.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbjson.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbjson.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbjson.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbjson.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbpy.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbpy.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/nbpy.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/nbpy.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/rwbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/rwbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v3/rwbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v3/rwbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/convert.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/convert.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/convert.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/convert.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbjson.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbjson.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/nbjson.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/nbjson.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/rwbase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/rwbase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/nbformat/v4/rwbase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/nbformat/v4/rwbase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_pytesttester.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_pytesttester.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ctypeslib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ctypeslib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_add_docstring.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_add_docstring.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_array_like.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_array_like.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_callable.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_callable.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_char_codes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_char_codes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_dtype_like.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_dtype_like.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_extended_precision.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_extended_precision.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_generic_alias.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_generic_alias.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nbit.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nbit.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nested_sequence.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_nested_sequence.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_scalars.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_scalars.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_shape.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_shape.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_ufunc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/_typing/_ufunc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/_inspect.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/_inspect.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/py3k.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/compat/py3k.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_asarray.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_asarray.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_internal.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_internal.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_type_aliases.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_type_aliases.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_ufunc_config.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/_ufunc_config.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/arrayprint.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/arrayprint.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/defchararray.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/defchararray.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/einsumfunc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/einsumfunc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/fromnumeric.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/fromnumeric.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/function_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/function_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/multiarray.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/multiarray.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numeric.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numeric.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numerictypes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/numerictypes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/overrides.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/overrides.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/records.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/records.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/shape_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/shape_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/umath.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/core/umath.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/_pocketfft.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/_pocketfft.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/helper.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/fft/helper.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/_version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/_version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraypad.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraypad.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraysetops.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arraysetops.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arrayterator.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/arrayterator.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/format.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/format.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/function_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/function_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/histograms.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/histograms.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/index_tricks.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/index_tricks.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/mixins.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/mixins.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/nanfunctions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/nanfunctions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/npyio.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/npyio.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/polynomial.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/polynomial.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/scimath.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/scimath.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/shape_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/shape_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/stride_tricks.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/stride_tricks.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/twodim_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/twodim_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/type_check.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/type_check.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/ufunclike.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/ufunclike.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/lib/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/linalg.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/linalg/linalg.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/core.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/core.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/extras.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/extras.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/mrecords.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/ma/mrecords.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/defmatrix.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/matrixlib/defmatrix.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/_polybase.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/_polybase.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/chebyshev.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/chebyshev.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite_e.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/hermite_e.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/laguerre.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/laguerre.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/legendre.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/legendre.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polynomial.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polynomial.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polyutils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/polynomial/polyutils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_generator.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_generator.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_mt19937.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_mt19937.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_pcg64.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_pcg64.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_philox.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_philox.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_sfc64.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/_sfc64.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/bit_generator.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/bit_generator.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/mtrand.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/random/mtrand.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/testing/_private/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/typing/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/numpy/typing/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_requestor.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_requestor.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_requestor.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_requestor.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/error.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/error.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/error.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/error.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/object_classes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/object_classes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/object_classes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/object_classes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/openai_object.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/openai_object.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/openai_object.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/openai_object.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/openai_response.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/openai_response.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/openai_response.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/openai_response.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/util.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/util.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/util.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/util.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/audio.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/audio.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/audio.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/audio.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/chat_completion.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/chat_completion.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/chat_completion.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/chat_completion.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/completion.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/completion.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/completion.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/completion.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/customer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/customer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/customer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/customer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/deployment.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/deployment.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/deployment.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/deployment.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/edit.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/edit.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/edit.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/edit.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/embedding.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/embedding.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/embedding.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/embedding.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/engine.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/engine.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/engine.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/engine.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/error_object.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/error_object.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/error_object.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/error_object.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/file.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/file.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/file.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/file.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/fine_tune.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/fine_tune.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/fine_tune.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/fine_tune.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/image.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/image.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/image.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/image.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/model.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/model.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/model.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/model.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/moderation.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/moderation.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/moderation.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/moderation.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/api_resource.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/createable_api_resource.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/deletable_api_resource.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/engine_api_resource.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/listable_api_resource.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/nested_resource_class_methods.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/abstract/updateable_api_resource.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/api_resources/experimental/completion_config.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/common.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/common.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/common.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/common.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/numpy_helper.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/numpy_helper.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/openai/datalib/numpy_helper.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/openai/datalib/numpy_helper.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/os/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/os/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/os/path.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/os/path.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/os/path.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_elffile.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_elffile.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_manylinux.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_manylinux.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_musllinux.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_musllinux.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_parser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_parser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_parser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_structures.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_structures.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_tokenizer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_tokenizer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/_tokenizer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/_tokenizer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/markers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/markers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/markers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/markers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/requirements.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/requirements.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/requirements.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/requirements.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/specifiers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/specifiers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/tags.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/tags.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/packaging/version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_typing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_typing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_typing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/testing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/testing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/testing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/testing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/config.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/config.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_config/config.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_config/config.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/indexing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/indexing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/indexing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/indexing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/interval.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/interval.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/interval.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/interval.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/lib.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/lib.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/lib.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/lib.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/missing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/missing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/missing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/missing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/ops_dispatch.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/ops_dispatch.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/ops_dispatch.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/ops_dispatch.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/properties.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/properties.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/properties.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/properties.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/nattype.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/np_datetime.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/offsets.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/period.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/period.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/period.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/period.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_libs/tslibs/timestamps.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_testing/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/_testing/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/_testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/extensions/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/extensions/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/extensions/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/extensions/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/indexers/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/indexers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/indexers/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/indexers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/types/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/types/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/api/types/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/api/types/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/arrays/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/arrays/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/arrays/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/arrays/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/accessor.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/accessor.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/accessor.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/accessor.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/algorithms.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/algorithms.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/algorithms.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arraylike.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arraylike.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arraylike.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arraylike.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/construction.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/construction.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/construction.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/construction.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/frame.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/frame.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/frame.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/frame.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/generic.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/generic.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/generic.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/generic.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/resample.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/resample.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/resample.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/resample.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/series.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/series.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/series.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/series.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/strings.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/strings.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/strings.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/strings.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/boolean.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/boolean.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/boolean.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/boolean.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/categorical.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/categorical.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/categorical.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/categorical.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimelike.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimelike.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimelike.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimelike.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/datetimes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/datetimes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/floating.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/floating.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/floating.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/floating.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/integer.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/integer.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/integer.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/integer.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/interval.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/interval.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/interval.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/interval.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/masked.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/masked.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/masked.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/masked.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numeric.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numeric.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numeric.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numpy_.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numpy_.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/numpy_.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/numpy_.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/period.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/period.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/period.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/period.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/string_.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/string_.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/string_.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/string_.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/timedeltas.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/timedeltas.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/arrow/dtype.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/accessor.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/array.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/array.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/array.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/array.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/arrays/sparse/dtype.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/eval.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/eval.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/eval.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/eval.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/expr.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/expr.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/expr.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/expr.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/ops.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/ops.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/ops.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/ops.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/pytables.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/pytables.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/pytables.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/pytables.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/scope.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/scope.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/computation/scope.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/computation/scope.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/common.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/common.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/common.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/common.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/concat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/concat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/concat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/concat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/dtypes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/dtypes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/dtypes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/dtypes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/generic.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/generic.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/generic.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/generic.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/inference.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/inference.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/inference.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/inference.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/missing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/missing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/dtypes/missing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/dtypes/missing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/generic.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/generic.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/generic.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/generic.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/groupby.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/groupby.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/groupby.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/groupby.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/grouper.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/grouper.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/grouper.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/grouper.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/ops.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/ops.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/groupby/ops.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/groupby/ops.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/accessors.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/accessors.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/accessors.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/accessors.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/category.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/category.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/category.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/category.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimelike.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimelike.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimelike.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimelike.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/datetimes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/datetimes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/extension.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/extension.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/extension.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/extension.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/interval.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/interval.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/interval.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/interval.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/multi.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/multi.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/multi.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/multi.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/period.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/period.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/period.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/period.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/range.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/range.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/range.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/range.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/timedeltas.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/indexes/timedeltas.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/indexes/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/interchange/dataframe_protocol.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/concat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/concat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/concat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/concat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/encoding.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/encoding.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/encoding.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/encoding.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/melt.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/melt.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/melt.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/melt.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/merge.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/merge.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/merge.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/merge.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/pivot.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/pivot.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/pivot.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/pivot.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/tile.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/tile.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/reshape/tile.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/reshape/tile.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/datetimes.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/datetimes.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/datetimes.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/datetimes.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/numeric.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/numeric.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/numeric.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/timedeltas.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/tools/timedeltas.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/tools/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/hashing.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/hashing.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/util/hashing.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/util/hashing.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/ewm.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/ewm.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/ewm.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/ewm.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/expanding.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/expanding.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/expanding.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/expanding.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/rolling.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/rolling.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/core/window/rolling.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/core/window/rolling.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/errors/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/errors/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/errors/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/errors/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/clipboards.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/clipboards.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/clipboards.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/clipboards.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/common.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/common.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/common.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/common.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/feather_format.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/feather_format.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/feather_format.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/feather_format.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/gbq.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/gbq.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/gbq.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/gbq.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/html.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/html.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/html.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/html.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/orc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/orc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/orc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/orc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parquet.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parquet.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parquet.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parquet.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pickle.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pickle.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pickle.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pytables.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pytables.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/pytables.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/pytables.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/spss.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/spss.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/spss.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/spss.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sql.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sql.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sql.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sql.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/stata.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/stata.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/stata.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/stata.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/xml.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/xml.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/xml.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/xml.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/_base.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/_base.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/excel/_base.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/excel/_base.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/format.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/format.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/format.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/format.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style_render.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style_render.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/formats/style_render.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/formats/style_render.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_json.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_json.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_json.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_json.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_normalize.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_normalize.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_normalize.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_normalize.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_table_schema.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_table_schema.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/json/_table_schema.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/json/_table_schema.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/readers.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/readers.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/parsers/readers.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/parsers/readers.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas7bdat.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas7bdat.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas7bdat.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas7bdat.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas_xport.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas_xport.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sas_xport.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sas_xport.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sasreader.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sasreader.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/io/sas/sasreader.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/io/sas/sasreader.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_core.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_core.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_core.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_core.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_misc.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_misc.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/plotting/_misc.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/plotting/_misc.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/api.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/api.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/api.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/api.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/frequencies.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/frequencies.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/frequencies.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/frequencies.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/holiday.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/holiday.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/holiday.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/holiday.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/offsets.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/offsets.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/tseries/offsets.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/tseries/offsets.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_decorators.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_decorators.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_print_versions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_print_versions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_print_versions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_print_versions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_tester.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_tester.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pandas/util/_tester.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pandas/util/_tester.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pytest/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/pytest/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/_config.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/_config.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/_config.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/_config.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/ai.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/ai.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/ai.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/ai.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/explain.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/explain.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/explain.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/explain.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/llm.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/llm.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/llm.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/llm.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/runtime.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/runtime.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/runtime.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/runtime.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/prompt.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/prompt.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/prompt.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/prompt.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/relyonai/prompt/examples/make_prompt.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sqlite3/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sqlite3/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sqlite3/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sqlite3/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sqlite3/dbapi2.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/sqlite3/dbapi2.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/sqlite3/dbapi2.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/sqlite3/dbapi2.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/_asyncio.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/_asyncio.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/_asyncio.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/_asyncio.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/_utils.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/_utils.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/_utils.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/after.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/after.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/after.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/after.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/before.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/before.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/before.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/before.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/before_sleep.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/before_sleep.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/before_sleep.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/before_sleep.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/nap.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/nap.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/nap.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/nap.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/retry.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/retry.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/retry.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/retry.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/stop.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/stop.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/stop.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/stop.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/tornadoweb.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/tornadoweb.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/tornadoweb.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/tornadoweb.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/wait.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/wait.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tenacity/wait.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tenacity/wait.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/core.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/core.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/core.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/core.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/model.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/model.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/model.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/model.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/registry.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/registry.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tiktoken/registry.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tiktoken/registry.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/_parser.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/_parser.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/_parser.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/_re.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/_re.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/_re.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/_re.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/_types.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/_types.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tomli/_types.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tomli/_types.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/concurrent.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/concurrent.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/concurrent.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/concurrent.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/escape.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/escape.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/escape.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/escape.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/gen.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/gen.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/gen.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/gen.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/ioloop.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/ioloop.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/ioloop.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/ioloop.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/iostream.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/iostream.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/iostream.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/iostream.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/log.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/log.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/log.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/log.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/netutil.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/netutil.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/netutil.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/netutil.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/options.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/options.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/options.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/options.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/process.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/process.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/process.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/process.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/util.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/util.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/util.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/util.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/asyncio.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/asyncio.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/tornado/platform/asyncio.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/tornado/platform/asyncio.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/_version.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/_version.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/_version.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/_version.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/log.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/log.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/log.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/log.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/traitlets.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/traitlets.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/traitlets.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/traitlets.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/application.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/application.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/application.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/application.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/argcomplete_config.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/argcomplete_config.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/argcomplete_config.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/argcomplete_config.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/configurable.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/configurable.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/configurable.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/configurable.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/loader.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/loader.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/config/loader.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/config/loader.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/bunch.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/bunch.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/bunch.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/bunch.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/decorators.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/decorators.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/decorators.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/descriptions.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/descriptions.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/descriptions.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/descriptions.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/getargspec.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/getargspec.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/getargspec.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/getargspec.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/importstring.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/importstring.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/importstring.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/importstring.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/nested_update.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/nested_update.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/nested_update.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/nested_update.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/sentinel.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/sentinel.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/sentinel.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/sentinel.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/text.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/text.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/traitlets/utils/text.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/traitlets/utils/text.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/async_case.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/async_case.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/case.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/case.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/loader.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/loader.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/main.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/main.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/result.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/result.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/runner.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/runner.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/signals.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/signals.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/suite.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/unittest/suite.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/error.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/error.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/error.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/error.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/parse.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/parse.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/request.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/request.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/request.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/request.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/response.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/response.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/urllib/response.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/urllib/response.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/yarl/__init__.data.json` & `relyonai-0.1.2/.mypy_cache/3.8/yarl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.mypy_cache/3.8/yarl/__init__.meta.json` & `relyonai-0.1.2/.mypy_cache/3.8/yarl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/.vscode/extensions.list` & `relyonai-0.1.2/.vscode/extensions.list`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/nbs/test.ipynb` & `relyonai-0.1.2/nbs/test.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/_config.py` & `relyonai-0.1.2/relyonai/_config.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/ai.py` & `relyonai-0.1.2/relyonai/ai.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/explain.py` & `relyonai-0.1.2/relyonai/explain.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/llm.py` & `relyonai-0.1.2/relyonai/llm.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/runtime.py` & `relyonai-0.1.2/relyonai/runtime.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/utils.py` & `relyonai-0.1.2/relyonai/utils.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/prompt.json` & `relyonai-0.1.2/relyonai/prompt/prompt.json`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/prompt.py` & `relyonai-0.1.2/relyonai/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/consts.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/consts.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/env.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/env.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/error_fixing.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/error_fixing.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/errors.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/errors.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/exploration.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/exploration.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/files.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/files.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/format.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/format.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/funcs1.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/funcs1.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/funcs2.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/funcs2.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/funcs3.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/funcs3.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/gpt.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/gpt.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/imports.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/imports.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/lambdas.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/lambdas.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/make_prompt.py` & `relyonai-0.1.2/relyonai/prompt/examples/make_prompt.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/plt.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/plt.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/session.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/session.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/examples/template.ipynb` & `relyonai-0.1.2/relyonai/prompt/examples/template.ipynb`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/schemas/NEW_SCHEMA.md` & `relyonai-0.1.2/relyonai/prompt/schemas/NEW_SCHEMA.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/schemas/SCHEMA.md` & `relyonai-0.1.2/relyonai/prompt/schemas/SCHEMA.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/schemas/SIMPLER_SCHEMA.md` & `relyonai-0.1.2/relyonai/prompt/schemas/SIMPLER_SCHEMA.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/system/default.md` & `relyonai-0.1.2/relyonai/prompt/system/default.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/system/gpt4-refined.md` & `relyonai-0.1.2/relyonai/prompt/system/gpt4-refined.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/system/gpt4.md` & `relyonai-0.1.2/relyonai/prompt/system/gpt4.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/system/simpler.md` & `relyonai-0.1.2/relyonai/prompt/system/simpler.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/relyonai/prompt/system/simpler2.md` & `relyonai-0.1.2/relyonai/prompt/system/simpler2.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/tests/conftest.py` & `relyonai-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/tests/ai/single/test_args.py` & `relyonai-0.1.2/tests/ai/single/test_args.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/tests/ai/single/test_files.py` & `relyonai-0.1.2/tests/ai/single/test_files.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/tests/ai/single/test_funcs.py` & `relyonai-0.1.2/tests/ai/single/test_funcs.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/tests/ai/single/test_imports.py` & `relyonai-0.1.2/tests/ai/single/test_imports.py`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/tests/data/cities.csv` & `relyonai-0.1.2/tests/data/cities.csv`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/LICENSE` & `relyonai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/README.md` & `relyonai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `relyonai-0.1.1/pyproject.toml` & `relyonai-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "relyonai"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Stanislav Beliaev", email="its@stanb.me" },
 ]
-description = "Inline AI in your Python code"
+description = "Python Runtime Inline AI Calls"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `relyonai-0.1.1/PKG-INFO` & `relyonai-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: relyonai
-Version: 0.1.1
-Summary: Inline AI in your Python code
+Version: 0.1.2
+Summary: Python Runtime Inline AI Calls
 Author-email: Stanislav Beliaev <its@stanb.me>
 License-File: LICENSE
 Keywords: ai,gpt3,openai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

