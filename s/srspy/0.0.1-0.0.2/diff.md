# Comparing `tmp/srspy-0.0.1.tar.gz` & `tmp/srspy-0.0.2.tar.gz`

## Comparing `srspy-0.0.1.tar` & `srspy-0.0.2.tar`

### file list

```diff
@@ -1,341 +1,374 @@
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 srspy-0.0.1/Makefile
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 srspy-0.0.1/requirements.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180389 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52421 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23357 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60697 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130433 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123338 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109225 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57766 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142229 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    90144 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85358 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    26818 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87509 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44414 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75218 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167566 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49762 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    17713 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srs.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srs.meta.json
--rw-r--r--   0        0        0   162185 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    42830 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239653 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432255 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33607 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    89075 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   408009 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129004 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dateutil/__init__.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dateutil/__init__.meta.json
--rw-r--r--   0        0        0    20958 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/__init__.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/__init__.meta.json
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/isoparser.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/isoparser.meta.json
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30878 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70600 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64592 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   322642 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/__init__.data.json
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/__init__.meta.json
--rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/log_entry.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/log_entry.meta.json
--rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/records.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/records.meta.json
--rw-r--r--   0        0        0    13391 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/runs.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/runs.meta.json
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/srs.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 srspy-0.0.1/.mypy_cache/3.11/srspy/srs.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/10fb82a6a5b1a167
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/12d6a662a1dcd8f2
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/16893488949543b5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/177993fc1ecdca81
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/198e580d5046dd3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/1b0938ae311045e1
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/1b264ca1a1f2619f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/1cd87d87419a361f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/1e873a54d53d33e0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/1f6df30fca596e5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/21490777d2a2aaa7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/21bdff545a494fe2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/22f2afcf15a6c536
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/242f7c56c5da39c9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/24c733872d3ae4ee
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/25911cf2048f02be
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/266f07be8bde9bd2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/26a17a85e14f33b1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/27cb8737aa6cda6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2894448493dd084c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2a295b8cb0489f44
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2bbe9874abf4b1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2becbe8b0ff22bf4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2d6513f82db79795
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2da3cb3126b7e14a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2edc7e740a5328ff
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2f4169343413da3f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2f6c41f78a20b124
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2fb2926b43a7d5c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/2feb96b94a620ea4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/312805cdecf61891
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/31863efe437400db
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/33c36c625419599f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/35b5b70ce0991578
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/3610963058adb406
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/36558a07b6fedca8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/3661f3d3da249f8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/370b998841feae4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/37a67139d21778da
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/38335edd437c46e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/3a7246b96b10039a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/3bc630598e95057a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/3ea0c75c93016e42
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/3edf02f949235428
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4009d832234ae015
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/435060340085ebb4
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/43598e7c237f4681
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/460a9bd40744fd4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/48243e380e0996e0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4b3bd2525f165177
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4c52196265328c1f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4cb19f0dbc0bef7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4cbf47e7397de70c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4e7d5bce4b6a37ef
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4efb0f33c7b30e9e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/4f60c74efe5b705e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/50bf890a1c4f722f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/50f0188d73372f16
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/51571dc6869005eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/521a27b07b6aaf5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/53f288fe814d0741
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/549838235a11840
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/54a52dc360666096
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/553c44ab2158fec7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5754edbbd23503c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/576bf926c5d02d55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5827b192d7c66b33
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5854d464ac833574
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/595f6f54c9dac756
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/59d94086262564b9
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5b6c4e6fbb5d4335
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5bd01976870e6d9b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5beff91272e39900
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/5f729afd0ffd2b72
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/62267ae6fe22018a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/64f2312904491cc6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/666ed4babcd27c69
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/6766458d67757abc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/67b15aa8436f7f3b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/681b1bc394bae6ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/689cff0fc07b7eea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/68da225aa6e8642e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/6bdaf31cb517570c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/6cd21dcbe621b5e4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/6d90c13f7a31de57
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/6dff048e457e3d9e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/727464aee5404573
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/73d7ea9396bebbf3
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/76176a6ca7cfd116
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/76ef8dcab6b37fee
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/77436814c5d4cf3a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/785b639f73945d5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7895c7359e14114f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7b042dd35c22779d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7cd5843499f57461
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7e816c1a531ea982
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7ebb813298c566cb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7f7c49cdaf7da1a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/7fcaba8c6a6db941
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/802e19242e3ca13f
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/804b0fd4fb4bbbd8
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/80d09d3c5c927322
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/82a0d7eb5d0665c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/82dbf75c632a7ffd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8353c5d3889365ca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/83a42a9d0ed6c42c
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/83abbac0c0fd74e4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/83b50618dfa9520a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/85f837175543fe8a
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/86cacf9d2971e509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/87ef3154fb375105
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/87f7b161d8576127
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/89cbc58af2a73dc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8a53f4f68a102e9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8c4cb25801c51777
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8c76a720cd0ba5c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8c91a0c9359eb501
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8d2ad3a55451847
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8d83cd2fcf4ac556
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/8dbf43ac46751f47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/908b74f27f07a872
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9096d8d8cbabe809
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/92192afcd64a81cf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9312b0e833c7b923
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/93f4a03e461571d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9408a2bdafdf33c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/947526de28276128
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/94f16de74e60572d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/97423dac26d3ab62
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/992dd93e9d795f26
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/99b3f51a7d5c2625
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9a616b08b8f2a8df
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9c67d9306617cccd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9cf0fa68d9857b0d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9e08da37fde74771
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/9ec215646e20107f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a05c1920d597bbf9
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a0b16a502b97599f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a246bd34e68bf7df
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a3da69d52ad6abfc
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a460735821de56e1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a5bf60c697936f14
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a635c093b5fbdf40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a7e33fc6532ff574
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/a9a9284c84f4bd94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ab7efb78dbc4fd90
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ac047ed55fd14676
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ad53003adf4c947d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ad571bbc497232de
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ade0fb5b01ca3ce1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ae744bdf26182ab1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ae91b397fe3aa6ed
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/b118fb08429e3f35
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/b3816ccdd15ed57
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/b4215f320ef8fe5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/b5b026c4c1e1e9ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/b5efc413a70b129b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/b9e6d0632cb70118
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/bab3ad25d0c35c48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/bb711c3f41fe979d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/bd845365a6978b37
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/bd8b889f446dfc35
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/c0e8d07589cfc6c9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/c619583cf58a9f1a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/c9d5964a430967c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ca132c76a55055f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ca2793fe106ccacb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/cb3591668d0ae4f7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/cb3ce4602ad99555
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ccc3e558e4fc656c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/cd261c7dccd5fca0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ce5d79aa60ad5128
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/cf15a2bfefb743c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/cf218313d8f93e12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/d168bb29fa5200f8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/d30f732af09bd8a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/d69cc64bfa74f007
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/d723ef1431c4dfd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/d7926a22d06ea870
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/d8348593e1bf2cad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/dc23be558dbb3061
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/dc7455c4747f50ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/dca8e75acb9c693c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/de87aa2fdae4cfa4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/df38dbf5c0a70e34
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/e1f5b85d2595db6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/e238f00bdc1ed6fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/e29970cf6feab08c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/e36579debc4a9ce4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/e405ed214c7e92d3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/eb4ae6684c89b085
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ee234f1f9a61a717
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ef4b3d398486ae28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f18458c1ca74f91c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f20d4e3ded10a127
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f2ff556283f5b9e3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f50a682ea748a37f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f601a63974554224
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f868dedd1025e020
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f8c5d06eafb9125b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/f8cf2a49834e98e6
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/fd7ef9aebfd37dd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/fdb7c99898e97ad3
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/fdde61a1c953e689
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.1/.ruff_cache/content/ff873635286e0820
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 srspy-0.0.1/src/srspy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srspy-0.0.1/src/srspy/py.typed
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 srspy-0.0.1/src/srspy/records.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 srspy-0.0.1/src/srspy/runs.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 srspy-0.0.1/tests/01_smoke_test:_records.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 srspy-0.0.1/tests/02_smoke_test:_runs.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 srspy-0.0.1/tests/03_smoke_test:_srspy.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 srspy-0.0.1/.gitignore
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 srspy-0.0.1/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 srspy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 srspy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 srspy-0.0.2/Makefile
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 srspy-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180389 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52421 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23357 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60697 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130433 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123338 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109225 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57766 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142229 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    90144 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85358 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    26818 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87509 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44414 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75218 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167566 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49762 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0    17713 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srs.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srs.meta.json
+-rw-r--r--   0        0        0   162185 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    42830 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239653 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432255 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33607 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    89075 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   408009 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129004 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dateutil/__init__.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dateutil/__init__.meta.json
+-rw-r--r--   0        0        0    20958 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/__init__.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/__init__.meta.json
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/isoparser.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/isoparser.meta.json
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30878 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70600 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64592 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   322642 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/__init__.data.json
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/__init__.meta.json
+-rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/log_entry.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/log_entry.meta.json
+-rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/records.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/records.meta.json
+-rw-r--r--   0        0        0    13819 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/runs.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/runs.meta.json
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/srs.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 srspy-0.0.2/.mypy_cache/3.11/srspy/srs.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/10fb82a6a5b1a167
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/12d6a662a1dcd8f2
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/16893488949543b5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/177993fc1ecdca81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/198e580d5046dd3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/1b0938ae311045e1
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/1b264ca1a1f2619f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/1cd87d87419a361f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/1e873a54d53d33e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/1f6df30fca596e5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/20f5cb312d9a8974
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/21490777d2a2aaa7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/21bdff545a494fe2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/22f2afcf15a6c536
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/242f7c56c5da39c9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/24c733872d3ae4ee
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/25911cf2048f02be
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/266f07be8bde9bd2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/26a17a85e14f33b1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/27cb8737aa6cda6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2894448493dd084c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/29d2c92943ee6af
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2a295b8cb0489f44
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2bbe9874abf4b1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2becbe8b0ff22bf4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2d6513f82db79795
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2da3cb3126b7e14a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2edc7e740a5328ff
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2f4169343413da3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2f6c41f78a20b124
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2fb2926b43a7d5c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/2feb96b94a620ea4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/308eb0b4711651e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/312805cdecf61891
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/31863efe437400db
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/33646faba44b6c77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/33c36c625419599f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/35b5b70ce0991578
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3610963058adb406
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/36558a07b6fedca8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3661f3d3da249f8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/370b998841feae4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/37a67139d21778da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3810015489dbb997
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/38335edd437c46e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3a7246b96b10039a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3bc630598e95057a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3ea0c75c93016e42
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3edf02f949235428
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/3f17201e0d09dafd
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4009d832234ae015
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/40fbeb2b8b18c9f7
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/415a1ebac7c1e7e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/42a916d77bd117ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/435060340085ebb4
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/43598e7c237f4681
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4499034201d086fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/460a9bd40744fd4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/48243e380e0996e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4a7b8d93f5da7610
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4b3bd2525f165177
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4c52196265328c1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4cb19f0dbc0bef7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4cbf47e7397de70c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4e7d5bce4b6a37ef
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4efb0f33c7b30e9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/4f60c74efe5b705e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/50bf890a1c4f722f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/50f0188d73372f16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/51571dc6869005eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/521a27b07b6aaf5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/53f288fe814d0741
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/541a86a666277c74
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/547a4deb6cb31f0d
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/549838235a11840
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/54a52dc360666096
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/553c44ab2158fec7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5754edbbd23503c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/576bf926c5d02d55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5827b192d7c66b33
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5854d464ac833574
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/595f6f54c9dac756
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/59d94086262564b9
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5b6c4e6fbb5d4335
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5bd01976870e6d9b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5beff91272e39900
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/5f729afd0ffd2b72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/62267ae6fe22018a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/64f2312904491cc6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/666ed4babcd27c69
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6766458d67757abc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/67b15aa8436f7f3b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/681b1bc394bae6ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/689cff0fc07b7eea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/68da225aa6e8642e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6aaf9e961881580c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6bdaf31cb517570c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6cd21dcbe621b5e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6d32274afd7dfab8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6d90c13f7a31de57
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/6dff048e457e3d9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/727464aee5404573
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/73d7ea9396bebbf3
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/76176a6ca7cfd116
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/76ef8dcab6b37fee
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/77436814c5d4cf3a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/784fe1c6e3e11529
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/785b639f73945d5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7895c7359e14114f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7ad8c8e872f30040
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7b042dd35c22779d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7bd206789f532692
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7cd5843499f57461
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7e816c1a531ea982
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7ebb813298c566cb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7f7c49cdaf7da1a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/7fcaba8c6a6db941
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/802e19242e3ca13f
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/804b0fd4fb4bbbd8
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/80d09d3c5c927322
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/82a0d7eb5d0665c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/82b290394fd0308e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/82dbf75c632a7ffd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8353c5d3889365ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/83a42a9d0ed6c42c
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/83abbac0c0fd74e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/83b50618dfa9520a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/85f837175543fe8a
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/86cacf9d2971e509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/87ef3154fb375105
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/87f7b161d8576127
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/89cbc58af2a73dc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8a53f4f68a102e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8c4cb25801c51777
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8c76a720cd0ba5c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8c91a0c9359eb501
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8d2ad3a55451847
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8d83cd2fcf4ac556
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/8dbf43ac46751f47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/908b74f27f07a872
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9096d8d8cbabe809
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/92192afcd64a81cf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9312b0e833c7b923
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/93f4a03e461571d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9408a2bdafdf33c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/947526de28276128
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/94f16de74e60572d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/97423dac26d3ab62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/992dd93e9d795f26
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/99b3f51a7d5c2625
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9a616b08b8f2a8df
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9c67d9306617cccd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9cf0fa68d9857b0d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9e08da37fde74771
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/9ec215646e20107f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a05c1920d597bbf9
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a0b16a502b97599f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a246bd34e68bf7df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a2c6715d36ad6e6e
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a3da69d52ad6abfc
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a460735821de56e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a4a707cf3f37877a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a503f943902d3fa6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a5bf60c697936f14
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a635c093b5fbdf40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a7e33fc6532ff574
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/a9a9284c84f4bd94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ab7efb78dbc4fd90
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ac047ed55fd14676
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ad53003adf4c947d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ad571bbc497232de
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ade0fb5b01ca3ce1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ae744bdf26182ab1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ae91b397fe3aa6ed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b032a7e4548f235c
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b118fb08429e3f35
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b3816ccdd15ed57
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b4215f320ef8fe5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b5b026c4c1e1e9ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b5e5d31b2a4990cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b5efc413a70b129b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/b9e6d0632cb70118
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ba40a1c2e74dec79
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/bab3ad25d0c35c48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/bb711c3f41fe979d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/bd845365a6978b37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/bd8b889f446dfc35
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/c0e8d07589cfc6c9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/c619583cf58a9f1a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/c9d5964a430967c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ca132c76a55055f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ca2793fe106ccacb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/cb3591668d0ae4f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/cb3ce4602ad99555
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ccc3e558e4fc656c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/cd261c7dccd5fca0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ce5d79aa60ad5128
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/cf15a2bfefb743c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/cf218313d8f93e12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d168bb29fa5200f8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d28f78c5c5c6d775
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d30f732af09bd8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d69cc64bfa74f007
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d723ef1431c4dfd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d7926a22d06ea870
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/d8348593e1bf2cad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/dac46d2b59594469
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/dbe7bf4a723a0a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/dc23be558dbb3061
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/dc7455c4747f50ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/dca8e75acb9c693c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/de87aa2fdae4cfa4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/df38dbf5c0a70e34
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/e1f5b85d2595db6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/e238f00bdc1ed6fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/e29970cf6feab08c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/e36579debc4a9ce4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/e405ed214c7e92d3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/e6ee2e9e93857aab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/eb4ae6684c89b085
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ee234f1f9a61a717
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ef4b3d398486ae28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/efeb46e355fc5185
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f18458c1ca74f91c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f20d4e3ded10a127
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f2ff556283f5b9e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f4002d9e7206bc85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f50a682ea748a37f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f601a63974554224
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f689ab44afe9670d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f868dedd1025e020
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f88f2cd14efbcf1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f8c5d06eafb9125b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/f8cf2a49834e98e6
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/fd7ef9aebfd37dd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/fdb7c99898e97ad3
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/fdde61a1c953e689
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 srspy-0.0.2/.ruff_cache/content/ff873635286e0820
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 srspy-0.0.2/src/srspy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srspy-0.0.2/src/srspy/py.typed
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 srspy-0.0.2/src/srspy/records.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 srspy-0.0.2/src/srspy/runs.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 srspy-0.0.2/tests/01_smoke_test:_records.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 srspy-0.0.2/tests/02_smoke_test:_runs.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 srspy-0.0.2/tests/03_smoke_test:_srspy.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 srspy-0.0.2/.gitignore
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 srspy-0.0.2/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 srspy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 srspy-0.0.2/PKG-INFO
```

### Comparing `srspy-0.0.1/Makefile` & `srspy-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_ast.data.json` & `srspy-0.0.2/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_ast.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_codecs.data.json` & `srspy-0.0.2/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_codecs.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_collections_abc.data.json` & `srspy-0.0.2/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_collections_abc.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_ctypes.data.json` & `srspy-0.0.2/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_ctypes.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/abc.data.json` & `srspy-0.0.2/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/abc.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/array.data.json` & `srspy-0.0.2/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/array.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/builtins.data.json` & `srspy-0.0.2/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/builtins.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/codecs.data.json` & `srspy-0.0.2/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/codecs.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/contextlib.data.json` & `srspy-0.0.2/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/contextlib.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dataclasses.data.json` & `srspy-0.0.2/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dataclasses.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/datetime.data.json` & `srspy-0.0.2/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/datetime.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/enum.data.json` & `srspy-0.0.2/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/enum.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/genericpath.data.json` & `srspy-0.0.2/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/genericpath.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/io.data.json` & `srspy-0.0.2/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/io.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/mmap.data.json` & `srspy-0.0.2/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/mmap.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/pathlib.data.json` & `srspy-0.0.2/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/pathlib.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/pickle.data.json` & `srspy-0.0.2/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/pickle.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/posixpath.data.json` & `srspy-0.0.2/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/posixpath.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/re.data.json` & `srspy-0.0.2/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/re.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sre_compile.data.json` & `srspy-0.0.2/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sre_compile.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sre_constants.data.json` & `srspy-0.0.2/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sre_constants.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sre_parse.data.json` & `srspy-0.0.2/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sre_parse.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srs.data.json` & `srspy-0.0.2/.mypy_cache/3.11/srs.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srs.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/srs.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/subprocess.data.json` & `srspy-0.0.2/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/subprocess.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sys.data.json` & `srspy-0.0.2/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/sys.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/time.data.json` & `srspy-0.0.2/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/time.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/types.data.json` & `srspy-0.0.2/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/types.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/typing.data.json` & `srspy-0.0.2/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/typing.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/typing_extensions.data.json` & `srspy-0.0.2/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/typing_extensions.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/uuid.data.json` & `srspy-0.0.2/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/uuid.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/collections/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/collections/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/collections/abc.data.json` & `srspy-0.0.2/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/collections/abc.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dateutil/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/dateutil/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dateutil/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/dateutil/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/isoparser.data.json` & `srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/isoparser.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/dateutil/parser/isoparser.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/dateutil/parser/isoparser.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/charset.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/charset.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/contentmanager.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/errors.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/errors.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/header.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/header.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/message.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/message.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/policy.data.json` & `srspy-0.0.2/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/email/policy.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/abc.data.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/abc.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/machinery.data.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/json/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/json/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/json/decoder.data.json` & `srspy-0.0.2/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/json/decoder.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/json/encoder.data.json` & `srspy-0.0.2/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/json/encoder.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/os/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/os/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/os/path.data.json` & `srspy-0.0.2/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/os/path.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/__init__.data.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/__init__.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/__init__.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'data_mtime'": '1686175900', "'mtime'": '1686176728'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1686174949,
+    "data_mtime": 1686175900,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
@@ -18,15 +18,15 @@
         "abc",
         "typing"
     ],
     "hash": "6ccba67a3088495136fc28f271ce7db95c952d8769e6c780a9899ca55677de3b",
     "id": "srspy",
     "ignore_all": false,
     "interface_hash": "bf1ab7c5058f39a4c8ab81b1c91e7735eeb5fa776b767d4d269a13916cbfe92d",
-    "mtime": 1686174932,
+    "mtime": 1686176728,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
```

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/log_entry.data.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/log_entry.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/log_entry.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/log_entry.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/records.data.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/records.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/records.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/records.meta.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/runs.data.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/runs.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999881382063%*

 * *Differences: {"'names'": "{'File': {'node': {'names': {'write': {'node': {'arg_names': {insert: [(1, 'b')], "*

 * *            "delete: [1]}, 'type': {replace: OrderedDict([('.class', 'CallableType'), "*

 * *            "('arg_kinds', [0, 0]), ('arg_names', ['self', 'b']), ('arg_types', "*

 * *            "['srspy.runs.File', 'builtins.bytes']), ('bound_args', []), ('def_extras', "*

 * *            "OrderedDict([('first_arg', 'self')])), ('fallback', 'builtins.function'), "*

 * *            "('from_concatenate', False), ('implicit', False), ('i […]*

```diff
@@ -227,23 +227,55 @@
                             "abstract_status": 2,
                             "arg_kinds": [
                                 0,
                                 0
                             ],
                             "arg_names": [
                                 "self",
-                                "bytes"
+                                "b"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [
                                 "is_trivial_body"
                             ],
                             "fullname": "srspy.runs.File.write",
                             "name": "write",
-                            "type": null
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self",
+                                    "b"
+                                ],
+                                "arg_types": [
+                                    "srspy.runs.File",
+                                    "builtins.bytes"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "write of File",
+                                "ret_type": {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 1
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
                         }
                     }
                 },
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
```

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/runs.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/srs.meta.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7571895424836601%*

 * *Differences: {"'data_mtime'": '1686172204',*

 * * "'dep_lines'": '{insert: [(0, 9), (6, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(7, 30)]}',*

 * * "'dependencies'": "{insert: [(12, 'json.decoder')]}",*

 * * "'hash'": "'e7d3baeae1b8db62d2de1438f835c0c1d8f1949175463922363b4ed2b84aa6b1'",*

 * * "'id'": "'srspy.srs'",*

 * * "'interface_hash'": "'bb603de6f4af291c9baf1f64bd704934dd325b5064de4c29745b7d645850daab'",*

 * * "'mtime'": '1686172203',*

 * * "'path'": "'src/srspy/srs.py'",*

 * * "'size'": '2907'}*

```diff
@@ -1,25 +1,26 @@
 {
-    "data_mtime": 1686174483,
+    "data_mtime": 1686172204,
     "dep_lines": [
-        8,
+        9,
         2,
         3,
         4,
         5,
         6,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         10,
@@ -30,14 +31,15 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
         "srspy.records",
         "typing",
         "datetime",
         "json",
@@ -45,24 +47,25 @@
         "uuid",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "io",
+        "json.decoder",
         "json.encoder",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "2fb46555cb22c1e86e8bfd3a897e674e255d6d5f760ef0abbddeb79ff44afa07",
-    "id": "srspy.runs",
+    "hash": "e7d3baeae1b8db62d2de1438f835c0c1d8f1949175463922363b4ed2b84aa6b1",
+    "id": "srspy.srs",
     "ignore_all": false,
-    "interface_hash": "34ac9dcf6b3523fb4fd4e7485a7138eaaeb2be4fa2c3fd2c45cb2edc6257bd63",
-    "mtime": 1686174499,
+    "interface_hash": "bb603de6f4af291c9baf1f64bd704934dd325b5064de4c29745b7d645850daab",
+    "mtime": 1686172203,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -96,13 +99,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/srspy/runs.py",
+    "path": "src/srspy/srs.py",
     "plugin_data": null,
-    "size": 3080,
+    "size": 2907,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/srs.data.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/srs.data.json`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.mypy_cache/3.11/srspy/srs.meta.json` & `srspy-0.0.2/.mypy_cache/3.11/srspy/runs.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7571895424836601%*

 * *Differences: {"'data_mtime'": '1686175900',*

 * * "'dep_lines'": '{insert: [(0, 8)], delete: [6, 0]}',*

 * * "'dep_prios'": '{delete: [7]}',*

 * * "'dependencies'": '{delete: [12]}',*

 * * "'hash'": "'225f326fa65941a850ea6f94b7b8cb487a25206c9bfa260c63b324d830475093'",*

 * * "'id'": "'srspy.runs'",*

 * * "'interface_hash'": "'2099c66bc57c0f71ce34fa5c0e9c2ab4e9680a607b08ceb75a0dd18255646821'",*

 * * "'mtime'": '1686176788',*

 * * "'path'": "'src/srspy/runs.py'",*

 * * "'size'": '3169'}*

```diff
@@ -1,26 +1,25 @@
 {
-    "data_mtime": 1686172204,
+    "data_mtime": 1686175900,
     "dep_lines": [
-        9,
+        8,
         2,
         3,
         4,
         5,
         6,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         10,
@@ -31,15 +30,14 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
         30
     ],
     "dependencies": [
         "srspy.records",
         "typing",
         "datetime",
         "json",
@@ -47,25 +45,24 @@
         "uuid",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "io",
-        "json.decoder",
         "json.encoder",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "e7d3baeae1b8db62d2de1438f835c0c1d8f1949175463922363b4ed2b84aa6b1",
-    "id": "srspy.srs",
+    "hash": "225f326fa65941a850ea6f94b7b8cb487a25206c9bfa260c63b324d830475093",
+    "id": "srspy.runs",
     "ignore_all": false,
-    "interface_hash": "bb603de6f4af291c9baf1f64bd704934dd325b5064de4c29745b7d645850daab",
-    "mtime": 1686172203,
+    "interface_hash": "2099c66bc57c0f71ce34fa5c0e9c2ab4e9680a607b08ceb75a0dd18255646821",
+    "mtime": 1686176788,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -99,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/srspy/srs.py",
+    "path": "src/srspy/runs.py",
     "plugin_data": null,
-    "size": 2907,
+    "size": 3169,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `srspy-0.0.1/.ruff_cache/content/1b264ca1a1f2619f` & `srspy-0.0.2/.ruff_cache/content/1b264ca1a1f2619f`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/25911cf2048f02be` & `srspy-0.0.2/.ruff_cache/content/25911cf2048f02be`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/2bbe9874abf4b1d` & `srspy-0.0.2/.ruff_cache/content/2bbe9874abf4b1d`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/2f4169343413da3f` & `srspy-0.0.2/.ruff_cache/content/2f4169343413da3f`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/4009d832234ae015` & `srspy-0.0.2/.ruff_cache/content/4009d832234ae015`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/43598e7c237f4681` & `srspy-0.0.2/.ruff_cache/content/43598e7c237f4681`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/4efb0f33c7b30e9e` & `srspy-0.0.2/.ruff_cache/content/4efb0f33c7b30e9e`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/549838235a11840` & `srspy-0.0.2/.ruff_cache/content/549838235a11840`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/54a52dc360666096` & `srspy-0.0.2/.ruff_cache/content/54a52dc360666096`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/5b6c4e6fbb5d4335` & `srspy-0.0.2/.ruff_cache/content/5b6c4e6fbb5d4335`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/5f729afd0ffd2b72` & `srspy-0.0.2/.ruff_cache/content/5f729afd0ffd2b72`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/73d7ea9396bebbf3` & `srspy-0.0.2/.ruff_cache/content/73d7ea9396bebbf3`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/76176a6ca7cfd116` & `srspy-0.0.2/.ruff_cache/content/76176a6ca7cfd116`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/76ef8dcab6b37fee` & `srspy-0.0.2/.ruff_cache/content/76ef8dcab6b37fee`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/77436814c5d4cf3a` & `srspy-0.0.2/.ruff_cache/content/77436814c5d4cf3a`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/7ebb813298c566cb` & `srspy-0.0.2/.ruff_cache/content/7ebb813298c566cb`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/804b0fd4fb4bbbd8` & `srspy-0.0.2/.ruff_cache/content/804b0fd4fb4bbbd8`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/80d09d3c5c927322` & `srspy-0.0.2/.ruff_cache/content/80d09d3c5c927322`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/86cacf9d2971e509` & `srspy-0.0.2/.ruff_cache/content/86cacf9d2971e509`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/8d83cd2fcf4ac556` & `srspy-0.0.2/.ruff_cache/content/8d83cd2fcf4ac556`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/9096d8d8cbabe809` & `srspy-0.0.2/.ruff_cache/content/9096d8d8cbabe809`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/9c67d9306617cccd` & `srspy-0.0.2/.ruff_cache/content/9c67d9306617cccd`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/9ec215646e20107f` & `srspy-0.0.2/.ruff_cache/content/9ec215646e20107f`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/a0b16a502b97599f` & `srspy-0.0.2/.ruff_cache/content/a0b16a502b97599f`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/a3da69d52ad6abfc` & `srspy-0.0.2/.ruff_cache/content/a3da69d52ad6abfc`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/a460735821de56e1` & `srspy-0.0.2/.ruff_cache/content/a460735821de56e1`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/ade0fb5b01ca3ce1` & `srspy-0.0.2/.ruff_cache/content/ade0fb5b01ca3ce1`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/b118fb08429e3f35` & `srspy-0.0.2/.ruff_cache/content/b118fb08429e3f35`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/ee234f1f9a61a717` & `srspy-0.0.2/.ruff_cache/content/ee234f1f9a61a717`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/f2ff556283f5b9e3` & `srspy-0.0.2/.ruff_cache/content/f2ff556283f5b9e3`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/fd7ef9aebfd37dd4` & `srspy-0.0.2/.ruff_cache/content/fd7ef9aebfd37dd4`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/.ruff_cache/content/fdde61a1c953e689` & `srspy-0.0.2/.ruff_cache/content/fdde61a1c953e689`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/src/srspy/records.py` & `srspy-0.0.2/src/srspy/records.py`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/src/srspy/runs.py` & `srspy-0.0.2/src/srspy/runs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     we can use as a path (e.g., it has no spaces).
 
     This function is a helper to `RunTrace.__init__` below
     """
     return str(datetime.datetime.now()).replace(" ", "_")
 
 
-# A type-hint interface for file system methods required.
+# A type-hint interface for a file system.
 class FS(Protocol):
     def open(self, name: str, mode: str = "wb") -> IO[bytes]:
         ...
 
 
-# A type-hint interface for File methods required.
+# A type-hint interface for a file.
 class File(Protocol):
-    def write(self, bytes):
+    def write(self, b: bytes):
         ...
 
     def flush(self):
         ...
 
     def close(self):
         ...
@@ -61,29 +61,29 @@
         name: str = "",
         log_dir: str = "",
         data: dict = {},
         fs: FS = LocalFS,
         verbose=False,
     ):
         if name == "":
-            raise ValueError("RunTrace.init: name must be set")
+            raise ValueError("RunTrace.init: must provide keyword argument `name`")
         self.name = name
 
         if log_dir == "":
             log_dir = DEFAULT_LOG_DIR
         self.log_dir = log_dir
 
         self.log_file_path = os.path.join(self.log_dir, f"{name}_{now_str()}.json")
 
         self.verbose = verbose
         if verbose:
             print(f"RunTrace.init at path: {self.log_file_path}")
 
         self._fs = fs
-        self.log_file = fs.open(self.log_file_path, "wb")
+        self.log_file = self._fs.open(self.log_file_path, "wb")
         self.log(summary=f"{name} {now_str()}", data=data)
 
     def log(self, summary: str = "", data: dict = {}, type: LogEntryType = LogEntryLog):
         if self.closed:
             raise Exception("RunTrace.log: called on closed log")
 
         s = json.dumps(
@@ -98,18 +98,22 @@
         self.log_file.write(bytes(s, "utf-8"))
         self.log_file.write(b"\n")
 
     def flush(self, summary: str = "", data: dict = {}):
         if self.closed:
             raise Exception("RunTrace.flush: called on closed log")
 
-        self.log(summary=summary, data=data)
+        if summary != "" or data != {}:
+            self.log(summary=summary, data=data)
+
         self.log_file.flush()
 
     def close(self, summary: str = "", data: dict = {}):
         if self.closed:
             raise Exception("RunTrace.close: called on closed log")
 
-        self.log(summary=summary, data=data, type=LogEntryClose)
+        if summary != "" or data != {}:
+            self.log(summary=summary, data=data, type=LogEntryClose)
+
         self.log_file.flush()
         self.log_file.close()
         self.closed = True
```

### Comparing `srspy-0.0.1/tests/01_smoke_test:_records.py` & `srspy-0.0.2/tests/01_smoke_test:_records.py`

 * *Files identical despite different names*

### Comparing `srspy-0.0.1/tests/02_smoke_test:_runs.py` & `srspy-0.0.2/tests/02_smoke_test:_runs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,97 @@
 import pytest
 import io
+from typing import IO
 
 from srspy import runs
 
 print("THIS IS SMOKE TEST 2: IT TESTS basics")
 
-# lightweight tests on some helpers
+# Sundry basic tests
 assert runs.DEFAULT_LOG_DIR
 
 assert runs.now_str()
 assert " " not in runs.now_str()  # doesn't have spaces
 
+assert runs.File
 assert runs.FS
 assert runs.LocalFS
 assert runs.LocalFS.open("/dev/null")  # basic open
 
 
 # Some stubs for the file system stuff.
+
+## File stub
+
+
 class StubFile(object):
     mode: str
     closed: bool = False
     flushed: bool = True
+    buffer: IO
 
     def __init__(self, mode: str):
+        if "w" not in mode:
+            raise ValueError("StubFile: mode not writable")
+
         self.mode = mode
         self.buffer = io.BytesIO()
 
     def write(self, bs: bytes):
-        if "w" not in self.mode:
-            raise Exception("StubFile: mode not writable")
         if self.closed:
             raise Exception("StubFile: write on closed file")
 
         self.buffer.write(bs)
         self.Flushed = False
 
     def flush(self):
         # no op
         self.flushed = True
 
     def close(self):
         self.closed = True
 
 
+with pytest.raises(ValueError):
+    StubFile("asdf")  # mode does not have w
+
+with pytest.raises(Exception):
+    f = StubFile("wb")
+    assert f.closed
+    f.write()  # file closed
+
+assert StubFile("wb").flushed
+
+f = StubFile("wb")
+f.write(b"asdf")
+
+
+## FS stub
+
+
 class StubFS(object):
     files: dict
 
     def __init__(self):
         self.files = {}
 
     def open(self, path, mode):
         file = StubFile(mode)
         self.files[path] = file
         return file
 
 
+fs = StubFS()
+assert len(fs.files) == 0
+fs.open("one", "wb")
+fs.open("two", "wb")
+assert len(fs.files) == 2
+
+## Test RunTrace
+
 with pytest.raises(ValueError):
     runs.RunTrace()  # lacks name
 
 ## Use the stubbed file system
 fs = StubFS()
 r = runs.RunTrace(name="test", fs=fs)
 r.log(summary="this is a test", data={"metric": 100})
```

### Comparing `srspy-0.0.1/pyproject.toml` & `srspy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "srspy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name = "N. C. Landolfi", email="crews.fixture.0f@icloud.com"},
 ]
 description = "A package for simple experiment run tracing."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `srspy-0.0.1/PKG-INFO` & `srspy-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: srspy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for simple experiment run tracing.
 Project-URL: Homepage, https://github.com/nlandolfi/srspy
 Author-email: "N. C. Landolfi" <crews.fixture.0f@icloud.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
-# srspy
+srspy
+-----
 
 A package for simple research experiment tracing. Python 3.
 
 ```bash
 pip install srspy
 ```
```

