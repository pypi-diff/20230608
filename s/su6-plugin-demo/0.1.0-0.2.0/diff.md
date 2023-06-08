# Comparing `tmp/su6_plugin_demo-0.1.0.tar.gz` & `tmp/su6_plugin_demo-0.2.0.tar.gz`

## Comparing `su6_plugin_demo-0.1.0.tar` & `su6_plugin_demo-0.2.0.tar`

### file list

```diff
@@ -1,889 +1,903 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/coverage.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/concurrency.data.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/concurrency.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    31386 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    27042 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/android.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/android.meta.json
--rw-r--r--   0        0        0    42264 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/unix.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/unix.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    82230 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    25025 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    55926 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0    18124 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/plugins.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/plugins.meta.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__about__.data.json
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__about__.meta.json
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__init__.data.json
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__init__.meta.json
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/cli.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/cli.meta.json
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/135f8502ea9220c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/16eb1e86ada927dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/1afe977825bc8a10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/1b3305298f982534
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/2105dd59821b0d2e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/218849aea14bb786
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/4459258ff34f7a6a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/4556b560cac380c6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/462cd0acebb2bad8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/482afb837807ad1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/4c913a3ca84bfcf0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/573f5af59ab10b19
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/5836aa819cc0bd0b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/5dc27c75087b09cf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/73eb44bc4a1696d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/815146cef1b2bb8a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/871084f147ddc392
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/89e3964695c8e5d2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/a922bf74d693355f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/add6734d1fca1ff5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/c4bc4955397f04d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/d1faf4bb55eec9e1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/e2bb878c09be8933
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/e9910029ab815bf0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/f1bcac0fc961af24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.ruff_cache/content/f55b43e31f7a1838
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/d_f23488167c00d510___about___py.html
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/d_f23488167c00d510___init___py.html
--rw-r--r--   0        0        0    11223 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/d_f23488167c00d510_cli_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/htmlcov/style.css
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/src/su6_plugin_demo/__about__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/src/su6_plugin_demo/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/src/su6_plugin_demo/cli.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/tests/test_about.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/tests/test_cli.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/README.md
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 su6_plugin_demo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/coverage.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/concurrency.data.json
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/concurrency.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    31386 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    27042 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    42264 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/unix.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/unix.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    82230 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    25156 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    66379 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0    45711 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/plugins.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/plugins.meta.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__about__.data.json
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__about__.meta.json
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__init__.data.json
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__init__.meta.json
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/cli.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/cli.meta.json
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/135f8502ea9220c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/16eb1e86ada927dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/1afe977825bc8a10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/1b3305298f982534
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/2105dd59821b0d2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/218849aea14bb786
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/32f03cb90ec9c97a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/382f7e1cf71d0aff
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/4459258ff34f7a6a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/4556b560cac380c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/462cd0acebb2bad8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/482afb837807ad1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/4a3ff6993294da2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/4c913a3ca84bfcf0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/573f5af59ab10b19
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/5836aa819cc0bd0b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/5dc27c75087b09cf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/73eb44bc4a1696d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/7ca2fb09fa912048
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/801fee28656cff61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/815146cef1b2bb8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/871084f147ddc392
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/89e3964695c8e5d2
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/98b0e80c1bd54491
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/9b853a4841f3affd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/a922bf74d693355f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/add6734d1fca1ff5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/bc0f6d653dbb88c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/bc11703377c50cc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/c4bc4955397f04d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/d1faf4bb55eec9e1
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/db201377b8e8a5d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/e00ea88e92b38c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/e2bb878c09be8933
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/e9910029ab815bf0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/f1bcac0fc961af24
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/f1da827436c251dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.ruff_cache/content/f55b43e31f7a1838
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/examples/cli_from_docs.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/d_f23488167c00d510___about___py.html
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/d_f23488167c00d510___init___py.html
+-rw-r--r--   0        0        0    23792 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/d_f23488167c00d510_cli_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/htmlcov/style.css
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/src/su6_plugin_demo/__about__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/src/su6_plugin_demo/__init__.py
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/src/su6_plugin_demo/cli.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/tests/test_about.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/README.md
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 su6_plugin_demo-0.2.0/PKG-INFO
```

### Comparing `su6_plugin_demo-0.1.0/coverage.svg` & `su6_plugin_demo-0.2.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/__future__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/__future__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ast.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ast.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_codecs.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_codecs.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_collections_abc.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_collections_abc.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_csv.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_csv.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ctypes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_ctypes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_decimal.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_decimal.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_operator.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_operator.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_random.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_random.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_socket.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_socket.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_stat.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_stat.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_thread.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_thread.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_warnings.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_warnings.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakref.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakref.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakrefset.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_weakrefset.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/abc.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/abc.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/argparse.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/argparse.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/array.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/array.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ast.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ast.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/builtins.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/builtins.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/codecs.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/codecs.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/colorsys.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/colorsys.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/configparser.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/configparser.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextlib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextlib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextvars.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/contextvars.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/copy.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/copy.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/copyreg.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/copyreg.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/csv.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/csv.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/dataclasses.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/dataclasses.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/datetime.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/datetime.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/decimal.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/decimal.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/difflib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/difflib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/dis.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/dis.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/enum.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/enum.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/errno.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/errno.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/fractions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/fractions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/functools.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/functools.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/genericpath.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/genericpath.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/getpass.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/getpass.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/gettext.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/gettext.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/glob.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/glob.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/hashlib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/hashlib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/hmac.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/hmac.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/inspect.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/inspect.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/io.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/io.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/itertools.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/itertools.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/linecache.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/linecache.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/marshal.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/marshal.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/math.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/math.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mmap.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mmap.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/msvcrt.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/msvcrt.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mypy_extensions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mypy_extensions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/numbers.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/numbers.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/opcode.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/opcode.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/operator.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/operator.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathlib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathlib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pickle.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pickle.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platform.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platform.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/posixpath.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/posixpath.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pty.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pty.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pydoc.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pydoc.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/queue.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/queue.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/random.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/random.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/re.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/re.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/reprlib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/reprlib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/secrets.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/secrets.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/selectors.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/selectors.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/shlex.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/shlex.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/shutil.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/shutil.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/signal.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/signal.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/socket.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/socket.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_compile.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_compile.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_constants.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_constants.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_parse.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sre_parse.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ssl.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ssl.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/stat.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/stat.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/string.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/string.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/struct.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/struct.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/subprocess.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/subprocess.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sys.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sys.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sysconfig.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/sysconfig.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tempfile.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tempfile.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/termios.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/termios.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/textwrap.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/textwrap.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/threading.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/threading.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/time.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/time.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/token.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/token.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tokenize.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tokenize.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tomllib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tomllib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/traceback.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/traceback.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tty.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/tty.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/types.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/types.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing_extensions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typing_extensions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/uuid.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/uuid.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/warnings.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/warnings.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/weakref.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/weakref.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/webbrowser.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/webbrowser.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/zlib.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/zlib.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/base_events.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/base_events.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/coroutines.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/events.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/events.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/exceptions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/futures.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/futures.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/locks.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/locks.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/mixins.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/mixins.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/protocols.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/protocols.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/queues.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/queues.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/runners.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/runners.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/selector_events.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/streams.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/streams.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/subprocess.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/tasks.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/tasks.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/threads.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/threads.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/timeouts.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/transports.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/transports.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/unix_events.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/_width_table.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/_width_table.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/brackets.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/brackets.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/cache.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/cache.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/comments.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/comments.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/concurrency.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/concurrency.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/const.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/const.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/files.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/files.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/linegen.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/linegen.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/lines.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/lines.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/mode.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/mode.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/nodes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/nodes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/numerics.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/numerics.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/output.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/output.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/parsing.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/parsing.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/report.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/report.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/rusty.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/rusty.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/strings.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/strings.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/trans.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/black/trans.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_compat.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_compat.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_textwrap.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/core.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/core.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/decorators.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/decorators.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/exceptions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/exceptions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/formatting.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/formatting.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/globals.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/globals.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/parser.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/parser.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/shell_completion.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/termui.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/termui.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/types.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/types.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/click/utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/abc.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/collections/abc.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/process.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/charset.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/charset.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/contentmanager.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/errors.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/errors.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/header.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/header.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/message.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/message.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/policy.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/email/policy.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/entities.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/html/entities.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/abc.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/abc.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/machinery.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/util.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/util.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/decoder.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/decoder.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/encoder.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/json/encoder.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/logging/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/logging/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/main.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/token.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_format.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_url.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/connection.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/context.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/context.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/managers.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/pool.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/process.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/process.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/queues.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/util.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/multiprocessing/util.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/path.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/os/path.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_elffile.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_elffile.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_manylinux.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_musllinux.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_structures.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/_structures.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/specifiers.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/specifiers.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/tags.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/tags.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/version.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/packaging/version.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/_meta.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/_meta.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/gitignore.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pathspec.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pattern.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/pattern.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/util.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/util.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/android.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/android.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/android.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/android.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/api.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/api.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/unix.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/unix.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/unix.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/unix.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/version.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/platformdirs/version.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__main__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/__main__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_export_format.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_extension.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_extension.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_fileno.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_inspect.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_log_render.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_loop.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_loop.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_null_file.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_palettes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_pick.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_pick.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_ratio.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_spinners.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_stack.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_stack.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_timer.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_timer.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_wrap.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/abc.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/abc.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/align.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/align.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/ansi.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/ansi.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/box.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/box.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/cells.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/cells.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/columns.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/columns.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/console.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/console.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/constrain.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/constrain.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/containers.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/containers.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/control.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/control.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/default_styles.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/emoji.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/emoji.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/errors.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/errors.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/highlighter.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/json.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/json.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/jupyter.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live_render.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/live_render.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markdown.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markdown.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markup.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/markup.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/measure.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/measure.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/padding.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/padding.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pager.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pager.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/palette.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/palette.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/panel.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/panel.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pretty.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/pretty.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/protocol.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/protocol.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/region.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/region.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/repr.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/repr.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/rule.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/rule.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/scope.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/scope.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/screen.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/screen.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/segment.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/segment.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/spinner.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/spinner.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/status.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/status.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/style.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/style.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/styled.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/styled.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/syntax.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/syntax.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/table.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/table.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/text.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/text.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/theme.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/theme.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/themes.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/themes.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/traceback.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/rich/traceback.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__about__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__about__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'hash'": "'bf760abac17b289a34bd4287600ad1382f1d856965973489dc49e04abc19dc21'",*

 * * "'mtime'": '1686083692'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "73e8fed372900169f1c9959efc8f6f4282f5ebcb9b9a1eefe4d0c02e63fc7362",
+    "hash": "bf760abac17b289a34bd4287600ad1382f1d856965973489dc49e04abc19dc21",
     "id": "su6.__about__",
     "ignore_all": true,
     "interface_hash": "12dd0e316978457d5448b2c1f641c4ec906a7394ec32e3890a3909c003b4605a",
-    "mtime": 1685961721,
+    "mtime": 1686083692,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__init__.data.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8477678571428572%*

 * *Differences: {"'_fullname'": "'su6_plugin_demo'",*

 * * "'names'": "{'__annotations__': {'node': {'fullname': 'su6_plugin_demo.__annotations__'}}, "*

 * *            "'__doc__': {'node': {'fullname': 'su6_plugin_demo.__doc__'}}, '__file__': {'node': "*

 * *            "{'fullname': 'su6_plugin_demo.__file__'}}, '__name__': {'node': {'fullname': "*

 * *            "'su6_plugin_demo.__name__'}}, '__package__': {'node': {'fullname': "*

 * *            "'su6_plugin_demo.__package__'}}, '__path__': {'node': {'fullname': "*

 * *            "'su6_plugin_de […]*

```diff
@@ -1,24 +1,24 @@
 {
     ".class": "MypyFile",
-    "_fullname": "su6",
+    "_fullname": "su6_plugin_demo",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.__annotations__",
+                "fullname": "su6_plugin_demo.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -35,80 +35,73 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.__doc__",
+                "fullname": "su6_plugin_demo.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.__file__",
+                "fullname": "su6_plugin_demo.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.__name__",
+                "fullname": "su6_plugin_demo.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.__package__",
+                "fullname": "su6_plugin_demo.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
         "__path__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.__path__",
+                "fullname": "su6_plugin_demo.__path__",
                 "name": "__path__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str"
                     ],
                     "type_ref": "builtins.list"
                 }
             }
-        },
-        "app": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "su6.cli.app",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
         }
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/__init__.py"
+    "path": "src/su6_plugin_demo/__init__.py"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7416666666666667%*

 * *Differences: {"'data_mtime'": '1685630893',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [0]}',*

 * * "'hash'": "'7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f'",*

 * * "'id'": "'typer.colors'",*

 * * "'interface_hash'": "'27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25'",*

 * * "'mtime'": '1685549646',*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py'",*

 * * "'size'": '430'}*

```diff
@@ -1,32 +1,29 @@
 {
-    "data_mtime": 1685631350,
+    "data_mtime": 1685630893,
     "dep_lines": [
-        9,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "su6.cli",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "cab9864f675f6c76c8579e49a2ea81629110297e5cafd6028bf9b9873113a865",
-    "id": "su6",
+    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
+    "id": "typer.colors",
     "ignore_all": true,
-    "interface_hash": "16acb7e7984dd61da7176eb0ea9b4cf19db74cf2f44d2fddab4d3308c1ffd510",
-    "mtime": 1685961721,
+    "interface_hash": "27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25",
+    "mtime": 1685549646,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -60,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/__init__.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py",
     "plugin_data": null,
-    "size": 236,
+    "size": 430,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/cli.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/cli.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986945346320347%*

 * *Differences: {"'names'": "{'T_directory': {'node': {'line': 44}}, 'Singleton': OrderedDict([('.class', "*

 * *            "'SymbolTableNode'), ('cross_ref', 'su6.core.Singleton'), ('kind', 'Gdef'), "*

 * *            "('module_hidden', True), ('module_public', False)])}"}*

```diff
@@ -80,23 +80,30 @@
         "RED_CIRCLE": {
             ".class": "SymbolTableNode",
             "cross_ref": "su6.core.RED_CIRCLE",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "Singleton": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "su6.core.Singleton",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "T_directory": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.cli.T_directory",
-                "line": 43,
+                "line": 44,
                 "no_args": true,
                 "normalized": false,
                 "target": "builtins.str"
             }
         },
         "Verbosity": {
             ".class": "SymbolTableNode",
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/cli.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8314285714285714%*

 * *Differences: {"'data_mtime'": '1686083962',*

 * * "'dep_lines'": '{insert: [(3, 37)], delete: [3]}',*

 * * "'hash'": "'16fb93de7eda47d8ad825382a1fd91ef228e5ab9f5006bf0a170d8a76ab1dfce'",*

 * * "'interface_hash'": "'a81d3670ed68231e4c5d3f6214cb377c9a7cfc8cd96eb9007e90cbb039c9d15a'",*

 * * "'mtime'": '1686083692',*

 * * "'size'": '12385'}*

```diff
@@ -1,14 +1,14 @@
 {
-    "data_mtime": 1685631350,
+    "data_mtime": 1686083962,
     "dep_lines": [
         8,
         16,
         17,
-        36,
+        37,
         2,
         3,
         4,
         5,
         6,
         7,
         9,
@@ -102,19 +102,19 @@
         "pickle",
         "typer.core",
         "typer.main",
         "typer.models",
         "types",
         "typing_extensions"
     ],
-    "hash": "d67f3a679a54a6b9004143688d8a8167dee82769073766aab12d65715e937590",
+    "hash": "16fb93de7eda47d8ad825382a1fd91ef228e5ab9f5006bf0a170d8a76ab1dfce",
     "id": "su6.cli",
     "ignore_all": true,
-    "interface_hash": "e81cf6314fd38d203b721a651dc678921d4bbe6be815b1f84e78b7a1aab5e4b0",
-    "mtime": 1685961721,
+    "interface_hash": "a81d3670ed68231e4c5d3f6214cb377c9a7cfc8cd96eb9007e90cbb039c9d15a",
+    "mtime": 1686083692,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -150,14 +150,14 @@
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
     "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/cli.py",
     "plugin_data": null,
-    "size": 12356,
+    "size": 12385,
     "suppressed": [
         "plumbum.machines",
         "plumbum"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/core.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/core.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996832017904226%*

 * *Differences: {"'names'": "{'ApplicationState': {'node': {'metadata': {'dataclass': {'attributes': {0: {'line': "*

 * *            "569}, 1: {'line': 570}, 2: {'line': 571}, 3: {'line': 572}}}}, 'names': "*

 * *            "{'__post_init__': OrderedDict([('.class', 'SymbolTableNode'), ('kind', 'Mdef'), "*

 * *            "('node', OrderedDict([('.class', 'FuncDef'), ('abstract_status', 0), ('arg_kinds', "*

 * *            "[0]), ('arg_names', ['self']), ('dataclass_transform_spec', None), ('flags', []), "*

 * *            "('fullname', 'su6.core […]*

```diff
@@ -2,14 +2,114 @@
     ".class": "MypyFile",
     "_fullname": "su6.core",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
+        "AbstractConfig": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "builtins.object"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": "su6.core.Singleton",
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "su6.core.AbstractConfig",
+                    "name": "AbstractConfig",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [],
+                "fullname": "su6.core.AbstractConfig",
+                "has_param_spec_type": false,
+                "metaclass_type": "su6.core.Singleton",
+                "metadata": {},
+                "module_name": "su6.core",
+                "mro": [
+                    "su6.core.AbstractConfig",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
+                    "update": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                1,
+                                4
+                            ],
+                            "arg_names": [
+                                "self",
+                                "strict",
+                                "kw"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.AbstractConfig.update",
+                            "name": "update",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    1,
+                                    4
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "strict",
+                                    "kw"
+                                ],
+                                "arg_types": [
+                                    "su6.core.AbstractConfig",
+                                    "builtins.bool",
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "update of AbstractConfig",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
+            }
+        },
         "ApplicationState": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
@@ -37,39 +137,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 503,
+                                "line": 569,
                                 "name": "verbosity",
                                 "type": "su6.core.Verbosity"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 504,
+                                "line": 570,
                                 "name": "output_format",
                                 "type": "su6.core.Format"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 505,
+                                "line": 571,
                                 "name": "config_file",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.str",
                                         {
                                             ".class": "NoneType"
@@ -81,15 +181,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 506,
+                                "line": 572,
                                 "name": "config",
                                 "type": {
                                     ".class": "TypeAliasType",
                                     "args": [],
                                     "type_ref": "su6.core.MaybeConfig"
                                 }
                             }
@@ -262,14 +362,242 @@
                                     ],
                                     "type_ref": "builtins.tuple"
                                 }
                             }
                         },
                         "plugin_generated": true
                     },
+                    "__post_init__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.ApplicationState.__post_init__",
+                            "name": "__post_init__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "su6.core.ApplicationState"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__post_init__ of ApplicationState",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "_get_plugin_specific_config_from_raw": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "self",
+                                "key"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.ApplicationState._get_plugin_specific_config_from_raw",
+                            "name": "_get_plugin_specific_config_from_raw",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "key"
+                                ],
+                                "arg_types": [
+                                    "su6.core.ApplicationState",
+                                    "builtins.str"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "_get_plugin_specific_config_from_raw of ApplicationState",
+                                "ret_type": {
+                                    ".class": "Instance",
+                                    "args": [
+                                        "builtins.str",
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    ],
+                                    "type_ref": "builtins.dict"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "_plugins": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "explicit_self_type",
+                                "is_ready",
+                                "is_inferred"
+                            ],
+                            "fullname": "su6.core.ApplicationState._plugins",
+                            "name": "_plugins",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    "builtins.str",
+                                    "su6.core.AbstractConfig"
+                                ],
+                                "type_ref": "builtins.dict"
+                            }
+                        }
+                    },
+                    "_setup_plugin_config_defaults": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.ApplicationState._setup_plugin_config_defaults",
+                            "name": "_setup_plugin_config_defaults",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "su6.core.ApplicationState"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "_setup_plugin_config_defaults of ApplicationState",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "attach_plugin_config": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "self",
+                                "name",
+                                "config_cls"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.ApplicationState.attach_plugin_config",
+                            "name": "attach_plugin_config",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "name",
+                                    "config_cls"
+                                ],
+                                "arg_types": [
+                                    "su6.core.ApplicationState",
+                                    "builtins.str",
+                                    "su6.core.AbstractConfig"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "attach_plugin_config of ApplicationState",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
                     "config": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
@@ -304,14 +632,57 @@
                                     {
                                         ".class": "NoneType"
                                     }
                                 ]
                             }
                         }
                     },
+                    "get_config": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.ApplicationState.get_config",
+                            "name": "get_config",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "su6.core.ApplicationState"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "get_config of ApplicationState",
+                                "ret_type": "su6.core.Config",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
                     "load_config": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
@@ -508,65 +879,65 @@
             "kind": "Gdef",
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
                 "alt_promote": null,
                 "bases": [
-                    "builtins.object"
+                    "su6.core.AbstractConfig"
                 ],
                 "dataclass_transform_spec": null,
                 "declared_metaclass": null,
                 "defn": {
                     ".class": "ClassDef",
                     "fullname": "su6.core.Config",
                     "name": "Config",
                     "type_vars": []
                 },
                 "deletable_attributes": [],
                 "flags": [],
                 "fullname": "su6.core.Config",
                 "has_param_spec_type": false,
-                "metaclass_type": null,
+                "metaclass_type": "su6.core.Singleton",
                 "metadata": {
                     "dataclass": {
                         "attributes": [
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 283,
+                                "line": 332,
                                 "name": "directory",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 284,
+                                "line": 333,
                                 "name": "pyproject",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 285,
+                                "line": 334,
                                 "name": "include",
                                 "type": {
                                     ".class": "Instance",
                                     "args": [
                                         "builtins.str"
                                     ],
                                     "type_ref": "builtins.list"
@@ -576,15 +947,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 286,
+                                "line": 335,
                                 "name": "exclude",
                                 "type": {
                                     ".class": "Instance",
                                     "args": [
                                         "builtins.str"
                                     ],
                                     "type_ref": "builtins.list"
@@ -594,27 +965,27 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 287,
+                                "line": 336,
                                 "name": "stop_after_first_failure",
                                 "type": "builtins.bool"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 290,
+                                "line": 339,
                                 "name": "coverage",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.float",
                                         {
                                             ".class": "NoneType"
@@ -626,15 +997,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 291,
+                                "line": 340,
                                 "name": "badge",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.bool",
                                         "builtins.str"
                                     ]
@@ -644,14 +1015,15 @@
                         "frozen": false
                     },
                     "dataclass_tag": {}
                 },
                 "module_name": "su6.core",
                 "mro": [
                     "su6.core.Config",
+                    "su6.core.AbstractConfig",
                     "builtins.object"
                 ],
                 "names": {
                     ".class": "SymbolTable",
                     "__dataclass_fields__": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
@@ -898,14 +1270,42 @@
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
+                    "__raw": {
+                        ".class": "SymbolTableNode",
+                        "implicit": true,
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "explicit_self_type",
+                                "is_ready",
+                                "is_inferred"
+                            ],
+                            "fullname": "su6.core.Config.__raw",
+                            "name": "__raw",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    "builtins.str",
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "type_ref": "builtins.dict"
+                            }
+                        }
+                    },
                     "badge": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
@@ -1184,14 +1584,69 @@
                                 "args": [
                                     "builtins.str"
                                 ],
                                 "type_ref": "builtins.list"
                             }
                         }
                     },
+                    "get_raw": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.Config.get_raw",
+                            "name": "get_raw",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "su6.core.Config"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "get_raw of Config",
+                                "ret_type": {
+                                    ".class": "Instance",
+                                    "args": [
+                                        "builtins.str",
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    ],
+                                    "type_ref": "builtins.dict"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
                     "include": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
@@ -1220,14 +1675,76 @@
                                 "has_explicit_value"
                             ],
                             "fullname": "su6.core.Config.pyproject",
                             "name": "pyproject",
                             "type": "builtins.str"
                         }
                     },
+                    "set_raw": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "self",
+                                "raw"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.Config.set_raw",
+                            "name": "set_raw",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "raw"
+                                ],
+                                "arg_types": [
+                                    "su6.core.Config",
+                                    {
+                                        ".class": "Instance",
+                                        "args": [
+                                            "builtins.str",
+                                            {
+                                                ".class": "AnyType",
+                                                "missing_import_name": null,
+                                                "source_any": null,
+                                                "type_of_any": 2
+                                            }
+                                        ],
+                                        "type_ref": "builtins.dict"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "set_raw of Config",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
                     "stop_after_first_failure": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
@@ -1278,27 +1795,27 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 340,
+                                "line": 404,
                                 "name": "key",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 341,
+                                "line": 405,
                                 "name": "value",
                                 "type": {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
                                     "type_of_any": 2
                                 }
@@ -1307,15 +1824,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 342,
+                                "line": 406,
                                 "name": "expected_type",
                                 "type": "builtins.type"
                             }
                         ],
                         "frozen": false
                     },
                     "dataclass_tag": {}
@@ -1956,15 +2473,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.MaybeConfig",
-                "line": 315,
+                "line": 379,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "su6.core.Config",
                         {
@@ -2060,14 +2577,238 @@
                     "has_explicit_value"
                 ],
                 "fullname": "su6.core.RED_CIRCLE",
                 "name": "RED_CIRCLE",
                 "type": "builtins.str"
             }
         },
+        "Singleton": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "builtins.type"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": null,
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "su6.core.Singleton",
+                    "name": "Singleton",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [],
+                "fullname": "su6.core.Singleton",
+                "has_param_spec_type": false,
+                "metaclass_type": null,
+                "metadata": {},
+                "module_name": "su6.core",
+                "mro": [
+                    "su6.core.Singleton",
+                    "builtins.type",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
+                    "__call__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                2,
+                                4
+                            ],
+                            "arg_names": [
+                                "self",
+                                "args",
+                                "kwargs"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.Singleton.__call__",
+                            "name": "__call__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    2,
+                                    4
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "args",
+                                    "kwargs"
+                                ],
+                                "arg_types": [
+                                    "su6.core.Singleton",
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    },
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__call__ of Singleton",
+                                "ret_type": {
+                                    ".class": "TypeType",
+                                    "item": {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "_instances": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "su6.core.Singleton._instances",
+                            "name": "_instances",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    {
+                                        ".class": "TypeType",
+                                        "item": {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    },
+                                    {
+                                        ".class": "TypeType",
+                                        "item": {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    }
+                                ],
+                                "type_ref": "builtins.dict"
+                            }
+                        }
+                    },
+                    "clear": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [],
+                                "arg_names": [],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_static",
+                                    "is_decorated"
+                                ],
+                                "fullname": "su6.core.Singleton.clear",
+                                "name": "clear",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [],
+                                    "arg_names": [],
+                                    "arg_types": [],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": null
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "clear of Singleton",
+                                    "ret_type": {
+                                        ".class": "NoneType"
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_staticmethod",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "su6.core.Singleton.clear",
+                                "name": "clear",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [],
+                                    "arg_names": [],
+                                    "arg_types": [],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": null
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "clear of Singleton",
+                                    "ret_type": {
+                                        ".class": "NoneType"
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
+            }
+        },
         "T": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeVarExpr",
                 "fullname": "su6.core.T",
                 "name": "T",
@@ -2257,15 +2998,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_typelike",
-                "line": 317,
+                "line": 381,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.type",
                         "types.UnionType",
@@ -3854,21 +4595,14 @@
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "replace": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "dataclasses.replace",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "run_tool": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/core.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.64535729567822%*

 * *Differences: {"'data_mtime'": '1685631349',*

 * * "'dep_lines'": '{insert: [(1, 2), (3, 3), (4, 4)], delete: [37, 36, 35, 34, 29, 28, 27, 26, 25, '*

 * *                '24, 23, 22, 21, 20, 19, 18, 17, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, '*

 * *                '2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [37, 36, 35, 34, 32, 31, 30, 29, 28, 27, 26, 25, 24, 23, 22, 21, 20, 19, '*

 * *                '18, 17, 13, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.result'), (1, 'collections.abc'), (2, 'unittes […]*

```diff
@@ -1,130 +1,41 @@
 {
-    "data_mtime": 1685961045,
+    "data_mtime": 1685631349,
     "dep_lines": [
-        16,
-        4,
-        5,
-        6,
-        7,
-        8,
-        9,
-        10,
-        11,
-        12,
-        13,
-        14,
-        16,
-        18,
-        21,
-        22,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
+        2,
         1,
+        3,
+        4,
         1,
-        17,
-        17,
-        20,
-        17
+        1
     ],
     "dep_prios": [
         10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
         5,
         20,
-        10,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        10,
-        20,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "black.files",
-        "enum",
-        "functools",
-        "inspect",
-        "json",
-        "operator",
-        "os",
-        "sys",
-        "tomllib",
-        "types",
+        "unittest.result",
+        "collections.abc",
+        "unittest",
         "typing",
-        "dataclasses",
-        "black",
-        "typer",
-        "rich",
-        "typeguard",
+        "typing_extensions",
         "builtins",
-        "_collections_abc",
-        "_operator",
-        "_typeshed",
-        "abc",
-        "array",
-        "click",
-        "click.exceptions",
-        "ctypes",
-        "io",
-        "json.encoder",
-        "mmap",
-        "pickle",
-        "typeguard._config",
-        "typeguard._exceptions",
-        "typeguard._functions",
-        "typeguard._memo",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "74e6ec523bdb8c188119767bd49dc9a8c6a68110ef0a3b4843138e62067f01d5",
-    "id": "su6.core",
+    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
+    "id": "unittest.signals",
     "ignore_all": true,
-    "interface_hash": "939f6bef245b2bdbdbae683bbdd55cd6d10de1a2e9da4be892896b01e264fe75",
-    "mtime": 1685961721,
+    "interface_hash": "92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720",
+    "mtime": 1685549818,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -158,18 +69,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/core.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
     "plugin_data": null,
-    "size": 18001,
-    "suppressed": [
-        "plumbum.commands.processes",
-        "plumbum.commands",
-        "plumbum.machines",
-        "plumbum"
-    ],
+    "size": 488,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/plugins.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.720344387755102%*

 * *Differences: {"'_fullname'": "'typeguard._importhook'",*

 * * "'future_import_flags'": "['annotations']",*

 * * "'names'": "{'__annotations__': {'node': {'fullname': 'typeguard._importhook.__annotations__'}, "*

 * *            "delete: ['module_public']}, '__doc__': {'node': {'fullname': "*

 * *            "'typeguard._importhook.__doc__'}, delete: ['module_public']}, '__file__': {'node': "*

 * *            "{'fullname': 'typeguard._importhook.__file__'}, delete: ['module_public']}, "*

 * *            "'__name__': {'node': {'fullname': 'typeguard._i […]*

```diff
@@ -1,672 +1,1038 @@
 {
     ".class": "MypyFile",
-    "_fullname": "su6.plugins",
-    "future_import_flags": [],
+    "_fullname": "typeguard._importhook",
+    "future_import_flags": [
+        "annotations"
+    ],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
-        "PluginRegistration": {
+        "Any": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Any",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "Callable": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Callable",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "CodeType": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "types.CodeType",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "ImportHookManager": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
                 "alt_promote": null,
                 "bases": [
                     "builtins.object"
                 ],
                 "dataclass_transform_spec": null,
                 "declared_metaclass": null,
                 "defn": {
                     ".class": "ClassDef",
-                    "fullname": "su6.plugins.PluginRegistration",
-                    "name": "PluginRegistration",
+                    "fullname": "typeguard._importhook.ImportHookManager",
+                    "name": "ImportHookManager",
                     "type_vars": []
                 },
                 "deletable_attributes": [],
                 "flags": [],
-                "fullname": "su6.plugins.PluginRegistration",
+                "fullname": "typeguard._importhook.ImportHookManager",
                 "has_param_spec_type": false,
                 "metaclass_type": null,
-                "metadata": {
-                    "dataclass": {
-                        "attributes": [
-                            {
-                                "alias": null,
-                                "column": 4,
-                                "has_default": false,
-                                "is_in_init": true,
-                                "is_init_var": false,
-                                "is_neither_frozen_nor_nonfrozen": false,
-                                "kw_only": false,
-                                "line": 26,
-                                "name": "func",
-                                "type": {
-                                    ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "su6.core.T_Command"
-                                }
-                            },
-                            {
-                                "alias": null,
-                                "column": 4,
-                                "has_default": true,
-                                "is_in_init": true,
-                                "is_init_var": false,
-                                "is_neither_frozen_nor_nonfrozen": false,
-                                "kw_only": false,
-                                "line": 27,
-                                "name": "args",
-                                "type": {
-                                    ".class": "Instance",
-                                    "args": [
-                                        {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 2
-                                        }
-                                    ],
-                                    "type_ref": "builtins.tuple"
-                                }
-                            },
-                            {
-                                "alias": null,
-                                "column": 4,
-                                "has_default": true,
-                                "is_in_init": true,
-                                "is_init_var": false,
-                                "is_neither_frozen_nor_nonfrozen": false,
-                                "kw_only": false,
-                                "line": 28,
-                                "name": "kwargs",
-                                "type": {
-                                    ".class": "Instance",
-                                    "args": [
-                                        "builtins.str",
-                                        {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 2
-                                        }
-                                    ],
-                                    "type_ref": "builtins.dict"
-                                }
-                            }
-                        ],
-                        "frozen": false
-                    },
-                    "dataclass_tag": {}
-                },
-                "module_name": "su6.plugins",
+                "metadata": {},
+                "module_name": "typeguard._importhook",
                 "mro": [
-                    "su6.plugins.PluginRegistration",
+                    "typeguard._importhook.ImportHookManager",
                     "builtins.object"
                 ],
                 "names": {
                     ".class": "SymbolTable",
-                    "IS_SU6_REGISTRATION": {
+                    "__enter__": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
-                            ".class": "Decorator",
-                            "func": {
-                                ".class": "FuncDef",
-                                "abstract_status": 0,
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typeguard._importhook.ImportHookManager.__enter__",
+                            "name": "__enter__",
+                            "type": {
+                                ".class": "CallableType",
                                 "arg_kinds": [
                                     0
                                 ],
                                 "arg_names": [
-                                    "self"
+                                    null
                                 ],
-                                "dataclass_transform_spec": null,
-                                "flags": [
-                                    "is_property",
-                                    "is_decorated"
+                                "arg_types": [
+                                    "typeguard._importhook.ImportHookManager"
                                 ],
-                                "fullname": "su6.plugins.PluginRegistration.IS_SU6_REGISTRATION",
-                                "name": "IS_SU6_REGISTRATION",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        0
-                                    ],
-                                    "arg_names": [
-                                        "self"
-                                    ],
-                                    "arg_types": [
-                                        "su6.plugins.PluginRegistration"
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": "self"
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "IS_SU6_REGISTRATION of PluginRegistration",
-                                    "ret_type": "builtins.bool",
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
-                            },
-                            "is_overload": false,
-                            "var": {
-                                ".class": "Var",
-                                "flags": [
-                                    "is_initialized_in_class",
-                                    "is_property",
-                                    "is_ready",
-                                    "is_inferred"
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__enter__ of ImportHookManager",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "__exit__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0,
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                null,
+                                null,
+                                null,
+                                null
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typeguard._importhook.ImportHookManager.__exit__",
+                            "name": "__exit__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0,
+                                    0,
+                                    0
                                 ],
-                                "fullname": "su6.plugins.PluginRegistration.IS_SU6_REGISTRATION",
-                                "name": "IS_SU6_REGISTRATION",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        0
-                                    ],
-                                    "arg_names": [
-                                        "self"
-                                    ],
-                                    "arg_types": [
-                                        "su6.plugins.PluginRegistration"
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": "self"
+                                "arg_names": [
+                                    null,
+                                    null,
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    "typeguard._importhook.ImportHookManager",
+                                    {
+                                        ".class": "TypeType",
+                                        "item": "builtins.BaseException"
                                     },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "IS_SU6_REGISTRATION of PluginRegistration",
-                                    "ret_type": "builtins.bool",
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
+                                    "builtins.BaseException",
+                                    "types.TracebackType"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__exit__ of ImportHookManager",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
                             }
                         }
                     },
-                    "__call__": {
+                    "__init__": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
-                                2,
-                                4
+                                0
                             ],
                             "arg_names": [
                                 "self",
-                                "args",
-                                "kwargs"
+                                "hook"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "su6.plugins.PluginRegistration.__call__",
-                            "name": "__call__",
+                            "fullname": "typeguard._importhook.ImportHookManager.__init__",
+                            "name": "__init__",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
-                                    2,
-                                    4
+                                    0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "args",
-                                    "kwargs"
+                                    "hook"
                                 ],
                                 "arg_types": [
-                                    "su6.plugins.PluginRegistration",
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    },
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
+                                    "typeguard._importhook.ImportHookManager",
+                                    "importlib.abc.MetaPathFinder"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "__call__ of PluginRegistration",
+                                "name": "__init__ of ImportHookManager",
                                 "ret_type": {
-                                    ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "su6.core.T_Command_Return"
+                                    ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "__dataclass_fields__": {
+                    "hook": {
                         ".class": "SymbolTableNode",
+                        "implicit": true,
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
-                                "is_classvar",
-                                "is_ready"
+                                "is_inferred"
+                            ],
+                            "fullname": "typeguard._importhook.ImportHookManager.hook",
+                            "name": "hook",
+                            "type": "importlib.abc.MetaPathFinder"
+                        }
+                    },
+                    "uninstall": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
                             ],
-                            "fullname": "su6.plugins.PluginRegistration.__dataclass_fields__",
-                            "name": "__dataclass_fields__",
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typeguard._importhook.ImportHookManager.uninstall",
+                            "name": "uninstall",
                             "type": {
-                                ".class": "Instance",
-                                "args": [
-                                    "builtins.str",
-                                    {
-                                        ".class": "Instance",
-                                        "args": [
-                                            {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 2
-                                            }
-                                        ],
-                                        "type_ref": "dataclasses.Field"
-                                    }
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
                                 ],
-                                "type_ref": "builtins.dict"
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "typeguard._importhook.ImportHookManager"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "uninstall of ImportHookManager",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
                             }
-                        },
-                        "plugin_generated": true
-                    },
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
+            }
+        },
+        "Iterable": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Iterable",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "MetaPathFinder": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "importlib.abc.MetaPathFinder",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "ModuleSpec": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "importlib.machinery.ModuleSpec",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "ModuleType": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "types.ModuleType",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "OPTIMIZATION": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "typeguard._importhook.OPTIMIZATION",
+                "name": "OPTIMIZATION",
+                "type": "builtins.str"
+            }
+        },
+        "P": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "ParamSpecExpr",
+                "fullname": "typeguard._importhook.P",
+                "name": "P",
+                "upper_bound": "builtins.object",
+                "variance": 0
+            }
+        },
+        "PackageNotFoundError": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "importlib.metadata.PackageNotFoundError",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "ParamSpec": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.ParamSpec",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "PathLike": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "os.PathLike",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "PickleBuffer": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "pickle.PickleBuffer",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "Sequence": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Sequence",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "SourceFileLoader": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "importlib.machinery.SourceFileLoader",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "T": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeVarExpr",
+                "fullname": "typeguard._importhook.T",
+                "name": "T",
+                "upper_bound": "builtins.object",
+                "values": [],
+                "variance": 0
+            }
+        },
+        "TYPE_CHECKING": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.TYPE_CHECKING",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "TracebackType": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "types.TracebackType",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "TypeVar": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.TypeVar",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "TypeguardFinder": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "importlib.abc.MetaPathFinder"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": null,
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "typeguard._importhook.TypeguardFinder",
+                    "name": "TypeguardFinder",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [],
+                "fullname": "typeguard._importhook.TypeguardFinder",
+                "has_param_spec_type": false,
+                "metaclass_type": "abc.ABCMeta",
+                "metadata": {},
+                "module_name": "typeguard._importhook",
+                "mro": [
+                    "typeguard._importhook.TypeguardFinder",
+                    "importlib.abc.MetaPathFinder",
+                    "importlib.abc.Finder",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
                     "__init__": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
                                 0,
-                                1,
-                                1
+                                0
                             ],
                             "arg_names": [
                                 "self",
-                                "func",
-                                "args",
-                                "kwargs"
+                                "packages",
+                                "original_pathfinder"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "su6.plugins.PluginRegistration.__init__",
+                            "fullname": "typeguard._importhook.TypeguardFinder.__init__",
                             "name": "__init__",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
                                     0,
-                                    1,
-                                    1
+                                    0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "func",
-                                    "args",
-                                    "kwargs"
+                                    "packages",
+                                    "original_pathfinder"
                                 ],
                                 "arg_types": [
-                                    "su6.plugins.PluginRegistration",
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6.core.T_Command"
-                                    },
+                                    "typeguard._importhook.TypeguardFinder",
                                     {
-                                        ".class": "Instance",
-                                        "args": [
+                                        ".class": "UnionType",
+                                        "items": [
                                             {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 2
-                                            }
-                                        ],
-                                        "type_ref": "builtins.tuple"
-                                    },
-                                    {
-                                        ".class": "Instance",
-                                        "args": [
-                                            "builtins.str",
+                                                ".class": "Instance",
+                                                "args": [
+                                                    "builtins.str"
+                                                ],
+                                                "type_ref": "builtins.list"
+                                            },
                                             {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 2
+                                                ".class": "NoneType"
                                             }
-                                        ],
-                                        "type_ref": "builtins.dict"
-                                    }
+                                        ]
+                                    },
+                                    "importlib.abc.MetaPathFinder"
                                 ],
                                 "bound_args": [],
-                                "def_extras": {},
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "__init__ of PluginRegistration",
+                                "name": "__init__ of TypeguardFinder",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
-                        },
-                        "plugin_generated": true
+                        }
                     },
-                    "__match_args__": {
+                    "_original_pathfinder": {
                         ".class": "SymbolTableNode",
+                        "implicit": true,
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
-                                "is_ready",
-                                "allow_incompatible_override"
+                                "is_inferred"
+                            ],
+                            "fullname": "typeguard._importhook.TypeguardFinder._original_pathfinder",
+                            "name": "_original_pathfinder",
+                            "type": "importlib.abc.MetaPathFinder"
+                        }
+                    },
+                    "find_spec": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0,
+                                0,
+                                1
                             ],
-                            "fullname": "su6.plugins.PluginRegistration.__match_args__",
-                            "name": "__match_args__",
+                            "arg_names": [
+                                "self",
+                                "fullname",
+                                "path",
+                                "target"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typeguard._importhook.TypeguardFinder.find_spec",
+                            "name": "find_spec",
                             "type": {
-                                ".class": "TupleType",
-                                "implicit": false,
-                                "items": [
-                                    {
-                                        ".class": "LiteralType",
-                                        "fallback": "builtins.str",
-                                        "value": "func"
-                                    },
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0,
+                                    0,
+                                    1
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "fullname",
+                                    "path",
+                                    "target"
+                                ],
+                                "arg_types": [
+                                    "typeguard._importhook.TypeguardFinder",
+                                    "builtins.str",
                                     {
-                                        ".class": "LiteralType",
-                                        "fallback": "builtins.str",
-                                        "value": "args"
+                                        ".class": "UnionType",
+                                        "items": [
+                                            {
+                                                ".class": "Instance",
+                                                "args": [
+                                                    "builtins.str"
+                                                ],
+                                                "type_ref": "typing.Sequence"
+                                            },
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
                                     },
                                     {
-                                        ".class": "LiteralType",
-                                        "fallback": "builtins.str",
-                                        "value": "kwargs"
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "types.ModuleType",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
                                     }
                                 ],
-                                "partial_fallback": {
-                                    ".class": "Instance",
-                                    "args": [
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "find_spec of TypeguardFinder",
+                                "ret_type": {
+                                    ".class": "UnionType",
+                                    "items": [
+                                        "importlib.machinery.ModuleSpec",
                                         {
-                                            ".class": "AnyType",
-                                            "missing_import_name": null,
-                                            "source_any": null,
-                                            "type_of_any": 6
+                                            ".class": "NoneType"
                                         }
-                                    ],
-                                    "type_ref": "builtins.tuple"
-                                }
+                                    ]
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
                             }
-                        },
-                        "plugin_generated": true
+                        }
                     },
-                    "args": {
+                    "packages": {
                         ".class": "SymbolTableNode",
+                        "implicit": true,
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
-                                "is_initialized_in_class",
-                                "is_ready",
-                                "has_explicit_value"
+                                "is_inferred"
                             ],
-                            "fullname": "su6.plugins.PluginRegistration.args",
-                            "name": "args",
+                            "fullname": "typeguard._importhook.TypeguardFinder.packages",
+                            "name": "packages",
                             "type": {
-                                ".class": "Instance",
-                                "args": [
+                                ".class": "UnionType",
+                                "items": [
+                                    {
+                                        ".class": "Instance",
+                                        "args": [
+                                            "builtins.str"
+                                        ],
+                                        "type_ref": "builtins.list"
+                                    },
                                     {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
+                                        ".class": "NoneType"
                                     }
-                                ],
-                                "type_ref": "builtins.tuple"
+                                ]
                             }
                         }
                     },
-                    "func": {
+                    "should_instrument": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_property",
-                                "is_settable_property",
-                                "is_ready"
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
                             ],
-                            "fullname": "su6.plugins.PluginRegistration.func",
-                            "name": "func",
-                            "type": {
-                                ".class": "TypeAliasType",
-                                "args": [],
-                                "type_ref": "su6.core.T_Command"
-                            }
-                        }
-                    },
-                    "kwargs": {
-                        ".class": "SymbolTableNode",
-                        "kind": "Mdef",
-                        "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_initialized_in_class",
-                                "is_ready",
-                                "has_explicit_value"
+                            "arg_names": [
+                                "self",
+                                "module_name"
                             ],
-                            "fullname": "su6.plugins.PluginRegistration.kwargs",
-                            "name": "kwargs",
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typeguard._importhook.TypeguardFinder.should_instrument",
+                            "name": "should_instrument",
                             "type": {
-                                ".class": "Instance",
-                                "args": [
-                                    "builtins.str",
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
                                 ],
-                                "type_ref": "builtins.dict"
+                                "arg_names": [
+                                    "self",
+                                    "module_name"
+                                ],
+                                "arg_types": [
+                                    "typeguard._importhook.TypeguardFinder",
+                                    "builtins.str"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "should_instrument of TypeguardFinder",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
                             }
                         }
                     }
                 },
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
             }
         },
-        "T_Command": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.T_Command",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "T_Command_Return": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.T_Command_Return",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "T_Commands": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "module_public": false,
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "su6.plugins.T_Commands",
-                "line": 114,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "Instance",
-                    "args": [
-                        "su6.plugins.PluginRegistration"
-                    ],
-                    "type_ref": "builtins.list"
-                }
-            }
-        },
-        "T_Inner": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "module_public": false,
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "su6.plugins.T_Inner",
-                "line": 49,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0
-                    ],
-                    "arg_names": [
-                        null
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "TypeAliasType",
-                            "args": [],
-                            "type_ref": "su6.core.T_Command"
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {},
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": null,
-                    "ret_type": "su6.plugins.PluginRegistration",
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "T_Namespaces": {
+        "TypeguardLoader": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "su6.plugins.T_Namespaces",
-                "line": 118,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "Instance",
-                    "args": [
-                        "builtins.str",
-                        {
-                            ".class": "TupleType",
-                            "implicit": false,
-                            "items": [
-                                "typer.main.Typer",
-                                "builtins.str"
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    "importlib.machinery.SourceFileLoader"
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": null,
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "typeguard._importhook.TypeguardLoader",
+                    "name": "TypeguardLoader",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [],
+                "fullname": "typeguard._importhook.TypeguardLoader",
+                "has_param_spec_type": false,
+                "metaclass_type": "abc.ABCMeta",
+                "metadata": {},
+                "module_name": "typeguard._importhook",
+                "mro": [
+                    "typeguard._importhook.TypeguardLoader",
+                    "importlib.machinery.SourceFileLoader",
+                    "importlib.abc.FileLoader",
+                    "importlib.abc.SourceLoader",
+                    "importlib.abc.ResourceLoader",
+                    "importlib.abc.ExecutionLoader",
+                    "importlib.abc.InspectLoader",
+                    "importlib.abc.Loader",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
+                    "exec_module": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
                             ],
-                            "partial_fallback": {
-                                ".class": "Instance",
-                                "args": [
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 6
-                                    }
+                            "arg_names": [
+                                "self",
+                                "module"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "typeguard._importhook.TypeguardLoader.exec_module",
+                            "name": "exec_module",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
                                 ],
-                                "type_ref": "builtins.tuple"
+                                "arg_names": [
+                                    "self",
+                                    "module"
+                                ],
+                                "arg_types": [
+                                    "typeguard._importhook.TypeguardLoader",
+                                    "types.ModuleType"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "exec_module of TypeguardLoader",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
                             }
                         }
-                    ],
-                    "type_ref": "builtins.dict"
-                }
+                    },
+                    "source_to_code": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0,
+                                    1
+                                ],
+                                "arg_names": [
+                                    "data",
+                                    "path"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_static",
+                                    "is_decorated"
+                                ],
+                                "fullname": "typeguard._importhook.TypeguardLoader.source_to_code",
+                                "name": "source_to_code",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        1
+                                    ],
+                                    "arg_names": [
+                                        "data",
+                                        "path"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "UnionType",
+                                            "items": [
+                                                "builtins.bytes",
+                                                "builtins.bytearray",
+                                                "builtins.memoryview",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "AnyType",
+                                                            "missing_import_name": null,
+                                                            "source_any": null,
+                                                            "type_of_any": 2
+                                                        }
+                                                    ],
+                                                    "type_ref": "array.array"
+                                                },
+                                                "mmap.mmap",
+                                                "ctypes._CData",
+                                                "pickle.PickleBuffer",
+                                                "builtins.str",
+                                                "_ast.Module",
+                                                "_ast.Expression",
+                                                "_ast.Interactive"
+                                            ]
+                                        },
+                                        {
+                                            ".class": "UnionType",
+                                            "items": [
+                                                "builtins.bytes",
+                                                "builtins.bytearray",
+                                                "builtins.memoryview",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "AnyType",
+                                                            "missing_import_name": null,
+                                                            "source_any": null,
+                                                            "type_of_any": 2
+                                                        }
+                                                    ],
+                                                    "type_ref": "array.array"
+                                                },
+                                                "mmap.mmap",
+                                                "ctypes._CData",
+                                                "pickle.PickleBuffer",
+                                                "builtins.str",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        "builtins.str"
+                                                    ],
+                                                    "type_ref": "os.PathLike"
+                                                }
+                                            ]
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": null
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "source_to_code of TypeguardLoader",
+                                    "ret_type": "types.CodeType",
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_staticmethod",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "typeguard._importhook.TypeguardLoader.source_to_code",
+                                "name": "source_to_code",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        1
+                                    ],
+                                    "arg_names": [
+                                        "data",
+                                        "path"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "UnionType",
+                                            "items": [
+                                                "builtins.bytes",
+                                                "builtins.bytearray",
+                                                "builtins.memoryview",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "AnyType",
+                                                            "missing_import_name": null,
+                                                            "source_any": null,
+                                                            "type_of_any": 2
+                                                        }
+                                                    ],
+                                                    "type_ref": "array.array"
+                                                },
+                                                "mmap.mmap",
+                                                "ctypes._CData",
+                                                "pickle.PickleBuffer",
+                                                "builtins.str",
+                                                "_ast.Module",
+                                                "_ast.Expression",
+                                                "_ast.Interactive"
+                                            ]
+                                        },
+                                        {
+                                            ".class": "UnionType",
+                                            "items": [
+                                                "builtins.bytes",
+                                                "builtins.bytearray",
+                                                "builtins.memoryview",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "AnyType",
+                                                            "missing_import_name": null,
+                                                            "source_any": null,
+                                                            "type_of_any": 2
+                                                        }
+                                                    ],
+                                                    "type_ref": "array.array"
+                                                },
+                                                "mmap.mmap",
+                                                "ctypes._CData",
+                                                "pickle.PickleBuffer",
+                                                "builtins.str",
+                                                {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        "builtins.str"
+                                                    ],
+                                                    "type_ref": "os.PathLike"
+                                                }
+                                            ]
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": null
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "source_to_code of TypeguardLoader",
+                                    "ret_type": "types.CodeType",
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": null,
+                "type_vars": [],
+                "typeddict_type": null
             }
         },
-        "Typer": {
+        "TypeguardTransformer": {
             ".class": "SymbolTableNode",
-            "cross_ref": "typer.main.Typer",
+            "cross_ref": "typeguard._transformer.TypeguardTransformer",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "__all__": {
+        "_CData": {
             ".class": "SymbolTableNode",
+            "cross_ref": "ctypes._CData",
             "kind": "Gdef",
-            "module_public": false,
-            "node": {
-                ".class": "Var",
-                "flags": [
-                    "is_inferred",
-                    "has_explicit_value"
-                ],
-                "fullname": "su6.plugins.__all__",
-                "name": "__all__",
-                "type": {
-                    ".class": "Instance",
-                    "args": [
-                        "builtins.str"
-                    ],
-                    "type_ref": "builtins.list"
-                }
-            }
+            "module_hidden": true,
+            "module_public": false
         },
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.plugins.__annotations__",
+                "fullname": "typeguard._importhook.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -678,615 +1044,468 @@
                     "type_ref": "builtins.dict"
                 }
             }
         },
         "__doc__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.plugins.__doc__",
+                "fullname": "typeguard._importhook.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.plugins.__file__",
+                "fullname": "typeguard._importhook.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.plugins.__name__",
+                "fullname": "typeguard._importhook.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "su6.plugins.__package__",
+                "fullname": "typeguard._importhook.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "dataclass": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "dataclasses.dataclass",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "discover_plugins": {
+        "_call_with_frames_removed": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
-                "arg_kinds": [],
-                "arg_names": [],
+                "arg_kinds": [
+                    0,
+                    2,
+                    4
+                ],
+                "arg_names": [
+                    "f",
+                    "args",
+                    "kwargs"
+                ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6.plugins.discover_plugins",
-                "name": "discover_plugins",
+                "fullname": "typeguard._importhook._call_with_frames_removed",
+                "name": "_call_with_frames_removed",
                 "type": {
                     ".class": "CallableType",
-                    "arg_kinds": [],
-                    "arg_names": [],
-                    "arg_types": [],
+                    "arg_kinds": [
+                        0,
+                        2,
+                        4
+                    ],
+                    "arg_names": [
+                        "f",
+                        "args",
+                        "kwargs"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "CallableType",
+                            "arg_kinds": [
+                                2,
+                                4
+                            ],
+                            "arg_names": [
+                                null,
+                                null
+                            ],
+                            "arg_types": [
+                                {
+                                    ".class": "ParamSpecType",
+                                    "flavor": 1,
+                                    "fullname": "typeguard._importhook.P",
+                                    "id": -1,
+                                    "name": "P",
+                                    "prefix": {
+                                        ".class": "Parameters",
+                                        "arg_kinds": [],
+                                        "arg_names": [],
+                                        "arg_types": [],
+                                        "variables": []
+                                    },
+                                    "upper_bound": {
+                                        ".class": "Instance",
+                                        "args": [
+                                            "builtins.object"
+                                        ],
+                                        "type_ref": "builtins.tuple"
+                                    }
+                                },
+                                {
+                                    ".class": "ParamSpecType",
+                                    "flavor": 2,
+                                    "fullname": "typeguard._importhook.P",
+                                    "id": -1,
+                                    "name": "P",
+                                    "prefix": {
+                                        ".class": "Parameters",
+                                        "arg_kinds": [],
+                                        "arg_names": [],
+                                        "arg_types": [],
+                                        "variables": []
+                                    },
+                                    "upper_bound": {
+                                        ".class": "Instance",
+                                        "args": [
+                                            "builtins.str",
+                                            "builtins.object"
+                                        ],
+                                        "type_ref": "builtins.dict"
+                                    }
+                                }
+                            ],
+                            "bound_args": [],
+                            "def_extras": {},
+                            "fallback": "builtins.function",
+                            "from_concatenate": false,
+                            "implicit": false,
+                            "is_ellipsis_args": false,
+                            "name": null,
+                            "ret_type": {
+                                ".class": "TypeVarType",
+                                "fullname": "typeguard._importhook.T",
+                                "id": -2,
+                                "name": "T",
+                                "namespace": "",
+                                "upper_bound": "builtins.object",
+                                "values": [],
+                                "variance": 0
+                            },
+                            "type_guard": null,
+                            "unpack_kwargs": false,
+                            "variables": []
+                        },
+                        {
+                            ".class": "ParamSpecType",
+                            "flavor": 1,
+                            "fullname": "typeguard._importhook.P",
+                            "id": -1,
+                            "name": "P",
+                            "prefix": {
+                                ".class": "Parameters",
+                                "arg_kinds": [],
+                                "arg_names": [],
+                                "arg_types": [],
+                                "variables": []
+                            },
+                            "upper_bound": {
+                                ".class": "Instance",
+                                "args": [
+                                    "builtins.object"
+                                ],
+                                "type_ref": "builtins.tuple"
+                            }
+                        },
+                        {
+                            ".class": "ParamSpecType",
+                            "flavor": 2,
+                            "fullname": "typeguard._importhook.P",
+                            "id": -1,
+                            "name": "P",
+                            "prefix": {
+                                ".class": "Parameters",
+                                "arg_kinds": [],
+                                "arg_names": [],
+                                "arg_types": [],
+                                "variables": []
+                            },
+                            "upper_bound": {
+                                ".class": "Instance",
+                                "args": [
+                                    "builtins.str",
+                                    "builtins.object"
+                                ],
+                                "type_ref": "builtins.dict"
+                            }
+                        }
+                    ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "discover_plugins",
+                    "name": "_call_with_frames_removed",
                     "ret_type": {
-                        ".class": "TupleType",
-                        "implicit": false,
-                        "items": [
-                            {
-                                ".class": "TypeAliasType",
-                                "args": [],
-                                "type_ref": "su6.plugins.T_Namespaces"
-                            },
-                            {
-                                ".class": "TypeAliasType",
-                                "args": [],
-                                "type_ref": "su6.plugins.T_Commands"
-                            }
-                        ],
-                        "partial_fallback": {
-                            ".class": "Instance",
-                            "args": [
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 6
-                                }
-                            ],
-                            "type_ref": "builtins.tuple"
-                        }
+                        ".class": "TypeVarType",
+                        "fullname": "typeguard._importhook.T",
+                        "id": -2,
+                        "name": "T",
+                        "namespace": "",
+                        "upper_bound": "builtins.object",
+                        "values": [],
+                        "variance": 0
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
-                    "variables": []
+                    "variables": [
+                        {
+                            ".class": "ParamSpecType",
+                            "flavor": 0,
+                            "fullname": "typeguard._importhook.P",
+                            "id": -1,
+                            "name": "P",
+                            "prefix": {
+                                ".class": "Parameters",
+                                "arg_kinds": [],
+                                "arg_names": [],
+                                "arg_types": [],
+                                "variables": []
+                            },
+                            "upper_bound": "builtins.object"
+                        },
+                        {
+                            ".class": "TypeVarType",
+                            "fullname": "typeguard._importhook.T",
+                            "id": -2,
+                            "name": "T",
+                            "namespace": "",
+                            "upper_bound": "builtins.object",
+                            "values": [],
+                            "variance": 0
+                        }
+                    ]
                 }
             }
         },
-        "entry_points": {
+        "annotations": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "__future__.annotations",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "array": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "array.array",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "ast": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "ast",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "cache_from_source": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "importlib.util.cache_from_source",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "decode_source": {
             ".class": "SymbolTableNode",
-            "cross_ref": "importlib.metadata.entry_points",
+            "cross_ref": "importlib.util.decode_source",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "field": {
+        "global_config": {
             ".class": "SymbolTableNode",
-            "cross_ref": "dataclasses.field",
+            "cross_ref": "typeguard._config.global_config",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "include_plugins": {
+        "install_import_hook": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
-                    0,
-                    1
+                    1,
+                    5
                 ],
                 "arg_names": [
-                    "app",
-                    "_with_exit_code"
+                    "packages",
+                    "cls"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6.plugins.include_plugins",
-                "name": "include_plugins",
+                "fullname": "typeguard._importhook.install_import_hook",
+                "name": "install_import_hook",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
-                        0,
-                        1
+                        1,
+                        5
                     ],
                     "arg_names": [
-                        "app",
-                        "_with_exit_code"
+                        "packages",
+                        "cls"
                     ],
                     "arg_types": [
-                        "typer.main.Typer",
-                        "builtins.bool"
+                        {
+                            ".class": "UnionType",
+                            "items": [
+                                {
+                                    ".class": "Instance",
+                                    "args": [
+                                        "builtins.str"
+                                    ],
+                                    "type_ref": "typing.Iterable"
+                                },
+                                {
+                                    ".class": "NoneType"
+                                }
+                            ]
+                        },
+                        {
+                            ".class": "TypeType",
+                            "item": "typeguard._importhook.TypeguardFinder"
+                        }
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "include_plugins",
-                    "ret_type": {
-                        ".class": "NoneType"
-                    },
+                    "name": "install_import_hook",
+                    "ret_type": "typeguard._importhook.ImportHookManager",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "is_registration": {
+        "isclass": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "inspect.isclass",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "mmap": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "mmap.mmap",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
+        "optimized_cache_from_source": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
-                    0
+                    0,
+                    1
                 ],
                 "arg_names": [
-                    "something"
+                    "path",
+                    "debug_override"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "su6.plugins.is_registration",
-                "name": "is_registration",
+                "fullname": "typeguard._importhook.optimized_cache_from_source",
+                "name": "optimized_cache_from_source",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
-                        0
+                        0,
+                        1
                     ],
                     "arg_names": [
-                        "something"
+                        "path",
+                        "debug_override"
                     ],
                     "arg_types": [
+                        "builtins.str",
                         {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 2
+                            ".class": "UnionType",
+                            "items": [
+                                "builtins.bool",
+                                {
+                                    ".class": "NoneType"
+                                }
+                            ]
                         }
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "is_registration",
-                    "ret_type": "builtins.bool",
+                    "name": "optimized_cache_from_source",
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "register": {
+        "patch": {
             ".class": "SymbolTableNode",
+            "cross_ref": "unittest.mock.patch",
             "kind": "Gdef",
-            "node": {
-                ".class": "OverloadedFuncDef",
-                "flags": [],
-                "fullname": "su6.plugins.register",
-                "impl": {
-                    ".class": "FuncDef",
-                    "abstract_status": 0,
-                    "arg_kinds": [
-                        1,
-                        2,
-                        4
-                    ],
-                    "arg_names": [
-                        "func_outer",
-                        "a_outer",
-                        "kw_outer"
-                    ],
-                    "dataclass_transform_spec": null,
-                    "flags": [
-                        "is_overload"
-                    ],
-                    "fullname": "su6.plugins.register",
-                    "name": "register",
-                    "type": {
-                        ".class": "CallableType",
-                        "arg_kinds": [
-                            1,
-                            2,
-                            4
-                        ],
-                        "arg_names": [
-                            "func_outer",
-                            "a_outer",
-                            "kw_outer"
-                        ],
-                        "arg_types": [
-                            {
-                                ".class": "UnionType",
-                                "items": [
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6.core.T_Command"
-                                    },
-                                    {
-                                        ".class": "NoneType"
-                                    }
-                                ]
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 2
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 2
-                            }
-                        ],
-                        "bound_args": [],
-                        "def_extras": {
-                            "first_arg": null
-                        },
-                        "fallback": "builtins.function",
-                        "from_concatenate": false,
-                        "implicit": false,
-                        "is_ellipsis_args": false,
-                        "name": "register",
-                        "ret_type": {
-                            ".class": "UnionType",
-                            "items": [
-                                "su6.plugins.PluginRegistration",
-                                {
-                                    ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "su6.plugins.T_Inner"
-                                }
-                            ]
-                        },
-                        "type_guard": null,
-                        "unpack_kwargs": false,
-                        "variables": []
-                    }
-                },
-                "items": [
-                    {
-                        ".class": "Decorator",
-                        "func": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                1,
-                                2,
-                                4
-                            ],
-                            "arg_names": [
-                                "func_outer",
-                                "a_outer",
-                                "kw_outer"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [
-                                "is_overload",
-                                "is_decorated"
-                            ],
-                            "fullname": "su6.plugins.register",
-                            "name": "register",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    1,
-                                    2,
-                                    4
-                                ],
-                                "arg_names": [
-                                    "func_outer",
-                                    "a_outer",
-                                    "kw_outer"
-                                ],
-                                "arg_types": [
-                                    {
-                                        ".class": "NoneType"
-                                    },
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    },
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": null
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "register",
-                                "ret_type": {
-                                    ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "su6.plugins.T_Inner"
-                                },
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        },
-                        "is_overload": true,
-                        "var": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_inferred"
-                            ],
-                            "fullname": "su6.plugins.register",
-                            "name": "register",
-                            "type": null
-                        }
-                    },
-                    {
-                        ".class": "Decorator",
-                        "func": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                2,
-                                4
-                            ],
-                            "arg_names": [
-                                "func_outer",
-                                "a_outer",
-                                "kw_outer"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [
-                                "is_overload",
-                                "is_decorated"
-                            ],
-                            "fullname": "su6.plugins.register",
-                            "name": "register",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    2,
-                                    4
-                                ],
-                                "arg_names": [
-                                    "func_outer",
-                                    "a_outer",
-                                    "kw_outer"
-                                ],
-                                "arg_types": [
-                                    {
-                                        ".class": "TypeAliasType",
-                                        "args": [],
-                                        "type_ref": "su6.core.T_Command"
-                                    },
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    },
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
-                                    }
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": null
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "register",
-                                "ret_type": "su6.plugins.PluginRegistration",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        },
-                        "is_overload": true,
-                        "var": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_inferred"
-                            ],
-                            "fullname": "su6.plugins.register",
-                            "name": "register",
-                            "type": null
-                        }
-                    }
-                ],
-                "type": {
-                    ".class": "Overloaded",
-                    "items": [
-                        {
-                            ".class": "CallableType",
-                            "arg_kinds": [
-                                1,
-                                2,
-                                4
-                            ],
-                            "arg_names": [
-                                "func_outer",
-                                "a_outer",
-                                "kw_outer"
-                            ],
-                            "arg_types": [
-                                {
-                                    ".class": "NoneType"
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 2
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 2
-                                }
-                            ],
-                            "bound_args": [],
-                            "def_extras": {
-                                "first_arg": null
-                            },
-                            "fallback": "builtins.function",
-                            "from_concatenate": false,
-                            "implicit": false,
-                            "is_ellipsis_args": false,
-                            "name": "register",
-                            "ret_type": {
-                                ".class": "TypeAliasType",
-                                "args": [],
-                                "type_ref": "su6.plugins.T_Inner"
-                            },
-                            "type_guard": null,
-                            "unpack_kwargs": false,
-                            "variables": []
-                        },
-                        {
-                            ".class": "CallableType",
-                            "arg_kinds": [
-                                0,
-                                2,
-                                4
-                            ],
-                            "arg_names": [
-                                "func_outer",
-                                "a_outer",
-                                "kw_outer"
-                            ],
-                            "arg_types": [
-                                {
-                                    ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "su6.core.T_Command"
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 2
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 2
-                                }
-                            ],
-                            "bound_args": [],
-                            "def_extras": {
-                                "first_arg": null
-                            },
-                            "fallback": "builtins.function",
-                            "from_concatenate": false,
-                            "implicit": false,
-                            "is_ellipsis_args": false,
-                            "name": "register",
-                            "ret_type": "su6.plugins.PluginRegistration",
-                            "type_guard": null,
-                            "unpack_kwargs": false,
-                            "variables": []
-                        }
-                    ]
-                }
-            }
+            "module_hidden": true,
+            "module_public": false
         },
-        "run_tool": {
+        "sys": {
             ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.run_tool",
-            "kind": "Gdef"
+            "cross_ref": "sys",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
         },
-        "typing": {
+        "types": {
             ".class": "SymbolTableNode",
-            "cross_ref": "typing",
+            "cross_ref": "types",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "with_exit_code": {
+        "version": {
             ".class": "SymbolTableNode",
-            "cross_ref": "su6.core.with_exit_code",
+            "cross_ref": "importlib.metadata.version",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         }
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/plugins.py"
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_importhook.py"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6/plugins.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7018207282913165%*

 * *Differences: {"'data_mtime'": '1685631348',*

 * * "'dep_lines'": '{insert: [(1, 2)], delete: [8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [10, 9, 8, 7, 6, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections'), (4, 'array'), (5, 'ctypes'), (6, 'mmap'), (7, "*

 * *                   "'pickle')], delete: [15, 14, 13, 12, 11, 10, 9, 7, 6, 4, 3, 1, 0]}",*

 * * "'hash'": "'6483de895f8505de449b0d8469677616f96caf08b8a1cc13d9f54604802d1dc4'",*

 * * "'id'": "'typeguard._exceptions'",*

 * * "'interface_hash'": "'7164d489c8a069228ff9509d […]*

```diff
@@ -1,68 +1,44 @@
 {
-    "data_mtime": 1685961753,
+    "data_mtime": 1685631348,
     "dep_lines": [
-        6,
-        10,
-        4,
-        5,
-        8,
-        1,
-        1,
-        1,
-        1,
         1,
+        2,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        5,
         5,
-        5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "importlib.metadata",
-        "su6.core",
+        "collections",
         "typing",
-        "dataclasses",
-        "typer",
         "builtins",
-        "_collections_abc",
-        "_typeshed",
         "abc",
-        "click",
-        "click.core",
-        "importlib",
-        "typer.core",
-        "typer.main",
-        "types",
-        "typing_extensions"
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "7a2ae1e59b904c5180bf21c1fccd2d2eea3be06b46c45b488c6a977253f23aca",
-    "id": "su6.plugins",
+    "hash": "6483de895f8505de449b0d8469677616f96caf08b8a1cc13d9f54604802d1dc4",
+    "id": "typeguard._exceptions",
     "ignore_all": true,
-    "interface_hash": "42473b35f5c4fb68ff203df05d3089581a8b6f3c0420f6e08f970c952da717b2",
-    "mtime": 1685961721,
+    "interface_hash": "7164d489c8a069228ff9509d068c54e28e38f89ecd81c0d5fa9ce57a73956c11",
+    "mtime": 1685549645,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -96,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/plugins.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_exceptions.py",
     "plugin_data": null,
-    "size": 5309,
+    "size": 1121,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__about__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__about__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__about__.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685981933'}*

```diff
@@ -15,15 +15,15 @@
         "abc",
         "typing"
     ],
     "hash": "9be3ef0f22aa29ecfd1ccd45be9c44cbff0a9ac688e0299ed6ddc3b2248d0c09",
     "id": "su6_plugin_demo.__about__",
     "ignore_all": false,
     "interface_hash": "d2e2db94c73908a2ac1dfeba30b39914ccd397258431b92aa6cd5ac6417efc7b",
-    "mtime": 1685961400,
+    "mtime": 1685981933,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/su6_plugin_demo/cli.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/models.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6629318394024276%*

 * *Differences: {"'data_mtime'": '1685630895',*

 * * "'dep_lines'": '{insert: [(0, 18), (1, 22), (2, 24), (3, 25), (5, 2), (6, 3), (7, 16)], delete: '*

 * *                '[4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (2, 25), (3, 25), (4, 10), (5, 10), (7, 10)], delete: [6, 5, '*

 * *                '4, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._compat_utils'), (1, 'click.shell_completion'), (4, "*

 * *                   "'inspect'), (5, 'io'), (7, 'click'), (8, 'builtins'), (9, 'abc'), (10, "*

 * *                   "'click.core') […]*

```diff
@@ -1,53 +1,59 @@
 {
-    "data_mtime": 1685961753,
+    "data_mtime": 1685630895,
     "dep_lines": [
-        5,
-        8,
-        1,
-        1,
-        1,
-        1,
+        18,
+        22,
+        24,
+        25,
+        1,
+        2,
+        3,
+        16,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        25,
+        25,
+        25,
+        10,
+        10,
         5,
+        10,
         5,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "su6.plugins",
-        "typer",
+        "typer._compat_utils",
+        "click.shell_completion",
+        "typer.core",
+        "typer.main",
+        "inspect",
+        "io",
+        "typing",
+        "click",
         "builtins",
-        "_typeshed",
         "abc",
-        "click",
         "click.core",
-        "su6.core",
-        "typer.core",
-        "typer.main",
-        "typing"
+        "click.types",
+        "enum"
     ],
-    "hash": "fb39e4f2fac6f5c08de1be92c70120544f41b3d4bd1933785911549036abf58d",
-    "id": "su6_plugin_demo.cli",
-    "ignore_all": false,
-    "interface_hash": "2a2cb2b611aec10aba5003f5a7beccf37e44f5349e74cbf8b3486516df9a7fbc",
-    "mtime": 1685961756,
+    "hash": "0d625201001a209a45048efff3154017d132f4d3479b8755ea29f6b81ecdeca9",
+    "id": "typer.models",
+    "ignore_all": true,
+    "interface_hash": "239046e43ed828fba7030bdc4119029e194d6de90d24865db4033b0bab8d21c6",
+    "mtime": 1685549646,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -81,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6_plugin_demo/cli.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/models.py",
     "plugin_data": null,
-    "size": 1166,
+    "size": 15981,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_checkers.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_config.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_config.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_decorators.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7046620046620047%*

 * *Differences: {"'data_mtime'": '1685630893',*

 * * "'dep_lines'": '{insert: [(2, 3), (3, 4), (4, 7)], delete: [3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (4, 5), (5, 5)], delete: [5, 4, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (3, 'typing_extensions'), (4, "*

 * *                   "'types'), (6, '_typeshed')], delete: [7, 6, 5, 4, 0]}",*

 * * "'hash'": "'9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1'",*

 * * "'id'": "'urllib.parse'",*

 * * "'interface_hash'": "'02fb690cfa1baa81d991e1e0cbefb […]*

```diff
@@ -1,44 +1,44 @@
 {
-    "data_mtime": 1685631348,
+    "data_mtime": 1685630893,
     "dep_lines": [
-        1,
         2,
         1,
-        1,
-        1,
+        3,
+        4,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
         5,
         5,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "collections",
+        "collections.abc",
+        "sys",
         "typing",
+        "typing_extensions",
+        "types",
         "builtins",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "6483de895f8505de449b0d8469677616f96caf08b8a1cc13d9f54604802d1dc4",
-    "id": "typeguard._exceptions",
+    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
+    "id": "urllib.parse",
     "ignore_all": true,
-    "interface_hash": "7164d489c8a069228ff9509d068c54e28e38f89ecd81c0d5fa9ce57a73956c11",
-    "mtime": 1685549645,
+    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
+    "mtime": 1685549818,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_exceptions.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
     "plugin_data": null,
-    "size": 1121,
+    "size": 6532,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_functions.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_functions.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_importhook.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/result.data.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6549303683737646%*

 * *Differences: {"'_fullname'": "'unittest.result'",*

 * * "'future_import_flags'": '[]',*

 * * "'is_stub'": 'True',*

 * * "'names'": "{'__annotations__': {'node': {'fullname': 'unittest.result.__annotations__'}}, "*

 * *            "'__doc__': {'node': {'fullname': 'unittest.result.__doc__'}}, '__file__': {'node': "*

 * *            "{'fullname': 'unittest.result.__file__'}}, '__name__': {'node': {'fullname': "*

 * *            "'unittest.result.__name__'}}, '__package__': {'node': {'fullname': "*

 * *            "'unittest.result.__package__'}}, 'OptExcIn […]*

```diff
@@ -1,15 +1,13 @@
 {
     ".class": "MypyFile",
-    "_fullname": "typeguard._importhook",
-    "future_import_flags": [
-        "annotations"
-    ],
+    "_fullname": "unittest.result",
+    "future_import_flags": [],
     "is_partial_stub_package": false,
-    "is_stub": false,
+    "is_stub": true,
     "names": {
         ".class": "SymbolTable",
         "Any": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Any",
             "kind": "Gdef",
             "module_hidden": true,
@@ -18,1021 +16,1219 @@
         "Callable": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Callable",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "CodeType": {
+        "OptExcInfo": {
             ".class": "SymbolTableNode",
-            "cross_ref": "types.CodeType",
+            "cross_ref": "_typeshed.OptExcInfo",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "ImportHookManager": {
+        "STDERR_LINE": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready"
+                ],
+                "fullname": "unittest.result.STDERR_LINE",
+                "name": "STDERR_LINE",
+                "type": "builtins.str"
+            }
+        },
+        "STDOUT_LINE": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready"
+                ],
+                "fullname": "unittest.result.STDOUT_LINE",
+                "name": "STDOUT_LINE",
+                "type": "builtins.str"
+            }
+        },
+        "TestResult": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
                 "alt_promote": null,
                 "bases": [
                     "builtins.object"
                 ],
                 "dataclass_transform_spec": null,
                 "declared_metaclass": null,
                 "defn": {
                     ".class": "ClassDef",
-                    "fullname": "typeguard._importhook.ImportHookManager",
-                    "name": "ImportHookManager",
+                    "fullname": "unittest.result.TestResult",
+                    "name": "TestResult",
                     "type_vars": []
                 },
                 "deletable_attributes": [],
                 "flags": [],
-                "fullname": "typeguard._importhook.ImportHookManager",
+                "fullname": "unittest.result.TestResult",
                 "has_param_spec_type": false,
                 "metaclass_type": null,
                 "metadata": {},
-                "module_name": "typeguard._importhook",
+                "module_name": "unittest.result",
                 "mro": [
-                    "typeguard._importhook.ImportHookManager",
+                    "unittest.result.TestResult",
                     "builtins.object"
                 ],
                 "names": {
                     ".class": "SymbolTable",
-                    "__enter__": {
+                    "__init__": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
-                                0
+                                0,
+                                1,
+                                1,
+                                1
                             ],
                             "arg_names": [
-                                null
+                                "self",
+                                "stream",
+                                "descriptions",
+                                "verbosity"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.ImportHookManager.__enter__",
-                            "name": "__enter__",
+                            "fullname": "unittest.result.TestResult.__init__",
+                            "name": "__init__",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
-                                    0
+                                    0,
+                                    1,
+                                    1,
+                                    1
                                 ],
                                 "arg_names": [
-                                    null
+                                    "self",
+                                    "stream",
+                                    "descriptions",
+                                    "verbosity"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.ImportHookManager"
+                                    "unittest.result.TestResult",
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "typing.TextIO",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.bool",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.int",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "__enter__ of ImportHookManager",
+                                "name": "__init__ of TestResult",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "__exit__": {
+                    "addError": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
                                 0,
-                                0,
                                 0
                             ],
                             "arg_names": [
-                                null,
-                                null,
-                                null,
-                                null
+                                "self",
+                                "test",
+                                "err"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.ImportHookManager.__exit__",
-                            "name": "__exit__",
+                            "fullname": "unittest.result.TestResult.addError",
+                            "name": "addError",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
                                     0,
-                                    0,
                                     0
                                 ],
                                 "arg_names": [
-                                    null,
-                                    null,
-                                    null,
-                                    null
+                                    "self",
+                                    "test",
+                                    "err"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.ImportHookManager",
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase",
                                     {
-                                        ".class": "TypeType",
-                                        "item": "builtins.BaseException"
-                                    },
-                                    "builtins.BaseException",
-                                    "types.TracebackType"
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "_typeshed.OptExcInfo"
+                                    }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "__exit__ of ImportHookManager",
+                                "name": "addError of TestResult",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "__init__": {
+                    "addExpectedFailure": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
+                                0,
                                 0
                             ],
                             "arg_names": [
                                 "self",
-                                "hook"
+                                "test",
+                                "err"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.ImportHookManager.__init__",
-                            "name": "__init__",
+                            "fullname": "unittest.result.TestResult.addExpectedFailure",
+                            "name": "addExpectedFailure",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
+                                    0,
                                     0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "hook"
+                                    "test",
+                                    "err"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.ImportHookManager",
-                                    "importlib.abc.MetaPathFinder"
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "_typeshed.OptExcInfo"
+                                    }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "__init__ of ImportHookManager",
+                                "name": "addExpectedFailure of TestResult",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "hook": {
+                    "addFailure": {
                         ".class": "SymbolTableNode",
-                        "implicit": true,
                         "kind": "Mdef",
                         "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_inferred"
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0,
+                                0
                             ],
-                            "fullname": "typeguard._importhook.ImportHookManager.hook",
-                            "name": "hook",
-                            "type": "importlib.abc.MetaPathFinder"
+                            "arg_names": [
+                                "self",
+                                "test",
+                                "err"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.addFailure",
+                            "name": "addFailure",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "test",
+                                    "err"
+                                ],
+                                "arg_types": [
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "_typeshed.OptExcInfo"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "addFailure of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
                         }
                     },
-                    "uninstall": {
+                    "addSkip": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
+                                0,
+                                0,
                                 0
                             ],
                             "arg_names": [
-                                "self"
+                                "self",
+                                "test",
+                                "reason"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.ImportHookManager.uninstall",
-                            "name": "uninstall",
+                            "fullname": "unittest.result.TestResult.addSkip",
+                            "name": "addSkip",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
+                                    0,
+                                    0,
                                     0
                                 ],
                                 "arg_names": [
-                                    "self"
+                                    "self",
+                                    "test",
+                                    "reason"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.ImportHookManager"
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase",
+                                    "builtins.str"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "uninstall of ImportHookManager",
+                                "name": "addSkip of TestResult",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
-                    }
-                },
-                "self_type": null,
-                "slots": null,
-                "tuple_type": null,
-                "type_vars": [],
-                "typeddict_type": null
-            }
-        },
-        "Iterable": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.Iterable",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "MetaPathFinder": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "importlib.abc.MetaPathFinder",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "ModuleSpec": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "importlib.machinery.ModuleSpec",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "ModuleType": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "types.ModuleType",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "OPTIMIZATION": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "Var",
-                "flags": [
-                    "is_inferred",
-                    "has_explicit_value"
-                ],
-                "fullname": "typeguard._importhook.OPTIMIZATION",
-                "name": "OPTIMIZATION",
-                "type": "builtins.str"
-            }
-        },
-        "P": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "ParamSpecExpr",
-                "fullname": "typeguard._importhook.P",
-                "name": "P",
-                "upper_bound": "builtins.object",
-                "variance": 0
-            }
-        },
-        "PackageNotFoundError": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "importlib.metadata.PackageNotFoundError",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "ParamSpec": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.ParamSpec",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "PathLike": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "os.PathLike",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "PickleBuffer": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "pickle.PickleBuffer",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "Sequence": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.Sequence",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "SourceFileLoader": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "importlib.machinery.SourceFileLoader",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "T": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeVarExpr",
-                "fullname": "typeguard._importhook.T",
-                "name": "T",
-                "upper_bound": "builtins.object",
-                "values": [],
-                "variance": 0
-            }
-        },
-        "TYPE_CHECKING": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.TYPE_CHECKING",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "TracebackType": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "types.TracebackType",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "TypeVar": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.TypeVar",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "TypeguardFinder": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeInfo",
-                "_promote": [],
-                "abstract_attributes": [],
-                "alt_promote": null,
-                "bases": [
-                    "importlib.abc.MetaPathFinder"
-                ],
-                "dataclass_transform_spec": null,
-                "declared_metaclass": null,
-                "defn": {
-                    ".class": "ClassDef",
-                    "fullname": "typeguard._importhook.TypeguardFinder",
-                    "name": "TypeguardFinder",
-                    "type_vars": []
-                },
-                "deletable_attributes": [],
-                "flags": [],
-                "fullname": "typeguard._importhook.TypeguardFinder",
-                "has_param_spec_type": false,
-                "metaclass_type": "abc.ABCMeta",
-                "metadata": {},
-                "module_name": "typeguard._importhook",
-                "mro": [
-                    "typeguard._importhook.TypeguardFinder",
-                    "importlib.abc.MetaPathFinder",
-                    "importlib.abc.Finder",
-                    "builtins.object"
-                ],
-                "names": {
-                    ".class": "SymbolTable",
-                    "__init__": {
+                    },
+                    "addSubTest": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
                                 0,
+                                0,
                                 0
                             ],
                             "arg_names": [
                                 "self",
-                                "packages",
-                                "original_pathfinder"
+                                "test",
+                                "subtest",
+                                "err"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.TypeguardFinder.__init__",
-                            "name": "__init__",
+                            "fullname": "unittest.result.TestResult.addSubTest",
+                            "name": "addSubTest",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
                                     0,
+                                    0,
                                     0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "packages",
-                                    "original_pathfinder"
+                                    "test",
+                                    "subtest",
+                                    "err"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.TypeguardFinder",
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase",
+                                    "unittest.case.TestCase",
                                     {
                                         ".class": "UnionType",
                                         "items": [
                                             {
-                                                ".class": "Instance",
-                                                "args": [
-                                                    "builtins.str"
-                                                ],
-                                                "type_ref": "builtins.list"
+                                                ".class": "TypeAliasType",
+                                                "args": [],
+                                                "type_ref": "_typeshed.OptExcInfo"
                                             },
                                             {
                                                 ".class": "NoneType"
                                             }
                                         ]
-                                    },
-                                    "importlib.abc.MetaPathFinder"
+                                    }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "__init__ of TypeguardFinder",
+                                "name": "addSubTest of TestResult",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "_original_pathfinder": {
+                    "addSuccess": {
                         ".class": "SymbolTableNode",
-                        "implicit": true,
                         "kind": "Mdef",
                         "node": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_inferred"
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
                             ],
-                            "fullname": "typeguard._importhook.TypeguardFinder._original_pathfinder",
-                            "name": "_original_pathfinder",
-                            "type": "importlib.abc.MetaPathFinder"
+                            "arg_names": [
+                                "self",
+                                "test"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.addSuccess",
+                            "name": "addSuccess",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "test"
+                                ],
+                                "arg_types": [
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "addSuccess of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
                         }
                     },
-                    "find_spec": {
+                    "addUnexpectedSuccess": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
-                                0,
-                                0,
-                                1
+                                0
                             ],
                             "arg_names": [
                                 "self",
-                                "fullname",
-                                "path",
-                                "target"
+                                "test"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.TypeguardFinder.find_spec",
-                            "name": "find_spec",
+                            "fullname": "unittest.result.TestResult.addUnexpectedSuccess",
+                            "name": "addUnexpectedSuccess",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
-                                    0,
-                                    0,
-                                    1
+                                    0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "fullname",
-                                    "path",
-                                    "target"
+                                    "test"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.TypeguardFinder",
-                                    "builtins.str",
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "addUnexpectedSuccess of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "buffer": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.buffer",
+                            "name": "buffer",
+                            "type": "builtins.bool"
+                        }
+                    },
+                    "errors": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.errors",
+                            "name": "errors",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
                                     {
-                                        ".class": "UnionType",
+                                        ".class": "TupleType",
+                                        "implicit": false,
                                         "items": [
-                                            {
-                                                ".class": "Instance",
-                                                "args": [
-                                                    "builtins.str"
-                                                ],
-                                                "type_ref": "typing.Sequence"
-                                            },
-                                            {
-                                                ".class": "NoneType"
-                                            }
-                                        ]
-                                    },
+                                            "unittest.case.TestCase",
+                                            "builtins.str"
+                                        ],
+                                        "partial_fallback": {
+                                            ".class": "Instance",
+                                            "args": [
+                                                {
+                                                    ".class": "AnyType",
+                                                    "missing_import_name": null,
+                                                    "source_any": null,
+                                                    "type_of_any": 6
+                                                }
+                                            ],
+                                            "type_ref": "builtins.tuple"
+                                        }
+                                    }
+                                ],
+                                "type_ref": "builtins.list"
+                            }
+                        }
+                    },
+                    "expectedFailures": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.expectedFailures",
+                            "name": "expectedFailures",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
                                     {
-                                        ".class": "UnionType",
+                                        ".class": "TupleType",
+                                        "implicit": false,
                                         "items": [
-                                            "types.ModuleType",
-                                            {
-                                                ".class": "NoneType"
-                                            }
-                                        ]
+                                            "unittest.case.TestCase",
+                                            "builtins.str"
+                                        ],
+                                        "partial_fallback": {
+                                            ".class": "Instance",
+                                            "args": [
+                                                {
+                                                    ".class": "AnyType",
+                                                    "missing_import_name": null,
+                                                    "source_any": null,
+                                                    "type_of_any": 6
+                                                }
+                                            ],
+                                            "type_ref": "builtins.tuple"
+                                        }
                                     }
                                 ],
+                                "type_ref": "builtins.list"
+                            }
+                        }
+                    },
+                    "failfast": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.failfast",
+                            "name": "failfast",
+                            "type": "builtins.bool"
+                        }
+                    },
+                    "failures": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.failures",
+                            "name": "failures",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    {
+                                        ".class": "TupleType",
+                                        "implicit": false,
+                                        "items": [
+                                            "unittest.case.TestCase",
+                                            "builtins.str"
+                                        ],
+                                        "partial_fallback": {
+                                            ".class": "Instance",
+                                            "args": [
+                                                {
+                                                    ".class": "AnyType",
+                                                    "missing_import_name": null,
+                                                    "source_any": null,
+                                                    "type_of_any": 6
+                                                }
+                                            ],
+                                            "type_ref": "builtins.tuple"
+                                        }
+                                    }
+                                ],
+                                "type_ref": "builtins.list"
+                            }
+                        }
+                    },
+                    "printErrors": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.printErrors",
+                            "name": "printErrors",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "unittest.result.TestResult"
+                                ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "find_spec of TypeguardFinder",
+                                "name": "printErrors of TestResult",
                                 "ret_type": {
-                                    ".class": "UnionType",
-                                    "items": [
-                                        "importlib.machinery.ModuleSpec",
-                                        {
-                                            ".class": "NoneType"
-                                        }
-                                    ]
+                                    ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "packages": {
+                    "shouldStop": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.shouldStop",
+                            "name": "shouldStop",
+                            "type": "builtins.bool"
+                        }
+                    },
+                    "skipped": {
                         ".class": "SymbolTableNode",
-                        "implicit": true,
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
-                                "is_inferred"
+                                "is_initialized_in_class",
+                                "is_ready"
                             ],
-                            "fullname": "typeguard._importhook.TypeguardFinder.packages",
-                            "name": "packages",
+                            "fullname": "unittest.result.TestResult.skipped",
+                            "name": "skipped",
                             "type": {
-                                ".class": "UnionType",
-                                "items": [
+                                ".class": "Instance",
+                                "args": [
                                     {
-                                        ".class": "Instance",
-                                        "args": [
+                                        ".class": "TupleType",
+                                        "implicit": false,
+                                        "items": [
+                                            "unittest.case.TestCase",
                                             "builtins.str"
                                         ],
-                                        "type_ref": "builtins.list"
-                                    },
-                                    {
-                                        ".class": "NoneType"
+                                        "partial_fallback": {
+                                            ".class": "Instance",
+                                            "args": [
+                                                {
+                                                    ".class": "AnyType",
+                                                    "missing_import_name": null,
+                                                    "source_any": null,
+                                                    "type_of_any": 6
+                                                }
+                                            ],
+                                            "type_ref": "builtins.tuple"
+                                        }
                                     }
-                                ]
+                                ],
+                                "type_ref": "builtins.list"
                             }
                         }
                     },
-                    "should_instrument": {
+                    "startTest": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
                                 0
                             ],
                             "arg_names": [
                                 "self",
-                                "module_name"
+                                "test"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.TypeguardFinder.should_instrument",
-                            "name": "should_instrument",
+                            "fullname": "unittest.result.TestResult.startTest",
+                            "name": "startTest",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
                                     0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "module_name"
+                                    "test"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.TypeguardFinder",
-                                    "builtins.str"
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "should_instrument of TypeguardFinder",
-                                "ret_type": "builtins.bool",
+                                "name": "startTest of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
-                    }
-                },
-                "self_type": null,
-                "slots": null,
-                "tuple_type": null,
-                "type_vars": [],
-                "typeddict_type": null
-            }
-        },
-        "TypeguardLoader": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeInfo",
-                "_promote": [],
-                "abstract_attributes": [],
-                "alt_promote": null,
-                "bases": [
-                    "importlib.machinery.SourceFileLoader"
-                ],
-                "dataclass_transform_spec": null,
-                "declared_metaclass": null,
-                "defn": {
-                    ".class": "ClassDef",
-                    "fullname": "typeguard._importhook.TypeguardLoader",
-                    "name": "TypeguardLoader",
-                    "type_vars": []
-                },
-                "deletable_attributes": [],
-                "flags": [],
-                "fullname": "typeguard._importhook.TypeguardLoader",
-                "has_param_spec_type": false,
-                "metaclass_type": "abc.ABCMeta",
-                "metadata": {},
-                "module_name": "typeguard._importhook",
-                "mro": [
-                    "typeguard._importhook.TypeguardLoader",
-                    "importlib.machinery.SourceFileLoader",
-                    "importlib.abc.FileLoader",
-                    "importlib.abc.SourceLoader",
-                    "importlib.abc.ResourceLoader",
-                    "importlib.abc.ExecutionLoader",
-                    "importlib.abc.InspectLoader",
-                    "importlib.abc.Loader",
-                    "builtins.object"
-                ],
-                "names": {
-                    ".class": "SymbolTable",
-                    "exec_module": {
+                    },
+                    "startTestRun": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.startTestRun",
+                            "name": "startTestRun",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "unittest.result.TestResult"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "startTestRun of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "stop": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.stop",
+                            "name": "stop",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "unittest.result.TestResult"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "stop of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "stopTest": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
                                 0
                             ],
                             "arg_names": [
                                 "self",
-                                "module"
+                                "test"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
-                            "fullname": "typeguard._importhook.TypeguardLoader.exec_module",
-                            "name": "exec_module",
+                            "fullname": "unittest.result.TestResult.stopTest",
+                            "name": "stopTest",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
                                     0
                                 ],
                                 "arg_names": [
                                     "self",
-                                    "module"
+                                    "test"
                                 ],
                                 "arg_types": [
-                                    "typeguard._importhook.TypeguardLoader",
-                                    "types.ModuleType"
+                                    "unittest.result.TestResult",
+                                    "unittest.case.TestCase"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
-                                "name": "exec_module of TypeguardLoader",
+                                "name": "stopTest of TestResult",
                                 "ret_type": {
                                     ".class": "NoneType"
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
-                    "source_to_code": {
+                    "stopTestRun": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
-                            ".class": "Decorator",
-                            "func": {
-                                ".class": "FuncDef",
-                                "abstract_status": 0,
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.stopTestRun",
+                            "name": "stopTestRun",
+                            "type": {
+                                ".class": "CallableType",
                                 "arg_kinds": [
-                                    0,
-                                    1
+                                    0
                                 ],
                                 "arg_names": [
-                                    "data",
-                                    "path"
+                                    "self"
                                 ],
-                                "dataclass_transform_spec": null,
-                                "flags": [
-                                    "is_static",
-                                    "is_decorated"
-                                ],
-                                "fullname": "typeguard._importhook.TypeguardLoader.source_to_code",
-                                "name": "source_to_code",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        0,
-                                        1
-                                    ],
-                                    "arg_names": [
-                                        "data",
-                                        "path"
-                                    ],
-                                    "arg_types": [
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                "builtins.bytes",
-                                                "builtins.bytearray",
-                                                "builtins.memoryview",
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        {
-                                                            ".class": "AnyType",
-                                                            "missing_import_name": null,
-                                                            "source_any": null,
-                                                            "type_of_any": 2
-                                                        }
-                                                    ],
-                                                    "type_ref": "array.array"
-                                                },
-                                                "mmap.mmap",
-                                                "ctypes._CData",
-                                                "pickle.PickleBuffer",
-                                                "builtins.str",
-                                                "_ast.Module",
-                                                "_ast.Expression",
-                                                "_ast.Interactive"
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                "builtins.bytes",
-                                                "builtins.bytearray",
-                                                "builtins.memoryview",
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        {
-                                                            ".class": "AnyType",
-                                                            "missing_import_name": null,
-                                                            "source_any": null,
-                                                            "type_of_any": 2
-                                                        }
-                                                    ],
-                                                    "type_ref": "array.array"
-                                                },
-                                                "mmap.mmap",
-                                                "ctypes._CData",
-                                                "pickle.PickleBuffer",
-                                                "builtins.str",
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        "builtins.str"
-                                                    ],
-                                                    "type_ref": "os.PathLike"
-                                                }
-                                            ]
-                                        }
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": null
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "source_to_code of TypeguardLoader",
-                                    "ret_type": "types.CodeType",
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
-                            },
-                            "is_overload": false,
-                            "var": {
-                                ".class": "Var",
-                                "flags": [
-                                    "is_initialized_in_class",
-                                    "is_staticmethod",
-                                    "is_ready",
-                                    "is_inferred"
-                                ],
-                                "fullname": "typeguard._importhook.TypeguardLoader.source_to_code",
-                                "name": "source_to_code",
-                                "type": {
-                                    ".class": "CallableType",
-                                    "arg_kinds": [
-                                        0,
-                                        1
-                                    ],
-                                    "arg_names": [
-                                        "data",
-                                        "path"
-                                    ],
-                                    "arg_types": [
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                "builtins.bytes",
-                                                "builtins.bytearray",
-                                                "builtins.memoryview",
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        {
-                                                            ".class": "AnyType",
-                                                            "missing_import_name": null,
-                                                            "source_any": null,
-                                                            "type_of_any": 2
-                                                        }
-                                                    ],
-                                                    "type_ref": "array.array"
-                                                },
-                                                "mmap.mmap",
-                                                "ctypes._CData",
-                                                "pickle.PickleBuffer",
-                                                "builtins.str",
-                                                "_ast.Module",
-                                                "_ast.Expression",
-                                                "_ast.Interactive"
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                "builtins.bytes",
-                                                "builtins.bytearray",
-                                                "builtins.memoryview",
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        {
-                                                            ".class": "AnyType",
-                                                            "missing_import_name": null,
-                                                            "source_any": null,
-                                                            "type_of_any": 2
-                                                        }
-                                                    ],
-                                                    "type_ref": "array.array"
-                                                },
-                                                "mmap.mmap",
-                                                "ctypes._CData",
-                                                "pickle.PickleBuffer",
-                                                "builtins.str",
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        "builtins.str"
-                                                    ],
-                                                    "type_ref": "os.PathLike"
-                                                }
-                                            ]
-                                        }
-                                    ],
-                                    "bound_args": [],
-                                    "def_extras": {
-                                        "first_arg": null
-                                    },
-                                    "fallback": "builtins.function",
-                                    "from_concatenate": false,
-                                    "implicit": false,
-                                    "is_ellipsis_args": false,
-                                    "name": "source_to_code of TypeguardLoader",
-                                    "ret_type": "types.CodeType",
-                                    "type_guard": null,
-                                    "unpack_kwargs": false,
-                                    "variables": []
-                                }
+                                "arg_types": [
+                                    "unittest.result.TestResult"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "stopTestRun of TestResult",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "tb_locals": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.tb_locals",
+                            "name": "tb_locals",
+                            "type": "builtins.bool"
+                        }
+                    },
+                    "testsRun": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.testsRun",
+                            "name": "testsRun",
+                            "type": "builtins.int"
+                        }
+                    },
+                    "unexpectedSuccesses": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready"
+                            ],
+                            "fullname": "unittest.result.TestResult.unexpectedSuccesses",
+                            "name": "unexpectedSuccesses",
+                            "type": {
+                                ".class": "Instance",
+                                "args": [
+                                    "unittest.case.TestCase"
+                                ],
+                                "type_ref": "builtins.list"
+                            }
+                        }
+                    },
+                    "wasSuccessful": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "unittest.result.TestResult.wasSuccessful",
+                            "name": "wasSuccessful",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "unittest.result.TestResult"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "wasSuccessful of TestResult",
+                                "ret_type": "builtins.bool",
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
                             }
                         }
                     }
                 },
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
             }
         },
-        "TypeguardTransformer": {
+        "TextIO": {
             ".class": "SymbolTableNode",
-            "cross_ref": "typeguard._transformer.TypeguardTransformer",
+            "cross_ref": "typing.TextIO",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
-        "_CData": {
+        "TypeVar": {
             ".class": "SymbolTableNode",
-            "cross_ref": "ctypes._CData",
+            "cross_ref": "typing.TypeVar",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "_F": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeVarExpr",
+                "fullname": "unittest.result._F",
+                "name": "_F",
+                "upper_bound": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        2,
+                        4
+                    ],
+                    "arg_names": [
+                        null,
+                        null
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {},
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": true,
+                    "name": null,
+                    "ret_type": {
+                        ".class": "AnyType",
+                        "missing_import_name": null,
+                        "source_any": null,
+                        "type_of_any": 2
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                },
+                "values": [],
+                "variance": 0
+            }
+        },
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "typeguard._importhook.__annotations__",
+                "fullname": "unittest.result.__annotations__",
                 "name": "__annotations__",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
                             ".class": "AnyType",
@@ -1049,463 +1245,253 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "typeguard._importhook.__doc__",
+                "fullname": "unittest.result.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "typeguard._importhook.__file__",
+                "fullname": "unittest.result.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "typeguard._importhook.__name__",
+                "fullname": "unittest.result.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
-                "fullname": "typeguard._importhook.__package__",
+                "fullname": "unittest.result.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "_call_with_frames_removed": {
+        "failfast": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
-                    0,
-                    2,
-                    4
+                    0
                 ],
                 "arg_names": [
-                    "f",
-                    "args",
-                    "kwargs"
+                    "method"
                 ],
                 "dataclass_transform_spec": null,
                 "flags": [],
-                "fullname": "typeguard._importhook._call_with_frames_removed",
-                "name": "_call_with_frames_removed",
+                "fullname": "unittest.result.failfast",
+                "name": "failfast",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
-                        0,
-                        2,
-                        4
+                        0
                     ],
                     "arg_names": [
-                        "f",
-                        "args",
-                        "kwargs"
+                        "method"
                     ],
                     "arg_types": [
                         {
+                            ".class": "TypeVarType",
+                            "fullname": "unittest.result._F",
+                            "id": -1,
+                            "name": "_F",
+                            "namespace": "",
+                            "upper_bound": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    2,
+                                    4
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    },
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {},
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": true,
+                                "name": null,
+                                "ret_type": {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            },
+                            "values": [],
+                            "variance": 0
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "failfast",
+                    "ret_type": {
+                        ".class": "TypeVarType",
+                        "fullname": "unittest.result._F",
+                        "id": -1,
+                        "name": "_F",
+                        "namespace": "",
+                        "upper_bound": {
                             ".class": "CallableType",
                             "arg_kinds": [
                                 2,
                                 4
                             ],
                             "arg_names": [
                                 null,
                                 null
                             ],
                             "arg_types": [
                                 {
-                                    ".class": "ParamSpecType",
-                                    "flavor": 1,
-                                    "fullname": "typeguard._importhook.P",
-                                    "id": -1,
-                                    "name": "P",
-                                    "prefix": {
-                                        ".class": "Parameters",
-                                        "arg_kinds": [],
-                                        "arg_names": [],
-                                        "arg_types": [],
-                                        "variables": []
-                                    },
-                                    "upper_bound": {
-                                        ".class": "Instance",
-                                        "args": [
-                                            "builtins.object"
-                                        ],
-                                        "type_ref": "builtins.tuple"
-                                    }
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
                                 },
                                 {
-                                    ".class": "ParamSpecType",
-                                    "flavor": 2,
-                                    "fullname": "typeguard._importhook.P",
-                                    "id": -1,
-                                    "name": "P",
-                                    "prefix": {
-                                        ".class": "Parameters",
-                                        "arg_kinds": [],
-                                        "arg_names": [],
-                                        "arg_types": [],
-                                        "variables": []
-                                    },
-                                    "upper_bound": {
-                                        ".class": "Instance",
-                                        "args": [
-                                            "builtins.str",
-                                            "builtins.object"
-                                        ],
-                                        "type_ref": "builtins.dict"
-                                    }
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
                                 }
                             ],
                             "bound_args": [],
                             "def_extras": {},
                             "fallback": "builtins.function",
                             "from_concatenate": false,
                             "implicit": false,
-                            "is_ellipsis_args": false,
+                            "is_ellipsis_args": true,
                             "name": null,
                             "ret_type": {
-                                ".class": "TypeVarType",
-                                "fullname": "typeguard._importhook.T",
-                                "id": -2,
-                                "name": "T",
-                                "namespace": "",
-                                "upper_bound": "builtins.object",
-                                "values": [],
-                                "variance": 0
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
                             },
                             "type_guard": null,
                             "unpack_kwargs": false,
                             "variables": []
                         },
-                        {
-                            ".class": "ParamSpecType",
-                            "flavor": 1,
-                            "fullname": "typeguard._importhook.P",
-                            "id": -1,
-                            "name": "P",
-                            "prefix": {
-                                ".class": "Parameters",
-                                "arg_kinds": [],
-                                "arg_names": [],
-                                "arg_types": [],
-                                "variables": []
-                            },
-                            "upper_bound": {
-                                ".class": "Instance",
-                                "args": [
-                                    "builtins.object"
-                                ],
-                                "type_ref": "builtins.tuple"
-                            }
-                        },
-                        {
-                            ".class": "ParamSpecType",
-                            "flavor": 2,
-                            "fullname": "typeguard._importhook.P",
-                            "id": -1,
-                            "name": "P",
-                            "prefix": {
-                                ".class": "Parameters",
-                                "arg_kinds": [],
-                                "arg_names": [],
-                                "arg_types": [],
-                                "variables": []
-                            },
-                            "upper_bound": {
-                                ".class": "Instance",
-                                "args": [
-                                    "builtins.str",
-                                    "builtins.object"
-                                ],
-                                "type_ref": "builtins.dict"
-                            }
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "_call_with_frames_removed",
-                    "ret_type": {
-                        ".class": "TypeVarType",
-                        "fullname": "typeguard._importhook.T",
-                        "id": -2,
-                        "name": "T",
-                        "namespace": "",
-                        "upper_bound": "builtins.object",
                         "values": [],
                         "variance": 0
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
-                            ".class": "ParamSpecType",
-                            "flavor": 0,
-                            "fullname": "typeguard._importhook.P",
+                            ".class": "TypeVarType",
+                            "fullname": "unittest.result._F",
                             "id": -1,
-                            "name": "P",
-                            "prefix": {
-                                ".class": "Parameters",
-                                "arg_kinds": [],
-                                "arg_names": [],
-                                "arg_types": [],
+                            "name": "_F",
+                            "namespace": "",
+                            "upper_bound": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    2,
+                                    4
+                                ],
+                                "arg_names": [
+                                    null,
+                                    null
+                                ],
+                                "arg_types": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    },
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {},
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": true,
+                                "name": null,
+                                "ret_type": {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
                                 "variables": []
                             },
-                            "upper_bound": "builtins.object"
-                        },
-                        {
-                            ".class": "TypeVarType",
-                            "fullname": "typeguard._importhook.T",
-                            "id": -2,
-                            "name": "T",
-                            "namespace": "",
-                            "upper_bound": "builtins.object",
                             "values": [],
                             "variance": 0
                         }
                     ]
                 }
             }
         },
-        "annotations": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "__future__.annotations",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "array": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "array.array",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "ast": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "ast",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "cache_from_source": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "importlib.util.cache_from_source",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "decode_source": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "importlib.util.decode_source",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "global_config": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typeguard._config.global_config",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "install_import_hook": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    1,
-                    5
-                ],
-                "arg_names": [
-                    "packages",
-                    "cls"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "typeguard._importhook.install_import_hook",
-                "name": "install_import_hook",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        1,
-                        5
-                    ],
-                    "arg_names": [
-                        "packages",
-                        "cls"
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "UnionType",
-                            "items": [
-                                {
-                                    ".class": "Instance",
-                                    "args": [
-                                        "builtins.str"
-                                    ],
-                                    "type_ref": "typing.Iterable"
-                                },
-                                {
-                                    ".class": "NoneType"
-                                }
-                            ]
-                        },
-                        {
-                            ".class": "TypeType",
-                            "item": "typeguard._importhook.TypeguardFinder"
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "install_import_hook",
-                    "ret_type": "typeguard._importhook.ImportHookManager",
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "isclass": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "inspect.isclass",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "mmap": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "mmap.mmap",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "optimized_cache_from_source": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    1
-                ],
-                "arg_names": [
-                    "path",
-                    "debug_override"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "typeguard._importhook.optimized_cache_from_source",
-                "name": "optimized_cache_from_source",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        1
-                    ],
-                    "arg_names": [
-                        "path",
-                        "debug_override"
-                    ],
-                    "arg_types": [
-                        "builtins.str",
-                        {
-                            ".class": "UnionType",
-                            "items": [
-                                "builtins.bool",
-                                {
-                                    ".class": "NoneType"
-                                }
-                            ]
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "optimized_cache_from_source",
-                    "ret_type": "builtins.str",
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "patch": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "unittest.mock.patch",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "sys": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "sys",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "types": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "types",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
-        "version": {
+        "unittest": {
             ".class": "SymbolTableNode",
-            "cross_ref": "importlib.metadata.version",
+            "cross_ref": "unittest",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         }
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_importhook.py"
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/result.pyi"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_memo.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_memo.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_suppression.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_transformer.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typeguard/_utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_typing.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/_typing.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/colors.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/colors.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6911111111111111%*

 * *Differences: {"'data_mtime'": '1685631349',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 2), (2, 3), (3, 4), (5, 5), (6, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (2, 10), (4, 20), (5, 5), (6, 5), (7, 5)], delete: '*

 * *                '[1]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (1, 'unittest.result'), (2, 'unittest.suite'), "*

 * *                   "(3, 'collections.abc'), (4, 'unittest'), (5, 'typing'), (6, "*

 * *                   "'typing_extensions')], delete: [2]}",*

 * * "'hash'": "'38357da7850b668627503d574cb […]*

```diff
@@ -1,29 +1,47 @@
 {
-    "data_mtime": 1685630893,
+    "data_mtime": 1685631349,
     "dep_lines": [
         1,
+        2,
+        3,
+        4,
+        1,
+        5,
+        6,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        10,
+        10,
+        5,
+        20,
+        5,
+        5,
         5,
-        30,
         30
     ],
     "dependencies": [
+        "unittest.case",
+        "unittest.result",
+        "unittest.suite",
+        "collections.abc",
+        "unittest",
+        "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
-    "id": "typer.colors",
+    "hash": "38357da7850b668627503d574cb0e5545a449f460bfbb9e8d6325f3820e0aeef",
+    "id": "unittest.runner",
     "ignore_all": true,
-    "interface_hash": "27b284b26e724e12cf37260c1baa2dfb8b4eacd2f12a30cc5a22b69d7b95ad25",
-    "mtime": 1685549646,
+    "interface_hash": "02e6573c902ff2345b6dd19320e6fa89b59116fd89a4eca6a56d093dec7db04e",
+    "mtime": 1685549818,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +75,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/colors.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi",
     "plugin_data": null,
-    "size": 430,
+    "size": 1353,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/completion.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/completion.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/core.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/core.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/main.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/main.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/models.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/models.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.772962962962963%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 7), (1, 8), (5, 5), (6, 1), (7, 1)], delete: [7, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5), (4, 5), (5, 5), (7, 30), (8, 30)], delete: [5, 4, 3, 2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._typing'), (1, 'typer.models'), (3, 'copy'), (5, "*

 * *                   "'typing_extensions'), (8, 'click'), (10, 'click.shell_completion'), (12, "*

 * *                   "'types')], delete: [12, 7, 5, 3, 2, 1, 0]}",*

 * * "'hash'": "'2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8 […]*

```diff
@@ -1,58 +1,58 @@
 {
     "data_mtime": 1685630895,
     "dep_lines": [
-        18,
-        22,
-        24,
-        25,
+        7,
+        8,
         1,
         2,
         3,
-        16,
+        5,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        25,
-        25,
-        25,
-        10,
-        10,
         5,
         10,
         5,
+        5,
+        5,
+        5,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "typer._compat_utils",
-        "click.shell_completion",
-        "typer.core",
-        "typer.main",
+        "typer._typing",
+        "typer.models",
         "inspect",
-        "io",
+        "copy",
         "typing",
-        "click",
+        "typing_extensions",
         "builtins",
         "abc",
+        "click",
         "click.core",
+        "click.shell_completion",
         "click.types",
-        "enum"
+        "types"
     ],
-    "hash": "0d625201001a209a45048efff3154017d132f4d3479b8755ea29f6b81ecdeca9",
-    "id": "typer.models",
+    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
+    "id": "typer.utils",
     "ignore_all": true,
-    "interface_hash": "239046e43ed828fba7030bdc4119029e194d6de90d24865db4033b0bab8d21c6",
+    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
     "mtime": 1685549646,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/models.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
     "plugin_data": null,
-    "size": 15981,
+    "size": 7293,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/params.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/params.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/utils.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/typer/utils.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/plugins.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7174456521739131%*

 * *Differences: {"'data_mtime'": '1686083962',*

 * * "'dep_lines'": '{insert: [(0, 6), (1, 11), (2, 4), (3, 5), (5, 9), (7, 1), (8, 1)], delete: [5, '*

 * *                '4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 30), (8, 30), (9, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib.metadata'), (1, 'su6.core'), (3, 'dataclasses'), (4, "*

 * *                   "'rich'), (5, 'typer'), (7, '_collections_abc'), (11, 'importlib'), (12, "*

 * *                   "'typer.core'), (13, 'typer.main'), (15, 'typing_extensions')], delete: [11, "*

 * *     […]*

```diff
@@ -1,16 +1,19 @@
 {
-    "data_mtime": 1685630895,
+    "data_mtime": 1686083962,
     "dep_lines": [
-        7,
+        6,
+        11,
+        4,
+        5,
         8,
+        9,
+        1,
+        1,
         1,
-        2,
-        3,
-        5,
         1,
         1,
         1,
         1,
         1,
         1,
         1
@@ -24,36 +27,42 @@
         5,
         5,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "typer._typing",
-        "typer.models",
-        "inspect",
-        "copy",
+        "importlib.metadata",
+        "su6.core",
         "typing",
-        "typing_extensions",
+        "dataclasses",
+        "rich",
+        "typer",
         "builtins",
+        "_collections_abc",
         "abc",
         "click",
         "click.core",
-        "click.shell_completion",
-        "click.types",
-        "types"
+        "importlib",
+        "typer.core",
+        "typer.main",
+        "types",
+        "typing_extensions"
     ],
-    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
-    "id": "typer.utils",
+    "hash": "8c2bb0cb8955befd93c31d60c13877cb7d1dcf22de0a435d01a1fe7ad7c330ad",
+    "id": "su6.plugins",
     "ignore_all": true,
-    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
-    "mtime": 1685549646,
+    "interface_hash": "1bf70c5cbce5c6ae93c1ca4240d010d52325177f6c31f5eee86d797de78d5b71",
+    "mtime": 1686083692,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -87,13 +96,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/plugins.py",
     "plugin_data": null,
-    "size": 7293,
+    "size": 10248,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/_log.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/_log.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/async_case.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/async_case.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/case.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/case.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/loader.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/loader.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/main.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/main.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/mock.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/mock.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/result.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/runner.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/runner.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8033333333333333%*

 * *Differences: {"'dep_lines'": '{insert: [(3, 1)], delete: [6, 5]}',*

 * * "'dep_prios'": '{insert: [(6, 30)], delete: [5, 0]}',*

 * * "'dependencies'": "{insert: [(7, 'typing')], delete: [5, 2]}",*

 * * "'hash'": "'82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e'",*

 * * "'id'": "'unittest.suite'",*

 * * "'interface_hash'": "'986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi'",*

 * * "'size'": '9 […]*

```diff
@@ -1,46 +1,43 @@
 {
     "data_mtime": 1685631349,
     "dep_lines": [
         1,
         2,
         3,
+        1,
         4,
         1,
-        5,
-        6,
         1,
         1
     ],
     "dep_prios": [
         10,
         10,
-        10,
         5,
         20,
         5,
         5,
-        5,
+        30,
         30
     ],
     "dependencies": [
         "unittest.case",
         "unittest.result",
-        "unittest.suite",
         "collections.abc",
         "unittest",
-        "typing",
         "typing_extensions",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "38357da7850b668627503d574cb0e5545a449f460bfbb9e8d6325f3820e0aeef",
-    "id": "unittest.runner",
+    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
+    "id": "unittest.suite",
     "ignore_all": true,
-    "interface_hash": "02e6573c902ff2345b6dd19320e6fa89b59116fd89a4eca6a56d093dec7db04e",
+    "interface_hash": "986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4",
     "mtime": 1685549818,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
     "plugin_data": null,
-    "size": 1353,
+    "size": 983,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/signals.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/signals.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6_plugin_demo/cli.meta.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6590476190476191%*

 * *Differences: {"'data_mtime'": '1686084078',*

 * * "'dep_lines'": '{insert: [(0, 6), (1, 4), (2, 9), (5, 1), (6, 1), (7, 1), (8, 1)], delete: [4, 3, '*

 * *                '1]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (4, 30), (5, 30), (6, 30), (7, 30), (8, 30), (9, 30)], delete: '*

 * *                '[2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'su6.plugins'), (2, 'typer'), (5, 'click'), (6, 'click.core'), "*

 * *                   "(7, 'rich'), (8, 'su6.core'), (9, 'typer.core'), (10, 'typer.main')], delete: "*

 * *                   '[4, 2,  […]*

```diff
@@ -1,41 +1,53 @@
 {
-    "data_mtime": 1685631349,
+    "data_mtime": 1686084078,
     "dep_lines": [
+        6,
+        4,
+        9,
+        1,
+        1,
+        1,
+        1,
         1,
-        2,
         1,
-        3,
-        4,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        20,
         5,
+        10,
         5,
         5,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "unittest.result",
-        "collections.abc",
-        "unittest",
+        "su6.plugins",
         "typing",
-        "typing_extensions",
+        "typer",
         "builtins",
-        "abc"
+        "abc",
+        "click",
+        "click.core",
+        "rich",
+        "su6.core",
+        "typer.core",
+        "typer.main"
     ],
-    "hash": "eabaac5475cebd23c74a4785fef60f7f9b1468b82aa854a6162864683a8f852c",
-    "id": "unittest.signals",
-    "ignore_all": true,
-    "interface_hash": "92394d833593a182a1c8b1a7f4bbde75b454b011f0d89a59947f25f24cf7b720",
-    "mtime": 1685549818,
+    "hash": "579595e15c97e044a6d45bd2e80e787b147cd06dc587b332a64a9720023f4cc9",
+    "id": "su6_plugin_demo.cli",
+    "ignore_all": false,
+    "interface_hash": "ce0be9328913eaf26fc4dfe495fce95082995f98f08185e7e93035ce515093b8",
+    "mtime": 1686084201,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -69,13 +81,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi",
+    "path": "src/su6_plugin_demo/cli.py",
     "plugin_data": null,
-    "size": 488,
+    "size": 2286,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/suite.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/unittest/suite.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7375%*

 * *Differences: {"'data_mtime'": '1685630893',*

 * * "'dep_lines'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'hash'": "'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'",*

 * * "'id'": "'urllib'",*

 * * "'interface_hash'": "'697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi'",*

 * * "'size'": '0'}*

```diff
@@ -1,43 +1,28 @@
 {
-    "data_mtime": 1685631349,
+    "data_mtime": 1685630893,
     "dep_lines": [
         1,
-        2,
-        3,
-        1,
-        4,
-        1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
-        5,
-        20,
-        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "unittest.case",
-        "unittest.result",
-        "collections.abc",
-        "unittest",
-        "typing_extensions",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
-    "id": "unittest.suite",
+    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+    "id": "urllib",
     "ignore_all": true,
-    "interface_hash": "986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4",
+    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
     "mtime": 1685549818,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
     "plugin_data": null,
-    "size": 983,
+    "size": 0,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/__init__.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7095238095238094%*

 * *Differences: {"'data_mtime'": '1685987574',*

 * * "'dep_lines'": '{insert: [(0, 11), (1, 12), (2, 20), (3, 9)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'su6.cli'), (1, 'su6.core'), (2, 'su6.plugins'), (3, 'rich')]}",*

 * * "'hash'": "'aeb68fb77133d94e4d21172e8eefc0de7be1267cf1c497c9b1c92b0724c1d6f9'",*

 * * "'id'": "'su6'",*

 * * "'interface_hash'": "'bb90c0c58243f5f20e9a4b5c4e51a8b221ad241fe4b6521836500e63ed7ff07e'",*

 * * "'mtime'": '1686083692',*

 * * "'path'": "'/home/robin/werk/Eigen/su6 […]*

```diff
@@ -1,29 +1,41 @@
 {
-    "data_mtime": 1685630893,
+    "data_mtime": 1685987574,
     "dep_lines": [
+        11,
+        12,
+        20,
+        9,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "su6.cli",
+        "su6.core",
+        "su6.plugins",
+        "rich",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
-    "id": "urllib",
+    "hash": "aeb68fb77133d94e4d21172e8eefc0de7be1267cf1c497c9b1c92b0724c1d6f9",
+    "id": "su6",
     "ignore_all": true,
-    "interface_hash": "697400897136c33c5e3043cedc5133ee860dd03594b47e3057da1e316143caf3",
-    "mtime": 1685549818,
+    "interface_hash": "bb90c0c58243f5f20e9a4b5c4e51a8b221ad241fe4b6521836500e63ed7ff07e",
+    "mtime": 1686083692,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +69,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/__init__.py",
     "plugin_data": null,
-    "size": 0,
+    "size": 627,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/parse.data.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.mypy_cache/3.11/urllib/parse.meta.json` & `su6_plugin_demo-0.2.0/.mypy_cache/3.11/su6/core.meta.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6478857844711503%*

 * *Differences: {"'data_mtime'": '1686083962',*

 * * "'dep_lines'": '{insert: [(0, 16), (2, 5), (3, 6), (5, 8), (6, 9), (7, 10), (8, 11), (9, 12), '*

 * *                '(10, 13), (11, 14), (12, 16), (13, 18), (14, 21), (15, 22), (16, 1), (17, 1), '*

 * *                '(18, 1), (19, 1), (20, 1), (21, 1), (22, 1), (23, 1), (24, 1), (25, 1), (26, 1), '*

 * *                '(27, 1), (28, 1), (29, 1), (30, 1), (34, 17), (35, 17), (36, 20), (37, 17)], '*

 * *                'delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (2, 10), […]*

```diff
@@ -1,44 +1,130 @@
 {
-    "data_mtime": 1685630893,
+    "data_mtime": 1686083962,
     "dep_lines": [
-        2,
-        1,
-        3,
+        16,
         4,
+        5,
+        6,
         7,
+        8,
+        9,
+        10,
+        11,
+        12,
+        13,
+        14,
+        16,
+        18,
+        21,
+        22,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        17,
+        17,
+        20,
+        17
     ],
     "dep_prios": [
-        5,
+        10,
+        10,
+        10,
+        10,
+        10,
+        10,
+        10,
+        10,
+        10,
+        10,
         10,
         5,
+        20,
+        10,
         5,
         5,
         5,
         30,
-        30
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        10,
+        20,
+        5,
+        5
     ],
     "dependencies": [
-        "collections.abc",
+        "black.files",
+        "enum",
+        "functools",
+        "inspect",
+        "json",
+        "operator",
+        "os",
         "sys",
-        "typing",
-        "typing_extensions",
+        "tomllib",
         "types",
+        "typing",
+        "dataclasses",
+        "black",
+        "typer",
+        "rich",
+        "typeguard",
         "builtins",
+        "_collections_abc",
+        "_operator",
         "_typeshed",
-        "abc"
+        "abc",
+        "array",
+        "click",
+        "click.exceptions",
+        "ctypes",
+        "io",
+        "json.encoder",
+        "mmap",
+        "pickle",
+        "typeguard._config",
+        "typeguard._exceptions",
+        "typeguard._functions",
+        "typeguard._memo",
+        "typing_extensions"
     ],
-    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
-    "id": "urllib.parse",
+    "hash": "cc83b7c6bb25f89c7949efca907168e9f8b8da0d4624f661645ff573afd88a70",
+    "id": "su6.core",
     "ignore_all": true,
-    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
-    "mtime": 1685549818,
+    "interface_hash": "8658fd9e77c9b6d7f3f029852716019637b9c843e656918d271227288bfa55be",
+    "mtime": 1686083692,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -72,13 +158,18 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/su6/core.py",
     "plugin_data": null,
-    "size": 6532,
-    "suppressed": [],
+    "size": 21865,
+    "suppressed": [
+        "plumbum.commands.processes",
+        "plumbum.commands",
+        "plumbum.machines",
+        "plumbum"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6_plugin_demo-0.1.0/.ruff_cache/content/4459258ff34f7a6a` & `su6_plugin_demo-0.2.0/.ruff_cache/content/4459258ff34f7a6a`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/.ruff_cache/content/5836aa819cc0bd0b` & `su6_plugin_demo-0.2.0/.ruff_cache/content/5836aa819cc0bd0b`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/htmlcov/coverage_html.js` & `su6_plugin_demo-0.2.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/htmlcov/d_f23488167c00d510___about___py.html` & `su6_plugin_demo-0.2.0/htmlcov/d_f23488167c00d510___init___py.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/su6_plugin_demo/__about__.py: 100%</title>
+    <title>Coverage for src/su6_plugin_demo/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/su6_plugin_demo/__about__.py</b>:
+            <span class="text">Coverage for </span><b>src/su6_plugin_demo/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,52 +50,55 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">1 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">1<span class="text"> run</span></button>
+            <span class="text">0 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_f23488167c00d510___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f23488167c00d510___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_f23488167c00d510_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 12:34 +0200
+            created at 2023-06-06 22:34 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.0.1"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This module serves as an example plugin for `su6`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_f23488167c00d510___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f23488167c00d510___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_f23488167c00d510_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 12:34 +0200
+            created at 2023-06-06 22:34 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
 
-****** Coverage for src/su6_plugin_demo/__about__.py: 100% ******
+****** Coverage for src/su6_plugin_demo/__init__.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 1 statements   1 run 0 missing 0 excluded *****
+***** 0 statements   0 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 12:34 +0200
+at 2023-06-06 22:34 +0200
 
 
-1# SPDX-FileCopyrightText: 2023-present Robin van der Noord
+1""" 
+2This module serves as an example plugin for `su6`. 
+3""" 
+4 
+5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
-2# 
-3# SPDX-License-Identifier: MIT 
-4__version__ = "0.0.1" 
+6# 
+7# SPDX-License-Identifier: MIT 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 12:34 +0200
+at 2023-06-06 22:34 +0200
```

### Comparing `su6_plugin_demo-0.1.0/htmlcov/d_f23488167c00d510___init___py.html` & `su6_plugin_demo-0.2.0/htmlcov/index.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,116 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/su6_plugin_demo/__init__.py: 100%</title>
+    <title>Coverage report</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
-<body class="pyfile">
+<body class="indexfile">
 <header>
     <div class="content">
-        <h1>
-            <span class="text">Coverage for </span><b>src/su6_plugin_demo/__init__.py</b>:
-            <span class="pc_cov">100%</span>
+        <h1>Coverage report:
+            <span class="pc_cov">92%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
-                        <kbd>r</kbd>
+                        <kbd>n</kbd>
+                        <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
-                        &nbsp; toggle line displays
-                    </p>
-                    <p>
-                        <kbd>j</kbd>
-                        <kbd>k</kbd>
-                        &nbsp; next/prev highlighted chunk
-                    </p>
-                    <p>
-                        <kbd>0</kbd> &nbsp; (zero) top of page
-                    </p>
-                    <p>
-                        <kbd>1</kbd> &nbsp; (one) first highlighted chunk
+                        <kbd>c</kbd>
+                        &nbsp; change column sorting
                     </p>
                     <p>
                         <kbd>[</kbd>
                         <kbd>]</kbd>
                         &nbsp; prev/next file
                     </p>
                     <p>
-                        <kbd>u</kbd> &nbsp; up to the index
-                    </p>
-                    <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
-        <h2>
-            <span class="text">0 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
-        </h2>
+        <form id="filter_container">
+            <input id="filter" type="text" value="" placeholder="filter..." />
+        </form>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_f23488167c00d510___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f23488167c00d510_cli_py.html">&#xbb; next</a>
-            &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 12:33 +0200
+            created at 2023-06-06 22:34 +0200
         </p>
-        <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"/>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
-            <button type="button" class="button_top_of_page" data-shortcut="0"/>
-            <button type="button" class="button_first_chunk" data-shortcut="1"/>
-            <button type="button" class="button_prev_file" data-shortcut="["/>
-            <button type="button" class="button_next_file" data-shortcut="]"/>
-            <button type="button" class="button_to_index" data-shortcut="u"/>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
-        </aside>
     </div>
 </header>
-<main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
+<main id="index">
+    <table class="index" data-sortable>
+        <thead>
+            <tr class="tablehead" title="Click to sort">
+                <th class="name left" aria-sort="none" data-shortcut="n">Module</th>
+                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements</th>
+                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing</th>
+                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded</th>
+                <th class="right" aria-sort="none" data-shortcut="c">coverage</th>
+            </tr>
+        </thead>
+        <tbody>
+            <tr class="file">
+                <td class="name left"><a href="d_f23488167c00d510___about___py.html">src/su6_plugin_demo/__about__.py</a></td>
+                <td>1</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="1 1">100%</td>
+            </tr>
+            <tr class="file">
+                <td class="name left"><a href="d_f23488167c00d510___init___py.html">src/su6_plugin_demo/__init__.py</a></td>
+                <td>0</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="0 0">100%</td>
+            </tr>
+            <tr class="file">
+                <td class="name left"><a href="d_f23488167c00d510_cli_py.html">src/su6_plugin_demo/cli.py</a></td>
+                <td>35</td>
+                <td>3</td>
+                <td>0</td>
+                <td class="right" data-ratio="32 35">91%</td>
+            </tr>
+        </tbody>
+        <tfoot>
+            <tr class="total">
+                <td class="name left">Total</td>
+                <td>36</td>
+                <td>3</td>
+                <td>0</td>
+                <td class="right" data-ratio="33 36">92%</td>
+            </tr>
+        </tfoot>
+    </table>
+    <p id="no_rows">
+        No items found using the specified filter.
+    </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_f23488167c00d510___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f23488167c00d510_cli_py.html">&#xbb; next</a>
-            &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 12:33 +0200
+            created at 2023-06-06 22:34 +0200
         </p>
     </div>
+    <aside class="hidden">
+        <a id="prevFileLink" class="nav" href="d_f23488167c00d510_cli_py.html"/>
+        <a id="nextFileLink" class="nav" href="d_f23488167c00d510___about___py.html"/>
+        <button type="button" class="button_prev_file" data-shortcut="["/>
+        <button type="button" class="button_next_file" data-shortcut="]"/>
+        <button type="button" class="button_show_hide_help" data-shortcut="?"/>
+    </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,23 +1,19 @@
 
-****** Coverage for src/su6_plugin_demo/__init__.py: 100% ******
+****** Coverage report: 92% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
-r m x   toggle line displays
-j k   next/prev highlighted chunk
-0   (zero) top of page
-1   (one) first highlighted chunk
+n s m x c   change column sorting
 [ ]   prev/next file
-u   up to the index
 ?   show/hide this help
-***** 0 statements   0 run 0 missing 0 excluded *****
-&#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 12:33 +0200
+[                    ]
+coverage.py_v7.2.7, created at 2023-06-06 22:34 +0200
 
+Module                           statements missing excluded coverage
+src/su6_plugin_demo/__about__.py 1          0       0        100%
+src/su6_plugin_demo/__init__.py  0          0       0        100%
+src/su6_plugin_demo/cli.py       35         3       0        91%
+Total                            36         3       0        92%
+No items found using the specified filter.
 
-1# SPDX-FileCopyrightText: 2023-present Robin van der Noord
-<robinvandernoord@gmail.com> 
-2# 
-3# SPDX-License-Identifier: MIT 
-
-&#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 12:33 +0200
+coverage.py_v7.2.7, created at 2023-06-06 22:34 +0200
+ ____
```

### Comparing `su6_plugin_demo-0.1.0/htmlcov/favicon_32.png` & `su6_plugin_demo-0.2.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/htmlcov/keybd_closed.png` & `su6_plugin_demo-0.2.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/htmlcov/keybd_open.png` & `su6_plugin_demo-0.2.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/htmlcov/status.json` & `su6_plugin_demo-0.2.0/htmlcov/status.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9840277777777777%*

 * *Differences: {"'files'": "{'d_f23488167c00d510___about___py': {'hash': 'e25ce5882b4e58d599ffa5c3b95f9b89'}, "*

 * *            "'d_f23488167c00d510___init___py': {'hash': '2e1c931f43679c37ada5dc59d3d8255e'}, "*

 * *            "'d_f23488167c00d510_cli_py': {'hash': '9494d5483b4cdaefb3270be605bce2de', 'index': "*

 * *            "{'nums': {insert: [(2, 35), (4, 3)], delete: [3, 2]}}}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_f23488167c00d510___about___py": {
-            "hash": "b088a8eff954ab772b292c40a919c395",
+            "hash": "e25ce5882b4e58d599ffa5c3b95f9b89",
             "index": {
                 "html_filename": "d_f23488167c00d510___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -14,15 +14,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_demo/__about__.py"
             }
         },
         "d_f23488167c00d510___init___py": {
-            "hash": "7eaa1e74771c14fddf97c3ea739cadfb",
+            "hash": "2e1c931f43679c37ada5dc59d3d8255e",
             "index": {
                 "html_filename": "d_f23488167c00d510___init___py.html",
                 "nums": [
                     0,
                     1,
                     0,
                     0,
@@ -31,23 +31,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_demo/__init__.py"
             }
         },
         "d_f23488167c00d510_cli_py": {
-            "hash": "fdd3e8389bfe61ac27526781f1edf68c",
+            "hash": "9494d5483b4cdaefb3270be605bce2de",
             "index": {
                 "html_filename": "d_f23488167c00d510_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    18,
-                    0,
+                    35,
                     0,
+                    3,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_demo/cli.py"
             }
         }
```

### Comparing `su6_plugin_demo-0.1.0/htmlcov/style.css` & `su6_plugin_demo-0.2.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/LICENSE.txt` & `su6_plugin_demo-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/README.md` & `su6_plugin_demo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `su6_plugin_demo-0.1.0/pyproject.toml` & `su6_plugin_demo-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,21 @@
 directory = "src"
 include = []
 exclude = []
 stop-after-first-failure = false
 coverage = 100
 badge = true
 
+[tool.su6.demo]
+boolean-arg = true
+optional-with-default = "overridden"
+
+[tool.su6.demo.extra]
+more = true
+
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
@@ -118,15 +125,16 @@
 ]
 extend-exclude = ["*.bak/", "venv*/"]
 
 [tool.bandit]
 # bandit -c pyproject.toml -r .
 exclude_dirs = [".bak", "venv"]
 skips = [
-    "B108"  # hard coded /tmp/... files are fine for me tbh
+    "B108",  # hard coded /tmp/... files are fine for me tbh
+    "B101",  # allow assert for the demo methods
 ]
 
 [tool.isort]
 profile = "black"
 extend_skip_glob = ["*.bak/*"]
 
 [tool.pydocstyle]
```

### Comparing `su6_plugin_demo-0.1.0/PKG-INFO` & `su6_plugin_demo-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6-plugin-demo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Demo plugin for su6-checker
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-plugin-demo#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-plugin-demo/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-plugin-demo
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

