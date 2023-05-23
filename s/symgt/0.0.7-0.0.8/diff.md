# Comparing `tmp/symgt-0.0.7.tar.gz` & `tmp/symgt-0.0.8.tar.gz`

## Comparing `symgt-0.0.7.tar` & `symgt-0.0.8.tar`

### file list

```diff
@@ -1,1067 +1,1067 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 symgt-0.0.7/.DS_Store
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 symgt-0.0.7/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 symgt-0.0.7/py.typed
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 symgt-0.0.7/requirements.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180389 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52421 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    23357 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60697 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137641 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130433 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123338 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109225 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57766 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142229 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    90144 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   132088 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85358 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    52532 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    26818 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87509 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44414 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75218 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167566 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49762 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   162185 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    19574 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64736 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    42830 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239653 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432255 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0    75654 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/zipfile.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/zipfile.meta.json
--rw-r--r--   0        0        0    89075 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   408009 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129004 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30878 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70600 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64592 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   144406 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0  2221260 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/__init__.data.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_version.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_version.meta.json
--rw-r--r--   0        0        0   112520 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/version.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/version.meta.json
--rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25413 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   260487 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41727 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34744 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261368 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28015 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169675 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36064 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330704 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301761 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196446 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    45705 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    25156 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52630 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/records.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52763 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21728 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    24019 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   154552 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    25938 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   223855 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    63633 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    89097 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    96631 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    96758 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    62232 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    89060 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    77007 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    97329 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    24865 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26137 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107792 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27682 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136767 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27004 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16481 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13111 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   253033 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323864 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114214 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   322642 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/__init__.data.json
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/__init__.meta.json
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/algorithms.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/algorithms.meta.json
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/models.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/models.meta.json
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/symgt/utils.meta.json
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24089 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9289 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   210175 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/@plugins_snapshot.json
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/__future__.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/__future__.meta.json
--rw-r--r--   0        0        0   106758 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_ast.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_ast.meta.json
--rw-r--r--   0        0        0    51787 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_codecs.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_codecs.meta.json
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_collections_abc.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_collections_abc.meta.json
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_ctypes.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_ctypes.meta.json
--rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_thread.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_thread.meta.json
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_warnings.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_warnings.meta.json
--rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/abc.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/abc.meta.json
--rw-r--r--   0        0        0    60660 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/array.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/array.meta.json
--rw-r--r--   0        0        0   130043 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/ast.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/ast.meta.json
--rw-r--r--   0        0        0  1028269 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/builtins.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/builtins.meta.json
--rw-r--r--   0        0        0   123237 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/codecs.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/codecs.meta.json
--rw-r--r--   0        0        0    92094 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/contextlib.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/contextlib.meta.json
--rw-r--r--   0        0        0    56115 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/dataclasses.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/dataclasses.meta.json
--rw-r--r--   0        0        0   141448 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/datetime.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/datetime.meta.json
--rw-r--r--   0        0        0    61051 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/enum.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/enum.meta.json
--rw-r--r--   0        0        0   131415 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/functools.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/functools.meta.json
--rw-r--r--   0        0        0    22419 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/genericpath.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/genericpath.meta.json
--rw-r--r--   0        0        0    85368 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/io.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/io.meta.json
--rw-r--r--   0        0        0    51312 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/math.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/math.meta.json
--rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/mmap.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/mmap.meta.json
--rw-r--r--   0        0        0    87387 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/pathlib.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/pathlib.meta.json
--rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/pickle.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/pickle.meta.json
--rw-r--r--   0        0        0    75098 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/posixpath.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/posixpath.meta.json
--rw-r--r--   0        0        0   167206 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/re.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/re.meta.json
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sre_compile.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sre_compile.meta.json
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sre_constants.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sre_constants.meta.json
--rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sre_parse.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sre_parse.meta.json
--rw-r--r--   0        0        0    26505 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/string.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/string.meta.json
--rw-r--r--   0        0        0   156601 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/subprocess.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/subprocess.meta.json
--rw-r--r--   0        0        0   143431 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sys.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/sys.meta.json
--rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/textwrap.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/textwrap.meta.json
--rw-r--r--   0        0        0    63401 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/threading.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/threading.meta.json
--rw-r--r--   0        0        0    41046 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/time.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/time.meta.json
--rw-r--r--   0        0        0   220699 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/types.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/types.meta.json
--rw-r--r--   0        0        0   398028 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/typing.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/typing.meta.json
--rw-r--r--   0        0        0    73791 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/typing_extensions.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/typing_extensions.meta.json
--rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/warnings.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/warnings.meta.json
--rw-r--r--   0        0        0    66522 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/zipfile.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/zipfile.meta.json
--rw-r--r--   0        0        0    90324 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   403019 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/collections/__init__.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/collections/__init__.meta.json
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/collections/abc.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/collections/abc.meta.json
--rw-r--r--   0        0        0   129025 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/__init__.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/__init__.meta.json
--rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/charset.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/charset.meta.json
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/contentmanager.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/errors.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/errors.meta.json
--rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/header.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/header.meta.json
--rw-r--r--   0        0        0    79312 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/message.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/message.meta.json
--rw-r--r--   0        0        0    30877 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/policy.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/email/policy.meta.json
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70195 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/abc.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/abc.meta.json
--rw-r--r--   0        0        0    65351 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/machinery.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/machinery.meta.json
--rw-r--r--   0        0        0    67599 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/json/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/json/__init__.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/json/decoder.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/json/decoder.meta.json
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/json/encoder.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/json/encoder.meta.json
--rw-r--r--   0        0        0   140791 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/logging/__init__.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/logging/__init__.meta.json
--rw-r--r--   0        0        0  2221259 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/__init__.data.json
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_version.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_version.meta.json
--rw-r--r--   0        0        0   112519 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/version.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/version.meta.json
--rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   260486 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41726 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34743 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261367 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28014 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169674 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36063 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330703 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49564 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301760 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196456 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    45668 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    24451 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52629 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/records.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52762 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    24018 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   154551 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    25937 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   223865 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    47377 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    89096 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    96630 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    96757 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    89059 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    77006 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    97328 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    24864 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26136 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107791 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27681 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136766 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23332 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27003 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   253032 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    66852 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323863 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114213 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   314802 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/os/__init__.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/os/__init__.meta.json
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/os/path.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/os/path.meta.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/__init__.data.json
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/__init__.meta.json
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/algorithms.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/algorithms.meta.json
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/group_testing.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/group_testing.meta.json
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/models.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/models.meta.json
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/symgt/utils.meta.json
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/__init__.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/__init__.meta.json
--rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/_log.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/_log.meta.json
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/async_case.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/async_case.meta.json
--rw-r--r--   0        0        0   205271 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/case.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/case.meta.json
--rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/loader.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/loader.meta.json
--rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/main.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/main.meta.json
--rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/result.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/result.meta.json
--rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/runner.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/runner.meta.json
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/signals.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/signals.meta.json
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/suite.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 symgt-0.0.7/.mypy_cache/3.9/unittest/suite.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1084e237657e9c84
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/10d8b371419046b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1104f03c130ebe17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/11694b85e7ceb18f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/12030af5785462a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/125c491662ec6759
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1387c30be4948c1e
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/139172a1d04f111c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1406495b142569a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/142b3ad340aecc42
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/148366360f53eba
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/14c651b336758ebb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1588a36a7cf894bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/160a8a59236ae3ba
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/16267a8fd146f85e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/16329b066f0bd583
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/17169888c04efbf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/17f5a2000c9cc3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/190b917587a7c715
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/191feee62b4e11ba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1999840ab376cde7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1a9f290d7e746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1bd7a2af896da89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1bdb737b09b6967e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1c46fdbab66d9a5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1cc47fafaf079308
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/1ec41655458704a1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/20118812b6ba52d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/208764f7afde1cbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2123c88bd1974d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/22b6e69dc71d93b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2340b19700a4d682
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/24818994cc746ede
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/24e1cc33e54565ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/276f09acfa09134a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/27c58301c0e5acd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/280f6498566753a8
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/29605448695c5466
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2ab08c94c18dffd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2c14827ec14ea571
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2c20119428eaef29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2c286a340f2aa34d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2c36207032b21c82
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2ce5607f55d6c3d2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2e422062b0466416
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2e4f72d891b1c583
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2f69b8ae8d6a1af6
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2fb9857b45c0fd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2fd14eda1f2186e6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/2fe134354de50e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/300534d19b176f2d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/346d3c8ad9160a9e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/351e1c52599eaade
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/35887b4b936c148b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/35a93401322147ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/35d64af84c840554
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/37f502c8357e13c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/39157434e3fb126b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/39e1ff9480640e0e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3a72fbc406d82784
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3b154c2d1cec0616
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3bfa87c8fdf73a40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3ceb8b67ac1e3b54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3e1429a0441749fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3ea1b58a9db201c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3ea29ca91ddb52ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3f699688bf43f8f2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3fa1a17c80f03bb6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/3ff7d03df56c2c53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4207472e6b4431d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/429b0be494936a73
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/42d8552f51aaba7b
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/433bf4565329474d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/434ff347ecd8136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/445a9c301e6f9922
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/47e8b9593cc01a2d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4922673566a1ee36
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4924663384114806
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/49c65df18b178ba5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/49d78ea2ad1ff125
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4ab47a5e6b0ce4b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4b16d2e9d3162c48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4b8ef09e34a6e6f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4c5bb22783f7485
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4cd3e54afda99d16
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4d48da242c41c251
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4da8e3407a357d79
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4e4a46625e35c15
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4e6c3a36e56edcd7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4f0e733faca1ede3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/4f712e49a203517e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/50628cc21b2693b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/50e745492e64fbfa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/51bc6c2f813c4147
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/525c55305bfaec45
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/52677450217c860f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5415b0de7be808d0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/54d4435e04213bbd
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/54edc30e4f152a52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5626133dcb4a8553
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/564fadc31aaaff26
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5771968da8511143
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/582595bb7a93a07c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/584980681ef79b8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/58da30ac0ef1e914
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/59fa34ac23547310
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5b1c3104b6d49fa7
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5b3817478e0fea4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5b607a9e1c529264
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5becb645be9619b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5d14aab19d73614b
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5dc13b6c60c12647
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5dcb16ea632eb538
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5e78700d4867768f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5ee2a00b44987472
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5f11352e822e4d3b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5f1d792cc4cf9352
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/5fbb01369aa100d3
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/61167eff0eefb0fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/618a6571ecee9116
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/625ee3adf426f2d0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/62ae216b5fa8f055
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/63361b077b4cd691
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/633b01dd53f206fb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/65101181d90f740f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/672303256db69556
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/687736531e4ff9e1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/68d415ae326e7202
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/68e89ae200afae03
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/68fe8c417a600da7
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6984a2e796257436
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6acd8b9654b4733
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6ba5d8344c04c216
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6ce6948f774cb000
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6d608ac54055e791
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6e464cd6d0ac79e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6e68403581b5450e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6edc7aa4bb602eee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/6fa7f8874726d1d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/70c50d94ce87c73
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/70caf455e8092af8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/716f4407f8bdceab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/722353a09ef198b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7279d468cc14f64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7296a018e6eee884
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/739ce25f2139008d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/740202b1b3cafcf6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/741f71c070b1e789
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/756e2156a18c95f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/757dc8d004fd798f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/75c661c946a4f212
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/75f1de43c5a01a66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/764b2aeeb1a42751
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/780c21de8321474c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/788fd5238ad14e80
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/79023d84cdbdccb2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/79abd0627c2bcacb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/79e44453591f4f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7b07818c62c7164f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7d4f8e36ab00b65e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7d4fae75818fdb66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7d61eaea3d9ef118
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7e6c22622d5bae2
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7e85677f179a32fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7e923e725a4524f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7f0b9ccd6df900a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7f4bd0ffbef234b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7f86f736a9393197
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/7fc701bb29e4ca9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/81a87b5b731364cf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/81dd275130bb3aab
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/823ef04562dcffe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/82e947b2b493e786
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8333e1b09076e99e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/83c0a74f7f9f36cc
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/83cc80f689aeb0e9
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/84d4d37f675422df
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/84f449be167ae7ca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/86f6f7623ec62813
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8799049f567c011a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/87aa3aa171354908
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/87bcfdb723a49105
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8be0ca3d1dfd2a4d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8c5ef5f9ec0304e3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8c9b7f30bd8890fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8cd1402b2ed6a498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8cdec151568f9620
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8cec5c0e9a89937e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8e896e417a2d97a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/8f05b3f0602172bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9163bcdb52a16e10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/91c4cfa349ea94a7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9274c18ed7ca2947
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9274cc4b6e089349
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/92c85442d1888809
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/92c8ce56a95a5f1f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9366ab2cb335d10f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/93fc9952d5f794da
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/941677631e46c545
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/943b3ef64129aea0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/945264f05bb524ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/949e97526982b6c1
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/94b91fcec9ba2ff5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/94dc087526f7be97
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/954f916cbc19a590
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/97a0e0123026ece2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/97c8dfd711c8cd5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/987dcb80d3d85036
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/99e1c923468950c9
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/99f1d2d12ed2e065
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9a4c7e19c575ef3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9a75fddda97013a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9ac6a9ef276ffdd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9ba71527bcd3d8d2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9bbe9dc48b8427ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9c0bfeca863efa79
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9c362dc9b7d60ab4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9c85627a25fe8448
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9da40748897d7d1c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/9e49495dad957125
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a0b4bfcb514e3b37
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a1cab7bcfb12c8e6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a2031ae3e3b8bdec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a2272809f12d0ff6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a23b3883903c9835
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a3ef884c778a2446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a4cb8fe5e077df67
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a4d9e2554138ad99
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a4f7a632cc5d259
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a661c25840550379
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a6b46d2dc660c905
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a6d313b912c8881d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a729f14f424b74d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a84f0efbd574bc9e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a8ff131b0669fbb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a982e103f934dc72
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/a9f8a3b7b6f2c386
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/aa90675e23944ae0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ab53134327ceac20
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/abc0d09574d84e17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ac68471a545c78c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ac77bbe64a8ec76b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ad80bb472b0c8e72
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/adf937274b462e10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b10b1e2cfbefc26d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b1922fcb718274a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b309a204e65d936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b3a1073a562e4649
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b3e6f64aef41356f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b41ac728d4354728
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b45df67a50d78b3e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b467385ec7c75659
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b4a04d8a26f2e09e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b4b79c84ca38c89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b4cff5fc09921392
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b5b5df558cad5c02
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b660a372afe52495
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b6bb9950d042daf3
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b7eae2d2e28b3cf4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/b8cf6d0f44e7fd8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/bae1d89444ac0da5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/baf82b7c177bcd74
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/bc47c5f10709d20f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/bc83c58d24b32448
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/be0446b85513b904
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/be35430973bd4acd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/bfb62a4104eab15b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/bfb8c862a3f87b66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c077729fc5e04c13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c2125fc13a78ac43
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c2459e9433efdb77
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c2abd34582b08377
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c2e4d771124137ca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c34f7ec3ec87bed9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c369d3ed21be8e47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c48e6a2f5e461a34
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c5a449924ca7dc16
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c6331437b3900f52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c7605789bc6ed51b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c7995819f0135276
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/c8dfecf945738849
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ca44fc332634dac5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ca45bc20f08a9b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cb846bee59a8a692
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cc0cb344434842b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cc1e5f79cd75f531
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cc45a31c7ce341e0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cec5733ba95e0e82
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cf0e86b6891e853c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cf2ee3702420c8c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/cfae1ce212715249
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d01d1cb9c55b5449
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d0c02fd910364fe2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d0f15f9db29a3305
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d10c937b2529a328
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d1640ca244055386
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d281825a2319859c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d61e6d62c0702de1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d70bf06c6eee23d5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d717803c14d175ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d80e9eb705d1d2a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d8a1efe5a918c9e0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d9458b78c6381b51
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/d9f344e7ff2bb0b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/da5a19f56b8f6d1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/da79a4701567a6e4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dab228a55ae5e659
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dae274ea1d9c2fca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dc49015279137580
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dc9e0757631346a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dd29af601fea4694
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dd7ffba10d230bb2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ddaa030a177fb15b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ddbe7a087cd6104d
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ddc5da72df007c6c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ddff07ec5c4d6998
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/de0dbe297e743771
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/de5fe853340e6a17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/df2b0dba6b763be1
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/df9955adb34a4343
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/dfb4f8a530195f73
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e1b247efa50cc298
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e20e976ab9a11b0f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e2ae383648735d1c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e3440dfd6effe2c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e36622b17a44486c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e371ae52020bdb1c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e371fd2fdea9d57c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e41b924848c9544c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e4db83144022a2e9
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e504bf6f224509f7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e66be7c82afe1fc0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e673a7a7e704bc45
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e71a804f096c5d51
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e858e289b8c427c7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e87047886e38588f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e88b3eaf296e1170
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e89c4b5bdad82e8e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e8c57a50b031ae28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/e8e608cfa0dc40f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ea73b16ff0bfe3d4
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/eaa603b09b9e063
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ec24ffbb3ec32139
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ec676bff4a562d63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ed21d1e13549d12f
--rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ed7cf892f44fb99f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/edac6f15e9c95ffb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/eeb88bdb5d460e88
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ef143d132b1b7ccd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/ef897eebe8e039a0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f1ba9380371848b7
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f1f975d7f1eda925
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f2a2ffa9535b96cd
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f335c26511af9131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f46ad7c0f5ad15f5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f49c1f0addec90a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f5512ddd30af586
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f5753dda1b071ccb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f5dc8524a5209f0a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f643355a40a865f8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f73e8f97bc3833ca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f82a9a188272aaae
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f86a276395fd7136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f8c38c0f42630437
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f8f07e0dd2e7876f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f9800a76eb3f99c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/f9b11d7f2fb4912f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fb612fe627f4238f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fb7d9ed212c385a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fc6bb2a90ba3034c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fc9ebb71114cfe85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fcf04a6f47941b62
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fcff3364fee7c06e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.7/.ruff_cache/content/fd640a0cb54eaf1c
--rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.7/data/X.npy
--rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.7/data/X_shuffled.npy
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 symgt-0.0.7/src/.DS_Store
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/__init__.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/algorithms.py
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/models.py
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/.pytest_cache/README.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.7/src/symgt/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 symgt-0.0.7/tests/01_smoke_test:_IIDModel.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 symgt-0.0.7/tests/02_smoke_test:_ExchangeableModel.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 symgt-0.0.7/tests/03_smoke_test:_algorithms.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 symgt-0.0.7/tests/04_smoke_test:_utils.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 symgt-0.0.7/tests/05_smoke_test:_golden.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 symgt-0.0.7/tests/06_smoke_test:_golden2.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 symgt-0.0.7/.gitignore
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 symgt-0.0.7/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 symgt-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 symgt-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 symgt-0.0.8/.DS_Store
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 symgt-0.0.8/Makefile
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 symgt-0.0.8/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180389 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52421 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    23357 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60697 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137641 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130433 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123338 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109225 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57766 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142229 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    90144 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   132088 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85358 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    52532 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    26818 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87509 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44414 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75218 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167566 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49762 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   162185 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    19574 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64736 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    42830 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239653 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432255 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0    75654 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/zipfile.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/zipfile.meta.json
+-rw-r--r--   0        0        0    89075 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   408009 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129004 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30878 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70600 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64592 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   144406 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2221260 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_version.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112520 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/version.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/version.meta.json
+-rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25413 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   260487 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41727 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34744 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261368 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    28015 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169675 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36064 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330704 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301761 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196446 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    45705 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    25156 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52630 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52763 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21728 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24019 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   154552 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    25938 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   223855 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    63633 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    89097 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    96631 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    96758 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62232 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    89060 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    77007 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0    97329 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    24865 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    26137 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107792 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27682 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136767 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27004 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16481 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13111 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253033 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323864 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114214 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0   322642 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/__init__.data.json
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/__init__.meta.json
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/algorithms.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/algorithms.meta.json
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/models.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/models.meta.json
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/symgt/utils.meta.json
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24089 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9289 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   210175 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/__future__.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/__future__.meta.json
+-rw-r--r--   0        0        0   106758 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_ast.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_ast.meta.json
+-rw-r--r--   0        0        0    51787 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_codecs.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_codecs.meta.json
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_collections_abc.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_ctypes.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_ctypes.meta.json
+-rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_thread.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_thread.meta.json
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_warnings.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_warnings.meta.json
+-rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/abc.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/abc.meta.json
+-rw-r--r--   0        0        0    60660 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/array.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/array.meta.json
+-rw-r--r--   0        0        0   130043 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/ast.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/ast.meta.json
+-rw-r--r--   0        0        0  1028269 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/builtins.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/builtins.meta.json
+-rw-r--r--   0        0        0   123237 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/codecs.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/codecs.meta.json
+-rw-r--r--   0        0        0    92094 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/contextlib.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/contextlib.meta.json
+-rw-r--r--   0        0        0    56115 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/dataclasses.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/dataclasses.meta.json
+-rw-r--r--   0        0        0   141448 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/datetime.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/datetime.meta.json
+-rw-r--r--   0        0        0    61051 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/enum.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/enum.meta.json
+-rw-r--r--   0        0        0   131415 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/functools.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/functools.meta.json
+-rw-r--r--   0        0        0    22419 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/genericpath.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/genericpath.meta.json
+-rw-r--r--   0        0        0    85368 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/io.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/io.meta.json
+-rw-r--r--   0        0        0    51312 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/math.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/math.meta.json
+-rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/mmap.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/mmap.meta.json
+-rw-r--r--   0        0        0    87387 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/pathlib.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/pathlib.meta.json
+-rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/pickle.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/pickle.meta.json
+-rw-r--r--   0        0        0    75098 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/posixpath.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/posixpath.meta.json
+-rw-r--r--   0        0        0   167206 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/re.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/re.meta.json
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sre_compile.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sre_compile.meta.json
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sre_constants.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sre_constants.meta.json
+-rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sre_parse.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sre_parse.meta.json
+-rw-r--r--   0        0        0    26505 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/string.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/string.meta.json
+-rw-r--r--   0        0        0   156601 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/subprocess.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/subprocess.meta.json
+-rw-r--r--   0        0        0   143431 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sys.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/sys.meta.json
+-rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/textwrap.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/textwrap.meta.json
+-rw-r--r--   0        0        0    63401 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/threading.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/threading.meta.json
+-rw-r--r--   0        0        0    41046 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/time.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/time.meta.json
+-rw-r--r--   0        0        0   220699 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/types.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/types.meta.json
+-rw-r--r--   0        0        0   398028 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/typing.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/typing.meta.json
+-rw-r--r--   0        0        0    73791 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/typing_extensions.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/typing_extensions.meta.json
+-rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/warnings.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/warnings.meta.json
+-rw-r--r--   0        0        0    66522 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/zipfile.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/zipfile.meta.json
+-rw-r--r--   0        0        0    90324 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   403019 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/collections/__init__.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/collections/abc.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/collections/abc.meta.json
+-rw-r--r--   0        0        0   129025 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/__init__.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/__init__.meta.json
+-rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/charset.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/charset.meta.json
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/errors.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/errors.meta.json
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/header.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/header.meta.json
+-rw-r--r--   0        0        0    79312 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/message.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/message.meta.json
+-rw-r--r--   0        0        0    30877 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/policy.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/email/policy.meta.json
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70195 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/abc.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/abc.meta.json
+-rw-r--r--   0        0        0    65351 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    67599 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/json/__init__.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/json/__init__.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/json/decoder.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/json/decoder.meta.json
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/json/encoder.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/json/encoder.meta.json
+-rw-r--r--   0        0        0   140791 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/logging/__init__.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2221259 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_version.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112519 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/version.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/version.meta.json
+-rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   260486 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41726 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34743 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261367 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    28014 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169674 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36063 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330703 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49564 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301760 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196456 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    45668 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    24451 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52629 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52762 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24018 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   154551 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    25937 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   223865 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47377 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    89096 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    96630 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    96757 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    89059 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    77006 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0    97328 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    24864 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    26136 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107791 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27681 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136766 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23332 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27003 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253032 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    66852 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323863 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114213 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0   314802 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/os/__init__.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/os/__init__.meta.json
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/os/path.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/os/path.meta.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/__init__.data.json
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/__init__.meta.json
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/algorithms.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/algorithms.meta.json
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/group_testing.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/group_testing.meta.json
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/models.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/models.meta.json
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/symgt/utils.meta.json
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/_log.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/_log.meta.json
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   205271 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/case.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/case.meta.json
+-rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/loader.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/main.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/main.meta.json
+-rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/result.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/result.meta.json
+-rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/runner.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/signals.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/suite.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 symgt-0.0.8/.mypy_cache/3.9/unittest/suite.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1084e237657e9c84
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/10d8b371419046b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1104f03c130ebe17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/11694b85e7ceb18f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/12030af5785462a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/125c491662ec6759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1387c30be4948c1e
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/139172a1d04f111c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1406495b142569a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/142b3ad340aecc42
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/148366360f53eba
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/14c651b336758ebb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1588a36a7cf894bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/160a8a59236ae3ba
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/16267a8fd146f85e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/16329b066f0bd583
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/17169888c04efbf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/17f5a2000c9cc3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/190b917587a7c715
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/191feee62b4e11ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1999840ab376cde7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1a9f290d7e746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1bd7a2af896da89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1bdb737b09b6967e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1c46fdbab66d9a5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1cc47fafaf079308
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/1ec41655458704a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/20118812b6ba52d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/208764f7afde1cbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2123c88bd1974d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/22b6e69dc71d93b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2340b19700a4d682
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/24818994cc746ede
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/24e1cc33e54565ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/276f09acfa09134a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/27c58301c0e5acd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/280f6498566753a8
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/29605448695c5466
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2ab08c94c18dffd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2c14827ec14ea571
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2c20119428eaef29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2c286a340f2aa34d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2c36207032b21c82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2ce5607f55d6c3d2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2e422062b0466416
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2e4f72d891b1c583
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2f69b8ae8d6a1af6
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2fb9857b45c0fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2fd14eda1f2186e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/2fe134354de50e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/300534d19b176f2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/346d3c8ad9160a9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/351e1c52599eaade
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/35887b4b936c148b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/35a93401322147ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/35d64af84c840554
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/37f502c8357e13c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/39157434e3fb126b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/39e1ff9480640e0e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3a72fbc406d82784
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3b154c2d1cec0616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3bfa87c8fdf73a40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3ceb8b67ac1e3b54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3e1429a0441749fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3ea1b58a9db201c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3ea29ca91ddb52ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3f699688bf43f8f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3fa1a17c80f03bb6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/3ff7d03df56c2c53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4207472e6b4431d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/429b0be494936a73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/42d8552f51aaba7b
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/433bf4565329474d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/434ff347ecd8136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/445a9c301e6f9922
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/47e8b9593cc01a2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4922673566a1ee36
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4924663384114806
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/49c65df18b178ba5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/49d78ea2ad1ff125
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4ab47a5e6b0ce4b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4b16d2e9d3162c48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4b8ef09e34a6e6f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4c5bb22783f7485
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4cd3e54afda99d16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4d48da242c41c251
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4da8e3407a357d79
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4e4a46625e35c15
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4e6c3a36e56edcd7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4f0e733faca1ede3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/4f712e49a203517e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/50628cc21b2693b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/50e745492e64fbfa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/51bc6c2f813c4147
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/525c55305bfaec45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/52677450217c860f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5415b0de7be808d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/54d4435e04213bbd
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/54edc30e4f152a52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5626133dcb4a8553
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/564fadc31aaaff26
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5771968da8511143
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/582595bb7a93a07c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/584980681ef79b8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/58da30ac0ef1e914
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/59fa34ac23547310
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5b1c3104b6d49fa7
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5b3817478e0fea4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5b607a9e1c529264
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5becb645be9619b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5d14aab19d73614b
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5dc13b6c60c12647
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5dcb16ea632eb538
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5e78700d4867768f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5ee2a00b44987472
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5f11352e822e4d3b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5f1d792cc4cf9352
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/5fbb01369aa100d3
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/61167eff0eefb0fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/618a6571ecee9116
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/625ee3adf426f2d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/62ae216b5fa8f055
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/63361b077b4cd691
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/633b01dd53f206fb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/65101181d90f740f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/672303256db69556
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/687736531e4ff9e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/68d415ae326e7202
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/68e89ae200afae03
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/68fe8c417a600da7
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6984a2e796257436
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6acd8b9654b4733
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6ba5d8344c04c216
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6ce6948f774cb000
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6d608ac54055e791
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6e464cd6d0ac79e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6e68403581b5450e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6edc7aa4bb602eee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/6fa7f8874726d1d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/70c50d94ce87c73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/70caf455e8092af8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/716f4407f8bdceab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/722353a09ef198b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7279d468cc14f64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7296a018e6eee884
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/739ce25f2139008d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/740202b1b3cafcf6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/741f71c070b1e789
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/756e2156a18c95f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/757dc8d004fd798f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/75c661c946a4f212
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/75f1de43c5a01a66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/764b2aeeb1a42751
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/780c21de8321474c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/788fd5238ad14e80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/79023d84cdbdccb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/79abd0627c2bcacb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/79e44453591f4f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7b07818c62c7164f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7d4f8e36ab00b65e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7d4fae75818fdb66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7d61eaea3d9ef118
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7e6c22622d5bae2
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7e85677f179a32fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7e923e725a4524f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7f0b9ccd6df900a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7f4bd0ffbef234b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7f86f736a9393197
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/7fc701bb29e4ca9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/81a87b5b731364cf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/81dd275130bb3aab
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/823ef04562dcffe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/82e947b2b493e786
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8333e1b09076e99e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/83c0a74f7f9f36cc
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/83cc80f689aeb0e9
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/84d4d37f675422df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/84f449be167ae7ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/86f6f7623ec62813
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8799049f567c011a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/87aa3aa171354908
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/87bcfdb723a49105
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8be0ca3d1dfd2a4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8c5ef5f9ec0304e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8c9b7f30bd8890fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8cd1402b2ed6a498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8cdec151568f9620
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8cec5c0e9a89937e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8e896e417a2d97a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/8f05b3f0602172bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9163bcdb52a16e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/91c4cfa349ea94a7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9274c18ed7ca2947
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9274cc4b6e089349
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/92c85442d1888809
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/92c8ce56a95a5f1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9366ab2cb335d10f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/93fc9952d5f794da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/941677631e46c545
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/943b3ef64129aea0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/945264f05bb524ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/949e97526982b6c1
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/94b91fcec9ba2ff5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/94dc087526f7be97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/954f916cbc19a590
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/97a0e0123026ece2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/97c8dfd711c8cd5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/987dcb80d3d85036
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/99e1c923468950c9
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/99f1d2d12ed2e065
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9a4c7e19c575ef3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9a75fddda97013a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9ac6a9ef276ffdd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9ba71527bcd3d8d2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9bbe9dc48b8427ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9c0bfeca863efa79
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9c362dc9b7d60ab4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9c85627a25fe8448
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9da40748897d7d1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/9e49495dad957125
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a0b4bfcb514e3b37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a1cab7bcfb12c8e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a2031ae3e3b8bdec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a2272809f12d0ff6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a23b3883903c9835
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a3ef884c778a2446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a4cb8fe5e077df67
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a4d9e2554138ad99
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a4f7a632cc5d259
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a661c25840550379
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a6b46d2dc660c905
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a6d313b912c8881d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a729f14f424b74d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a84f0efbd574bc9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a8ff131b0669fbb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a982e103f934dc72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/a9f8a3b7b6f2c386
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/aa90675e23944ae0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ab53134327ceac20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/abc0d09574d84e17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ac68471a545c78c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ac77bbe64a8ec76b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ad80bb472b0c8e72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/adf937274b462e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b10b1e2cfbefc26d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b1922fcb718274a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b309a204e65d936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b3a1073a562e4649
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b3e6f64aef41356f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b41ac728d4354728
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b45df67a50d78b3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b467385ec7c75659
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b4a04d8a26f2e09e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b4b79c84ca38c89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b4cff5fc09921392
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b5b5df558cad5c02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b660a372afe52495
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b6bb9950d042daf3
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b7eae2d2e28b3cf4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/b8cf6d0f44e7fd8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/bae1d89444ac0da5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/baf82b7c177bcd74
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/bc47c5f10709d20f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/bc83c58d24b32448
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/be0446b85513b904
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/be35430973bd4acd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/bfb62a4104eab15b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/bfb8c862a3f87b66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c077729fc5e04c13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c2125fc13a78ac43
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c2459e9433efdb77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c2abd34582b08377
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c2e4d771124137ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c34f7ec3ec87bed9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c369d3ed21be8e47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c48e6a2f5e461a34
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c5a449924ca7dc16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c6331437b3900f52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c7605789bc6ed51b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c7995819f0135276
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/c8dfecf945738849
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ca44fc332634dac5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ca45bc20f08a9b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cb846bee59a8a692
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cc0cb344434842b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cc1e5f79cd75f531
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cc45a31c7ce341e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cec5733ba95e0e82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cf0e86b6891e853c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cf2ee3702420c8c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/cfae1ce212715249
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d01d1cb9c55b5449
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d0c02fd910364fe2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d0f15f9db29a3305
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d10c937b2529a328
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d1640ca244055386
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d281825a2319859c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d61e6d62c0702de1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d70bf06c6eee23d5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d717803c14d175ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d80e9eb705d1d2a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d8a1efe5a918c9e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d9458b78c6381b51
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/d9f344e7ff2bb0b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/da5a19f56b8f6d1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/da79a4701567a6e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dab228a55ae5e659
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dae274ea1d9c2fca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dc49015279137580
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dc9e0757631346a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dd29af601fea4694
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dd7ffba10d230bb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ddaa030a177fb15b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ddbe7a087cd6104d
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ddc5da72df007c6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ddff07ec5c4d6998
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/de0dbe297e743771
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/de5fe853340e6a17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/df2b0dba6b763be1
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/df9955adb34a4343
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/dfb4f8a530195f73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e1b247efa50cc298
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e20e976ab9a11b0f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e2ae383648735d1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e3440dfd6effe2c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e36622b17a44486c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e371ae52020bdb1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e371fd2fdea9d57c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e41b924848c9544c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e4db83144022a2e9
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e504bf6f224509f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e66be7c82afe1fc0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e673a7a7e704bc45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e71a804f096c5d51
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e858e289b8c427c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e87047886e38588f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e88b3eaf296e1170
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e89c4b5bdad82e8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e8c57a50b031ae28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/e8e608cfa0dc40f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ea73b16ff0bfe3d4
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/eaa603b09b9e063
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ec24ffbb3ec32139
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ec676bff4a562d63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ed21d1e13549d12f
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ed7cf892f44fb99f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/edac6f15e9c95ffb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/eeb88bdb5d460e88
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ef143d132b1b7ccd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/ef897eebe8e039a0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f1ba9380371848b7
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f1f975d7f1eda925
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f2a2ffa9535b96cd
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f335c26511af9131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f46ad7c0f5ad15f5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f49c1f0addec90a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f5512ddd30af586
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f5753dda1b071ccb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f5dc8524a5209f0a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f643355a40a865f8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f73e8f97bc3833ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f82a9a188272aaae
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f86a276395fd7136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f8c38c0f42630437
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f8f07e0dd2e7876f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f9800a76eb3f99c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/f9b11d7f2fb4912f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fb612fe627f4238f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fb7d9ed212c385a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fc6bb2a90ba3034c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fc9ebb71114cfe85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fcf04a6f47941b62
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fcff3364fee7c06e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.8/.ruff_cache/content/fd640a0cb54eaf1c
+-rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.8/data/X.npy
+-rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.8/data/X_shuffled.npy
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 symgt-0.0.8/src/.DS_Store
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/__init__.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/algorithms.py
+-rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/py.typed
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/.pytest_cache/README.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.8/src/symgt/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 symgt-0.0.8/tests/01_smoke_test:_IIDModel.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 symgt-0.0.8/tests/02_smoke_test:_ExchangeableModel.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 symgt-0.0.8/tests/03_smoke_test:_algorithms.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 symgt-0.0.8/tests/04_smoke_test:_utils.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 symgt-0.0.8/tests/05_smoke_test:_golden.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 symgt-0.0.8/tests/06_smoke_test:_golden2.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 symgt-0.0.8/.gitignore
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 symgt-0.0.8/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 symgt-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 symgt-0.0.8/PKG-INFO
```

### Comparing `symgt-0.0.7/.DS_Store` & `symgt-0.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/Makefile` & `symgt-0.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/__future__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/__future__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_ast.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_ast.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_codecs.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_codecs.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_collections_abc.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_collections_abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_ctypes.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_ctypes.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_thread.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_thread.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_warnings.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_warnings.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/abc.data.json` & `symgt-0.0.8/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/array.data.json` & `symgt-0.0.8/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/array.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/ast.data.json` & `symgt-0.0.8/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/ast.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/builtins.data.json` & `symgt-0.0.8/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/builtins.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/codecs.data.json` & `symgt-0.0.8/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/codecs.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/contextlib.data.json` & `symgt-0.0.8/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/contextlib.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/dataclasses.data.json` & `symgt-0.0.8/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/dataclasses.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/datetime.data.json` & `symgt-0.0.8/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/datetime.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/enum.data.json` & `symgt-0.0.8/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/enum.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/functools.data.json` & `symgt-0.0.8/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/functools.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/genericpath.data.json` & `symgt-0.0.8/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/genericpath.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/io.data.json` & `symgt-0.0.8/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/io.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/math.data.json` & `symgt-0.0.8/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/math.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/mmap.data.json` & `symgt-0.0.8/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/mmap.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/pathlib.data.json` & `symgt-0.0.8/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/pathlib.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/pickle.data.json` & `symgt-0.0.8/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/pickle.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/posixpath.data.json` & `symgt-0.0.8/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/posixpath.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/re.data.json` & `symgt-0.0.8/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/re.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sre_compile.data.json` & `symgt-0.0.8/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sre_compile.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sre_constants.data.json` & `symgt-0.0.8/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sre_constants.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sre_parse.data.json` & `symgt-0.0.8/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sre_parse.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/string.data.json` & `symgt-0.0.8/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/string.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/subprocess.data.json` & `symgt-0.0.8/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/subprocess.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sys.data.json` & `symgt-0.0.8/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/sys.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/textwrap.data.json` & `symgt-0.0.8/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/textwrap.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/threading.data.json` & `symgt-0.0.8/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/threading.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/time.data.json` & `symgt-0.0.8/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/time.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/types.data.json` & `symgt-0.0.8/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/types.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/typing.data.json` & `symgt-0.0.8/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/typing.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/typing_extensions.data.json` & `symgt-0.0.8/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/typing_extensions.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/warnings.data.json` & `symgt-0.0.8/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/warnings.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/zipfile.data.json` & `symgt-0.0.8/.mypy_cache/3.11/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/zipfile.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_typeshed/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/collections/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/collections/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/collections/abc.data.json` & `symgt-0.0.8/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/collections/abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/ctypes/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/ctypes/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/charset.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/charset.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/contentmanager.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/contentmanager.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/errors.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/errors.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/header.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/header.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/message.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/message.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/policy.data.json` & `symgt-0.0.8/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/email/policy.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/abc.data.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/machinery.data.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/machinery.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/json/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/json/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/json/decoder.data.json` & `symgt-0.0.8/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/json/decoder.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/json/encoder.data.json` & `symgt-0.0.8/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/json/encoder.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/logging/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/logging/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_pytesttester.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_pytesttester.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_version.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_version.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ctypeslib.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ctypeslib.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/version.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/version.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_array_like.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_callable.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_callable.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nbit.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_scalars.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_shape.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_shape.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/compat/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/compat/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/compat/_inspect.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/compat/_inspect.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/compat/py3k.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/compat/py3k.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_asarray.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_asarray.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_internal.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_internal.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_type_aliases.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/arrayprint.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/arrayprint.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/defchararray.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/defchararray.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/einsumfunc.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/fromnumeric.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/function_base.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/function_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/multiarray.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/multiarray.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/numeric.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/numeric.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/numerictypes.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/numerictypes.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/overrides.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/overrides.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/records.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/records.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/shape_base.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/shape_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/umath.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/core/umath.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/fft/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/fft/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/fft/helper.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/fft/helper.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/_version.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/_version.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraypad.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraypad.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraysetops.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arrayterator.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/format.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/format.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/function_base.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/function_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/histograms.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/histograms.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/index_tricks.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/mixins.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/mixins.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/npyio.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/npyio.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/polynomial.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/polynomial.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/scimath.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/scimath.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/shape_base.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/shape_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/twodim_base.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/type_check.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/type_check.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/ufunclike.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/utils.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/lib/utils.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/linalg.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/linalg/linalg.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/core.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/core.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/extras.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/extras.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/mrecords.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/ma/mrecords.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/legendre.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_generator.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_generator.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_mt19937.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_mt19937.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_pcg64.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_pcg64.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_philox.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_philox.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_sfc64.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/_sfc64.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/bit_generator.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/bit_generator.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/mtrand.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/random/mtrand.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/testing/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/testing/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/utils.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/typing/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/numpy/typing/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/os/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/os/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/os/path.data.json` & `symgt-0.0.8/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/os/path.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/algorithms.data.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/algorithms.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/algorithms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/models.data.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/models.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/models.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/models.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/utils.data.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/symgt/utils.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/symgt/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/_log.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/_log.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/async_case.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/async_case.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/case.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/case.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/loader.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/loader.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/main.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/main.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/result.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/result.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/runner.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/runner.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/signals.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/signals.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/suite.data.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.11/unittest/suite.meta.json` & `symgt-0.0.8/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/__future__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/__future__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/__future__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_ast.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_ast.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_codecs.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_codecs.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_collections_abc.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_collections_abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_ctypes.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_ctypes.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_thread.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_thread.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_thread.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_warnings.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_warnings.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/abc.data.json` & `symgt-0.0.8/.mypy_cache/3.9/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/array.data.json` & `symgt-0.0.8/.mypy_cache/3.9/array.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/array.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/array.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/ast.data.json` & `symgt-0.0.8/.mypy_cache/3.9/ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/ast.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/builtins.data.json` & `symgt-0.0.8/.mypy_cache/3.9/builtins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/builtins.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/codecs.data.json` & `symgt-0.0.8/.mypy_cache/3.9/codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/codecs.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/contextlib.data.json` & `symgt-0.0.8/.mypy_cache/3.9/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/contextlib.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/dataclasses.data.json` & `symgt-0.0.8/.mypy_cache/3.9/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/dataclasses.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/datetime.data.json` & `symgt-0.0.8/.mypy_cache/3.9/datetime.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/datetime.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/enum.data.json` & `symgt-0.0.8/.mypy_cache/3.9/enum.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/enum.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/enum.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/functools.data.json` & `symgt-0.0.8/.mypy_cache/3.9/functools.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/functools.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/functools.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/genericpath.data.json` & `symgt-0.0.8/.mypy_cache/3.9/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/genericpath.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/io.data.json` & `symgt-0.0.8/.mypy_cache/3.9/io.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/io.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/io.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/math.data.json` & `symgt-0.0.8/.mypy_cache/3.9/math.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/math.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/math.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/mmap.data.json` & `symgt-0.0.8/.mypy_cache/3.9/mmap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/mmap.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/pathlib.data.json` & `symgt-0.0.8/.mypy_cache/3.9/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/pathlib.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/pickle.data.json` & `symgt-0.0.8/.mypy_cache/3.9/pickle.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/pickle.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/posixpath.data.json` & `symgt-0.0.8/.mypy_cache/3.9/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/posixpath.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/re.data.json` & `symgt-0.0.8/.mypy_cache/3.9/re.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/re.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/re.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sre_compile.data.json` & `symgt-0.0.8/.mypy_cache/3.9/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sre_compile.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sre_constants.data.json` & `symgt-0.0.8/.mypy_cache/3.9/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sre_constants.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sre_parse.data.json` & `symgt-0.0.8/.mypy_cache/3.9/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sre_parse.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/string.data.json` & `symgt-0.0.8/.mypy_cache/3.9/string.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/string.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/string.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/subprocess.data.json` & `symgt-0.0.8/.mypy_cache/3.9/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/subprocess.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sys.data.json` & `symgt-0.0.8/.mypy_cache/3.9/sys.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/sys.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/sys.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/textwrap.data.json` & `symgt-0.0.8/.mypy_cache/3.9/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/textwrap.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/threading.data.json` & `symgt-0.0.8/.mypy_cache/3.9/threading.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/threading.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/threading.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/time.data.json` & `symgt-0.0.8/.mypy_cache/3.9/time.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/time.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/time.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/types.data.json` & `symgt-0.0.8/.mypy_cache/3.9/types.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/types.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/types.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/typing.data.json` & `symgt-0.0.8/.mypy_cache/3.9/typing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/typing.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/typing.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/typing_extensions.data.json` & `symgt-0.0.8/.mypy_cache/3.9/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/typing_extensions.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/warnings.data.json` & `symgt-0.0.8/.mypy_cache/3.9/warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/warnings.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/zipfile.data.json` & `symgt-0.0.8/.mypy_cache/3.9/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/zipfile.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_typeshed/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/_typeshed/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/collections/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/collections/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/collections/abc.data.json` & `symgt-0.0.8/.mypy_cache/3.9/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/collections/abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/ctypes/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/ctypes/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/charset.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/charset.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/contentmanager.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/contentmanager.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/errors.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/errors.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/header.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/header.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/header.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/message.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/message.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/message.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/policy.data.json` & `symgt-0.0.8/.mypy_cache/3.9/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/email/policy.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/abc.data.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/abc.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/machinery.data.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/machinery.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/metadata/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/importlib/metadata/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/json/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/json/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/json/decoder.data.json` & `symgt-0.0.8/.mypy_cache/3.9/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/json/decoder.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/json/encoder.data.json` & `symgt-0.0.8/.mypy_cache/3.9/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/json/encoder.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/logging/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/logging/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_pytesttester.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_pytesttester.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_version.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_version.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ctypeslib.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ctypeslib.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/version.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/version.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_array_like.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_callable.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_callable.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nbit.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_scalars.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_shape.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_shape.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/compat/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/compat/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/compat/_inspect.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/compat/_inspect.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/compat/py3k.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/compat/py3k.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_asarray.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_asarray.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_internal.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_internal.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_type_aliases.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/arrayprint.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/arrayprint.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/defchararray.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/defchararray.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/einsumfunc.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/fromnumeric.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/function_base.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/function_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/multiarray.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/multiarray.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/numeric.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/numeric.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/numerictypes.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/numerictypes.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/overrides.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/overrides.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/records.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/records.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/shape_base.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/shape_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/umath.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/core/umath.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/fft/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/fft/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/fft/helper.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/fft/helper.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/_version.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/_version.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraypad.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraypad.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraysetops.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arrayterator.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/format.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/format.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/function_base.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/function_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/histograms.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/histograms.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/index_tricks.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/mixins.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/mixins.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/npyio.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/npyio.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/polynomial.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/polynomial.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/scimath.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/scimath.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/shape_base.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/shape_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/twodim_base.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/type_check.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/type_check.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/ufunclike.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/utils.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/lib/utils.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/linalg.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/linalg/linalg.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/core.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/core.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/extras.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/extras.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/mrecords.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/ma/mrecords.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/legendre.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_generator.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_generator.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_mt19937.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_mt19937.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_pcg64.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_pcg64.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_philox.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_philox.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_sfc64.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/_sfc64.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/bit_generator.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/bit_generator.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/mtrand.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/random/mtrand.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/testing/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/testing/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/utils.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/typing/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/numpy/typing/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/os/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/os/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/os/path.data.json` & `symgt-0.0.8/.mypy_cache/3.9/os/path.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/os/path.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/algorithms.data.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/algorithms.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/algorithms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/group_testing.data.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/group_testing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/group_testing.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/group_testing.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/models.data.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/models.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/models.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/models.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/utils.data.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/symgt/utils.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/symgt/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/__init__.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/__init__.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/_log.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/_log.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/async_case.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/async_case.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/case.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/case.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/loader.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/loader.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/main.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/main.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/result.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/result.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/runner.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/runner.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/signals.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/signals.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/suite.data.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.mypy_cache/3.9/unittest/suite.meta.json` & `symgt-0.0.8/.mypy_cache/3.9/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/139172a1d04f111c` & `symgt-0.0.8/.ruff_cache/content/139172a1d04f111c`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/14c651b336758ebb` & `symgt-0.0.8/.ruff_cache/content/14c651b336758ebb`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/16267a8fd146f85e` & `symgt-0.0.8/.ruff_cache/content/16267a8fd146f85e`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/29605448695c5466` & `symgt-0.0.8/.ruff_cache/content/29605448695c5466`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/2ab08c94c18dffd8` & `symgt-0.0.8/.ruff_cache/content/2ab08c94c18dffd8`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/2f69b8ae8d6a1af6` & `symgt-0.0.8/.ruff_cache/content/2f69b8ae8d6a1af6`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/2fb9857b45c0fd8` & `symgt-0.0.8/.ruff_cache/content/2fb9857b45c0fd8`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/433bf4565329474d` & `symgt-0.0.8/.ruff_cache/content/433bf4565329474d`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/4924663384114806` & `symgt-0.0.8/.ruff_cache/content/4924663384114806`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/4da8e3407a357d79` & `symgt-0.0.8/.ruff_cache/content/4da8e3407a357d79`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/54edc30e4f152a52` & `symgt-0.0.8/.ruff_cache/content/54edc30e4f152a52`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/5b3817478e0fea4b` & `symgt-0.0.8/.ruff_cache/content/5b3817478e0fea4b`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/5dc13b6c60c12647` & `symgt-0.0.8/.ruff_cache/content/5dc13b6c60c12647`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/5e78700d4867768f` & `symgt-0.0.8/.ruff_cache/content/5e78700d4867768f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/61167eff0eefb0fe` & `symgt-0.0.8/.ruff_cache/content/61167eff0eefb0fe`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/6984a2e796257436` & `symgt-0.0.8/.ruff_cache/content/6984a2e796257436`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/7e85677f179a32fa` & `symgt-0.0.8/.ruff_cache/content/7e85677f179a32fa`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/823ef04562dcffe6` & `symgt-0.0.8/.ruff_cache/content/823ef04562dcffe6`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/83cc80f689aeb0e9` & `symgt-0.0.8/.ruff_cache/content/83cc80f689aeb0e9`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/84d4d37f675422df` & `symgt-0.0.8/.ruff_cache/content/84d4d37f675422df`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/94b91fcec9ba2ff5` & `symgt-0.0.8/.ruff_cache/content/94b91fcec9ba2ff5`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/99f1d2d12ed2e065` & `symgt-0.0.8/.ruff_cache/content/99f1d2d12ed2e065`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/a6b46d2dc660c905` & `symgt-0.0.8/.ruff_cache/content/a6b46d2dc660c905`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/b7eae2d2e28b3cf4` & `symgt-0.0.8/.ruff_cache/content/b7eae2d2e28b3cf4`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/d01d1cb9c55b5449` & `symgt-0.0.8/.ruff_cache/content/d01d1cb9c55b5449`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/d0c02fd910364fe2` & `symgt-0.0.8/.ruff_cache/content/d0c02fd910364fe2`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/d9f344e7ff2bb0b7` & `symgt-0.0.8/.ruff_cache/content/d9f344e7ff2bb0b7`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/ddc5da72df007c6c` & `symgt-0.0.8/.ruff_cache/content/ddc5da72df007c6c`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/df9955adb34a4343` & `symgt-0.0.8/.ruff_cache/content/df9955adb34a4343`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/e20e976ab9a11b0f` & `symgt-0.0.8/.ruff_cache/content/e20e976ab9a11b0f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/e504bf6f224509f7` & `symgt-0.0.8/.ruff_cache/content/e504bf6f224509f7`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/eaa603b09b9e063` & `symgt-0.0.8/.ruff_cache/content/eaa603b09b9e063`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/ec24ffbb3ec32139` & `symgt-0.0.8/.ruff_cache/content/ec24ffbb3ec32139`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/ed7cf892f44fb99f` & `symgt-0.0.8/.ruff_cache/content/ed7cf892f44fb99f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/f1f975d7f1eda925` & `symgt-0.0.8/.ruff_cache/content/f1f975d7f1eda925`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/f2a2ffa9535b96cd` & `symgt-0.0.8/.ruff_cache/content/f2a2ffa9535b96cd`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/f335c26511af9131` & `symgt-0.0.8/.ruff_cache/content/f335c26511af9131`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/f86a276395fd7136` & `symgt-0.0.8/.ruff_cache/content/f86a276395fd7136`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/f8f07e0dd2e7876f` & `symgt-0.0.8/.ruff_cache/content/f8f07e0dd2e7876f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/.ruff_cache/content/fcff3364fee7c06e` & `symgt-0.0.8/.ruff_cache/content/fcff3364fee7c06e`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/data/X.npy` & `symgt-0.0.8/data/X.npy`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/data/X_shuffled.npy` & `symgt-0.0.8/data/X_shuffled.npy`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/src/.DS_Store` & `symgt-0.0.8/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/src/symgt/algorithms.py` & `symgt-0.0.8/src/symgt/algorithms.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/src/symgt/models.py` & `symgt-0.0.8/src/symgt/models.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/src/symgt/utils.py` & `symgt-0.0.8/src/symgt/utils.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/tests/01_smoke_test:_IIDModel.py` & `symgt-0.0.8/tests/01_smoke_test:_IIDModel.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/tests/02_smoke_test:_ExchangeableModel.py` & `symgt-0.0.8/tests/02_smoke_test:_ExchangeableModel.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/tests/03_smoke_test:_algorithms.py` & `symgt-0.0.8/tests/03_smoke_test:_algorithms.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/tests/04_smoke_test:_utils.py` & `symgt-0.0.8/tests/04_smoke_test:_utils.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/tests/05_smoke_test:_golden.py` & `symgt-0.0.8/tests/05_smoke_test:_golden.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/tests/06_smoke_test:_golden2.py` & `symgt-0.0.8/tests/06_smoke_test:_golden2.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/README.md` & `symgt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `symgt-0.0.7/pyproject.toml` & `symgt-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "symgt"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name = "N. C. Landolfi", email="crews.fixture.0f@icloud.com"},
 ]
 description = "A package for group testing against symmetric distributions."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `symgt-0.0.7/PKG-INFO` & `symgt-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symgt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for group testing against symmetric distributions.
 Project-URL: Homepage, https://github.com/nlandolfi/symgt
 Author-email: "N. C. Landolfi" <crews.fixture.0f@icloud.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

