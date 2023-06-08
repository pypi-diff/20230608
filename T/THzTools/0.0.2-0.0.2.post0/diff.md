# Comparing `tmp/thztools-0.0.2.tar.gz` & `tmp/thztools-0.0.2.post0.tar.gz`

## Comparing `thztools-0.0.2.tar` & `thztools-0.0.2.post0.tar`

### file list

```diff
@@ -1,716 +1,21 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 thztools-0.0.2/.DS_Store
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 thztools-0.0.2/.gitattributes
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/other.xml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180412 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52444 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18271 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19674 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23905 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    23380 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60720 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137664 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130456 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123361 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109248 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    29692 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142252 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    90167 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   132111 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22432 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85381 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    52555 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87532 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44437 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75241 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167589 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14417 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49785 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    27792 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   162208 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    19597 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64759 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    42853 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239676 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432278 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57889 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    23833 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/zipfile.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/zipfile.meta.json
--rw-r--r--   0        0        0    89098 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   408032 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129027 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12244 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25117 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79314 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30901 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70623 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64615 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91163 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    15423 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   144429 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0  2217665 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/__init__.data.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_version.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_version.meta.json
--rw-r--r--   0        0        0   112541 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/version.meta.json
--rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25436 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   256912 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41750 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30730 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34767 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16797 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261391 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13683 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11255 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28038 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36087 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330727 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49588 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301784 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196469 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    44548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52653 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/records.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52786 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107815 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27705 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136790 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23356 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14308 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27027 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   252832 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15496 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    67750 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323551 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114237 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   322665 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/__init__.data.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/__init__.meta.json
--rw-r--r--   0        0        0   100879 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_typing.data.json
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_typing.meta.json
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/testing.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/testing.meta.json
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/__init__.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/__init__.meta.json
--rw-r--r--   0        0        0    56793 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/config.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/config.meta.json
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/__init__.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/__init__.meta.json
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/indexing.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/indexing.meta.json
--rw-r--r--   0        0        0   175959 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/interval.data.json
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/interval.meta.json
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/lib.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/lib.meta.json
--rw-r--r--   0        0        0    31747 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/missing.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/missing.meta.json
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/ops_dispatch.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/ops_dispatch.meta.json
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/properties.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/properties.meta.json
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.meta.json
--rw-r--r--   0        0        0    58580 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.meta.json
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.meta.json
--rw-r--r--   0        0        0   125210 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.data.json
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.meta.json
--rw-r--r--   0        0        0    92339 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/period.data.json
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/period.meta.json
--rw-r--r--   0        0        0   190061 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.data.json
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.meta.json
--rw-r--r--   0        0        0   148766 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.data.json
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.meta.json
--rw-r--r--   0        0        0    30709 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_testing/__init__.data.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_testing/__init__.meta.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/__init__.meta.json
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/extensions/__init__.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/extensions/__init__.meta.json
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/indexers/__init__.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/indexers/__init__.meta.json
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/types/__init__.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/types/__init__.meta.json
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/arrays/__init__.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/arrays/__init__.meta.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/__init__.meta.json
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/accessor.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/accessor.meta.json
--rw-r--r--   0        0        0    30009 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/algorithms.data.json
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/algorithms.meta.json
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/api.data.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/api.meta.json
--rw-r--r--   0        0        0    37419 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arraylike.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arraylike.meta.json
--rw-r--r--   0        0        0    36633 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/base.data.json
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/base.meta.json
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/construction.data.json
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/construction.meta.json
--rw-r--r--   0        0        0   636494 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/frame.data.json
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/frame.meta.json
--rw-r--r--   0        0        0   125208 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/generic.data.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/generic.meta.json
--rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexers.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexers.meta.json
--rw-r--r--   0        0        0    26405 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexing.data.json
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexing.meta.json
--rw-r--r--   0        0        0    90504 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/resample.data.json
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/resample.meta.json
--rw-r--r--   0        0        0  1275823 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/series.data.json
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/series.meta.json
--rw-r--r--   0        0        0   130213 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/strings.data.json
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/strings.meta.json
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/__init__.data.json
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/__init__.meta.json
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow.meta.json
--rw-r--r--   0        0        0    33018 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/base.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/base.meta.json
--rw-r--r--   0        0        0    12401 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/boolean.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/boolean.meta.json
--rw-r--r--   0        0        0   102698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/categorical.data.json
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/categorical.meta.json
--rw-r--r--   0        0        0    39620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimelike.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimelike.meta.json
--rw-r--r--   0        0        0    27640 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimes.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimes.meta.json
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/floating.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/floating.meta.json
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/integer.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/integer.meta.json
--rw-r--r--   0        0        0    39175 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/interval.data.json
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/interval.meta.json
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/masked.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/masked.meta.json
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numeric.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numeric.meta.json
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numpy_.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numpy_.meta.json
--rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/period.data.json
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/period.meta.json
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/string_.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/string_.meta.json
--rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/timedeltas.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/timedeltas.meta.json
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.meta.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.meta.json
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.meta.json
--rw-r--r--   0        0        0    32253 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/array.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/array.meta.json
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.meta.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/__init__.meta.json
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/api.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/api.meta.json
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/eval.data.json
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/eval.meta.json
--rw-r--r--   0        0        0    23609 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/expr.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/expr.meta.json
--rw-r--r--   0        0        0    44801 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/ops.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/ops.meta.json
--rw-r--r--   0        0        0    43699 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/pytables.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/pytables.meta.json
--rw-r--r--   0        0        0    11682 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/scope.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/scope.meta.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/__init__.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/__init__.meta.json
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/api.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/api.meta.json
--rw-r--r--   0        0        0    14799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/base.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/base.meta.json
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/common.data.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/common.meta.json
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/concat.data.json
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/concat.meta.json
--rw-r--r--   0        0        0    24363 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/dtypes.data.json
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/dtypes.meta.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/generic.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/generic.meta.json
--rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/inference.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/inference.meta.json
--rw-r--r--   0        0        0    22579 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/missing.data.json
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/missing.meta.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/__init__.meta.json
--rw-r--r--   0        0        0   245511 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/generic.data.json
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/generic.meta.json
--rw-r--r--   0        0        0    59252 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/groupby.data.json
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/groupby.meta.json
--rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/grouper.data.json
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/grouper.meta.json
--rw-r--r--   0        0        0    41348 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/ops.data.json
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/ops.meta.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/__init__.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/__init__.meta.json
--rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/accessors.data.json
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/accessors.meta.json
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/api.data.json
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/api.meta.json
--rw-r--r--   0        0        0   145219 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/base.data.json
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/base.meta.json
--rw-r--r--   0        0        0    20215 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/category.data.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/category.meta.json
--rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimelike.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimelike.meta.json
--rw-r--r--   0        0        0    39507 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimes.data.json
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimes.meta.json
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/extension.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/extension.meta.json
--rw-r--r--   0        0        0   201220 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/interval.data.json
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/interval.meta.json
--rw-r--r--   0        0        0    64788 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/multi.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/multi.meta.json
--rw-r--r--   0        0        0    32074 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/period.data.json
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/period.meta.json
--rw-r--r--   0        0        0    34018 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/range.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/range.meta.json
--rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/timedeltas.data.json
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/timedeltas.meta.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/__init__.meta.json
--rw-r--r--   0        0        0    56107 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.meta.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/__init__.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/__init__.meta.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/api.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/api.meta.json
--rw-r--r--   0        0        0    22894 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/concat.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/concat.meta.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/encoding.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/encoding.meta.json
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/melt.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/melt.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/merge.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/merge.meta.json
--rw-r--r--   0        0        0    40852 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/pivot.data.json
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/pivot.meta.json
--rw-r--r--   0        0        0    79047 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/tile.data.json
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/tile.meta.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/__init__.meta.json
--rw-r--r--   0        0        0    19830 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/datetimes.data.json
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/datetimes.meta.json
--rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/numeric.data.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/numeric.meta.json
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/timedeltas.data.json
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/timedeltas.meta.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/__init__.meta.json
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/hashing.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/hashing.meta.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/__init__.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/__init__.meta.json
--rw-r--r--   0        0        0    22745 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/ewm.data.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/ewm.meta.json
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/expanding.data.json
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/expanding.meta.json
--rw-r--r--   0        0        0    66490 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/rolling.data.json
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/rolling.meta.json
--rw-r--r--   0        0        0    29402 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/errors/__init__.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/errors/__init__.meta.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/__init__.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/__init__.meta.json
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/api.data.json
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/api.meta.json
--rw-r--r--   0        0        0    51839 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/clipboards.data.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/clipboards.meta.json
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/common.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/common.meta.json
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/feather_format.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/feather_format.meta.json
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/gbq.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/gbq.meta.json
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/html.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/html.meta.json
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/orc.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/orc.meta.json
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parquet.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parquet.meta.json
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pickle.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pickle.meta.json
--rw-r--r--   0        0        0    57844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pytables.data.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pytables.meta.json
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/spss.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/spss.meta.json
--rw-r--r--   0        0        0    43579 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sql.data.json
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sql.meta.json
--rw-r--r--   0        0        0    32903 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/stata.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/stata.meta.json
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/xml.data.json
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/xml.meta.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/__init__.meta.json
--rw-r--r--   0        0        0    79643 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/_base.data.json
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/_base.meta.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/__init__.meta.json
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/format.meta.json
--rw-r--r--   0        0        0    80751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style.meta.json
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style_render.data.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style_render.meta.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/__init__.meta.json
--rw-r--r--   0        0        0    39700 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_json.data.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_json.meta.json
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_normalize.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_normalize.meta.json
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_table_schema.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_table_schema.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/__init__.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/__init__.meta.json
--rw-r--r--   0        0        0   135774 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/readers.data.json
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/readers.meta.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/__init__.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas7bdat.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas7bdat.meta.json
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas_xport.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas_xport.meta.json
--rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sasreader.data.json
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sasreader.meta.json
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/__init__.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/__init__.meta.json
--rw-r--r--   0        0        0   150951 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_core.data.json
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_core.meta.json
--rw-r--r--   0        0        0    18244 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_misc.data.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_misc.meta.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/__init__.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/__init__.meta.json
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/api.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/api.meta.json
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/frequencies.data.json
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/frequencies.meta.json
--rw-r--r--   0        0        0    36704 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/holiday.data.json
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/holiday.meta.json
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/offsets.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/offsets.meta.json
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/__init__.meta.json
--rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_decorators.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_decorators.meta.json
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_print_versions.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_print_versions.meta.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_tester.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_tester.meta.json
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/__init__.meta.json
--rw-r--r--   0        0        0   165256 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/dbapi2.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/dbapi2.meta.json
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/__init__.data.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/__init__.meta.json
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/consistency_test.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/consistency_test.meta.json
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/test_thzools.data.json
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/test_thzools.meta.json
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__about__.data.json
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__about__.meta.json
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__init__.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__init__.meta.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/_util.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/_util.meta.json
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/thztools.data.json
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/thztools.meta.json
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24112 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   210198 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    59137 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/14f6e2943b324e9
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/19eb4dc3198b7596
--rw-r--r--   0        0        0    24586 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/1a47944f2ee50e57
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/21d7d90f768e061d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/2489146c9c65f567
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/25a23a381adbd7dc
--rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/27ac16db57cce60b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/2ac966be8abee2ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/36a1a17650d2dfa1
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/3d63d95d98e94a84
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/3f80f26e48fff3b9
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/416d77137606cbda
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/4448948485c70ed1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/46e2ada7eb15b40c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/548cc228a53b18a5
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/56b969a195ceb5bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/570264bdcf8403c5
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/587f16d197c00560
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/5e59e90f4a6610ae
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/5ff7b770a0424a48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/6d641745ea6797b
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/6f15fce0c98cc954
--rw-r--r--   0        0        0    37978 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/6f1765f8409e0c71
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/70343190c55d1467
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/72ab51576de41248
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/7699f8385d3e8ad9
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/780a098b6a97fc9e
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/7deb5a6d9d02374
--rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/7e14ee9fb2ba88af
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/80828fea9567907b
--rw-r--r--   0        0        0    30580 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/89753c64299c4c16
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8a285058467be843
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8c06aade77eca546
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8d40ef997999e5c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8e8b5a7a2416699
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8f3375e559447e11
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/90c0976f06937b1a
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/946677cfaae5d078
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/95ff3cbdf9c9c4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/96f9a668fe5ce99
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/9faaf717898e7034
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/a24306571d8d9be7
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/a8022447c114b8da
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ab14541dc83065aa
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/abf48d11c0afd9ef
--rw-r--r--   0        0        0    30352 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ac982820098a0c6b
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ad867f0bb8f9c9dc
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ad90ede8303e1447
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/aef044181d2d5de7
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/b0448d2cb1c22a2e
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/b70dc04ea668b378
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bac347fb4506c042
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bacc2bb0dfbb7db1
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bf063c6ce36565c
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bf6f8221e6c1c812
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c068bcc1830cc02
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c2fae3237f5f1a4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c56e095cdea1456a
--rw-r--r--   0        0        0    30524 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c753ff9e605d5bb8
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ceb8a922afdc37f4
--rw-r--r--   0        0        0    67766 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/d2551b373b0a40ff
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/da5cccbe0375db71
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/db6089938babdddb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/e14a2a99e27ee9d0
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/e3874541bd014547
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/e46c2b97b92a413c
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/eb52cda4d1bf1d50
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ec89cb2438d79a93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/f556c70333c5b8f9
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/fa6062adf3c39eac
--rw-r--r--   0        0        0    30523 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/fb453ce093001723
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 thztools-0.0.2/envs/environment-dev.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/__about__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/_util.py
--rw-r--r--   0        0        0    28925 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/thztools.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 thztools-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.2/LICENSE
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 thztools-0.0.2/README.md
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 thztools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 thztools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.gitattributes
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/simulation-example.ipynb
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/other.xml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/envs/environment-dev.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/envs/environment-test.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/__about__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/_util.py
+-rw-r--r--   0        0        0    28725 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/LICENSE
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/README.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/pyproject.toml
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/PKG-INFO
```

### Comparing `thztools-0.0.2/.idea/thztools.iml` & `thztools-0.0.2.post0/.idea/thztools.iml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.0.2.post0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2/.ruff_cache/content/89753c64299c4c16` & `thztools-0.0.2.post0/src/thztools/thztools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,1912 +1,1796 @@
-00000000: 0100 0000 0000 0000 1100 0000 0000 0000  ................
-00000010: 7468 7a74 6f6f 6c73 2e74 687a 746f 6f6c  thztools.thztool
-00000020: 7308 0000 0000 0000 0008 0000 0000 0000  s...............
-00000030: 0077 6172 6e69 6e67 7300 0000 000f 0000  .warnings.......
-00000040: 0005 0000 0000 0000 006e 756d 7079 1300  .........numpy..
-00000050: 0000 2500 0000 0600 0000 0000 0000 7061  ..%...........pa
-00000060: 6e64 6173 2700 0000 3a00 0000 0c00 0000  ndas'...:.......
-00000070: 0000 0000 7363 6970 792e 6c69 6e61 6c67  ....scipy.linalg
-00000080: 3c00 0000 4f00 0000 0f00 0000 0000 0000  <...O...........
-00000090: 6e75 6d70 792e 6666 742e 6972 6666 7467  numpy.fft.irfftg
-000000a0: 0000 006c 0000 000e 0000 0000 0000 006e  ...l...........n
-000000b0: 756d 7079 2e66 6674 2e72 6666 746e 0000  umpy.fft.rfftn..
-000000c0: 0072 0000 0012 0000 0000 0000 006e 756d  .r...........num
-000000d0: 7079 2e66 6674 2e72 6666 7466 7265 7174  py.fft.rfftfreqt
-000000e0: 0000 007c 0000 0017 0000 0000 0000 0073  ...|...........s
-000000f0: 6369 7079 2e6f 7074 696d 697a 652e 6d69  cipy.optimize.mi
-00000100: 6e69 6d69 7a65 9900 0000 a100 0000 0500  nimize..........
-00000110: 0000 0000 0000 1400 0000 0000 0000 4e6f  ..............No
-00000120: 4578 706c 6963 6974 5374 6163 6b6c 6576  ExplicitStacklev
-00000130: 656c 2f00 0000 0000 0000 4e6f 2065 7870  el/.......No exp
-00000140: 6c69 6369 7420 6073 7461 636b 6c65 7665  licit `stackleve
-00000150: 6c60 206b 6579 776f 7264 2061 7267 756d  l` keyword argum
-00000160: 656e 7420 666f 756e 6400 6b37 0000 7837  ent found.k7..x7
-00000170: 0000 0000 0000 0000 0000 006b 3700 0016  ...........k7...
-00000180: 0000 0000 0000 004d 7574 6162 6c65 4172  .......MutableAr
-00000190: 6775 6d65 6e74 4465 6661 756c 7438 0000  gumentDefault8..
-000001a0: 0000 0000 0044 6f20 6e6f 7420 7573 6520  .....Do not use 
-000001b0: 6d75 7461 626c 6520 6461 7461 2073 7472  mutable data str
-000001c0: 7563 7475 7265 7320 666f 7220 6172 6775  uctures for argu
-000001d0: 6d65 6e74 2064 6566 6175 6c74 7300 3d4d  ment defaults.=M
-000001e0: 0000 554d 0000 0000 0000 0000 0000 003d  ..UM...........=
-000001f0: 4d00 0016 0000 0000 0000 004d 7574 6162  M..........Mutab
-00000200: 6c65 4172 6775 6d65 6e74 4465 6661 756c  leArgumentDefaul
-00000210: 7438 0000 0000 0000 0044 6f20 6e6f 7420  t8.......Do not 
-00000220: 7573 6520 6d75 7461 626c 6520 6461 7461  use mutable data
-00000230: 2073 7472 7563 7475 7265 7320 666f 7220   structures for 
-00000240: 6172 6775 6d65 6e74 2064 6566 6175 6c74  argument default
-00000250: 7300 f04c 0000 244d 0000 0000 0000 0000  s..L..$M........
-00000260: 0000 00f0 4c00 0005 0000 0000 0000 0050  ....L..........P
-00000270: 7269 6e74 0d00 0000 0000 0000 6070 7269  rint........`pri
-00000280: 6e74 6020 666f 756e 6400 1668 0000 1b68  nt` found..h...h
-00000290: 0000 0000 0000 0000 0000 0016 6800 000b  ............h...
-000002a0: 0000 0000 0000 004c 696e 6554 6f6f 4c6f  .......LineTooLo
-000002b0: 6e67 2200 0000 0000 0000 4c69 6e65 2074  ng".......Line t
-000002c0: 6f6f 206c 6f6e 6720 2838 3720 3e20 3739  oo long (87 > 79
-000002d0: 2063 6861 7261 6374 6572 7329 002b 4900   characters).+I.
-000002e0: 0033 4900 0000 0000 0000 0000 0000 2b49  .3I...........+I
-000002f0: 0000 0100 0000 0000 0000 6b00 0000 0000  ..........k.....
-00000300: 0000 2f55 7365 7273 2f6a 7364 2f4c 6962  ../Users/jsd/Lib
-00000310: 7261 7279 2f43 6c6f 7564 5374 6f72 6167  rary/CloudStorag
-00000320: 652f 4f6e 6544 7269 7665 2d53 696d 6f6e  e/OneDrive-Simon
-00000330: 4672 6173 6572 556e 6976 6572 7369 7479  FraserUniversity
-00000340: 2831 7366 7529 2f70 726f 6a65 6374 732f  (1sfu)/projects/
-00000350: 7468 7a74 6f6f 6c73 2f74 687a 746f 6f6c  thztools/thztool
-00000360: 732f 7468 7a74 6f6f 6c73 2e70 79ff 7300  s/thztools.py.s.
-00000370: 0000 0000 0069 6d70 6f72 7420 7761 726e  .....import warn
-00000380: 696e 6773 0d0a 0d0a 696d 706f 7274 206e  ings....import n
-00000390: 756d 7079 2061 7320 6e70 0d0a 696d 706f  umpy as np..impo
-000003a0: 7274 2070 616e 6461 7320 6173 2070 640d  rt pandas as pd.
-000003b0: 0a69 6d70 6f72 7420 7363 6970 792e 6c69  .import scipy.li
-000003c0: 6e61 6c67 0d0a 6672 6f6d 206e 756d 7079  nalg..from numpy
-000003d0: 2e66 6674 2069 6d70 6f72 7420 6972 6666  .fft import irff
-000003e0: 742c 2072 6666 742c 2072 6666 7466 7265  t, rfft, rfftfre
-000003f0: 710d 0a66 726f 6d20 7363 6970 792e 6f70  q..from scipy.op
-00000400: 7469 6d69 7a65 2069 6d70 6f72 7420 6d69  timize import mi
-00000410: 6e69 6d69 7a65 0d0a 0d0a 0d0a 6465 6620  nimize......def 
-00000420: 6666 7466 7265 7128 6e2c 2074 293a 0d0a  fftfreq(n, t):..
-00000430: 2020 2020 2222 2243 6f6d 7075 7465 7320      """Computes 
-00000440: 7468 6520 706f 7369 7469 7665 2061 6e64  the positive and
-00000450: 206e 6567 6174 6976 6520 6672 6571 7565   negative freque
-00000460: 6e63 6965 7320 7361 6d70 6c65 6420 696e  ncies sampled in
-00000470: 2074 6865 2046 6173 740d 0a20 2020 2046   the Fast..    F
-00000480: 6f75 7269 6572 2054 7261 6e73 666f 726d  ourier Transform
-00000490: 2e0d 0a0d 0a20 2020 2050 6172 616d 6574  .....    Paramet
-000004a0: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
-000004b0: 2d2d 2d0d 0a20 2020 206e 203a 2069 6e74  ---..    n : int
-000004c0: 0d0a 2020 2020 2020 2020 4e75 6d62 6572  ..        Number
-000004d0: 206f 6620 7469 6d65 2073 616d 706c 6573   of time samples
-000004e0: 0d0a 2020 2020 743a 2066 6c6f 6174 0d0a  ..    t: float..
-000004f0: 2020 2020 2020 2020 5361 6d70 6c69 6e67          Sampling
-00000500: 2074 696d 650d 0a0d 0a20 2020 2052 6574   time....    Ret
-00000510: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
-00000520: 2d0d 0a20 2020 2066 203a 206e 6461 7272  -..    f : ndarr
-00000530: 6179 0d0a 2020 2020 2020 2020 4672 6571  ay..        Freq
-00000540: 7565 6e63 7920 7665 6374 6f72 2028 312f  uency vector (1/
-00000550: 7473 2920 6f66 206c 656e 6774 6820 6e20  ts) of length n 
-00000560: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
-00000570: 616d 706c 6520 6672 6571 7565 6e63 6965  ample frequencie
-00000580: 732e 0d0a 2020 2020 2222 220d 0a0d 0a20  s...    """.... 
-00000590: 2020 2069 6620 6e20 2520 3220 3d3d 2031     if n % 2 == 1
-000005a0: 3a0d 0a20 2020 2020 2020 2066 203d 206e  :..        f = n
-000005b0: 702e 6666 742e 6666 7466 7265 7128 6e2c  p.fft.fftfreq(n,
-000005c0: 2074 290d 0a20 2020 2065 6c73 653a 0d0a   t)..    else:..
-000005d0: 2020 2020 2020 2020 6620 3d20 6e70 2e66          f = np.f
-000005e0: 6674 2e66 6674 6672 6571 286e 2c20 7429  ft.fftfreq(n, t)
-000005f0: 0d0a 2020 2020 2020 2020 665b 696e 7428  ..        f[int(
-00000600: 6e20 2f20 3229 5d20 3d20 2d66 5b69 6e74  n / 2)] = -f[int
-00000610: 286e 202f 2032 295d 0d0a 0d0a 2020 2020  (n / 2)]....    
-00000620: 7265 7475 726e 2066 0d0a 0d0a 0d0a 6465  return f......de
-00000630: 6620 6e6f 6973 6576 6172 2873 6967 6d61  f noisevar(sigma
-00000640: 2c20 6d75 2c20 7473 293a 0d0a 2020 2020  , mu, ts):..    
-00000650: 7222 2222 0d0a 2020 2020 4e6f 6973 6576  r"""..    Noisev
-00000660: 6172 2063 6f6d 7075 7465 7320 7468 6520  ar computes the 
-00000670: 7469 6d65 2d64 6f6d 6169 6e20 6e6f 6973  time-domain nois
-00000680: 6520 7661 7269 616e 6365 2066 6f72 206e  e variance for n
-00000690: 6f69 7365 2070 6172 616d 6574 6572 730d  oise parameters.
-000006a0: 0a20 2020 2073 6967 6d61 2c20 7769 7468  .    sigma, with
-000006b0: 2061 2073 6967 6e61 6c20 6d75 2061 6e64   a signal mu and
-000006c0: 2073 616d 706c 696e 6720 696e 7465 7276   sampling interv
-000006d0: 616c 2054 2e20 5468 6572 6520 6172 6520  al T. There are 
-000006e0: 7468 7265 6520 6e6f 6973 650d 0a20 2020  three noise..   
-000006f0: 2070 6172 616d 6574 6572 733a 2074 6865   parameters: the
-00000700: 2066 6972 7374 2063 6f72 7265 7370 6f6e   first correspon
-00000710: 6473 2074 6f20 616d 706c 6974 7564 6520  ds to amplitude 
-00000720: 6e6f 6973 652c 2069 6e20 7369 676e 616c  noise, in signal
-00000730: 2075 6e69 7473 2028 0d0a 2020 2020 692e   units (..    i.
-00000740: 652c 2074 6865 2073 616d 6520 756e 6974  e, the same unit
-00000750: 7320 6173 206d 7529 203b 2020 7468 6520  s as mu) ;  the 
-00000760: 7365 636f 6e64 2063 6f72 7265 7370 6f6e  second correspon
-00000770: 6473 2074 6f20 6d75 6c74 6970 6c69 6361  ds to multiplica
-00000780: 7469 7665 0d0a 2020 2020 6e6f 6973 652c  tive..    noise,
-00000790: 2077 6869 6368 2069 7320 6469 6d65 6e73   which is dimens
-000007a0: 696f 6e6c 6573 733b 2061 6e64 2074 6865  ionless; and the
-000007b0: 2074 6869 7264 2063 6f72 7265 7370 6f6e   third correspon
-000007c0: 6473 2074 6f20 7469 6d65 6261 7365 0d0a  ds to timebase..
-000007d0: 2020 2020 6e6f 6973 652c 2069 6e20 756e      noise, in un
-000007e0: 6974 7320 6f66 2073 6967 6e61 6c2f 7469  its of signal/ti
-000007f0: 6d65 2c20 7768 6572 6520 7468 6520 756e  me, where the un
-00000800: 6974 7320 666f 7220 7469 6d65 2061 7265  its for time are
-00000810: 2074 6865 2073 616d 6520 6173 0d0a 2020   the same as..  
-00000820: 2020 666f 7220 542e 2054 6865 206f 7574    for T. The out
-00000830: 7075 742c 2056 6d75 2c20 6973 2067 6976  put, Vmu, is giv
-00000840: 656e 2069 6e20 756e 6974 7320 7468 6174  en in units that
-00000850: 2061 7265 2074 6865 2073 7175 6172 6520   are the square 
-00000860: 6f66 2074 6865 0d0a 2020 2020 7369 676e  of the..    sign
-00000870: 616c 2075 6e69 7473 2e0d 0a0d 0a20 2020  al units.....   
-00000880: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-00000890: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-000008a0: 2073 6967 6d61 203a 206e 6461 7272 6179   sigma : ndarray
-000008b0: 0d0a 2020 2020 2020 2020 2833 2c20 2920  ..        (3, ) 
-000008c0: 6172 7261 7920 2063 6f6e 7461 696e 696e  array  containin
-000008d0: 6720 6e6f 6973 6520 7061 7261 6d65 7465  g noise paramete
-000008e0: 7273 0d0a 2020 2020 6d75 203a 206e 6461  rs..    mu : nda
-000008f0: 7272 6179 0d0a 2020 2020 2020 2020 286e  rray..        (n
-00000900: 2c20 2920 6172 7261 7920 2063 6f6e 7461  , ) array  conta
-00000910: 696e 696e 6720 2073 6967 6e61 6c20 7665  ining  signal ve
-00000920: 6374 6f72 0d0a 2020 2020 7473 203a 2066  ctor..    ts : f
-00000930: 6c6f 6174 0d0a 2020 2020 2020 2020 5361  loat..        Sa
-00000940: 6d70 6c69 6e67 2074 696d 650d 0a0d 0a20  mpling time.... 
-00000950: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00000960: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 766d  --------..    vm
-00000970: 7520 3a20 6e64 6172 7261 790d 0a20 2020  u : ndarray..   
-00000980: 2020 2020 204e 6f69 7365 2076 6172 6961       Noise varia
-00000990: 6e63 650d 0a20 2020 2022 2222 0d0a 0d0a  nce..    """....
-000009a0: 2020 2020 6e20 3d20 6d75 2e73 6861 7065      n = mu.shape
-000009b0: 5b30 5d0d 0a20 2020 2077 203d 2032 202a  [0]..    w = 2 *
-000009c0: 206e 702e 7069 202a 2072 6666 7466 7265   np.pi * rfftfre
-000009d0: 7128 6e2c 2074 7329 0d0a 2020 2020 6d75  q(n, ts)..    mu
-000009e0: 646f 7420 3d20 6972 6666 7428 316a 202a  dot = irfft(1j *
-000009f0: 2077 202a 2072 6666 7428 6d75 292c 206e   w * rfft(mu), n
-00000a00: 3d6e 290d 0a0d 0a20 2020 2072 6574 7572  =n)....    retur
-00000a10: 6e20 7369 676d 615b 305d 202a 2a20 3220  n sigma[0] ** 2 
-00000a20: 2b20 2873 6967 6d61 5b31 5d20 2a20 6d75  + (sigma[1] * mu
-00000a30: 2920 2a2a 2032 202b 2028 7369 676d 615b  ) ** 2 + (sigma[
-00000a40: 325d 202a 206d 7564 6f74 2920 2a2a 2032  2] * mudot) ** 2
-00000a50: 0d0a 0d0a 0d0a 6465 6620 6e6f 6973 6561  ......def noisea
-00000a60: 6d70 2873 6967 6d61 2c20 6d75 2c20 7473  mp(sigma, mu, ts
-00000a70: 293a 0d0a 2020 2020 7222 2222 0d0a 2020  ):..    r"""..  
-00000a80: 2020 6e6f 6973 6561 6d70 2063 6f6d 7075    noiseamp compu
-00000a90: 7465 7320 7468 6520 7469 6d65 2d64 6f6d  tes the time-dom
-00000aa0: 6169 6e20 6e6f 6973 6520 616d 706c 6974  ain noise amplit
-00000ab0: 7564 6573 2066 6f72 206e 6f69 7365 2070  udes for noise p
-00000ac0: 6172 616d 6574 6572 730d 0a20 2020 2073  arameters..    s
-00000ad0: 6967 6d61 2c20 7769 7468 2061 2073 6967  igma, with a sig
-00000ae0: 6e61 6c20 6d75 2061 6e64 2073 616d 706c  nal mu and sampl
-00000af0: 696e 6720 696e 7465 7276 616c 2074 2e20  ing interval t. 
-00000b00: 2054 6865 7265 2061 7265 2074 6872 6565   There are three
-00000b10: 206e 6f69 7365 0d0a 2020 2020 7061 7261   noise..    para
-00000b20: 6d65 7465 7273 3a20 7468 6520 6669 7273  meters: the firs
-00000b30: 7420 636f 7272 6573 706f 6e64 7320 746f  t corresponds to
-00000b40: 2061 6d70 6c69 7475 6465 206e 6f69 7365   amplitude noise
-00000b50: 2c20 696e 2073 6967 6e61 6c20 756e 6974  , in signal unit
-00000b60: 7320 280d 0a20 2020 2069 652c 2074 6865  s (..    ie, the
-00000b70: 2073 616d 6520 756e 6974 7320 6173 206d   same units as m
-00000b80: 7529 3b20 7468 6520 7365 636f 6e64 2063  u); the second c
-00000b90: 6f72 7265 7370 6f6e 6473 2074 6f20 6d75  orresponds to mu
-00000ba0: 6c74 6970 6c69 6361 7469 7665 0d0a 2020  ltiplicative..  
-00000bb0: 2020 6e6f 6973 652c 2077 6869 6368 2069    noise, which i
-00000bc0: 7320 6469 6d65 6e73 696f 6e6c 6573 733b  s dimensionless;
-00000bd0: 2061 6e64 2074 6865 2074 6869 7264 2063   and the third c
-00000be0: 6f72 7265 7370 6f6e 6473 2074 6f20 7469  orresponds to ti
-00000bf0: 6d65 6261 7365 0d0a 2020 2020 6e6f 6973  mebase..    nois
-00000c00: 652c 2069 6e20 756e 6974 7320 6f66 2073  e, in units of s
-00000c10: 6967 6e61 6c2f 7469 6d65 2c20 7768 6572  ignal/time, wher
-00000c20: 6520 7468 6520 756e 6974 7320 666f 7220  e the units for 
-00000c30: 7469 6d65 2061 7265 2074 6865 2073 616d  time are the sam
-00000c40: 6520 6173 0d0a 2020 2020 666f 7220 742e  e as..    for t.
-00000c50: 2054 6865 206f 7574 7075 742c 2073 6967   The output, sig
-00000c60: 6d61 6d75 2c20 6973 2067 6976 656e 2069  mamu, is given i
-00000c70: 6e20 7369 676e 616c 2075 6e69 7473 2e0d  n signal units..
-00000c80: 0a0d 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00000c90: 730d 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  s..    ---------
-00000ca0: 2d0d 0a20 2020 2073 6967 6d61 203a 206e  -..    sigma : n
-00000cb0: 6461 7272 6179 0d0a 2020 2020 2020 2020  darray..        
-00000cc0: 2833 2c20 2920 6172 7261 7920 2063 6f6e  (3, ) array  con
-00000cd0: 7461 696e 696e 6720 6e6f 6973 6520 7061  taining noise pa
-00000ce0: 7261 6d65 7465 7273 0d0a 2020 2020 6d75  rameters..    mu
-00000cf0: 203a 2020 7369 676e 616c 2076 6563 746f   :  signal vecto
-00000d00: 720d 0a20 2020 2020 2020 2028 6e2c 2029  r..        (n, )
-00000d10: 2061 7272 6179 2020 636f 6e74 6169 6e69   array  containi
-00000d20: 6e67 2020 7369 676e 616c 2076 6563 746f  ng  signal vecto
-00000d30: 720d 0a20 2020 2074 7320 3a20 666c 6f61  r..    ts : floa
-00000d40: 740d 0a20 2020 2020 2020 2073 616d 706c  t..        sampl
-00000d50: 696e 6720 7469 6d65 0d0a 0d0a 2020 2020  ing time....    
-00000d60: 5265 7475 726e 730d 0a20 2020 202d 2d2d  Returns..    ---
-00000d70: 2d2d 2d2d 0d0a 2020 2020 7369 676d 616d  ----..    sigmam
-00000d80: 7520 3a20 6e64 6172 7261 790d 0a20 2020  u : ndarray..   
-00000d90: 2020 2020 2028 6e2c 2029 2061 7272 6179       (n, ) array
-00000da0: 2063 6f6e 7461 696e 696e 6720 6e6f 6973   containing nois
-00000db0: 6520 616d 706c 6974 7564 650d 0a20 2020  e amplitude..   
-00000dc0: 2022 2222 0d0a 0d0a 2020 2020 7265 7475   """....    retu
-00000dd0: 726e 206e 702e 7371 7274 286e 6f69 7365  rn np.sqrt(noise
-00000de0: 7661 7228 7369 676d 612c 206d 752c 2074  var(sigma, mu, t
-00000df0: 7329 290d 0a0d 0a0d 0a64 6566 2074 687a  s))......def thz
-00000e00: 6765 6e28 6e2c 2074 732c 2074 302c 2061  gen(n, ts, t0, a
-00000e10: 3d31 2e30 2c20 7461 7572 3d30 2e33 2c20  =1.0, taur=0.3, 
-00000e20: 7461 7563 3d30 2e31 2c20 6677 686d 3d30  tauc=0.1, fwhm=0
-00000e30: 2e30 3529 3a0d 0a20 2020 2072 2222 2247  .05):..    r"""G
-00000e40: 656e 6572 6174 6520 6120 7465 7261 6865  enerate a terahe
-00000e50: 7274 7a20 7075 6c73 652e 0d0a 0d0a 2020  rtz pulse.....  
-00000e60: 2020 5265 7475 726e 7320 616e 2069 6465    Returns an ide
-00000e70: 616c 697a 6564 2077 6176 6566 6f72 6d20  alized waveform 
-00000e80: 7769 7468 206e 2070 6f69 6e74 7320 6174  with n points at
-00000e90: 2073 616d 706c 696e 6720 696e 7465 7276   sampling interv
-00000ea0: 616c 2074 2061 6e64 0d0a 2020 2020 6365  al t and..    ce
-00000eb0: 6e74 6572 6564 2061 7420 7430 2e0d 0a0d  ntered at t0....
-00000ec0: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
-00000ed0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
-00000ee0: 0a0d 0a20 2020 206e 203a 2069 6e74 0d0a  ...    n : int..
-00000ef0: 2020 2020 2020 2020 6e75 6d62 6572 206f          number o
-00000f00: 6620 7361 6d70 6c65 6420 706f 696e 7473  f sampled points
-00000f10: 2e0d 0a0d 0a20 2020 2074 7320 3a20 666c  .....    ts : fl
-00000f20: 6f61 740d 0a20 2020 2020 2020 2073 616d  oat..        sam
-00000f30: 706c 696e 6720 7469 6d65 0d0a 0d0a 2020  pling time....  
-00000f40: 2020 7430 203a 2066 6c6f 6174 0d0a 2020    t0 : float..  
-00000f50: 2020 2020 2020 7075 6c73 6520 6365 6e74        pulse cent
-00000f60: 6572 0d0a 0d0a 2020 2020 6120 3a20 666c  er....    a : fl
-00000f70: 6f61 742c 206f 7074 696f 6e61 6c0d 0a20  oat, optional.. 
-00000f80: 2020 2020 2020 2050 6561 6b20 616d 706c         Peak ampl
-00000f90: 6974 7564 652e 0d0a 0d0a 2020 2020 7461  itude.....    ta
-00000fa0: 7572 203a 2066 6c6f 6174 2c20 6f70 7469  ur : float, opti
-00000fb0: 6f6e 616c 0d0a 2020 2020 2020 2020 4375  onal..        Cu
-00000fc0: 7272 656e 7420 7075 6c73 6520 7269 7365  rrent pulse rise
-00000fd0: 2074 696d 652e 0d0a 0d0a 2020 2020 7461   time.....    ta
-00000fe0: 7563 203a 2066 6c6f 6174 2c20 6f70 7469  uc : float, opti
-00000ff0: 6f6e 616c 0d0a 2020 2020 2020 2020 4375  onal..        Cu
-00001000: 7272 656e 7420 7075 6c73 6520 6465 6361  rrent pulse deca
-00001010: 7920 7469 6d65 2e0d 0a0d 0a20 2020 2066  y time.....    f
-00001020: 7768 6d20 3a20 666c 6f61 742c 206f 7074  whm : float, opt
-00001030: 696f 6e61 6c0d 0a20 2020 2020 2020 204c  ional..        L
-00001040: 6173 6572 2070 756c 7365 2046 5748 4d2e  aser pulse FWHM.
-00001050: 0d0a 0d0a 2020 2020 5265 7475 726e 730d  ....    Returns.
-00001060: 0a20 2020 202d 2d2d 2d2d 2d2d 0d0a 0d0a  .    -------....
-00001070: 2020 2020 7920 3a20 6e64 6172 7261 790d      y : ndarray.
-00001080: 0a20 2020 2020 2020 2073 6967 6e61 6c20  .        signal 
-00001090: 2875 2e61 290d 0a0d 0a20 2020 2074 203a  (u.a)....    t :
-000010a0: 2066 6c6f 6174 0d0a 2020 2020 2020 2020   float..        
-000010b0: 7469 6d65 6261 7365 0d0a 0d0a 2020 2020  timebase....    
-000010c0: 2222 220d 0a0d 0a20 2020 2074 6175 6c20  """....    taul 
-000010d0: 3d20 6677 686d 202f 206e 702e 7371 7274  = fwhm / np.sqrt
-000010e0: 2832 202a 206e 702e 6c6f 6728 3229 290d  (2 * np.log(2)).
-000010f0: 0a0d 0a20 2020 2066 203d 2072 6666 7466  ...    f = rfftf
-00001100: 7265 7128 6e2c 2074 7329 0d0a 0d0a 2020  req(n, ts)....  
-00001110: 2020 7720 3d20 3220 2a20 6e70 2e70 6920    w = 2 * np.pi 
-00001120: 2a20 660d 0a20 2020 2065 6c6c 203d 206e  * f..    ell = n
-00001130: 702e 6578 7028 2d28 7720 2a20 7461 756c  p.exp(-(w * taul
-00001140: 2920 2a2a 2032 202f 2032 2920 2f20 6e70  ) ** 2 / 2) / np
-00001150: 2e73 7172 7428 3220 2a20 6e70 2e70 6920  .sqrt(2 * np.pi 
-00001160: 2a20 7461 756c 202a 2a20 3229 0d0a 2020  * taul ** 2)..  
-00001170: 2020 7220 3d20 3120 2f20 2831 202f 2074    r = 1 / (1 / t
-00001180: 6175 7220 2d20 316a 202a 2077 2920 2d20  aur - 1j * w) - 
-00001190: 3120 2f20 2831 202f 2074 6175 7220 2b20  1 / (1 / taur + 
-000011a0: 3120 2f20 7461 7563 202d 2031 6a20 2a20  1 / tauc - 1j * 
-000011b0: 7729 0d0a 2020 2020 7320 3d20 2d31 6a20  w)..    s = -1j 
-000011c0: 2a20 7720 2a20 2865 6c6c 202a 2072 2920  * w * (ell * r) 
-000011d0: 2a2a 2032 202a 206e 702e 6578 7028 316a  ** 2 * np.exp(1j
-000011e0: 202a 2077 202a 2074 3029 0d0a 0d0a 2020   * w * t0)....  
-000011f0: 2020 7432 203d 2074 7320 2a20 6e70 2e61    t2 = ts * np.a
-00001200: 7261 6e67 6528 6e29 0d0a 0d0a 2020 2020  range(n)....    
-00001210: 7920 3d20 6972 6666 7428 6e70 2e63 6f6e  y = irfft(np.con
-00001220: 6a28 7329 2c20 6e3d 6e29 0d0a 2020 2020  j(s), n=n)..    
-00001230: 7920 3d20 6120 2a20 7920 2f20 6e70 2e6d  y = a * y / np.m
-00001240: 6178 2879 290d 0a0d 0a20 2020 2072 6574  ax(y)....    ret
-00001250: 7572 6e20 5b79 2c20 7432 5d0d 0a0d 0a0d  urn [y, t2].....
-00001260: 0a63 6c61 7373 2044 6174 6150 756c 7365  .class DataPulse
-00001270: 3a0d 0a0d 0a20 2020 2064 6566 205f 5f69  :....    def __i
-00001280: 6e69 745f 5f28 7365 6c66 2c20 6669 6c65  nit__(self, file
-00001290: 6e61 6d65 3d22 2229 3a0d 0a20 2020 2020  name=""):..     
-000012a0: 2020 2073 656c 662e 4163 7175 6973 6974     self.Acquisit
-000012b0: 696f 6e54 696d 6520 3d20 4e6f 6e65 0d0a  ionTime = None..
-000012c0: 2020 2020 2020 2020 7365 6c66 2e44 6573          self.Des
-000012d0: 6372 6970 7469 6f6e 203d 204e 6f6e 650d  cription = None.
-000012e0: 0a20 2020 2020 2020 2073 656c 662e 5469  .        self.Ti
-000012f0: 6d65 436f 6e73 7461 6e74 203d 204e 6f6e  meConstant = Non
-00001300: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001310: 5761 6974 5469 6d65 203d 204e 6f6e 650d  WaitTime = None.
-00001320: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00001330: 7450 6f69 6e74 203d 204e 6f6e 650d 0a20  tPoint = None.. 
-00001340: 2020 2020 2020 2073 656c 662e 7363 616e         self.scan
-00001350: 4f66 6673 6574 203d 204e 6f6e 650d 0a20  Offset = None.. 
-00001360: 2020 2020 2020 2073 656c 662e 7465 6d70         self.temp
-00001370: 6572 6174 7572 6520 3d20 4e6f 6e65 0d0a  erature = None..
-00001380: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-00001390: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
-000013a0: 2020 7365 6c66 2e61 6d70 6c69 7475 6465    self.amplitude
-000013b0: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-000013c0: 2073 656c 662e 4368 616e 6e65 6c41 4d61   self.ChannelAMa
-000013d0: 7869 6d75 6d20 3d20 4e6f 6e65 0d0a 2020  ximum = None..  
-000013e0: 2020 2020 2020 7365 6c66 2e43 6861 6e6e        self.Chann
-000013f0: 656c 414d 696e 696d 756d 203d 204e 6f6e  elAMinimum = Non
-00001400: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001410: 4368 616e 6e65 6c41 5661 7269 616e 6365  ChannelAVariance
-00001420: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00001430: 2073 656c 662e 4368 616e 6e65 6c41 536c   self.ChannelASl
-00001440: 6f70 6520 3d20 4e6f 6e65 0d0a 2020 2020  ope = None..    
-00001450: 2020 2020 7365 6c66 2e43 6861 6e6e 656c      self.Channel
-00001460: 414f 6666 7365 7420 3d20 4e6f 6e65 0d0a  AOffset = None..
-00001470: 2020 2020 2020 2020 7365 6c66 2e43 6861          self.Cha
-00001480: 6e6e 656c 424d 6178 696d 756d 203d 204e  nnelBMaximum = N
-00001490: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-000014a0: 662e 4368 616e 6e65 6c42 4d69 6e69 6d75  f.ChannelBMinimu
-000014b0: 6d20 3d20 4e6f 6e65 0d0a 2020 2020 2020  m = None..      
-000014c0: 2020 7365 6c66 2e43 6861 6e6e 656c 4256    self.ChannelBV
-000014d0: 6172 6961 6e63 6520 3d20 4e6f 6e65 0d0a  ariance = None..
-000014e0: 2020 2020 2020 2020 7365 6c66 2e43 6861          self.Cha
-000014f0: 6e6e 656c 4253 6c6f 7065 203d 204e 6f6e  nnelBSlope = Non
-00001500: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001510: 4368 616e 6e65 6c42 4f66 6673 6574 203d  ChannelBOffset =
-00001520: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
-00001530: 656c 662e 4368 616e 6e65 6c43 4d61 7869  elf.ChannelCMaxi
-00001540: 6d75 6d20 3d20 4e6f 6e65 0d0a 2020 2020  mum = None..    
-00001550: 2020 2020 7365 6c66 2e43 6861 6e6e 656c      self.Channel
-00001560: 434d 696e 696d 756d 203d 204e 6f6e 650d  CMinimum = None.
-00001570: 0a20 2020 2020 2020 2073 656c 662e 4368  .        self.Ch
-00001580: 616e 6e65 6c43 5661 7269 616e 6365 203d  annelCVariance =
-00001590: 204e 6f6e 650d 0a20 2020 2020 2020 2073   None..        s
-000015a0: 656c 662e 4368 616e 6e65 6c43 536c 6f70  elf.ChannelCSlop
-000015b0: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
-000015c0: 2020 7365 6c66 2e43 6861 6e6e 656c 434f    self.ChannelCO
-000015d0: 6666 7365 7420 3d20 4e6f 6e65 0d0a 2020  ffset = None..  
-000015e0: 2020 2020 2020 7365 6c66 2e43 6861 6e6e        self.Chann
-000015f0: 656c 444d 6178 696d 756d 203d 204e 6f6e  elDMaximum = Non
-00001600: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001610: 4368 616e 6e65 6c44 4d69 6e69 6d75 6d20  ChannelDMinimum 
-00001620: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00001630: 7365 6c66 2e43 6861 6e6e 656c 4456 6172  self.ChannelDVar
-00001640: 6961 6e63 6520 3d20 4e6f 6e65 0d0a 2020  iance = None..  
-00001650: 2020 2020 2020 7365 6c66 2e43 6861 6e6e        self.Chann
-00001660: 656c 4453 6c6f 7065 203d 204e 6f6e 650d  elDSlope = None.
-00001670: 0a20 2020 2020 2020 2073 656c 662e 4368  .        self.Ch
-00001680: 616e 6e65 6c44 4f66 6673 6574 203d 204e  annelDOffset = N
-00001690: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-000016a0: 662e 6469 726e 616d 6520 3d20 4e6f 6e65  f.dirname = None
-000016b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
-000016c0: 696c 6520 3d20 4e6f 6e65 0d0a 2020 2020  ile = None..    
-000016d0: 2020 2020 7365 6c66 2e66 696c 656e 616d      self.filenam
-000016e0: 6520 3d20 6669 6c65 6e61 6d65 0d0a 2020  e = filename..  
-000016f0: 2020 2020 2020 7365 6c66 2e66 7265 7175        self.frequ
-00001700: 656e 6379 203d 204e 6f6e 650d 0a0d 0a20  ency = None.... 
-00001710: 2020 2020 2020 2069 6620 6669 6c65 6e61         if filena
-00001720: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0d  me is not None:.
-00001730: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001740: 6120 3d20 7064 2e72 6561 645f 6373 7628  a = pd.read_csv(
-00001750: 6669 6c65 6e61 6d65 2c20 6865 6164 6572  filename, header
-00001760: 3d4e 6f6e 652c 2064 656c 696d 6974 6572  =None, delimiter
-00001770: 3d22 5c74 2229 0d0a 0d0a 2020 2020 2020  ="\t")....      
-00001780: 2020 2020 2020 696e 6420 3d20 300d 0a20        ind = 0.. 
-00001790: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000017a0: 2069 6e20 7261 6e67 6528 6461 7461 2e73   in range(data.s
-000017b0: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
-000017c0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-000017d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000017e0: 2020 2020 2066 6c6f 6174 2864 6174 615b       float(data[
-000017f0: 305d 5b69 5d29 0d0a 2020 2020 2020 2020  0][i])..        
-00001800: 2020 2020 2020 2020 6578 6365 7074 2056          except V
-00001810: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 696e 6420 3d20 6920 2b20 310d 0a20 2020  ind = i + 1..   
-00001840: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00001850: 730d 0a0d 0a20 2020 2020 2020 2020 2020  s....           
-00001860: 206b 6579 7320 3d20 6461 7461 5b30 5d5b   keys = data[0][
-00001870: 303a 696e 645d 2e74 6f5f 6c69 7374 2829  0:ind].to_list()
-00001880: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00001890: 6c73 203d 2064 6174 615b 315d 5b30 3a69  ls = data[1][0:i
-000018a0: 6e64 5d2e 746f 5f6c 6973 7428 290d 0a0d  nd].to_list()...
-000018b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000018c0: 206b 2069 6e20 7261 6e67 6528 6c65 6e28   k in range(len(
-000018d0: 6b65 7973 2929 3a0d 0a20 2020 2020 2020  keys)):..       
-000018e0: 2020 2020 2020 2020 2069 6620 6b65 7973           if keys
-000018f0: 5b6b 5d20 696e 206c 6973 7428 7365 6c66  [k] in list(self
-00001900: 2e5f 5f64 6963 745f 5f2e 6b65 7973 2829  .__dict__.keys()
-00001910: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00001920: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2020 2020 666c 6f61 7428 7661 6c73        float(vals
-00001950: 5b6b 5d29 0d0a 2020 2020 2020 2020 2020  [k])..          
-00001960: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001970: 7461 7474 7228 7365 6c66 2c20 6b65 7973  tattr(self, keys
-00001980: 5b6b 5d2c 2066 6c6f 6174 2876 616c 735b  [k], float(vals[
-00001990: 6b5d 2929 0d0a 2020 2020 2020 2020 2020  k]))..          
-000019a0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-000019b0: 2056 616c 7565 4572 726f 723a 0d0a 2020   ValueError:..  
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 2020 2020 7365 7461 7474 7228 7365        setattr(se
-000019e0: 6c66 2c20 6b65 7973 5b6b 5d2c 2076 616c  lf, keys[k], val
-000019f0: 735b 6b5d 290d 0a0d 0a20 2020 2020 2020  s[k])....       
-00001a00: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 6d73 6720 3d20 2254 6865 2064      msg = "The d
-00001a30: 6174 6120 6b65 7920 6973 206e 6f74 2064  ata key is not d
-00001a40: 6566 6965 6422 0d0a 2020 2020 2020 2020  efied"..        
-00001a50: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00001a60: 6520 5761 726e 696e 6728 6d73 6729 0d0a  e Warning(msg)..
-00001a70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001a80: 6c66 2e74 696d 6520 3d20 6461 7461 5b30  lf.time = data[0
-00001a90: 5d5b 696e 643a 5d2e 746f 5f6e 756d 7079  ][ind:].to_numpy
-00001aa0: 2864 7479 7065 3d66 6c6f 6174 290d 0a20  (dtype=float).. 
-00001ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001ac0: 616d 706c 6974 7564 6520 3d20 6461 7461  amplitude = data
-00001ad0: 5b31 5d5b 696e 643a 5d2e 746f 5f6e 756d  [1][ind:].to_num
-00001ae0: 7079 2864 7479 7065 3d66 6c6f 6174 290d  py(dtype=float).
-00001af0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00001b00: 2043 616c 6375 6c61 7465 2066 7265 7175   Calculate frequ
-00001b10: 656e 6379 2072 616e 6765 0d0a 2020 2020  ency range..    
-00001b20: 2020 2020 2020 2020 7365 6c66 2e66 7265          self.fre
-00001b30: 7175 656e 6379 203d 2028 6e70 2e61 7261  quency = (np.ara
-00001b40: 6e67 6528 0d0a 2020 2020 2020 2020 2020  nge(..          
-00001b50: 2020 2020 2020 6e70 2e66 6c6f 6f72 286c        np.floor(l
-00001b60: 656e 2873 656c 662e 7469 6d65 2929 2920  en(self.time))) 
-00001b70: 2f20 3220 2d20 3129 2e54 202f 2028 0d0a  / 2 - 1).T / (..
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 2073 656c 662e 7469 6d65 5b2d       self.time[-
-00001bb0: 315d 202d 2073 656c 662e 7469 6d65 5b30  1] - self.time[0
-00001bc0: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
-00001bd0: 2020 2320 4361 6c63 756c 6174 6520 6666    # Calculate ff
-00001be0: 740d 0a20 2020 2020 2020 2020 2020 2066  t..            f
-00001bf0: 616d 7020 3d20 6e70 2e66 6674 2e66 6674  amp = np.fft.fft
-00001c00: 2873 656c 662e 616d 706c 6974 7564 6529  (self.amplitude)
-00001c10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001c20: 6c66 2e66 616d 7020 3d20 6661 6d70 5b30  lf.famp = famp[0
-00001c30: 3a69 6e74 286e 702e 666c 6f6f 7228 6c65  :int(np.floor(le
-00001c40: 6e28 6661 6d70 2920 2f20 3229 295d 0d0a  n(famp) / 2))]..
-00001c50: 0d0a 0d0a 6465 6620 7368 6966 746d 7478  ....def shiftmtx
-00001c60: 2874 6175 2c20 6e2c 2074 7329 3a0d 0a20  (tau, n, ts):.. 
-00001c70: 2020 2022 2222 0d0a 2020 2020 5368 6966     """..    Shif
-00001c80: 746d 7478 2063 6f6d 7075 7465 7320 7468  tmtx computes th
-00001c90: 6520 6e20 6279 206e 2074 7261 6e73 6665  e n by n transfe
-00001ca0: 7220 6d61 7472 6978 2066 6f72 2061 2063  r matrix for a c
-00001cb0: 6f6e 7469 6e75 6f75 7320 7469 6d65 2d73  ontinuous time-s
-00001cc0: 6869 6674 2e0d 0a0d 0a20 2020 2050 6172  hift.....    Par
-00001cd0: 616d 6574 6572 730d 0a20 2020 202d 2d2d  ameters..    ---
-00001ce0: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 2020 2020  --------....    
-00001cf0: 7461 7520 3a20 666c 6f61 740d 0a20 2020  tau : float..   
-00001d00: 2020 2020 2049 6e70 7574 2070 6172 616d       Input param
-00001d10: 6574 6572 7320 666f 7220 7468 6520 6675  eters for the fu
-00001d20: 6e63 7469 6f6e 0d0a 0d0a 2020 2020 6e20  nction....    n 
-00001d30: 3a20 696e 740d 0a20 2020 2020 2020 204e  : int..        N
-00001d40: 756d 6265 7220 6f66 2074 696d 6520 7361  umber of time sa
-00001d50: 6d70 6c65 730d 0a0d 0a20 2020 2074 733a  mples....    ts:
-00001d60: 2069 6e74 0d0a 2020 2020 2020 2020 7361   int..        sa
-00001d70: 6d70 6c69 6e67 2074 696d 650d 0a0d 0a20  mpling time.... 
-00001d80: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00001d90: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2068 3a20  -------..    h: 
-00001da0: 6e64 6172 7261 7920 6f72 206d 6174 7269  ndarray or matri
-00001db0: 780d 0a20 2020 2020 2020 2028 6e2c 206e  x..        (n, n
-00001dc0: 2920 5472 616e 7366 6572 206d 6174 7269  ) Transfer matri
-00001dd0: 780d 0a0d 0a20 2020 2022 2222 0d0a 0d0a  x....    """....
-00001de0: 2020 2020 2320 466f 7572 6965 7220 6d65      # Fourier me
-00001df0: 7468 6f64 0d0a 2020 2020 6620 3d20 7266  thod..    f = rf
-00001e00: 6674 6672 6571 286e 2c20 7473 290d 0a20  ftfreq(n, ts).. 
-00001e10: 2020 2077 203d 2032 202a 206e 702e 7069     w = 2 * np.pi
-00001e20: 202a 2066 0d0a 0d0a 2020 2020 696d 7020   * f....    imp 
-00001e30: 3d20 6972 6666 7428 6e70 2e65 7870 282d  = irfft(np.exp(-
-00001e40: 316a 202a 2077 202a 2074 6175 292c 206e  1j * w * tau), n
-00001e50: 3d6e 290d 0a0d 0a20 2020 2023 2063 6f6d  =n)....    # com
-00001e60: 7075 7465 7320 7468 6520 6e20 6279 206e  putes the n by n
-00001e70: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-00001e80: 6d61 7472 6978 0d0a 2020 2020 6820 3d20  matrix..    h = 
-00001e90: 7363 6970 792e 6c69 6e61 6c67 2e74 6f65  scipy.linalg.toe
-00001ea0: 706c 6974 7a28 696d 702c 206e 702e 726f  plitz(imp, np.ro
-00001eb0: 6c6c 286e 702e 666c 6970 7564 2869 6d70  ll(np.flipud(imp
-00001ec0: 292c 2031 2929 0d0a 0d0a 2020 2020 7265  ), 1))....    re
-00001ed0: 7475 726e 2068 0d0a 0d0a 0d0a 6465 6620  turn h......def 
-00001ee0: 6169 7273 6361 6e63 6f72 7265 6374 2878  airscancorrect(x
-00001ef0: 2c20 7061 7261 6d29 3a0d 0a20 2020 2022  , param):..    "
-00001f00: 2222 4169 7273 6361 6e63 6f72 7265 6374  ""Airscancorrect
-00001f10: 2072 6573 6361 6c65 7320 616e 6420 7368   rescales and sh
-00001f20: 6966 7473 2065 6163 6820 636f 6c75 6d6e  ifts each column
-00001f30: 206f 6620 7468 6520 6461 7461 206d 6174   of the data mat
-00001f40: 7269 7820 782c 0d0a 2020 2020 6173 7375  rix x,..    assu
-00001f50: 6d69 6e67 2074 6861 7420 6561 6368 2063  ming that each c
-00001f60: 6f6c 756d 6e20 6973 2072 656c 6174 6564  olumn is related
-00001f70: 2074 6f20 6120 636f 6d6d 6f6e 2073 6967   to a common sig
-00001f80: 6e61 6c20 6279 2061 6e20 616d 706c 6974  nal by an amplit
-00001f90: 7564 6520 410d 0a20 2020 2061 6e64 2061  ude A..    and a
-00001fa0: 2064 656c 6179 2065 7461 2e0d 0a0d 0a20   delay eta..... 
-00001fb0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-00001fc0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00001fd0: 2020 2078 203a 206e 6461 7272 6179 206f     x : ndarray o
-00001fe0: 7220 6d61 7472 6978 0d0a 2020 2020 2020  r matrix..      
-00001ff0: 2020 286e 2c6d 2920 6461 7461 206d 6174    (n,m) data mat
-00002000: 7269 780d 0a0d 0a0d 0a20 2020 2070 6172  rix......    par
-00002010: 616d 3a20 6469 6374 0d0a 2020 2020 2020  am: dict..      
-00002020: 2020 5061 7261 6d65 7465 7220 6469 6374    Parameter dict
-00002030: 696f 6e61 7279 2069 6e63 6c75 6469 6e67  ionary including
-00002040: 3a0d 0a20 2020 2020 2020 2020 2020 2041  :..            A
-00002050: 203a 206e 6461 7272 6179 0d0a 2020 2020   : ndarray..    
-00002060: 2020 2020 2020 2020 2020 2020 286d 2c20              (m, 
-00002070: 2920 6172 7261 7920 636f 6e74 6169 6e69  ) array containi
-00002080: 6e67 2061 6d70 6c69 7475 6465 2076 6563  ng amplitude vec
-00002090: 746f 720d 0a20 2020 2020 2020 2020 2020  tor..           
-000020a0: 2065 7461 203a 206e 6461 7272 6179 0d0a   eta : ndarray..
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 286d 2c20 2920 6172 7261 7920 636f 6e74  (m, ) array cont
-000020d0: 6169 6e69 6e67 2064 656c 6179 2076 6563  aining delay vec
-000020e0: 746f 720d 0a20 2020 2020 2020 2020 2020  tor..           
-000020f0: 2074 7320 3a20 666c 6f61 740d 0a20 2020   ts : float..   
-00002100: 2020 2020 2020 2020 2020 2020 2073 616d               sam
-00002110: 706c 696e 6720 7469 6d65 0d0a 0d0a 0d0a  pling time......
-00002120: 0d0a 2020 2020 5265 7475 726e 730d 0a20  ..    Returns.. 
-00002130: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
-00002140: 7861 646a 203a 206e 6461 7272 6179 206f  xadj : ndarray o
-00002150: 7220 6d61 7472 6978 0d0a 2020 2020 2020  r matrix..      
-00002160: 2020 4164 6a75 7374 6564 2064 6174 6120    Adjusted data 
-00002170: 6d61 7472 6978 0d0a 0d0a 2020 2020 2222  matrix....    ""
-00002180: 220d 0a0d 0a20 2020 2023 2050 6172 7365  "....    # Parse
-00002190: 2066 756e 6374 696f 6e20 696e 7075 7473   function inputs
-000021a0: 0d0a 2020 2020 5b6e 2c20 6d5d 203d 2078  ..    [n, m] = x
-000021b0: 2e73 6861 7065 0d0a 0d0a 2020 2020 2320  .shape....    # 
-000021c0: 5061 7273 6520 7061 7261 6d65 7465 7220  Parse parameter 
-000021d0: 7374 7275 6374 7572 650d 0a20 2020 2070  structure..    p
-000021e0: 6669 656c 6473 203d 2070 6172 616d 2e6b  fields = param.k
-000021f0: 6579 7328 290d 0a20 2020 2069 6620 2261  eys()..    if "a
-00002200: 2220 696e 2070 6669 656c 6473 2061 6e64  " in pfields and
-00002210: 2070 6172 616d 2e67 6574 2822 6122 2920   param.get("a") 
-00002220: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00002230: 2020 2020 2020 6120 3d20 7061 7261 6d2e        a = param.
-00002240: 6765 7428 2261 2229 2e54 0d0a 2020 2020  get("a").T..    
-00002250: 656c 7365 3a0d 0a20 2020 2020 2020 2061  else:..        a
-00002260: 203d 206e 702e 6f6e 6573 2828 6d2c 2031   = np.ones((m, 1
-00002270: 2929 0d0a 2020 2020 2020 2020 2320 4967  ))..        # Ig
-00002280: 6e6f 7265 2e41 203d 2074 7275 650d 0a20  nore.A = true.. 
-00002290: 2020 2069 6620 2265 7461 2220 696e 2070     if "eta" in p
-000022a0: 6669 656c 6473 2061 6e64 2070 6172 616d  fields and param
-000022b0: 2e67 6574 2822 6574 6122 2920 6973 206e  .get("eta") is n
-000022c0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000022d0: 2020 6574 6120 3d20 7061 7261 6d2e 6765    eta = param.ge
-000022e0: 7428 2265 7461 2229 0d0a 2020 2020 656c  t("eta")..    el
-000022f0: 7365 3a0d 0a20 2020 2020 2020 2065 7461  se:..        eta
-00002300: 203d 206e 702e 7a65 726f 7328 286d 2c20   = np.zeros((m, 
-00002310: 3129 290d 0a20 2020 2069 6620 2274 7322  1))..    if "ts"
-00002320: 2069 6e20 7066 6965 6c64 733a 0d0a 2020   in pfields:..  
-00002330: 2020 2020 2020 7473 203d 2070 6172 616d        ts = param
-00002340: 5b22 7473 225d 0d0a 2020 2020 656c 7365  ["ts"]..    else
-00002350: 3a0d 0a20 2020 2020 2020 2074 7320 3d20  :..        ts = 
-00002360: 310d 0a0d 0a20 2020 2078 6164 6a20 3d20  1....    xadj = 
-00002370: 6e70 2e7a 6572 6f73 2828 6e2c 206d 2929  np.zeros((n, m))
-00002380: 0d0a 2020 2020 666f 7220 6920 696e 206e  ..    for i in n
-00002390: 702e 6172 616e 6765 286d 293a 0d0a 2020  p.arange(m):..  
-000023a0: 2020 2020 2020 7320 3d20 7368 6966 746d        s = shiftm
-000023b0: 7478 282d 6574 615b 695d 2c20 6e2c 2074  tx(-eta[i], n, t
-000023c0: 7329 0d0a 2020 2020 2020 2020 7861 646a  s)..        xadj
-000023d0: 5b3a 2c20 695d 203d 2073 2040 2028 785b  [:, i] = s @ (x[
-000023e0: 3a2c 2069 5d20 2f20 615b 695d 290d 0a0d  :, i] / a[i])...
-000023f0: 0a20 2020 2072 6574 7572 6e20 7861 646a  .    return xadj
-00002400: 0d0a 0d0a 0d0a 6465 6620 636f 7374 6675  ......def costfu
-00002410: 6e6c 7371 2866 756e 2c20 7468 6574 612c  nlsq(fun, theta,
-00002420: 2078 782c 2079 792c 2073 6967 6d61 782c   xx, yy, sigmax,
-00002430: 2073 6967 6d61 792c 2074 7329 3a0d 0a20   sigmay, ts):.. 
-00002440: 2020 2072 2222 2243 6f6d 7075 7465 7320     r"""Computes 
-00002450: 7468 6520 6d61 7869 6d75 6d20 6c69 6b65  the maximum like
-00002460: 6c69 686f 6f64 2063 6f73 7420 6675 6e63  lihood cost func
-00002470: 7469 6f6e 2e0d 0a0d 0a20 2020 2050 6172  tion.....    Par
-00002480: 616d 6574 6572 730d 0a20 2020 202d 2d2d  ameters..    ---
-00002490: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000024a0: 2066 756e 203a 2063 616c 6c61 626c 650d   fun : callable.
-000024b0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
-000024c0: 6e73 6665 7220 6675 6e63 7469 6f6e 2c20  nsfer function, 
-000024d0: 696e 2074 6865 2066 6f72 6d20 6675 6e28  in the form fun(
-000024e0: 7468 6574 612c 7729 2c20 2d69 7774 2063  theta,w), -iwt c
-000024f0: 6f6e 7665 6e74 696f 6e2e 0d0a 0d0a 2020  onvention.....  
-00002500: 2020 2020 2020 7468 6574 6120 3a20 6e64        theta : nd
-00002510: 6172 7261 790d 0a20 2020 2020 2020 2020  array..         
-00002520: 2020 2049 6e70 7574 2070 6172 616d 6574     Input paramet
-00002530: 6572 7320 666f 7220 7468 6520 6675 6e63  ers for the func
-00002540: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
-00002550: 2078 7820 3a20 6e64 6172 7261 790d 0a20   xx : ndarray.. 
-00002560: 2020 2020 2020 2020 2020 204d 6561 7375             Measu
-00002570: 7265 6420 696e 7075 7420 7369 676e 616c  red input signal
-00002580: 2e0d 0a0d 0a20 2020 2020 2020 2079 7920  .....        yy 
-00002590: 3a20 6e64 6172 7261 790d 0a20 2020 2020  : ndarray..     
-000025a0: 2020 2020 2020 204d 6561 7375 7265 6420         Measured 
-000025b0: 6f75 7470 7574 2073 6967 6e61 6c2e 0d0a  output signal...
-000025c0: 0d0a 2020 2020 2020 2020 7369 676d 6178  ..        sigmax
-000025d0: 203a 206e 6461 7272 6179 206f 7220 6d61   : ndarray or ma
-000025e0: 7472 6978 0d0a 2020 2020 2020 2020 2020  trix..          
-000025f0: 2020 4e6f 6973 6520 636f 7661 7269 616e    Noise covarian
-00002600: 6365 206d 6174 7269 7820 6f66 2074 6865  ce matrix of the
-00002610: 2069 6e70 7574 2073 6967 6e61 6c2e 0d0a   input signal...
-00002620: 0d0a 2020 2020 2020 2020 7369 676d 6179  ..        sigmay
-00002630: 203a 206e 6164 6172 7261 790d 0a20 2020   : nadarray..   
-00002640: 2020 2020 2020 2020 204e 6f69 7365 2063           Noise c
-00002650: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-00002660: 206f 6620 7468 6520 6f75 7470 7574 2073   of the output s
-00002670: 6967 6e61 6c2e 0d0a 0d0a 2020 2020 2020  ignal.....      
-00002680: 2020 7473 203a 2066 6c6f 6174 0d0a 2020    ts : float..  
-00002690: 2020 2020 2020 2020 2020 5361 6d70 6c69            Sampli
-000026a0: 6e67 2074 696d 652e 0d0a 0d0a 2020 2020  ng time.....    
-000026b0: 5265 7475 726e 730d 0a20 2020 202d 2d2d  Returns..    ---
-000026c0: 2d2d 2d2d 0d0a 2020 2020 7265 7320 3a20  ----..    res : 
-000026d0: 6361 6c6c 6162 6c65 0d0a 0d0a 0d0a 2020  callable......  
-000026e0: 2020 2222 220d 0a20 2020 206e 203d 2078    """..    n = x
-000026f0: 782e 7368 6170 655b 305d 0d0a 2020 2020  x.shape[0]..    
-00002700: 7766 6674 203d 2032 202a 206e 702e 7069  wfft = 2 * np.pi
-00002710: 202a 2072 6666 7466 7265 7128 6e2c 2074   * rfftfreq(n, t
-00002720: 7329 0d0a 2020 2020 6820 3d20 6e70 2e63  s)..    h = np.c
-00002730: 6f6e 6a28 6675 6e28 7468 6574 612c 2077  onj(fun(theta, w
-00002740: 6666 7429 290d 0a0d 0a20 2020 2072 7920  fft))....    ry 
-00002750: 3d20 7979 202d 2069 7266 6674 2872 6666  = yy - irfft(rff
-00002760: 7428 7878 2920 2a20 682c 206e 3d6e 290d  t(xx) * h, n=n).
-00002770: 0a20 2020 2076 7920 3d20 6e70 2e64 6961  .    vy = np.dia
-00002780: 6728 7369 676d 6179 202a 2a20 3229 0d0a  g(sigmay ** 2)..
-00002790: 0d0a 2020 2020 6874 696c 6465 203d 2069  ..    htilde = i
-000027a0: 7266 6674 2868 2c20 6e3d 6e29 0d0a 0d0a  rfft(h, n=n)....
-000027b0: 2020 2020 7579 203d 206e 702e 7a65 726f      uy = np.zero
-000027c0: 7328 286e 2c20 6e29 290d 0a20 2020 2066  s((n, n))..    f
-000027d0: 6f72 206b 2069 6e20 6e70 2e61 7261 6e67  or k in np.arang
-000027e0: 6528 6e29 3a0d 0a20 2020 2020 2020 2061  e(n):..        a
-000027f0: 203d 206e 702e 7265 7368 6170 6528 6e70   = np.reshape(np
-00002800: 2e72 6f6c 6c28 6874 696c 6465 2c20 6b29  .roll(htilde, k)
-00002810: 2c20 286e 2c20 3129 290d 0a20 2020 2020  , (n, 1))..     
-00002820: 2020 2062 203d 206e 702e 7265 7368 6170     b = np.reshap
-00002830: 6528 6e70 2e63 6f6e 6a28 6e70 2e72 6f6c  e(np.conj(np.rol
-00002840: 6c28 6874 696c 6465 2c20 6b29 292c 2028  l(htilde, k)), (
-00002850: 312c 206e 2929 0d0a 2020 2020 2020 2020  1, n))..        
-00002860: 7579 203d 2075 7920 2b20 6e70 2e72 6561  uy = uy + np.rea
-00002870: 6c28 6e70 2e64 6f74 2861 2c20 6229 2920  l(np.dot(a, b)) 
-00002880: 2a20 7369 676d 6178 5b6b 5d20 2a2a 2032  * sigmax[k] ** 2
-00002890: 0d0a 2020 2020 2020 2020 2320 7579 203d  ..        # uy =
-000028a0: 2075 7920 2b20 6e70 2e72 6561 6c28 6e70   uy + np.real(np
-000028b0: 2e72 6f6c 6c28 6874 696c 6465 2c20 6b2d  .roll(htilde, k-
-000028c0: 3129 2040 206e 702e 726f 6c6c 2868 7469  1) @ np.roll(hti
-000028d0: 6c64 652c 206b 2d31 292e 5429 2040 0d0a  lde, k-1).T) @..
-000028e0: 2020 2020 2020 2020 2320 7369 676d 6178          # sigmax
-000028f0: 5b6b 5d2a 2a32 0d0a 0d0a 2020 2020 7720  [k]**2....    w 
-00002900: 3d20 6e70 2e64 6f74 286e 702e 6579 6528  = np.dot(np.eye(
-00002910: 6e29 2c20 7363 6970 792e 6c69 6e61 6c67  n), scipy.linalg
-00002920: 2e69 6e76 2873 6369 7079 2e6c 696e 616c  .inv(scipy.linal
-00002930: 672e 7371 7274 6d28 7579 202b 2076 7929  g.sqrtm(uy + vy)
-00002940: 2929 0d0a 2020 2020 7265 7320 3d20 6e70  ))..    res = np
-00002950: 2e64 6f74 2877 2c20 7279 290d 0a0d 0a20  .dot(w, ry).... 
-00002960: 2020 2072 6574 7572 6e20 7265 730d 0a0d     return res...
-00002970: 0a0d 0a64 6566 2074 6474 6628 6675 6e2c  ...def tdtf(fun,
-00002980: 2074 6865 7461 2c20 6e2c 2074 7329 3a0d   theta, n, ts):.
-00002990: 0a20 2020 2022 2222 0d0a 2020 2020 5265  .    """..    Re
-000029a0: 7475 726e 7320 7468 6520 7472 616e 7366  turns the transf
-000029b0: 6572 206d 6174 7269 7820 666f 7220 6120  er matrix for a 
-000029c0: 6769 7665 6e20 6675 6e63 7469 6f6e 2e0d  given function..
-000029d0: 0a0d 0a20 2020 2049 7420 636f 6d70 7574  ...    It comput
-000029e0: 6573 2074 6865 206e 2d62 792d 6e20 7472  es the n-by-n tr
-000029f0: 616e 7366 6572 206d 6174 7269 7820 666f  ansfer matrix fo
-00002a00: 7220 7468 6520 6769 7665 6e20 6675 6e63  r the given func
-00002a10: 7469 6f6e 2066 756e 2077 6974 680d 0a20  tion fun with.. 
-00002a20: 2020 2069 6e70 7574 2070 6172 616d 6574     input paramet
-00002a30: 6572 2074 6865 7461 2e20 4e6f 7465 2074  er theta. Note t
-00002a40: 6861 7420 7468 6520 7472 616e 7366 6572  hat the transfer
-00002a50: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
-00002a60: 2062 6520 7772 6974 7465 6e0d 0a20 2020   be written..   
-00002a70: 2075 7369 6e67 2074 6865 2070 6879 7369   using the physi
-00002a80: 6369 7374 2773 202d 6977 7420 636f 6e76  cist's -iwt conv
-00002a90: 656e 7469 6f6e 2c20 616e 6420 7468 6174  ention, and that
-00002aa0: 2069 7420 7368 6f75 6c64 2062 6520 696e   it should be in
-00002ab0: 2074 6865 0d0a 2020 2020 666f 726d 6174   the..    format
-00002ac0: 2066 756e 2874 6865 7461 2c77 292c 2077   fun(theta,w), w
-00002ad0: 6865 7265 2074 6865 7461 0d0a 2020 2020  here theta..    
-00002ae0: 6973 2061 2076 6563 746f 7220 6f66 2074  is a vector of t
-00002af0: 6865 2066 756e 6374 696f 6e20 7061 7261  he function para
-00002b00: 6d65 7465 7273 2e20 5468 6520 7472 616e  meters. The tran
-00002b10: 7366 6572 2066 756e 6374 696f 6e20 6d75  sfer function mu
-00002b20: 7374 2062 650d 0a20 2020 2048 6572 6d69  st be..    Hermi
-00002b30: 7469 616e 2e0d 0a0d 0a20 2020 2050 6172  tian.....    Par
-00002b40: 616d 6574 6572 730d 0a20 2020 202d 2d2d  ameters..    ---
-00002b50: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-00002b60: 2066 756e 203a 2063 616c 6c61 626c 650d   fun : callable.
-00002b70: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
-00002b80: 6e73 6665 7220 6675 6e63 7469 6f6e 2c20  nsfer function, 
-00002b90: 696e 2074 6865 2066 6f72 6d20 6675 6e28  in the form fun(
-00002ba0: 7468 6574 612c 7729 2c20 2d69 7774 2063  theta,w), -iwt c
-00002bb0: 6f6e 7665 6e74 696f 6e2e 0d0a 0d0a 2020  onvention.....  
-00002bc0: 2020 2020 2020 7468 6574 6120 3a20 6e64        theta : nd
-00002bd0: 6172 7261 790d 0a20 2020 2020 2020 2020  array..         
-00002be0: 2020 2049 6e70 7574 2070 6172 616d 6574     Input paramet
-00002bf0: 6572 7320 666f 7220 7468 6520 6675 6e63  ers for the func
-00002c00: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
-00002c10: 206e 203a 2069 6e74 0d0a 2020 2020 2020   n : int..      
-00002c20: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
-00002c30: 7469 6d65 2073 616d 706c 6573 2e0d 0a0d  time samples....
-00002c40: 0a20 2020 2020 2020 2074 7320 3a20 6e64  .        ts : nd
-00002c50: 6172 7261 790d 0a20 2020 2020 2020 2020  array..         
-00002c60: 2020 2053 616d 706c 696e 6720 7469 6d65     Sampling time
-00002c70: 2e0d 0a0d 0a20 2020 2052 6574 7572 6e73  .....    Returns
-00002c80: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20  ..    -------.. 
-00002c90: 2020 2020 2020 2068 203a 206e 6461 7272         h : ndarr
-00002ca0: 6179 206f 7220 6d61 7472 6978 0d0a 2020  ay or matrix..  
-00002cb0: 2020 2020 2020 2020 2020 5472 616e 7366            Transf
-00002cc0: 6572 206d 6174 7269 7820 7769 7468 2073  er matrix with s
-00002cd0: 697a 6520 286e 2c6e 292e 0d0a 0d0a 2020  ize (n,n).....  
-00002ce0: 2020 2222 220d 0a0d 0a20 2020 2023 2063    """....    # c
-00002cf0: 6f6d 7075 7465 2074 6865 2074 7261 6e73  ompute the trans
-00002d00: 6665 7220 6675 6e63 7469 6f6e 206f 7665  fer function ove
-00002d10: 7220 706f 7369 7469 7665 2066 7265 7175  r positive frequ
-00002d20: 656e 6369 6573 0d0a 2020 2020 6966 206e  encies..    if n
-00002d30: 6f74 2069 7369 6e73 7461 6e63 6528 7473  ot isinstance(ts
-00002d40: 2c20 6e70 2e6e 6461 7272 6179 293a 0d0a  , np.ndarray):..
-00002d50: 2020 2020 2020 2020 7473 203d 206e 702e          ts = np.
-00002d60: 6172 7261 7928 5b74 735d 290d 0a20 2020  array([ts])..   
-00002d70: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00002d80: 7473 203d 2074 730d 0a0d 0a20 2020 2066  ts = ts....    f
-00002d90: 7320 3d20 3120 2f20 2874 7320 2a20 6e29  s = 1 / (ts * n)
-00002da0: 0d0a 2020 2020 6670 203d 2066 7320 2a20  ..    fp = fs * 
-00002db0: 6e70 2e61 7261 6e67 6528 302c 2028 6e20  np.arange(0, (n 
-00002dc0: 2d20 3129 202f 2f20 3220 2b20 3129 0d0a  - 1) // 2 + 1)..
-00002dd0: 2020 2020 7770 203d 2032 202a 206e 702e      wp = 2 * np.
-00002de0: 7069 202a 2066 700d 0a20 2020 2074 6675  pi * fp..    tfu
-00002df0: 6e70 203d 2066 756e 2874 6865 7461 2c20  np = fun(theta, 
-00002e00: 7770 290d 0a0d 0a20 2020 2023 2054 6865  wp)....    # The
-00002e10: 2074 7261 6e73 6665 7220 6675 6e63 7469   transfer functi
-00002e20: 6f6e 2069 7320 4865 726d 6974 6961 6e2c  on is Hermitian,
-00002e30: 2073 6f20 7765 2065 7661 6c75 6174 6520   so we evaluate 
-00002e40: 6e65 6761 7469 7665 2066 7265 7175 656e  negative frequen
-00002e50: 6369 6573 0d0a 2020 2020 2320 6279 2074  cies..    # by t
-00002e60: 616b 696e 6720 7468 6520 636f 6d70 6c65  aking the comple
-00002e70: 7820 636f 6e6a 7567 6174 6520 6f66 2074  x conjugate of t
-00002e80: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00002e90: 2070 6f73 6974 6976 6520 6672 6571 7565   positive freque
-00002ea0: 6e63 792e 0d0a 2020 2020 2320 496e 636c  ncy...    # Incl
-00002eb0: 7564 6520 7468 6520 7661 6c75 6520 6f66  ude the value of
-00002ec0: 2074 6865 2074 7261 6e73 6665 7220 6675   the transfer fu
-00002ed0: 6e63 7469 6f6e 2061 7420 7468 6520 4e79  nction at the Ny
-00002ee0: 7175 6973 7420 6672 6571 7565 6e63 7920  quist frequency 
-00002ef0: 666f 720d 0a20 2020 2023 2065 7665 6e20  for..    # even 
-00002f00: 6e2e 0d0a 2020 2020 6966 206e 2025 2032  n...    if n % 2
-00002f10: 2021 3d20 303a 0d0a 2020 2020 2020 2020   != 0:..        
-00002f20: 7466 756e 203d 206e 702e 636f 6e63 6174  tfun = np.concat
-00002f30: 656e 6174 6528 2874 6675 6e70 2c20 6e70  enate((tfunp, np
-00002f40: 2e63 6f6e 6a28 6e70 2e66 6c69 7075 6428  .conj(np.flipud(
-00002f50: 7466 756e 705b 313a 5d29 2929 290d 0a0d  tfunp[1:]))))...
-00002f60: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00002f70: 2020 2020 776e 7920 3d20 6e70 2e70 6920      wny = np.pi 
-00002f80: 2a20 6e20 2a20 6673 0d0a 2020 2020 2020  * n * fs..      
-00002f90: 2020 2320 7072 696e 7428 2774 6675 6e70    # print('tfunp
-00002fa0: 272c 2074 6675 6e70 290d 0a20 2020 2020  ', tfunp)..     
-00002fb0: 2020 2074 6675 6e20 3d20 6e70 2e63 6f6e     tfun = np.con
-00002fc0: 6361 7465 6e61 7465 280d 0a20 2020 2020  catenate(..     
-00002fd0: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
-00002fe0: 2020 2020 2020 2020 2020 7466 756e 702c            tfunp,
-00002ff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003000: 2020 6e70 2e63 6f6e 6a28 0d0a 2020 2020    np.conj(..    
-00003010: 2020 2020 2020 2020 2020 2020 206e 702e               np.
-00003020: 636f 6e63 6174 656e 6174 6528 2866 756e  concatenate((fun
-00003030: 2874 6865 7461 2c20 776e 7929 2c20 6e70  (theta, wny), np
-00003040: 2e66 6c69 7075 6428 7466 756e 705b 313a  .flipud(tfunp[1:
-00003050: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
-00003060: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-00003070: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00003080: 2020 290d 0a0d 0a20 2020 2023 2045 7661    )....    # Eva
-00003090: 6c75 6174 6520 7468 6520 696d 7075 6c73  luate the impuls
-000030a0: 6520 7265 7370 6f6e 7365 2062 7920 7461  e response by ta
-000030b0: 6b69 6e67 2074 6865 2069 6e76 6572 7365  king the inverse
-000030c0: 2046 6f75 7269 6572 2074 7261 6e73 666f   Fourier transfo
-000030d0: 726d 2c0d 0a20 2020 2023 2074 616b 696e  rm,..    # takin
-000030e0: 6720 7468 6520 636f 6d70 6c65 7820 636f  g the complex co
-000030f0: 6e6a 7567 6174 6520 6669 7273 7420 746f  njugate first to
-00003100: 2063 6f6e 7665 7274 2074 6f20 2e2e 2e20   convert to ... 
-00003110: 2b69 7774 2063 6f6e 7665 6e74 696f 6e0d  +iwt convention.
-00003120: 0a0d 0a20 2020 2069 6d70 203d 206e 702e  ...    imp = np.
-00003130: 7265 616c 286e 702e 6666 742e 6966 6674  real(np.fft.ifft
-00003140: 286e 702e 636f 6e6a 2874 6675 6e29 2929  (np.conj(tfun)))
-00003150: 0d0a 2020 2020 6820 3d20 7363 6970 792e  ..    h = scipy.
-00003160: 6c69 6e61 6c67 2e74 6f65 706c 6974 7a28  linalg.toeplitz(
-00003170: 696d 702c 206e 702e 726f 6c6c 286e 702e  imp, np.roll(np.
-00003180: 666c 6970 7564 2869 6d70 292c 2031 2929  flipud(imp), 1))
-00003190: 0d0a 0d0a 2020 2020 7265 7475 726e 2068  ....    return h
-000031a0: 0d0a 0d0a 0d0a 6465 6620 7464 6e6c 6c28  ......def tdnll(
-000031b0: 782c 2070 6172 616d 2c20 6669 7829 3a0d  x, param, fix):.
-000031c0: 0a20 2020 2072 2222 2220 436f 6d70 7574  .    r""" Comput
-000031d0: 6573 206e 6567 6174 6976 6520 6c6f 672d  es negative log-
-000031e0: 6c69 6b65 6c69 686f 6f64 2066 6f72 2074  likelihood for t
-000031f0: 6865 2074 696d 652d 646f 6d61 696e 206e  he time-domain n
-00003200: 6f69 7365 206d 6f64 656c 2e0d 0a0d 0a20  oise model..... 
-00003210: 2020 2043 6f6d 7075 7465 7320 7468 6520     Computes the 
-00003220: 6e65 6761 7469 7665 206c 6f67 2d6c 696b  negative log-lik
-00003230: 656c 6968 6f6f 6420 6675 6e63 7469 6f6e  elihood function
-00003240: 2066 6f72 206f 6274 6169 6e69 6e67 2074   for obtaining t
-00003250: 6865 0d0a 2020 2020 2064 6174 6120 6d61  he..     data ma
-00003260: 7472 6978 2078 2c20 6769 7665 6e20 7468  trix x, given th
-00003270: 6520 7061 7261 6d65 7465 7220 6469 6374  e parameter dict
-00003280: 696f 6e61 7279 2070 6172 616d 2e0d 0a0d  ionary param....
-00003290: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
-000032a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
-000032b0: 0a20 2020 2078 203a 206e 6461 7272 6179  .    x : ndarray
-000032c0: 206f 7220 6d61 7472 6978 0d0a 2020 2020   or matrix..    
-000032d0: 2020 2020 4461 7461 206d 6174 7269 780d      Data matrix.
-000032e0: 0a20 2020 2070 6172 616d 203a 2064 6963  .    param : dic
-000032f0: 740d 0a20 2020 2020 2020 2041 2064 6963  t..        A dic
-00003300: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-00003310: 6e67 2070 6172 616d 6574 6572 7320 696e  ng parameters in
-00003320: 636c 7564 696e 673a 0d0a 2020 2020 2020  cluding:..      
-00003330: 2020 6c6f 6776 203a 206e 6461 7272 6179    logv : ndarray
-00003340: 0d0a 2020 2020 2020 2020 2020 2020 4172  ..            Ar
-00003350: 7261 7920 6f66 2073 697a 6520 2833 2c20  ray of size (3, 
-00003360: 2920 636f 6e74 6169 6e69 6e67 206c 6f67  ) containing log
-00003370: 206f 6620 6e6f 6973 6520 7061 7261 6d65   of noise parame
-00003380: 7465 7273 2e0d 0a20 2020 2020 2020 206d  ters...        m
-00003390: 7520 3a20 6e64 6172 7261 790d 0a20 2020  u : ndarray..   
-000033a0: 2020 2020 2020 2020 2053 6967 6e61 6c20           Signal 
-000033b0: 7665 6374 6f72 206f 6620 7369 7a65 2028  vector of size (
-000033c0: 6e2c 292e 0d0a 2020 2020 2020 2020 613a  n,)...        a:
-000033d0: 206e 6461 7272 6179 0d0a 2020 2020 2020   ndarray..      
-000033e0: 2020 2020 2020 416d 706c 6974 7564 6520        Amplitude 
-000033f0: 7665 6374 6f72 206f 6620 7369 7a65 2028  vector of size (
-00003400: 6d2c 292e 0d0a 2020 2020 2020 2020 6574  m,)...        et
-00003410: 6120 3a20 6e64 6172 7261 790d 0a20 2020  a : ndarray..   
-00003420: 2020 2020 2020 2020 2044 656c 6179 2076           Delay v
-00003430: 6563 746f 7220 6f66 2073 697a 6520 286d  ector of size (m
-00003440: 2c29 2e0d 0a20 2020 2020 2020 2074 7320  ,)...        ts 
-00003450: 3a20 666c 6f61 740d 0a20 2020 2020 2020  : float..       
-00003460: 2020 2020 2053 616d 706c 696e 6720 7469       Sampling ti
-00003470: 6d65 2e0d 0a20 2020 2020 2020 2064 203a  me...        d :
-00003480: 206e 6461 7272 6179 206f 7220 6d61 7472   ndarray or matr
-00003490: 6978 0d0a 2020 2020 2020 2020 2020 2020  ix..            
-000034a0: 6e2d 6279 2d6e 2064 6572 6976 6174 6976  n-by-n derivativ
-000034b0: 6520 6d61 7472 6978 2e0d 0a20 2020 2066  e matrix...    f
-000034c0: 6978 203a 2064 6963 740d 0a20 2020 2020  ix : dict..     
-000034d0: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
-000034e0: 636f 6e74 6169 6e69 6e67 2076 6172 6961  containing varia
-000034f0: 626c 6573 2074 6f20 6669 7820 666f 7220  bles to fix for 
-00003500: 7468 6520 6772 6164 6965 6e74 2063 616c  the gradient cal
-00003510: 6375 6c61 7469 6f6e 2e0d 0a20 2020 2020  culation...     
-00003520: 2020 206c 6f67 7620 3a20 626f 6f6c 0d0a     logv : bool..
-00003530: 2020 2020 2020 2020 2020 2020 4c6f 6720              Log 
-00003540: 6f66 206e 6f69 7365 2070 6172 616d 6574  of noise paramet
-00003550: 6572 732e 0d0a 2020 2020 2020 2020 6d75  ers...        mu
-00003560: 203a 2062 6f6f 6c0d 0a20 2020 2020 2020   : bool..       
-00003570: 2020 2020 2053 6967 6e61 6c20 7665 6374       Signal vect
-00003580: 6f72 2e0d 0a20 2020 2020 2020 2061 203a  or...        a :
-00003590: 2062 6f6f 6c0d 0a20 2020 2020 2020 2020   bool..         
-000035a0: 2020 2041 6d70 6c69 7475 6465 2076 6563     Amplitude vec
-000035b0: 746f 722e 0d0a 2020 2020 2020 2020 6574  tor...        et
-000035c0: 6120 3a20 626f 6f6c 0d0a 2020 2020 2020  a : bool..      
-000035d0: 2020 2020 2020 4465 6c61 7920 7665 6374        Delay vect
-000035e0: 6f72 2e0d 0a0d 0a20 2020 2052 6574 7572  or.....    Retur
-000035f0: 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d  ns..    -------.
-00003600: 0a20 2020 206e 6c6c 203a 2063 616c 6c61  .    nll : calla
-00003610: 626c 650d 0a20 2020 2020 2020 204e 6567  ble..        Neg
-00003620: 6174 6976 6520 6c6f 672d 6c69 6b65 6c69  ative log-likeli
-00003630: 686f 6f64 2066 756e 6374 696f 6e0d 0a20  hood function.. 
-00003640: 2020 2067 7261 646e 6c6c 203a 206e 6461     gradnll : nda
-00003650: 7272 6179 0d0a 2020 2020 2020 2020 4772  rray..        Gr
-00003660: 6164 6965 6e74 206f 6620 7468 6520 6e65  adient of the ne
-00003670: 6761 7469 7665 206c 6f67 2d6c 696b 656c  gative log-likel
-00003680: 6968 6f6f 6420 6675 6e63 7469 6f6e 0d0a  ihood function..
-00003690: 2020 2020 2222 220d 0a20 2020 2023 2050      """..    # P
-000036a0: 6172 7365 2066 756e 6374 696f 6e20 696e  arse function in
-000036b0: 7075 7473 0d0a 2020 2020 5b6e 2c20 6d5d  puts..    [n, m]
-000036c0: 203d 2078 2e73 6861 7065 0d0a 0d0a 2020   = x.shape....  
-000036d0: 2020 2320 5061 7273 6520 7061 7261 6d65    # Parse parame
-000036e0: 7465 7220 6469 6374 696f 6e61 7279 0d0a  ter dictionary..
-000036f0: 2020 2020 7066 6965 6c64 7320 3d20 7061      pfields = pa
-00003700: 7261 6d2e 6b65 7973 2829 0d0a 2020 2020  ram.keys()..    
-00003710: 6967 6e6f 7265 203d 207b 7d0d 0a20 2020  ignore = {}..   
-00003720: 2069 6620 226c 6f67 7622 2069 6e20 7066   if "logv" in pf
-00003730: 6965 6c64 733a 0d0a 2020 2020 2020 2020  ields:..        
-00003740: 7620 3d20 6e70 2e65 7870 2870 6172 616d  v = np.exp(param
-00003750: 5b22 6c6f 6776 225d 290d 0a20 2020 2020  ["logv"])..     
-00003760: 2020 2076 203d 206e 702e 7265 7368 6170     v = np.reshap
-00003770: 6528 762c 2028 6c65 6e28 7629 2c20 3129  e(v, (len(v), 1)
-00003780: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
-00003790: 2020 2020 2020 6d73 6720 3d20 2254 646e        msg = "Tdn
-000037a0: 6c6c 2072 6571 7569 7265 7320 5061 7261  ll requires Para
-000037b0: 6d20 7374 7275 6374 7572 6520 7769 7468  m structure with
-000037c0: 206c 6f67 7620 6669 656c 6422 0d0a 2020   logv field"..  
-000037d0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000037e0: 6545 7272 6f72 286d 7367 290d 0a0d 0a20  eError(msg).... 
-000037f0: 2020 2069 6620 226d 7522 2069 6e20 7066     if "mu" in pf
-00003800: 6965 6c64 733a 0d0a 2020 2020 2020 2020  ields:..        
-00003810: 6d75 203d 2070 6172 616d 5b22 6d75 225d  mu = param["mu"]
-00003820: 0d0a 2020 2020 2020 2020 6d75 203d 206e  ..        mu = n
-00003830: 702e 7265 7368 6170 6528 6d75 2c20 286c  p.reshape(mu, (l
-00003840: 656e 286d 7529 2c20 3129 290d 0a20 2020  en(mu), 1))..   
-00003850: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00003860: 6d73 6720 3d20 2254 646e 6c6c 2072 6571  msg = "Tdnll req
-00003870: 7569 7265 7320 7061 7261 6d20 7374 7275  uires param stru
-00003880: 6374 7572 6520 7769 7468 206d 7520 6669  cture with mu fi
-00003890: 656c 6422 0d0a 2020 2020 2020 2020 7261  eld"..        ra
-000038a0: 6973 6520 5661 6c75 6545 7272 6f72 286d  ise ValueError(m
-000038b0: 7367 290d 0a20 2020 2070 6173 730d 0a0d  sg)..    pass...
-000038c0: 0a20 2020 2069 6620 2261 2220 696e 2070  .    if "a" in p
-000038d0: 6669 656c 6473 2061 6e64 2070 6172 616d  fields and param
-000038e0: 5b22 6122 5d20 213d 205b 5d3a 0d0a 2020  ["a"] != []:..  
-000038f0: 2020 2020 2020 6120 3d20 7061 7261 6d5b        a = param[
-00003900: 2261 225d 0d0a 2020 2020 2020 2020 6120  "a"]..        a 
-00003910: 3d20 6e70 2e72 6573 6861 7065 2861 2c20  = np.reshape(a, 
-00003920: 286c 656e 2861 292c 2031 2929 0d0a 2020  (len(a), 1))..  
-00003930: 2020 2020 2020 6967 6e6f 7265 5b22 6122        ignore["a"
-00003940: 5d20 3d20 4661 6c73 650d 0a20 2020 2065  ] = False..    e
-00003950: 6c73 653a 0d0a 2020 2020 2020 2020 6120  lse:..        a 
-00003960: 3d20 6e70 2e6f 6e65 7328 286d 2c20 3129  = np.ones((m, 1)
-00003970: 290d 0a20 2020 2020 2020 2069 676e 6f72  )..        ignor
-00003980: 655b 2261 225d 203d 2054 7275 650d 0a20  e["a"] = True.. 
-00003990: 2020 2070 6173 730d 0a0d 0a20 2020 2069     pass....    i
-000039a0: 6620 2265 7461 2220 696e 2070 6669 656c  f "eta" in pfiel
-000039b0: 6473 2061 6e64 2070 6172 616d 5b22 6574  ds and param["et
-000039c0: 6122 5d20 213d 205b 5d3a 0d0a 2020 2020  a"] != []:..    
-000039d0: 2020 2020 6574 6120 3d20 7061 7261 6d5b      eta = param[
-000039e0: 2265 7461 225d 0d0a 2020 2020 2020 2020  "eta"]..        
-000039f0: 6574 6120 3d20 6e70 2e72 6573 6861 7065  eta = np.reshape
-00003a00: 2865 7461 2c20 286c 656e 2865 7461 292c  (eta, (len(eta),
-00003a10: 2031 2929 0d0a 2020 2020 2020 2020 6967   1))..        ig
-00003a20: 6e6f 7265 5b22 6574 6122 5d20 3d20 4661  nore["eta"] = Fa
-00003a30: 6c73 650d 0a20 2020 2065 6c73 653a 0d0a  lse..    else:..
-00003a40: 2020 2020 2020 2020 6574 6120 3d20 6e70          eta = np
-00003a50: 2e7a 6572 6f73 2828 6d2c 2031 2929 0d0a  .zeros((m, 1))..
-00003a60: 2020 2020 2020 2020 6967 6e6f 7265 5b22          ignore["
-00003a70: 6574 6122 5d20 3d20 5472 7565 0d0a 2020  eta"] = True..  
-00003a80: 2020 7061 7373 0d0a 0d0a 2020 2020 6966    pass....    if
-00003a90: 2022 7473 2220 696e 2070 6669 656c 6473   "ts" in pfields
-00003aa0: 3a0d 0a20 2020 2020 2020 2074 7320 3d20  :..        ts = 
-00003ab0: 7061 7261 6d5b 2274 7322 5d0d 0a20 2020  param["ts"]..   
-00003ac0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00003ad0: 7473 203d 2031 0d0a 2020 2020 2020 2020  ts = 1..        
-00003ae0: 7761 726e 696e 6773 2e77 6172 6e28 0d0a  warnings.warn(..
-00003af0: 2020 2020 2020 2020 2020 2020 2254 444e              "TDN
-00003b00: 4c4c 2072 6563 6569 7665 6420 5061 7261  LL received Para
-00003b10: 6d20 7374 7275 6374 7572 6520 7769 7468  m structure with
-00003b20: 6f75 7420 7473 2066 6965 6c64 3b20 7365  out ts field; se
-00003b30: 7420 746f 206f 6e65 220d 0a20 2020 2020  t to one"..     
-00003b40: 2020 2029 0d0a 2020 2020 7061 7373 0d0a     )..    pass..
-00003b50: 0d0a 2020 2020 6966 2022 6422 2069 6e20  ..    if "d" in 
-00003b60: 7066 6965 6c64 733a 0d0a 2020 2020 2020  pfields:..      
-00003b70: 2020 6420 3d20 7061 7261 6d5b 2264 225d    d = param["d"]
-00003b80: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-00003b90: 2020 2020 2023 2043 6f6d 7075 7465 2064       # Compute d
-00003ba0: 6572 6976 6174 6976 6520 6d61 7472 6978  erivative matrix
-00003bb0: 0d0a 2020 2020 2020 2020 6465 6620 6675  ..        def fu
-00003bc0: 6e28 5f2c 205f 7729 3a0d 0a20 2020 2020  n(_, _w):..     
-00003bd0: 2020 2020 2020 2072 6574 7572 6e20 2d20         return - 
-00003be0: 316a 202a 205f 770d 0a0d 0a20 2020 2020  1j * _w....     
-00003bf0: 2020 2064 203d 2074 6474 6628 6675 6e2c     d = tdtf(fun,
-00003c00: 2030 2c20 6e2c 2074 7329 0d0a 2020 2020   0, n, ts)..    
-00003c10: 7061 7373 0d0a 0d0a 2020 2020 2320 436f  pass....    # Co
-00003c20: 6d70 7574 6520 6672 6571 7565 6e63 7920  mpute frequency 
-00003c30: 7665 6374 6f72 2061 6e64 2046 6f75 7269  vector and Fouri
-00003c40: 6572 2063 6f65 6666 6963 6965 6e74 7320  er coefficients 
-00003c50: 6f66 206d 750d 0a20 2020 2066 203d 2066  of mu..    f = f
-00003c60: 6674 6672 6571 286e 2c20 7473 290d 0a20  ftfreq(n, ts).. 
-00003c70: 2020 2077 203d 2032 202a 206e 702e 7069     w = 2 * np.pi
-00003c80: 202a 2066 0d0a 2020 2020 7720 3d20 772e   * f..    w = w.
-00003c90: 7265 7368 6170 6528 6c65 6e28 7729 2c20  reshape(len(w), 
-00003ca0: 3129 0d0a 2020 2020 6d75 5f66 203d 206e  1)..    mu_f = n
-00003cb0: 702e 6666 742e 6666 7428 6d75 2e66 6c61  p.fft.fft(mu.fla
-00003cc0: 7474 656e 2829 292e 7265 7368 6170 6528  tten()).reshape(
-00003cd0: 6c65 6e28 6d75 292c 2031 290d 0a0d 0a20  len(mu), 1).... 
-00003ce0: 2020 2067 7261 6463 616c 6320 3d20 6e70     gradcalc = np
-00003cf0: 2e6c 6f67 6963 616c 5f6e 6f74 280d 0a20  .logical_not(.. 
-00003d00: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
-00003d10: 2020 2020 2020 5b66 6978 5b22 6c6f 6776        [fix["logv
-00003d20: 225d 5d2c 0d0a 2020 2020 2020 2020 2020  "]],..          
-00003d30: 2020 5b66 6978 5b22 6d75 225d 5d2c 0d0a    [fix["mu"]],..
-00003d40: 2020 2020 2020 2020 2020 2020 5b66 6978              [fix
-00003d50: 5b22 6122 5d20 6f72 2069 676e 6f72 655b  ["a"] or ignore[
-00003d60: 2261 225d 5d2c 0d0a 2020 2020 2020 2020  "a"]],..        
-00003d70: 2020 2020 5b66 6978 5b22 6574 6122 5d20      [fix["eta"] 
-00003d80: 6f72 2069 676e 6f72 655b 2265 7461 225d  or ignore["eta"]
-00003d90: 5d0d 0a20 2020 2020 2020 205d 0d0a 2020  ]..        ]..  
-00003da0: 2020 290d 0a0d 0a20 2020 2069 6620 6967    )....    if ig
-00003db0: 6e6f 7265 5b22 6574 6122 5d3a 0d0a 2020  nore["eta"]:..  
-00003dc0: 2020 2020 2020 7a65 7461 203d 206d 7520        zeta = mu 
-00003dd0: 2a20 6e70 2e63 6f6e 6a28 6129 2e54 0d0a  * np.conj(a).T..
-00003de0: 2020 2020 2020 2020 7a65 7461 5f66 203d          zeta_f =
-00003df0: 206e 702e 6666 742e 6666 7428 7a65 7461   np.fft.fft(zeta
-00003e00: 2c20 6178 6973 3d30 290d 0a20 2020 2065  , axis=0)..    e
-00003e10: 6c73 653a 0d0a 2020 2020 2020 2020 6578  lse:..        ex
-00003e20: 705f 6977 6574 6120 3d20 6e70 2e65 7870  p_iweta = np.exp
-00003e30: 2831 6a20 2a20 6e70 2e74 696c 6528 772c  (1j * np.tile(w,
-00003e40: 206d 2920 2a20 6e70 2e63 6f6e 6a28 6e70   m) * np.conj(np
-00003e50: 2e74 696c 6528 6574 612c 206e 2929 2e54  .tile(eta, n)).T
-00003e60: 290d 0a20 2020 2020 2020 207a 6574 615f  )..        zeta_
-00003e70: 6620 3d20 280d 0a20 2020 2020 2020 2020  f = (..         
-00003e80: 2020 206e 702e 636f 6e6a 286e 702e 7469     np.conj(np.ti
-00003e90: 6c65 2861 2c20 6e29 292e 5420 2a20 6e70  le(a, n)).T * np
-00003ea0: 2e63 6f6e 6a28 6578 705f 6977 6574 6129  .conj(exp_iweta)
-00003eb0: 202a 206e 702e 7469 6c65 286d 755f 662c   * np.tile(mu_f,
-00003ec0: 206d 290d 0a20 2020 2020 2020 2029 0d0a   m)..        )..
-00003ed0: 2020 2020 2020 2020 7a65 7461 203d 206e          zeta = n
-00003ee0: 702e 7265 616c 286e 702e 6666 742e 6966  p.real(np.fft.if
-00003ef0: 6674 287a 6574 615f 662c 2061 7869 733d  ft(zeta_f, axis=
-00003f00: 3029 290d 0a0d 0a20 2020 2023 2043 6f6d  0))....    # Com
-00003f10: 7075 7465 206e 6567 6174 6976 6520 2d20  pute negative - 
-00003f20: 6c6f 6720 6c69 6b65 6c69 686f 6f64 2061  log likelihood a
-00003f30: 6e64 2067 7261 6469 656e 740d 0a0d 0a20  nd gradient.... 
-00003f40: 2020 2023 2043 6f6d 7075 7465 2072 6573     # Compute res
-00003f50: 6964 7561 6c73 2061 6e64 2074 6865 6972  iduals and their
-00003f60: 2073 7175 6172 6573 2066 6f72 2073 7562   squares for sub
-00003f70: 7365 7175 656e 7420 636f 6d70 7574 6174  sequent computat
-00003f80: 696f 6e73 0d0a 2020 2020 7265 7320 3d20  ions..    res = 
-00003f90: 7820 2d20 7a65 7461 0d0a 2020 2020 7265  x - zeta..    re
-00003fa0: 7373 7120 3d20 7265 7320 2a2a 2032 0d0a  ssq = res ** 2..
-00003fb0: 0d0a 2020 2020 2320 5369 6d70 6c65 7374  ..    # Simplest
-00003fc0: 2063 6173 653a 206a 7573 7420 7661 7269   case: just vari
-00003fd0: 616e 6365 2061 6e64 2073 6967 6e61 6c20  ance and signal 
-00003fe0: 7061 7261 6d65 7465 7273 2c20 4120 616e  parameters, A an
-00003ff0: 6420 6574 6120 6669 7865 6420 6174 0d0a  d eta fixed at..
-00004000: 2020 2020 2320 6465 6661 756c 7473 0d0a      # defaults..
-00004010: 2020 2020 6966 2069 676e 6f72 655b 2261      if ignore["a
-00004020: 225d 2061 6e64 2069 676e 6f72 655b 2265  "] and ignore["e
-00004030: 7461 225d 3a0d 0a20 2020 2020 2020 2064  ta"]:..        d
-00004040: 6d75 203d 206e 702e 7265 616c 286e 702e  mu = np.real(np.
-00004050: 6666 742e 6966 6674 2831 6a20 2a20 7720  fft.ifft(1j * w 
-00004060: 2a20 6d75 5f66 2c20 6178 6973 3d30 2929  * mu_f, axis=0))
-00004070: 0d0a 2020 2020 2020 2020 7661 6c70 6861  ..        valpha
-00004080: 203d 2076 5b30 5d0d 0a20 2020 2020 2020   = v[0]..       
-00004090: 2076 6265 7461 203d 2076 5b31 5d20 2a20   vbeta = v[1] * 
-000040a0: 6d75 202a 2a20 320d 0a20 2020 2020 2020  mu ** 2..       
-000040b0: 2076 7461 7520 3d20 765b 325d 202a 2064   vtau = v[2] * d
-000040c0: 6d75 202a 2a20 320d 0a20 2020 2020 2020  mu ** 2..       
-000040d0: 2076 746f 7420 3d20 7661 6c70 6861 202b   vtot = valpha +
-000040e0: 2076 6265 7461 202b 2076 7461 750d 0a0d   vbeta + vtau...
-000040f0: 0a20 2020 2020 2020 2072 6573 6e6f 726d  .        resnorm
-00004100: 7371 203d 2072 6573 7371 202f 206e 702e  sq = ressq / np.
-00004110: 7469 6c65 2876 746f 742c 206d 290d 0a20  tile(vtot, m).. 
-00004120: 2020 2020 2020 206e 6c6c 203d 2028 0d0a         nll = (..
-00004130: 2020 2020 2020 2020 2020 2020 6d20 2a20              m * 
-00004140: 6e20 2a20 6e70 2e6c 6f67 2832 202a 206e  n * np.log(2 * n
-00004150: 702e 7069 2920 2f20 320d 0a20 2020 2020  p.pi) / 2..     
-00004160: 2020 2020 2020 202b 2028 6d20 2f20 3229         + (m / 2)
-00004170: 202a 206e 702e 7375 6d28 6e70 2e6c 6f67   * np.sum(np.log
-00004180: 2876 746f 7429 290d 0a20 2020 2020 2020  (vtot))..       
-00004190: 2020 2020 202b 206e 702e 7375 6d28 7265       + np.sum(re
-000041a0: 736e 6f72 6d73 7129 202f 2032 0d0a 2020  snormsq) / 2..  
-000041b0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
-000041c0: 2020 2023 2043 6f6d 7075 7465 2067 7261     # Compute gra
-000041d0: 6469 656e 7420 6966 2072 6571 7565 7374  dient if request
-000041e0: 6564 0d0a 2020 2020 2020 2020 2320 6966  ed..        # if
-000041f0: 206e 6172 676f 7574 203e 2031 3a0d 0a20   nargout > 1:.. 
-00004200: 2020 2020 2020 206e 6772 6164 203d 206e         ngrad = n
-00004210: 702e 7375 6d28 6772 6164 6361 6c63 5b30  p.sum(gradcalc[0
-00004220: 3a32 5d20 2a20 5b5b 335d 2c20 5b6e 5d5d  :2] * [[3], [n]]
-00004230: 290d 0a20 2020 2020 2020 2067 7261 646e  )..        gradn
-00004240: 6c6c 203d 206e 702e 7a65 726f 7328 286e  ll = np.zeros((n
-00004250: 6772 6164 2c20 3129 290d 0a20 2020 2020  grad, 1))..     
-00004260: 2020 206e 7374 6172 7420 3d20 300d 0a20     nstart = 0.. 
-00004270: 2020 2020 2020 2064 7661 7220 3d20 2876         dvar = (v
-00004280: 746f 7420 2d20 6e70 2e6d 6561 6e28 7265  tot - np.mean(re
-00004290: 7373 712c 2061 7869 733d 3129 2e72 6573  ssq, axis=1).res
-000042a0: 6861 7065 286e 2c20 3129 2920 2f20 7674  hape(n, 1)) / vt
-000042b0: 6f74 202a 2a20 320d 0a20 2020 2020 2020  ot ** 2..       
-000042c0: 2069 6620 6772 6164 6361 6c63 5b30 5d3a   if gradcalc[0]:
-000042d0: 0d0a 2020 2020 2020 2020 2020 2020 6772  ..            gr
-000042e0: 6164 6e6c 6c5b 6e73 7461 7274 5d20 3d20  adnll[nstart] = 
-000042f0: 286d 202f 2032 2920 2a20 6e70 2e73 756d  (m / 2) * np.sum
-00004300: 2864 7661 7229 202a 2076 5b30 5d0d 0a20  (dvar) * v[0].. 
-00004310: 2020 2020 2020 2020 2020 2067 7261 646e             gradn
-00004320: 6c6c 5b6e 7374 6172 7420 2b20 315d 203d  ll[nstart + 1] =
-00004330: 2028 6d20 2f20 3229 202a 206e 702e 7375   (m / 2) * np.su
-00004340: 6d28 6d75 202a 2a20 3220 2a20 6476 6172  m(mu ** 2 * dvar
-00004350: 2920 2a20 765b 315d 0d0a 2020 2020 2020  ) * v[1]..      
-00004360: 2020 2020 2020 6772 6164 6e6c 6c5b 6e73        gradnll[ns
-00004370: 7461 7274 202b 2032 5d20 3d20 286d 202f  tart + 2] = (m /
-00004380: 2032 2920 2a20 6e70 2e73 756d 2864 6d75   2) * np.sum(dmu
-00004390: 202a 2a20 322e 202a 2064 7661 7229 202a   ** 2. * dvar) *
-000043a0: 2076 5b32 5d0d 0a20 2020 2020 2020 2020   v[2]..         
-000043b0: 2020 206e 7374 6172 7420 3d20 6e73 7461     nstart = nsta
-000043c0: 7274 202b 2033 0d0a 2020 2020 2020 2020  rt + 3..        
-000043d0: 6966 2067 7261 6463 616c 635b 315d 3a0d  if gradcalc[1]:.
-000043e0: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
-000043f0: 7269 6e74 2827 6d75 2073 6861 7065 203a  rint('mu shape :
-00004400: 2027 2c20 6d75 2e73 6861 7065 290d 0a20   ', mu.shape).. 
-00004410: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
-00004420: 6e74 2827 6476 6172 2073 6861 7065 3a20  nt('dvar shape: 
-00004430: 272c 2064 7661 722e 7368 6170 6529 0d0a  ', dvar.shape)..
-00004440: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
-00004450: 696e 7428 2764 2073 6861 7065 3a20 272c  int('d shape: ',
-00004460: 2064 2e73 6861 7065 290d 0a20 2020 2020   d.shape)..     
-00004470: 2020 2020 2020 2023 2070 7269 6e74 2827         # print('
-00004480: 446d 7520 7368 6170 653a 2027 2c20 646d  Dmu shape: ', dm
-00004490: 752e 7368 6170 6529 0d0a 2020 2020 2020  u.shape)..      
-000044a0: 2020 2020 2020 6772 6164 6e6c 6c5b 6e73        gradnll[ns
-000044b0: 7461 7274 3a6e 7374 6172 7420 2b20 6e5d  tart:nstart + n]
-000044c0: 203d 206d 202a 2028 0d0a 2020 2020 2020   = m * (..      
-000044d0: 2020 2020 2020 2020 2020 2020 2020 765b                v[
-000044e0: 315d 202a 206d 7520 2a20 6476 6172 0d0a  1] * mu * dvar..
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 2020 2b20 765b 325d 202a 206e 702e      + v[2] * np.
-00004510: 646f 7428 642e 542c 2028 646d 7520 2a20  dot(d.T, (dmu * 
-00004520: 6476 6172 2929 0d0a 2020 2020 2020 2020  dvar))..        
-00004530: 2020 2020 2020 2020 2020 2020 2d20 6e70              - np
-00004540: 2e6d 6561 6e28 7265 732c 2061 7869 733d  .mean(res, axis=
-00004550: 3129 2e72 6573 6861 7065 286e 2c20 3129  1).reshape(n, 1)
-00004560: 202f 2076 746f 740d 0a20 2020 2020 2020   / vtot..       
-00004570: 2020 2020 2029 0d0a 0d0a 2020 2020 2320       )....    # 
-00004580: 416c 7465 726e 6174 6976 6520 6361 7365  Alternative case
-00004590: 3a20 412c 2065 7461 2c20 6f72 2062 6f74  : A, eta, or bot
-000045a0: 6820 6172 6520 6e6f 7420 7365 7420 746f  h are not set to
-000045b0: 2064 6566 6175 6c74 730d 0a20 2020 2065   defaults..    e
-000045c0: 6c73 653a 0d0a 2020 2020 2020 2020 647a  lse:..        dz
-000045d0: 6574 6120 3d20 6e70 2e72 6561 6c28 6e70  eta = np.real(np
-000045e0: 2e66 6674 2e69 6666 7428 316a 202a 206e  .fft.ifft(1j * n
-000045f0: 702e 7469 6c65 2877 2c20 6d29 202a 207a  p.tile(w, m) * z
-00004600: 6574 615f 662c 2061 7869 733d 3029 290d  eta_f, axis=0)).
-00004610: 0a0d 0a20 2020 2020 2020 2076 616c 7068  ...        valph
-00004620: 6120 3d20 765b 305d 0d0a 2020 2020 2020  a = v[0]..      
-00004630: 2020 7662 6574 6120 3d20 765b 315d 202a    vbeta = v[1] *
-00004640: 207a 6574 6120 2a2a 2032 0d0a 2020 2020   zeta ** 2..    
-00004650: 2020 2020 7674 6175 203d 2076 5b32 5d20      vtau = v[2] 
-00004660: 2a20 647a 6574 6120 2a2a 2032 0d0a 2020  * dzeta ** 2..  
-00004670: 2020 2020 2020 7674 6f74 203d 2076 616c        vtot = val
-00004680: 7068 6120 2b20 7662 6574 6120 2b20 7674  pha + vbeta + vt
-00004690: 6175 0d0a 0d0a 2020 2020 2020 2020 7265  au....        re
-000046a0: 736e 6f72 6d73 7120 3d20 7265 7373 7120  snormsq = ressq 
-000046b0: 2f20 7674 6f74 0d0a 2020 2020 2020 2020  / vtot..        
-000046c0: 6e6c 6c20 3d20 280d 0a20 2020 2020 2020  nll = (..       
-000046d0: 2020 2020 206d 202a 206e 202a 206e 702e       m * n * np.
-000046e0: 6c6f 6728 3220 2a20 6e70 2e70 6929 202f  log(2 * np.pi) /
-000046f0: 2032 0d0a 2020 2020 2020 2020 2020 2020   2..            
-00004700: 2b20 6e70 2e73 756d 286e 702e 6c6f 6728  + np.sum(np.log(
-00004710: 7674 6f74 2929 202f 2032 0d0a 2020 2020  vtot)) / 2..    
-00004720: 2020 2020 2020 2020 2b20 6e70 2e73 756d          + np.sum
-00004730: 2872 6573 6e6f 726d 7371 2920 2f20 320d  (resnormsq) / 2.
-00004740: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
-00004750: 2020 2020 2020 2320 436f 6d70 7574 6520        # Compute 
-00004760: 6772 6164 6965 6e74 2069 6620 7265 7175  gradient if requ
-00004770: 6573 7465 640d 0a20 2020 2020 2020 2023  ested..        #
-00004780: 2069 6620 6e61 7267 6f75 7420 3e20 313a   if nargout > 1:
-00004790: 0d0a 2020 2020 2020 2020 6e67 7261 6420  ..        ngrad 
-000047a0: 3d20 6e70 2e73 756d 2867 7261 6463 616c  = np.sum(gradcal
-000047b0: 6320 2a20 5b5b 335d 2c20 5b6e 5d2c 205b  c * [[3], [n], [
-000047c0: 6d5d 2c20 5b6d 5d5d 290d 0a20 2020 2020  m], [m]])..     
-000047d0: 2020 2067 7261 646e 6c6c 203d 206e 702e     gradnll = np.
-000047e0: 7a65 726f 7328 286e 6772 6164 2c20 3129  zeros((ngrad, 1)
-000047f0: 290d 0a20 2020 2020 2020 206e 7374 6172  )..        nstar
-00004800: 7420 3d20 300d 0a20 2020 2020 2020 2072  t = 0..        r
-00004810: 6573 7774 203d 2072 6573 202f 2076 746f  eswt = res / vto
-00004820: 740d 0a20 2020 2020 2020 2064 7661 7220  t..        dvar 
-00004830: 3d20 2876 746f 7420 2d20 7265 7373 7129  = (vtot - ressq)
-00004840: 202f 2076 746f 7420 2a2a 2032 0d0a 2020   / vtot ** 2..  
-00004850: 2020 2020 2020 6966 2067 7261 6463 616c        if gradcal
-00004860: 635b 305d 3a0d 0a20 2020 2020 2020 2020  c[0]:..         
-00004870: 2020 2023 2047 7261 6469 656e 7420 7772     # Gradient wr
-00004880: 7420 6c6f 6776 0d0a 2020 2020 2020 2020  t logv..        
-00004890: 2020 2020 6772 6164 6e6c 6c5b 6e73 7461      gradnll[nsta
-000048a0: 7274 5d20 3d20 302e 3520 2a20 6e70 2e73  rt] = 0.5 * np.s
-000048b0: 756d 2864 7661 7229 202a 2076 5b30 5d0d  um(dvar) * v[0].
-000048c0: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
-000048d0: 646e 6c6c 5b6e 7374 6172 7420 2b20 315d  dnll[nstart + 1]
-000048e0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-000048f0: 2020 2020 2020 302e 3520 2a20 6e70 2e73        0.5 * np.s
-00004900: 756d 287a 6574 612e 666c 6174 7465 6e28  um(zeta.flatten(
-00004910: 2920 2a2a 2032 202a 2064 7661 722e 666c  ) ** 2 * dvar.fl
-00004920: 6174 7465 6e28 2929 202a 2076 5b31 5d0d  atten()) * v[1].
-00004930: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00004940: 2020 2020 2020 2020 2020 2020 6772 6164              grad
-00004950: 6e6c 6c5b 6e73 7461 7274 202b 2032 5d20  nll[nstart + 2] 
-00004960: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00004970: 2020 2020 2030 2e35 202a 206e 702e 7375       0.5 * np.su
-00004980: 6d28 647a 6574 612e 666c 6174 7465 6e28  m(dzeta.flatten(
-00004990: 2920 2a2a 2032 202a 2064 7661 722e 666c  ) ** 2 * dvar.fl
-000049a0: 6174 7465 6e28 2929 202a 2076 5b32 5d0d  atten()) * v[2].
-000049b0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-000049c0: 2020 2020 2020 2020 2020 2020 6e73 7461              nsta
-000049d0: 7274 203d 206e 7374 6172 7420 2b20 330d  rt = nstart + 3.
-000049e0: 0a20 2020 2020 2020 2069 6620 6772 6164  .        if grad
-000049f0: 6361 6c63 5b31 5d3a 0d0a 2020 2020 2020  calc[1]:..      
-00004a00: 2020 2020 2020 2320 4772 6164 6965 6e74        # Gradient
-00004a10: 2077 7274 206d 750d 0a20 2020 2020 2020   wrt mu..       
-00004a20: 2020 2020 2070 203d 2028 0d0a 2020 2020       p = (..    
-00004a30: 2020 2020 2020 2020 2020 2020 6e70 2e66              np.f
-00004a40: 6674 2e66 6674 2876 5b31 5d20 2a20 6476  ft.fft(v[1] * dv
-00004a50: 6172 202a 207a 6574 6120 2d20 7265 7377  ar * zeta - resw
-00004a60: 742c 2061 7869 733d 3029 0d0a 2020 2020  t, axis=0)..    
-00004a70: 2020 2020 2020 2020 2020 2020 2d20 316a              - 1j
-00004a80: 202a 2076 5b32 5d20 2a20 7720 2a20 6e70   * v[2] * w * np
-00004a90: 2e66 6674 2e66 6674 2864 7661 7220 2a20  .fft.fft(dvar * 
-00004aa0: 647a 6574 612c 2061 7869 733d 3029 0d0a  dzeta, axis=0)..
-00004ab0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00004ac0: 2020 2020 2020 2020 2020 2067 7261 646e             gradn
-00004ad0: 6c6c 5b6e 7374 6172 743a 6e73 7461 7274  ll[nstart:nstart
-00004ae0: 202b 206e 5d20 3d20 280d 0a20 2020 2020   + n] = (..     
-00004af0: 2020 2020 2020 2020 2020 206e 702e 7375             np.su
-00004b00: 6d28 6e70 2e63 6f6e 6a28 6129 2e54 0d0a  m(np.conj(a).T..
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 202a 206e 702e 7265 616c         * np.real
-00004b30: 286e 702e 6666 742e 6966 6674 2865 7870  (np.fft.ifft(exp
-00004b40: 5f69 7765 7461 202a 2070 2c20 6178 6973  _iweta * p, axis
-00004b50: 3d30 2929 2c20 6178 6973 3d31 0d0a 2020  =0)), axis=1..  
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2020 2020 2029 2e72 6573 6861 7065 286e       ).reshape(n
-00004b80: 2c20 3129 0d0a 2020 2020 2020 2020 2020  , 1)..          
-00004b90: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00004ba0: 206e 7374 6172 7420 3d20 6e73 7461 7274   nstart = nstart
-00004bb0: 202b 206e 0d0a 2020 2020 2020 2020 6966   + n..        if
-00004bc0: 2067 7261 6463 616c 635b 325d 3a0d 0a20   gradcalc[2]:.. 
-00004bd0: 2020 2020 2020 2020 2020 2023 2047 7261             # Gra
-00004be0: 6469 656e 7420 7772 7420 410d 0a20 2020  dient wrt A..   
-00004bf0: 2020 2020 2020 2020 2074 6572 6d20 3d20           term = 
-00004c00: 2876 746f 7420 2d20 7661 6c70 6861 2920  (vtot - valpha) 
-00004c10: 2a20 6476 6172 202d 2072 6573 7774 202a  * dvar - reswt *
-00004c20: 207a 6574 610d 0a20 2020 2020 2020 2020   zeta..         
-00004c30: 2020 2069 6620 6e70 2e61 6e79 286e 702e     if np.any(np.
-00004c40: 6973 636c 6f73 6528 612c 2030 2929 3a0d  isclose(a, 0)):.
-00004c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c60: 206d 7367 203d 2022 4f6e 6520 6f72 206d   msg = "One or m
-00004c70: 6f72 6520 656c 656d 656e 7473 206f 6620  ore elements of 
-00004c80: 7468 6520 616d 706c 6974 7564 6520 7665  the amplitude ve
-00004c90: 6374 6f72 2061 7265 2063 6c6f 7365 2074  ctor are close t
-00004ca0: 6f20 7a65 726f 2022 0d0a 2020 2020 2020  o zero "..      
-00004cb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004cc0: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 206d 7367 0d0a 2020 2020 2020 2020 2020   msg..          
-00004cf0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00004d00: 2020 2020 2067 7261 646e 6c6c 5b6e 7374       gradnll[nst
-00004d10: 6172 743a 6e73 7461 7274 202b 206d 5d20  art:nstart + m] 
-00004d20: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-00004d30: 2020 2020 2020 2020 206e 702e 636f 6e6a           np.conj
-00004d40: 286e 702e 7375 6d28 7465 726d 2c20 6178  (np.sum(term, ax
-00004d50: 6973 3d30 2929 2e72 6573 6861 7065 286d  is=0)).reshape(m
-00004d60: 2c20 3129 202f 2061 0d0a 2020 2020 2020  , 1) / a..      
-00004d70: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00004d80: 2020 2020 2069 6620 6e6f 7420 6669 785b       if not fix[
-00004d90: 226d 7522 5d3a 0d0a 2020 2020 2020 2020  "mu"]:..        
-00004da0: 2020 2020 2020 2020 6772 6164 6e6c 6c20          gradnll 
-00004db0: 3d20 6e70 2e64 656c 6574 6528 6772 6164  = np.delete(grad
-00004dc0: 6e6c 6c2c 206e 7374 6172 7429 0d0a 2020  nll, nstart)..  
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 6e73                ns
-00004de0: 7461 7274 203d 206e 7374 6172 7420 2b20  tart = nstart + 
-00004df0: 6d20 2d20 310d 0a20 2020 2020 2020 2020  m - 1..         
-00004e00: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00004e10: 2020 2020 2020 2020 2020 6e73 7461 7274            nstart
-00004e20: 203d 206e 7374 6172 7420 2b20 6d0d 0a20   = nstart + m.. 
-00004e30: 2020 2020 2020 2069 6620 6772 6164 6361         if gradca
-00004e40: 6c63 5b33 5d3a 0d0a 2020 2020 2020 2020  lc[3]:..        
-00004e50: 2020 2020 2320 4772 6164 6965 6e74 2077      # Gradient w
-00004e60: 7274 2065 7461 0d0a 2020 2020 2020 2020  rt eta..        
-00004e70: 2020 2020 6464 7a65 7461 203d 206e 702e      ddzeta = np.
-00004e80: 7265 616c 286e 702e 6666 742e 6966 6674  real(np.fft.ifft
-00004e90: 282d 6e70 2e74 696c 6528 772c 206d 2920  (-np.tile(w, m) 
-00004ea0: 2a2a 2032 202a 207a 6574 615f 662c 2061  ** 2 * zeta_f, a
-00004eb0: 7869 733d 3029 290d 0a20 2020 2020 2020  xis=0))..       
-00004ec0: 2020 2020 2067 7261 646e 6c6c 203d 206e       gradnll = n
-00004ed0: 702e 7371 7565 657a 6528 6772 6164 6e6c  p.squeeze(gradnl
-00004ee0: 6c29 0d0a 2020 2020 2020 2020 2020 2020  l)..            
-00004ef0: 6772 6164 6e6c 6c5b 6e73 7461 7274 3a6e  gradnll[nstart:n
-00004f00: 7374 6172 7420 2b20 6d5d 203d 202d 6e70  start + m] = -np
-00004f10: 2e73 756d 280d 0a20 2020 2020 2020 2020  .sum(..         
-00004f20: 2020 2020 2020 2064 7661 7220 2a20 287a         dvar * (z
-00004f30: 6574 6120 2a20 647a 6574 6120 2a20 765b  eta * dzeta * v[
-00004f40: 315d 202b 2064 7a65 7461 202a 2064 647a  1] + dzeta * ddz
-00004f50: 6574 6120 2a20 765b 325d 290d 0a20 2020  eta * v[2])..   
-00004f60: 2020 2020 2020 2020 2020 2020 202d 2072               - r
-00004f70: 6573 7774 202a 2064 7a65 7461 2c20 6178  eswt * dzeta, ax
-00004f80: 6973 3d30 0d0a 2020 2020 2020 2020 2020  is=0..          
-00004f90: 2020 292e 7265 7368 6170 6528 6d2c 290d    ).reshape(m,).
-00004fa0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00004fb0: 6620 6e6f 7420 6669 785b 226d 7522 5d3a  f not fix["mu"]:
-00004fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004fd0: 2020 6772 6164 6e6c 6c20 3d20 6e70 2e64    gradnll = np.d
-00004fe0: 656c 6574 6528 6772 6164 6e6c 6c2c 206e  elete(gradnll, n
-00004ff0: 7374 6172 7429 0d0a 2020 2020 6772 6164  start)..    grad
-00005000: 6e6c 6c20 3d20 6772 6164 6e6c 6c2e 666c  nll = gradnll.fl
-00005010: 6174 7465 6e28 290d 0a0d 0a20 2020 2072  atten()....    r
-00005020: 6574 7572 6e20 6e6c 6c2c 2067 7261 646e  eturn nll, gradn
-00005030: 6c6c 0d0a 0d0a 0d0a 6465 6620 7464 6e6f  ll......def tdno
-00005040: 6973 6566 6974 2878 2c20 7061 7261 6d2c  isefit(x, param,
-00005050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005060: 2066 6978 3d7b 226c 6f67 7622 3a20 4661   fix={"logv": Fa
-00005070: 6c73 652c 2022 6d75 223a 2046 616c 7365  lse, "mu": False
-00005080: 2c20 2261 223a 2054 7275 652c 2022 6574  , "a": True, "et
-00005090: 6122 3a20 5472 7565 7d2c 0d0a 2020 2020  a": True},..    
-000050a0: 2020 2020 2020 2020 2020 2069 676e 6f72             ignor
-000050b0: 653d 7b22 6122 3a20 5472 7565 2c20 2265  e={"a": True, "e
-000050c0: 7461 223a 2054 7275 657d 293a 0d0a 2020  ta": True}):..  
-000050d0: 2020 2222 2220 436f 6d70 7574 6573 2074    """ Computes t
-000050e0: 696d 652d 646f 6d61 696e 206e 6f69 7365  ime-domain noise
-000050f0: 206d 6f64 656c 2070 6172 616d 6574 6572   model parameter
-00005100: 732e 0d0a 0d0a 2020 2020 436f 6d70 7574  s.....    Comput
-00005110: 6573 2074 6865 206e 6f69 7365 2070 6172  es the noise par
-00005120: 616d 6574 6572 7320 7369 676d 6120 616e  ameters sigma an
-00005130: 6420 7468 6520 756e 6465 726c 7969 6e67  d the underlying
-00005140: 2073 6967 6e61 6c20 7665 6374 6f72 206d   signal vector m
-00005150: 750d 0a20 2020 2066 6f72 2074 6865 2064  u..    for the d
-00005160: 6174 6120 6d61 7472 6978 2078 2c20 7768  ata matrix x, wh
-00005170: 6572 6520 7468 6520 636f 6c75 6d6e 7320  ere the columns 
-00005180: 6f66 2078 2061 7265 2065 6163 6820 6e6f  of x are each no
-00005190: 6973 790d 0a20 2020 206d 6561 7375 7265  isy..    measure
-000051a0: 6d65 6e74 7320 6f66 206d 752e 0d0a 0d0a  ments of mu.....
-000051b0: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-000051c0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-000051d0: 2020 2020 7820 3a20 6e64 6172 7261 7920      x : ndarray 
-000051e0: 6f72 206d 6174 7269 780d 0a20 2020 2020  or matrix..     
-000051f0: 2020 2044 6174 6120 6d61 7472 6978 2e0d     Data matrix..
-00005200: 0a20 2020 2070 6172 616d 203a 2064 6963  .    param : dic
-00005210: 740d 0a20 2020 2020 2020 2041 2064 6963  t..        A dic
-00005220: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-00005230: 6e67 2069 6e69 7469 616c 2067 7565 7373  ng initial guess
-00005240: 2066 6f72 2074 6865 2070 6172 616d 6574   for the paramet
-00005250: 6572 733a 0d0a 2020 2020 2020 2020 7630  ers:..        v0
-00005260: 203a 206e 6461 7272 6179 0d0a 2020 2020   : ndarray..    
-00005270: 2020 2020 2020 2020 496e 6974 6961 6c20          Initial 
-00005280: 6775 6573 732c 206e 6f69 7365 206d 6f64  guess, noise mod
-00005290: 656c 2070 6172 616d 6574 6572 732e 2041  el parameters. A
-000052a0: 7272 6179 206f 6620 7265 616c 2065 6c65  rray of real ele
-000052b0: 6d65 6e74 7320 6f66 0d0a 2020 2020 2020  ments of..      
-000052c0: 2020 2020 2020 7369 7a65 2028 332c 2029        size (3, )
-000052d0: 0d0a 2020 2020 2020 2020 6d75 3020 3a20  ..        mu0 : 
-000052e0: 6e64 6172 7261 790d 0a20 2020 2020 2020  ndarray..       
-000052f0: 2020 2020 2049 6e69 7469 616c 2067 7565       Initial gue
-00005300: 7373 2c20 7369 676e 616c 2076 6563 746f  ss, signal vecto
-00005310: 722e 2041 7272 6179 206f 6620 7265 616c  r. Array of real
-00005320: 2065 6c65 6d65 6e74 7320 6f66 2073 697a   elements of siz
-00005330: 6520 2028 6e2c 2029 0d0a 2020 2020 2020  e  (n, )..      
-00005340: 2020 6130 203a 206e 6461 7272 6179 0d0a    a0 : ndarray..
-00005350: 2020 2020 2020 2020 2020 2020 496e 6974              Init
-00005360: 6961 6c20 6775 6573 732c 2061 6d70 6c69  ial guess, ampli
-00005370: 7475 6465 2076 6563 746f 722e 2041 7272  tude vector. Arr
-00005380: 6179 206f 6620 7265 616c 2065 6c65 6d65  ay of real eleme
-00005390: 6e74 7320 6f66 2073 697a 650d 0a20 2020  nts of size..   
-000053a0: 2020 2020 2020 2020 2028 6d2c 2029 0d0a           (m, )..
-000053b0: 2020 2020 2020 2020 6574 6130 203a 206e          eta0 : n
-000053c0: 6461 7272 6179 0d0a 2020 2020 2020 2020  darray..        
-000053d0: 2020 2020 496e 6974 6961 6c20 6775 6573      Initial gues
-000053e0: 732c 2064 656c 6179 2076 6563 746f 722e  s, delay vector.
-000053f0: 2041 7272 6179 206f 6620 7265 616c 2065   Array of real e
-00005400: 6c65 6d65 6e74 7320 6f66 2073 697a 6520  lements of size 
-00005410: 286d 2c20 290d 0a20 2020 2020 2020 2074  (m, )..        t
-00005420: 7320 3a20 666c 6f61 740d 0a20 2020 2020  s : float..     
-00005430: 2020 2020 2020 2053 616d 706c 696e 6720         Sampling 
-00005440: 7469 6d65 0d0a 2020 2020 6669 7820 3a20  time..    fix : 
-00005450: 6469 6374 2c20 6f70 7469 6f6e 616c 0d0a  dict, optional..
-00005460: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-00005470: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-00005480: 7661 7269 6162 6c65 7320 746f 2066 6978  variables to fix
-00005490: 2066 6f72 2074 6865 206d 696e 696d 697a   for the minimiz
-000054a0: 6174 696f 6e2e 0d0a 2020 2020 2020 2020  ation...        
-000054b0: 6c6f 6776 203a 2062 6f6f 6c0d 0a20 2020  logv : bool..   
-000054c0: 2020 2020 2020 2020 204c 6f67 206f 6620           Log of 
-000054d0: 6e6f 6973 6520 7061 7261 6d65 7465 7273  noise parameters
-000054e0: 2e0d 0a20 2020 2020 2020 206d 7520 3a20  ...        mu : 
-000054f0: 626f 6f6c 0d0a 2020 2020 2020 2020 2020  bool..          
-00005500: 2020 5369 676e 616c 2076 6563 746f 722e    Signal vector.
-00005510: 0d0a 2020 2020 2020 2020 6120 3a20 626f  ..        a : bo
-00005520: 6f6c 0d0a 2020 2020 2020 2020 2020 2020  ol..            
-00005530: 416d 706c 6974 7564 6520 7665 6374 6f72  Amplitude vector
-00005540: 2e0d 0a20 2020 2020 2020 2065 7461 203a  ...        eta :
-00005550: 2062 6f6f 6c0d 0a20 2020 2020 2020 2020   bool..         
-00005560: 2020 2044 656c 6179 2076 6563 746f 722e     Delay vector.
-00005570: 0d0a 2020 2020 2020 2020 4966 206e 6f74  ..        If not
-00005580: 2067 6976 656e 2c20 6368 6f73 656e 2074   given, chosen t
-00005590: 6f20 7365 7420 6672 6565 2061 6c6c 2074  o set free all t
-000055a0: 6865 2076 6172 6961 626c 6573 2e0d 0a20  he variables... 
-000055b0: 2020 2069 676e 6f72 6520 3a20 6469 6374     ignore : dict
-000055c0: 0d0a 2020 2020 2020 2020 4120 6469 6374  ..        A dict
-000055d0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-000055e0: 6720 7661 7269 6162 6c65 7320 746f 2069  g variables to i
-000055f0: 676e 6f72 6520 666f 7220 7468 6520 6d69  gnore for the mi
-00005600: 6e69 6d69 7a61 7469 6f6e 2e0d 0a20 2020  nimization...   
-00005610: 2020 2020 2061 203a 2062 6f6f 6c0d 0a20       a : bool.. 
-00005620: 2020 2020 2020 2020 2020 2041 6d70 6c69             Ampli
-00005630: 7475 6465 2076 6563 746f 722e 0d0a 2020  tude vector...  
-00005640: 2020 2020 2020 6574 6120 3a20 626f 6f6c        eta : bool
-00005650: 0d0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-00005660: 6c61 7920 7665 6374 6f72 2e0d 0a20 2020  lay vector...   
-00005670: 2020 2020 2049 6620 6e6f 7420 6769 7665       If not give
-00005680: 6e2c 2063 686f 7365 6e20 746f 2069 676e  n, chosen to ign
-00005690: 6f72 6520 626f 7468 2061 6d70 6c69 7475  ore both amplitu
-000056a0: 6465 2061 6e64 2064 656c 6179 2e0d 0a0d  de and delay....
-000056b0: 0a20 2020 2052 6574 7572 6e73 0d0a 2020  .    Returns..  
-000056c0: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
-000056d0: 7020 3a20 6469 6374 0d0a 2020 2020 2020  p : dict..      
-000056e0: 2020 4f75 7470 7574 2070 6172 616d 6574    Output paramet
-000056f0: 6572 2064 6963 7469 6f6e 6172 7920 636f  er dictionary co
-00005700: 6e74 6169 6e69 6e67 3a0d 0a20 2020 2020  ntaining:..     
-00005710: 2020 2020 2020 2065 7461 203a 206e 6461         eta : nda
-00005720: 7272 6179 0d0a 2020 2020 2020 2020 2020  rray..          
-00005730: 2020 2020 2020 4465 6c61 7920 7665 6374        Delay vect
-00005740: 6f72 2e0d 0a20 2020 2020 2020 2020 2020  or...           
-00005750: 2061 203a 206e 6461 7272 6179 0d0a 2020   a : ndarray..  
-00005760: 2020 2020 2020 2020 2020 2020 2020 416d                Am
-00005770: 706c 6974 7564 6520 7665 6374 6f72 2e0d  plitude vector..
-00005780: 0a20 2020 2020 2020 2020 2020 206d 7520  .            mu 
-00005790: 3a20 6e64 6172 7261 790d 0a20 2020 2020  : ndarray..     
-000057a0: 2020 2020 2020 2020 2020 2053 6967 6e61             Signa
-000057b0: 6c20 7665 6374 6f72 2e0d 0a20 2020 2020  l vector...     
-000057c0: 2020 2020 2020 2076 6172 203a 206e 6461         var : nda
-000057d0: 7272 6179 0d0a 2020 2020 2020 2020 2020  rray..          
-000057e0: 2020 2020 2020 4c6f 6720 6f66 206e 6f69        Log of noi
-000057f0: 7365 2070 6172 616d 6574 6572 730d 0a20  se parameters.. 
-00005800: 2020 2066 7661 6c20 3a20 666c 6f61 740d     fval : float.
-00005810: 0a20 2020 2020 2020 2056 616c 7565 206f  .        Value o
-00005820: 6620 4e4c 4c20 636f 7374 2066 756e 6374  f NLL cost funct
-00005830: 696f 6e20 6672 6f6d 2046 4d49 4e55 4e43  ion from FMINUNC
-00005840: 0d0a 2020 2020 4469 6167 6e6f 7374 6963  ..    Diagnostic
-00005850: 203a 2064 6963 740d 0a20 2020 2020 2020   : dict..       
-00005860: 2044 6963 7469 6f6e 6172 7920 636f 6e74   Dictionary cont
-00005870: 6169 6e69 6e67 2064 6961 676e 6f73 7469  aining diagnosti
-00005880: 6320 696e 666f 726d 6174 696f 6e0d 0a20  c information.. 
-00005890: 2020 2020 2020 2020 2020 2065 7272 203a             err :
-000058a0: 2064 6963 0d0a 2020 2020 2020 2020 2020   dic..          
-000058b0: 2020 2020 2020 4469 6374 696f 6e61 7279        Dictionary
-000058c0: 2063 6f6e 7461 696e 696e 6720 2065 7272   containing  err
-000058d0: 6f72 206f 6620 7468 6520 7061 7261 6d65  or of the parame
-000058e0: 7465 7273 2e0d 0a20 2020 2020 2020 2020  ters...         
-000058f0: 2020 2067 7261 6420 3a20 6e64 6172 7261     grad : ndarra
-00005900: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
-00005910: 2020 204e 6567 6174 6976 6520 6c6f 676c     Negative logl
-00005920: 696b 656c 6968 6f6f 6420 636f 7374 2066  ikelihood cost f
-00005930: 756e 6374 696f 6e20 6772 6164 6965 6e74  unction gradient
-00005940: 2066 726f 6d0d 0a20 2020 2020 2020 2020   from..         
-00005950: 2020 2020 2020 2073 6369 7079 2e6f 7074         scipy.opt
-00005960: 696d 697a 652e 6d69 6e69 6d69 7a65 2042  imize.minimize B
-00005970: 4647 5320 6d65 7468 6f64 2e0d 0a20 2020  FGS method...   
-00005980: 2020 2020 2020 2020 2068 6573 7369 616e           hessian
-00005990: 203a 206e 6461 7272 6179 0d0a 2020 2020   : ndarray..    
-000059a0: 2020 2020 2020 2020 2020 2020 4e65 6761              Nega
-000059b0: 7469 7665 206c 6f67 6c69 6b65 6c69 686f  tive loglikeliho
-000059c0: 6f64 2063 6f73 7420 6675 6e63 7469 6f6e  od cost function
-000059d0: 2068 6573 7369 616e 2066 726f 6d0d 0a20   hessian from.. 
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000059f0: 6369 7079 2e6f 7074 696d 697a 652e 6d69  cipy.optimize.mi
-00005a00: 6e69 6d69 7a65 2042 4647 5320 6d65 7468  nimize BFGS meth
-00005a10: 6f64 2e0d 0a20 2020 2022 2222 0d0a 2020  od...    """..  
-00005a20: 2020 6e2c 206d 203d 2078 2e73 6861 7065    n, m = x.shape
-00005a30: 0d0a 0d0a 2020 2020 2320 5061 7273 6520  ....    # Parse 
-00005a40: 496e 7075 7473 0d0a 2020 2020 6966 2022  Inputs..    if "
-00005a50: 7630 2220 696e 2070 6172 616d 3a0d 0a20  v0" in param:.. 
-00005a60: 2020 2020 2020 2076 3020 3d20 7061 7261         v0 = para
-00005a70: 6d5b 2276 3022 5d0d 0a20 2020 2065 6c73  m["v0"]..    els
-00005a80: 653a 0d0a 2020 2020 2020 2020 7630 203d  e:..        v0 =
-00005a90: 206e 702e 6d65 616e 286e 702e 7661 7228   np.mean(np.var(
-00005aa0: 782c 2031 2929 202a 206e 702e 6172 7261  x, 1)) * np.arra
-00005ab0: 7928 5b31 2c20 312c 2031 5d29 0d0a 2020  y([1, 1, 1])..  
-00005ac0: 2020 2020 2020 7061 7261 6d5b 2276 3022        param["v0"
-00005ad0: 5d20 3d20 7630 0d0a 0d0a 2020 2020 6966  ] = v0....    if
-00005ae0: 2022 6d75 3022 2069 6e20 7061 7261 6d3a   "mu0" in param:
-00005af0: 0d0a 2020 2020 2020 2020 6d75 3020 3d20  ..        mu0 = 
-00005b00: 7061 7261 6d5b 226d 7530 225d 0d0a 2020  param["mu0"]..  
-00005b10: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00005b20: 206d 7530 203d 206e 702e 6d65 616e 2878   mu0 = np.mean(x
-00005b30: 2c20 3129 0d0a 2020 2020 2020 2020 7061  , 1)..        pa
-00005b40: 7261 6d5b 226d 7530 225d 203d 206d 7530  ram["mu0"] = mu0
-00005b50: 0d0a 0d0a 2020 2020 6966 2022 6130 2220  ....    if "a0" 
-00005b60: 696e 2070 6172 616d 3a0d 0a20 2020 2020  in param:..     
-00005b70: 2020 2061 3020 3d20 7061 7261 6d5b 2261     a0 = param["a
-00005b80: 3022 5d0d 0a20 2020 2065 6c73 653a 0d0a  0"]..    else:..
-00005b90: 2020 2020 2020 2020 6130 203d 206e 702e          a0 = np.
-00005ba0: 6f6e 6573 286d 290d 0a20 2020 2020 2020  ones(m)..       
-00005bb0: 2070 6172 616d 5b22 6130 225d 203d 2061   param["a0"] = a
-00005bc0: 300d 0a0d 0a20 2020 2069 6620 2265 7461  0....    if "eta
-00005bd0: 3022 2069 6e20 7061 7261 6d3a 0d0a 2020  0" in param:..  
-00005be0: 2020 2020 2020 6574 6130 203d 2070 6172        eta0 = par
-00005bf0: 616d 5b22 6574 6130 225d 0d0a 2020 2020  am["eta0"]..    
-00005c00: 656c 7365 3a0d 0a20 2020 2020 2020 2065  else:..        e
-00005c10: 7461 3020 3d20 6e70 2e7a 6572 6f73 286d  ta0 = np.zeros(m
-00005c20: 290d 0a20 2020 2020 2020 2070 6172 616d  )..        param
-00005c30: 5b22 6574 6130 225d 203d 2065 7461 300d  ["eta0"] = eta0.
-00005c40: 0a0d 0a20 2020 2069 6620 2274 7322 2069  ...    if "ts" i
-00005c50: 6e20 7061 7261 6d3a 0d0a 2020 2020 2020  n param:..      
-00005c60: 2020 7061 7261 6d5b 2274 7322 5d0d 0a20    param["ts"].. 
-00005c70: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00005c80: 2020 7061 7261 6d5b 2274 7322 5d20 3d20    param["ts"] = 
-00005c90: 310d 0a0d 0a20 2020 206d 6c65 203d 207b  1....    mle = {
-00005ca0: 2278 3022 3a20 6e70 2e61 7272 6179 285b  "x0": np.array([
-00005cb0: 5d29 7d0d 0a20 2020 2069 6478 7374 6172  ])}..    idxstar
-00005cc0: 7420 3d20 300d 0a20 2020 2069 6478 7261  t = 0..    idxra
-00005cd0: 6e67 6520 3d20 7b7d 0d0a 0d0a 2020 2020  nge = {}....    
-00005ce0: 2320 4966 2066 6978 5b27 6c6f 6776 275d  # If fix['logv']
-00005cf0: 2c20 7265 7475 726e 206c 6f67 2876 3029  , return log(v0)
-00005d00: 3b20 6f74 6865 7277 6973 6520 7265 7475  ; otherwise retu
-00005d10: 726e 206c 6f67 7620 7061 7261 6d65 7465  rn logv paramete
-00005d20: 7273 0d0a 2020 2020 6966 2066 6978 5b22  rs..    if fix["
-00005d30: 6c6f 6776 225d 3a0d 0a0d 0a20 2020 2020  logv"]:....     
-00005d40: 2020 2064 6566 2073 6574 706c 6f67 7628     def setplogv(
-00005d50: 5f29 3a0d 0a20 2020 2020 2020 2020 2020  _):..           
-00005d60: 2072 6574 7572 6e20 6e70 2e6c 6f67 2870   return np.log(p
-00005d70: 6172 616d 5b22 7630 225d 290d 0a0d 0a20  aram["v0"]).... 
-00005d80: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00005d90: 2020 6d6c 655b 2278 3022 5d20 3d20 6e70    mle["x0"] = np
-00005da0: 2e63 6f6e 6361 7465 6e61 7465 2828 6d6c  .concatenate((ml
-00005db0: 655b 2278 3022 5d2c 206e 702e 6c6f 6728  e["x0"], np.log(
-00005dc0: 7061 7261 6d5b 2276 3022 5d29 2929 0d0a  param["v0"])))..
-00005dd0: 2020 2020 2020 2020 6964 7865 6e64 203d          idxend =
-00005de0: 2069 6478 7374 6172 7420 2b20 330d 0a20   idxstart + 3.. 
-00005df0: 2020 2020 2020 2069 6478 7261 6e67 655b         idxrange[
-00005e00: 226c 6f67 7622 5d20 3d20 6e70 2e61 7261  "logv"] = np.ara
-00005e10: 6e67 6528 6964 7873 7461 7274 2c20 6964  nge(idxstart, id
-00005e20: 7865 6e64 290d 0a0d 0a20 2020 2020 2020  xend)....       
-00005e30: 2064 6566 2073 6574 706c 6f67 7628 5f70   def setplogv(_p
-00005e40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00005e50: 7265 7475 726e 205f 705b 6964 7872 616e  return _p[idxran
-00005e60: 6765 5b22 6c6f 6776 225d 5d0d 0a0d 0a20  ge["logv"]].... 
-00005e70: 2020 2020 2020 2069 6478 7374 6172 7420         idxstart 
-00005e80: 3d20 6964 7865 6e64 0d0a 2020 2020 7061  = idxend..    pa
-00005e90: 7373 0d0a 0d0a 2020 2020 2320 4966 2046  ss....    # If F
-00005ea0: 6978 5b27 6d75 275d 2c20 7265 7475 726e  ix['mu'], return
-00005eb0: 206d 7530 2c20 6f74 6865 7277 6973 652c   mu0, otherwise,
-00005ec0: 2072 6574 7572 6e20 6d75 2070 6172 616d   return mu param
-00005ed0: 6574 6572 730d 0a20 2020 2069 6620 6669  eters..    if fi
-00005ee0: 785b 226d 7522 5d3a 0d0a 0d0a 2020 2020  x["mu"]:....    
-00005ef0: 2020 2020 6465 6620 7365 7470 6d75 285f      def setpmu(_
-00005f00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00005f10: 7265 7475 726e 2070 6172 616d 5b22 6d75  return param["mu
-00005f20: 3022 5d0d 0a0d 0a20 2020 2065 6c73 653a  0"]....    else:
-00005f30: 0d0a 2020 2020 2020 2020 6d6c 655b 2278  ..        mle["x
-00005f40: 3022 5d20 3d20 6e70 2e63 6f6e 6361 7465  0"] = np.concate
-00005f50: 6e61 7465 2828 6d6c 655b 2278 3022 5d2c  nate((mle["x0"],
-00005f60: 2070 6172 616d 5b22 6d75 3022 5d29 290d   param["mu0"])).
-00005f70: 0a20 2020 2020 2020 2069 6478 656e 6420  .        idxend 
-00005f80: 3d20 6964 7873 7461 7274 202b 206e 0d0a  = idxstart + n..
-00005f90: 2020 2020 2020 2020 6964 7872 616e 6765          idxrange
-00005fa0: 5b22 6d75 225d 203d 206e 702e 6172 616e  ["mu"] = np.aran
-00005fb0: 6765 2869 6478 7374 6172 742c 2069 6478  ge(idxstart, idx
-00005fc0: 656e 6429 0d0a 0d0a 2020 2020 2020 2020  end)....        
-00005fd0: 6465 6620 7365 7470 6d75 285f 7029 3a0d  def setpmu(_p):.
-00005fe0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00005ff0: 7572 6e20 5f70 5b69 6478 7261 6e67 655b  urn _p[idxrange[
-00006000: 226d 7522 5d5d 0d0a 0d0a 2020 2020 2020  "mu"]]....      
-00006010: 2020 6964 7873 7461 7274 203d 2069 6478    idxstart = idx
-00006020: 656e 640d 0a20 2020 2070 6173 730d 0a0d  end..    pass...
-00006030: 0a20 2020 2023 2049 6620 6967 6e6f 7265  .    # If ignore
-00006040: 2041 2c20 7265 7475 726e 205b 5d3b 2069   A, return []; i
-00006050: 6620 4669 785b 2741 275d 2c20 7265 7475  f Fix['A'], retu
-00006060: 726e 2041 303b 2069 6620 7e46 6978 2e41  rn A0; if ~Fix.A
-00006070: 2026 2046 6978 2e6d 752c 0d0a 2020 2020   & Fix.mu,..    
-00006080: 2320 7265 7475 726e 2061 6c6c 2041 2070  # return all A p
-00006090: 6172 616d 6574 6572 733b 0d0a 2020 2020  arameters;..    
-000060a0: 2320 4966 207e 4669 782e 4120 2620 7e46  # If ~Fix.A & ~F
-000060b0: 6978 2e6d 752c 2072 6574 7572 6e20 616c  ix.mu, return al
-000060c0: 6c20 4120 7061 7261 6d65 7465 7273 2062  l A parameters b
-000060d0: 7574 2066 6972 7374 0d0a 0d0a 2020 2020  ut first....    
-000060e0: 6966 2069 676e 6f72 655b 2261 225d 3a0d  if ignore["a"]:.
-000060f0: 0a0d 0a20 2020 2020 2020 2064 6566 2073  ...        def s
-00006100: 6574 7061 285f 293a 0d0a 2020 2020 2020  etpa(_):..      
-00006110: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
-00006120: 0a0d 0a20 2020 2065 6c69 6620 6669 785b  ...    elif fix[
-00006130: 2261 225d 3a0d 0a0d 0a20 2020 2020 2020  "a"]:....       
-00006140: 2064 6566 2073 6574 7061 285f 293a 0d0a   def setpa(_):..
-00006150: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006160: 726e 2070 6172 616d 5b22 6130 225d 0d0a  rn param["a0"]..
-00006170: 0d0a 2020 2020 656c 6966 2066 6978 5b22  ..    elif fix["
-00006180: 6d75 225d 3a0d 0a20 2020 2020 2020 206d  mu"]:..        m
-00006190: 6c65 5b22 7830 225d 203d 206e 702e 636f  le["x0"] = np.co
-000061a0: 6e63 6174 656e 6174 6528 286d 6c65 5b22  ncatenate((mle["
-000061b0: 7830 225d 2c20 7061 7261 6d5b 2261 3022  x0"], param["a0"
-000061c0: 5d29 290d 0a20 2020 2020 2020 2069 6478  ]))..        idx
-000061d0: 656e 6420 3d20 6964 7873 7461 7274 202b  end = idxstart +
-000061e0: 206d 0d0a 2020 2020 2020 2020 6964 7872   m..        idxr
-000061f0: 616e 6765 5b22 6122 5d20 3d20 6e70 2e61  ange["a"] = np.a
-00006200: 7261 6e67 6528 6964 7873 7461 7274 2c20  range(idxstart, 
-00006210: 6964 7865 6e64 290d 0a0d 0a20 2020 2020  idxend)....     
-00006220: 2020 2064 6566 2073 6574 7061 285f 7029     def setpa(_p)
-00006230: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00006240: 6574 7572 6e20 5f70 5b69 6478 7261 6e67  eturn _p[idxrang
-00006250: 655b 2261 225d 5d0d 0a0d 0a20 2020 2020  e["a"]]....     
-00006260: 2020 2069 6478 7374 6172 7420 3d20 6964     idxstart = id
-00006270: 7865 6e64 0d0a 2020 2020 656c 7365 3a0d  xend..    else:.
-00006280: 0a20 2020 2020 2020 206d 6c65 5b22 7830  .        mle["x0
-00006290: 225d 203d 206e 702e 636f 6e63 6174 656e  "] = np.concaten
-000062a0: 6174 6528 0d0a 2020 2020 2020 2020 2020  ate(..          
-000062b0: 2020 286d 6c65 5b22 7830 225d 2c20 7061    (mle["x0"], pa
-000062c0: 7261 6d5b 2261 3022 5d5b 313a 5d20 2f20  ram["a0"][1:] / 
-000062d0: 7061 7261 6d5b 2261 3022 5d5b 305d 290d  param["a0"][0]).
-000062e0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-000062f0: 2020 2020 6964 7865 6e64 203d 2069 6478      idxend = idx
-00006300: 7374 6172 7420 2b20 6d20 2d20 310d 0a20  start + m - 1.. 
-00006310: 2020 2020 2020 2069 6478 7261 6e67 655b         idxrange[
-00006320: 2261 225d 203d 206e 702e 6172 616e 6765  "a"] = np.arange
-00006330: 2869 6478 7374 6172 742c 2069 6478 656e  (idxstart, idxen
-00006340: 6429 0d0a 0d0a 2020 2020 2020 2020 6465  d)....        de
-00006350: 6620 7365 7470 6128 5f70 293a 0d0a 2020  f setpa(_p):..  
-00006360: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006370: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
-00006380: 285b 315d 2c20 5f70 5b69 6478 7261 6e67  ([1], _p[idxrang
-00006390: 655b 2261 225d 5d29 2c20 6178 6973 3d30  e["a"]]), axis=0
-000063a0: 290d 0a0d 0a20 2020 2020 2020 2069 6478  )....        idx
-000063b0: 7374 6172 7420 3d20 6964 7865 6e64 0d0a  start = idxend..
-000063c0: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-000063d0: 2320 4966 2049 676e 6f72 652e 6574 612c  # If Ignore.eta,
-000063e0: 2072 6574 7572 6e20 5b5d 3b20 6966 2046   return []; if F
-000063f0: 6978 2e65 7461 2c20 7265 7475 726e 2065  ix.eta, return e
-00006400: 7461 303b 2069 6620 7e46 6978 2e65 7461  ta0; if ~Fix.eta
-00006410: 2026 0d0a 2020 2020 2320 4669 782e 6d75   &..    # Fix.mu
-00006420: 2c72 6574 7572 6e20 616c 6c20 6574 6120  ,return all eta 
-00006430: 7061 7261 6d65 7465 7273 3b0d 0a20 2020  parameters;..   
-00006440: 2023 2069 6620 7e46 6978 2e65 7461 2026   # if ~Fix.eta &
-00006450: 207e 4669 782e 6d75 2c20 7265 7475 726e   ~Fix.mu, return
-00006460: 2061 6c6c 2065 7461 2070 6172 616d 6574   all eta paramet
-00006470: 6572 7320 6275 7420 6669 7273 740d 0a0d  ers but first...
-00006480: 0a20 2020 2069 6620 6967 6e6f 7265 5b22  .    if ignore["
-00006490: 6574 6122 5d3a 0d0a 0d0a 2020 2020 2020  eta"]:....      
-000064a0: 2020 6465 6620 7365 7470 6574 6128 5f29    def setpeta(_)
-000064b0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000064c0: 6574 7572 6e20 5b5d 0d0a 0d0a 2020 2020  eturn []....    
-000064d0: 656c 6966 2066 6978 5b22 6574 6122 5d3a  elif fix["eta"]:
-000064e0: 0d0a 0d0a 2020 2020 2020 2020 6465 6620  ....        def 
-000064f0: 7365 7470 6574 6128 5f29 3a0d 0a20 2020  setpeta(_):..   
-00006500: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006510: 7061 7261 6d5b 2265 7461 3022 5d0d 0a0d  param["eta0"]...
-00006520: 0a20 2020 2065 6c69 6620 6669 785b 226d  .    elif fix["m
-00006530: 7522 5d3a 0d0a 2020 2020 2020 2020 6d6c  u"]:..        ml
-00006540: 655b 2278 3022 5d20 3d20 6e70 2e63 6f6e  e["x0"] = np.con
-00006550: 6361 7465 6e61 7465 2828 6d6c 655b 2278  catenate((mle["x
-00006560: 3022 5d2c 2070 6172 616d 5b22 6574 6130  0"], param["eta0
-00006570: 225d 2929 0d0a 2020 2020 2020 2020 6964  "]))..        id
-00006580: 7865 6e64 203d 2069 6478 7374 6172 7420  xend = idxstart 
-00006590: 2b20 6d0d 0a20 2020 2020 2020 2069 6478  + m..        idx
-000065a0: 7261 6e67 655b 2265 7461 225d 203d 206e  range["eta"] = n
-000065b0: 702e 6172 616e 6765 2869 6478 7374 6172  p.arange(idxstar
-000065c0: 742c 2069 6478 656e 6429 0d0a 0d0a 2020  t, idxend)....  
-000065d0: 2020 2020 2020 6465 6620 7365 7470 6574        def setpet
-000065e0: 6128 5f70 293a 0d0a 2020 2020 2020 2020  a(_p):..        
-000065f0: 2020 2020 7265 7475 726e 205f 705b 6964      return _p[id
-00006600: 7872 616e 6765 5b22 6574 6122 5d5d 0d0a  xrange["eta"]]..
-00006610: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-00006620: 2020 2020 206d 6c65 5b22 7830 225d 203d       mle["x0"] =
-00006630: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
-00006640: 0d0a 2020 2020 2020 2020 2020 2020 286d  ..            (m
-00006650: 6c65 5b22 7830 225d 2c20 7061 7261 6d5b  le["x0"], param[
-00006660: 2265 7461 3022 5d5b 313a 5d20 2d20 7061  "eta0"][1:] - pa
-00006670: 7261 6d5b 2265 7461 3022 5d5b 305d 290d  ram["eta0"][0]).
-00006680: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-00006690: 2020 2020 6964 7865 6e64 203d 2069 6478      idxend = idx
-000066a0: 7374 6172 7420 2b20 6d20 2d20 310d 0a20  start + m - 1.. 
-000066b0: 2020 2020 2020 2069 6478 7261 6e67 655b         idxrange[
-000066c0: 2265 7461 225d 203d 206e 702e 6172 616e  "eta"] = np.aran
-000066d0: 6765 2869 6478 7374 6172 742c 2069 6478  ge(idxstart, idx
-000066e0: 656e 6429 0d0a 0d0a 2020 2020 2020 2020  end)....        
-000066f0: 6465 6620 7365 7470 6574 6128 5f70 293a  def setpeta(_p):
-00006700: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006710: 7475 726e 206e 702e 636f 6e63 6174 656e  turn np.concaten
-00006720: 6174 6528 285b 305d 2c20 5f70 5b69 6478  ate(([0], _p[idx
-00006730: 7261 6e67 655b 2265 7461 225d 5d29 2c20  range["eta"]]), 
-00006740: 6178 6973 3d30 290d 0a20 2020 2070 6173  axis=0)..    pas
-00006750: 730d 0a0d 0a20 2020 2064 6566 2066 756e  s....    def fun
-00006760: 285f 2c20 5f77 293a 0d0a 2020 2020 2020  (_, _w):..      
-00006770: 2020 7265 7475 726e 202d 316a 202a 205f    return -1j * _
-00006780: 770d 0a0d 0a20 2020 2064 203d 2074 6474  w....    d = tdt
-00006790: 6628 6675 6e2c 2030 2c20 6e2c 2070 6172  f(fun, 0, n, par
-000067a0: 616d 5b22 7473 225d 290d 0a0d 0a20 2020  am["ts"])....   
-000067b0: 2064 6566 2070 6172 7365 696e 285f 7029   def parsein(_p)
-000067c0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-000067d0: 6e20 7b0d 0a20 2020 2020 2020 2020 2020  n {..           
-000067e0: 2022 6c6f 6776 223a 2073 6574 706c 6f67   "logv": setplog
-000067f0: 7628 5f70 292c 0d0a 2020 2020 2020 2020  v(_p),..        
-00006800: 2020 2020 226d 7522 3a20 7365 7470 6d75      "mu": setpmu
-00006810: 285f 7029 2c0d 0a20 2020 2020 2020 2020  (_p),..         
-00006820: 2020 2022 6122 3a20 7365 7470 6128 5f70     "a": setpa(_p
-00006830: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00006840: 2265 7461 223a 2073 6574 7065 7461 285f  "eta": setpeta(_
-00006850: 7029 2c0d 0a20 2020 2020 2020 2020 2020  p),..           
-00006860: 2022 7473 223a 2070 6172 616d 5b22 7473   "ts": param["ts
-00006870: 225d 2c0d 0a20 2020 2020 2020 2020 2020  "],..           
-00006880: 2022 6422 3a20 642c 0d0a 2020 2020 2020   "d": d,..      
-00006890: 2020 7d0d 0a0d 0a20 2020 2064 6566 206f    }....    def o
-000068a0: 626a 6563 7469 7665 285f 7029 3a0d 0a20  bjective(_p):.. 
-000068b0: 2020 2020 2020 2072 6574 7572 6e20 7464         return td
-000068c0: 6e6c 6c28 782c 2070 6172 7365 696e 285f  nll(x, parsein(_
-000068d0: 7029 2c20 6669 7829 5b30 5d0d 0a0d 0a20  p), fix)[0].... 
-000068e0: 2020 2064 6566 206a 6163 6f62 6961 6e28     def jacobian(
-000068f0: 5f70 293a 0d0a 2020 2020 2020 2020 7265  _p):..        re
-00006900: 7475 726e 2074 646e 6c6c 2878 2c20 7061  turn tdnll(x, pa
-00006910: 7273 6569 6e28 5f70 292c 2066 6978 295b  rsein(_p), fix)[
-00006920: 315d 0d0a 0d0a 2020 2020 6d6c 655b 226f  1]....    mle["o
-00006930: 626a 6563 7469 7665 225d 203d 206f 626a  bjective"] = obj
-00006940: 6563 7469 7665 0d0a 2020 2020 6f75 7420  ective..    out 
-00006950: 3d20 6d69 6e69 6d69 7a65 286d 6c65 5b22  = minimize(mle["
-00006960: 6f62 6a65 6374 6976 6522 5d2c 206d 6c65  objective"], mle
-00006970: 5b22 7830 225d 2c20 6d65 7468 6f64 3d22  ["x0"], method="
-00006980: 4246 4753 222c 206a 6163 3d6a 6163 6f62  BFGS", jac=jacob
-00006990: 6961 6e29 0d0a 0d0a 2020 2020 2320 5468  ian)....    # Th
-000069a0: 6520 7472 7573 742d 7265 6769 6f6e 2061  e trust-region a
-000069b0: 6c67 6f72 6974 686d 2072 6574 7572 6e73  lgorithm returns
-000069c0: 2074 6865 2048 6573 7369 616e 2066 6f72   the Hessian for
-000069d0: 2074 6865 206e 6578 742d 746f 2d6c 6173   the next-to-las
-000069e0: 740d 0a20 2020 2023 2069 7465 7261 7465  t..    # iterate
-000069f0: 2c20 7768 6963 6820 6d61 7920 6e6f 7420  , which may not 
-00006a00: 6265 206e 6561 7220 7468 6520 6669 6e61  be near the fina
-00006a10: 6c20 706f 696e 742e 2054 6f20 6368 6563  l point. To chec
-00006a20: 6b2c 2074 6573 7420 666f 720d 0a20 2020  k, test for..   
-00006a30: 2023 2070 6f73 6974 6976 6520 6465 6669   # positive defi
-00006a40: 6e69 7465 6e65 7373 2062 7920 6174 7465  niteness by atte
-00006a50: 6d70 7469 6e67 2074 6f20 4368 6f6c 6573  mpting to Choles
-00006a60: 6b79 2066 6163 746f 7269 7a65 2069 742e  ky factorize it.
-00006a70: 2049 6620 6974 0d0a 2020 2020 2320 7265   If it..    # re
-00006a80: 7475 726e 7320 616e 2065 7272 6f72 2c20  turns an error, 
-00006a90: 7265 7275 6e20 7468 6520 6f70 7469 6d69  rerun the optimi
-00006aa0: 7a61 7469 6f6e 2077 6974 6820 7468 6520  zation with the 
-00006ab0: 7175 6173 692d 4e65 7774 6f6e 2061 6c67  quasi-Newton alg
-00006ac0: 6f72 6974 686d 0d0a 2020 2020 2320 6672  orithm..    # fr
-00006ad0: 6f6d 2074 6865 2063 7572 7265 6e74 206f  om the current o
-00006ae0: 7074 696d 616c 2070 6f69 6e74 2e0d 0a0d  ptimal point....
-00006af0: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
-00006b00: 2020 206e 702e 6c69 6e61 6c67 2e63 686f     np.linalg.cho
-00006b10: 6c65 736b 7928 6e70 2e6c 696e 616c 672e  lesky(np.linalg.
-00006b20: 696e 7628 6f75 742e 6865 7373 5f69 6e76  inv(out.hess_inv
-00006b30: 2929 0d0a 2020 2020 2020 2020 6865 7373  ))..        hess
-00006b40: 203d 206e 702e 6c69 6e61 6c67 2e69 6e76   = np.linalg.inv
-00006b50: 286f 7574 2e68 6573 735f 696e 7629 0d0a  (out.hess_inv)..
-00006b60: 2020 2020 6578 6365 7074 206e 702e 6c69      except np.li
-00006b70: 6e61 6c67 2e4c 696e 416c 6745 7272 6f72  nalg.LinAlgError
-00006b80: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-00006b90: 280d 0a20 2020 2020 2020 2020 2020 2022  (..            "
-00006ba0: 4865 7373 6961 6e20 7265 7475 726e 6564  Hessian returned
-00006bb0: 2062 7920 464d 494e 554e 4320 6973 206e   by FMINUNC is n
-00006bc0: 6f74 2070 6f73 6974 6976 6520 6465 6669  ot positive defi
-00006bd0: 6e69 7465 3b5c 6e22 0d0a 2020 2020 2020  nite;\n"..      
-00006be0: 2020 2020 2020 2272 6563 616c 6375 6c61        "recalcula
-00006bf0: 7469 6e67 2077 6974 6820 7175 6173 692d  ting with quasi-
-00006c00: 4e65 7774 6f6e 2061 6c67 6f72 6974 686d  Newton algorithm
-00006c10: 220d 0a20 2020 2020 2020 2029 0d0a 0d0a  "..        )....
-00006c20: 2020 2020 2020 2020 6d6c 655b 2278 3022          mle["x0"
-00006c30: 5d20 3d20 6f75 742e 780d 0a20 2020 2020  ] = out.x..     
-00006c40: 2020 206f 7574 3220 3d20 6d69 6e69 6d69     out2 = minimi
-00006c50: 7a65 280d 0a20 2020 2020 2020 2020 2020  ze(..           
-00006c60: 206d 6c65 5b22 6f62 6a65 6374 6976 6522   mle["objective"
-00006c70: 5d2c 206d 6c65 5b22 7830 225d 2c20 6d65  ], mle["x0"], me
-00006c80: 7468 6f64 3d22 4246 4753 222c 206a 6163  thod="BFGS", jac
-00006c90: 3d6a 6163 6f62 6961 6e0d 0a20 2020 2020  =jacobian..     
-00006ca0: 2020 2029 0d0a 2020 2020 2020 2020 6865     )..        he
-00006cb0: 7373 203d 206e 702e 6c69 6e61 6c67 2e69  ss = np.linalg.i
-00006cc0: 6e76 286f 7574 322e 6865 7373 5f69 6e76  nv(out2.hess_inv
-00006cd0: 290d 0a0d 0a20 2020 2023 2050 6172 7365  )....    # Parse
-00006ce0: 206f 7574 7075 740d 0a20 2020 2070 203d   output..    p =
-00006cf0: 207b 7d0d 0a20 2020 2069 6478 7261 6e67   {}..    idxrang
-00006d00: 6520 3d20 7b7d 0d0a 2020 2020 6964 7873  e = {}..    idxs
-00006d10: 7461 7274 203d 2030 0d0a 0d0a 2020 2020  tart = 0....    
-00006d20: 6966 2066 6978 5b22 6c6f 6776 225d 3a0d  if fix["logv"]:.
-00006d30: 0a20 2020 2020 2020 2070 5b22 7661 7222  .        p["var"
-00006d40: 5d20 3d20 7061 7261 6d5b 2276 3022 5d0d  ] = param["v0"].
-00006d50: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00006d60: 2020 2020 6964 7865 6e64 203d 2069 6478      idxend = idx
-00006d70: 7374 6172 7420 2b20 330d 0a20 2020 2020  start + 3..     
-00006d80: 2020 2069 6478 7261 6e67 655b 226c 6f67     idxrange["log
-00006d90: 7622 5d20 3d20 6e70 2e61 7261 6e67 6528  v"] = np.arange(
-00006da0: 6964 7873 7461 7274 2c20 6964 7865 6e64  idxstart, idxend
-00006db0: 290d 0a20 2020 2020 2020 2069 6478 7374  )..        idxst
-00006dc0: 6172 7420 3d20 6964 7865 6e64 0d0a 2020  art = idxend..  
-00006dd0: 2020 2020 2020 705b 2276 6172 225d 203d        p["var"] =
-00006de0: 206e 702e 6578 7028 6f75 742e 785b 6964   np.exp(out.x[id
-00006df0: 7872 616e 6765 5b22 6c6f 6776 225d 5d29  xrange["logv"]])
-00006e00: 0d0a 2020 2020 7061 7373 0d0a 0d0a 2020  ..    pass....  
-00006e10: 2020 6966 2066 6978 5b22 6d75 225d 3a0d    if fix["mu"]:.
-00006e20: 0a20 2020 2020 2020 2070 5b22 6d75 225d  .        p["mu"]
-00006e30: 203d 2070 6172 616d 5b22 6d75 3022 5d0d   = param["mu0"].
-00006e40: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00006e50: 2020 2020 6964 7865 6e64 203d 2069 6478      idxend = idx
-00006e60: 7374 6172 7420 2b20 6e0d 0a20 2020 2020  start + n..     
-00006e70: 2020 2069 6478 7261 6e67 655b 226d 7522     idxrange["mu"
-00006e80: 5d20 3d20 6e70 2e61 7261 6e67 6528 6964  ] = np.arange(id
-00006e90: 7873 7461 7274 2c20 6964 7865 6e64 290d  xstart, idxend).
-00006ea0: 0a20 2020 2020 2020 2069 6478 7374 6172  .        idxstar
-00006eb0: 7420 3d20 6964 7865 6e64 0d0a 2020 2020  t = idxend..    
-00006ec0: 2020 2020 705b 226d 7522 5d20 3d20 6f75      p["mu"] = ou
-00006ed0: 742e 785b 6964 7872 616e 6765 5b22 6d75  t.x[idxrange["mu
-00006ee0: 225d 5d0d 0a20 2020 2070 6173 730d 0a0d  "]]..    pass...
-00006ef0: 0a20 2020 2069 6620 6967 6e6f 7265 5b22  .    if ignore["
-00006f00: 6122 5d20 6f72 2066 6978 5b22 6122 5d3a  a"] or fix["a"]:
-00006f10: 0d0a 2020 2020 2020 2020 705b 2261 225d  ..        p["a"]
-00006f20: 203d 2070 6172 616d 5b22 6130 225d 0d0a   = param["a0"]..
-00006f30: 2020 2020 656c 6966 2066 6978 5b22 6d75      elif fix["mu
-00006f40: 225d 3a0d 0a20 2020 2020 2020 2069 6478  "]:..        idx
-00006f50: 656e 6420 3d20 6964 7873 7461 7274 202b  end = idxstart +
-00006f60: 206d 0d0a 2020 2020 2020 2020 6964 7872   m..        idxr
-00006f70: 616e 6765 5b22 6122 5d20 3d20 6e70 2e61  ange["a"] = np.a
-00006f80: 7261 6e67 6528 6964 7873 7461 7274 2c20  range(idxstart, 
-00006f90: 6964 7865 6e64 290d 0a20 2020 2020 2020  idxend)..       
-00006fa0: 2069 6478 7374 6172 7420 3d20 6964 7865   idxstart = idxe
-00006fb0: 6e64 0d0a 2020 2020 2020 2020 705b 2261  nd..        p["a
-00006fc0: 225d 203d 206f 7574 2e78 5b69 6478 7261  "] = out.x[idxra
-00006fd0: 6e67 655b 2261 225d 5d0d 0a20 2020 2065  nge["a"]]..    e
-00006fe0: 6c73 653a 0d0a 2020 2020 2020 2020 6964  lse:..        id
-00006ff0: 7865 6e64 203d 2069 6478 7374 6172 7420  xend = idxstart 
-00007000: 2b20 6d20 2d20 310d 0a20 2020 2020 2020  + m - 1..       
-00007010: 2069 6478 7261 6e67 655b 2261 225d 203d   idxrange["a"] =
-00007020: 206e 702e 6172 616e 6765 2869 6478 7374   np.arange(idxst
-00007030: 6172 742c 2069 6478 656e 6429 0d0a 2020  art, idxend)..  
-00007040: 2020 2020 2020 6964 7873 7461 7274 203d        idxstart =
-00007050: 2069 6478 656e 640d 0a20 2020 2020 2020   idxend..       
-00007060: 2070 5b22 6122 5d20 3d20 6e70 2e63 6f6e   p["a"] = np.con
-00007070: 6361 7465 6e61 7465 2828 5b31 5d2c 206f  catenate(([1], o
-00007080: 7574 2e78 5b69 6478 7261 6e67 655b 2261  ut.x[idxrange["a
-00007090: 225d 5d29 2c20 6178 6973 3d30 290d 0a20  "]]), axis=0).. 
-000070a0: 2020 2070 6173 730d 0a0d 0a20 2020 2069     pass....    i
-000070b0: 6620 6967 6e6f 7265 5b22 6574 6122 5d20  f ignore["eta"] 
-000070c0: 6f72 2066 6978 5b22 6574 6122 5d3a 0d0a  or fix["eta"]:..
-000070d0: 2020 2020 2020 2020 705b 2265 7461 225d          p["eta"]
-000070e0: 203d 2070 6172 616d 5b22 6574 6130 225d   = param["eta0"]
-000070f0: 0d0a 2020 2020 656c 6966 2066 6978 5b22  ..    elif fix["
-00007100: 6d75 225d 3a0d 0a20 2020 2020 2020 2069  mu"]:..        i
-00007110: 6478 656e 6420 3d20 6964 7873 7461 7274  dxend = idxstart
-00007120: 202b 206d 0d0a 2020 2020 2020 2020 6964   + m..        id
-00007130: 7872 616e 6765 5b22 6574 6122 5d20 3d20  xrange["eta"] = 
-00007140: 6e70 2e61 7261 6e67 6528 6964 7873 7461  np.arange(idxsta
-00007150: 7274 2c20 6964 7865 6e64 290d 0a20 2020  rt, idxend)..   
-00007160: 2020 2020 2070 5b22 6574 6122 5d20 3d20       p["eta"] = 
-00007170: 6f75 742e 785b 6964 7872 616e 6765 5b22  out.x[idxrange["
-00007180: 6574 6122 5d5d 0d0a 2020 2020 656c 7365  eta"]]..    else
-00007190: 3a0d 0a20 2020 2020 2020 2069 6478 656e  :..        idxen
-000071a0: 6420 3d20 6964 7873 7461 7274 202b 206d  d = idxstart + m
-000071b0: 202d 2031 0d0a 2020 2020 2020 2020 6964   - 1..        id
-000071c0: 7872 616e 6765 5b22 6574 6122 5d20 3d20  xrange["eta"] = 
-000071d0: 6e70 2e61 7261 6e67 6528 6964 7873 7461  np.arange(idxsta
-000071e0: 7274 2c20 6964 7865 6e64 290d 0a20 2020  rt, idxend)..   
-000071f0: 2020 2020 2070 5b22 6574 6122 5d20 3d20       p["eta"] = 
-00007200: 6e70 2e63 6f6e 6361 7465 6e61 7465 2828  np.concatenate((
-00007210: 5b30 5d2c 206f 7574 2e78 5b69 6478 7261  [0], out.x[idxra
-00007220: 6e67 655b 2265 7461 225d 5d29 2c20 6178  nge["eta"]]), ax
-00007230: 6973 3d30 290d 0a20 2020 2070 6173 730d  is=0)..    pass.
-00007240: 0a0d 0a20 2020 2070 5b22 7473 225d 203d  ...    p["ts"] =
-00007250: 2070 6172 616d 5b22 7473 225d 0d0a 0d0a   param["ts"]....
-00007260: 2020 2020 7661 7279 5f70 6172 616d 203d      vary_param =
-00007270: 206e 702e 6c6f 6769 6361 6c5f 6e6f 7428   np.logical_not(
-00007280: 0d0a 2020 2020 2020 2020 5b0d 0a20 2020  ..        [..   
-00007290: 2020 2020 2020 2020 2066 6978 5b22 6c6f           fix["lo
-000072a0: 6776 225d 2c0d 0a20 2020 2020 2020 2020  gv"],..         
-000072b0: 2020 2066 6978 5b22 6d75 225d 2c0d 0a20     fix["mu"],.. 
-000072c0: 2020 2020 2020 2020 2020 2066 6978 5b22             fix["
-000072d0: 6122 5d20 6f72 2069 676e 6f72 655b 2261  a"] or ignore["a
-000072e0: 225d 2c0d 0a20 2020 2020 2020 2020 2020  "],..           
-000072f0: 2066 6978 5b22 6574 6122 5d20 6f72 2069   fix["eta"] or i
-00007300: 676e 6f72 655b 2265 7461 225d 0d0a 2020  gnore["eta"]..  
-00007310: 2020 2020 2020 5d0d 0a20 2020 2029 0d0a        ]..    )..
-00007320: 2020 2020 6469 6167 6e6f 7374 6963 203d      diagnostic =
-00007330: 207b 0d0a 2020 2020 2020 2020 2267 7261   {..        "gra
-00007340: 6422 3a20 6f75 742e 6a61 632c 0d0a 2020  d": out.jac,..  
-00007350: 2020 2020 2020 2268 6573 7369 616e 223a        "hessian":
-00007360: 2068 6573 732c 0d0a 2020 2020 2020 2020   hess,..        
-00007370: 2265 7272 223a 207b 2276 6172 223a 205b  "err": {"var": [
-00007380: 5d2c 2022 6d75 223a 205b 5d2c 2022 6122  ], "mu": [], "a"
-00007390: 3a20 5b5d 2c20 2265 7461 223a 205b 5d7d  : [], "eta": []}
-000073a0: 0d0a 2020 2020 7d0d 0a20 2020 2076 203d  ..    }..    v =
-000073b0: 206e 702e 646f 7428 6e70 2e65 7965 2868   np.dot(np.eye(h
-000073c0: 6573 732e 7368 6170 655b 305d 292c 2073  ess.shape[0]), s
-000073d0: 6369 7079 2e6c 696e 616c 672e 696e 7628  cipy.linalg.inv(
-000073e0: 6865 7373 2929 0d0a 2020 2020 6572 7220  hess))..    err 
-000073f0: 3d20 6e70 2e73 7172 7428 6e70 2e64 6961  = np.sqrt(np.dia
-00007400: 6728 7629 290d 0a20 2020 2069 6478 7374  g(v))..    idxst
-00007410: 6172 7420 3d20 300d 0a20 2020 2069 6620  art = 0..    if 
-00007420: 7661 7279 5f70 6172 616d 5b30 5d3a 0d0a  vary_param[0]:..
-00007430: 2020 2020 2020 2020 6469 6167 6e6f 7374          diagnost
-00007440: 6963 5b22 6572 7222 5d5b 2276 6172 225d  ic["err"]["var"]
-00007450: 203d 206e 702e 7371 7274 280d 0a20 2020   = np.sqrt(..   
-00007460: 2020 2020 2020 2020 206e 702e 6469 6167           np.diag
-00007470: 286e 702e 6469 6167 2870 5b22 7661 7222  (np.diag(p["var"
-00007480: 5d29 202a 2076 5b30 3a33 2c20 303a 335d  ]) * v[0:3, 0:3]
-00007490: 2920 2a20 6e70 2e64 6961 6728 705b 2276  ) * np.diag(p["v
-000074a0: 6172 225d 2929 0d0a 2020 2020 2020 2020  ar"]))..        
-000074b0: 6964 7873 7461 7274 203d 2069 6478 7374  idxstart = idxst
-000074c0: 6172 7420 2b20 330d 0a20 2020 2070 6173  art + 3..    pas
-000074d0: 730d 0a0d 0a20 2020 2069 6620 7661 7279  s....    if vary
-000074e0: 5f70 6172 616d 5b31 5d3a 0d0a 2020 2020  _param[1]:..    
-000074f0: 2020 2020 6469 6167 6e6f 7374 6963 5b22      diagnostic["
-00007500: 6572 7222 5d5b 226d 7522 5d20 3d20 6572  err"]["mu"] = er
-00007510: 725b 6964 7873 7461 7274 3a69 6478 7374  r[idxstart:idxst
-00007520: 6172 7420 2b20 6e5d 0d0a 2020 2020 2020  art + n]..      
-00007530: 2020 6964 7873 7461 7274 203d 2069 6478    idxstart = idx
-00007540: 7374 6172 7420 2b20 6e0d 0a20 2020 2070  start + n..    p
-00007550: 6173 730d 0a0d 0a20 2020 2069 6620 7661  ass....    if va
-00007560: 7279 5f70 6172 616d 5b32 5d3a 0d0a 2020  ry_param[2]:..  
-00007570: 2020 2020 2020 6966 2076 6172 795f 7061        if vary_pa
-00007580: 7261 6d5b 315d 3a0d 0a20 2020 2020 2020  ram[1]:..       
-00007590: 2020 2020 2064 6961 676e 6f73 7469 635b       diagnostic[
-000075a0: 2265 7272 225d 5b22 6122 5d20 3d20 6572  "err"]["a"] = er
-000075b0: 725b 6964 7873 7461 7274 3a69 6478 7374  r[idxstart:idxst
-000075c0: 6172 7420 2b20 6d20 2d20 315d 0d0a 2020  art + m - 1]..  
-000075d0: 2020 2020 2020 2020 2020 6964 7873 7461            idxsta
-000075e0: 7274 203d 2069 6478 7374 6172 7420 2b20  rt = idxstart + 
-000075f0: 6d20 2d20 310d 0a20 2020 2020 2020 2065  m - 1..        e
-00007600: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00007610: 2020 6469 6167 6e6f 7374 6963 5b22 6572    diagnostic["er
-00007620: 7222 5d5b 2261 225d 203d 2065 7272 5b69  r"]["a"] = err[i
-00007630: 6478 7374 6172 743a 6964 7873 7461 7274  dxstart:idxstart
-00007640: 202b 206d 5d0d 0a20 2020 2020 2020 2020   + m]..         
-00007650: 2020 2069 6478 7374 6172 7420 3d20 6964     idxstart = id
-00007660: 7873 7461 7274 202b 206d 0d0a 2020 2020  xstart + m..    
-00007670: 7061 7373 0d0a 0d0a 2020 2020 6966 2076  pass....    if v
-00007680: 6172 795f 7061 7261 6d5b 335d 3a0d 0a20  ary_param[3]:.. 
-00007690: 2020 2020 2020 2069 6620 7661 7279 5f70         if vary_p
-000076a0: 6172 616d 5b31 5d3a 0d0a 2020 2020 2020  aram[1]:..      
-000076b0: 2020 2020 2020 6469 6167 6e6f 7374 6963        diagnostic
-000076c0: 5b22 6572 7222 5d5b 2265 7461 225d 203d  ["err"]["eta"] =
-000076d0: 2065 7272 5b69 6478 7374 6172 743a 6964   err[idxstart:id
-000076e0: 7873 7461 7274 202b 206d 202d 2031 5d0d  xstart + m - 1].
-000076f0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00007700: 2020 2020 2020 2020 2020 2020 6469 6167              diag
-00007710: 6e6f 7374 6963 5b22 6572 7222 5d5b 2265  nostic["err"]["e
-00007720: 7461 225d 203d 2065 7272 5b69 6478 7374  ta"] = err[idxst
-00007730: 6172 743a 6964 7873 7461 7274 202b 206d  art:idxstart + m
-00007740: 5d0d 0a20 2020 2070 6173 730d 0a0d 0a20  ]..    pass.... 
-00007750: 2020 2072 6574 7572 6e20 5b70 2c20 6f75     return [p, ou
-00007760: 742e 6675 6e2c 2064 6961 676e 6f73 7469  t.fun, diagnosti
-00007770: 635d 0d0a                                c]..
+00000000: 696d 706f 7274 2077 6172 6e69 6e67 730a  import warnings.
+00000010: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000020: 7274 2043 616c 6c61 626c 652c 2054 7570  rt Callable, Tup
+00000030: 6c65 2c20 556e 696f 6e0a 0a69 6d70 6f72  le, Union..impor
+00000040: 7420 6e75 6d70 7920 6173 206e 700a 696d  t numpy as np.im
+00000050: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+00000060: 640a 696d 706f 7274 2073 6369 7079 2e6c  d.import scipy.l
+00000070: 696e 616c 6720 2023 2074 7970 653a 2069  inalg  # type: i
+00000080: 676e 6f72 650a 6672 6f6d 206e 756d 7079  gnore.from numpy
+00000090: 2e66 6674 2069 6d70 6f72 7420 6972 6666  .fft import irff
+000000a0: 742c 2072 6666 742c 2072 6666 7466 7265  t, rfft, rfftfre
+000000b0: 710a 6672 6f6d 206e 756d 7079 2e74 7970  q.from numpy.typ
+000000c0: 696e 6720 696d 706f 7274 2041 7272 6179  ing import Array
+000000d0: 4c69 6b65 0a66 726f 6d20 7363 6970 792e  Like.from scipy.
+000000e0: 6f70 7469 6d69 7a65 2069 6d70 6f72 7420  optimize import 
+000000f0: 6d69 6e69 6d69 7a65 2020 2320 7479 7065  minimize  # type
+00000100: 3a20 6967 6e6f 7265 0a0a 0a64 6566 2066  : ignore...def f
+00000110: 6674 6672 6571 286e 2c20 7429 3a0a 2020  ftfreq(n, t):.  
+00000120: 2020 2222 2243 6f6d 7075 7465 7320 7468    """Computes th
+00000130: 6520 706f 7369 7469 7665 2061 6e64 206e  e positive and n
+00000140: 6567 6174 6976 6520 6672 6571 7565 6e63  egative frequenc
+00000150: 6965 7320 7361 6d70 6c65 6420 696e 2074  ies sampled in t
+00000160: 6865 2046 6173 740a 2020 2020 466f 7572  he Fast.    Four
+00000170: 6965 7220 5472 616e 7366 6f72 6d2e 0a0a  ier Transform...
+00000180: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00000190: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000001a0: 2020 6e20 3a20 696e 740a 2020 2020 2020    n : int.      
+000001b0: 2020 4e75 6d62 6572 206f 6620 7469 6d65    Number of time
+000001c0: 2073 616d 706c 6573 0a20 2020 2074 3a20   samples.    t: 
+000001d0: 666c 6f61 740a 2020 2020 2020 2020 5361  float.        Sa
+000001e0: 6d70 6c69 6e67 2074 696d 650a 0a20 2020  mpling time..   
+000001f0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00000200: 2d2d 2d2d 0a20 2020 2066 203a 206e 6461  ----.    f : nda
+00000210: 7272 6179 0a20 2020 2020 2020 2046 7265  rray.        Fre
+00000220: 7175 656e 6379 2076 6563 746f 7220 2831  quency vector (1
+00000230: 2f74 7329 206f 6620 6c65 6e67 7468 206e  /ts) of length n
+00000240: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00000250: 7361 6d70 6c65 2066 7265 7175 656e 6369  sample frequenci
+00000260: 6573 2e0a 2020 2020 2222 220a 0a20 2020  es..    """..   
+00000270: 2069 6620 6e20 2520 3220 3d3d 2031 3a0a   if n % 2 == 1:.
+00000280: 2020 2020 2020 2020 6620 3d20 6e70 2e66          f = np.f
+00000290: 6674 2e66 6674 6672 6571 286e 2c20 7429  ft.fftfreq(n, t)
+000002a0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000002b0: 2020 2066 203d 206e 702e 6666 742e 6666     f = np.fft.ff
+000002c0: 7466 7265 7128 6e2c 2074 290a 2020 2020  tfreq(n, t).    
+000002d0: 2020 2020 665b 696e 7428 6e20 2f20 3229      f[int(n / 2)
+000002e0: 5d20 3d20 2d66 5b69 6e74 286e 202f 2032  ] = -f[int(n / 2
+000002f0: 295d 0a0a 2020 2020 7265 7475 726e 2066  )]..    return f
+00000300: 0a0a 0a64 6566 206e 6f69 7365 7661 7228  ...def noisevar(
+00000310: 7369 676d 613a 2041 7272 6179 4c69 6b65  sigma: ArrayLike
+00000320: 2c20 6d75 3a20 4172 7261 794c 696b 652c  , mu: ArrayLike,
+00000330: 2074 733a 2066 6c6f 6174 2920 2d3e 2041   ts: float) -> A
+00000340: 7272 6179 4c69 6b65 3a0a 2020 2020 7222  rrayLike:.    r"
+00000350: 2222 0a20 2020 2043 6f6d 7075 7465 2074  "".    Compute t
+00000360: 6865 2074 696d 652d 646f 6d61 696e 206e  he time-domain n
+00000370: 6f69 7365 2076 6172 6961 6e63 652e 0a0a  oise variance...
+00000380: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00000390: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000003a0: 2020 7369 676d 6120 3a20 6172 7261 795f    sigma : array_
+000003b0: 6c69 6b65 0a20 2020 2020 2020 204e 6f69  like.        Noi
+000003c0: 7365 2070 6172 616d 6574 6572 2061 7272  se parameter arr
+000003d0: 6179 2077 6974 6820 7368 6170 6520 2833  ay with shape (3
+000003e0: 2c20 292e 2054 6865 2066 6972 7374 2065  , ). The first e
+000003f0: 6c65 6d65 6e74 2063 6f72 7265 7370 6f6e  lement correspon
+00000400: 6473 0a20 2020 2020 2020 2074 6f20 7468  ds.        to th
+00000410: 6520 616d 706c 6974 7564 6520 6e6f 6973  e amplitude nois
+00000420: 652c 2069 6e20 7369 676e 616c 2075 6e69  e, in signal uni
+00000430: 7473 2028 6965 2c20 7468 6520 7361 6d65  ts (ie, the same
+00000440: 2075 6e69 7473 2061 7320 6d75 293b 0a20   units as mu);. 
+00000450: 2020 2020 2020 2074 6865 2073 6563 6f6e         the secon
+00000460: 6420 656c 656d 656e 7420 636f 7272 6573  d element corres
+00000470: 706f 6e64 7320 746f 206d 756c 7469 706c  ponds to multipl
+00000480: 6963 6174 6976 6520 6e6f 6973 652c 2077  icative noise, w
+00000490: 6869 6368 2069 730a 2020 2020 2020 2020  hich is.        
+000004a0: 6469 6d65 6e73 696f 6e6c 6573 733b 2061  dimensionless; a
+000004b0: 6e64 2074 6865 2074 6869 7264 2065 6c65  nd the third ele
+000004c0: 6d65 6e74 2063 6f72 7265 7370 6f6e 6473  ment corresponds
+000004d0: 2074 6f20 7469 6d65 6261 7365 206e 6f69   to timebase noi
+000004e0: 7365 2c20 696e 0a20 2020 2020 2020 2075  se, in.        u
+000004f0: 6e69 7473 206f 6620 7369 676e 616c 2f74  nits of signal/t
+00000500: 696d 652c 2077 6865 7265 2074 6865 2075  ime, where the u
+00000510: 6e69 7473 2066 6f72 2074 696d 6520 6172  nits for time ar
+00000520: 6520 7468 6520 7361 6d65 2061 7320 666f  e the same as fo
+00000530: 7220 742e 0a20 2020 206d 7520 3a20 2061  r t..    mu :  a
+00000540: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
+00000550: 2020 5469 6d65 2d64 6f6d 6169 6e20 7369    Time-domain si
+00000560: 676e 616c 2e0a 2020 2020 7473 203a 2066  gnal..    ts : f
+00000570: 6c6f 6174 0a20 2020 2020 2020 2053 616d  loat.        Sam
+00000580: 706c 696e 6720 7469 6d65 2e0a 0a20 2020  pling time...   
+00000590: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+000005a0: 2d2d 2d2d 0a20 2020 2076 6d75 203a 206e  ----.    vmu : n
+000005b0: 6461 7272 6179 0a20 2020 2020 2020 2054  darray.        T
+000005c0: 696d 652d 646f 6d61 696e 206e 6f69 7365  ime-domain noise
+000005d0: 2076 6172 6961 6e63 652e 0a20 2020 2022   variance..    "
+000005e0: 2222 0a20 2020 2073 6967 6d61 203d 206e  "".    sigma = n
+000005f0: 702e 6173 6172 7261 7928 7369 676d 6129  p.asarray(sigma)
+00000600: 0a20 2020 206d 7520 3d20 6e70 2e61 7361  .    mu = np.asa
+00000610: 7272 6179 286d 7529 0a0a 2020 2020 6e20  rray(mu)..    n 
+00000620: 3d20 6d75 2e73 6861 7065 5b30 5d0a 2020  = mu.shape[0].  
+00000630: 2020 7720 3d20 3220 2a20 6e70 2e70 6920    w = 2 * np.pi 
+00000640: 2a20 7266 6674 6672 6571 286e 2c20 7473  * rfftfreq(n, ts
+00000650: 290a 2020 2020 6d75 646f 7420 3d20 6972  ).    mudot = ir
+00000660: 6666 7428 316a 202a 2077 202a 2072 6666  fft(1j * w * rff
+00000670: 7428 6d75 292c 206e 3d6e 290a 0a20 2020  t(mu), n=n)..   
+00000680: 2072 6574 7572 6e20 7369 676d 615b 305d   return sigma[0]
+00000690: 202a 2a20 3220 2b20 2873 6967 6d61 5b31   ** 2 + (sigma[1
+000006a0: 5d20 2a20 6d75 2920 2a2a 2032 202b 2028  ] * mu) ** 2 + (
+000006b0: 7369 676d 615b 325d 202a 206d 7564 6f74  sigma[2] * mudot
+000006c0: 2920 2a2a 2032 0a0a 0a64 6566 206e 6f69  ) ** 2...def noi
+000006d0: 7365 616d 7028 7369 676d 613a 2041 7272  seamp(sigma: Arr
+000006e0: 6179 4c69 6b65 2c20 6d75 3a20 4172 7261  ayLike, mu: Arra
+000006f0: 794c 696b 652c 2074 733a 2066 6c6f 6174  yLike, ts: float
+00000700: 2920 2d3e 2041 7272 6179 4c69 6b65 3a0a  ) -> ArrayLike:.
+00000710: 2020 2020 7222 2222 0a20 2020 2043 6f6d      r""".    Com
+00000720: 7075 7465 2074 6865 2074 696d 652d 646f  pute the time-do
+00000730: 6d61 696e 206e 6f69 7365 2061 6d70 6c69  main noise ampli
+00000740: 7475 6465 2e0a 0a20 2020 2050 6172 616d  tude...    Param
+00000750: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00000760: 2d2d 2d2d 0a20 2020 2073 6967 6d61 203a  ----.    sigma :
+00000770: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+00000780: 2020 2020 4e6f 6973 6520 7061 7261 6d65      Noise parame
+00000790: 7465 7220 6172 7261 7920 7769 7468 2073  ter array with s
+000007a0: 6861 7065 2028 332c 2029 2e20 5468 6520  hape (3, ). The 
+000007b0: 6669 7273 7420 656c 656d 656e 7420 636f  first element co
+000007c0: 7272 6573 706f 6e64 730a 2020 2020 2020  rresponds.      
+000007d0: 2020 746f 2074 6865 2061 6d70 6c69 7475    to the amplitu
+000007e0: 6465 206e 6f69 7365 2c20 696e 2073 6967  de noise, in sig
+000007f0: 6e61 6c20 756e 6974 7320 2869 652c 2074  nal units (ie, t
+00000800: 6865 2073 616d 6520 756e 6974 7320 6173  he same units as
+00000810: 206d 7529 3b0a 2020 2020 2020 2020 7468   mu);.        th
+00000820: 6520 7365 636f 6e64 2065 6c65 6d65 6e74  e second element
+00000830: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+00000840: 6d75 6c74 6970 6c69 6361 7469 7665 206e  multiplicative n
+00000850: 6f69 7365 2c20 7768 6963 6820 6973 0a20  oise, which is. 
+00000860: 2020 2020 2020 2064 696d 656e 7369 6f6e         dimension
+00000870: 6c65 7373 3b20 616e 6420 7468 6520 7468  less; and the th
+00000880: 6972 6420 656c 656d 656e 7420 636f 7272  ird element corr
+00000890: 6573 706f 6e64 7320 746f 2074 696d 6562  esponds to timeb
+000008a0: 6173 6520 6e6f 6973 652c 2069 6e0a 2020  ase noise, in.  
+000008b0: 2020 2020 2020 756e 6974 7320 6f66 2073        units of s
+000008c0: 6967 6e61 6c2f 7469 6d65 2c20 7768 6572  ignal/time, wher
+000008d0: 6520 7468 6520 756e 6974 7320 666f 7220  e the units for 
+000008e0: 7469 6d65 2061 7265 2074 6865 2073 616d  time are the sam
+000008f0: 6520 6173 2066 6f72 2074 2e0a 2020 2020  e as for t..    
+00000900: 6d75 203a 2020 6172 7261 795f 6c69 6b65  mu :  array_like
+00000910: 0a20 2020 2020 2020 2054 696d 652d 646f  .        Time-do
+00000920: 6d61 696e 2073 6967 6e61 6c2e 0a20 2020  main signal..   
+00000930: 2074 7320 3a20 666c 6f61 740a 2020 2020   ts : float.    
+00000940: 2020 2020 5361 6d70 6c69 6e67 2074 696d      Sampling tim
+00000950: 652e 0a0a 2020 2020 5265 7475 726e 730a  e...    Returns.
+00000960: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00000970: 7369 676d 616d 7520 3a20 6e64 6172 7261  sigmamu : ndarra
+00000980: 790a 2020 2020 2020 2020 5469 6d65 2d64  y.        Time-d
+00000990: 6f6d 6169 6e20 6e6f 6973 6520 616d 706c  omain noise ampl
+000009a0: 6974 7564 652c 2069 6e20 7369 676e 616c  itude, in signal
+000009b0: 2075 6e69 7473 2e0a 0a20 2020 2022 2222   units...    """
+000009c0: 0a0a 2020 2020 7265 7475 726e 206e 702e  ..    return np.
+000009d0: 7371 7274 286e 6f69 7365 7661 7228 7369  sqrt(noisevar(si
+000009e0: 676d 612c 206d 752c 2074 7329 290a 0a0a  gma, mu, ts))...
+000009f0: 6465 6620 7468 7a67 656e 286e 3a20 696e  def thzgen(n: in
+00000a00: 742c 2074 733a 2066 6c6f 6174 2c20 7430  t, ts: float, t0
+00000a10: 3a20 666c 6f61 742c 2061 3a20 666c 6f61  : float, a: floa
+00000a20: 7420 3d20 312e 302c 2074 6175 723a 2066  t = 1.0, taur: f
+00000a30: 6c6f 6174 203d 2030 2e33 2c0a 2020 2020  loat = 0.3,.    
+00000a40: 2020 2020 2020 2074 6175 633a 2066 6c6f         tauc: flo
+00000a50: 6174 203d 2030 2e31 2c20 6677 686d 3a20  at = 0.1, fwhm: 
+00000a60: 666c 6f61 7420 3d20 302e 3035 0a20 2020  float = 0.05.   
+00000a70: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
+00000a80: 6c65 5b41 7272 6179 4c69 6b65 2c20 4172  le[ArrayLike, Ar
+00000a90: 7261 794c 696b 655d 3a0a 2020 2020 7222  rayLike]:.    r"
+00000aa0: 2222 5369 6d75 6c61 7465 2061 2074 6572  ""Simulate a ter
+00000ab0: 6168 6572 747a 2070 756c 7365 2e0a 0a20  ahertz pulse... 
+00000ac0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00000ad0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020    ----------..  
+00000ae0: 2020 6e20 3a20 696e 740a 2020 2020 2020    n : int.      
+00000af0: 2020 4e75 6d62 6572 206f 6620 7361 6d70    Number of samp
+00000b00: 6c65 732e 0a0a 2020 2020 7473 203a 2066  les...    ts : f
+00000b10: 6c6f 6174 0a20 2020 2020 2020 2053 616d  loat.        Sam
+00000b20: 706c 696e 6720 7469 6d65 2e0a 0a20 2020  pling time...   
+00000b30: 2074 3020 3a20 666c 6f61 740a 2020 2020   t0 : float.    
+00000b40: 2020 2020 5075 6c73 6520 6365 6e74 6572      Pulse center
+00000b50: 2e0a 0a20 2020 2061 203a 2066 6c6f 6174  ...    a : float
+00000b60: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00000b70: 2020 2050 6561 6b20 616d 706c 6974 7564     Peak amplitud
+00000b80: 652e 0a0a 2020 2020 7461 7572 203a 2066  e...    taur : f
+00000b90: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
+00000ba0: 2020 2020 2020 2043 7572 7265 6e74 2070         Current p
+00000bb0: 756c 7365 2072 6973 6520 7469 6d65 2e0a  ulse rise time..
+00000bc0: 0a20 2020 2074 6175 6320 3a20 666c 6f61  .    tauc : floa
+00000bd0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+00000be0: 2020 2020 4375 7272 656e 7420 7075 6c73      Current puls
+00000bf0: 6520 6465 6361 7920 7469 6d65 2e0a 0a20  e decay time... 
+00000c00: 2020 2066 7768 6d20 3a20 666c 6f61 742c     fwhm : float,
+00000c10: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00000c20: 2020 4c61 7365 7220 7075 6c73 6520 4657    Laser pulse FW
+00000c30: 484d 2e0a 0a20 2020 2052 6574 7572 6e73  HM...    Returns
+00000c40: 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a 2020  .    -------..  
+00000c50: 2020 7920 3a20 6e64 6172 7261 790a 2020    y : ndarray.  
+00000c60: 2020 2020 2020 7369 676e 616c 2028 752e        signal (u.
+00000c70: 6129 0a0a 2020 2020 7420 3a20 6e64 6172  a)..    t : ndar
+00000c80: 7261 790a 2020 2020 2020 2020 7469 6d65  ray.        time
+00000c90: 6261 7365 0a0a 2020 2020 2222 220a 0a20  base..    """.. 
+00000ca0: 2020 2074 6175 6c20 3d20 6677 686d 202f     taul = fwhm /
+00000cb0: 206e 702e 7371 7274 2832 202a 206e 702e   np.sqrt(2 * np.
+00000cc0: 6c6f 6728 3229 290a 0a20 2020 2066 203d  log(2))..    f =
+00000cd0: 2072 6666 7466 7265 7128 6e2c 2074 7329   rfftfreq(n, ts)
+00000ce0: 0a0a 2020 2020 7720 3d20 3220 2a20 6e70  ..    w = 2 * np
+00000cf0: 2e70 6920 2a20 660a 2020 2020 656c 6c20  .pi * f.    ell 
+00000d00: 3d20 6e70 2e65 7870 282d 2828 7720 2a20  = np.exp(-((w * 
+00000d10: 7461 756c 2920 2a2a 2032 2920 2f20 3229  taul) ** 2) / 2)
+00000d20: 202f 206e 702e 7371 7274 2832 202a 206e   / np.sqrt(2 * n
+00000d30: 702e 7069 202a 2074 6175 6c20 2a2a 2032  p.pi * taul ** 2
+00000d40: 290a 2020 2020 7220 3d20 3120 2f20 2831  ).    r = 1 / (1
+00000d50: 202f 2074 6175 7220 2d20 316a 202a 2077   / taur - 1j * w
+00000d60: 2920 2d20 3120 2f20 2831 202f 2074 6175  ) - 1 / (1 / tau
+00000d70: 7220 2b20 3120 2f20 7461 7563 202d 2031  r + 1 / tauc - 1
+00000d80: 6a20 2a20 7729 0a20 2020 2073 203d 202d  j * w).    s = -
+00000d90: 316a 202a 2077 202a 2028 656c 6c20 2a20  1j * w * (ell * 
+00000da0: 7229 202a 2a20 3220 2a20 6e70 2e65 7870  r) ** 2 * np.exp
+00000db0: 2831 6a20 2a20 7720 2a20 7430 290a 0a20  (1j * w * t0).. 
+00000dc0: 2020 2074 3220 3d20 7473 202a 206e 702e     t2 = ts * np.
+00000dd0: 6172 616e 6765 286e 290a 0a20 2020 2079  arange(n)..    y
+00000de0: 203d 2069 7266 6674 286e 702e 636f 6e6a   = irfft(np.conj
+00000df0: 2873 292c 206e 3d6e 290a 2020 2020 7920  (s), n=n).    y 
+00000e00: 3d20 6120 2a20 7920 2f20 6e70 2e6d 6178  = a * y / np.max
+00000e10: 2879 290a 0a20 2020 2072 6574 7572 6e20  (y)..    return 
+00000e20: 792c 2074 320a 0a0a 636c 6173 7320 4461  y, t2...class Da
+00000e30: 7461 5075 6c73 653a 0a20 2020 2064 6566  taPulse:.    def
+00000e40: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00000e50: 6669 6c65 6e61 6d65 3d22 2229 3a0a 2020  filename=""):.  
+00000e60: 2020 2020 2020 7365 6c66 2e41 6371 7569        self.Acqui
+00000e70: 7369 7469 6f6e 5469 6d65 203d 204e 6f6e  sitionTime = Non
+00000e80: 650a 2020 2020 2020 2020 7365 6c66 2e44  e.        self.D
+00000e90: 6573 6372 6970 7469 6f6e 203d 204e 6f6e  escription = Non
+00000ea0: 650a 2020 2020 2020 2020 7365 6c66 2e54  e.        self.T
+00000eb0: 696d 6543 6f6e 7374 616e 7420 3d20 4e6f  imeConstant = No
+00000ec0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00000ed0: 5761 6974 5469 6d65 203d 204e 6f6e 650a  WaitTime = None.
+00000ee0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00000ef0: 506f 696e 7420 3d20 4e6f 6e65 0a20 2020  Point = None.   
+00000f00: 2020 2020 2073 656c 662e 7363 616e 4f66       self.scanOf
+00000f10: 6673 6574 203d 204e 6f6e 650a 2020 2020  fset = None.    
+00000f20: 2020 2020 7365 6c66 2e74 656d 7065 7261      self.tempera
+00000f30: 7475 7265 203d 204e 6f6e 650a 2020 2020  ture = None.    
+00000f40: 2020 2020 7365 6c66 2e74 696d 6520 3d20      self.time = 
+00000f50: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00000f60: 662e 616d 706c 6974 7564 6520 3d20 4e6f  f.amplitude = No
+00000f70: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00000f80: 4368 616e 6e65 6c41 4d61 7869 6d75 6d20  ChannelAMaximum 
+00000f90: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00000fa0: 656c 662e 4368 616e 6e65 6c41 4d69 6e69  elf.ChannelAMini
+00000fb0: 6d75 6d20 3d20 4e6f 6e65 0a20 2020 2020  mum = None.     
+00000fc0: 2020 2073 656c 662e 4368 616e 6e65 6c41     self.ChannelA
+00000fd0: 5661 7269 616e 6365 203d 204e 6f6e 650a  Variance = None.
+00000fe0: 2020 2020 2020 2020 7365 6c66 2e43 6861          self.Cha
+00000ff0: 6e6e 656c 4153 6c6f 7065 203d 204e 6f6e  nnelASlope = Non
+00001000: 650a 2020 2020 2020 2020 7365 6c66 2e43  e.        self.C
+00001010: 6861 6e6e 656c 414f 6666 7365 7420 3d20  hannelAOffset = 
+00001020: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00001030: 662e 4368 616e 6e65 6c42 4d61 7869 6d75  f.ChannelBMaximu
+00001040: 6d20 3d20 4e6f 6e65 0a20 2020 2020 2020  m = None.       
+00001050: 2073 656c 662e 4368 616e 6e65 6c42 4d69   self.ChannelBMi
+00001060: 6e69 6d75 6d20 3d20 4e6f 6e65 0a20 2020  nimum = None.   
+00001070: 2020 2020 2073 656c 662e 4368 616e 6e65       self.Channe
+00001080: 6c42 5661 7269 616e 6365 203d 204e 6f6e  lBVariance = Non
+00001090: 650a 2020 2020 2020 2020 7365 6c66 2e43  e.        self.C
+000010a0: 6861 6e6e 656c 4253 6c6f 7065 203d 204e  hannelBSlope = N
+000010b0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+000010c0: 2e43 6861 6e6e 656c 424f 6666 7365 7420  .ChannelBOffset 
+000010d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+000010e0: 656c 662e 4368 616e 6e65 6c43 4d61 7869  elf.ChannelCMaxi
+000010f0: 6d75 6d20 3d20 4e6f 6e65 0a20 2020 2020  mum = None.     
+00001100: 2020 2073 656c 662e 4368 616e 6e65 6c43     self.ChannelC
+00001110: 4d69 6e69 6d75 6d20 3d20 4e6f 6e65 0a20  Minimum = None. 
+00001120: 2020 2020 2020 2073 656c 662e 4368 616e         self.Chan
+00001130: 6e65 6c43 5661 7269 616e 6365 203d 204e  nelCVariance = N
+00001140: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00001150: 2e43 6861 6e6e 656c 4353 6c6f 7065 203d  .ChannelCSlope =
+00001160: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00001170: 6c66 2e43 6861 6e6e 656c 434f 6666 7365  lf.ChannelCOffse
+00001180: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
+00001190: 2073 656c 662e 4368 616e 6e65 6c44 4d61   self.ChannelDMa
+000011a0: 7869 6d75 6d20 3d20 4e6f 6e65 0a20 2020  ximum = None.   
+000011b0: 2020 2020 2073 656c 662e 4368 616e 6e65       self.Channe
+000011c0: 6c44 4d69 6e69 6d75 6d20 3d20 4e6f 6e65  lDMinimum = None
+000011d0: 0a20 2020 2020 2020 2073 656c 662e 4368  .        self.Ch
+000011e0: 616e 6e65 6c44 5661 7269 616e 6365 203d  annelDVariance =
+000011f0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00001200: 6c66 2e43 6861 6e6e 656c 4453 6c6f 7065  lf.ChannelDSlope
+00001210: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00001220: 7365 6c66 2e43 6861 6e6e 656c 444f 6666  self.ChannelDOff
+00001230: 7365 7420 3d20 4e6f 6e65 0a20 2020 2020  set = None.     
+00001240: 2020 2073 656c 662e 6469 726e 616d 6520     self.dirname 
+00001250: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00001260: 656c 662e 6669 6c65 203d 204e 6f6e 650a  elf.file = None.
+00001270: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00001280: 656e 616d 6520 3d20 6669 6c65 6e61 6d65  ename = filename
+00001290: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
+000012a0: 6571 7565 6e63 7920 3d20 4e6f 6e65 0a0a  equency = None..
+000012b0: 2020 2020 2020 2020 6966 2066 696c 656e          if filen
+000012c0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000012d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000012e0: 6120 3d20 7064 2e72 6561 645f 6373 7628  a = pd.read_csv(
+000012f0: 6669 6c65 6e61 6d65 2c20 6865 6164 6572  filename, header
+00001300: 3d4e 6f6e 652c 2064 656c 696d 6974 6572  =None, delimiter
+00001310: 3d22 5c74 2229 0a0a 2020 2020 2020 2020  ="\t")..        
+00001320: 2020 2020 696e 6420 3d20 300a 2020 2020      ind = 0.    
+00001330: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00001340: 2072 616e 6765 2864 6174 612e 7368 6170   range(data.shap
+00001350: 655b 305d 293a 0a20 2020 2020 2020 2020  e[0]):.         
+00001360: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 666c 6f61 7428 6461 7461 5b30 5d5b 695d  float(data[0][i]
+00001390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000013a0: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+000013b0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+000013c0: 2020 2020 2020 2020 2069 6e64 203d 2069           ind = i
+000013d0: 202b 2031 0a20 2020 2020 2020 2020 2020   + 1.           
+000013e0: 2020 2020 2070 6173 730a 0a20 2020 2020       pass..     
+000013f0: 2020 2020 2020 206b 6579 7320 3d20 6461         keys = da
+00001400: 7461 5b30 5d5b 303a 696e 645d 2e74 6f5f  ta[0][0:ind].to_
+00001410: 6c69 7374 2829 0a20 2020 2020 2020 2020  list().         
+00001420: 2020 2076 616c 7320 3d20 6461 7461 5b31     vals = data[1
+00001430: 5d5b 303a 696e 645d 2e74 6f5f 6c69 7374  ][0:ind].to_list
+00001440: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00001450: 666f 7220 6b20 696e 2072 616e 6765 286c  for k in range(l
+00001460: 656e 286b 6579 7329 293a 0a20 2020 2020  en(keys)):.     
+00001470: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+00001480: 7973 5b6b 5d20 696e 206c 6973 7428 7365  ys[k] in list(se
+00001490: 6c66 2e5f 5f64 6963 745f 5f2e 6b65 7973  lf.__dict__.keys
+000014a0: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+000014b0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2020 2020 2020 666c 6f61 7428 7661 6c73        float(vals
+000014e0: 5b6b 5d29 0a20 2020 2020 2020 2020 2020  [k]).           
+000014f0: 2020 2020 2020 2020 2020 2020 2073 6574               set
+00001500: 6174 7472 2873 656c 662c 206b 6579 735b  attr(self, keys[
+00001510: 6b5d 2c20 666c 6f61 7428 7661 6c73 5b6b  k], float(vals[k
+00001520: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+00001530: 2020 2020 2020 2020 6578 6365 7074 2056          except V
+00001540: 616c 7565 4572 726f 723a 0a20 2020 2020  alueError:.     
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 2073 6574 6174 7472 2873 656c 662c     setattr(self,
+00001570: 206b 6579 735b 6b5d 2c20 7661 6c73 5b6b   keys[k], vals[k
+00001580: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+00001590: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000015a0: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+000015b0: 6720 3d20 2254 6865 2064 6174 6120 6b65  g = "The data ke
+000015c0: 7920 6973 206e 6f74 2064 6566 6965 6422  y is not defied"
+000015d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000015e0: 2020 2020 2072 6169 7365 2057 6172 6e69       raise Warni
+000015f0: 6e67 286d 7367 290a 0a20 2020 2020 2020  ng(msg)..       
+00001600: 2020 2020 2073 656c 662e 7469 6d65 203d       self.time =
+00001610: 2064 6174 615b 305d 5b69 6e64 3a5d 2e74   data[0][ind:].t
+00001620: 6f5f 6e75 6d70 7928 6474 7970 653d 666c  o_numpy(dtype=fl
+00001630: 6f61 7429 0a20 2020 2020 2020 2020 2020  oat).           
+00001640: 2073 656c 662e 616d 706c 6974 7564 6520   self.amplitude 
+00001650: 3d20 6461 7461 5b31 5d5b 696e 643a 5d2e  = data[1][ind:].
+00001660: 746f 5f6e 756d 7079 2864 7479 7065 3d66  to_numpy(dtype=f
+00001670: 6c6f 6174 290a 0a20 2020 2020 2020 2020  loat)..         
+00001680: 2020 2023 2043 616c 6375 6c61 7465 2066     # Calculate f
+00001690: 7265 7175 656e 6379 2072 616e 6765 0a20  requency range. 
+000016a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000016b0: 6672 6571 7565 6e63 7920 3d20 280a 2020  frequency = (.  
+000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 2020 206e 702e 6172 616e 6765 280a 2020     np.arange(.  
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2020 2020 2020 206e 702e 666c 6f6f 7228         np.floor(
+00001720: 6c65 6e28 7365 6c66 2e74 696d 6529 2929  len(self.time)))
+00001730: 202f 2032 202d 2031 0a20 2020 2020 2020   / 2 - 1.       
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 2020 2020 2020 292e 5420 2f20 2873 656c        ).T / (sel
+00001760: 662e 7469 6d65 5b2d 315d 202d 2073 656c  f.time[-1] - sel
+00001770: 662e 7469 6d65 5b30 5d29 0a0a 2020 2020  f.time[0])..    
+00001780: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
+00001790: 6174 6520 6666 740a 2020 2020 2020 2020  ate fft.        
+000017a0: 2020 2020 6661 6d70 203d 206e 702e 6666      famp = np.ff
+000017b0: 742e 6666 7428 7365 6c66 2e61 6d70 6c69  t.fft(self.ampli
+000017c0: 7475 6465 290a 2020 2020 2020 2020 2020  tude).          
+000017d0: 2020 7365 6c66 2e66 616d 7020 3d20 6661    self.famp = fa
+000017e0: 6d70 5b30 3a20 696e 7428 6e70 2e66 6c6f  mp[0: int(np.flo
+000017f0: 6f72 286c 656e 2866 616d 7029 202f 2032  or(len(famp) / 2
+00001800: 2929 5d0a 0a0a 6465 6620 7368 6966 746d  ))]...def shiftm
+00001810: 7478 2874 6175 3a20 666c 6f61 742c 206e  tx(tau: float, n
+00001820: 3a20 696e 742c 2074 733a 2066 6c6f 6174  : int, ts: float
+00001830: 203d 2031 2920 2d3e 2041 7272 6179 4c69   = 1) -> ArrayLi
+00001840: 6b65 3a0a 2020 2020 2222 220a 2020 2020  ke:.    """.    
+00001850: 5368 6966 746d 7478 2063 6f6d 7075 7465  Shiftmtx compute
+00001860: 7320 7468 6520 6e20 6279 206e 2074 7261  s the n by n tra
+00001870: 6e73 6665 7220 6d61 7472 6978 2066 6f72  nsfer matrix for
+00001880: 2061 2063 6f6e 7469 6e75 6f75 7320 7469   a continuous ti
+00001890: 6d65 2d73 6869 6674 2e0a 0a20 2020 2050  me-shift...    P
+000018a0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+000018b0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020 2074  ---------..    t
+000018c0: 6175 203a 2066 6c6f 6174 0a20 2020 2020  au : float.     
+000018d0: 2020 2044 656c 6179 2e0a 0a20 2020 206e     Delay...    n
+000018e0: 203a 2069 6e74 0a20 2020 2020 2020 204e   : int.        N
+000018f0: 756d 6265 7220 6f66 2073 616d 706c 6573  umber of samples
+00001900: 2e0a 0a20 2020 2074 733a 2066 6c6f 6174  ...    ts: float
+00001910: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00001920: 2020 2053 616d 706c 696e 6720 7469 6d65     Sampling time
+00001930: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00001940: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2068     -------.    h
+00001950: 3a20 6e64 6172 7261 790a 2020 2020 2020  : ndarray.      
+00001960: 2020 5472 616e 7366 6572 206d 6174 7269    Transfer matri
+00001970: 7820 7769 7468 2073 6861 7065 2028 6e2c  x with shape (n,
+00001980: 206e 292e 0a0a 2020 2020 2222 220a 0a20   n)...    """.. 
+00001990: 2020 2023 2046 6f75 7269 6572 206d 6574     # Fourier met
+000019a0: 686f 640a 2020 2020 6620 3d20 7266 6674  hod.    f = rfft
+000019b0: 6672 6571 286e 2c20 7473 290a 2020 2020  freq(n, ts).    
+000019c0: 7720 3d20 3220 2a20 6e70 2e70 6920 2a20  w = 2 * np.pi * 
+000019d0: 660a 0a20 2020 2069 6d70 203d 2069 7266  f..    imp = irf
+000019e0: 6674 286e 702e 6578 7028 2d31 6a20 2a20  ft(np.exp(-1j * 
+000019f0: 7720 2a20 7461 7529 2c20 6e3d 6e29 0a0a  w * tau), n=n)..
+00001a00: 2020 2020 2320 636f 6d70 7574 6573 2074      # computes t
+00001a10: 6865 206e 2062 7920 6e20 7472 616e 7366  he n by n transf
+00001a20: 6f72 6d61 7469 6f6e 206d 6174 7269 780a  ormation matrix.
+00001a30: 2020 2020 6820 3d20 7363 6970 792e 6c69      h = scipy.li
+00001a40: 6e61 6c67 2e74 6f65 706c 6974 7a28 696d  nalg.toeplitz(im
+00001a50: 702c 206e 702e 726f 6c6c 286e 702e 666c  p, np.roll(np.fl
+00001a60: 6970 7564 2869 6d70 292c 2031 2929 0a0a  ipud(imp), 1))..
+00001a70: 2020 2020 7265 7475 726e 2068 0a0a 0a64      return h...d
+00001a80: 6566 2061 6972 7363 616e 636f 7272 6563  ef airscancorrec
+00001a90: 7428 783a 2041 7272 6179 4c69 6b65 2c20  t(x: ArrayLike, 
+00001aa0: 2a2c 2061 3a20 556e 696f 6e5b 4172 7261  *, a: Union[Arra
+00001ab0: 794c 696b 652c 204e 6f6e 655d 203d 204e  yLike, None] = N
+00001ac0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001ad0: 2020 2020 2020 2020 6574 613a 2055 6e69          eta: Uni
+00001ae0: 6f6e 5b41 7272 6179 4c69 6b65 2c20 4e6f  on[ArrayLike, No
+00001af0: 6e65 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ne] = None,.    
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001b10: 733a 2066 6c6f 6174 203d 2031 2e30 2920  s: float = 1.0) 
+00001b20: 2d3e 2041 7272 6179 4c69 6b65 3a0a 2020  -> ArrayLike:.  
+00001b30: 2020 2222 2252 6573 6361 6c65 7320 616e    """Rescales an
+00001b40: 6420 7368 6966 7473 2065 6163 6820 636f  d shifts each co
+00001b50: 6c75 6d6e 206f 6620 7468 6520 6d61 7472  lumn of the matr
+00001b60: 6978 2078 2e0a 0a20 2020 2050 6172 616d  ix x...    Param
+00001b70: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00001b80: 2d2d 2d2d 0a20 2020 2078 203a 2061 7272  ----.    x : arr
+00001b90: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+00001ba0: 4461 7461 2061 7272 6179 2077 6974 6820  Data array with 
+00001bb0: 7368 6170 6520 286e 2c20 6d29 2e0a 2020  shape (n, m)..  
+00001bc0: 2020 6120 3a20 6172 7261 795f 6c69 6b65    a : array_like
+00001bd0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00001be0: 2020 2041 6d70 6c69 7475 6465 2063 6f72     Amplitude cor
+00001bf0: 7265 6374 696f 6e2e 2049 6620 7365 742c  rection. If set,
+00001c00: 2061 206d 7573 7420 6861 7665 2073 6861   a must have sha
+00001c10: 7065 2028 6d2c 292e 204f 7468 6572 7769  pe (m,). Otherwi
+00001c20: 7365 2c20 6e6f 0a20 2020 2020 2020 2063  se, no.        c
+00001c30: 6f72 7265 6374 696f 6e20 6973 2061 7070  orrection is app
+00001c40: 6c69 6564 2e0a 2020 2020 6574 6120 3a20  lied..    eta : 
+00001c50: 6172 7261 795f 6c69 6b65 2c20 6f70 7469  array_like, opti
+00001c60: 6f6e 616c 0a20 2020 2020 2020 2044 656c  onal.        Del
+00001c70: 6179 2063 6f72 7265 6374 696f 6e2e 2049  ay correction. I
+00001c80: 6620 7365 742c 2061 206d 7573 7420 6861  f set, a must ha
+00001c90: 7665 2073 6861 7065 2028 6d2c 292e 204f  ve shape (m,). O
+00001ca0: 7468 6572 7769 7365 2c20 6e6f 0a20 2020  therwise, no.   
+00001cb0: 2020 2020 2063 6f72 7265 6374 696f 6e20       correction 
+00001cc0: 6973 2061 7070 6c69 6564 2e0a 2020 2020  is applied..    
+00001cd0: 7473 203a 2066 6c6f 6174 2c20 6f70 7469  ts : float, opti
+00001ce0: 6f6e 616c 0a20 2020 2020 2020 2053 616d  onal.        Sam
+00001cf0: 706c 696e 6720 7469 6d65 2e20 4465 6661  pling time. Defa
+00001d00: 756c 7420 6973 2031 2e30 2e0a 0a20 2020  ult is 1.0...   
+00001d10: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00001d20: 2d2d 2d2d 0a20 2020 2078 6164 6a20 3a20  ----.    xadj : 
+00001d30: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+00001d40: 4164 6a75 7374 6564 2064 6174 6120 6172  Adjusted data ar
+00001d50: 7261 792e 0a0a 2020 2020 2222 220a 2020  ray...    """.  
+00001d60: 2020 7820 3d20 6e70 2e61 7361 7272 6179    x = np.asarray
+00001d70: 2878 290a 0a20 2020 205b 6e2c 206d 5d20  (x)..    [n, m] 
+00001d80: 3d20 782e 7368 6170 650a 0a20 2020 2069  = x.shape..    i
+00001d90: 6620 6120 6973 204e 6f6e 653a 0a20 2020  f a is None:.   
+00001da0: 2020 2020 2061 203d 206e 702e 6f6e 6573       a = np.ones
+00001db0: 2828 6d2c 2029 290a 2020 2020 656c 7365  ((m, )).    else
+00001dc0: 3a0a 2020 2020 2020 2020 6120 3d20 6e70  :.        a = np
+00001dd0: 2e61 7361 7272 6179 2861 290a 0a20 2020  .asarray(a)..   
+00001de0: 2069 6620 6574 6120 6973 204e 6f6e 653a   if eta is None:
+00001df0: 0a20 2020 2020 2020 2065 7461 203d 206e  .        eta = n
+00001e00: 702e 7a65 726f 7328 286d 2c20 2929 0a20  p.zeros((m, )). 
+00001e10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00001e20: 2065 7461 203d 206e 702e 6173 6172 7261   eta = np.asarra
+00001e30: 7928 6574 6129 0a0a 2020 2020 7861 646a  y(eta)..    xadj
+00001e40: 203d 206e 702e 7a65 726f 7328 286e 2c20   = np.zeros((n, 
+00001e50: 6d29 290a 2020 2020 2320 544f 444f 3a20  m)).    # TODO: 
+00001e60: 7265 6661 6374 6f72 2077 6974 6820 6272  refactor with br
+00001e70: 6f61 6463 6173 7469 6e67 0a20 2020 2066  oadcasting.    f
+00001e80: 6f72 2069 2069 6e20 6e70 2e61 7261 6e67  or i in np.arang
+00001e90: 6528 6d29 3a0a 2020 2020 2020 2020 7320  e(m):.        s 
+00001ea0: 3d20 7368 6966 746d 7478 282d 6574 615b  = shiftmtx(-eta[
+00001eb0: 695d 2c20 6e2c 2074 7329 0a20 2020 2020  i], n, ts).     
+00001ec0: 2020 2078 6164 6a5b 3a2c 2069 5d20 3d20     xadj[:, i] = 
+00001ed0: 7320 4020 2878 5b3a 2c20 695d 202f 2061  s @ (x[:, i] / a
+00001ee0: 5b69 5d29 0a0a 2020 2020 7265 7475 726e  [i])..    return
+00001ef0: 2078 6164 6a0a 0a0a 6465 6620 636f 7374   xadj...def cost
+00001f00: 6675 6e6c 7371 2866 756e 3a20 4361 6c6c  funlsq(fun: Call
+00001f10: 6162 6c65 2c20 7468 6574 613a 2041 7272  able, theta: Arr
+00001f20: 6179 4c69 6b65 2c20 7878 3a20 4172 7261  ayLike, xx: Arra
+00001f30: 794c 696b 652c 2079 793a 2041 7272 6179  yLike, yy: Array
+00001f40: 4c69 6b65 2c0a 2020 2020 2020 2020 2020  Like,.          
+00001f50: 2020 2020 2073 6967 6d61 783a 2041 7272       sigmax: Arr
+00001f60: 6179 4c69 6b65 2c20 7369 676d 6179 3a20  ayLike, sigmay: 
+00001f70: 4172 7261 794c 696b 652c 2074 733a 2066  ArrayLike, ts: f
+00001f80: 6c6f 6174 2920 2d3e 2041 7272 6179 4c69  loat) -> ArrayLi
+00001f90: 6b65 3a0a 2020 2020 7222 2222 436f 6d70  ke:.    r"""Comp
+00001fa0: 7574 6573 2074 6865 206d 6178 696d 756d  utes the maximum
+00001fb0: 206c 696b 656c 6968 6f6f 6420 636f 7374   likelihood cost
+00001fc0: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
+00001fd0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00001fe0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00001ff0: 2020 6675 6e20 3a20 6361 6c6c 6162 6c65    fun : callable
+00002000: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
+00002010: 6e73 6665 7220 6675 6e63 7469 6f6e 2c20  nsfer function, 
+00002020: 696e 2074 6865 2066 6f72 6d20 6675 6e28  in the form fun(
+00002030: 7468 6574 612c 7729 2c20 2d69 7774 2063  theta,w), -iwt c
+00002040: 6f6e 7665 6e74 696f 6e2e 0a0a 2020 2020  onvention...    
+00002050: 2020 2020 7468 6574 6120 3a20 6172 7261      theta : arra
+00002060: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+00002070: 2020 2049 6e70 7574 2070 6172 616d 6574     Input paramet
+00002080: 6572 7320 666f 7220 7468 6520 6675 6e63  ers for the func
+00002090: 7469 6f6e 2e0a 0a20 2020 2020 2020 2078  tion...        x
+000020a0: 7820 3a20 6172 7261 795f 6c69 6b65 0a20  x : array_like. 
+000020b0: 2020 2020 2020 2020 2020 204d 6561 7375             Measu
+000020c0: 7265 6420 696e 7075 7420 7369 676e 616c  red input signal
+000020d0: 2e0a 0a20 2020 2020 2020 2079 7920 3a20  ...        yy : 
+000020e0: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+000020f0: 2020 2020 2020 204d 6561 7375 7265 6420         Measured 
+00002100: 6f75 7470 7574 2073 6967 6e61 6c2e 0a0a  output signal...
+00002110: 2020 2020 2020 2020 7369 676d 6178 203a          sigmax :
+00002120: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+00002130: 2020 2020 2020 2020 4e6f 6973 6520 636f          Noise co
+00002140: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+00002150: 6f66 2074 6865 2069 6e70 7574 2073 6967  of the input sig
+00002160: 6e61 6c2e 0a0a 2020 2020 2020 2020 7369  nal...        si
+00002170: 676d 6179 203a 2061 7272 6179 5f6c 696b  gmay : array_lik
+00002180: 650a 2020 2020 2020 2020 2020 2020 4e6f  e.            No
+00002190: 6973 6520 636f 7661 7269 616e 6365 206d  ise covariance m
+000021a0: 6174 7269 7820 6f66 2074 6865 206f 7574  atrix of the out
+000021b0: 7075 7420 7369 676e 616c 2e0a 0a20 2020  put signal...   
+000021c0: 2020 2020 2074 7320 3a20 666c 6f61 740a       ts : float.
+000021d0: 2020 2020 2020 2020 2020 2020 5361 6d70              Samp
+000021e0: 6c69 6e67 2074 696d 652e 0a0a 2020 2020  ling time...    
+000021f0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00002200: 2d2d 2d0a 2020 2020 7265 7320 3a20 6172  ---.    res : ar
+00002210: 7261 795f 6c69 6b65 0a0a 0a20 2020 2022  ray_like...    "
+00002220: 2222 0a20 2020 206e 203d 2078 782e 7368  "".    n = xx.sh
+00002230: 6170 655b 305d 0a20 2020 2077 6666 7420  ape[0].    wfft 
+00002240: 3d20 3220 2a20 6e70 2e70 6920 2a20 7266  = 2 * np.pi * rf
+00002250: 6674 6672 6571 286e 2c20 7473 290a 2020  ftfreq(n, ts).  
+00002260: 2020 6820 3d20 6e70 2e63 6f6e 6a28 6675    h = np.conj(fu
+00002270: 6e28 7468 6574 612c 2077 6666 7429 290a  n(theta, wfft)).
+00002280: 0a20 2020 2072 7920 3d20 7979 202d 2069  .    ry = yy - i
+00002290: 7266 6674 2872 6666 7428 7878 2920 2a20  rfft(rfft(xx) * 
+000022a0: 682c 206e 3d6e 290a 2020 2020 7679 203d  h, n=n).    vy =
+000022b0: 206e 702e 6469 6167 2873 6967 6d61 7920   np.diag(sigmay 
+000022c0: 2a2a 2032 290a 0a20 2020 2068 7469 6c64  ** 2)..    htild
+000022d0: 6520 3d20 6972 6666 7428 682c 206e 3d6e  e = irfft(h, n=n
+000022e0: 290a 0a20 2020 2075 7920 3d20 6e70 2e7a  )..    uy = np.z
+000022f0: 6572 6f73 2828 6e2c 206e 2929 0a20 2020  eros((n, n)).   
+00002300: 2066 6f72 206b 2069 6e20 6e70 2e61 7261   for k in np.ara
+00002310: 6e67 6528 6e29 3a0a 2020 2020 2020 2020  nge(n):.        
+00002320: 6120 3d20 6e70 2e72 6573 6861 7065 286e  a = np.reshape(n
+00002330: 702e 726f 6c6c 2868 7469 6c64 652c 206b  p.roll(htilde, k
+00002340: 292c 2028 6e2c 2031 2929 0a20 2020 2020  ), (n, 1)).     
+00002350: 2020 2062 203d 206e 702e 7265 7368 6170     b = np.reshap
+00002360: 6528 6e70 2e63 6f6e 6a28 6e70 2e72 6f6c  e(np.conj(np.rol
+00002370: 6c28 6874 696c 6465 2c20 6b29 292c 2028  l(htilde, k)), (
+00002380: 312c 206e 2929 0a20 2020 2020 2020 2075  1, n)).        u
+00002390: 7920 3d20 7579 202b 206e 702e 7265 616c  y = uy + np.real
+000023a0: 286e 702e 646f 7428 612c 2062 2929 202a  (np.dot(a, b)) *
+000023b0: 2073 6967 6d61 785b 6b5d 202a 2a20 320a   sigmax[k] ** 2.
+000023c0: 2020 2020 2020 2020 2320 7579 203d 2075          # uy = u
+000023d0: 7920 2b20 6e70 2e72 6561 6c28 6e70 2e72  y + np.real(np.r
+000023e0: 6f6c 6c28 6874 696c 6465 2c20 6b2d 3129  oll(htilde, k-1)
+000023f0: 2040 206e 702e 726f 6c6c 2868 7469 6c64   @ np.roll(htild
+00002400: 652c 206b 2d31 292e 5429 2040 0a20 2020  e, k-1).T) @.   
+00002410: 2020 2020 2023 2073 6967 6d61 785b 6b5d       # sigmax[k]
+00002420: 2a2a 320a 0a20 2020 2077 203d 206e 702e  **2..    w = np.
+00002430: 646f 7428 6e70 2e65 7965 286e 292c 2073  dot(np.eye(n), s
+00002440: 6369 7079 2e6c 696e 616c 672e 696e 7628  cipy.linalg.inv(
+00002450: 7363 6970 792e 6c69 6e61 6c67 2e73 7172  scipy.linalg.sqr
+00002460: 746d 2875 7920 2b20 7679 2929 290a 2020  tm(uy + vy))).  
+00002470: 2020 7265 7320 3d20 6e70 2e64 6f74 2877    res = np.dot(w
+00002480: 2c20 7279 290a 0a20 2020 2072 6574 7572  , ry)..    retur
+00002490: 6e20 7265 730a 0a0a 6465 6620 7464 7466  n res...def tdtf
+000024a0: 2866 756e 3a20 4361 6c6c 6162 6c65 2c20  (fun: Callable, 
+000024b0: 7468 6574 613a 2041 7272 6179 4c69 6b65  theta: ArrayLike
+000024c0: 2c20 6e3a 2069 6e74 2c20 7473 3a20 666c  , n: int, ts: fl
+000024d0: 6f61 7429 202d 3e20 4172 7261 794c 696b  oat) -> ArrayLik
+000024e0: 653a 0a20 2020 2022 2222 0a20 2020 2043  e:.    """.    C
+000024f0: 6f6d 7075 7465 7320 7468 6520 7469 6d65  omputes the time
+00002500: 2d64 6f6d 6169 6e20 7472 616e 7366 6572  -domain transfer
+00002510: 206d 6174 7269 7820 666f 7220 6120 6672   matrix for a fr
+00002520: 6571 7565 6e63 7920 7265 7370 6f6e 7365  equency response
+00002530: 2066 756e 6374 696f 6e2e 0a0a 2020 2020   function...    
+00002540: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00002550: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00002560: 2020 6675 6e20 3a20 6361 6c6c 6162 6c65    fun : callable
+00002570: 0a20 2020 2020 2020 2020 2020 2046 7265  .            Fre
+00002580: 7175 656e 6379 2066 756e 6374 696f 6e2c  quency function,
+00002590: 2069 6e20 7468 6520 666f 726d 2066 756e   in the form fun
+000025a0: 2874 6865 7461 2c20 7729 2c20 7768 6572  (theta, w), wher
+000025b0: 6520 7468 6574 610a 2020 2020 2020 2020  e theta.        
+000025c0: 2020 2020 6973 2061 2076 6563 746f 7220      is a vector 
+000025d0: 6f66 2074 6865 2066 756e 6374 696f 6e20  of the function 
+000025e0: 7061 7261 6d65 7465 7273 2e20 5468 6520  parameters. The 
+000025f0: 6675 6e63 7469 6f6e 2073 686f 756c 6420  function should 
+00002600: 6265 0a20 2020 2020 2020 2020 2020 2065  be.            e
+00002610: 7870 7265 7373 6564 2069 6e20 7468 6520  xpressed in the 
+00002620: 2d69 7774 2063 6f6e 7665 6e74 696f 6e20  -iwt convention 
+00002630: 616e 6420 6d75 7374 2062 6520 4865 726d  and must be Herm
+00002640: 6974 6961 6e2e 0a0a 2020 2020 2020 2020  itian...        
+00002650: 7468 6574 6120 3a20 6172 7261 795f 6c69  theta : array_li
+00002660: 6b65 0a20 2020 2020 2020 2020 2020 2049  ke.            I
+00002670: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
+00002680: 666f 7220 7468 6520 6675 6e63 7469 6f6e  for the function
+00002690: 2e0a 0a20 2020 2020 2020 206e 203a 2069  ...        n : i
+000026a0: 6e74 0a20 2020 2020 2020 2020 2020 204e  nt.            N
+000026b0: 756d 6265 7220 6f66 2074 696d 6520 7361  umber of time sa
+000026c0: 6d70 6c65 732e 0a0a 2020 2020 2020 2020  mples...        
+000026d0: 7473 203a 2061 7272 6179 5f6c 696b 650a  ts : array_like.
+000026e0: 2020 2020 2020 2020 2020 2020 5361 6d70              Samp
+000026f0: 6c69 6e67 2074 696d 652e 0a0a 2020 2020  ling time...    
+00002700: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00002710: 2d2d 2d0a 2020 2020 2020 2020 6820 3a20  ---.        h : 
+00002720: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+00002730: 2020 2020 2020 2054 7261 6e73 6665 7220         Transfer 
+00002740: 6d61 7472 6978 2077 6974 6820 7369 7a65  matrix with size
+00002750: 2028 6e2c 6e29 2e0a 0a20 2020 2022 2222   (n,n)...    """
+00002760: 0a0a 2020 2020 2320 636f 6d70 7574 6520  ..    # compute 
+00002770: 7468 6520 7472 616e 7366 6572 2066 756e  the transfer fun
+00002780: 6374 696f 6e20 6f76 6572 2070 6f73 6974  ction over posit
+00002790: 6976 6520 6672 6571 7565 6e63 6965 730a  ive frequencies.
+000027a0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+000027b0: 7461 6e63 6528 7473 2c20 6e70 2e6e 6461  tance(ts, np.nda
+000027c0: 7272 6179 293a 0a20 2020 2020 2020 2074  rray):.        t
+000027d0: 7320 3d20 6e70 2e61 7272 6179 285b 7473  s = np.array([ts
+000027e0: 5d29 0a20 2020 2065 6c73 653a 0a20 2020  ]).    else:.   
+000027f0: 2020 2020 2074 7320 3d20 7473 0a0a 2020       ts = ts..  
+00002800: 2020 6673 203d 2031 202f 2028 7473 202a    fs = 1 / (ts *
+00002810: 206e 290a 2020 2020 6670 203d 2066 7320   n).    fp = fs 
+00002820: 2a20 6e70 2e61 7261 6e67 6528 302c 2028  * np.arange(0, (
+00002830: 6e20 2d20 3129 202f 2f20 3220 2b20 3129  n - 1) // 2 + 1)
+00002840: 0a20 2020 2077 7020 3d20 3220 2a20 6e70  .    wp = 2 * np
+00002850: 2e70 6920 2a20 6670 0a20 2020 2074 6675  .pi * fp.    tfu
+00002860: 6e70 203d 2066 756e 2874 6865 7461 2c20  np = fun(theta, 
+00002870: 7770 290a 0a20 2020 2023 2054 6865 2074  wp)..    # The t
+00002880: 7261 6e73 6665 7220 6675 6e63 7469 6f6e  ransfer function
+00002890: 2069 7320 4865 726d 6974 6961 6e2c 2073   is Hermitian, s
+000028a0: 6f20 7765 2065 7661 6c75 6174 6520 6e65  o we evaluate ne
+000028b0: 6761 7469 7665 2066 7265 7175 656e 6369  gative frequenci
+000028c0: 6573 0a20 2020 2023 2062 7920 7461 6b69  es.    # by taki
+000028d0: 6e67 2074 6865 2063 6f6d 706c 6578 2063  ng the complex c
+000028e0: 6f6e 6a75 6761 7465 206f 6620 7468 6520  onjugate of the 
+000028f0: 636f 7272 6573 706f 6e64 696e 6720 706f  corresponding po
+00002900: 7369 7469 7665 2066 7265 7175 656e 6379  sitive frequency
+00002910: 2e0a 2020 2020 2320 496e 636c 7564 6520  ..    # Include 
+00002920: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
+00002930: 2074 7261 6e73 6665 7220 6675 6e63 7469   transfer functi
+00002940: 6f6e 2061 7420 7468 6520 4e79 7175 6973  on at the Nyquis
+00002950: 7420 6672 6571 7565 6e63 7920 666f 720a  t frequency for.
+00002960: 2020 2020 2320 6576 656e 206e 2e0a 2020      # even n..  
+00002970: 2020 6966 206e 2025 2032 2021 3d20 303a    if n % 2 != 0:
+00002980: 0a20 2020 2020 2020 2074 6675 6e20 3d20  .        tfun = 
+00002990: 6e70 2e63 6f6e 6361 7465 6e61 7465 2828  np.concatenate((
+000029a0: 7466 756e 702c 206e 702e 636f 6e6a 286e  tfunp, np.conj(n
+000029b0: 702e 666c 6970 7564 2874 6675 6e70 5b31  p.flipud(tfunp[1
+000029c0: 3a5d 2929 2929 0a0a 2020 2020 656c 7365  :]))))..    else
+000029d0: 3a0a 2020 2020 2020 2020 776e 7920 3d20  :.        wny = 
+000029e0: 6e70 2e70 6920 2a20 6e20 2a20 6673 0a20  np.pi * n * fs. 
+000029f0: 2020 2020 2020 2023 2070 7269 6e74 2827         # print('
+00002a00: 7466 756e 7027 2c20 7466 756e 7029 0a20  tfunp', tfunp). 
+00002a10: 2020 2020 2020 2074 6675 6e20 3d20 6e70         tfun = np
+00002a20: 2e63 6f6e 6361 7465 6e61 7465 280a 2020  .concatenate(.  
+00002a30: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
+00002a40: 2020 2020 2020 2020 2020 2020 7466 756e              tfun
+00002a50: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+00002a60: 2020 206e 702e 636f 6e6a 280a 2020 2020     np.conj(.    
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a80: 6e70 2e63 6f6e 6361 7465 6e61 7465 2828  np.concatenate((
+00002a90: 6675 6e28 7468 6574 612c 2077 6e79 292c  fun(theta, wny),
+00002aa0: 206e 702e 666c 6970 7564 2874 6675 6e70   np.flipud(tfunp
+00002ab0: 5b31 3a5d 2929 290a 2020 2020 2020 2020  [1:]))).        
+00002ac0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00002ad0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00002ae0: 2029 0a0a 2020 2020 2320 4576 616c 7561   )..    # Evalua
+00002af0: 7465 2074 6865 2069 6d70 756c 7365 2072  te the impulse r
+00002b00: 6573 706f 6e73 6520 6279 2074 616b 696e  esponse by takin
+00002b10: 6720 7468 6520 696e 7665 7273 6520 466f  g the inverse Fo
+00002b20: 7572 6965 7220 7472 616e 7366 6f72 6d2c  urier transform,
+00002b30: 0a20 2020 2023 2074 616b 696e 6720 7468  .    # taking th
+00002b40: 6520 636f 6d70 6c65 7820 636f 6e6a 7567  e complex conjug
+00002b50: 6174 6520 6669 7273 7420 746f 2063 6f6e  ate first to con
+00002b60: 7665 7274 2074 6f20 2e2e 2e20 2b69 7774  vert to ... +iwt
+00002b70: 2063 6f6e 7665 6e74 696f 6e0a 0a20 2020   convention..   
+00002b80: 2069 6d70 203d 206e 702e 7265 616c 286e   imp = np.real(n
+00002b90: 702e 6666 742e 6966 6674 286e 702e 636f  p.fft.ifft(np.co
+00002ba0: 6e6a 2874 6675 6e29 2929 0a20 2020 2068  nj(tfun))).    h
+00002bb0: 203d 2073 6369 7079 2e6c 696e 616c 672e   = scipy.linalg.
+00002bc0: 746f 6570 6c69 747a 2869 6d70 2c20 6e70  toeplitz(imp, np
+00002bd0: 2e72 6f6c 6c28 6e70 2e66 6c69 7075 6428  .roll(np.flipud(
+00002be0: 696d 7029 2c20 3129 290a 0a20 2020 2072  imp), 1))..    r
+00002bf0: 6574 7572 6e20 680a 0a0a 6465 6620 7464  eturn h...def td
+00002c00: 6e6c 6c28 783a 2041 7272 6179 4c69 6b65  nll(x: ArrayLike
+00002c10: 2c20 7061 7261 6d2c 2066 6978 293a 0a20  , param, fix):. 
+00002c20: 2020 2072 2222 2243 6f6d 7075 7465 7320     r"""Computes 
+00002c30: 6e65 6761 7469 7665 206c 6f67 2d6c 696b  negative log-lik
+00002c40: 656c 6968 6f6f 6420 666f 7220 7468 6520  elihood for the 
+00002c50: 7469 6d65 2d64 6f6d 6169 6e20 6e6f 6973  time-domain nois
+00002c60: 6520 6d6f 6465 6c2e 0a0a 2020 2020 436f  e model...    Co
+00002c70: 6d70 7574 6573 2074 6865 206e 6567 6174  mputes the negat
+00002c80: 6976 6520 6c6f 672d 6c69 6b65 6c69 686f  ive log-likeliho
+00002c90: 6f64 2066 756e 6374 696f 6e20 666f 7220  od function for 
+00002ca0: 6f62 7461 696e 696e 6720 7468 650a 2020  obtaining the.  
+00002cb0: 2020 2064 6174 6120 6d61 7472 6978 2078     data matrix x
+00002cc0: 2c20 6769 7665 6e20 7468 6520 7061 7261  , given the para
+00002cd0: 6d65 7465 7220 6469 6374 696f 6e61 7279  meter dictionary
+00002ce0: 2070 6172 616d 2e0a 0a20 2020 2050 6172   param...    Par
+00002cf0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00002d00: 2d2d 2d2d 2d2d 0a20 2020 2078 203a 206e  ------.    x : n
+00002d10: 6461 7272 6179 206f 7220 6d61 7472 6978  darray or matrix
+00002d20: 0a20 2020 2020 2020 2044 6174 6120 6d61  .        Data ma
+00002d30: 7472 6978 0a20 2020 2070 6172 616d 203a  trix.    param :
+00002d40: 2064 6963 740a 2020 2020 2020 2020 4120   dict.        A 
+00002d50: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
+00002d60: 696e 696e 6720 7061 7261 6d65 7465 7273  ining parameters
+00002d70: 2069 6e63 6c75 6469 6e67 3a0a 2020 2020   including:.    
+00002d80: 2020 2020 6c6f 6776 203a 206e 6461 7272      logv : ndarr
+00002d90: 6179 0a20 2020 2020 2020 2020 2020 2041  ay.            A
+00002da0: 7272 6179 206f 6620 7369 7a65 2028 332c  rray of size (3,
+00002db0: 2029 2063 6f6e 7461 696e 696e 6720 6c6f   ) containing lo
+00002dc0: 6720 6f66 206e 6f69 7365 2070 6172 616d  g of noise param
+00002dd0: 6574 6572 732e 0a20 2020 2020 2020 206d  eters..        m
+00002de0: 7520 3a20 6e64 6172 7261 790a 2020 2020  u : ndarray.    
+00002df0: 2020 2020 2020 2020 5369 676e 616c 2076          Signal v
+00002e00: 6563 746f 7220 6f66 2073 697a 6520 286e  ector of size (n
+00002e10: 2c29 2e0a 2020 2020 2020 2020 613a 206e  ,)..        a: n
+00002e20: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
+00002e30: 2020 2041 6d70 6c69 7475 6465 2076 6563     Amplitude vec
+00002e40: 746f 7220 6f66 2073 697a 6520 286d 2c29  tor of size (m,)
+00002e50: 2e0a 2020 2020 2020 2020 6574 6120 3a20  ..        eta : 
+00002e60: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+00002e70: 2020 2020 4465 6c61 7920 7665 6374 6f72      Delay vector
+00002e80: 206f 6620 7369 7a65 2028 6d2c 292e 0a20   of size (m,).. 
+00002e90: 2020 2020 2020 2074 7320 3a20 666c 6f61         ts : floa
+00002ea0: 740a 2020 2020 2020 2020 2020 2020 5361  t.            Sa
+00002eb0: 6d70 6c69 6e67 2074 696d 652e 0a20 2020  mpling time..   
+00002ec0: 2020 2020 2064 203a 206e 6461 7272 6179       d : ndarray
+00002ed0: 206f 7220 6d61 7472 6978 0a20 2020 2020   or matrix.     
+00002ee0: 2020 2020 2020 206e 2d62 792d 6e20 6465         n-by-n de
+00002ef0: 7269 7661 7469 7665 206d 6174 7269 782e  rivative matrix.
+00002f00: 0a20 2020 2066 6978 203a 2064 6963 740a  .    fix : dict.
+00002f10: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
+00002f20: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00002f30: 7661 7269 6162 6c65 7320 746f 2066 6978  variables to fix
+00002f40: 2066 6f72 2074 6865 2067 7261 6469 656e   for the gradien
+00002f50: 7420 6361 6c63 756c 6174 696f 6e2e 0a20  t calculation.. 
+00002f60: 2020 2020 2020 206c 6f67 7620 3a20 626f         logv : bo
+00002f70: 6f6c 0a20 2020 2020 2020 2020 2020 204c  ol.            L
+00002f80: 6f67 206f 6620 6e6f 6973 6520 7061 7261  og of noise para
+00002f90: 6d65 7465 7273 2e0a 2020 2020 2020 2020  meters..        
+00002fa0: 6d75 203a 2062 6f6f 6c0a 2020 2020 2020  mu : bool.      
+00002fb0: 2020 2020 2020 5369 676e 616c 2076 6563        Signal vec
+00002fc0: 746f 722e 0a20 2020 2020 2020 2061 203a  tor..        a :
+00002fd0: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+00002fe0: 2020 416d 706c 6974 7564 6520 7665 6374    Amplitude vect
+00002ff0: 6f72 2e0a 2020 2020 2020 2020 6574 6120  or..        eta 
+00003000: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+00003010: 2020 2044 656c 6179 2076 6563 746f 722e     Delay vector.
+00003020: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00003030: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6e6c    -------.    nl
+00003040: 6c20 3a20 6361 6c6c 6162 6c65 0a20 2020  l : callable.   
+00003050: 2020 2020 204e 6567 6174 6976 6520 6c6f       Negative lo
+00003060: 672d 6c69 6b65 6c69 686f 6f64 2066 756e  g-likelihood fun
+00003070: 6374 696f 6e0a 2020 2020 6772 6164 6e6c  ction.    gradnl
+00003080: 6c20 3a20 6e64 6172 7261 790a 2020 2020  l : ndarray.    
+00003090: 2020 2020 4772 6164 6965 6e74 206f 6620      Gradient of 
+000030a0: 7468 6520 6e65 6761 7469 7665 206c 6f67  the negative log
+000030b0: 2d6c 696b 656c 6968 6f6f 6420 6675 6e63  -likelihood func
+000030c0: 7469 6f6e 0a20 2020 2022 2222 0a20 2020  tion.    """.   
+000030d0: 2023 2050 6172 7365 2066 756e 6374 696f   # Parse functio
+000030e0: 6e20 696e 7075 7473 0a20 2020 205b 6e2c  n inputs.    [n,
+000030f0: 206d 5d20 3d20 782e 7368 6170 650a 0a20   m] = x.shape.. 
+00003100: 2020 2023 2050 6172 7365 2070 6172 616d     # Parse param
+00003110: 6574 6572 2064 6963 7469 6f6e 6172 790a  eter dictionary.
+00003120: 2020 2020 7066 6965 6c64 7320 3d20 7061      pfields = pa
+00003130: 7261 6d2e 6b65 7973 2829 0a20 2020 2069  ram.keys().    i
+00003140: 676e 6f72 6520 3d20 7b7d 0a20 2020 2069  gnore = {}.    i
+00003150: 6620 226c 6f67 7622 2069 6e20 7066 6965  f "logv" in pfie
+00003160: 6c64 733a 0a20 2020 2020 2020 2076 203d  lds:.        v =
+00003170: 206e 702e 6578 7028 7061 7261 6d5b 226c   np.exp(param["l
+00003180: 6f67 7622 5d29 0a20 2020 2020 2020 2076  ogv"]).        v
+00003190: 203d 206e 702e 7265 7368 6170 6528 762c   = np.reshape(v,
+000031a0: 2028 6c65 6e28 7629 2c20 3129 290a 2020   (len(v), 1)).  
+000031b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000031c0: 6d73 6720 3d20 2254 646e 6c6c 2072 6571  msg = "Tdnll req
+000031d0: 7569 7265 7320 5061 7261 6d20 7374 7275  uires Param stru
+000031e0: 6374 7572 6520 7769 7468 206c 6f67 7620  cture with logv 
+000031f0: 6669 656c 6422 0a20 2020 2020 2020 2072  field".        r
+00003200: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00003210: 6d73 6729 0a0a 2020 2020 6966 2022 6d75  msg)..    if "mu
+00003220: 2220 696e 2070 6669 656c 6473 3a0a 2020  " in pfields:.  
+00003230: 2020 2020 2020 6d75 203d 2070 6172 616d        mu = param
+00003240: 5b22 6d75 225d 0a20 2020 2020 2020 206d  ["mu"].        m
+00003250: 7520 3d20 6e70 2e72 6573 6861 7065 286d  u = np.reshape(m
+00003260: 752c 2028 6c65 6e28 6d75 292c 2031 2929  u, (len(mu), 1))
+00003270: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00003280: 2020 206d 7367 203d 2022 5464 6e6c 6c20     msg = "Tdnll 
+00003290: 7265 7175 6972 6573 2070 6172 616d 2073  requires param s
+000032a0: 7472 7563 7475 7265 2077 6974 6820 6d75  tructure with mu
+000032b0: 2066 6965 6c64 220a 2020 2020 2020 2020   field".        
+000032c0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000032d0: 286d 7367 290a 2020 2020 7061 7373 0a0a  (msg).    pass..
+000032e0: 2020 2020 6966 2022 6122 2069 6e20 7066      if "a" in pf
+000032f0: 6965 6c64 7320 616e 6420 7061 7261 6d5b  ields and param[
+00003300: 2261 225d 2021 3d20 5b5d 3a0a 2020 2020  "a"] != []:.    
+00003310: 2020 2020 6120 3d20 7061 7261 6d5b 2261      a = param["a
+00003320: 225d 0a20 2020 2020 2020 2061 203d 206e  "].        a = n
+00003330: 702e 7265 7368 6170 6528 612c 2028 6c65  p.reshape(a, (le
+00003340: 6e28 6129 2c20 3129 290a 2020 2020 2020  n(a), 1)).      
+00003350: 2020 6967 6e6f 7265 5b22 6122 5d20 3d20    ignore["a"] = 
+00003360: 4661 6c73 650a 2020 2020 656c 7365 3a0a  False.    else:.
+00003370: 2020 2020 2020 2020 6120 3d20 6e70 2e6f          a = np.o
+00003380: 6e65 7328 286d 2c20 3129 290a 2020 2020  nes((m, 1)).    
+00003390: 2020 2020 6967 6e6f 7265 5b22 6122 5d20      ignore["a"] 
+000033a0: 3d20 5472 7565 0a20 2020 2070 6173 730a  = True.    pass.
+000033b0: 0a20 2020 2069 6620 2265 7461 2220 696e  .    if "eta" in
+000033c0: 2070 6669 656c 6473 2061 6e64 2070 6172   pfields and par
+000033d0: 616d 5b22 6574 6122 5d20 213d 205b 5d3a  am["eta"] != []:
+000033e0: 0a20 2020 2020 2020 2065 7461 203d 2070  .        eta = p
+000033f0: 6172 616d 5b22 6574 6122 5d0a 2020 2020  aram["eta"].    
+00003400: 2020 2020 6574 6120 3d20 6e70 2e72 6573      eta = np.res
+00003410: 6861 7065 2865 7461 2c20 286c 656e 2865  hape(eta, (len(e
+00003420: 7461 292c 2031 2929 0a20 2020 2020 2020  ta), 1)).       
+00003430: 2069 676e 6f72 655b 2265 7461 225d 203d   ignore["eta"] =
+00003440: 2046 616c 7365 0a20 2020 2065 6c73 653a   False.    else:
+00003450: 0a20 2020 2020 2020 2065 7461 203d 206e  .        eta = n
+00003460: 702e 7a65 726f 7328 286d 2c20 3129 290a  p.zeros((m, 1)).
+00003470: 2020 2020 2020 2020 6967 6e6f 7265 5b22          ignore["
+00003480: 6574 6122 5d20 3d20 5472 7565 0a20 2020  eta"] = True.   
+00003490: 2070 6173 730a 0a20 2020 2069 6620 2274   pass..    if "t
+000034a0: 7322 2069 6e20 7066 6965 6c64 733a 0a20  s" in pfields:. 
+000034b0: 2020 2020 2020 2074 7320 3d20 7061 7261         ts = para
+000034c0: 6d5b 2274 7322 5d0a 2020 2020 656c 7365  m["ts"].    else
+000034d0: 3a0a 2020 2020 2020 2020 7473 203d 2031  :.        ts = 1
+000034e0: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
+000034f0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00003500: 2020 2020 2254 444e 4c4c 2072 6563 6569      "TDNLL recei
+00003510: 7665 6420 5061 7261 6d20 7374 7275 6374  ved Param struct
+00003520: 7572 6520 7769 7468 6f75 7420 7473 2066  ure without ts f
+00003530: 6965 6c64 3b20 7365 7420 746f 206f 6e65  ield; set to one
+00003540: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+00003550: 7461 636b 6c65 7665 6c3d 322c 0a20 2020  tacklevel=2,.   
+00003560: 2020 2020 2029 0a20 2020 2070 6173 730a       ).    pass.
+00003570: 0a20 2020 2069 6620 2264 2220 696e 2070  .    if "d" in p
+00003580: 6669 656c 6473 3a0a 2020 2020 2020 2020  fields:.        
+00003590: 6420 3d20 7061 7261 6d5b 2264 225d 0a20  d = param["d"]. 
+000035a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000035b0: 2023 2043 6f6d 7075 7465 2064 6572 6976   # Compute deriv
+000035c0: 6174 6976 6520 6d61 7472 6978 0a20 2020  ative matrix.   
+000035d0: 2020 2020 2064 6566 2066 756e 285f 2c20       def fun(_, 
+000035e0: 5f77 293a 0a20 2020 2020 2020 2020 2020  _w):.           
+000035f0: 2072 6574 7572 6e20 2d31 6a20 2a20 5f77   return -1j * _w
+00003600: 0a0a 2020 2020 2020 2020 6420 3d20 7464  ..        d = td
+00003610: 7466 2866 756e 2c20 302c 206e 2c20 7473  tf(fun, 0, n, ts
+00003620: 290a 2020 2020 7061 7373 0a0a 2020 2020  ).    pass..    
+00003630: 2320 436f 6d70 7574 6520 6672 6571 7565  # Compute freque
+00003640: 6e63 7920 7665 6374 6f72 2061 6e64 2046  ncy vector and F
+00003650: 6f75 7269 6572 2063 6f65 6666 6963 6965  ourier coefficie
+00003660: 6e74 7320 6f66 206d 750a 2020 2020 6620  nts of mu.    f 
+00003670: 3d20 6666 7466 7265 7128 6e2c 2074 7329  = fftfreq(n, ts)
+00003680: 0a20 2020 2077 203d 2032 202a 206e 702e  .    w = 2 * np.
+00003690: 7069 202a 2066 0a20 2020 2077 203d 2077  pi * f.    w = w
+000036a0: 2e72 6573 6861 7065 286c 656e 2877 292c  .reshape(len(w),
+000036b0: 2031 290a 2020 2020 6d75 5f66 203d 206e   1).    mu_f = n
+000036c0: 702e 6666 742e 6666 7428 6d75 2e66 6c61  p.fft.fft(mu.fla
+000036d0: 7474 656e 2829 292e 7265 7368 6170 6528  tten()).reshape(
+000036e0: 6c65 6e28 6d75 292c 2031 290a 0a20 2020  len(mu), 1)..   
+000036f0: 2067 7261 6463 616c 6320 3d20 6e70 2e6c   gradcalc = np.l
+00003700: 6f67 6963 616c 5f6e 6f74 280a 2020 2020  ogical_not(.    
+00003710: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00003720: 2020 5b66 6978 5b22 6c6f 6776 225d 5d2c    [fix["logv"]],
+00003730: 0a20 2020 2020 2020 2020 2020 205b 6669  .            [fi
+00003740: 785b 226d 7522 5d5d 2c0a 2020 2020 2020  x["mu"]],.      
+00003750: 2020 2020 2020 5b66 6978 5b22 6122 5d20        [fix["a"] 
+00003760: 6f72 2069 676e 6f72 655b 2261 225d 5d2c  or ignore["a"]],
+00003770: 0a20 2020 2020 2020 2020 2020 205b 6669  .            [fi
+00003780: 785b 2265 7461 225d 206f 7220 6967 6e6f  x["eta"] or igno
+00003790: 7265 5b22 6574 6122 5d5d 2c0a 2020 2020  re["eta"]],.    
+000037a0: 2020 2020 5d0a 2020 2020 290a 0a20 2020      ].    )..   
+000037b0: 2069 6620 6967 6e6f 7265 5b22 6574 6122   if ignore["eta"
+000037c0: 5d3a 0a20 2020 2020 2020 207a 6574 6120  ]:.        zeta 
+000037d0: 3d20 6d75 202a 206e 702e 636f 6e6a 2861  = mu * np.conj(a
+000037e0: 292e 540a 2020 2020 2020 2020 7a65 7461  ).T.        zeta
+000037f0: 5f66 203d 206e 702e 6666 742e 6666 7428  _f = np.fft.fft(
+00003800: 7a65 7461 2c20 6178 6973 3d30 290a 2020  zeta, axis=0).  
+00003810: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003820: 6578 705f 6977 6574 6120 3d20 6e70 2e65  exp_iweta = np.e
+00003830: 7870 2831 6a20 2a20 6e70 2e74 696c 6528  xp(1j * np.tile(
+00003840: 772c 206d 2920 2a20 6e70 2e63 6f6e 6a28  w, m) * np.conj(
+00003850: 6e70 2e74 696c 6528 6574 612c 206e 2929  np.tile(eta, n))
+00003860: 2e54 290a 2020 2020 2020 2020 7a65 7461  .T).        zeta
+00003870: 5f66 203d 2028 0a20 2020 2020 2020 2020  _f = (.         
+00003880: 2020 2020 2020 206e 702e 636f 6e6a 286e         np.conj(n
+00003890: 702e 7469 6c65 2861 2c20 6e29 292e 5420  p.tile(a, n)).T 
+000038a0: 2a20 6e70 2e63 6f6e 6a28 6578 705f 6977  * np.conj(exp_iw
+000038b0: 6574 6129 202a 206e 702e 7469 6c65 286d  eta) * np.tile(m
+000038c0: 755f 662c 0a20 2020 2020 2020 2020 2020  u_f,.           
+000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2020 2020 2020 2020 2020 206d 290a               m).
+00003910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00003920: 2020 7a65 7461 203d 206e 702e 7265 616c    zeta = np.real
+00003930: 286e 702e 6666 742e 6966 6674 287a 6574  (np.fft.ifft(zet
+00003940: 615f 662c 2061 7869 733d 3029 290a 0a20  a_f, axis=0)).. 
+00003950: 2020 2023 2043 6f6d 7075 7465 206e 6567     # Compute neg
+00003960: 6174 6976 6520 2d20 6c6f 6720 6c69 6b65  ative - log like
+00003970: 6c69 686f 6f64 2061 6e64 2067 7261 6469  lihood and gradi
+00003980: 656e 740a 0a20 2020 2023 2043 6f6d 7075  ent..    # Compu
+00003990: 7465 2072 6573 6964 7561 6c73 2061 6e64  te residuals and
+000039a0: 2074 6865 6972 2073 7175 6172 6573 2066   their squares f
+000039b0: 6f72 2073 7562 7365 7175 656e 7420 636f  or subsequent co
+000039c0: 6d70 7574 6174 696f 6e73 0a20 2020 2072  mputations.    r
+000039d0: 6573 203d 2078 202d 207a 6574 610a 2020  es = x - zeta.  
+000039e0: 2020 7265 7373 7120 3d20 7265 7320 2a2a    ressq = res **
+000039f0: 2032 0a0a 2020 2020 2320 5369 6d70 6c65   2..    # Simple
+00003a00: 7374 2063 6173 653a 206a 7573 7420 7661  st case: just va
+00003a10: 7269 616e 6365 2061 6e64 2073 6967 6e61  riance and signa
+00003a20: 6c20 7061 7261 6d65 7465 7273 2c20 4120  l parameters, A 
+00003a30: 616e 6420 6574 6120 6669 7865 6420 6174  and eta fixed at
+00003a40: 0a20 2020 2023 2064 6566 6175 6c74 730a  .    # defaults.
+00003a50: 2020 2020 6966 2069 676e 6f72 655b 2261      if ignore["a
+00003a60: 225d 2061 6e64 2069 676e 6f72 655b 2265  "] and ignore["e
+00003a70: 7461 225d 3a0a 2020 2020 2020 2020 646d  ta"]:.        dm
+00003a80: 7520 3d20 6e70 2e72 6561 6c28 6e70 2e66  u = np.real(np.f
+00003a90: 6674 2e69 6666 7428 316a 202a 2077 202a  ft.ifft(1j * w *
+00003aa0: 206d 755f 662c 2061 7869 733d 3029 290a   mu_f, axis=0)).
+00003ab0: 2020 2020 2020 2020 7661 6c70 6861 203d          valpha =
+00003ac0: 2076 5b30 5d0a 2020 2020 2020 2020 7662   v[0].        vb
+00003ad0: 6574 6120 3d20 765b 315d 202a 206d 7520  eta = v[1] * mu 
+00003ae0: 2a2a 2032 0a20 2020 2020 2020 2076 7461  ** 2.        vta
+00003af0: 7520 3d20 765b 325d 202a 2064 6d75 202a  u = v[2] * dmu *
+00003b00: 2a20 320a 2020 2020 2020 2020 7674 6f74  * 2.        vtot
+00003b10: 203d 2076 616c 7068 6120 2b20 7662 6574   = valpha + vbet
+00003b20: 6120 2b20 7674 6175 0a0a 2020 2020 2020  a + vtau..      
+00003b30: 2020 7265 736e 6f72 6d73 7120 3d20 7265    resnormsq = re
+00003b40: 7373 7120 2f20 6e70 2e74 696c 6528 7674  ssq / np.tile(vt
+00003b50: 6f74 2c20 6d29 0a20 2020 2020 2020 206e  ot, m).        n
+00003b60: 6c6c 203d 2028 0a20 2020 2020 2020 2020  ll = (.         
+00003b70: 2020 2020 2020 206d 202a 206e 202a 206e         m * n * n
+00003b80: 702e 6c6f 6728 3220 2a20 6e70 2e70 6929  p.log(2 * np.pi)
+00003b90: 202f 2032 0a20 2020 2020 2020 2020 2020   / 2.           
+00003ba0: 2020 2020 202b 2028 6d20 2f20 3229 202a       + (m / 2) *
+00003bb0: 206e 702e 7375 6d28 6e70 2e6c 6f67 2876   np.sum(np.log(v
+00003bc0: 746f 7429 290a 2020 2020 2020 2020 2020  tot)).          
+00003bd0: 2020 2020 2020 2b20 6e70 2e73 756d 2872        + np.sum(r
+00003be0: 6573 6e6f 726d 7371 2920 2f20 320a 2020  esnormsq) / 2.  
+00003bf0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00003c00: 2023 2043 6f6d 7075 7465 2067 7261 6469   # Compute gradi
+00003c10: 656e 7420 6966 2072 6571 7565 7374 6564  ent if requested
+00003c20: 0a20 2020 2020 2020 2023 2069 6620 6e61  .        # if na
+00003c30: 7267 6f75 7420 3e20 313a 0a20 2020 2020  rgout > 1:.     
+00003c40: 2020 206e 6772 6164 203d 206e 702e 7375     ngrad = np.su
+00003c50: 6d28 6772 6164 6361 6c63 5b30 3a32 5d20  m(gradcalc[0:2] 
+00003c60: 2a20 5b5b 335d 2c20 5b6e 5d5d 290a 2020  * [[3], [n]]).  
+00003c70: 2020 2020 2020 6772 6164 6e6c 6c20 3d20        gradnll = 
+00003c80: 6e70 2e7a 6572 6f73 2828 6e67 7261 642c  np.zeros((ngrad,
+00003c90: 2031 2929 0a20 2020 2020 2020 206e 7374   1)).        nst
+00003ca0: 6172 7420 3d20 300a 2020 2020 2020 2020  art = 0.        
+00003cb0: 6476 6172 203d 2028 7674 6f74 202d 206e  dvar = (vtot - n
+00003cc0: 702e 6d65 616e 2872 6573 7371 2c20 6178  p.mean(ressq, ax
+00003cd0: 6973 3d31 292e 7265 7368 6170 6528 6e2c  is=1).reshape(n,
+00003ce0: 2031 2929 202f 2076 746f 7420 2a2a 2032   1)) / vtot ** 2
+00003cf0: 0a20 2020 2020 2020 2069 6620 6772 6164  .        if grad
+00003d00: 6361 6c63 5b30 5d3a 0a20 2020 2020 2020  calc[0]:.       
+00003d10: 2020 2020 2067 7261 646e 6c6c 5b6e 7374       gradnll[nst
+00003d20: 6172 745d 203d 2028 6d20 2f20 3229 202a  art] = (m / 2) *
+00003d30: 206e 702e 7375 6d28 6476 6172 2920 2a20   np.sum(dvar) * 
+00003d40: 765b 305d 0a20 2020 2020 2020 2020 2020  v[0].           
+00003d50: 2067 7261 646e 6c6c 5b6e 7374 6172 7420   gradnll[nstart 
+00003d60: 2b20 315d 203d 2028 6d20 2f20 3229 202a  + 1] = (m / 2) *
+00003d70: 206e 702e 7375 6d28 6d75 202a 2a20 3220   np.sum(mu ** 2 
+00003d80: 2a20 6476 6172 2920 2a20 765b 315d 0a20  * dvar) * v[1]. 
+00003d90: 2020 2020 2020 2020 2020 2067 7261 646e             gradn
+00003da0: 6c6c 5b6e 7374 6172 7420 2b20 325d 203d  ll[nstart + 2] =
+00003db0: 2028 6d20 2f20 3229 202a 206e 702e 7375   (m / 2) * np.su
+00003dc0: 6d28 646d 7520 2a2a 2032 2e30 202a 2064  m(dmu ** 2.0 * d
+00003dd0: 7661 7229 202a 2076 5b32 5d0a 2020 2020  var) * v[2].    
+00003de0: 2020 2020 2020 2020 6e73 7461 7274 203d          nstart =
+00003df0: 206e 7374 6172 7420 2b20 330a 2020 2020   nstart + 3.    
+00003e00: 2020 2020 6966 2067 7261 6463 616c 635b      if gradcalc[
+00003e10: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
+00003e20: 2320 7072 696e 7428 276d 7520 7368 6170  # print('mu shap
+00003e30: 6520 3a20 272c 206d 752e 7368 6170 6529  e : ', mu.shape)
+00003e40: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
+00003e50: 7269 6e74 2827 6476 6172 2073 6861 7065  rint('dvar shape
+00003e60: 3a20 272c 2064 7661 722e 7368 6170 6529  : ', dvar.shape)
+00003e70: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
+00003e80: 7269 6e74 2827 6420 7368 6170 653a 2027  rint('d shape: '
+00003e90: 2c20 642e 7368 6170 6529 0a20 2020 2020  , d.shape).     
+00003ea0: 2020 2020 2020 2023 2070 7269 6e74 2827         # print('
+00003eb0: 446d 7520 7368 6170 653a 2027 2c20 646d  Dmu shape: ', dm
+00003ec0: 752e 7368 6170 6529 0a20 2020 2020 2020  u.shape).       
+00003ed0: 2020 2020 2067 7261 646e 6c6c 5b6e 7374       gradnll[nst
+00003ee0: 6172 743a 206e 7374 6172 7420 2b20 6e5d  art: nstart + n]
+00003ef0: 203d 206d 202a 2028 0a20 2020 2020 2020   = m * (.       
+00003f00: 2020 2020 2020 2020 2020 2020 2076 5b31               v[1
+00003f10: 5d20 2a20 6d75 202a 2064 7661 720a 2020  ] * mu * dvar.  
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2b20 765b 325d 202a 206e 702e 646f    + v[2] * np.do
+00003f40: 7428 642e 542c 2028 646d 7520 2a20 6476  t(d.T, (dmu * dv
+00003f50: 6172 2929 0a20 2020 2020 2020 2020 2020  ar)).           
+00003f60: 2020 2020 2020 2020 202d 206e 702e 6d65           - np.me
+00003f70: 616e 2872 6573 2c20 6178 6973 3d31 292e  an(res, axis=1).
+00003f80: 7265 7368 6170 6528 6e2c 2031 2920 2f20  reshape(n, 1) / 
+00003f90: 7674 6f74 0a20 2020 2020 2020 2020 2020  vtot.           
+00003fa0: 2029 0a0a 2020 2020 2320 416c 7465 726e   )..    # Altern
+00003fb0: 6174 6976 6520 6361 7365 3a20 412c 2065  ative case: A, e
+00003fc0: 7461 2c20 6f72 2062 6f74 6820 6172 6520  ta, or both are 
+00003fd0: 6e6f 7420 7365 7420 746f 2064 6566 6175  not set to defau
+00003fe0: 6c74 730a 2020 2020 656c 7365 3a0a 2020  lts.    else:.  
+00003ff0: 2020 2020 2020 647a 6574 6120 3d20 6e70        dzeta = np
+00004000: 2e72 6561 6c28 6e70 2e66 6674 2e69 6666  .real(np.fft.iff
+00004010: 7428 316a 202a 206e 702e 7469 6c65 2877  t(1j * np.tile(w
+00004020: 2c20 6d29 202a 207a 6574 615f 662c 2061  , m) * zeta_f, a
+00004030: 7869 733d 3029 290a 0a20 2020 2020 2020  xis=0))..       
+00004040: 2076 616c 7068 6120 3d20 765b 305d 0a20   valpha = v[0]. 
+00004050: 2020 2020 2020 2076 6265 7461 203d 2076         vbeta = v
+00004060: 5b31 5d20 2a20 7a65 7461 202a 2a20 320a  [1] * zeta ** 2.
+00004070: 2020 2020 2020 2020 7674 6175 203d 2076          vtau = v
+00004080: 5b32 5d20 2a20 647a 6574 6120 2a2a 2032  [2] * dzeta ** 2
+00004090: 0a20 2020 2020 2020 2076 746f 7420 3d20  .        vtot = 
+000040a0: 7661 6c70 6861 202b 2076 6265 7461 202b  valpha + vbeta +
+000040b0: 2076 7461 750a 0a20 2020 2020 2020 2072   vtau..        r
+000040c0: 6573 6e6f 726d 7371 203d 2072 6573 7371  esnormsq = ressq
+000040d0: 202f 2076 746f 740a 2020 2020 2020 2020   / vtot.        
+000040e0: 6e6c 6c20 3d20 280a 2020 2020 2020 2020  nll = (.        
+000040f0: 2020 2020 2020 2020 6d20 2a20 6e20 2a20          m * n * 
+00004100: 6e70 2e6c 6f67 2832 202a 206e 702e 7069  np.log(2 * np.pi
+00004110: 2920 2f20 320a 2020 2020 2020 2020 2020  ) / 2.          
+00004120: 2020 2020 2020 2b20 6e70 2e73 756d 286e        + np.sum(n
+00004130: 702e 6c6f 6728 7674 6f74 2929 202f 2032  p.log(vtot)) / 2
+00004140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004150: 202b 206e 702e 7375 6d28 7265 736e 6f72   + np.sum(resnor
+00004160: 6d73 7129 202f 2032 0a20 2020 2020 2020  msq) / 2.       
+00004170: 2029 0a0a 2020 2020 2020 2020 2320 436f   )..        # Co
+00004180: 6d70 7574 6520 6772 6164 6965 6e74 2069  mpute gradient i
+00004190: 6620 7265 7175 6573 7465 640a 2020 2020  f requested.    
+000041a0: 2020 2020 2320 6966 206e 6172 676f 7574      # if nargout
+000041b0: 203e 2031 3a0a 2020 2020 2020 2020 6e67   > 1:.        ng
+000041c0: 7261 6420 3d20 6e70 2e73 756d 2867 7261  rad = np.sum(gra
+000041d0: 6463 616c 6320 2a20 5b5b 335d 2c20 5b6e  dcalc * [[3], [n
+000041e0: 5d2c 205b 6d5d 2c20 5b6d 5d5d 290a 2020  ], [m], [m]]).  
+000041f0: 2020 2020 2020 6772 6164 6e6c 6c20 3d20        gradnll = 
+00004200: 6e70 2e7a 6572 6f73 2828 6e67 7261 642c  np.zeros((ngrad,
+00004210: 2031 2929 0a20 2020 2020 2020 206e 7374   1)).        nst
+00004220: 6172 7420 3d20 300a 2020 2020 2020 2020  art = 0.        
+00004230: 7265 7377 7420 3d20 7265 7320 2f20 7674  reswt = res / vt
+00004240: 6f74 0a20 2020 2020 2020 2064 7661 7220  ot.        dvar 
+00004250: 3d20 2876 746f 7420 2d20 7265 7373 7129  = (vtot - ressq)
+00004260: 202f 2076 746f 7420 2a2a 2032 0a20 2020   / vtot ** 2.   
+00004270: 2020 2020 2069 6620 6772 6164 6361 6c63       if gradcalc
+00004280: 5b30 5d3a 0a20 2020 2020 2020 2020 2020  [0]:.           
+00004290: 2023 2047 7261 6469 656e 7420 7772 7420   # Gradient wrt 
+000042a0: 6c6f 6776 0a20 2020 2020 2020 2020 2020  logv.           
+000042b0: 2067 7261 646e 6c6c 5b6e 7374 6172 745d   gradnll[nstart]
+000042c0: 203d 2030 2e35 202a 206e 702e 7375 6d28   = 0.5 * np.sum(
+000042d0: 6476 6172 2920 2a20 765b 305d 0a20 2020  dvar) * v[0].   
+000042e0: 2020 2020 2020 2020 2067 7261 646e 6c6c           gradnll
+000042f0: 5b6e 7374 6172 7420 2b20 315d 203d 2028  [nstart + 1] = (
+00004300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004310: 2020 2020 2030 2e35 202a 206e 702e 7375       0.5 * np.su
+00004320: 6d28 7a65 7461 2e66 6c61 7474 656e 2829  m(zeta.flatten()
+00004330: 202a 2a20 3220 2a20 6476 6172 2e66 6c61   ** 2 * dvar.fla
+00004340: 7474 656e 2829 2920 2a20 765b 315d 0a20  tten()) * v[1]. 
+00004350: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004360: 2020 2020 2020 2020 2067 7261 646e 6c6c           gradnll
+00004370: 5b6e 7374 6172 7420 2b20 325d 203d 2028  [nstart + 2] = (
+00004380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004390: 2020 2020 2030 2e35 202a 206e 702e 7375       0.5 * np.su
+000043a0: 6d28 647a 6574 612e 666c 6174 7465 6e28  m(dzeta.flatten(
+000043b0: 2920 2a2a 2032 202a 2064 7661 722e 666c  ) ** 2 * dvar.fl
+000043c0: 6174 7465 6e28 2929 202a 2076 5b32 5d0a  atten()) * v[2].
+000043d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000043e0: 2020 2020 2020 2020 2020 6e73 7461 7274            nstart
+000043f0: 203d 206e 7374 6172 7420 2b20 330a 2020   = nstart + 3.  
+00004400: 2020 2020 2020 6966 2067 7261 6463 616c        if gradcal
+00004410: 635b 315d 3a0a 2020 2020 2020 2020 2020  c[1]:.          
+00004420: 2020 2320 4772 6164 6965 6e74 2077 7274    # Gradient wrt
+00004430: 206d 750a 2020 2020 2020 2020 2020 2020   mu.            
+00004440: 7020 3d20 6e70 2e66 6674 2e66 6674 2876  p = np.fft.fft(v
+00004450: 5b31 5d20 2a20 6476 6172 202a 207a 6574  [1] * dvar * zet
+00004460: 6120 2d20 7265 7377 742c 2061 7869 733d  a - reswt, axis=
+00004470: 3029 202d 2031 6a20 2a20 765b 0a20 2020  0) - 1j * v[.   
+00004480: 2020 2020 2020 2020 2020 2020 2032 0a20               2. 
+00004490: 2020 2020 2020 2020 2020 205d 202a 2077             ] * w
+000044a0: 202a 206e 702e 6666 742e 6666 7428 6476   * np.fft.fft(dv
+000044b0: 6172 202a 2064 7a65 7461 2c20 6178 6973  ar * dzeta, axis
+000044c0: 3d30 290a 2020 2020 2020 2020 2020 2020  =0).            
+000044d0: 6772 6164 6e6c 6c5b 6e73 7461 7274 3a20  gradnll[nstart: 
+000044e0: 6e73 7461 7274 202b 206e 5d20 3d20 6e70  nstart + n] = np
+000044f0: 2e73 756d 280a 2020 2020 2020 2020 2020  .sum(.          
+00004500: 2020 2020 2020 6e70 2e63 6f6e 6a28 6129        np.conj(a)
+00004510: 2e54 202a 206e 702e 7265 616c 286e 702e  .T * np.real(np.
+00004520: 6666 742e 6966 6674 2865 7870 5f69 7765  fft.ifft(exp_iwe
+00004530: 7461 202a 2070 2c20 6178 6973 3d30 2929  ta * p, axis=0))
+00004540: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004550: 2020 6178 6973 3d31 2c0a 2020 2020 2020    axis=1,.      
+00004560: 2020 2020 2020 292e 7265 7368 6170 6528        ).reshape(
+00004570: 6e2c 2031 290a 2020 2020 2020 2020 2020  n, 1).          
+00004580: 2020 6e73 7461 7274 203d 206e 7374 6172    nstart = nstar
+00004590: 7420 2b20 6e0a 2020 2020 2020 2020 6966  t + n.        if
+000045a0: 2067 7261 6463 616c 635b 325d 3a0a 2020   gradcalc[2]:.  
+000045b0: 2020 2020 2020 2020 2020 2320 4772 6164            # Grad
+000045c0: 6965 6e74 2077 7274 2041 0a20 2020 2020  ient wrt A.     
+000045d0: 2020 2020 2020 2074 6572 6d20 3d20 2876         term = (v
+000045e0: 746f 7420 2d20 7661 6c70 6861 2920 2a20  tot - valpha) * 
+000045f0: 6476 6172 202d 2072 6573 7774 202a 207a  dvar - reswt * z
+00004600: 6574 610a 2020 2020 2020 2020 2020 2020  eta.            
+00004610: 6966 206e 702e 616e 7928 6e70 2e69 7363  if np.any(np.isc
+00004620: 6c6f 7365 2861 2c20 3029 293a 0a20 2020  lose(a, 0)):.   
+00004630: 2020 2020 2020 2020 2020 2020 206d 7367               msg
+00004640: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00004650: 2020 2020 2020 2020 2022 4f6e 6520 6f72           "One or
+00004660: 206d 6f72 6520 656c 656d 656e 7473 206f   more elements o
+00004670: 6620 7468 6520 616d 706c 6974 7564 6520  f the amplitude 
+00004680: 7665 6374 6f72 2061 7265 2022 0a20 2020  vector are ".   
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2022 636c 6f73 6520 746f 207a 6572 6f20   "close to zero 
+000046b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000046c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000046d0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000046e0: 7272 6f72 286d 7367 290a 2020 2020 2020  rror(msg).      
+000046f0: 2020 2020 2020 6772 6164 6e6c 6c5b 6e73        gradnll[ns
+00004700: 7461 7274 3a20 6e73 7461 7274 202b 206d  tart: nstart + m
+00004710: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+00004720: 2020 2020 2020 2020 2020 6e70 2e63 6f6e            np.con
+00004730: 6a28 6e70 2e73 756d 2874 6572 6d2c 2061  j(np.sum(term, a
+00004740: 7869 733d 3029 292e 7265 7368 6170 6528  xis=0)).reshape(
+00004750: 6d2c 2031 2920 2f20 610a 2020 2020 2020  m, 1) / a.      
+00004760: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004770: 2020 2020 6966 206e 6f74 2066 6978 5b22      if not fix["
+00004780: 6d75 225d 3a0a 2020 2020 2020 2020 2020  mu"]:.          
+00004790: 2020 2020 2020 6772 6164 6e6c 6c20 3d20        gradnll = 
+000047a0: 6e70 2e64 656c 6574 6528 6772 6164 6e6c  np.delete(gradnl
+000047b0: 6c2c 206e 7374 6172 7429 0a20 2020 2020  l, nstart).     
+000047c0: 2020 2020 2020 2020 2020 206e 7374 6172             nstar
+000047d0: 7420 3d20 6e73 7461 7274 202b 206d 202d  t = nstart + m -
+000047e0: 2031 0a20 2020 2020 2020 2020 2020 2065   1.            e
+000047f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00004800: 2020 2020 206e 7374 6172 7420 3d20 6e73       nstart = ns
+00004810: 7461 7274 202b 206d 0a20 2020 2020 2020  tart + m.       
+00004820: 2069 6620 6772 6164 6361 6c63 5b33 5d3a   if gradcalc[3]:
+00004830: 0a20 2020 2020 2020 2020 2020 2023 2047  .            # G
+00004840: 7261 6469 656e 7420 7772 7420 6574 610a  radient wrt eta.
+00004850: 2020 2020 2020 2020 2020 2020 6464 7a65              ddze
+00004860: 7461 203d 206e 702e 7265 616c 286e 702e  ta = np.real(np.
+00004870: 6666 742e 6966 6674 282d 6e70 2e74 696c  fft.ifft(-np.til
+00004880: 6528 772c 206d 2920 2a2a 2032 202a 207a  e(w, m) ** 2 * z
+00004890: 6574 615f 662c 2061 7869 733d 3029 290a  eta_f, axis=0)).
+000048a0: 2020 2020 2020 2020 2020 2020 6772 6164              grad
+000048b0: 6e6c 6c20 3d20 6e70 2e73 7175 6565 7a65  nll = np.squeeze
+000048c0: 2867 7261 646e 6c6c 290a 2020 2020 2020  (gradnll).      
+000048d0: 2020 2020 2020 6772 6164 6e6c 6c5b 6e73        gradnll[ns
+000048e0: 7461 7274 3a20 6e73 7461 7274 202b 206d  tart: nstart + m
+000048f0: 5d20 3d20 2d6e 702e 7375 6d28 0a20 2020  ] = -np.sum(.   
+00004900: 2020 2020 2020 2020 2020 2020 2064 7661               dva
+00004910: 7220 2a20 287a 6574 6120 2a20 647a 6574  r * (zeta * dzet
+00004920: 6120 2a20 765b 315d 202b 2064 7a65 7461  a * v[1] + dzeta
+00004930: 202a 2064 647a 6574 6120 2a20 765b 325d   * ddzeta * v[2]
+00004940: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004950: 2020 2d20 7265 7377 7420 2a20 647a 6574    - reswt * dzet
+00004960: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00004970: 2020 2061 7869 733d 302c 0a20 2020 2020     axis=0,.     
+00004980: 2020 2020 2020 2029 2e72 6573 6861 7065         ).reshape
+00004990: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000049a0: 2020 6d2c 0a20 2020 2020 2020 2020 2020    m,.           
+000049b0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+000049c0: 6966 206e 6f74 2066 6978 5b22 6d75 225d  if not fix["mu"]
+000049d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000049e0: 2020 6772 6164 6e6c 6c20 3d20 6e70 2e64    gradnll = np.d
+000049f0: 656c 6574 6528 6772 6164 6e6c 6c2c 206e  elete(gradnll, n
+00004a00: 7374 6172 7429 0a20 2020 2067 7261 646e  start).    gradn
+00004a10: 6c6c 203d 2067 7261 646e 6c6c 2e66 6c61  ll = gradnll.fla
+00004a20: 7474 656e 2829 0a0a 2020 2020 7265 7475  tten()..    retu
+00004a30: 726e 206e 6c6c 2c20 6772 6164 6e6c 6c0a  rn nll, gradnll.
+00004a40: 0a0a 6465 6620 7464 6e6f 6973 6566 6974  ..def tdnoisefit
+00004a50: 280a 2020 2020 2020 2020 782c 0a20 2020  (.        x,.   
+00004a60: 2020 2020 2070 6172 616d 2c0a 2020 2020       param,.    
+00004a70: 2020 2020 6669 783d 7b22 6c6f 6776 223a      fix={"logv":
+00004a80: 2046 616c 7365 2c20 226d 7522 3a20 4661   False, "mu": Fa
+00004a90: 6c73 652c 2022 6122 3a20 5472 7565 2c20  lse, "a": True, 
+00004aa0: 2265 7461 223a 2054 7275 657d 2c0a 2020  "eta": True},.  
+00004ab0: 2020 2020 2020 6967 6e6f 7265 3d7b 2261        ignore={"a
+00004ac0: 223a 2054 7275 652c 2022 6574 6122 3a20  ": True, "eta": 
+00004ad0: 5472 7565 7d2c 0a29 3a0a 2020 2020 2222  True},.):.    ""
+00004ae0: 2243 6f6d 7075 7465 7320 7469 6d65 2d64  "Computes time-d
+00004af0: 6f6d 6169 6e20 6e6f 6973 6520 6d6f 6465  omain noise mode
+00004b00: 6c20 7061 7261 6d65 7465 7273 2e0a 0a20  l parameters... 
+00004b10: 2020 2043 6f6d 7075 7465 7320 7468 6520     Computes the 
+00004b20: 6e6f 6973 6520 7061 7261 6d65 7465 7273  noise parameters
+00004b30: 2073 6967 6d61 2061 6e64 2074 6865 2075   sigma and the u
+00004b40: 6e64 6572 6c79 696e 6720 7369 676e 616c  nderlying signal
+00004b50: 2076 6563 746f 7220 6d75 0a20 2020 2066   vector mu.    f
+00004b60: 6f72 2074 6865 2064 6174 6120 6d61 7472  or the data matr
+00004b70: 6978 2078 2c20 7768 6572 6520 7468 6520  ix x, where the 
+00004b80: 636f 6c75 6d6e 7320 6f66 2078 2061 7265  columns of x are
+00004b90: 2065 6163 6820 6e6f 6973 790a 2020 2020   each noisy.    
+00004ba0: 6d65 6173 7572 656d 656e 7473 206f 6620  measurements of 
+00004bb0: 6d75 2e0a 0a20 2020 2050 6172 616d 6574  mu...    Paramet
+00004bc0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00004bd0: 2d2d 0a20 2020 2078 203a 206e 6461 7272  --.    x : ndarr
+00004be0: 6179 206f 7220 6d61 7472 6978 0a20 2020  ay or matrix.   
+00004bf0: 2020 2020 2044 6174 6120 6d61 7472 6978       Data matrix
+00004c00: 2e0a 2020 2020 7061 7261 6d20 3a20 6469  ..    param : di
+00004c10: 6374 0a20 2020 2020 2020 2041 2064 6963  ct.        A dic
+00004c20: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+00004c30: 6e67 2069 6e69 7469 616c 2067 7565 7373  ng initial guess
+00004c40: 2066 6f72 2074 6865 2070 6172 616d 6574   for the paramet
+00004c50: 6572 733a 0a20 2020 2020 2020 2076 3020  ers:.        v0 
+00004c60: 3a20 6e64 6172 7261 790a 2020 2020 2020  : ndarray.      
+00004c70: 2020 2020 2020 496e 6974 6961 6c20 6775        Initial gu
+00004c80: 6573 732c 206e 6f69 7365 206d 6f64 656c  ess, noise model
+00004c90: 2070 6172 616d 6574 6572 732e 2041 7272   parameters. Arr
+00004ca0: 6179 206f 6620 7265 616c 2065 6c65 6d65  ay of real eleme
+00004cb0: 6e74 7320 6f66 0a20 2020 2020 2020 2020  nts of.         
+00004cc0: 2020 2073 697a 6520 2833 2c20 290a 2020     size (3, ).  
+00004cd0: 2020 2020 2020 6d75 3020 3a20 6e64 6172        mu0 : ndar
+00004ce0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+00004cf0: 496e 6974 6961 6c20 6775 6573 732c 2073  Initial guess, s
+00004d00: 6967 6e61 6c20 7665 6374 6f72 2e20 4172  ignal vector. Ar
+00004d10: 7261 7920 6f66 2072 6561 6c20 656c 656d  ray of real elem
+00004d20: 656e 7473 206f 6620 7369 7a65 2020 286e  ents of size  (n
+00004d30: 2c20 290a 2020 2020 2020 2020 6130 203a  , ).        a0 :
+00004d40: 206e 6461 7272 6179 0a20 2020 2020 2020   ndarray.       
+00004d50: 2020 2020 2049 6e69 7469 616c 2067 7565       Initial gue
+00004d60: 7373 2c20 616d 706c 6974 7564 6520 7665  ss, amplitude ve
+00004d70: 6374 6f72 2e20 4172 7261 7920 6f66 2072  ctor. Array of r
+00004d80: 6561 6c20 656c 656d 656e 7473 206f 6620  eal elements of 
+00004d90: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
+00004da0: 2028 6d2c 2029 0a20 2020 2020 2020 2065   (m, ).        e
+00004db0: 7461 3020 3a20 6e64 6172 7261 790a 2020  ta0 : ndarray.  
+00004dc0: 2020 2020 2020 2020 2020 496e 6974 6961            Initia
+00004dd0: 6c20 6775 6573 732c 2064 656c 6179 2076  l guess, delay v
+00004de0: 6563 746f 722e 2041 7272 6179 206f 6620  ector. Array of 
+00004df0: 7265 616c 2065 6c65 6d65 6e74 7320 6f66  real elements of
+00004e00: 2073 697a 6520 286d 2c20 290a 2020 2020   size (m, ).    
+00004e10: 2020 2020 7473 203a 2066 6c6f 6174 0a20      ts : float. 
+00004e20: 2020 2020 2020 2020 2020 2053 616d 706c             Sampl
+00004e30: 696e 6720 7469 6d65 0a20 2020 2066 6978  ing time.    fix
+00004e40: 203a 2064 6963 742c 206f 7074 696f 6e61   : dict, optiona
+00004e50: 6c0a 2020 2020 2020 2020 4120 6469 6374  l.        A dict
+00004e60: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+00004e70: 6720 7661 7269 6162 6c65 7320 746f 2066  g variables to f
+00004e80: 6978 2066 6f72 2074 6865 206d 696e 696d  ix for the minim
+00004e90: 697a 6174 696f 6e2e 0a20 2020 2020 2020  ization..       
+00004ea0: 206c 6f67 7620 3a20 626f 6f6c 0a20 2020   logv : bool.   
+00004eb0: 2020 2020 2020 2020 204c 6f67 206f 6620           Log of 
+00004ec0: 6e6f 6973 6520 7061 7261 6d65 7465 7273  noise parameters
+00004ed0: 2e0a 2020 2020 2020 2020 6d75 203a 2062  ..        mu : b
+00004ee0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00004ef0: 5369 676e 616c 2076 6563 746f 722e 0a20  Signal vector.. 
+00004f00: 2020 2020 2020 2061 203a 2062 6f6f 6c0a         a : bool.
+00004f10: 2020 2020 2020 2020 2020 2020 416d 706c              Ampl
+00004f20: 6974 7564 6520 7665 6374 6f72 2e0a 2020  itude vector..  
+00004f30: 2020 2020 2020 6574 6120 3a20 626f 6f6c        eta : bool
+00004f40: 0a20 2020 2020 2020 2020 2020 2044 656c  .            Del
+00004f50: 6179 2076 6563 746f 722e 0a20 2020 2020  ay vector..     
+00004f60: 2020 2049 6620 6e6f 7420 6769 7665 6e2c     If not given,
+00004f70: 2063 686f 7365 6e20 746f 2073 6574 2066   chosen to set f
+00004f80: 7265 6520 616c 6c20 7468 6520 7661 7269  ree all the vari
+00004f90: 6162 6c65 732e 0a20 2020 2069 676e 6f72  ables..    ignor
+00004fa0: 6520 3a20 6469 6374 0a20 2020 2020 2020  e : dict.       
+00004fb0: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+00004fc0: 6e74 6169 6e69 6e67 2076 6172 6961 626c  ntaining variabl
+00004fd0: 6573 2074 6f20 6967 6e6f 7265 2066 6f72  es to ignore for
+00004fe0: 2074 6865 206d 696e 696d 697a 6174 696f   the minimizatio
+00004ff0: 6e2e 0a20 2020 2020 2020 2061 203a 2062  n..        a : b
+00005000: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00005010: 416d 706c 6974 7564 6520 7665 6374 6f72  Amplitude vector
+00005020: 2e0a 2020 2020 2020 2020 6574 6120 3a20  ..        eta : 
+00005030: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00005040: 2044 656c 6179 2076 6563 746f 722e 0a20   Delay vector.. 
+00005050: 2020 2020 2020 2049 6620 6e6f 7420 6769         If not gi
+00005060: 7665 6e2c 2063 686f 7365 6e20 746f 2069  ven, chosen to i
+00005070: 676e 6f72 6520 626f 7468 2061 6d70 6c69  gnore both ampli
+00005080: 7475 6465 2061 6e64 2064 656c 6179 2e0a  tude and delay..
+00005090: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+000050a0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 7020   --------.    p 
+000050b0: 3a20 6469 6374 0a20 2020 2020 2020 204f  : dict.        O
+000050c0: 7574 7075 7420 7061 7261 6d65 7465 7220  utput parameter 
+000050d0: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
+000050e0: 696e 696e 673a 0a20 2020 2020 2020 2020  ining:.         
+000050f0: 2020 2065 7461 203a 206e 6461 7272 6179     eta : ndarray
+00005100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005110: 2044 656c 6179 2076 6563 746f 722e 0a20   Delay vector.. 
+00005120: 2020 2020 2020 2020 2020 2061 203a 206e             a : n
+00005130: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
+00005140: 2020 2020 2020 2041 6d70 6c69 7475 6465         Amplitude
+00005150: 2076 6563 746f 722e 0a20 2020 2020 2020   vector..       
+00005160: 2020 2020 206d 7520 3a20 6e64 6172 7261       mu : ndarra
+00005170: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+00005180: 2020 5369 676e 616c 2076 6563 746f 722e    Signal vector.
+00005190: 0a20 2020 2020 2020 2020 2020 2076 6172  .            var
+000051a0: 203a 206e 6461 7272 6179 0a20 2020 2020   : ndarray.     
+000051b0: 2020 2020 2020 2020 2020 204c 6f67 206f             Log o
+000051c0: 6620 6e6f 6973 6520 7061 7261 6d65 7465  f noise paramete
+000051d0: 7273 0a20 2020 2066 7661 6c20 3a20 666c  rs.    fval : fl
+000051e0: 6f61 740a 2020 2020 2020 2020 5661 6c75  oat.        Valu
+000051f0: 6520 6f66 204e 4c4c 2063 6f73 7420 6675  e of NLL cost fu
+00005200: 6e63 7469 6f6e 2066 726f 6d20 464d 494e  nction from FMIN
+00005210: 554e 430a 2020 2020 4469 6167 6e6f 7374  UNC.    Diagnost
+00005220: 6963 203a 2064 6963 740a 2020 2020 2020  ic : dict.      
+00005230: 2020 4469 6374 696f 6e61 7279 2063 6f6e    Dictionary con
+00005240: 7461 696e 696e 6720 6469 6167 6e6f 7374  taining diagnost
+00005250: 6963 2069 6e66 6f72 6d61 7469 6f6e 0a20  ic information. 
+00005260: 2020 2020 2020 2020 2020 2065 7272 203a             err :
+00005270: 2064 6963 0a20 2020 2020 2020 2020 2020   dic.           
+00005280: 2020 2020 2044 6963 7469 6f6e 6172 7920       Dictionary 
+00005290: 636f 6e74 6169 6e69 6e67 2020 6572 726f  containing  erro
+000052a0: 7220 6f66 2074 6865 2070 6172 616d 6574  r of the paramet
+000052b0: 6572 732e 0a20 2020 2020 2020 2020 2020  ers..           
+000052c0: 2067 7261 6420 3a20 6e64 6172 7261 790a   grad : ndarray.
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052e0: 4e65 6761 7469 7665 206c 6f67 6c69 6b65  Negative loglike
+000052f0: 6c69 686f 6f64 2063 6f73 7420 6675 6e63  lihood cost func
+00005300: 7469 6f6e 2067 7261 6469 656e 7420 6672  tion gradient fr
+00005310: 6f6d 0a20 2020 2020 2020 2020 2020 2020  om.             
+00005320: 2020 2073 6369 7079 2e6f 7074 696d 697a     scipy.optimiz
+00005330: 652e 6d69 6e69 6d69 7a65 2042 4647 5320  e.minimize BFGS 
+00005340: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+00005350: 2020 2020 6865 7373 6961 6e20 3a20 6e64      hessian : nd
+00005360: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
+00005370: 2020 2020 2020 4e65 6761 7469 7665 206c        Negative l
+00005380: 6f67 6c69 6b65 6c69 686f 6f64 2063 6f73  oglikelihood cos
+00005390: 7420 6675 6e63 7469 6f6e 2068 6573 7369  t function hessi
+000053a0: 616e 2066 726f 6d0a 2020 2020 2020 2020  an from.        
+000053b0: 2020 2020 2020 2020 7363 6970 792e 6f70          scipy.op
+000053c0: 7469 6d69 7a65 2e6d 696e 696d 697a 6520  timize.minimize 
+000053d0: 4246 4753 206d 6574 686f 642e 0a20 2020  BFGS method..   
+000053e0: 2022 2222 0a20 2020 206e 2c20 6d20 3d20   """.    n, m = 
+000053f0: 782e 7368 6170 650a 0a20 2020 2023 2050  x.shape..    # P
+00005400: 6172 7365 2049 6e70 7574 730a 2020 2020  arse Inputs.    
+00005410: 6966 2022 7630 2220 696e 2070 6172 616d  if "v0" in param
+00005420: 3a0a 2020 2020 2020 2020 7630 203d 2070  :.        v0 = p
+00005430: 6172 616d 5b22 7630 225d 0a20 2020 2065  aram["v0"].    e
+00005440: 6c73 653a 0a20 2020 2020 2020 2076 3020  lse:.        v0 
+00005450: 3d20 6e70 2e6d 6561 6e28 6e70 2e76 6172  = np.mean(np.var
+00005460: 2878 2c20 3129 2920 2a20 6e70 2e61 7272  (x, 1)) * np.arr
+00005470: 6179 285b 312c 2031 2c20 315d 290a 2020  ay([1, 1, 1]).  
+00005480: 2020 2020 2020 7061 7261 6d5b 2276 3022        param["v0"
+00005490: 5d20 3d20 7630 0a0a 2020 2020 6966 2022  ] = v0..    if "
+000054a0: 6d75 3022 2069 6e20 7061 7261 6d3a 0a20  mu0" in param:. 
+000054b0: 2020 2020 2020 206d 7530 203d 2070 6172         mu0 = par
+000054c0: 616d 5b22 6d75 3022 5d0a 2020 2020 656c  am["mu0"].    el
+000054d0: 7365 3a0a 2020 2020 2020 2020 6d75 3020  se:.        mu0 
+000054e0: 3d20 6e70 2e6d 6561 6e28 782c 2031 290a  = np.mean(x, 1).
+000054f0: 2020 2020 2020 2020 7061 7261 6d5b 226d          param["m
+00005500: 7530 225d 203d 206d 7530 0a0a 2020 2020  u0"] = mu0..    
+00005510: 6966 2022 6130 2220 696e 2070 6172 616d  if "a0" in param
+00005520: 3a0a 2020 2020 2020 2020 6130 203d 2070  :.        a0 = p
+00005530: 6172 616d 5b22 6130 225d 0a20 2020 2065  aram["a0"].    e
+00005540: 6c73 653a 0a20 2020 2020 2020 2061 3020  lse:.        a0 
+00005550: 3d20 6e70 2e6f 6e65 7328 6d29 0a20 2020  = np.ones(m).   
+00005560: 2020 2020 2070 6172 616d 5b22 6130 225d       param["a0"]
+00005570: 203d 2061 300a 0a20 2020 2069 6620 2265   = a0..    if "e
+00005580: 7461 3022 2069 6e20 7061 7261 6d3a 0a20  ta0" in param:. 
+00005590: 2020 2020 2020 2065 7461 3020 3d20 7061         eta0 = pa
+000055a0: 7261 6d5b 2265 7461 3022 5d0a 2020 2020  ram["eta0"].    
+000055b0: 656c 7365 3a0a 2020 2020 2020 2020 6574  else:.        et
+000055c0: 6130 203d 206e 702e 7a65 726f 7328 6d29  a0 = np.zeros(m)
+000055d0: 0a20 2020 2020 2020 2070 6172 616d 5b22  .        param["
+000055e0: 6574 6130 225d 203d 2065 7461 300a 0a20  eta0"] = eta0.. 
+000055f0: 2020 2069 6620 2274 7322 2069 6e20 7061     if "ts" in pa
+00005600: 7261 6d3a 0a20 2020 2020 2020 2070 6172  ram:.        par
+00005610: 616d 5b22 7473 225d 0a20 2020 2065 6c73  am["ts"].    els
+00005620: 653a 0a20 2020 2020 2020 2070 6172 616d  e:.        param
+00005630: 5b22 7473 225d 203d 2031 0a0a 2020 2020  ["ts"] = 1..    
+00005640: 6d6c 6520 3d20 7b22 7830 223a 206e 702e  mle = {"x0": np.
+00005650: 6172 7261 7928 5b5d 297d 0a20 2020 2069  array([])}.    i
+00005660: 6478 7374 6172 7420 3d20 300a 2020 2020  dxstart = 0.    
+00005670: 6964 7872 616e 6765 203d 207b 7d0a 0a20  idxrange = {}.. 
+00005680: 2020 2023 2049 6620 6669 785b 276c 6f67     # If fix['log
+00005690: 7627 5d2c 2072 6574 7572 6e20 6c6f 6728  v'], return log(
+000056a0: 7630 293b 206f 7468 6572 7769 7365 2072  v0); otherwise r
+000056b0: 6574 7572 6e20 6c6f 6776 2070 6172 616d  eturn logv param
+000056c0: 6574 6572 730a 2020 2020 6966 2066 6978  eters.    if fix
+000056d0: 5b22 6c6f 6776 225d 3a0a 0a20 2020 2020  ["logv"]:..     
+000056e0: 2020 2064 6566 2073 6574 706c 6f67 7628     def setplogv(
+000056f0: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
+00005700: 7265 7475 726e 206e 702e 6c6f 6728 7061  return np.log(pa
+00005710: 7261 6d5b 2276 3022 5d29 0a0a 2020 2020  ram["v0"])..    
+00005720: 656c 7365 3a0a 2020 2020 2020 2020 6d6c  else:.        ml
+00005730: 655b 2278 3022 5d20 3d20 6e70 2e63 6f6e  e["x0"] = np.con
+00005740: 6361 7465 6e61 7465 2828 6d6c 655b 2278  catenate((mle["x
+00005750: 3022 5d2c 206e 702e 6c6f 6728 7061 7261  0"], np.log(para
+00005760: 6d5b 2276 3022 5d29 2929 0a20 2020 2020  m["v0"]))).     
+00005770: 2020 2069 6478 656e 6420 3d20 6964 7873     idxend = idxs
+00005780: 7461 7274 202b 2033 0a20 2020 2020 2020  tart + 3.       
+00005790: 2069 6478 7261 6e67 655b 226c 6f67 7622   idxrange["logv"
+000057a0: 5d20 3d20 6e70 2e61 7261 6e67 6528 6964  ] = np.arange(id
+000057b0: 7873 7461 7274 2c20 6964 7865 6e64 290a  xstart, idxend).
+000057c0: 0a20 2020 2020 2020 2064 6566 2073 6574  .        def set
+000057d0: 706c 6f67 7628 5f70 293a 0a20 2020 2020  plogv(_p):.     
+000057e0: 2020 2020 2020 2072 6574 7572 6e20 5f70         return _p
+000057f0: 5b69 6478 7261 6e67 655b 226c 6f67 7622  [idxrange["logv"
+00005800: 5d5d 0a0a 2020 2020 2020 2020 6964 7873  ]]..        idxs
+00005810: 7461 7274 203d 2069 6478 656e 640a 2020  tart = idxend.  
+00005820: 2020 7061 7373 0a0a 2020 2020 2320 4966    pass..    # If
+00005830: 2046 6978 5b27 6d75 275d 2c20 7265 7475   Fix['mu'], retu
+00005840: 726e 206d 7530 2c20 6f74 6865 7277 6973  rn mu0, otherwis
+00005850: 652c 2072 6574 7572 6e20 6d75 2070 6172  e, return mu par
+00005860: 616d 6574 6572 730a 2020 2020 6966 2066  ameters.    if f
+00005870: 6978 5b22 6d75 225d 3a0a 0a20 2020 2020  ix["mu"]:..     
+00005880: 2020 2064 6566 2073 6574 706d 7528 5f29     def setpmu(_)
+00005890: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000058a0: 7475 726e 2070 6172 616d 5b22 6d75 3022  turn param["mu0"
+000058b0: 5d0a 0a20 2020 2065 6c73 653a 0a20 2020  ]..    else:.   
+000058c0: 2020 2020 206d 6c65 5b22 7830 225d 203d       mle["x0"] =
+000058d0: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
+000058e0: 286d 6c65 5b22 7830 225d 2c20 7061 7261  (mle["x0"], para
+000058f0: 6d5b 226d 7530 225d 2929 0a20 2020 2020  m["mu0"])).     
+00005900: 2020 2069 6478 656e 6420 3d20 6964 7873     idxend = idxs
+00005910: 7461 7274 202b 206e 0a20 2020 2020 2020  tart + n.       
+00005920: 2069 6478 7261 6e67 655b 226d 7522 5d20   idxrange["mu"] 
+00005930: 3d20 6e70 2e61 7261 6e67 6528 6964 7873  = np.arange(idxs
+00005940: 7461 7274 2c20 6964 7865 6e64 290a 0a20  tart, idxend).. 
+00005950: 2020 2020 2020 2064 6566 2073 6574 706d         def setpm
+00005960: 7528 5f70 293a 0a20 2020 2020 2020 2020  u(_p):.         
+00005970: 2020 2072 6574 7572 6e20 5f70 5b69 6478     return _p[idx
+00005980: 7261 6e67 655b 226d 7522 5d5d 0a0a 2020  range["mu"]]..  
+00005990: 2020 2020 2020 6964 7873 7461 7274 203d        idxstart =
+000059a0: 2069 6478 656e 640a 2020 2020 7061 7373   idxend.    pass
+000059b0: 0a0a 2020 2020 2320 4966 2069 676e 6f72  ..    # If ignor
+000059c0: 6520 412c 2072 6574 7572 6e20 5b5d 3b20  e A, return []; 
+000059d0: 6966 2046 6978 5b27 4127 5d2c 2072 6574  if Fix['A'], ret
+000059e0: 7572 6e20 4130 3b20 6966 207e 4669 782e  urn A0; if ~Fix.
+000059f0: 4120 2620 4669 782e 6d75 2c0a 2020 2020  A & Fix.mu,.    
+00005a00: 2320 7265 7475 726e 2061 6c6c 2041 2070  # return all A p
+00005a10: 6172 616d 6574 6572 733b 0a20 2020 2023  arameters;.    #
+00005a20: 2049 6620 7e46 6978 2e41 2026 207e 4669   If ~Fix.A & ~Fi
+00005a30: 782e 6d75 2c20 7265 7475 726e 2061 6c6c  x.mu, return all
+00005a40: 2041 2070 6172 616d 6574 6572 7320 6275   A parameters bu
+00005a50: 7420 6669 7273 740a 0a20 2020 2069 6620  t first..    if 
+00005a60: 6967 6e6f 7265 5b22 6122 5d3a 0a0a 2020  ignore["a"]:..  
+00005a70: 2020 2020 2020 6465 6620 7365 7470 6128        def setpa(
+00005a80: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
+00005a90: 7265 7475 726e 205b 5d0a 0a20 2020 2065  return []..    e
+00005aa0: 6c69 6620 6669 785b 2261 225d 3a0a 0a20  lif fix["a"]:.. 
+00005ab0: 2020 2020 2020 2064 6566 2073 6574 7061         def setpa
+00005ac0: 285f 293a 0a20 2020 2020 2020 2020 2020  (_):.           
+00005ad0: 2072 6574 7572 6e20 7061 7261 6d5b 2261   return param["a
+00005ae0: 3022 5d0a 0a20 2020 2065 6c69 6620 6669  0"]..    elif fi
+00005af0: 785b 226d 7522 5d3a 0a20 2020 2020 2020  x["mu"]:.       
+00005b00: 206d 6c65 5b22 7830 225d 203d 206e 702e   mle["x0"] = np.
+00005b10: 636f 6e63 6174 656e 6174 6528 286d 6c65  concatenate((mle
+00005b20: 5b22 7830 225d 2c20 7061 7261 6d5b 2261  ["x0"], param["a
+00005b30: 3022 5d29 290a 2020 2020 2020 2020 6964  0"])).        id
+00005b40: 7865 6e64 203d 2069 6478 7374 6172 7420  xend = idxstart 
+00005b50: 2b20 6d0a 2020 2020 2020 2020 6964 7872  + m.        idxr
+00005b60: 616e 6765 5b22 6122 5d20 3d20 6e70 2e61  ange["a"] = np.a
+00005b70: 7261 6e67 6528 6964 7873 7461 7274 2c20  range(idxstart, 
+00005b80: 6964 7865 6e64 290a 0a20 2020 2020 2020  idxend)..       
+00005b90: 2064 6566 2073 6574 7061 285f 7029 3a0a   def setpa(_p):.
+00005ba0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005bb0: 726e 205f 705b 6964 7872 616e 6765 5b22  rn _p[idxrange["
+00005bc0: 6122 5d5d 0a0a 2020 2020 2020 2020 6964  a"]]..        id
+00005bd0: 7873 7461 7274 203d 2069 6478 656e 640a  xstart = idxend.
+00005be0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005bf0: 2020 6d6c 655b 2278 3022 5d20 3d20 6e70    mle["x0"] = np
+00005c00: 2e63 6f6e 6361 7465 6e61 7465 280a 2020  .concatenate(.  
+00005c10: 2020 2020 2020 2020 2020 286d 6c65 5b22            (mle["
+00005c20: 7830 225d 2c20 7061 7261 6d5b 2261 3022  x0"], param["a0"
+00005c30: 5d5b 313a 5d20 2f20 7061 7261 6d5b 2261  ][1:] / param["a
+00005c40: 3022 5d5b 305d 290a 2020 2020 2020 2020  0"][0]).        
+00005c50: 290a 2020 2020 2020 2020 6964 7865 6e64  ).        idxend
+00005c60: 203d 2069 6478 7374 6172 7420 2b20 6d20   = idxstart + m 
+00005c70: 2d20 310a 2020 2020 2020 2020 6964 7872  - 1.        idxr
+00005c80: 616e 6765 5b22 6122 5d20 3d20 6e70 2e61  ange["a"] = np.a
+00005c90: 7261 6e67 6528 6964 7873 7461 7274 2c20  range(idxstart, 
+00005ca0: 6964 7865 6e64 290a 0a20 2020 2020 2020  idxend)..       
+00005cb0: 2064 6566 2073 6574 7061 285f 7029 3a0a   def setpa(_p):.
+00005cc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005cd0: 726e 206e 702e 636f 6e63 6174 656e 6174  rn np.concatenat
+00005ce0: 6528 285b 315d 2c20 5f70 5b69 6478 7261  e(([1], _p[idxra
+00005cf0: 6e67 655b 2261 225d 5d29 2c20 6178 6973  nge["a"]]), axis
+00005d00: 3d30 290a 0a20 2020 2020 2020 2069 6478  =0)..        idx
+00005d10: 7374 6172 7420 3d20 6964 7865 6e64 0a20  start = idxend. 
+00005d20: 2020 2070 6173 730a 0a20 2020 2023 2049     pass..    # I
+00005d30: 6620 4967 6e6f 7265 2e65 7461 2c20 7265  f Ignore.eta, re
+00005d40: 7475 726e 205b 5d3b 2069 6620 4669 782e  turn []; if Fix.
+00005d50: 6574 612c 2072 6574 7572 6e20 6574 6130  eta, return eta0
+00005d60: 3b20 6966 207e 4669 782e 6574 6120 260a  ; if ~Fix.eta &.
+00005d70: 2020 2020 2320 4669 782e 6d75 2c72 6574      # Fix.mu,ret
+00005d80: 7572 6e20 616c 6c20 6574 6120 7061 7261  urn all eta para
+00005d90: 6d65 7465 7273 3b0a 2020 2020 2320 6966  meters;.    # if
+00005da0: 207e 4669 782e 6574 6120 2620 7e46 6978   ~Fix.eta & ~Fix
+00005db0: 2e6d 752c 2072 6574 7572 6e20 616c 6c20  .mu, return all 
+00005dc0: 6574 6120 7061 7261 6d65 7465 7273 2062  eta parameters b
+00005dd0: 7574 2066 6972 7374 0a0a 2020 2020 6966  ut first..    if
+00005de0: 2069 676e 6f72 655b 2265 7461 225d 3a0a   ignore["eta"]:.
+00005df0: 0a20 2020 2020 2020 2064 6566 2073 6574  .        def set
+00005e00: 7065 7461 285f 293a 0a20 2020 2020 2020  peta(_):.       
+00005e10: 2020 2020 2072 6574 7572 6e20 5b5d 0a0a       return []..
+00005e20: 2020 2020 656c 6966 2066 6978 5b22 6574      elif fix["et
+00005e30: 6122 5d3a 0a0a 2020 2020 2020 2020 6465  a"]:..        de
+00005e40: 6620 7365 7470 6574 6128 5f29 3a0a 2020  f setpeta(_):.  
+00005e50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00005e60: 2070 6172 616d 5b22 6574 6130 225d 0a0a   param["eta0"]..
+00005e70: 2020 2020 656c 6966 2066 6978 5b22 6d75      elif fix["mu
+00005e80: 225d 3a0a 2020 2020 2020 2020 6d6c 655b  "]:.        mle[
+00005e90: 2278 3022 5d20 3d20 6e70 2e63 6f6e 6361  "x0"] = np.conca
+00005ea0: 7465 6e61 7465 2828 6d6c 655b 2278 3022  tenate((mle["x0"
+00005eb0: 5d2c 2070 6172 616d 5b22 6574 6130 225d  ], param["eta0"]
+00005ec0: 2929 0a20 2020 2020 2020 2069 6478 656e  )).        idxen
+00005ed0: 6420 3d20 6964 7873 7461 7274 202b 206d  d = idxstart + m
+00005ee0: 0a20 2020 2020 2020 2069 6478 7261 6e67  .        idxrang
+00005ef0: 655b 2265 7461 225d 203d 206e 702e 6172  e["eta"] = np.ar
+00005f00: 616e 6765 2869 6478 7374 6172 742c 2069  ange(idxstart, i
+00005f10: 6478 656e 6429 0a0a 2020 2020 2020 2020  dxend)..        
+00005f20: 6465 6620 7365 7470 6574 6128 5f70 293a  def setpeta(_p):
+00005f30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00005f40: 7572 6e20 5f70 5b69 6478 7261 6e67 655b  urn _p[idxrange[
+00005f50: 2265 7461 225d 5d0a 0a20 2020 2065 6c73  "eta"]]..    els
+00005f60: 653a 0a20 2020 2020 2020 206d 6c65 5b22  e:.        mle["
+00005f70: 7830 225d 203d 206e 702e 636f 6e63 6174  x0"] = np.concat
+00005f80: 656e 6174 6528 0a20 2020 2020 2020 2020  enate(.         
+00005f90: 2020 2028 6d6c 655b 2278 3022 5d2c 2070     (mle["x0"], p
+00005fa0: 6172 616d 5b22 6574 6130 225d 5b31 3a5d  aram["eta0"][1:]
+00005fb0: 202d 2070 6172 616d 5b22 6574 6130 225d   - param["eta0"]
+00005fc0: 5b30 5d29 0a20 2020 2020 2020 2029 0a20  [0]).        ). 
+00005fd0: 2020 2020 2020 2069 6478 656e 6420 3d20         idxend = 
+00005fe0: 6964 7873 7461 7274 202b 206d 202d 2031  idxstart + m - 1
+00005ff0: 0a20 2020 2020 2020 2069 6478 7261 6e67  .        idxrang
+00006000: 655b 2265 7461 225d 203d 206e 702e 6172  e["eta"] = np.ar
+00006010: 616e 6765 2869 6478 7374 6172 742c 2069  ange(idxstart, i
+00006020: 6478 656e 6429 0a0a 2020 2020 2020 2020  dxend)..        
+00006030: 6465 6620 7365 7470 6574 6128 5f70 293a  def setpeta(_p):
+00006040: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006050: 7572 6e20 6e70 2e63 6f6e 6361 7465 6e61  urn np.concatena
+00006060: 7465 2828 5b30 5d2c 205f 705b 6964 7872  te(([0], _p[idxr
+00006070: 616e 6765 5b22 6574 6122 5d5d 292c 2061  ange["eta"]]), a
+00006080: 7869 733d 3029 0a0a 2020 2020 7061 7373  xis=0)..    pass
+00006090: 0a0a 2020 2020 6465 6620 6675 6e28 5f2c  ..    def fun(_,
+000060a0: 205f 7729 3a0a 2020 2020 2020 2020 7265   _w):.        re
+000060b0: 7475 726e 202d 316a 202a 205f 770a 0a20  turn -1j * _w.. 
+000060c0: 2020 2064 203d 2074 6474 6628 6675 6e2c     d = tdtf(fun,
+000060d0: 2030 2c20 6e2c 2070 6172 616d 5b22 7473   0, n, param["ts
+000060e0: 225d 290a 0a20 2020 2064 6566 2070 6172  "])..    def par
+000060f0: 7365 696e 285f 7029 3a0a 2020 2020 2020  sein(_p):.      
+00006100: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
+00006110: 2020 2020 2020 2022 6c6f 6776 223a 2073         "logv": s
+00006120: 6574 706c 6f67 7628 5f70 292c 0a20 2020  etplogv(_p),.   
+00006130: 2020 2020 2020 2020 2022 6d75 223a 2073           "mu": s
+00006140: 6574 706d 7528 5f70 292c 0a20 2020 2020  etpmu(_p),.     
+00006150: 2020 2020 2020 2022 6122 3a20 7365 7470         "a": setp
+00006160: 6128 5f70 292c 0a20 2020 2020 2020 2020  a(_p),.         
+00006170: 2020 2022 6574 6122 3a20 7365 7470 6574     "eta": setpet
+00006180: 6128 5f70 292c 0a20 2020 2020 2020 2020  a(_p),.         
+00006190: 2020 2022 7473 223a 2070 6172 616d 5b22     "ts": param["
+000061a0: 7473 225d 2c0a 2020 2020 2020 2020 2020  ts"],.          
+000061b0: 2020 2264 223a 2064 2c0a 2020 2020 2020    "d": d,.      
+000061c0: 2020 7d0a 0a20 2020 2064 6566 206f 626a    }..    def obj
+000061d0: 6563 7469 7665 285f 7029 3a0a 2020 2020  ective(_p):.    
+000061e0: 2020 2020 7265 7475 726e 2074 646e 6c6c      return tdnll
+000061f0: 2878 2c20 7061 7273 6569 6e28 5f70 292c  (x, parsein(_p),
+00006200: 2066 6978 295b 305d 0a0a 2020 2020 6465   fix)[0]..    de
+00006210: 6620 6a61 636f 6269 616e 285f 7029 3a0a  f jacobian(_p):.
+00006220: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00006230: 646e 6c6c 2878 2c20 7061 7273 6569 6e28  dnll(x, parsein(
+00006240: 5f70 292c 2066 6978 295b 315d 0a0a 2020  _p), fix)[1]..  
+00006250: 2020 6d6c 655b 226f 626a 6563 7469 7665    mle["objective
+00006260: 225d 203d 206f 626a 6563 7469 7665 0a20  "] = objective. 
+00006270: 2020 206f 7574 203d 206d 696e 696d 697a     out = minimiz
+00006280: 6528 6d6c 655b 226f 626a 6563 7469 7665  e(mle["objective
+00006290: 225d 2c20 6d6c 655b 2278 3022 5d2c 206d  "], mle["x0"], m
+000062a0: 6574 686f 643d 2242 4647 5322 2c20 6a61  ethod="BFGS", ja
+000062b0: 633d 6a61 636f 6269 616e 290a 0a20 2020  c=jacobian)..   
+000062c0: 2023 2054 6865 2074 7275 7374 2d72 6567   # The trust-reg
+000062d0: 696f 6e20 616c 676f 7269 7468 6d20 7265  ion algorithm re
+000062e0: 7475 726e 7320 7468 6520 4865 7373 6961  turns the Hessia
+000062f0: 6e20 666f 7220 7468 6520 6e65 7874 2d74  n for the next-t
+00006300: 6f2d 6c61 7374 0a20 2020 2023 2069 7465  o-last.    # ite
+00006310: 7261 7465 2c20 7768 6963 6820 6d61 7920  rate, which may 
+00006320: 6e6f 7420 6265 206e 6561 7220 7468 6520  not be near the 
+00006330: 6669 6e61 6c20 706f 696e 742e 2054 6f20  final point. To 
+00006340: 6368 6563 6b2c 2074 6573 7420 666f 720a  check, test for.
+00006350: 2020 2020 2320 706f 7369 7469 7665 2064      # positive d
+00006360: 6566 696e 6974 656e 6573 7320 6279 2061  efiniteness by a
+00006370: 7474 656d 7074 696e 6720 746f 2043 686f  ttempting to Cho
+00006380: 6c65 736b 7920 6661 6374 6f72 697a 6520  lesky factorize 
+00006390: 6974 2e20 4966 2069 740a 2020 2020 2320  it. If it.    # 
+000063a0: 7265 7475 726e 7320 616e 2065 7272 6f72  returns an error
+000063b0: 2c20 7265 7275 6e20 7468 6520 6f70 7469  , rerun the opti
+000063c0: 6d69 7a61 7469 6f6e 2077 6974 6820 7468  mization with th
+000063d0: 6520 7175 6173 692d 4e65 7774 6f6e 2061  e quasi-Newton a
+000063e0: 6c67 6f72 6974 686d 0a20 2020 2023 2066  lgorithm.    # f
+000063f0: 726f 6d20 7468 6520 6375 7272 656e 7420  rom the current 
+00006400: 6f70 7469 6d61 6c20 706f 696e 742e 0a0a  optimal point...
+00006410: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00006420: 206e 702e 6c69 6e61 6c67 2e63 686f 6c65   np.linalg.chole
+00006430: 736b 7928 6e70 2e6c 696e 616c 672e 696e  sky(np.linalg.in
+00006440: 7628 6f75 742e 6865 7373 5f69 6e76 2929  v(out.hess_inv))
+00006450: 0a20 2020 2020 2020 2068 6573 7320 3d20  .        hess = 
+00006460: 6e70 2e6c 696e 616c 672e 696e 7628 6f75  np.linalg.inv(ou
+00006470: 742e 6865 7373 5f69 6e76 290a 2020 2020  t.hess_inv).    
+00006480: 6578 6365 7074 206e 702e 6c69 6e61 6c67  except np.linalg
+00006490: 2e4c 696e 416c 6745 7272 6f72 3a0a 2020  .LinAlgError:.  
+000064a0: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
+000064b0: 2020 2020 2020 2020 2022 4865 7373 6961           "Hessia
+000064c0: 6e20 7265 7475 726e 6564 2062 7920 464d  n returned by FM
+000064d0: 494e 554e 4320 6973 206e 6f74 2070 6f73  INUNC is not pos
+000064e0: 6974 6976 6520 6465 6669 6e69 7465 3b5c  itive definite;\
+000064f0: 6e22 0a20 2020 2020 2020 2020 2020 2022  n".            "
+00006500: 7265 6361 6c63 756c 6174 696e 6720 7769  recalculating wi
+00006510: 7468 2071 7561 7369 2d4e 6577 746f 6e20  th quasi-Newton 
+00006520: 616c 676f 7269 7468 6d22 0a20 2020 2020  algorithm".     
+00006530: 2020 2029 0a0a 2020 2020 2020 2020 6d6c     )..        ml
+00006540: 655b 2278 3022 5d20 3d20 6f75 742e 780a  e["x0"] = out.x.
+00006550: 2020 2020 2020 2020 6f75 7432 203d 206d          out2 = m
+00006560: 696e 696d 697a 6528 0a20 2020 2020 2020  inimize(.       
+00006570: 2020 2020 206d 6c65 5b22 6f62 6a65 6374       mle["object
+00006580: 6976 6522 5d2c 206d 6c65 5b22 7830 225d  ive"], mle["x0"]
+00006590: 2c20 6d65 7468 6f64 3d22 4246 4753 222c  , method="BFGS",
+000065a0: 206a 6163 3d6a 6163 6f62 6961 6e0a 2020   jac=jacobian.  
+000065b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000065c0: 6865 7373 203d 206e 702e 6c69 6e61 6c67  hess = np.linalg
+000065d0: 2e69 6e76 286f 7574 322e 6865 7373 5f69  .inv(out2.hess_i
+000065e0: 6e76 290a 0a20 2020 2023 2050 6172 7365  nv)..    # Parse
+000065f0: 206f 7574 7075 740a 2020 2020 7020 3d20   output.    p = 
+00006600: 7b7d 0a20 2020 2069 6478 7261 6e67 6520  {}.    idxrange 
+00006610: 3d20 7b7d 0a20 2020 2069 6478 7374 6172  = {}.    idxstar
+00006620: 7420 3d20 300a 0a20 2020 2069 6620 6669  t = 0..    if fi
+00006630: 785b 226c 6f67 7622 5d3a 0a20 2020 2020  x["logv"]:.     
+00006640: 2020 2070 5b22 7661 7222 5d20 3d20 7061     p["var"] = pa
+00006650: 7261 6d5b 2276 3022 5d0a 2020 2020 656c  ram["v0"].    el
+00006660: 7365 3a0a 2020 2020 2020 2020 6964 7865  se:.        idxe
+00006670: 6e64 203d 2069 6478 7374 6172 7420 2b20  nd = idxstart + 
+00006680: 330a 2020 2020 2020 2020 6964 7872 616e  3.        idxran
+00006690: 6765 5b22 6c6f 6776 225d 203d 206e 702e  ge["logv"] = np.
+000066a0: 6172 616e 6765 2869 6478 7374 6172 742c  arange(idxstart,
+000066b0: 2069 6478 656e 6429 0a20 2020 2020 2020   idxend).       
+000066c0: 2069 6478 7374 6172 7420 3d20 6964 7865   idxstart = idxe
+000066d0: 6e64 0a20 2020 2020 2020 2070 5b22 7661  nd.        p["va
+000066e0: 7222 5d20 3d20 6e70 2e65 7870 286f 7574  r"] = np.exp(out
+000066f0: 2e78 5b69 6478 7261 6e67 655b 226c 6f67  .x[idxrange["log
+00006700: 7622 5d5d 290a 2020 2020 7061 7373 0a0a  v"]]).    pass..
+00006710: 2020 2020 6966 2066 6978 5b22 6d75 225d      if fix["mu"]
+00006720: 3a0a 2020 2020 2020 2020 705b 226d 7522  :.        p["mu"
+00006730: 5d20 3d20 7061 7261 6d5b 226d 7530 225d  ] = param["mu0"]
+00006740: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00006750: 2020 2069 6478 656e 6420 3d20 6964 7873     idxend = idxs
+00006760: 7461 7274 202b 206e 0a20 2020 2020 2020  tart + n.       
+00006770: 2069 6478 7261 6e67 655b 226d 7522 5d20   idxrange["mu"] 
+00006780: 3d20 6e70 2e61 7261 6e67 6528 6964 7873  = np.arange(idxs
+00006790: 7461 7274 2c20 6964 7865 6e64 290a 2020  tart, idxend).  
+000067a0: 2020 2020 2020 6964 7873 7461 7274 203d        idxstart =
+000067b0: 2069 6478 656e 640a 2020 2020 2020 2020   idxend.        
+000067c0: 705b 226d 7522 5d20 3d20 6f75 742e 785b  p["mu"] = out.x[
+000067d0: 6964 7872 616e 6765 5b22 6d75 225d 5d0a  idxrange["mu"]].
+000067e0: 2020 2020 7061 7373 0a0a 2020 2020 6966      pass..    if
+000067f0: 2069 676e 6f72 655b 2261 225d 206f 7220   ignore["a"] or 
+00006800: 6669 785b 2261 225d 3a0a 2020 2020 2020  fix["a"]:.      
+00006810: 2020 705b 2261 225d 203d 2070 6172 616d    p["a"] = param
+00006820: 5b22 6130 225d 0a20 2020 2065 6c69 6620  ["a0"].    elif 
+00006830: 6669 785b 226d 7522 5d3a 0a20 2020 2020  fix["mu"]:.     
+00006840: 2020 2069 6478 656e 6420 3d20 6964 7873     idxend = idxs
+00006850: 7461 7274 202b 206d 0a20 2020 2020 2020  tart + m.       
+00006860: 2069 6478 7261 6e67 655b 2261 225d 203d   idxrange["a"] =
+00006870: 206e 702e 6172 616e 6765 2869 6478 7374   np.arange(idxst
+00006880: 6172 742c 2069 6478 656e 6429 0a20 2020  art, idxend).   
+00006890: 2020 2020 2069 6478 7374 6172 7420 3d20       idxstart = 
+000068a0: 6964 7865 6e64 0a20 2020 2020 2020 2070  idxend.        p
+000068b0: 5b22 6122 5d20 3d20 6f75 742e 785b 6964  ["a"] = out.x[id
+000068c0: 7872 616e 6765 5b22 6122 5d5d 0a20 2020  xrange["a"]].   
+000068d0: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+000068e0: 6478 656e 6420 3d20 6964 7873 7461 7274  dxend = idxstart
+000068f0: 202b 206d 202d 2031 0a20 2020 2020 2020   + m - 1.       
+00006900: 2069 6478 7261 6e67 655b 2261 225d 203d   idxrange["a"] =
+00006910: 206e 702e 6172 616e 6765 2869 6478 7374   np.arange(idxst
+00006920: 6172 742c 2069 6478 656e 6429 0a20 2020  art, idxend).   
+00006930: 2020 2020 2069 6478 7374 6172 7420 3d20       idxstart = 
+00006940: 6964 7865 6e64 0a20 2020 2020 2020 2070  idxend.        p
+00006950: 5b22 6122 5d20 3d20 6e70 2e63 6f6e 6361  ["a"] = np.conca
+00006960: 7465 6e61 7465 2828 5b31 5d2c 206f 7574  tenate(([1], out
+00006970: 2e78 5b69 6478 7261 6e67 655b 2261 225d  .x[idxrange["a"]
+00006980: 5d29 2c20 6178 6973 3d30 290a 2020 2020  ]), axis=0).    
+00006990: 7061 7373 0a0a 2020 2020 6966 2069 676e  pass..    if ign
+000069a0: 6f72 655b 2265 7461 225d 206f 7220 6669  ore["eta"] or fi
+000069b0: 785b 2265 7461 225d 3a0a 2020 2020 2020  x["eta"]:.      
+000069c0: 2020 705b 2265 7461 225d 203d 2070 6172    p["eta"] = par
+000069d0: 616d 5b22 6574 6130 225d 0a20 2020 2065  am["eta0"].    e
+000069e0: 6c69 6620 6669 785b 226d 7522 5d3a 0a20  lif fix["mu"]:. 
+000069f0: 2020 2020 2020 2069 6478 656e 6420 3d20         idxend = 
+00006a00: 6964 7873 7461 7274 202b 206d 0a20 2020  idxstart + m.   
+00006a10: 2020 2020 2069 6478 7261 6e67 655b 2265       idxrange["e
+00006a20: 7461 225d 203d 206e 702e 6172 616e 6765  ta"] = np.arange
+00006a30: 2869 6478 7374 6172 742c 2069 6478 656e  (idxstart, idxen
+00006a40: 6429 0a20 2020 2020 2020 2070 5b22 6574  d).        p["et
+00006a50: 6122 5d20 3d20 6f75 742e 785b 6964 7872  a"] = out.x[idxr
+00006a60: 616e 6765 5b22 6574 6122 5d5d 0a20 2020  ange["eta"]].   
+00006a70: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+00006a80: 6478 656e 6420 3d20 6964 7873 7461 7274  dxend = idxstart
+00006a90: 202b 206d 202d 2031 0a20 2020 2020 2020   + m - 1.       
+00006aa0: 2069 6478 7261 6e67 655b 2265 7461 225d   idxrange["eta"]
+00006ab0: 203d 206e 702e 6172 616e 6765 2869 6478   = np.arange(idx
+00006ac0: 7374 6172 742c 2069 6478 656e 6429 0a20  start, idxend). 
+00006ad0: 2020 2020 2020 2070 5b22 6574 6122 5d20         p["eta"] 
+00006ae0: 3d20 6e70 2e63 6f6e 6361 7465 6e61 7465  = np.concatenate
+00006af0: 2828 5b30 5d2c 206f 7574 2e78 5b69 6478  (([0], out.x[idx
+00006b00: 7261 6e67 655b 2265 7461 225d 5d29 2c20  range["eta"]]), 
+00006b10: 6178 6973 3d30 290a 2020 2020 7061 7373  axis=0).    pass
+00006b20: 0a0a 2020 2020 705b 2274 7322 5d20 3d20  ..    p["ts"] = 
+00006b30: 7061 7261 6d5b 2274 7322 5d0a 0a20 2020  param["ts"]..   
+00006b40: 2076 6172 795f 7061 7261 6d20 3d20 6e70   vary_param = np
+00006b50: 2e6c 6f67 6963 616c 5f6e 6f74 280a 2020  .logical_not(.  
+00006b60: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00006b70: 2020 2020 6669 785b 226c 6f67 7622 5d2c      fix["logv"],
+00006b80: 0a20 2020 2020 2020 2020 2020 2066 6978  .            fix
+00006b90: 5b22 6d75 225d 2c0a 2020 2020 2020 2020  ["mu"],.        
+00006ba0: 2020 2020 6669 785b 2261 225d 206f 7220      fix["a"] or 
+00006bb0: 6967 6e6f 7265 5b22 6122 5d2c 0a20 2020  ignore["a"],.   
+00006bc0: 2020 2020 2020 2020 2066 6978 5b22 6574           fix["et
+00006bd0: 6122 5d20 6f72 2069 676e 6f72 655b 2265  a"] or ignore["e
+00006be0: 7461 225d 2c0a 2020 2020 2020 2020 5d0a  ta"],.        ].
+00006bf0: 2020 2020 290a 2020 2020 6469 6167 6e6f      ).    diagno
+00006c00: 7374 6963 203d 207b 0a20 2020 2020 2020  stic = {.       
+00006c10: 2022 6772 6164 223a 206f 7574 2e6a 6163   "grad": out.jac
+00006c20: 2c0a 2020 2020 2020 2020 2268 6573 7369  ,.        "hessi
+00006c30: 616e 223a 2068 6573 732c 0a20 2020 2020  an": hess,.     
+00006c40: 2020 2022 6572 7222 3a20 7b22 7661 7222     "err": {"var"
+00006c50: 3a20 5b5d 2c20 226d 7522 3a20 5b5d 2c20  : [], "mu": [], 
+00006c60: 2261 223a 205b 5d2c 2022 6574 6122 3a20  "a": [], "eta": 
+00006c70: 5b5d 7d2c 0a20 2020 207d 0a20 2020 2076  []},.    }.    v
+00006c80: 203d 206e 702e 646f 7428 6e70 2e65 7965   = np.dot(np.eye
+00006c90: 2868 6573 732e 7368 6170 655b 305d 292c  (hess.shape[0]),
+00006ca0: 2073 6369 7079 2e6c 696e 616c 672e 696e   scipy.linalg.in
+00006cb0: 7628 6865 7373 2929 0a20 2020 2065 7272  v(hess)).    err
+00006cc0: 203d 206e 702e 7371 7274 286e 702e 6469   = np.sqrt(np.di
+00006cd0: 6167 2876 2929 0a20 2020 2069 6478 7374  ag(v)).    idxst
+00006ce0: 6172 7420 3d20 300a 2020 2020 6966 2076  art = 0.    if v
+00006cf0: 6172 795f 7061 7261 6d5b 305d 3a0a 2020  ary_param[0]:.  
+00006d00: 2020 2020 2020 6469 6167 6e6f 7374 6963        diagnostic
+00006d10: 5b22 6572 7222 5d5b 2276 6172 225d 203d  ["err"]["var"] =
+00006d20: 206e 702e 7371 7274 280a 2020 2020 2020   np.sqrt(.      
+00006d30: 2020 2020 2020 6e70 2e64 6961 6728 6e70        np.diag(np
+00006d40: 2e64 6961 6728 705b 2276 6172 225d 2920  .diag(p["var"]) 
+00006d50: 2a20 765b 303a 332c 2030 3a33 5d29 202a  * v[0:3, 0:3]) *
+00006d60: 206e 702e 6469 6167 2870 5b22 7661 7222   np.diag(p["var"
+00006d70: 5d29 0a20 2020 2020 2020 2029 0a20 2020  ]).        ).   
+00006d80: 2020 2020 2069 6478 7374 6172 7420 3d20       idxstart = 
+00006d90: 6964 7873 7461 7274 202b 2033 0a20 2020  idxstart + 3.   
+00006da0: 2070 6173 730a 0a20 2020 2069 6620 7661   pass..    if va
+00006db0: 7279 5f70 6172 616d 5b31 5d3a 0a20 2020  ry_param[1]:.   
+00006dc0: 2020 2020 2064 6961 676e 6f73 7469 635b       diagnostic[
+00006dd0: 2265 7272 225d 5b22 6d75 225d 203d 2065  "err"]["mu"] = e
+00006de0: 7272 5b69 6478 7374 6172 743a 2069 6478  rr[idxstart: idx
+00006df0: 7374 6172 7420 2b20 6e5d 0a20 2020 2020  start + n].     
+00006e00: 2020 2069 6478 7374 6172 7420 3d20 6964     idxstart = id
+00006e10: 7873 7461 7274 202b 206e 0a20 2020 2070  xstart + n.    p
+00006e20: 6173 730a 0a20 2020 2069 6620 7661 7279  ass..    if vary
+00006e30: 5f70 6172 616d 5b32 5d3a 0a20 2020 2020  _param[2]:.     
+00006e40: 2020 2069 6620 7661 7279 5f70 6172 616d     if vary_param
+00006e50: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
+00006e60: 2064 6961 676e 6f73 7469 635b 2265 7272   diagnostic["err
+00006e70: 225d 5b22 6122 5d20 3d20 6572 725b 6964  "]["a"] = err[id
+00006e80: 7873 7461 7274 3a20 6964 7873 7461 7274  xstart: idxstart
+00006e90: 202b 206d 202d 2031 5d0a 2020 2020 2020   + m - 1].      
+00006ea0: 2020 2020 2020 6964 7873 7461 7274 203d        idxstart =
+00006eb0: 2069 6478 7374 6172 7420 2b20 6d20 2d20   idxstart + m - 
+00006ec0: 310a 2020 2020 2020 2020 656c 7365 3a0a  1.        else:.
+00006ed0: 2020 2020 2020 2020 2020 2020 6469 6167              diag
+00006ee0: 6e6f 7374 6963 5b22 6572 7222 5d5b 2261  nostic["err"]["a
+00006ef0: 225d 203d 2065 7272 5b69 6478 7374 6172  "] = err[idxstar
+00006f00: 743a 2069 6478 7374 6172 7420 2b20 6d5d  t: idxstart + m]
+00006f10: 0a20 2020 2020 2020 2020 2020 2069 6478  .            idx
+00006f20: 7374 6172 7420 3d20 6964 7873 7461 7274  start = idxstart
+00006f30: 202b 206d 0a20 2020 2070 6173 730a 0a20   + m.    pass.. 
+00006f40: 2020 2069 6620 7661 7279 5f70 6172 616d     if vary_param
+00006f50: 5b33 5d3a 0a20 2020 2020 2020 2069 6620  [3]:.        if 
+00006f60: 7661 7279 5f70 6172 616d 5b31 5d3a 0a20  vary_param[1]:. 
+00006f70: 2020 2020 2020 2020 2020 2064 6961 676e             diagn
+00006f80: 6f73 7469 635b 2265 7272 225d 5b22 6574  ostic["err"]["et
+00006f90: 6122 5d20 3d20 6572 725b 6964 7873 7461  a"] = err[idxsta
+00006fa0: 7274 3a20 6964 7873 7461 7274 202b 206d  rt: idxstart + m
+00006fb0: 202d 2031 5d0a 2020 2020 2020 2020 656c   - 1].        el
+00006fc0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006fd0: 6469 6167 6e6f 7374 6963 5b22 6572 7222  diagnostic["err"
+00006fe0: 5d5b 2265 7461 225d 203d 2065 7272 5b69  ]["eta"] = err[i
+00006ff0: 6478 7374 6172 743a 2069 6478 7374 6172  dxstart: idxstar
+00007000: 7420 2b20 6d5d 0a20 2020 2070 6173 730a  t + m].    pass.
+00007010: 0a20 2020 2072 6574 7572 6e20 5b70 2c20  .    return [p, 
+00007020: 6f75 742e 6675 6e2c 2064 6961 676e 6f73  out.fun, diagnos
+00007030: 7469 635d 0a                             tic].
```

### Comparing `thztools-0.0.2/.ruff_cache/content/c068bcc1830cc02` & `thztools-0.0.2.post0/src/thztools/_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,207 +1,179 @@
-00000000: 0100 0000 0000 0000 0e00 0000 0000 0000  ................
-00000010: 7468 7a74 6f6f 6c73 2e5f 7574 696c 0100  thztools._util..
-00000020: 0000 0000 0000 0500 0000 0000 0000 6e75  ..............nu
-00000030: 6d70 7900 0000 0012 0000 0002 0000 0000  mpy.............
-00000040: 0000 0022 0000 0000 0000 0041 6d62 6967  ...".......Ambig
-00000050: 756f 7573 556e 6963 6f64 6543 6861 7261  uousUnicodeChara
-00000060: 6374 6572 446f 6373 7472 696e 674e 0000  cterDocstringN..
-00000070: 0000 0000 0044 6f63 7374 7269 6e67 2063  .....Docstring c
-00000080: 6f6e 7461 696e 7320 616d 6269 6775 6f75  ontains ambiguou
-00000090: 7320 60e2 8093 6020 2845 4e20 4441 5348  s `...` (EN DASH
-000000a0: 292e 2044 6964 2079 6f75 206d 6561 6e20  ). Did you mean 
-000000b0: 602d 6020 2848 5950 4845 4e2d 4d49 4e55  `-` (HYPHEN-MINU
-000000c0: 5329 3f01 2f00 0000 0000 0000 5265 706c  S)?./.......Repl
-000000d0: 6163 6520 60e2 8093 6020 2845 4e20 4441  ace `...` (EN DA
-000000e0: 5348 2920 7769 7468 2060 2d60 2028 4859  SH) with `-` (HY
-000000f0: 5048 454e 2d4d 494e 5553 2953 0200 0056  PHEN-MINUS)S...V
-00000100: 0200 0001 0100 0000 0000 0000 5302 0000  ............S...
-00000110: 5602 0000 0101 0000 0000 0000 002d 0300  V............-..
-00000120: 0000 0000 0000 0000 0000 d702 0000 2200  ..............".
-00000130: 0000 0000 0000 416d 6269 6775 6f75 7355  ......AmbiguousU
-00000140: 6e69 636f 6465 4368 6172 6163 7465 7244  nicodeCharacterD
-00000150: 6f63 7374 7269 6e67 4e00 0000 0000 0000  ocstringN.......
-00000160: 446f 6373 7472 696e 6720 636f 6e74 6169  Docstring contai
-00000170: 6e73 2061 6d62 6967 756f 7573 2060 e280  ns ambiguous `..
-00000180: 9360 2028 454e 2044 4153 4829 2e20 4469  .` (EN DASH). Di
-00000190: 6420 796f 7520 6d65 616e 2060 2d60 2028  d you mean `-` (
-000001a0: 4859 5048 454e 2d4d 494e 5553 293f 012f  HYPHEN-MINUS)?./
-000001b0: 0000 0000 0000 0052 6570 6c61 6365 2060  .......Replace `
-000001c0: e280 9360 2028 454e 2044 4153 4829 2077  ...` (EN DASH) w
-000001d0: 6974 6820 602d 6020 2848 5950 4845 4e2d  ith `-` (HYPHEN-
-000001e0: 4d49 4e55 5329 8002 0000 8302 0000 0101  MINUS)..........
-000001f0: 0000 0000 0000 0080 0200 0083 0200 0001  ................
-00000200: 0100 0000 0000 0000 2d03 0000 0000 0000  ........-.......
-00000210: 0000 0000 00d7 0200 0001 0000 0000 0000  ................
-00000220: 0068 0000 0000 0000 002f 5573 6572 732f  .h......./Users/
-00000230: 6a73 642f 4c69 6272 6172 792f 436c 6f75  jsd/Library/Clou
-00000240: 6453 746f 7261 6765 2f4f 6e65 4472 6976  dStorage/OneDriv
-00000250: 652d 5369 6d6f 6e46 7261 7365 7255 6e69  e-SimonFraserUni
-00000260: 7665 7273 6974 7928 3173 6675 292f 7072  versity(1sfu)/pr
-00000270: 6f6a 6563 7473 2f74 687a 746f 6f6c 732f  ojects/thztools/
-00000280: 7468 7a74 6f6f 6c73 2f5f 7574 696c 2e70  thztools/_util.p
-00000290: 7957 0a00 0000 0000 0069 6d70 6f72 7420  yW.......import 
-000002a0: 6e75 6d70 7920 6173 206e 700a 0a0a 6465  numpy as np...de
-000002b0: 6620 6570 7377 6174 6572 2866 2c20 743d  f epswater(f, t=
-000002c0: 3235 293a 0a20 2020 2072 2222 2243 6f6d  25):.    r"""Com
-000002d0: 7075 7465 7320 7468 6520 636f 6d70 6c65  putes the comple
-000002e0: 7820 7265 6c61 7469 7665 2070 6572 6d69  x relative permi
-000002f0: 7474 6976 6974 7920 6f66 2077 6174 6572  ttivity of water
-00000300: 2e0a 0a20 2020 2052 6574 7572 6e73 2074  ...    Returns t
-00000310: 6865 2063 6f6d 706c 6578 2072 656c 6174  he complex relat
-00000320: 6976 6520 7065 726d 6974 7469 7669 7479  ive permittivity
-00000330: 2061 7420 6672 6571 7565 6e63 7920 6620   at frequency f 
-00000340: 2854 487a 2920 616e 640a 2020 2020 7465  (THz) and.    te
-00000350: 6d70 6572 6174 7572 6520 5420 2864 6567  mperature T (deg
-00000360: 2043 292e 2053 6565 205b 315d 5f20 666f   C). See [1]_ fo
-00000370: 7220 6465 7461 696c 732e 0a0a 2020 2020  r details...    
-00000380: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00000390: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6620  ---------.    f 
-000003a0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-000003b0: 4672 6571 7565 6e63 7920 2854 487a 290a  Frequency (THz).
-000003c0: 2020 2020 7420 3a20 666c 6f61 740a 2020      t : float.  
-000003d0: 2020 2020 2020 5465 6d70 6572 6174 7572        Temperatur
-000003e0: 6520 2864 6567 2043 2920 286f 7074 696f  e (deg C) (optio
-000003f0: 6e61 6c29 0a0a 2020 2020 5265 7475 726e  nal)..    Return
-00000400: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00000410: 2020 636f 6d70 6c65 780a 2020 2020 2020    complex.      
-00000420: 2020 436f 6d70 6c65 7820 7265 6c61 7469    Complex relati
-00000430: 7665 2070 6572 6d69 7474 6976 6974 7920  ve permittivity 
-00000440: 6f66 2077 6174 6572 2e0a 0a20 2020 2052  of water...    R
-00000450: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
-00000460: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
-00000470: 205b 315d 2045 6c6c 6973 6f6e 2c20 572e   [1] Ellison, W.
-00000480: 204a 2e20 2832 3030 3729 2e20 5065 726d   J. (2007). Perm
-00000490: 6974 7469 7669 7479 206f 6620 7075 7265  ittivity of pure
-000004a0: 2077 6174 6572 2c20 6174 2073 7461 6e64   water, at stand
-000004b0: 6172 640a 2020 2020 2020 2020 6174 6d6f  ard.        atmo
-000004c0: 7370 6865 7269 6320 7072 6573 7375 7265  spheric pressure
-000004d0: 2c20 6f76 6572 2074 6865 2066 7265 7175  , over the frequ
-000004e0: 656e 6379 2072 616e 6765 2030 e280 9332  ency range 0...2
-000004f0: 3520 5448 7a20 616e 6420 7468 650a 2020  5 THz and the.  
-00000500: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-00000510: 6520 7261 6e67 6520 30e2 8093 3130 3020  e range 0...100 
-00000520: 432e 204a 6f75 726e 616c 206f 6620 7068  C. Journal of ph
-00000530: 7973 6963 616c 2061 6e64 2063 6865 6d69  ysical and chemi
-00000540: 6361 6c20 7265 6665 7265 6e63 650a 2020  cal reference.  
-00000550: 2020 2020 2020 6461 7461 2c20 3336 2831        data, 36(1
-00000560: 292c 2031 2d31 382e 0a20 2020 2022 2222  ), 1-18..    """
-00000570: 0a20 2020 2023 2046 7265 7175 656e 6379  .    # Frequency
-00000580: 2063 6f6e 7665 7273 696f 6e20 746f 2048   conversion to H
-00000590: 7a0a 2020 2020 6620 3d20 6620 2a20 3165  z.    f = f * 1e
-000005a0: 3132 0a0a 2020 2020 2320 4465 6669 6e65  12..    # Define
-000005b0: 2072 656c 6178 6174 696f 6e20 7061 7261   relaxation para
-000005c0: 6d65 7465 7273 0a20 2020 2061 203d 206e  meters.    a = n
-000005d0: 702e 6172 7261 7928 5b37 392e 3233 3838  p.array([79.2388
-000005e0: 322c 2033 2e38 3135 3836 362c 2031 2e36  2, 3.815866, 1.6
-000005f0: 3334 3936 375d 290a 2020 2020 6220 3d20  34967]).    b = 
-00000600: 6e70 2e61 7272 6179 285b 302e 3030 3433  np.array([0.0043
-00000610: 3030 3539 382c 2030 2e30 3131 3137 3239  00598, 0.0111729
-00000620: 352c 2030 2e30 3036 3834 3135 3438 5d29  5, 0.006841548])
-00000630: 0a20 2020 2063 203d 206e 702e 6172 7261  .    c = np.arra
-00000640: 7928 5b31 2e33 3832 3236 3465 2d31 332c  y([1.382264e-13,
-00000650: 2033 2e35 3130 3335 3465 2d31 362c 2036   3.510354e-16, 6
-00000660: 2e33 3030 3335 652d 3135 5d29 0a20 2020  .30035e-15]).   
-00000670: 2064 203d 206e 702e 6172 7261 7928 5b36   d = np.array([6
-00000680: 3532 2e37 3634 382c 2031 3234 392e 3533  52.7648, 1249.53
-00000690: 332c 2034 3035 2e35 3136 395d 290a 2020  3, 405.5169]).  
-000006a0: 2020 7463 203d 2031 3333 2e31 3338 330a    tc = 133.1383.
-000006b0: 0a20 2020 2023 2044 6566 696e 6520 7265  .    # Define re
-000006c0: 736f 6e61 6e63 6520 7061 7261 6d65 7465  sonance paramete
-000006d0: 7273 0a20 2020 2070 3020 3d20 302e 3833  rs.    p0 = 0.83
-000006e0: 3739 3639 320a 2020 2020 7020 3d20 6e70  79692.    p = np
-000006f0: 2e61 7272 6179 285b 2d30 2e30 3036 3131  .array([-0.00611
-00000700: 3835 3934 2c20 2d30 2e30 3030 3031 3239  8594, -0.0000129
-00000710: 3336 3739 382c 2034 3233 3539 3031 3030  36798, 423590100
-00000720: 3030 3030 2c20 2d31 3432 3630 3838 3030  0000, -142608800
-00000730: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-00000740: 2020 2020 2020 3237 3338 3135 3730 302c        273815700,
-00000750: 202d 3132 3436 3934 332c 2039 2e36 3138   -1246943, 9.618
-00000760: 3634 3265 2d31 342c 2031 2e37 3935 3738  642e-14, 1.79578
-00000770: 3665 2d31 362c 0a20 2020 2020 2020 2020  6e-16,.         
-00000780: 2020 2020 2020 2020 202d 392e 3331 3030           -9.3100
-00000790: 3137 652d 3138 2c20 312e 3635 3534 3733  17e-18, 1.655473
-000007a0: 652d 3139 2c20 302e 3631 3635 3533 322c  e-19, 0.6165532,
-000007b0: 2030 2e30 3037 3233 3835 3332 2c0a 2020   0.007238532,.  
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2d30 2e30 3030 3039 3532 3333 3636 2c20  -0.00009523366, 
-000007e0: 3135 3938 3331 3730 3030 3030 3030 2c20  15983170000000, 
-000007f0: 2d37 3434 3133 3537 3030 3030 2c20 3439  -74413570000, 49
-00000800: 3734 3438 3030 302c 0a20 2020 2020 2020  7448000,.       
-00000810: 2020 2020 2020 2020 2020 2032 2e38 3832             2.882
-00000820: 3437 3665 2d31 342c 202d 332e 3134 3231  476e-14, -3.1421
-00000830: 3138 652d 3136 2c20 332e 3532 3830 3531  18e-16, 3.528051
-00000840: 652d 3138 5d29 0a0a 2020 2020 2320 436f  e-18])..    # Co
-00000850: 6d70 7574 6520 7465 6d70 6572 6174 7572  mpute temperatur
-00000860: 6520 2d20 6465 7065 6e64 656e 7420 6675  e - dependent fu
-00000870: 6e63 7469 6f6e 730a 2020 2020 6570 7330  nctions.    eps0
-00000880: 203d 2038 372e 3931 3434 202d 2030 2e34   = 87.9144 - 0.4
-00000890: 3034 3339 3920 2a20 7420 2b20 392e 3538  04399 * t + 9.58
-000008a0: 3732 3665 2d34 202a 2074 202a 2a20 3220  726e-4 * t ** 2 
-000008b0: 2d20 312e 3332 3830 3265 2d36 202a 2074  - 1.32802e-6 * t
-000008c0: 202a 2a20 330a 2020 2020 6465 6c74 6120   ** 3.    delta 
-000008d0: 3d20 6120 2a20 6e70 2e65 7870 282d 6220  = a * np.exp(-b 
-000008e0: 2a20 7429 0a20 2020 2074 6175 203d 2063  * t).    tau = c
-000008f0: 202a 206e 702e 6578 7028 6420 2f20 2874   * np.exp(d / (t
-00000900: 202b 2074 6329 290a 0a20 2020 2064 656c   + tc))..    del
-00000910: 7461 3420 3d20 7030 202b 2070 5b30 5d20  ta4 = p0 + p[0] 
-00000920: 2a20 7420 2b20 705b 315d 202a 2074 202a  * t + p[1] * t *
-00000930: 2a20 320a 2020 2020 6630 203d 2070 5b32  * 2.    f0 = p[2
-00000940: 5d20 2b20 705b 335d 202a 2074 202b 2070  ] + p[3] * t + p
-00000950: 5b34 5d20 2a20 7420 2a2a 2032 202b 2070  [4] * t ** 2 + p
-00000960: 5b35 5d20 2a20 7420 2a2a 2033 0a20 2020  [5] * t ** 3.   
-00000970: 2074 6175 3420 3d20 705b 365d 202b 2070   tau4 = p[6] + p
-00000980: 5b37 5d20 2a20 7420 2b20 705b 385d 202a  [7] * t + p[8] *
-00000990: 2074 202a 2a20 3220 2b20 705b 395d 202a   t ** 2 + p[9] *
-000009a0: 2074 202a 2a20 330a 2020 2020 6465 6c74   t ** 3.    delt
-000009b0: 6135 203d 2070 5b31 305d 202b 2070 5b31  a5 = p[10] + p[1
-000009c0: 315d 202a 2074 202b 2070 5b31 325d 202a  1] * t + p[12] *
-000009d0: 2074 202a 2a20 320a 2020 2020 6631 203d   t ** 2.    f1 =
-000009e0: 2070 5b31 335d 202b 2070 5b31 345d 202a   p[13] + p[14] *
-000009f0: 2074 202b 2070 5b31 355d 202a 2074 202a   t + p[15] * t *
-00000a00: 2a20 320a 2020 2020 7461 7535 203d 2070  * 2.    tau5 = p
-00000a10: 5b31 365d 202b 2070 5b31 375d 202a 2074  [16] + p[17] * t
-00000a20: 202b 2070 5b31 385d 202a 2074 202a 2a20   + p[18] * t ** 
-00000a30: 320a 0a20 2020 2023 2050 7574 2069 7420  2..    # Put it 
-00000a40: 616c 6c20 746f 6765 7468 6572 0a20 2020  all together.   
-00000a50: 2065 7073 696c 6f6e 7220 3d20 2865 7073   epsilonr = (eps
-00000a60: 3020 2b20 3220 2a20 316a 202a 206e 702e  0 + 2 * 1j * np.
-00000a70: 7069 202a 2066 0a20 2020 2020 2020 2020  pi * f.         
-00000a80: 2020 2020 2020 202a 2028 6465 6c74 615b         * (delta[
-00000a90: 305d 202a 2074 6175 5b30 5d20 2f0a 2020  0] * tau[0] /.  
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2028 3120 2d20 3220 2a20 316a 202a 206e   (1 - 2 * 1j * n
-00000ac0: 702e 7069 202a 2066 202a 2074 6175 5b30  p.pi * f * tau[0
-00000ad0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00000ae0: 2020 2020 2020 2b20 6465 6c74 615b 315d        + delta[1]
-00000af0: 202a 2074 6175 5b31 5d20 2f20 2831 202d   * tau[1] / (1 -
-00000b00: 2032 202a 2031 6a20 2a20 6e70 2e70 6920   2 * 1j * np.pi 
-00000b10: 2a20 6620 2a20 7461 755b 315d 290a 2020  * f * tau[1]).  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 202b 2064 656c 7461 5b32 5d20 2a20 7461   + delta[2] * ta
-00000b40: 755b 325d 202f 2028 3120 2d20 3220 2a20  u[2] / (1 - 2 * 
-00000b50: 316a 202a 206e 702e 7069 202a 2066 202a  1j * np.pi * f *
-00000b60: 2074 6175 5b32 5d29 290a 2020 2020 2020   tau[2])).      
-00000b70: 2020 2020 2020 2020 2020 2b20 316a 202a            + 1j *
-00000b80: 206e 702e 7069 202a 2066 0a20 2020 2020   np.pi * f.     
-00000b90: 2020 2020 2020 2020 2020 202a 2028 6465             * (de
-00000ba0: 6c74 6134 202a 2074 6175 3420 2f20 2831  lta4 * tau4 / (1
-00000bb0: 202d 2032 202a 2031 6a20 2a20 6e70 2e70   - 2 * 1j * np.p
-00000bc0: 6920 2a20 7461 7534 202a 2028 6630 202b  i * tau4 * (f0 +
-00000bd0: 2066 2929 0a20 2020 2020 2020 2020 2020   f)).           
-00000be0: 2020 2020 2020 2020 2b20 6465 6c74 6134          + delta4
-00000bf0: 202a 2074 6175 3420 2f20 2831 202b 2032   * tau4 / (1 + 2
-00000c00: 202a 2031 6a20 2a20 6e70 2e70 6920 2a20   * 1j * np.pi * 
-00000c10: 7461 7534 202a 2028 6630 202d 2066 2929  tau4 * (f0 - f))
-00000c20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00000c30: 2020 2b20 316a 202a 206e 702e 7069 202a    + 1j * np.pi *
-00000c40: 2066 0a20 2020 2020 2020 2020 2020 2020   f.             
-00000c50: 2020 202a 2028 6465 6c74 6135 202a 2074     * (delta5 * t
-00000c60: 6175 3520 2f20 2831 202d 2032 202a 2031  au5 / (1 - 2 * 1
-00000c70: 6a20 2a20 6e70 2e70 6920 2a20 7461 7535  j * np.pi * tau5
-00000c80: 202a 2028 6631 202b 2066 2929 0a20 2020   * (f1 + f)).   
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ca0: 2b20 6465 6c74 6135 202a 2074 6175 3520  + delta5 * tau5 
-00000cb0: 2f20 2831 202b 2032 202a 2031 6a20 2a20  / (1 + 2 * 1j * 
-00000cc0: 6e70 2e70 6920 2a20 7461 7535 202a 2028  np.pi * tau5 * (
-00000cd0: 6631 202d 2066 2929 2929 0a0a 2020 2020  f1 - f))))..    
-00000ce0: 7265 7475 726e 2065 7073 696c 6f6e 720a  return epsilonr.
+00000000: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+00000010: 6e70 0a0a 0a64 6566 2065 7073 7761 7465  np...def epswate
+00000020: 7228 662c 2074 3d32 3529 3a0a 2020 2020  r(f, t=25):.    
+00000030: 7222 2222 436f 6d70 7574 6573 2074 6865  r"""Computes the
+00000040: 2063 6f6d 706c 6578 2072 656c 6174 6976   complex relativ
+00000050: 6520 7065 726d 6974 7469 7669 7479 206f  e permittivity o
+00000060: 6620 7761 7465 722e 0a0a 2020 2020 5265  f water...    Re
+00000070: 7475 726e 7320 7468 6520 636f 6d70 6c65  turns the comple
+00000080: 7820 7265 6c61 7469 7665 2070 6572 6d69  x relative permi
+00000090: 7474 6976 6974 7920 6174 2066 7265 7175  ttivity at frequ
+000000a0: 656e 6379 2066 2028 5448 7a29 2061 6e64  ency f (THz) and
+000000b0: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
+000000c0: 2054 2028 6465 6720 4329 2e20 5365 6520   T (deg C). See 
+000000d0: 5b31 5d5f 2066 6f72 2064 6574 6169 6c73  [1]_ for details
+000000e0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+000000f0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00000100: 0a20 2020 2066 203a 2066 6c6f 6174 0a20  .    f : float. 
+00000110: 2020 2020 2020 2046 7265 7175 656e 6379         Frequency
+00000120: 2028 5448 7a29 0a20 2020 2074 203a 2066   (THz).    t : f
+00000130: 6c6f 6174 0a20 2020 2020 2020 2054 656d  loat.        Tem
+00000140: 7065 7261 7475 7265 2028 6465 6720 4329  perature (deg C)
+00000150: 2028 6f70 7469 6f6e 616c 290a 0a20 2020   (optional)..   
+00000160: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00000170: 2d2d 2d2d 0a20 2020 2063 6f6d 706c 6578  ----.    complex
+00000180: 0a20 2020 2020 2020 2043 6f6d 706c 6578  .        Complex
+00000190: 2072 656c 6174 6976 6520 7065 726d 6974   relative permit
+000001a0: 7469 7669 7479 206f 6620 7761 7465 722e  tivity of water.
+000001b0: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
+000001c0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000001d0: 2020 2020 2e2e 2020 5b31 5d20 456c 6c69      ..  [1] Elli
+000001e0: 736f 6e2c 2057 2e20 4a2e 2028 3230 3037  son, W. J. (2007
+000001f0: 292e 2050 6572 6d69 7474 6976 6974 7920  ). Permittivity 
+00000200: 6f66 2070 7572 6520 7761 7465 722c 2061  of pure water, a
+00000210: 7420 7374 616e 6461 7264 0a20 2020 2020  t standard.     
+00000220: 2020 2061 746d 6f73 7068 6572 6963 2070     atmospheric p
+00000230: 7265 7373 7572 652c 206f 7665 7220 7468  ressure, over th
+00000240: 6520 6672 6571 7565 6e63 7920 7261 6e67  e frequency rang
+00000250: 6520 302d 3235 2054 487a 2061 6e64 2074  e 0-25 THz and t
+00000260: 6865 0a20 2020 2020 2020 2074 656d 7065  he.        tempe
+00000270: 7261 7475 7265 2072 616e 6765 2030 2d31  rature range 0-1
+00000280: 3030 2043 2e20 4a6f 7572 6e61 6c20 6f66  00 C. Journal of
+00000290: 2070 6879 7369 6361 6c20 616e 6420 6368   physical and ch
+000002a0: 656d 6963 616c 2072 6566 6572 656e 6365  emical reference
+000002b0: 0a20 2020 2020 2020 2064 6174 612c 2033  .        data, 3
+000002c0: 3628 3129 2c20 312d 3138 2e0a 2020 2020  6(1), 1-18..    
+000002d0: 2222 220a 2020 2020 2320 4672 6571 7565  """.    # Freque
+000002e0: 6e63 7920 636f 6e76 6572 7369 6f6e 2074  ncy conversion t
+000002f0: 6f20 487a 0a20 2020 2066 203d 2066 202a  o Hz.    f = f *
+00000300: 2031 6531 320a 0a20 2020 2023 2044 6566   1e12..    # Def
+00000310: 696e 6520 7265 6c61 7861 7469 6f6e 2070  ine relaxation p
+00000320: 6172 616d 6574 6572 730a 2020 2020 6120  arameters.    a 
+00000330: 3d20 6e70 2e61 7272 6179 285b 3739 2e32  = np.array([79.2
+00000340: 3338 3832 2c20 332e 3831 3538 3636 2c20  3882, 3.815866, 
+00000350: 312e 3633 3439 3637 5d29 0a20 2020 2062  1.634967]).    b
+00000360: 203d 206e 702e 6172 7261 7928 5b30 2e30   = np.array([0.0
+00000370: 3034 3330 3035 3938 2c20 302e 3031 3131  04300598, 0.0111
+00000380: 3732 3935 2c20 302e 3030 3638 3431 3534  7295, 0.00684154
+00000390: 385d 290a 2020 2020 6320 3d20 6e70 2e61  8]).    c = np.a
+000003a0: 7272 6179 285b 312e 3338 3232 3634 652d  rray([1.382264e-
+000003b0: 3133 2c20 332e 3531 3033 3534 652d 3136  13, 3.510354e-16
+000003c0: 2c20 362e 3330 3033 3565 2d31 355d 290a  , 6.30035e-15]).
+000003d0: 2020 2020 6420 3d20 6e70 2e61 7272 6179      d = np.array
+000003e0: 285b 3635 322e 3736 3438 2c20 3132 3439  ([652.7648, 1249
+000003f0: 2e35 3333 2c20 3430 352e 3531 3639 5d29  .533, 405.5169])
+00000400: 0a20 2020 2074 6320 3d20 3133 332e 3133  .    tc = 133.13
+00000410: 3833 0a0a 2020 2020 2320 4465 6669 6e65  83..    # Define
+00000420: 2072 6573 6f6e 616e 6365 2070 6172 616d   resonance param
+00000430: 6574 6572 730a 2020 2020 7030 203d 2030  eters.    p0 = 0
+00000440: 2e38 3337 3936 3932 0a20 2020 2070 203d  .8379692.    p =
+00000450: 206e 702e 6172 7261 7928 0a20 2020 2020   np.array(.     
+00000460: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00000470: 202d 302e 3030 3631 3138 3539 342c 0a20   -0.006118594,. 
+00000480: 2020 2020 2020 2020 2020 202d 302e 3030             -0.00
+00000490: 3030 3132 3933 3637 3938 2c0a 2020 2020  0012936798,.    
+000004a0: 2020 2020 2020 2020 3432 3335 3930 3130          42359010
+000004b0: 3030 3030 302c 0a20 2020 2020 2020 2020  00000,.         
+000004c0: 2020 202d 3134 3236 3038 3830 3030 302c     -14260880000,
+000004d0: 0a20 2020 2020 2020 2020 2020 2032 3733  .            273
+000004e0: 3831 3537 3030 2c0a 2020 2020 2020 2020  815700,.        
+000004f0: 2020 2020 2d31 3234 3639 3433 2c0a 2020      -1246943,.  
+00000500: 2020 2020 2020 2020 2020 392e 3631 3836            9.6186
+00000510: 3432 652d 3134 2c0a 2020 2020 2020 2020  42e-14,.        
+00000520: 2020 2020 312e 3739 3537 3836 652d 3136      1.795786e-16
+00000530: 2c0a 2020 2020 2020 2020 2020 2020 2d39  ,.            -9
+00000540: 2e33 3130 3031 3765 2d31 382c 0a20 2020  .310017e-18,.   
+00000550: 2020 2020 2020 2020 2031 2e36 3535 3437           1.65547
+00000560: 3365 2d31 392c 0a20 2020 2020 2020 2020  3e-19,.         
+00000570: 2020 2030 2e36 3136 3535 3332 2c0a 2020     0.6165532,.  
+00000580: 2020 2020 2020 2020 2020 302e 3030 3732            0.0072
+00000590: 3338 3533 322c 0a20 2020 2020 2020 2020  38532,.         
+000005a0: 2020 202d 302e 3030 3030 3935 3233 3336     -0.0000952336
+000005b0: 362c 0a20 2020 2020 2020 2020 2020 2031  6,.            1
+000005c0: 3539 3833 3137 3030 3030 3030 302c 0a20  5983170000000,. 
+000005d0: 2020 2020 2020 2020 2020 202d 3734 3431             -7441
+000005e0: 3335 3730 3030 302c 0a20 2020 2020 2020  3570000,.       
+000005f0: 2020 2020 2034 3937 3434 3830 3030 2c0a       497448000,.
+00000600: 2020 2020 2020 2020 2020 2020 322e 3838              2.88
+00000610: 3234 3736 652d 3134 2c0a 2020 2020 2020  2476e-14,.      
+00000620: 2020 2020 2020 2d33 2e31 3432 3131 3865        -3.142118e
+00000630: 2d31 362c 0a20 2020 2020 2020 2020 2020  -16,.           
+00000640: 2033 2e35 3238 3035 3165 2d31 382c 0a20   3.528051e-18,. 
+00000650: 2020 2020 2020 205d 0a20 2020 2029 0a0a         ].    )..
+00000660: 2020 2020 2320 436f 6d70 7574 6520 7465      # Compute te
+00000670: 6d70 6572 6174 7572 6520 2d20 6465 7065  mperature - depe
+00000680: 6e64 656e 7420 6675 6e63 7469 6f6e 730a  ndent functions.
+00000690: 2020 2020 6570 7330 203d 2038 372e 3931      eps0 = 87.91
+000006a0: 3434 202d 2030 2e34 3034 3339 3920 2a20  44 - 0.404399 * 
+000006b0: 7420 2b20 392e 3538 3732 3665 2d34 202a  t + 9.58726e-4 *
+000006c0: 2074 2a2a 3220 2d20 312e 3332 3830 3265   t**2 - 1.32802e
+000006d0: 2d36 202a 2074 2a2a 330a 2020 2020 6465  -6 * t**3.    de
+000006e0: 6c74 6120 3d20 6120 2a20 6e70 2e65 7870  lta = a * np.exp
+000006f0: 282d 6220 2a20 7429 0a20 2020 2074 6175  (-b * t).    tau
+00000700: 203d 2063 202a 206e 702e 6578 7028 6420   = c * np.exp(d 
+00000710: 2f20 2874 202b 2074 6329 290a 0a20 2020  / (t + tc))..   
+00000720: 2064 656c 7461 3420 3d20 7030 202b 2070   delta4 = p0 + p
+00000730: 5b30 5d20 2a20 7420 2b20 705b 315d 202a  [0] * t + p[1] *
+00000740: 2074 2a2a 320a 2020 2020 6630 203d 2070   t**2.    f0 = p
+00000750: 5b32 5d20 2b20 705b 335d 202a 2074 202b  [2] + p[3] * t +
+00000760: 2070 5b34 5d20 2a20 742a 2a32 202b 2070   p[4] * t**2 + p
+00000770: 5b35 5d20 2a20 742a 2a33 0a20 2020 2074  [5] * t**3.    t
+00000780: 6175 3420 3d20 705b 365d 202b 2070 5b37  au4 = p[6] + p[7
+00000790: 5d20 2a20 7420 2b20 705b 385d 202a 2074  ] * t + p[8] * t
+000007a0: 2a2a 3220 2b20 705b 395d 202a 2074 2a2a  **2 + p[9] * t**
+000007b0: 330a 2020 2020 6465 6c74 6135 203d 2070  3.    delta5 = p
+000007c0: 5b31 305d 202b 2070 5b31 315d 202a 2074  [10] + p[11] * t
+000007d0: 202b 2070 5b31 325d 202a 2074 2a2a 320a   + p[12] * t**2.
+000007e0: 2020 2020 6631 203d 2070 5b31 335d 202b      f1 = p[13] +
+000007f0: 2070 5b31 345d 202a 2074 202b 2070 5b31   p[14] * t + p[1
+00000800: 355d 202a 2074 2a2a 320a 2020 2020 7461  5] * t**2.    ta
+00000810: 7535 203d 2070 5b31 365d 202b 2070 5b31  u5 = p[16] + p[1
+00000820: 375d 202a 2074 202b 2070 5b31 385d 202a  7] * t + p[18] *
+00000830: 2074 2a2a 320a 0a20 2020 2023 2050 7574   t**2..    # Put
+00000840: 2069 7420 616c 6c20 746f 6765 7468 6572   it all together
+00000850: 0a20 2020 2065 7073 696c 6f6e 7220 3d20  .    epsilonr = 
+00000860: 280a 2020 2020 2020 2020 6570 7330 0a20  (.        eps0. 
+00000870: 2020 2020 2020 202b 2032 0a20 2020 2020         + 2.     
+00000880: 2020 202a 2031 6a0a 2020 2020 2020 2020     * 1j.        
+00000890: 2a20 6e70 2e70 690a 2020 2020 2020 2020  * np.pi.        
+000008a0: 2a20 660a 2020 2020 2020 2020 2a20 280a  * f.        * (.
+000008b0: 2020 2020 2020 2020 2020 2020 6465 6c74              delt
+000008c0: 615b 305d 202a 2074 6175 5b30 5d20 2f20  a[0] * tau[0] / 
+000008d0: 2831 202d 2032 202a 2031 6a20 2a20 6e70  (1 - 2 * 1j * np
+000008e0: 2e70 6920 2a20 6620 2a20 7461 755b 305d  .pi * f * tau[0]
+000008f0: 290a 2020 2020 2020 2020 2020 2020 2b20  ).            + 
+00000900: 6465 6c74 615b 315d 202a 2074 6175 5b31  delta[1] * tau[1
+00000910: 5d20 2f20 2831 202d 2032 202a 2031 6a20  ] / (1 - 2 * 1j 
+00000920: 2a20 6e70 2e70 6920 2a20 6620 2a20 7461  * np.pi * f * ta
+00000930: 755b 315d 290a 2020 2020 2020 2020 2020  u[1]).          
+00000940: 2020 2b20 6465 6c74 615b 325d 202a 2074    + delta[2] * t
+00000950: 6175 5b32 5d20 2f20 2831 202d 2032 202a  au[2] / (1 - 2 *
+00000960: 2031 6a20 2a20 6e70 2e70 6920 2a20 6620   1j * np.pi * f 
+00000970: 2a20 7461 755b 325d 290a 2020 2020 2020  * tau[2]).      
+00000980: 2020 290a 2020 2020 2020 2020 2b20 316a    ).        + 1j
+00000990: 0a20 2020 2020 2020 202a 206e 702e 7069  .        * np.pi
+000009a0: 0a20 2020 2020 2020 202a 2066 0a20 2020  .        * f.   
+000009b0: 2020 2020 202a 2028 0a20 2020 2020 2020       * (.       
+000009c0: 2020 2020 2064 656c 7461 3420 2a20 7461       delta4 * ta
+000009d0: 7534 202f 2028 3120 2d20 3220 2a20 316a  u4 / (1 - 2 * 1j
+000009e0: 202a 206e 702e 7069 202a 2074 6175 3420   * np.pi * tau4 
+000009f0: 2a20 2866 3020 2b20 6629 290a 2020 2020  * (f0 + f)).    
+00000a00: 2020 2020 2020 2020 2b20 6465 6c74 6134          + delta4
+00000a10: 202a 2074 6175 3420 2f20 2831 202b 2032   * tau4 / (1 + 2
+00000a20: 202a 2031 6a20 2a20 6e70 2e70 6920 2a20   * 1j * np.pi * 
+00000a30: 7461 7534 202a 2028 6630 202d 2066 2929  tau4 * (f0 - f))
+00000a40: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00000a50: 2020 202b 2031 6a0a 2020 2020 2020 2020     + 1j.        
+00000a60: 2a20 6e70 2e70 690a 2020 2020 2020 2020  * np.pi.        
+00000a70: 2a20 660a 2020 2020 2020 2020 2a20 280a  * f.        * (.
+00000a80: 2020 2020 2020 2020 2020 2020 6465 6c74              delt
+00000a90: 6135 202a 2074 6175 3520 2f20 2831 202d  a5 * tau5 / (1 -
+00000aa0: 2032 202a 2031 6a20 2a20 6e70 2e70 6920   2 * 1j * np.pi 
+00000ab0: 2a20 7461 7535 202a 2028 6631 202b 2066  * tau5 * (f1 + f
+00000ac0: 2929 0a20 2020 2020 2020 2020 2020 202b  )).            +
+00000ad0: 2064 656c 7461 3520 2a20 7461 7535 202f   delta5 * tau5 /
+00000ae0: 2028 3120 2b20 3220 2a20 316a 202a 206e   (1 + 2 * 1j * n
+00000af0: 702e 7069 202a 2074 6175 3520 2a20 2866  p.pi * tau5 * (f
+00000b00: 3120 2d20 6629 290a 2020 2020 2020 2020  1 - f)).        
+00000b10: 290a 2020 2020 290a 0a20 2020 2072 6574  ).    )..    ret
+00000b20: 7572 6e20 6570 7369 6c6f 6e72 0a         urn epsilonr.
```

### Comparing `thztools-0.0.2/.gitignore` & `thztools-0.0.2.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2/LICENSE` & `thztools-0.0.2.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2/pyproject.toml` & `thztools-0.0.2.post0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "THzTools"
 dynamic = ["version"]
 description = "Tools for terahertz time-domain spectroscopy (THz-TDS)"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = ["terahertz", "THz", "time-domain spectroscopy", "data analysis"]
 authors = [
     { name="Steve Dodge", email="jsdodge@sfu.ca" },
     { name="Santiago Higuera Quintero", email="s.higuera@uniandes.edu.co" },
     { name="Jonathan Posada", email="jonathan.posada1@udea.edu.co" },
 ]
 maintainers = [
     { name="Steve Dodge", email="jsdodge@sfu.ca" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
   	"Programming Language :: Python",
-  	"Programming Language :: Python :: 3.7",
   	"Programming Language :: Python :: 3.8",
   	"Programming Language :: Python :: 3.9",
   	"Programming Language :: Python :: 3.10",
   	"Programming Language :: Python :: 3.11",
   	"Programming Language :: Python :: Implementation :: CPython",
   	"Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
@@ -63,22 +62,23 @@
 ]
 cov = [
     "test-cov",
     "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
     "black>=23.1.0",
     "black[jupyter]",
     "mypy>=1.0.0",
+    "numpy>=1.21",
     "ruff>=0.0.243",
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/thztools tests}"
 style = [
     "ruff {args:.}",
     "black --check --diff {args:.}",
@@ -90,20 +90,20 @@
 ]
 all = [
     "style",
     "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 79
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 79
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
@@ -174,14 +174,15 @@
     "if TYPE_CHECKING:",
 ]
 
 [tool.hatch.envs.docs]
 dependencies = [
     "sphinx",
     "pydata-sphinx-theme",
+    "numpydoc",
     "tomli",
 ]
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs/source docs/build/html"
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
```

### Comparing `thztools-0.0.2/PKG-INFO` & `thztools-0.0.2.post0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: THzTools
-Version: 0.0.2
+Version: 0.0.2.post0
 Summary: Tools for terahertz time-domain spectroscopy (THz-TDS)
 Project-URL: Documentation, https://dodge-research-group.github.io/thztools/
 Project-URL: Issues, https://github.com/dodge-research-group/thztools/issues
 Project-URL: Source, https://github.com/dodge-research-group/thztools
 Author-email: Steve Dodge <jsdodge@sfu.ca>, Santiago Higuera Quintero <s.higuera@uniandes.edu.co>, Jonathan Posada <jonathan.posada1@udea.edu.co>
 Maintainer-email: Steve Dodge <jsdodge@sfu.ca>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: THz,data analysis,terahertz,time-domain spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: jupyter
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # THzTools
 
 Data analysis tools for terahertz time-domain spectroscopy.
 
 This is *alpha* software that is currently under development.
 
-| Information       | Links                                                                                                                                                                                                                                                                                                                                   |
-|:------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/python-package-conda.yml?label=build%3Atests)                                |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                        |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                    |
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)                                                                                                                                                                                                                                                                                             |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-conda.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
 
 The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

