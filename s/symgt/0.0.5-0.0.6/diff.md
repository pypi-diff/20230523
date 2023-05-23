# Comparing `tmp/symgt-0.0.5.tar.gz` & `tmp/symgt-0.0.6.tar.gz`

## Comparing `symgt-0.0.5.tar` & `symgt-0.0.6.tar`

### file list

```diff
@@ -1,983 +1,1033 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 symgt-0.0.5/.DS_Store
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 symgt-0.0.5/Makefile
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 symgt-0.0.5/requirements.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180389 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52421 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    23357 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60697 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137641 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130433 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123338 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109225 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57766 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142229 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    90144 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   132088 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85358 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    52532 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    26818 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87509 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44414 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75218 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167566 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49762 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   162185 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    19574 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64736 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    42830 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239653 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432255 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0    75654 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/zipfile.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/zipfile.meta.json
--rw-r--r--   0        0        0    89075 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   408009 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129004 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30878 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70600 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64592 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   144406 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0  2221260 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/__init__.data.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_version.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_version.meta.json
--rw-r--r--   0        0        0   112520 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/version.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/version.meta.json
--rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25413 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   260487 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41727 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34744 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261368 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28015 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169675 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36064 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330704 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301761 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196446 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    45705 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    25156 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52630 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/records.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52763 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21728 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    24019 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   154552 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    25938 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   223855 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    63633 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    89097 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    96631 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    96758 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    62232 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    89060 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    77007 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    97329 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    24865 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26137 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107792 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27682 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136767 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27004 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16481 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13111 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   253033 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323864 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114214 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   322642 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/__init__.data.json
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/__init__.meta.json
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/algorithms.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/algorithms.meta.json
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/models.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/models.meta.json
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/symgt/utils.meta.json
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24089 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9289 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   210175 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/@plugins_snapshot.json
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/__future__.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/__future__.meta.json
--rw-r--r--   0        0        0   106758 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_ast.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_ast.meta.json
--rw-r--r--   0        0        0    51787 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_codecs.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_codecs.meta.json
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_collections_abc.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_collections_abc.meta.json
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_ctypes.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_ctypes.meta.json
--rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_thread.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_thread.meta.json
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_warnings.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_warnings.meta.json
--rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/abc.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/abc.meta.json
--rw-r--r--   0        0        0    60660 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/array.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/array.meta.json
--rw-r--r--   0        0        0   130043 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/ast.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/ast.meta.json
--rw-r--r--   0        0        0  1028269 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/builtins.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/builtins.meta.json
--rw-r--r--   0        0        0   123237 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/codecs.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/codecs.meta.json
--rw-r--r--   0        0        0    92094 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/contextlib.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/contextlib.meta.json
--rw-r--r--   0        0        0    56115 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/dataclasses.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/dataclasses.meta.json
--rw-r--r--   0        0        0   141448 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/datetime.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/datetime.meta.json
--rw-r--r--   0        0        0    61051 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/enum.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/enum.meta.json
--rw-r--r--   0        0        0   131415 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/functools.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/functools.meta.json
--rw-r--r--   0        0        0    22419 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/genericpath.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/genericpath.meta.json
--rw-r--r--   0        0        0    85368 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/io.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/io.meta.json
--rw-r--r--   0        0        0    51312 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/math.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/math.meta.json
--rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/mmap.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/mmap.meta.json
--rw-r--r--   0        0        0    87387 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/pathlib.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/pathlib.meta.json
--rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/pickle.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/pickle.meta.json
--rw-r--r--   0        0        0    75098 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/posixpath.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/posixpath.meta.json
--rw-r--r--   0        0        0   167206 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/re.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/re.meta.json
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sre_compile.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sre_compile.meta.json
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sre_constants.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sre_constants.meta.json
--rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sre_parse.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sre_parse.meta.json
--rw-r--r--   0        0        0    26505 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/string.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/string.meta.json
--rw-r--r--   0        0        0   156601 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/subprocess.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/subprocess.meta.json
--rw-r--r--   0        0        0   143431 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sys.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/sys.meta.json
--rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/textwrap.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/textwrap.meta.json
--rw-r--r--   0        0        0    63401 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/threading.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/threading.meta.json
--rw-r--r--   0        0        0    41046 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/time.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/time.meta.json
--rw-r--r--   0        0        0   220699 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/types.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/types.meta.json
--rw-r--r--   0        0        0   398028 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/typing.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/typing.meta.json
--rw-r--r--   0        0        0    73791 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/typing_extensions.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/typing_extensions.meta.json
--rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/warnings.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/warnings.meta.json
--rw-r--r--   0        0        0    66522 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/zipfile.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/zipfile.meta.json
--rw-r--r--   0        0        0    90324 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   403019 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/collections/__init__.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/collections/__init__.meta.json
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/collections/abc.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/collections/abc.meta.json
--rw-r--r--   0        0        0   129025 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/__init__.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/__init__.meta.json
--rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/charset.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/charset.meta.json
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/contentmanager.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/errors.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/errors.meta.json
--rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/header.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/header.meta.json
--rw-r--r--   0        0        0    79312 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/message.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/message.meta.json
--rw-r--r--   0        0        0    30877 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/policy.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/email/policy.meta.json
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70195 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/abc.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/abc.meta.json
--rw-r--r--   0        0        0    65351 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/machinery.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/machinery.meta.json
--rw-r--r--   0        0        0    67599 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/json/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/json/__init__.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/json/decoder.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/json/decoder.meta.json
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/json/encoder.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/json/encoder.meta.json
--rw-r--r--   0        0        0   140791 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/logging/__init__.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/logging/__init__.meta.json
--rw-r--r--   0        0        0  2221259 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/__init__.data.json
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_version.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_version.meta.json
--rw-r--r--   0        0        0   112519 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/version.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/version.meta.json
--rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   260486 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41726 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34743 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261367 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28014 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169674 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36063 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330703 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49564 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301760 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196456 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    45668 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    24451 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52629 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/records.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52762 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    24018 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   154551 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    25937 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   223865 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    47377 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    89096 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    96630 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    96757 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    89059 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    77006 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    97328 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    24864 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26136 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107791 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27681 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136766 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23332 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27003 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   253032 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    66852 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323863 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114213 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   314802 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/os/__init__.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/os/__init__.meta.json
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/os/path.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/os/path.meta.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/__init__.data.json
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/__init__.meta.json
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/algorithms.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/algorithms.meta.json
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/group_testing.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/group_testing.meta.json
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/models.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/models.meta.json
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/symgt/utils.meta.json
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/__init__.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/__init__.meta.json
--rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/_log.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/_log.meta.json
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/async_case.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/async_case.meta.json
--rw-r--r--   0        0        0   205271 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/case.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/case.meta.json
--rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/loader.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/loader.meta.json
--rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/main.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/main.meta.json
--rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/result.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/result.meta.json
--rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/runner.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/runner.meta.json
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/signals.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/signals.meta.json
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/suite.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 symgt-0.0.5/.mypy_cache/3.9/unittest/suite.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1084e237657e9c84
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/11694b85e7ceb18f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/12030af5785462a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/125c491662ec6759
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1387c30be4948c1e
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/139172a1d04f111c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1406495b142569a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/142b3ad340aecc42
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/148366360f53eba
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/14c651b336758ebb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/160a8a59236ae3ba
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/16267a8fd146f85e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/16329b066f0bd583
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/17169888c04efbf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/17f5a2000c9cc3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/190b917587a7c715
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/191feee62b4e11ba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1bd7a2af896da89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1bdb737b09b6967e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1c46fdbab66d9a5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1cc47fafaf079308
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/1ec41655458704a1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/20118812b6ba52d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/208764f7afde1cbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2123c88bd1974d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/22b6e69dc71d93b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2340b19700a4d682
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/24818994cc746ede
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/24e1cc33e54565ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/276f09acfa09134a
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/29605448695c5466
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2ab08c94c18dffd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2c14827ec14ea571
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2c20119428eaef29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2ce5607f55d6c3d2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2e4f72d891b1c583
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2f69b8ae8d6a1af6
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2fb9857b45c0fd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/2fd14eda1f2186e6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/300534d19b176f2d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/351e1c52599eaade
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/35a93401322147ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/37f502c8357e13c2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/39157434e3fb126b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/39e1ff9480640e0e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3a72fbc406d82784
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3b154c2d1cec0616
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3bfa87c8fdf73a40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3ceb8b67ac1e3b54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3e1429a0441749fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3ea1b58a9db201c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3ea29ca91ddb52ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3fa1a17c80f03bb6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/3ff7d03df56c2c53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/429b0be494936a73
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/434ff347ecd8136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/445a9c301e6f9922
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/47e8b9593cc01a2d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4922673566a1ee36
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4924663384114806
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/49c65df18b178ba5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/49d78ea2ad1ff125
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4ab47a5e6b0ce4b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4b16d2e9d3162c48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4c5bb22783f7485
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4cd3e54afda99d16
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4d48da242c41c251
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4da8e3407a357d79
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4e4a46625e35c15
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4e6c3a36e56edcd7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4f0e733faca1ede3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/4f712e49a203517e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/50e745492e64fbfa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/51bc6c2f813c4147
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/525c55305bfaec45
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/52677450217c860f
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/54edc30e4f152a52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5626133dcb4a8553
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/564fadc31aaaff26
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5771968da8511143
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/582595bb7a93a07c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/584980681ef79b8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/58da30ac0ef1e914
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/59fa34ac23547310
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5b1c3104b6d49fa7
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5b3817478e0fea4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5b607a9e1c529264
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5becb645be9619b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5d14aab19d73614b
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5dc13b6c60c12647
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5e78700d4867768f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5ee2a00b44987472
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5f11352e822e4d3b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5f1d792cc4cf9352
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/5fbb01369aa100d3
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/61167eff0eefb0fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/618a6571ecee9116
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/62ae216b5fa8f055
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/63361b077b4cd691
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/633b01dd53f206fb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/65101181d90f740f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/687736531e4ff9e1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/68e89ae200afae03
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/68fe8c417a600da7
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6984a2e796257436
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6acd8b9654b4733
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6ba5d8344c04c216
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6ce6948f774cb000
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6d608ac54055e791
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6e464cd6d0ac79e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6edc7aa4bb602eee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/6fa7f8874726d1d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/70c50d94ce87c73
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/70caf455e8092af8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/716f4407f8bdceab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/722353a09ef198b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7296a018e6eee884
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/739ce25f2139008d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/740202b1b3cafcf6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/741f71c070b1e789
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/756e2156a18c95f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/757dc8d004fd798f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/75c661c946a4f212
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/788fd5238ad14e80
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/79023d84cdbdccb2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/79abd0627c2bcacb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/79e44453591f4f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7b07818c62c7164f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7d4f8e36ab00b65e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7d4fae75818fdb66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7d61eaea3d9ef118
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7e6c22622d5bae2
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7e85677f179a32fa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7e923e725a4524f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7f0b9ccd6df900a6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/7f86f736a9393197
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/81dd275130bb3aab
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/823ef04562dcffe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/82e947b2b493e786
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/8333e1b09076e99e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/83c0a74f7f9f36cc
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/83cc80f689aeb0e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/84f449be167ae7ca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/86f6f7623ec62813
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/8799049f567c011a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/87aa3aa171354908
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/87bcfdb723a49105
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/8c9b7f30bd8890fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/8cec5c0e9a89937e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/8e896e417a2d97a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/8f05b3f0602172bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9163bcdb52a16e10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9274c18ed7ca2947
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9274cc4b6e089349
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/92c85442d1888809
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/92c8ce56a95a5f1f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9366ab2cb335d10f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/93fc9952d5f794da
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/943b3ef64129aea0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/945264f05bb524ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/949e97526982b6c1
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/94b91fcec9ba2ff5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/94dc087526f7be97
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/954f916cbc19a590
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/97c8dfd711c8cd5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/987dcb80d3d85036
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/99e1c923468950c9
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/99f1d2d12ed2e065
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9a75fddda97013a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9ac6a9ef276ffdd4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9bbe9dc48b8427ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9c85627a25fe8448
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/9e49495dad957125
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a0b4bfcb514e3b37
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a1cab7bcfb12c8e6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a23b3883903c9835
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a3ef884c778a2446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a4cb8fe5e077df67
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a4d9e2554138ad99
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a6b46d2dc660c905
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a6d313b912c8881d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a729f14f424b74d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a84f0efbd574bc9e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a8ff131b0669fbb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/a982e103f934dc72
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/aa90675e23944ae0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ab53134327ceac20
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/abc0d09574d84e17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ac68471a545c78c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ac77bbe64a8ec76b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ad80bb472b0c8e72
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/adf937274b462e10
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b10b1e2cfbefc26d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b1922fcb718274a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b309a204e65d936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b3e6f64aef41356f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b41ac728d4354728
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b45df67a50d78b3e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b4a04d8a26f2e09e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b4b79c84ca38c89
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b4cff5fc09921392
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b5b5df558cad5c02
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b660a372afe52495
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/b8cf6d0f44e7fd8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/bae1d89444ac0da5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/baf82b7c177bcd74
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/bc47c5f10709d20f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/be0446b85513b904
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/be35430973bd4acd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/bfb62a4104eab15b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/bfb8c862a3f87b66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c077729fc5e04c13
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c2459e9433efdb77
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c2abd34582b08377
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c2e4d771124137ca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c34f7ec3ec87bed9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c369d3ed21be8e47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c5a449924ca7dc16
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c6331437b3900f52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c7995819f0135276
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/c8dfecf945738849
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ca44fc332634dac5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ca45bc20f08a9b2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cb846bee59a8a692
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cc0cb344434842b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cc1e5f79cd75f531
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cc45a31c7ce341e0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cec5733ba95e0e82
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cf0e86b6891e853c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cf2ee3702420c8c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/cfae1ce212715249
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d01d1cb9c55b5449
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d0c02fd910364fe2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d10c937b2529a328
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d281825a2319859c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d61e6d62c0702de1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d70bf06c6eee23d5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d80e9eb705d1d2a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d8a1efe5a918c9e0
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/d9f344e7ff2bb0b7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dab228a55ae5e659
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dae274ea1d9c2fca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dc49015279137580
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dc9e0757631346a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dd29af601fea4694
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dd7ffba10d230bb2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ddaa030a177fb15b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/de0dbe297e743771
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/de5fe853340e6a17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/df2b0dba6b763be1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/dfb4f8a530195f73
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e20e976ab9a11b0f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e2ae383648735d1c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e3440dfd6effe2c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e371ae52020bdb1c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e371fd2fdea9d57c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e41b924848c9544c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e4db83144022a2e9
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e504bf6f224509f7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e66be7c82afe1fc0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e673a7a7e704bc45
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e71a804f096c5d51
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e858e289b8c427c7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e87047886e38588f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e88b3eaf296e1170
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e89c4b5bdad82e8e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e8c57a50b031ae28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/e8e608cfa0dc40f4
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/eaa603b09b9e063
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ec24ffbb3ec32139
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ed21d1e13549d12f
--rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ed7cf892f44fb99f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/edac6f15e9c95ffb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/eeb88bdb5d460e88
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ef143d132b1b7ccd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/ef897eebe8e039a0
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f1f975d7f1eda925
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f2a2ffa9535b96cd
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f335c26511af9131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f46ad7c0f5ad15f5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f49c1f0addec90a5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f643355a40a865f8
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f86a276395fd7136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f8c38c0f42630437
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f8f07e0dd2e7876f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/f9800a76eb3f99c8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/fb612fe627f4238f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/fb7d9ed212c385a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/fc6bb2a90ba3034c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/fc9ebb71114cfe85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.5/.ruff_cache/content/fcf04a6f47941b62
--rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.5/data/X.npy
--rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.5/data/X_shuffled.npy
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 symgt-0.0.5/src/.DS_Store
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/__init__.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/algorithms.py
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/models.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/.pytest_cache/README.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.5/src/symgt/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 symgt-0.0.5/tests/01_smoke_test:_IIDModel.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 symgt-0.0.5/tests/02_smoke_test:_ExchangeableModel.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 symgt-0.0.5/tests/03_smoke_test:_algorithms.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 symgt-0.0.5/tests/04_smoke_test:_utils.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 symgt-0.0.5/tests/05_smoke_test:_golden.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 symgt-0.0.5/tests/06_smoke_test:_golden2.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 symgt-0.0.5/.gitignore
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 symgt-0.0.5/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 symgt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 symgt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 symgt-0.0.6/.DS_Store
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 symgt-0.0.6/Makefile
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 symgt-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180389 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52421 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    23357 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60697 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137641 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130433 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123338 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109225 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57766 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142229 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    90144 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   132088 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85358 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    52532 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    26818 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87509 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44414 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75218 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167566 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28501 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49762 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   162185 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    19574 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64736 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    42830 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239653 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432255 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    23810 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0    75654 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/zipfile.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/zipfile.meta.json
+-rw-r--r--   0        0        0    89075 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   408009 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129004 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30878 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70600 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64592 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91140 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14525 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   144406 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2221260 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_version.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112520 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/version.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/version.meta.json
+-rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25413 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   260487 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41727 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34744 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261368 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    28015 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169675 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36064 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330704 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301761 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196446 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    45705 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    25156 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52630 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52763 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21728 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24019 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   154552 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    25938 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   223855 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    63633 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    89097 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    96631 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    96758 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62232 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    89060 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    77007 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0    97329 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    24865 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    26137 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107792 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27682 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136767 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27004 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16481 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14032 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13111 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253033 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323864 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114214 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0   322642 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/__init__.data.json
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/__init__.meta.json
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/algorithms.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/algorithms.meta.json
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/models.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/models.meta.json
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/symgt/utils.meta.json
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24089 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9289 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   210175 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/__future__.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/__future__.meta.json
+-rw-r--r--   0        0        0   106758 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_ast.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_ast.meta.json
+-rw-r--r--   0        0        0    51787 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_codecs.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_codecs.meta.json
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_collections_abc.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_ctypes.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_ctypes.meta.json
+-rw-r--r--   0        0        0    22800 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_thread.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_thread.meta.json
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_warnings.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_warnings.meta.json
+-rw-r--r--   0        0        0    22331 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/abc.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/abc.meta.json
+-rw-r--r--   0        0        0    60660 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/array.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/array.meta.json
+-rw-r--r--   0        0        0   130043 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/ast.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/ast.meta.json
+-rw-r--r--   0        0        0  1028269 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/builtins.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/builtins.meta.json
+-rw-r--r--   0        0        0   123237 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/codecs.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/codecs.meta.json
+-rw-r--r--   0        0        0    92094 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/contextlib.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/contextlib.meta.json
+-rw-r--r--   0        0        0    56115 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/dataclasses.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/dataclasses.meta.json
+-rw-r--r--   0        0        0   141448 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/datetime.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/datetime.meta.json
+-rw-r--r--   0        0        0    61051 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/enum.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/enum.meta.json
+-rw-r--r--   0        0        0   131415 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/functools.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/functools.meta.json
+-rw-r--r--   0        0        0    22419 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/genericpath.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/genericpath.meta.json
+-rw-r--r--   0        0        0    85368 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/io.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/io.meta.json
+-rw-r--r--   0        0        0    51312 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/math.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/math.meta.json
+-rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/mmap.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/mmap.meta.json
+-rw-r--r--   0        0        0    87387 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/pathlib.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/pathlib.meta.json
+-rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/pickle.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/pickle.meta.json
+-rw-r--r--   0        0        0    75098 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/posixpath.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/posixpath.meta.json
+-rw-r--r--   0        0        0   167206 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/re.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/re.meta.json
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sre_compile.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sre_compile.meta.json
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sre_constants.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sre_constants.meta.json
+-rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sre_parse.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sre_parse.meta.json
+-rw-r--r--   0        0        0    26505 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/string.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/string.meta.json
+-rw-r--r--   0        0        0   156601 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/subprocess.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/subprocess.meta.json
+-rw-r--r--   0        0        0   143431 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sys.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/sys.meta.json
+-rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/textwrap.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/textwrap.meta.json
+-rw-r--r--   0        0        0    63401 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/threading.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/threading.meta.json
+-rw-r--r--   0        0        0    41046 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/time.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/time.meta.json
+-rw-r--r--   0        0        0   220699 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/types.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/types.meta.json
+-rw-r--r--   0        0        0   398028 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/typing.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/typing.meta.json
+-rw-r--r--   0        0        0    73791 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/typing_extensions.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/typing_extensions.meta.json
+-rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/warnings.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/warnings.meta.json
+-rw-r--r--   0        0        0    66522 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/zipfile.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/zipfile.meta.json
+-rw-r--r--   0        0        0    90324 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   403019 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/collections/__init__.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/collections/abc.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/collections/abc.meta.json
+-rw-r--r--   0        0        0   129025 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/__init__.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/__init__.meta.json
+-rw-r--r--   0        0        0    12220 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/charset.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/charset.meta.json
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/errors.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/errors.meta.json
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/header.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/header.meta.json
+-rw-r--r--   0        0        0    79312 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/message.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/message.meta.json
+-rw-r--r--   0        0        0    30877 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/policy.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/email/policy.meta.json
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70195 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/abc.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/abc.meta.json
+-rw-r--r--   0        0        0    65351 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    67599 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/json/__init__.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/json/__init__.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/json/decoder.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/json/decoder.meta.json
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/json/encoder.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/json/encoder.meta.json
+-rw-r--r--   0        0        0   140791 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/logging/__init__.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2221259 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_version.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112519 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/version.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/version.meta.json
+-rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25412 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   260486 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41726 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30706 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34743 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261367 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    28014 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169674 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36063 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330703 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49564 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301760 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196456 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    45668 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    24451 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52629 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52762 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18756 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    24018 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     8962 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   154551 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    25937 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   223865 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    47377 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    89096 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    96630 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0    96757 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    89059 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    77006 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0    97328 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    24864 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    26136 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107791 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27681 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136766 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23332 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27003 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14192 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14031 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13110 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   253032 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15472 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    66852 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323863 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114213 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0   314802 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/os/__init__.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/os/__init__.meta.json
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/os/path.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/os/path.meta.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/__init__.data.json
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/__init__.meta.json
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/algorithms.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/algorithms.meta.json
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/group_testing.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/group_testing.meta.json
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/models.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/models.meta.json
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/symgt/utils.meta.json
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/_log.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/_log.meta.json
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   205271 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/case.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/case.meta.json
+-rw-r--r--   0        0        0    14649 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/loader.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/main.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/main.meta.json
+-rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/result.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/result.meta.json
+-rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/runner.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/signals.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/suite.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 symgt-0.0.6/.mypy_cache/3.9/unittest/suite.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1084e237657e9c84
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1104f03c130ebe17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/11694b85e7ceb18f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/12030af5785462a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/125c491662ec6759
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1387c30be4948c1e
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/139172a1d04f111c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1406495b142569a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/142b3ad340aecc42
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/148366360f53eba
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/14c651b336758ebb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/160a8a59236ae3ba
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/16267a8fd146f85e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/16329b066f0bd583
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/17169888c04efbf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/17f5a2000c9cc3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/190b917587a7c715
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/191feee62b4e11ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1bd7a2af896da89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1bdb737b09b6967e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1c46fdbab66d9a5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1cc47fafaf079308
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/1ec41655458704a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/20118812b6ba52d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/208764f7afde1cbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2123c88bd1974d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/22b6e69dc71d93b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2340b19700a4d682
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/24818994cc746ede
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/24e1cc33e54565ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/276f09acfa09134a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/27c58301c0e5acd6
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/29605448695c5466
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2ab08c94c18dffd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2c14827ec14ea571
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2c20119428eaef29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2c286a340f2aa34d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2ce5607f55d6c3d2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2e422062b0466416
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2e4f72d891b1c583
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2f69b8ae8d6a1af6
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2fb9857b45c0fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/2fd14eda1f2186e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/300534d19b176f2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/346d3c8ad9160a9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/351e1c52599eaade
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/35887b4b936c148b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/35a93401322147ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/37f502c8357e13c2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/39157434e3fb126b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/39e1ff9480640e0e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3a72fbc406d82784
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3b154c2d1cec0616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3bfa87c8fdf73a40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3ceb8b67ac1e3b54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3e1429a0441749fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3ea1b58a9db201c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3ea29ca91ddb52ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3f699688bf43f8f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3fa1a17c80f03bb6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/3ff7d03df56c2c53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4207472e6b4431d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/429b0be494936a73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/42d8552f51aaba7b
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/433bf4565329474d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/434ff347ecd8136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/445a9c301e6f9922
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/47e8b9593cc01a2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4922673566a1ee36
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4924663384114806
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/49c65df18b178ba5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/49d78ea2ad1ff125
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4ab47a5e6b0ce4b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4b16d2e9d3162c48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4b8ef09e34a6e6f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4c5bb22783f7485
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4cd3e54afda99d16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4d48da242c41c251
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4da8e3407a357d79
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4e4a46625e35c15
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4e6c3a36e56edcd7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4f0e733faca1ede3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/4f712e49a203517e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/50628cc21b2693b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/50e745492e64fbfa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/51bc6c2f813c4147
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/525c55305bfaec45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/52677450217c860f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5415b0de7be808d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/54d4435e04213bbd
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/54edc30e4f152a52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5626133dcb4a8553
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/564fadc31aaaff26
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5771968da8511143
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/582595bb7a93a07c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/584980681ef79b8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/58da30ac0ef1e914
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/59fa34ac23547310
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5b1c3104b6d49fa7
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5b3817478e0fea4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5b607a9e1c529264
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5becb645be9619b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5d14aab19d73614b
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5dc13b6c60c12647
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5e78700d4867768f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5ee2a00b44987472
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5f11352e822e4d3b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5f1d792cc4cf9352
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/5fbb01369aa100d3
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/61167eff0eefb0fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/618a6571ecee9116
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/625ee3adf426f2d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/62ae216b5fa8f055
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/63361b077b4cd691
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/633b01dd53f206fb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/65101181d90f740f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/672303256db69556
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/687736531e4ff9e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/68e89ae200afae03
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/68fe8c417a600da7
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6984a2e796257436
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6acd8b9654b4733
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6ba5d8344c04c216
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6ce6948f774cb000
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6d608ac54055e791
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6e464cd6d0ac79e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6e68403581b5450e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6edc7aa4bb602eee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/6fa7f8874726d1d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/70c50d94ce87c73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/70caf455e8092af8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/716f4407f8bdceab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/722353a09ef198b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7279d468cc14f64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7296a018e6eee884
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/739ce25f2139008d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/740202b1b3cafcf6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/741f71c070b1e789
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/756e2156a18c95f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/757dc8d004fd798f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/75c661c946a4f212
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/75f1de43c5a01a66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/764b2aeeb1a42751
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/788fd5238ad14e80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/79023d84cdbdccb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/79abd0627c2bcacb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/79e44453591f4f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7b07818c62c7164f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7d4f8e36ab00b65e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7d4fae75818fdb66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7d61eaea3d9ef118
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7e6c22622d5bae2
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7e85677f179a32fa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7e923e725a4524f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7f0b9ccd6df900a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7f4bd0ffbef234b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7f86f736a9393197
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/7fc701bb29e4ca9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/81a87b5b731364cf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/81dd275130bb3aab
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/823ef04562dcffe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/82e947b2b493e786
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8333e1b09076e99e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/83c0a74f7f9f36cc
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/83cc80f689aeb0e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/84f449be167ae7ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/86f6f7623ec62813
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8799049f567c011a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/87aa3aa171354908
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/87bcfdb723a49105
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8c5ef5f9ec0304e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8c9b7f30bd8890fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8cdec151568f9620
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8cec5c0e9a89937e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8e896e417a2d97a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/8f05b3f0602172bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9163bcdb52a16e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/91c4cfa349ea94a7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9274c18ed7ca2947
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9274cc4b6e089349
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/92c85442d1888809
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/92c8ce56a95a5f1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9366ab2cb335d10f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/93fc9952d5f794da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/943b3ef64129aea0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/945264f05bb524ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/949e97526982b6c1
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/94b91fcec9ba2ff5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/94dc087526f7be97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/954f916cbc19a590
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/97c8dfd711c8cd5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/987dcb80d3d85036
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/99e1c923468950c9
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/99f1d2d12ed2e065
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9a75fddda97013a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9ac6a9ef276ffdd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9ba71527bcd3d8d2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9bbe9dc48b8427ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9c362dc9b7d60ab4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9c85627a25fe8448
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/9e49495dad957125
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a0b4bfcb514e3b37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a1cab7bcfb12c8e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a2031ae3e3b8bdec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a2272809f12d0ff6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a23b3883903c9835
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a3ef884c778a2446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a4cb8fe5e077df67
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a4d9e2554138ad99
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a4f7a632cc5d259
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a6b46d2dc660c905
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a6d313b912c8881d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a729f14f424b74d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a84f0efbd574bc9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a8ff131b0669fbb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/a982e103f934dc72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/aa90675e23944ae0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ab53134327ceac20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/abc0d09574d84e17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ac68471a545c78c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ac77bbe64a8ec76b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ad80bb472b0c8e72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/adf937274b462e10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b10b1e2cfbefc26d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b1922fcb718274a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b309a204e65d936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b3a1073a562e4649
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b3e6f64aef41356f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b41ac728d4354728
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b45df67a50d78b3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b467385ec7c75659
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b4a04d8a26f2e09e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b4b79c84ca38c89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b4cff5fc09921392
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b5b5df558cad5c02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b660a372afe52495
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b7eae2d2e28b3cf4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/b8cf6d0f44e7fd8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/bae1d89444ac0da5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/baf82b7c177bcd74
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/bc47c5f10709d20f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/bc83c58d24b32448
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/be0446b85513b904
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/be35430973bd4acd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/bfb62a4104eab15b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/bfb8c862a3f87b66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c077729fc5e04c13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c2125fc13a78ac43
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c2459e9433efdb77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c2abd34582b08377
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c2e4d771124137ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c34f7ec3ec87bed9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c369d3ed21be8e47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c48e6a2f5e461a34
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c5a449924ca7dc16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c6331437b3900f52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c7605789bc6ed51b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c7995819f0135276
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/c8dfecf945738849
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ca44fc332634dac5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ca45bc20f08a9b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cb846bee59a8a692
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cc0cb344434842b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cc1e5f79cd75f531
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cc45a31c7ce341e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cec5733ba95e0e82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cf0e86b6891e853c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cf2ee3702420c8c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/cfae1ce212715249
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d01d1cb9c55b5449
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d0c02fd910364fe2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d0f15f9db29a3305
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d10c937b2529a328
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d281825a2319859c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d61e6d62c0702de1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d70bf06c6eee23d5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d717803c14d175ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d80e9eb705d1d2a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d8a1efe5a918c9e0
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/d9f344e7ff2bb0b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/da5a19f56b8f6d1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dab228a55ae5e659
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dae274ea1d9c2fca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dc49015279137580
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dc9e0757631346a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dd29af601fea4694
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dd7ffba10d230bb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ddaa030a177fb15b
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ddc5da72df007c6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/de0dbe297e743771
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/de5fe853340e6a17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/df2b0dba6b763be1
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/df9955adb34a4343
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/dfb4f8a530195f73
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e1b247efa50cc298
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e20e976ab9a11b0f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e2ae383648735d1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e3440dfd6effe2c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e36622b17a44486c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e371ae52020bdb1c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e371fd2fdea9d57c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e41b924848c9544c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e4db83144022a2e9
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e504bf6f224509f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e66be7c82afe1fc0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e673a7a7e704bc45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e71a804f096c5d51
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e858e289b8c427c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e87047886e38588f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e88b3eaf296e1170
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e89c4b5bdad82e8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e8c57a50b031ae28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/e8e608cfa0dc40f4
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/eaa603b09b9e063
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ec24ffbb3ec32139
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ec676bff4a562d63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ed21d1e13549d12f
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ed7cf892f44fb99f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/edac6f15e9c95ffb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/eeb88bdb5d460e88
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ef143d132b1b7ccd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/ef897eebe8e039a0
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f1f975d7f1eda925
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f2a2ffa9535b96cd
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f335c26511af9131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f46ad7c0f5ad15f5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f49c1f0addec90a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f5512ddd30af586
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f5753dda1b071ccb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f643355a40a865f8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f82a9a188272aaae
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f86a276395fd7136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f8c38c0f42630437
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f8f07e0dd2e7876f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/f9800a76eb3f99c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/fb612fe627f4238f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/fb7d9ed212c385a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/fc6bb2a90ba3034c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/fc9ebb71114cfe85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/fcf04a6f47941b62
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 symgt-0.0.6/.ruff_cache/content/fcff3364fee7c06e
+-rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.6/data/X.npy
+-rw-r--r--   0        0        0   320128 2020-02-02 00:00:00.000000 symgt-0.0.6/data/X_shuffled.npy
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 symgt-0.0.6/src/.DS_Store
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/__init__.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/algorithms.py
+-rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/models.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/.pytest_cache/README.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 symgt-0.0.6/src/symgt/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 symgt-0.0.6/tests/01_smoke_test:_IIDModel.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 symgt-0.0.6/tests/02_smoke_test:_ExchangeableModel.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 symgt-0.0.6/tests/03_smoke_test:_algorithms.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 symgt-0.0.6/tests/04_smoke_test:_utils.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 symgt-0.0.6/tests/05_smoke_test:_golden.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 symgt-0.0.6/tests/06_smoke_test:_golden2.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 symgt-0.0.6/.gitignore
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 symgt-0.0.6/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 symgt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 symgt-0.0.6/PKG-INFO
```

### Comparing `symgt-0.0.5/.DS_Store` & `symgt-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/Makefile` & `symgt-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/__future__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/__future__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_ast.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_ast.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_codecs.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_codecs.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_collections_abc.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_collections_abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_ctypes.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_ctypes.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_thread.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_thread.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_warnings.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_warnings.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/abc.data.json` & `symgt-0.0.6/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/array.data.json` & `symgt-0.0.6/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/array.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/ast.data.json` & `symgt-0.0.6/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/ast.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/builtins.data.json` & `symgt-0.0.6/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/builtins.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/codecs.data.json` & `symgt-0.0.6/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/codecs.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/contextlib.data.json` & `symgt-0.0.6/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/contextlib.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/dataclasses.data.json` & `symgt-0.0.6/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/dataclasses.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/datetime.data.json` & `symgt-0.0.6/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/datetime.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/enum.data.json` & `symgt-0.0.6/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/enum.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/functools.data.json` & `symgt-0.0.6/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/functools.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/genericpath.data.json` & `symgt-0.0.6/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/genericpath.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/io.data.json` & `symgt-0.0.6/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/io.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/math.data.json` & `symgt-0.0.6/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/math.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/mmap.data.json` & `symgt-0.0.6/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/mmap.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/pathlib.data.json` & `symgt-0.0.6/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/pathlib.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/pickle.data.json` & `symgt-0.0.6/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/pickle.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/posixpath.data.json` & `symgt-0.0.6/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/posixpath.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/re.data.json` & `symgt-0.0.6/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/re.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sre_compile.data.json` & `symgt-0.0.6/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sre_compile.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sre_constants.data.json` & `symgt-0.0.6/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sre_constants.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sre_parse.data.json` & `symgt-0.0.6/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sre_parse.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/string.data.json` & `symgt-0.0.6/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/string.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/subprocess.data.json` & `symgt-0.0.6/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/subprocess.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sys.data.json` & `symgt-0.0.6/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/sys.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/textwrap.data.json` & `symgt-0.0.6/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/textwrap.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/threading.data.json` & `symgt-0.0.6/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/threading.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/time.data.json` & `symgt-0.0.6/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/time.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/types.data.json` & `symgt-0.0.6/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/types.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/typing.data.json` & `symgt-0.0.6/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/typing.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/typing_extensions.data.json` & `symgt-0.0.6/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/typing_extensions.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/warnings.data.json` & `symgt-0.0.6/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/warnings.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/zipfile.data.json` & `symgt-0.0.6/.mypy_cache/3.11/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/zipfile.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_typeshed/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/collections/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/collections/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/collections/abc.data.json` & `symgt-0.0.6/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/collections/abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/ctypes/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/ctypes/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/charset.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/charset.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/contentmanager.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/contentmanager.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/errors.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/errors.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/header.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/header.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/message.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/message.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/policy.data.json` & `symgt-0.0.6/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/email/policy.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/abc.data.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/machinery.data.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/machinery.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/json/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/json/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/json/decoder.data.json` & `symgt-0.0.6/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/json/decoder.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/json/encoder.data.json` & `symgt-0.0.6/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/json/encoder.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/logging/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/logging/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_pytesttester.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_pytesttester.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_version.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_version.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ctypeslib.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ctypeslib.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/version.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/version.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_array_like.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_callable.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_callable.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nbit.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_scalars.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_shape.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_shape.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/compat/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/compat/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/compat/_inspect.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/compat/_inspect.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/compat/py3k.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/compat/py3k.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_asarray.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_asarray.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_internal.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_internal.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_type_aliases.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/arrayprint.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/arrayprint.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/defchararray.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/defchararray.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/einsumfunc.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/fromnumeric.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/function_base.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/function_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/multiarray.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/multiarray.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/numeric.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/numeric.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/numerictypes.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/numerictypes.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/overrides.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/overrides.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/records.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/records.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/shape_base.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/shape_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/umath.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/core/umath.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/fft/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/fft/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/fft/helper.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/fft/helper.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/_version.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/_version.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraypad.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraypad.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraysetops.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arrayterator.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/format.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/format.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/function_base.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/function_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/histograms.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/histograms.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/index_tricks.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/mixins.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/mixins.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/npyio.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/npyio.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/polynomial.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/polynomial.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/scimath.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/scimath.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/shape_base.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/shape_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/twodim_base.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/type_check.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/type_check.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/ufunclike.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/utils.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/lib/utils.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/linalg.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/linalg/linalg.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/core.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/core.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/extras.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/extras.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/mrecords.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/ma/mrecords.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/legendre.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_generator.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_generator.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_mt19937.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_mt19937.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_pcg64.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_pcg64.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_philox.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_philox.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_sfc64.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/_sfc64.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/bit_generator.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/bit_generator.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/mtrand.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/random/mtrand.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/testing/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/testing/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/utils.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/typing/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/numpy/typing/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/os/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/os/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/os/path.data.json` & `symgt-0.0.6/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/os/path.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/algorithms.data.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/algorithms.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/group_testing.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7385185185185185%*

 * *Differences: {"'data_mtime'": '1684471031',*

 * * "'dep_lines'": '{delete: [3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [5, 4, 3, 0]}',*

 * * "'dependencies'": "{insert: [(9, 'numpy._typing._dtype_like'), (10, "*

 * *                   "'numpy._typing._nested_sequence')], delete: [17, 16, 12, 11, 10, 0]}",*

 * * "'hash'": "'d910411f8c5c3ef54ae6be480f0b5fcb37a062eecae7b0ba5ee54b056a6a0d77'",*

 * * "'id'": "'symgt.group_testing'",*

 * * "'interface_hash'": "'bd659cc6e1e98ccefb27d92580ac9837431d431836c4b87f1f04300199b09ecd'",*

 * * "'mtime'": '1684471017',*

 * * "' […]*

```diff
@@ -1,14 +1,10 @@
 {
-    "data_mtime": 1684618176,
+    "data_mtime": 1684471031,
     "dep_lines": [
-        3,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
@@ -17,58 +13,50 @@
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "symgt.utils",
         "numpy",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "numpy._typing",
         "numpy._typing._array_like",
-        "numpy.core",
-        "numpy.core.fromnumeric",
-        "numpy.core.multiarray",
+        "numpy._typing._dtype_like",
+        "numpy._typing._nested_sequence",
         "pickle",
         "typing",
-        "typing_extensions",
-        "numpy._typing._dtype_like",
-        "numpy._typing._nested_sequence"
+        "typing_extensions"
     ],
-    "hash": "22f6112ee16e9536ec959fd71216ebc7e2f80e7ca46bebe64e84dae68838188f",
-    "id": "symgt.algorithms",
+    "hash": "d910411f8c5c3ef54ae6be480f0b5fcb37a062eecae7b0ba5ee54b056a6a0d77",
+    "id": "symgt.group_testing",
     "ignore_all": false,
-    "interface_hash": "62f4822e0150e34a0229e2b7f0ab5bbc92b04c2db7d3fd60c82e8fc4d0bdfbfd",
-    "mtime": 1684627927,
+    "interface_hash": "bd659cc6e1e98ccefb27d92580ac9837431d431836c4b87f1f04300199b09ecd",
+    "mtime": 1684471017,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -102,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/symgt/algorithms.py",
+    "path": "src/symgt/group_testing.py",
     "plugin_data": null,
-    "size": 4795,
+    "size": 1463,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/models.data.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/models.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/models.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/models.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/utils.data.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/utils.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994047619047619%*

 * *Differences: {"'names'": "{delete: ['grouptest_array']}"}*

```diff
@@ -303,79 +303,14 @@
                     "is_ready"
                 ],
                 "fullname": "symgt.utils.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
-        "grouptest_array": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0
-                ],
-                "arg_names": [
-                    "multfn"
-                ],
-                "dataclass_transform_spec": null,
-                "flags": [],
-                "fullname": "symgt.utils.grouptest_array",
-                "name": "grouptest_array",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0
-                    ],
-                    "arg_names": [
-                        "multfn"
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
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
-                    "name": "grouptest_array",
-                    "ret_type": {
-                        ".class": "Instance",
-                        "args": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 4
-                            },
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 4
-                            }
-                        ],
-                        "type_ref": "numpy.ndarray"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
         "intpart_from_multfn": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
```

### Comparing `symgt-0.0.5/.mypy_cache/3.11/symgt/utils.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/models.meta.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7174019607843137%*

 * *Differences: {"'data_mtime'": '1684436408',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 1), (16, 2)]}',*

 * * "'dep_prios'": '{insert: [(2, 30), (3, 30), (16, 5)]}',*

 * * "'dependencies'": "{insert: [(6, 'enum'), (12, 'numpy._typing._ufunc')]}",*

 * * "'hash'": "'7aedb860a2c6b13e832b72f1d9566f76f05521abd3cf41929e1dfa4e8417364a'",*

 * * "'id'": "'symgt.models'",*

 * * "'interface_hash'": "'0e80c76e9a8836fc6df896fd0c5a0a2e7bc40ea3c838d493650ea4810808e512'",*

 * * "'mtime'": '1684450247',*

 * * "'path'": "'src/symgt/models.py'",*

 * * "'size'": '6765',*

 * * "'suppressed […]*

```diff
@@ -1,24 +1,27 @@
 {
-    "data_mtime": 1684624087,
+    "data_mtime": 1684436408,
     "dep_lines": [
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        2
     ],
     "dep_prios": [
         10,
         5,
         30,
         30,
         30,
@@ -26,37 +29,42 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        30,
+        30,
+        30,
+        5
     ],
     "dependencies": [
         "numpy",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
+        "enum",
         "mmap",
         "numpy._typing",
         "numpy._typing._array_like",
         "numpy._typing._dtype_like",
         "numpy._typing._nested_sequence",
+        "numpy._typing._ufunc",
         "pickle",
         "typing",
         "typing_extensions"
     ],
-    "hash": "cafd0fa0aaa9dd655b995fddd524a6040b44bdb20f18f060585f59341a6e633f",
-    "id": "symgt.utils",
+    "hash": "7aedb860a2c6b13e832b72f1d9566f76f05521abd3cf41929e1dfa4e8417364a",
+    "id": "symgt.models",
     "ignore_all": false,
-    "interface_hash": "ebd4929141ad9af594742fe684f136f7316c93e99c388bc473cfababcb623cba",
-    "mtime": 1684628246,
+    "interface_hash": "0e80c76e9a8836fc6df896fd0c5a0a2e7bc40ea3c838d493650ea4810808e512",
+    "mtime": 1684450247,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -90,13 +98,15 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/symgt/utils.py",
+    "path": "src/symgt/models.py",
     "plugin_data": null,
-    "size": 3298,
-    "suppressed": [],
+    "size": 6765,
+    "suppressed": [
+        "scipy.special"
+    ],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/_log.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/_log.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/async_case.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/async_case.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/case.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/case.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/loader.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/loader.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/main.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/main.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/result.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/result.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/runner.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/runner.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/signals.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/signals.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/suite.data.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.11/unittest/suite.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/__future__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/__future__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/__future__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_ast.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_ast.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_codecs.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_codecs.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_collections_abc.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_collections_abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_ctypes.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_ctypes.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_thread.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_thread.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_thread.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_warnings.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_warnings.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/abc.data.json` & `symgt-0.0.6/.mypy_cache/3.9/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/array.data.json` & `symgt-0.0.6/.mypy_cache/3.9/array.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/array.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/array.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/ast.data.json` & `symgt-0.0.6/.mypy_cache/3.9/ast.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/ast.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/ast.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/builtins.data.json` & `symgt-0.0.6/.mypy_cache/3.9/builtins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/builtins.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/codecs.data.json` & `symgt-0.0.6/.mypy_cache/3.9/codecs.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/codecs.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/contextlib.data.json` & `symgt-0.0.6/.mypy_cache/3.9/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/contextlib.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/dataclasses.data.json` & `symgt-0.0.6/.mypy_cache/3.9/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/dataclasses.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/datetime.data.json` & `symgt-0.0.6/.mypy_cache/3.9/datetime.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/datetime.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/enum.data.json` & `symgt-0.0.6/.mypy_cache/3.9/enum.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/enum.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/enum.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/functools.data.json` & `symgt-0.0.6/.mypy_cache/3.9/functools.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/functools.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/functools.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/genericpath.data.json` & `symgt-0.0.6/.mypy_cache/3.9/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/genericpath.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/io.data.json` & `symgt-0.0.6/.mypy_cache/3.9/io.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/io.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/io.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/math.data.json` & `symgt-0.0.6/.mypy_cache/3.9/math.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/math.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/math.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/mmap.data.json` & `symgt-0.0.6/.mypy_cache/3.9/mmap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/mmap.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/pathlib.data.json` & `symgt-0.0.6/.mypy_cache/3.9/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/pathlib.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/pickle.data.json` & `symgt-0.0.6/.mypy_cache/3.9/pickle.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/pickle.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/posixpath.data.json` & `symgt-0.0.6/.mypy_cache/3.9/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/posixpath.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/re.data.json` & `symgt-0.0.6/.mypy_cache/3.9/re.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/re.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/re.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sre_compile.data.json` & `symgt-0.0.6/.mypy_cache/3.9/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sre_compile.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sre_constants.data.json` & `symgt-0.0.6/.mypy_cache/3.9/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sre_constants.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sre_parse.data.json` & `symgt-0.0.6/.mypy_cache/3.9/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sre_parse.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/string.data.json` & `symgt-0.0.6/.mypy_cache/3.9/string.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/string.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/string.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/subprocess.data.json` & `symgt-0.0.6/.mypy_cache/3.9/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/subprocess.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sys.data.json` & `symgt-0.0.6/.mypy_cache/3.9/sys.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/sys.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/sys.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/textwrap.data.json` & `symgt-0.0.6/.mypy_cache/3.9/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/textwrap.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/threading.data.json` & `symgt-0.0.6/.mypy_cache/3.9/threading.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/threading.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/threading.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/time.data.json` & `symgt-0.0.6/.mypy_cache/3.9/time.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/time.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/time.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/types.data.json` & `symgt-0.0.6/.mypy_cache/3.9/types.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/types.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/types.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/typing.data.json` & `symgt-0.0.6/.mypy_cache/3.9/typing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/typing.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/typing.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/typing_extensions.data.json` & `symgt-0.0.6/.mypy_cache/3.9/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/typing_extensions.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/warnings.data.json` & `symgt-0.0.6/.mypy_cache/3.9/warnings.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/warnings.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/zipfile.data.json` & `symgt-0.0.6/.mypy_cache/3.9/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/zipfile.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_typeshed/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/_typeshed/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/collections/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/collections/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/collections/abc.data.json` & `symgt-0.0.6/.mypy_cache/3.9/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/collections/abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/ctypes/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/ctypes/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/charset.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/charset.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/contentmanager.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/contentmanager.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/errors.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/errors.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/header.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/header.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/header.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/message.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/message.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/message.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/policy.data.json` & `symgt-0.0.6/.mypy_cache/3.9/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/email/policy.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/abc.data.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/abc.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/machinery.data.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/machinery.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/metadata/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/importlib/metadata/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/json/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/json/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/json/decoder.data.json` & `symgt-0.0.6/.mypy_cache/3.9/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/json/decoder.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/json/encoder.data.json` & `symgt-0.0.6/.mypy_cache/3.9/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/json/encoder.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/logging/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/logging/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_pytesttester.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_pytesttester.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_version.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_version.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ctypeslib.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ctypeslib.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/version.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/version.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_array_like.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_callable.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_callable.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nbit.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_scalars.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_shape.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_shape.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/compat/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/compat/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/compat/_inspect.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/compat/_inspect.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/compat/py3k.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/compat/py3k.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_asarray.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_asarray.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_internal.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_internal.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_type_aliases.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/arrayprint.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/arrayprint.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/defchararray.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/defchararray.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/einsumfunc.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/fromnumeric.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/function_base.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/function_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/multiarray.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/multiarray.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/numeric.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/numeric.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/numerictypes.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/numerictypes.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/overrides.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/overrides.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/records.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/records.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/shape_base.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/shape_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/umath.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/core/umath.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/fft/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/fft/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/fft/helper.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/fft/helper.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/_version.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/_version.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraypad.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraypad.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraysetops.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arrayterator.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/format.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/format.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/function_base.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/function_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/histograms.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/histograms.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/index_tricks.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/mixins.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/mixins.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/npyio.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/npyio.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/polynomial.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/polynomial.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/scimath.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/scimath.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/shape_base.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/shape_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/twodim_base.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/type_check.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/type_check.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/ufunclike.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/utils.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/lib/utils.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/linalg.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/linalg/linalg.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/core.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/core.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/extras.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/extras.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/mrecords.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/ma/mrecords.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/legendre.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_generator.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_generator.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_mt19937.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_mt19937.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_pcg64.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_pcg64.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_philox.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_philox.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_sfc64.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/_sfc64.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/bit_generator.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/bit_generator.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/mtrand.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/random/mtrand.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/testing/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/testing/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/utils.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/typing/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/numpy/typing/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/os/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/os/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/os/path.data.json` & `symgt-0.0.6/.mypy_cache/3.9/os/path.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/os/path.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/algorithms.data.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/algorithms.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/algorithms.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/group_testing.data.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/group_testing.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/group_testing.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/utils.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7666666666666667%*

 * *Differences: {"'data_mtime'": '1684775898',*

 * * "'hash'": "'692cf8d0c59f9a18127d33d8aa8c36dd8e0649e9d858f91920055e8cc50e01cb'",*

 * * "'id'": "'symgt.utils'",*

 * * "'interface_hash'": "'bc04b5f46b88520c0dfd428ff06d3aa53f63a5b172ec78a4eed998a480afe143'",*

 * * "'mtime'": '1684779583',*

 * * "'path'": "'src/symgt/utils.py'",*

 * * "'size'": '5400'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1684471031,
+    "data_mtime": 1684775898,
     "dep_lines": [
         1,
         1,
         1,
         1,
         1,
         1,
@@ -44,19 +44,19 @@
         "numpy._typing._array_like",
         "numpy._typing._dtype_like",
         "numpy._typing._nested_sequence",
         "pickle",
         "typing",
         "typing_extensions"
     ],
-    "hash": "d910411f8c5c3ef54ae6be480f0b5fcb37a062eecae7b0ba5ee54b056a6a0d77",
-    "id": "symgt.group_testing",
+    "hash": "692cf8d0c59f9a18127d33d8aa8c36dd8e0649e9d858f91920055e8cc50e01cb",
+    "id": "symgt.utils",
     "ignore_all": false,
-    "interface_hash": "bd659cc6e1e98ccefb27d92580ac9837431d431836c4b87f1f04300199b09ecd",
-    "mtime": 1684471017,
+    "interface_hash": "bc04b5f46b88520c0dfd428ff06d3aa53f63a5b172ec78a4eed998a480afe143",
+    "mtime": 1684779583,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -90,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/symgt/group_testing.py",
+    "path": "src/symgt/utils.py",
     "plugin_data": null,
-    "size": 1463,
+    "size": 5400,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/models.data.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/models.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/models.meta.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/algorithms.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7076555023923444%*

 * *Differences: {"'data_mtime'": '1684618176',*

 * * "'dep_lines'": '{insert: [(0, 3), (17, 1)], delete: [16]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (17, 30)], delete: [16]}',*

 * * "'dependencies'": "{insert: [(0, 'symgt.utils'), (10, 'numpy.core'), (11, "*

 * *                   "'numpy.core.fromnumeric'), (12, 'numpy.core.multiarray'), (16, "*

 * *                   "'numpy._typing._dtype_like'), (17, 'numpy._typing._nested_sequence')], delete: "*

 * *                   '[12, 11, 10, 6]}',*

 * * "'hash'": "'22f6112ee16e9536ec959fd71216ebc7e2f80e7ca46 […]*

```diff
@@ -1,10 +1,11 @@
 {
-    "data_mtime": 1684436408,
+    "data_mtime": 1684618176,
     "dep_lines": [
+        3,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
@@ -13,17 +14,18 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        2
+        1
     ],
     "dep_prios": [
+        5,
         10,
         5,
         30,
         30,
         30,
         30,
         30,
@@ -32,39 +34,41 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        5
+        30
     ],
     "dependencies": [
+        "symgt.utils",
         "numpy",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "enum",
         "mmap",
         "numpy._typing",
         "numpy._typing._array_like",
-        "numpy._typing._dtype_like",
-        "numpy._typing._nested_sequence",
-        "numpy._typing._ufunc",
+        "numpy.core",
+        "numpy.core.fromnumeric",
+        "numpy.core.multiarray",
         "pickle",
         "typing",
-        "typing_extensions"
+        "typing_extensions",
+        "numpy._typing._dtype_like",
+        "numpy._typing._nested_sequence"
     ],
-    "hash": "7aedb860a2c6b13e832b72f1d9566f76f05521abd3cf41929e1dfa4e8417364a",
-    "id": "symgt.models",
+    "hash": "22f6112ee16e9536ec959fd71216ebc7e2f80e7ca46bebe64e84dae68838188f",
+    "id": "symgt.algorithms",
     "ignore_all": false,
-    "interface_hash": "0e80c76e9a8836fc6df896fd0c5a0a2e7bc40ea3c838d493650ea4810808e512",
-    "mtime": 1684450247,
+    "interface_hash": "62f4822e0150e34a0229e2b7f0ab5bbc92b04c2db7d3fd60c82e8fc4d0bdfbfd",
+    "mtime": 1684627927,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -98,15 +102,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/symgt/models.py",
+    "path": "src/symgt/algorithms.py",
     "plugin_data": null,
-    "size": 6765,
-    "suppressed": [
-        "scipy.special"
-    ],
+    "size": 4795,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/utils.data.json` & `symgt-0.0.6/.mypy_cache/3.11/symgt/utils.data.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'names'": "{'empirical_tests_used': OrderedDict([('.class', 'SymbolTableNode'), ('kind', "*

 * *            "'Gdef'), ('node', OrderedDict([('.class', 'FuncDef'), ('abstract_status', 0), "*

 * *            "('arg_kinds', [0, 0]), ('arg_names', ['A', 'X']), ('dataclass_transform_spec', None), "*

 * *            "('flags', []), ('fullname', 'symgt.utils.empirical_tests_used'), ('name', "*

 * *            "'empirical_tests_used'), ('type', OrderedDict([('.class', 'CallableType'), "*

 * *            "('arg_kinds', [0, 0]), ('arg_name […]*

```diff
@@ -303,14 +303,173 @@
                     "is_ready"
                 ],
                 "fullname": "symgt.utils.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
+        "empirical_tests_used": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    0
+                ],
+                "arg_names": [
+                    "A",
+                    "X"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "symgt.utils.empirical_tests_used",
+                "name": "empirical_tests_used",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        0
+                    ],
+                    "arg_names": [
+                        "A",
+                        "X"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "Instance",
+                            "args": [
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 4
+                                },
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 4
+                                }
+                            ],
+                            "type_ref": "numpy.ndarray"
+                        },
+                        {
+                            ".class": "Instance",
+                            "args": [
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 4
+                                },
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 4
+                                }
+                            ],
+                            "type_ref": "numpy.ndarray"
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
+                    "name": "empirical_tests_used",
+                    "ret_type": "builtins.int",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "grouptest_array": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0
+                ],
+                "arg_names": [
+                    "multfn"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "symgt.utils.grouptest_array",
+                "name": "grouptest_array",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        "multfn"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "Instance",
+                            "args": [
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 4
+                                },
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 4
+                                }
+                            ],
+                            "type_ref": "numpy.ndarray"
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
+                    "name": "grouptest_array",
+                    "ret_type": {
+                        ".class": "Instance",
+                        "args": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 4
+                            },
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 4
+                            }
+                        ],
+                        "type_ref": "numpy.ndarray"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
         "intpart_from_multfn": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
```

### Comparing `symgt-0.0.5/.mypy_cache/3.9/symgt/utils.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/symgt/utils.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/__init__.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/__init__.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/_log.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/_log.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/async_case.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/async_case.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/case.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/case.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/loader.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/loader.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/main.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/main.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/result.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/result.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/runner.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/runner.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/signals.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/signals.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/suite.data.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.mypy_cache/3.9/unittest/suite.meta.json` & `symgt-0.0.6/.mypy_cache/3.9/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/139172a1d04f111c` & `symgt-0.0.6/.ruff_cache/content/139172a1d04f111c`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/14c651b336758ebb` & `symgt-0.0.6/.ruff_cache/content/14c651b336758ebb`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/16267a8fd146f85e` & `symgt-0.0.6/.ruff_cache/content/16267a8fd146f85e`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/29605448695c5466` & `symgt-0.0.6/.ruff_cache/content/29605448695c5466`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/2ab08c94c18dffd8` & `symgt-0.0.6/.ruff_cache/content/2ab08c94c18dffd8`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/2f69b8ae8d6a1af6` & `symgt-0.0.6/.ruff_cache/content/2f69b8ae8d6a1af6`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/2fb9857b45c0fd8` & `symgt-0.0.6/.ruff_cache/content/2fb9857b45c0fd8`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/4924663384114806` & `symgt-0.0.6/.ruff_cache/content/4924663384114806`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/4da8e3407a357d79` & `symgt-0.0.6/.ruff_cache/content/4da8e3407a357d79`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/54edc30e4f152a52` & `symgt-0.0.6/.ruff_cache/content/54edc30e4f152a52`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/5b3817478e0fea4b` & `symgt-0.0.6/.ruff_cache/content/5b3817478e0fea4b`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/5dc13b6c60c12647` & `symgt-0.0.6/.ruff_cache/content/5dc13b6c60c12647`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/5e78700d4867768f` & `symgt-0.0.6/.ruff_cache/content/5e78700d4867768f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/61167eff0eefb0fe` & `symgt-0.0.6/.ruff_cache/content/61167eff0eefb0fe`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/6984a2e796257436` & `symgt-0.0.6/.ruff_cache/content/6984a2e796257436`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/7e85677f179a32fa` & `symgt-0.0.6/.ruff_cache/content/7e85677f179a32fa`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/823ef04562dcffe6` & `symgt-0.0.6/.ruff_cache/content/823ef04562dcffe6`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/83cc80f689aeb0e9` & `symgt-0.0.6/.ruff_cache/content/83cc80f689aeb0e9`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/94b91fcec9ba2ff5` & `symgt-0.0.6/.ruff_cache/content/94b91fcec9ba2ff5`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/99f1d2d12ed2e065` & `symgt-0.0.6/.ruff_cache/content/99f1d2d12ed2e065`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/a6b46d2dc660c905` & `symgt-0.0.6/.ruff_cache/content/a6b46d2dc660c905`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/d01d1cb9c55b5449` & `symgt-0.0.6/.ruff_cache/content/d01d1cb9c55b5449`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/d0c02fd910364fe2` & `symgt-0.0.6/.ruff_cache/content/d0c02fd910364fe2`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/d9f344e7ff2bb0b7` & `symgt-0.0.6/.ruff_cache/content/d9f344e7ff2bb0b7`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/e20e976ab9a11b0f` & `symgt-0.0.6/.ruff_cache/content/e20e976ab9a11b0f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/e504bf6f224509f7` & `symgt-0.0.6/.ruff_cache/content/e504bf6f224509f7`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/eaa603b09b9e063` & `symgt-0.0.6/.ruff_cache/content/eaa603b09b9e063`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/ec24ffbb3ec32139` & `symgt-0.0.6/.ruff_cache/content/ec24ffbb3ec32139`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/ed7cf892f44fb99f` & `symgt-0.0.6/.ruff_cache/content/ed7cf892f44fb99f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/f1f975d7f1eda925` & `symgt-0.0.6/.ruff_cache/content/f1f975d7f1eda925`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/f2a2ffa9535b96cd` & `symgt-0.0.6/.ruff_cache/content/f2a2ffa9535b96cd`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/f335c26511af9131` & `symgt-0.0.6/.ruff_cache/content/f335c26511af9131`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/f86a276395fd7136` & `symgt-0.0.6/.ruff_cache/content/f86a276395fd7136`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/.ruff_cache/content/f8f07e0dd2e7876f` & `symgt-0.0.6/.ruff_cache/content/f8f07e0dd2e7876f`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/data/X.npy` & `symgt-0.0.6/data/X.npy`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/data/X_shuffled.npy` & `symgt-0.0.6/data/X_shuffled.npy`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/src/.DS_Store` & `symgt-0.0.6/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/src/symgt/algorithms.py` & `symgt-0.0.6/src/symgt/algorithms.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/src/symgt/models.py` & `symgt-0.0.6/src/symgt/models.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/tests/01_smoke_test:_IIDModel.py` & `symgt-0.0.6/tests/01_smoke_test:_IIDModel.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/tests/02_smoke_test:_ExchangeableModel.py` & `symgt-0.0.6/tests/02_smoke_test:_ExchangeableModel.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/tests/03_smoke_test:_algorithms.py` & `symgt-0.0.6/tests/03_smoke_test:_algorithms.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/tests/04_smoke_test:_utils.py` & `symgt-0.0.6/.ruff_cache/content/433bf4565329474d`

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,200 @@
-00000000: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-00000010: 6e70 0a0a 6672 6f6d 2073 796d 6774 2e6d  np..from symgt.m
-00000020: 6f64 656c 7320 696d 706f 7274 2049 4944  odels import IID
-00000030: 4d6f 6465 6c0a 6672 6f6d 2073 796d 6774  Model.from symgt
-00000040: 2e75 7469 6c73 2069 6d70 6f72 7420 696e  .utils import in
-00000050: 7470 6172 745f 6672 6f6d 5f6d 756c 7466  tpart_from_multf
-00000060: 6e2c 2055 5f66 726f 6d5f 712c 2045 436f  n, U_from_q, ECo
-00000070: 7374 2c20 4554 6573 7473 2c20 6772 6f75  st, ETests, grou
-00000080: 7074 6573 745f 6172 7261 790a 0a70 7269  ptest_array..pri
-00000090: 6e74 2822 5448 4953 2049 5320 534d 4f4b  nt("THIS IS SMOK
-000000a0: 4520 5445 5354 2034 3a20 4954 2054 4553  E TEST 4: IT TES
-000000b0: 5453 2075 7469 6c73 2e70 7922 290a 0a23  TS utils.py")..#
-000000c0: 2054 6573 7420 696e 7470 6172 745f 6672   Test intpart_fr
-000000d0: 6f6d 5f6d 756c 7466 6e0a 6173 7365 7274  om_multfn.assert
-000000e0: 206e 702e 616c 6c63 6c6f 7365 2869 6e74   np.allclose(int
-000000f0: 7061 7274 5f66 726f 6d5f 6d75 6c74 666e  part_from_multfn
-00000100: 285b 302c 2030 2c20 315d 292c 205b 325d  ([0, 0, 1]), [2]
-00000110: 290a 6173 7365 7274 206e 702e 616c 6c63  ).assert np.allc
-00000120: 6c6f 7365 2869 6e74 7061 7274 5f66 726f  lose(intpart_fro
-00000130: 6d5f 6d75 6c74 666e 285b 302c 2030 2c20  m_multfn([0, 0, 
-00000140: 325d 292c 205b 322c 2032 5d29 0a61 7373  2]), [2, 2]).ass
-00000150: 6572 7420 6e70 2e61 6c6c 636c 6f73 6528  ert np.allclose(
-00000160: 696e 7470 6172 745f 6672 6f6d 5f6d 756c  intpart_from_mul
-00000170: 7466 6e28 5b30 2c20 302c 2032 2c20 312c  tfn([0, 0, 2, 1,
-00000180: 2031 5d29 2c20 5b34 2c20 332c 2032 2c20   1]), [4, 3, 2, 
-00000190: 325d 290a 6173 7365 7274 206e 702e 616c  2]).assert np.al
-000001a0: 6c63 6c6f 7365 2869 6e74 7061 7274 5f66  lclose(intpart_f
-000001b0: 726f 6d5f 6d75 6c74 666e 285b 302c 2030  rom_multfn([0, 0
-000001c0: 2c20 305d 292c 205b 5d29 0a0a 2320 5465  , 0]), [])..# Te
-000001d0: 7374 2055 5f66 726f 6d5f 710a 2320 7468  st U_from_q.# th
-000001e0: 6520 6265 6c6f 7720 6172 6520 7720 7265  e below are w re
-000001f0: 7072 6573 656e 7461 7469 6f6e 733a 2077  presentations: w
-00000200: 5b69 5d20 3d20 7028 7829 2077 6865 7265  [i] = p(x) where
-00000210: 206e 6e7a 2878 2920 3d20 693b 2073 6565   nnz(x) = i; see
-00000220: 2070 6170 6572 0a23 2077 5f72 203d 206e   paper.# w_r = n
-00000230: 702e 6172 7261 7928 5b30 2c20 302e 352c  p.array([0, 0.5,
-00000240: 2030 5d29 0a23 2077 5f73 203d 206e 702e   0]).# w_s = np.
-00000250: 6172 7261 7928 5b30 2c20 302c 2031 2e30  array([0, 0, 1.0
-00000260: 5d29 0a23 2074 6865 7365 2067 6976 650a  ]).# these give.
-00000270: 715f 7220 3d20 6e70 2e61 7272 6179 285b  q_r = np.array([
-00000280: 312e 302c 2030 2e35 2c20 302e 305d 290a  1.0, 0.5, 0.0]).
-00000290: 715f 7320 3d20 6e70 2e61 7272 6179 285b  q_s = np.array([
-000002a0: 312e 302c 2030 2e30 2c20 302e 305d 290a  1.0, 0.0, 0.0]).
-000002b0: 0a55 5f72 203d 2055 5f66 726f 6d5f 7128  .U_r = U_from_q(
-000002c0: 715f 7229 0a55 5f73 203d 2055 5f66 726f  q_r).U_s = U_fro
-000002d0: 6d5f 7128 715f 7329 0a0a 7761 6e74 203d  m_q(q_s)..want =
-000002e0: 206e 702e 6172 7261 7928 5b31 2c20 312c   np.array([1, 1,
-000002f0: 2033 5d29 0a0a 6173 7365 7274 206e 702e   3])..assert np.
-00000300: 616c 6c28 555f 7220 3d3d 2077 616e 7429  all(U_r == want)
-00000310: 2c20 6622 555f 7220 6973 206e 6f74 207b  , f"U_r is not {
-00000320: 7761 6e74 7d22 0a61 7373 6572 7420 6e70  want}".assert np
-00000330: 2e61 6c6c 2855 5f73 203d 3d20 7761 6e74  .all(U_s == want
-00000340: 292c 2066 2255 5f72 2069 7320 6e6f 7420  ), f"U_r is not 
-00000350: 7b77 616e 747d 220a 6173 7365 7274 206e  {want}".assert n
-00000360: 702e 616c 6c28 555f 7220 3d3d 2055 5f73  p.all(U_r == U_s
-00000370: 292c 2022 555f 7220 6973 206e 6f74 2055  ), "U_r is not U
-00000380: 5f73 220a 2320 7468 6579 2073 686f 756c  _s".# they shoul
-00000390: 6420 6d61 7463 6820 2870 726f 6f66 2074  d match (proof t
-000003a0: 6861 7420 5520 6973 206e 6f74 2061 2072  hat U is not a r
-000003b0: 6570 7265 7365 6e74 6174 696f 6e29 0a0a  epresentation)..
-000003c0: 2320 5465 7374 2045 5465 7374 7320 2861  # Test ETests (a
-000003d0: 6e64 2069 6d70 6c69 6369 746c 792c 2049  nd implicitly, I
-000003e0: 4944 4d6f 6465 6c2c 2055 5f66 726f 6d5f  IDModel, U_from_
-000003f0: 7129 0a71 203d 206e 702e 6172 7261 7928  q).q = np.array(
-00000400: 5b31 2c20 312c 2031 5d29 0a61 7373 6572  [1, 1, 1]).asser
-00000410: 7420 4554 6573 7473 2871 2c20 3129 203d  t ETests(q, 1) =
-00000420: 3d20 310a 6173 7365 7274 2045 5465 7374  = 1.assert ETest
-00000430: 7328 712c 2032 2920 3d3d 2031 0a71 203d  s(q, 2) == 1.q =
-00000440: 206e 702e 6172 7261 7928 5b30 2c20 302c   np.array([0, 0,
-00000450: 2030 5d29 0a61 7373 6572 7420 4554 6573   0]).assert ETes
-00000460: 7473 285b 302c 2030 2c20 305d 2c20 3129  ts([0, 0, 0], 1)
-00000470: 203d 3d20 310a 6173 7365 7274 2045 5465   == 1.assert ETe
-00000480: 7374 7328 5b30 2c20 302c 2030 5d2c 2032  sts([0, 0, 0], 2
-00000490: 2920 3d3d 2033 0a0a 2320 5465 7374 2045  ) == 3..# Test E
-000004a0: 436f 7374 2028 616e 6420 696d 706c 6963  Cost (and implic
-000004b0: 6974 6c79 2c20 4949 444d 6f64 656c 2c20  itly, IIDModel, 
-000004c0: 555f 6672 6f6d 5f71 290a 7120 3d20 6e70  U_from_q).q = np
-000004d0: 2e65 7870 2849 4944 4d6f 6465 6c28 3130  .exp(IIDModel(10
-000004e0: 2c20 302e 3129 2e6c 6f67 5f71 2829 290a  , 0.1).log_q()).
-000004f0: 5520 3d20 555f 6672 6f6d 5f71 2871 290a  U = U_from_q(q).
-00000500: 6173 7365 7274 206e 702e 616c 6c63 6c6f  assert np.allclo
-00000510: 7365 2845 436f 7374 2871 2c20 5b30 2c20  se(ECost(q, [0, 
-00000520: 302c 2030 2c20 302c 2030 2c20 325d 292c  0, 0, 0, 0, 2]),
-00000530: 2032 202a 2055 5b35 5d29 0a61 7373 6572   2 * U[5]).asser
-00000540: 7420 6e70 2e61 6c6c 636c 6f73 6528 4543  t np.allclose(EC
-00000550: 6f73 7428 712c 205b 302c 2030 2c20 302c  ost(q, [0, 0, 0,
-00000560: 2030 2c20 302c 2032 5d29 2c20 362e 3039   0, 0, 2]), 6.09
-00000570: 3531 290a 6173 7365 7274 206e 702e 616c  51).assert np.al
-00000580: 6c63 6c6f 7365 2845 436f 7374 2871 2c20  lclose(ECost(q, 
-00000590: 5b30 2c20 302c 2030 2c20 302c 2030 2c20  [0, 0, 0, 0, 0, 
-000005a0: 302c 2030 2c20 302c 2030 2c20 302c 2031  0, 0, 0, 0, 0, 1
-000005b0: 5d29 2c20 555b 3130 5d29 0a61 7373 6572  ]), U[10]).asser
-000005c0: 7420 6e70 2e61 6c6c 636c 6f73 6528 4543  t np.allclose(EC
-000005d0: 6f73 7428 712c 205b 302c 2030 2c20 322c  ost(q, [0, 0, 2,
-000005e0: 2030 2c20 302c 2030 2c20 312c 2030 2c20   0, 0, 0, 1, 0, 
-000005f0: 302c 2030 2c20 305d 292c 2032 202a 2055  0, 0, 0]), 2 * U
-00000600: 5b32 5d20 2b20 3120 2a20 555b 365d 290a  [2] + 1 * U[6]).
-00000610: 6173 7365 7274 206e 702e 616c 6c63 6c6f  assert np.allclo
-00000620: 7365 2845 436f 7374 2871 2c20 5b30 2c20  se(ECost(q, [0, 
-00000630: 302c 2032 2c20 302c 2030 2c20 302c 2031  0, 2, 0, 0, 0, 1
-00000640: 2c20 302c 2030 2c20 302c 2030 5d29 2c20  , 0, 0, 0, 0]), 
-00000650: 362e 3537 3133 3534 290a 0a23 2031 2e33  6.571354)..# 1.3
-00000660: 3820 3d20 3120 2b20 3228 3120 2d20 2e39  8 = 1 + 2(1 - .9
-00000670: 5e32 290a 2320 312e 3831 3320 3d20 3120  ^2).# 1.813 = 1 
-00000680: 2b20 3328 3120 2d20 2e39 5e33 290a 2320  + 3(1 - .9^3).# 
-00000690: 322e 3337 3536 203d 2031 202b 2034 2831  2.3756 = 1 + 4(1
-000006a0: 202d 202e 395e 3429 0a23 2033 2e30 3437   - .9^4).# 3.047
-000006b0: 3535 203d 2031 202b 2035 2831 202d 202e  55 = 1 + 5(1 - .
-000006c0: 395e 3529 0a23 2033 2e38 3131 3335 3420  9^5).# 3.811354 
-000006d0: 3d20 3120 2b20 3628 3120 2d20 2e39 5e36  = 1 + 6(1 - .9^6
-000006e0: 290a 2320 342e 3635 3139 3231 3720 3d20  ).# 4.6519217 = 
-000006f0: 3120 2b20 3728 3120 2d20 2e39 5e37 290a  1 + 7(1 - .9^7).
-00000700: 2320 352e 3535 3632 3632 3332 203d 2031  # 5.55626232 = 1
-00000710: 202b 2038 2831 202d 202e 395e 3829 0a23   + 8(1 - .9^8).#
-00000720: 2036 2e35 3133 3231 3535 3939 203d 2031   6.513215599 = 1
-00000730: 202b 2039 2831 202d 202e 395e 3929 0a23   + 9(1 - .9^9).#
-00000740: 2037 2e35 3133 3231 3535 3939 203d 2031   7.513215599 = 1
-00000750: 202b 2031 3028 3120 2d20 2e39 5e31 3029   + 10(1 - .9^10)
-00000760: 0a61 7373 6572 7420 6e70 2e61 6c6c 636c  .assert np.allcl
-00000770: 6f73 6528 0a20 2020 2055 2c0a 2020 2020  ose(.    U,.    
-00000780: 6e70 2e61 7272 6179 280a 2020 2020 2020  np.array(.      
-00000790: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000007a0: 312c 0a20 2020 2020 2020 2020 2020 2031  1,.            1
-000007b0: 2c0a 2020 2020 2020 2020 2020 2020 312e  ,.            1.
-000007c0: 3338 2c0a 2020 2020 2020 2020 2020 2020  38,.            
-000007d0: 312e 3831 332c 0a20 2020 2020 2020 2020  1.813,.         
-000007e0: 2020 2032 2e33 3735 362c 0a20 2020 2020     2.3756,.     
-000007f0: 2020 2020 2020 2033 2e30 3437 3535 2c0a         3.04755,.
-00000800: 2020 2020 2020 2020 2020 2020 332e 3831              3.81
-00000810: 3133 3534 2c0a 2020 2020 2020 2020 2020  1354,.          
-00000820: 2020 342e 3635 3139 3231 372c 0a20 2020    4.6519217,.   
-00000830: 2020 2020 2020 2020 2035 2e35 3536 3236           5.55626
-00000840: 3233 322c 0a20 2020 2020 2020 2020 2020  232,.           
-00000850: 2036 2e35 3133 3231 3535 3939 2c0a 2020   6.513215599,.  
-00000860: 2020 2020 2020 2020 2020 372e 3531 3332            7.5132
-00000870: 3135 3539 392c 0a20 2020 2020 2020 205d  15599,.        ]
-00000880: 0a20 2020 2029 2c0a 290a 0a23 2054 6573  .    ),.)..# Tes
-00000890: 7420 6772 6f75 7074 6573 745f 6172 7261  t grouptest_arra
-000008a0: 790a 6d75 6c74 666e 203d 205b 302c 2031  y.multfn = [0, 1
-000008b0: 2c20 325d 0a61 7373 6572 7420 6e70 2e61  , 2].assert np.a
-000008c0: 6c6c 636c 6f73 6528 0a20 2020 2067 726f  llclose(.    gro
-000008d0: 7570 7465 7374 5f61 7272 6179 286d 756c  uptest_array(mul
-000008e0: 7466 6e29 2c0a 2020 2020 6e70 2e61 7272  tfn),.    np.arr
-000008f0: 6179 285b 5b31 2c20 312c 2030 2c20 302c  ay([[1, 1, 0, 0,
-00000900: 2030 5d2c 205b 302c 2030 2c20 312c 2031   0], [0, 0, 1, 1
-00000910: 2c20 305d 2c20 5b30 2c20 302c 2030 2c20  , 0], [0, 0, 0, 
-00000920: 302c 2031 5d5d 292c 0a29 0a6d 756c 7466  0, 1]]),.).multf
-00000930: 6e20 3d20 5b30 2c20 302c 2030 2c20 315d  n = [0, 0, 0, 1]
-00000940: 0a61 7373 6572 7420 6e70 2e61 6c6c 636c  .assert np.allcl
-00000950: 6f73 6528 0a20 2020 2067 726f 7570 7465  ose(.    groupte
-00000960: 7374 5f61 7272 6179 286d 756c 7466 6e29  st_array(multfn)
-00000970: 2c0a 2020 2020 6e70 2e61 7272 6179 285b  ,.    np.array([
-00000980: 5b31 2c20 312c 2031 5d5d 292c 0a29 0a6d  [1, 1, 1]]),.).m
-00000990: 756c 7466 6e20 3d20 5b30 2c20 302c 2030  ultfn = [0, 0, 0
-000009a0: 2c20 312c 2031 5d0a 6173 7365 7274 206e  , 1, 1].assert n
-000009b0: 702e 616c 6c63 6c6f 7365 280a 2020 2020  p.allclose(.    
-000009c0: 6772 6f75 7074 6573 745f 6172 7261 7928  grouptest_array(
-000009d0: 6d75 6c74 666e 292c 0a20 2020 206e 702e  multfn),.    np.
-000009e0: 6172 7261 7928 5b5b 312c 2031 2c20 312c  array([[1, 1, 1,
-000009f0: 2031 2c20 302c 2030 2c20 305d 2c20 5b30   1, 0, 0, 0], [0
-00000a00: 2c20 302c 2030 2c20 302c 2031 2c20 312c  , 0, 0, 0, 1, 1,
-00000a10: 2031 5d5d 292c 0a29 0a                    1]]),.).
+00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000010: 0d00 0000 0000 0000 556e 6465 6669 6e65  ........Undefine
+00000020: 644e 616d 6525 0000 0000 0000 0055 6e64  dName%.......Und
+00000030: 6566 696e 6564 206e 616d 6520 6065 6d70  efined name `emp
+00000040: 6972 6963 616c 5f74 6573 7473 5f75 7365  irical_tests_use
+00000050: 6460 0043 0b00 0057 0b00 0000 0000 0000  d`.C...W........
+00000060: 0000 0000 430b 0000 0100 0000 0000 0000  ....C...........
+00000070: 4c00 0000 0000 0000 2f55 7365 7273 2f6e  L......./Users/n
+00000080: 6963 686f 6c61 7363 6861 726c 6573 6c61  icholascharlesla
+00000090: 6e64 6f6c 6669 2f77 6f72 6b73 7061 6365  ndolfi/workspace
+000000a0: 2f73 796d 6774 2f74 6573 7473 2f30 345f  /symgt/tests/04_
+000000b0: 736d 6f6b 655f 7465 7374 3a5f 7574 696c  smoke_test:_util
+000000c0: 732e 7079 a50b 0000 0000 0000 696d 706f  s.py........impo
+000000d0: 7274 206e 756d 7079 2061 7320 6e70 0a0a  rt numpy as np..
+000000e0: 6672 6f6d 2073 796d 6774 2e6d 6f64 656c  from symgt.model
+000000f0: 7320 696d 706f 7274 2049 4944 4d6f 6465  s import IIDMode
+00000100: 6c0a 6672 6f6d 2073 796d 6774 2e75 7469  l.from symgt.uti
+00000110: 6c73 2069 6d70 6f72 7420 696e 7470 6172  ls import intpar
+00000120: 745f 6672 6f6d 5f6d 756c 7466 6e2c 2055  t_from_multfn, U
+00000130: 5f66 726f 6d5f 712c 2045 436f 7374 2c20  _from_q, ECost, 
+00000140: 4554 6573 7473 2c20 6772 6f75 7074 6573  ETests, grouptes
+00000150: 745f 6172 7261 790a 0a70 7269 6e74 2822  t_array..print("
+00000160: 5448 4953 2049 5320 534d 4f4b 4520 5445  THIS IS SMOKE TE
+00000170: 5354 2034 3a20 4954 2054 4553 5453 2075  ST 4: IT TESTS u
+00000180: 7469 6c73 2e70 7922 290a 0a23 2054 6573  tils.py")..# Tes
+00000190: 7420 696e 7470 6172 745f 6672 6f6d 5f6d  t intpart_from_m
+000001a0: 756c 7466 6e0a 6173 7365 7274 206e 702e  ultfn.assert np.
+000001b0: 616c 6c63 6c6f 7365 2869 6e74 7061 7274  allclose(intpart
+000001c0: 5f66 726f 6d5f 6d75 6c74 666e 285b 302c  _from_multfn([0,
+000001d0: 2030 2c20 315d 292c 205b 325d 290a 6173   0, 1]), [2]).as
+000001e0: 7365 7274 206e 702e 616c 6c63 6c6f 7365  sert np.allclose
+000001f0: 2869 6e74 7061 7274 5f66 726f 6d5f 6d75  (intpart_from_mu
+00000200: 6c74 666e 285b 302c 2030 2c20 325d 292c  ltfn([0, 0, 2]),
+00000210: 205b 322c 2032 5d29 0a61 7373 6572 7420   [2, 2]).assert 
+00000220: 6e70 2e61 6c6c 636c 6f73 6528 696e 7470  np.allclose(intp
+00000230: 6172 745f 6672 6f6d 5f6d 756c 7466 6e28  art_from_multfn(
+00000240: 5b30 2c20 302c 2032 2c20 312c 2031 5d29  [0, 0, 2, 1, 1])
+00000250: 2c20 5b34 2c20 332c 2032 2c20 325d 290a  , [4, 3, 2, 2]).
+00000260: 6173 7365 7274 206e 702e 616c 6c63 6c6f  assert np.allclo
+00000270: 7365 2869 6e74 7061 7274 5f66 726f 6d5f  se(intpart_from_
+00000280: 6d75 6c74 666e 285b 302c 2030 2c20 305d  multfn([0, 0, 0]
+00000290: 292c 205b 5d29 0a0a 2320 5465 7374 2055  ), [])..# Test U
+000002a0: 5f66 726f 6d5f 710a 2320 7468 6520 6265  _from_q.# the be
+000002b0: 6c6f 7720 6172 6520 7720 7265 7072 6573  low are w repres
+000002c0: 656e 7461 7469 6f6e 733a 2077 5b69 5d20  entations: w[i] 
+000002d0: 3d20 7028 7829 2077 6865 7265 206e 6e7a  = p(x) where nnz
+000002e0: 2878 2920 3d20 693b 2073 6565 2070 6170  (x) = i; see pap
+000002f0: 6572 0a23 2077 5f72 203d 206e 702e 6172  er.# w_r = np.ar
+00000300: 7261 7928 5b30 2c20 302e 352c 2030 5d29  ray([0, 0.5, 0])
+00000310: 0a23 2077 5f73 203d 206e 702e 6172 7261  .# w_s = np.arra
+00000320: 7928 5b30 2c20 302c 2031 2e30 5d29 0a23  y([0, 0, 1.0]).#
+00000330: 2074 6865 7365 2067 6976 650a 715f 7220   these give.q_r 
+00000340: 3d20 6e70 2e61 7272 6179 285b 312e 302c  = np.array([1.0,
+00000350: 2030 2e35 2c20 302e 305d 290a 715f 7320   0.5, 0.0]).q_s 
+00000360: 3d20 6e70 2e61 7272 6179 285b 312e 302c  = np.array([1.0,
+00000370: 2030 2e30 2c20 302e 305d 290a 0a55 5f72   0.0, 0.0])..U_r
+00000380: 203d 2055 5f66 726f 6d5f 7128 715f 7229   = U_from_q(q_r)
+00000390: 0a55 5f73 203d 2055 5f66 726f 6d5f 7128  .U_s = U_from_q(
+000003a0: 715f 7329 0a0a 7761 6e74 203d 206e 702e  q_s)..want = np.
+000003b0: 6172 7261 7928 5b31 2c20 312c 2033 5d29  array([1, 1, 3])
+000003c0: 0a0a 6173 7365 7274 206e 702e 616c 6c28  ..assert np.all(
+000003d0: 555f 7220 3d3d 2077 616e 7429 2c20 6622  U_r == want), f"
+000003e0: 555f 7220 6973 206e 6f74 207b 7761 6e74  U_r is not {want
+000003f0: 7d22 0a61 7373 6572 7420 6e70 2e61 6c6c  }".assert np.all
+00000400: 2855 5f73 203d 3d20 7761 6e74 292c 2066  (U_s == want), f
+00000410: 2255 5f72 2069 7320 6e6f 7420 7b77 616e  "U_r is not {wan
+00000420: 747d 220a 6173 7365 7274 206e 702e 616c  t}".assert np.al
+00000430: 6c28 555f 7220 3d3d 2055 5f73 292c 2022  l(U_r == U_s), "
+00000440: 555f 7220 6973 206e 6f74 2055 5f73 220a  U_r is not U_s".
+00000450: 2320 7468 6579 2073 686f 756c 6420 6d61  # they should ma
+00000460: 7463 6820 2870 726f 6f66 2074 6861 7420  tch (proof that 
+00000470: 5520 6973 206e 6f74 2061 2072 6570 7265  U is not a repre
+00000480: 7365 6e74 6174 696f 6e29 0a0a 2320 5465  sentation)..# Te
+00000490: 7374 2045 5465 7374 7320 2861 6e64 2069  st ETests (and i
+000004a0: 6d70 6c69 6369 746c 792c 2049 4944 4d6f  mplicitly, IIDMo
+000004b0: 6465 6c2c 2055 5f66 726f 6d5f 7129 0a71  del, U_from_q).q
+000004c0: 203d 206e 702e 6172 7261 7928 5b31 2c20   = np.array([1, 
+000004d0: 312c 2031 5d29 0a61 7373 6572 7420 4554  1, 1]).assert ET
+000004e0: 6573 7473 2871 2c20 3129 203d 3d20 310a  ests(q, 1) == 1.
+000004f0: 6173 7365 7274 2045 5465 7374 7328 712c  assert ETests(q,
+00000500: 2032 2920 3d3d 2031 0a71 203d 206e 702e   2) == 1.q = np.
+00000510: 6172 7261 7928 5b30 2c20 302c 2030 5d29  array([0, 0, 0])
+00000520: 0a61 7373 6572 7420 4554 6573 7473 285b  .assert ETests([
+00000530: 302c 2030 2c20 305d 2c20 3129 203d 3d20  0, 0, 0], 1) == 
+00000540: 310a 6173 7365 7274 2045 5465 7374 7328  1.assert ETests(
+00000550: 5b30 2c20 302c 2030 5d2c 2032 2920 3d3d  [0, 0, 0], 2) ==
+00000560: 2033 0a0a 2320 5465 7374 2045 436f 7374   3..# Test ECost
+00000570: 2028 616e 6420 696d 706c 6963 6974 6c79   (and implicitly
+00000580: 2c20 4949 444d 6f64 656c 2c20 555f 6672  , IIDModel, U_fr
+00000590: 6f6d 5f71 290a 7120 3d20 6e70 2e65 7870  om_q).q = np.exp
+000005a0: 2849 4944 4d6f 6465 6c28 3130 2c20 302e  (IIDModel(10, 0.
+000005b0: 3129 2e6c 6f67 5f71 2829 290a 5520 3d20  1).log_q()).U = 
+000005c0: 555f 6672 6f6d 5f71 2871 290a 6173 7365  U_from_q(q).asse
+000005d0: 7274 206e 702e 616c 6c63 6c6f 7365 2845  rt np.allclose(E
+000005e0: 436f 7374 2871 2c20 5b30 2c20 302c 2030  Cost(q, [0, 0, 0
+000005f0: 2c20 302c 2030 2c20 325d 292c 2032 202a  , 0, 0, 2]), 2 *
+00000600: 2055 5b35 5d29 0a61 7373 6572 7420 6e70   U[5]).assert np
+00000610: 2e61 6c6c 636c 6f73 6528 4543 6f73 7428  .allclose(ECost(
+00000620: 712c 205b 302c 2030 2c20 302c 2030 2c20  q, [0, 0, 0, 0, 
+00000630: 302c 2032 5d29 2c20 362e 3039 3531 290a  0, 2]), 6.0951).
+00000640: 6173 7365 7274 206e 702e 616c 6c63 6c6f  assert np.allclo
+00000650: 7365 2845 436f 7374 2871 2c20 5b30 2c20  se(ECost(q, [0, 
+00000660: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00000670: 2c20 302c 2030 2c20 302c 2031 5d29 2c20  , 0, 0, 0, 1]), 
+00000680: 555b 3130 5d29 0a61 7373 6572 7420 6e70  U[10]).assert np
+00000690: 2e61 6c6c 636c 6f73 6528 4543 6f73 7428  .allclose(ECost(
+000006a0: 712c 205b 302c 2030 2c20 322c 2030 2c20  q, [0, 0, 2, 0, 
+000006b0: 302c 2030 2c20 312c 2030 2c20 302c 2030  0, 0, 1, 0, 0, 0
+000006c0: 2c20 305d 292c 2032 202a 2055 5b32 5d20  , 0]), 2 * U[2] 
+000006d0: 2b20 3120 2a20 555b 365d 290a 6173 7365  + 1 * U[6]).asse
+000006e0: 7274 206e 702e 616c 6c63 6c6f 7365 2845  rt np.allclose(E
+000006f0: 436f 7374 2871 2c20 5b30 2c20 302c 2032  Cost(q, [0, 0, 2
+00000700: 2c20 302c 2030 2c20 302c 2031 2c20 302c  , 0, 0, 0, 1, 0,
+00000710: 2030 2c20 302c 2030 5d29 2c20 362e 3537   0, 0, 0]), 6.57
+00000720: 3133 3534 290a 0a23 2031 2e33 3820 3d20  1354)..# 1.38 = 
+00000730: 3120 2b20 3228 3120 2d20 2e39 5e32 290a  1 + 2(1 - .9^2).
+00000740: 2320 312e 3831 3320 3d20 3120 2b20 3328  # 1.813 = 1 + 3(
+00000750: 3120 2d20 2e39 5e33 290a 2320 322e 3337  1 - .9^3).# 2.37
+00000760: 3536 203d 2031 202b 2034 2831 202d 202e  56 = 1 + 4(1 - .
+00000770: 395e 3429 0a23 2033 2e30 3437 3535 203d  9^4).# 3.04755 =
+00000780: 2031 202b 2035 2831 202d 202e 395e 3529   1 + 5(1 - .9^5)
+00000790: 0a23 2033 2e38 3131 3335 3420 3d20 3120  .# 3.811354 = 1 
+000007a0: 2b20 3628 3120 2d20 2e39 5e36 290a 2320  + 6(1 - .9^6).# 
+000007b0: 342e 3635 3139 3231 3720 3d20 3120 2b20  4.6519217 = 1 + 
+000007c0: 3728 3120 2d20 2e39 5e37 290a 2320 352e  7(1 - .9^7).# 5.
+000007d0: 3535 3632 3632 3332 203d 2031 202b 2038  55626232 = 1 + 8
+000007e0: 2831 202d 202e 395e 3829 0a23 2036 2e35  (1 - .9^8).# 6.5
+000007f0: 3133 3231 3535 3939 203d 2031 202b 2039  13215599 = 1 + 9
+00000800: 2831 202d 202e 395e 3929 0a23 2037 2e35  (1 - .9^9).# 7.5
+00000810: 3133 3231 3535 3939 203d 2031 202b 2031  13215599 = 1 + 1
+00000820: 3028 3120 2d20 2e39 5e31 3029 0a61 7373  0(1 - .9^10).ass
+00000830: 6572 7420 6e70 2e61 6c6c 636c 6f73 6528  ert np.allclose(
+00000840: 0a20 2020 2055 2c0a 2020 2020 6e70 2e61  .    U,.    np.a
+00000850: 7272 6179 280a 2020 2020 2020 2020 5b0a  rray(.        [.
+00000860: 2020 2020 2020 2020 2020 2020 312c 0a20              1,. 
+00000870: 2020 2020 2020 2020 2020 2031 2c0a 2020             1,.  
+00000880: 2020 2020 2020 2020 2020 312e 3338 2c0a            1.38,.
+00000890: 2020 2020 2020 2020 2020 2020 312e 3831              1.81
+000008a0: 332c 0a20 2020 2020 2020 2020 2020 2032  3,.            2
+000008b0: 2e33 3735 362c 0a20 2020 2020 2020 2020  .3756,.         
+000008c0: 2020 2033 2e30 3437 3535 2c0a 2020 2020     3.04755,.    
+000008d0: 2020 2020 2020 2020 332e 3831 3133 3534          3.811354
+000008e0: 2c0a 2020 2020 2020 2020 2020 2020 342e  ,.            4.
+000008f0: 3635 3139 3231 372c 0a20 2020 2020 2020  6519217,.       
+00000900: 2020 2020 2035 2e35 3536 3236 3233 322c       5.55626232,
+00000910: 0a20 2020 2020 2020 2020 2020 2036 2e35  .            6.5
+00000920: 3133 3231 3535 3939 2c0a 2020 2020 2020  13215599,.      
+00000930: 2020 2020 2020 372e 3531 3332 3135 3539        7.51321559
+00000940: 392c 0a20 2020 2020 2020 205d 0a20 2020  9,.        ].   
+00000950: 2029 2c0a 290a 0a23 2054 6573 7420 6772   ),.)..# Test gr
+00000960: 6f75 7074 6573 745f 6172 7261 790a 6d75  ouptest_array.mu
+00000970: 6c74 666e 203d 205b 302c 2031 2c20 325d  ltfn = [0, 1, 2]
+00000980: 0a61 7373 6572 7420 6e70 2e61 6c6c 636c  .assert np.allcl
+00000990: 6f73 6528 0a20 2020 2067 726f 7570 7465  ose(.    groupte
+000009a0: 7374 5f61 7272 6179 286d 756c 7466 6e29  st_array(multfn)
+000009b0: 2c0a 2020 2020 6e70 2e61 7272 6179 285b  ,.    np.array([
+000009c0: 5b31 2c20 312c 2030 2c20 302c 2030 5d2c  [1, 1, 0, 0, 0],
+000009d0: 205b 302c 2030 2c20 312c 2031 2c20 305d   [0, 0, 1, 1, 0]
+000009e0: 2c20 5b30 2c20 302c 2030 2c20 302c 2031  , [0, 0, 0, 0, 1
+000009f0: 5d5d 292c 0a29 0a6d 756c 7466 6e20 3d20  ]]),.).multfn = 
+00000a00: 5b30 2c20 302c 2030 2c20 315d 0a61 7373  [0, 0, 0, 1].ass
+00000a10: 6572 7420 6e70 2e61 6c6c 636c 6f73 6528  ert np.allclose(
+00000a20: 0a20 2020 2067 726f 7570 7465 7374 5f61  .    grouptest_a
+00000a30: 7272 6179 286d 756c 7466 6e29 2c0a 2020  rray(multfn),.  
+00000a40: 2020 6e70 2e61 7272 6179 285b 5b31 2c20    np.array([[1, 
+00000a50: 312c 2031 5d5d 292c 0a29 0a6d 756c 7466  1, 1]]),.).multf
+00000a60: 6e20 3d20 5b30 2c20 302c 2030 2c20 312c  n = [0, 0, 0, 1,
+00000a70: 2031 5d0a 6173 7365 7274 206e 702e 616c   1].assert np.al
+00000a80: 6c63 6c6f 7365 280a 2020 2020 6772 6f75  lclose(.    grou
+00000a90: 7074 6573 745f 6172 7261 7928 6d75 6c74  ptest_array(mult
+00000aa0: 666e 292c 0a20 2020 206e 702e 6172 7261  fn),.    np.arra
+00000ab0: 7928 5b5b 312c 2031 2c20 312c 2031 2c20  y([[1, 1, 1, 1, 
+00000ac0: 302c 2030 2c20 305d 2c20 5b30 2c20 302c  0, 0, 0], [0, 0,
+00000ad0: 2030 2c20 302c 2031 2c20 312c 2031 5d5d   0, 0, 1, 1, 1]]
+00000ae0: 292c 0a29 0a0a 2320 5465 7374 2065 6d70  ),.)..# Test emp
+00000af0: 6972 6963 616c 5f74 6573 7473 5f75 7365  irical_tests_use
+00000b00: 640a 6d75 6c74 666e 203d 205b 302c 2030  d.multfn = [0, 0
+00000b10: 2c20 302c 2032 2c20 315d 2020 2320 6e20  , 0, 2, 1]  # n 
+00000b20: 3d20 3130 0a41 203d 2067 726f 7570 7465  = 10.A = groupte
+00000b30: 7374 5f61 7272 6179 286d 756c 7466 6e29  st_array(multfn)
+00000b40: 0a58 203d 206e 702e 6172 7261 7928 0a20  .X = np.array(. 
+00000b50: 2020 205b 0a20 2020 2020 2020 205b 302c     [.        [0,
+00000b60: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00000b70: 302c 2030 2c20 302c 2030 5d2c 0a20 2020  0, 0, 0, 0],.   
+00000b80: 2020 2020 205b 312c 2030 2c20 302c 2030       [1, 0, 0, 0
+00000b90: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00000ba0: 2030 5d2c 0a20 2020 2020 2020 205b 302c   0],.        [0,
+00000bb0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00000bc0: 302c 2030 2c20 302c 2031 5d2c 0a20 2020  0, 0, 0, 1],.   
+00000bd0: 205d 0a29 0a23 2073 686f 756c 6420 7573   ].).# should us
+00000be0: 6520 3320 2b20 2833 202b 2034 2920 2b20  e 3 + (3 + 4) + 
+00000bf0: 2833 202b 2033 2920 3d20 3136 2074 6573  (3 + 3) = 16 tes
+00000c00: 7473 0a67 6f74 2c20 7761 6e74 203d 2065  ts.got, want = e
+00000c10: 6d70 6972 6963 616c 5f74 6573 7473 5f75  mpirical_tests_u
+00000c20: 7365 6428 412c 2058 292c 2031 360a 6173  sed(A, X), 16.as
+00000c30: 7365 7274 2067 6f74 203d 3d20 7761 6e74  sert got == want
+00000c40: 2c20 6622 656d 7069 7269 6361 6c20 7465  , f"empirical te
+00000c50: 7374 7320 7573 6564 2067 6f74 207b 676f  sts used got {go
+00000c60: 747d 2c20 7761 6e74 207b 7761 6e74 7d22  t}, want {want}"
+00000c70: 0a                                       .
```

### Comparing `symgt-0.0.5/tests/05_smoke_test:_golden.py` & `symgt-0.0.6/tests/05_smoke_test:_golden.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/tests/06_smoke_test:_golden2.py` & `symgt-0.0.6/tests/06_smoke_test:_golden2.py`

 * *Files identical despite different names*

### Comparing `symgt-0.0.5/README.md` & `symgt-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,12 +7,22 @@
 ```
 
 For example, to compute an optimal partition for a symmetric distribution...
 ```python
 import numpy as np
 from symgt import models, algorithms, utils
 
-m = models.ExchangeableModel(10, np.array([0.5, 0.2, 0.0, 0.0, 0.0, 0.0, 0.2, 0.1, 0.0, 0.0, 0.0]))
-q = np.exp(m.log_q()) # the representation q
+# the representation alpha of symmetric distribution
+alpha = np.array([0.5, 0.2, 0.0, 0.0, 0.0, 0.0, 0.2, 0.1, 0.0, 0.0, 0.0])
+m = models.ExchangeableModel(10, alpha)
+q = np.exp(m.log_q()) # the representation q of the symmetric distribution
 multfn, cost = algorithms.symmetric_multfn(q) # cost is 6
 intpart = utils.intpart_from_multfn(multfn) # intpart is [10]
+
+# which differs from that computed using the IID approximation
+m_iid = models.IIDModel(10, m.prevalence())
+multfn_iid, _ = algorithms.symmetric_multfn(np.exp(m_iid.log_q()))
+intpart_iid = utils.intpart_from_multfn(multfn_iid) # is [4, 3, 3]
+
+utils.ECost(q, multfn) # 6
+utils.ECost(q, multfn_iid) # 6.63
 ```
```

### Comparing `symgt-0.0.5/pyproject.toml` & `symgt-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "symgt"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name = "N. C. Landolfi", email="crews.fixture.0f@icloud.com"},
 ]
 description = "A package for group testing against symmetric distributions."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `symgt-0.0.5/PKG-INFO` & `symgt-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symgt
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for group testing against symmetric distributions.
 Project-URL: Homepage, https://github.com/nlandolfi/symgt
 Author-email: "N. C. Landolfi" <crews.fixture.0f@icloud.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -20,12 +20,22 @@
 ```
 
 For example, to compute an optimal partition for a symmetric distribution...
 ```python
 import numpy as np
 from symgt import models, algorithms, utils
 
-m = models.ExchangeableModel(10, np.array([0.5, 0.2, 0.0, 0.0, 0.0, 0.0, 0.2, 0.1, 0.0, 0.0, 0.0]))
-q = np.exp(m.log_q()) # the representation q
+# the representation alpha of symmetric distribution
+alpha = np.array([0.5, 0.2, 0.0, 0.0, 0.0, 0.0, 0.2, 0.1, 0.0, 0.0, 0.0])
+m = models.ExchangeableModel(10, alpha)
+q = np.exp(m.log_q()) # the representation q of the symmetric distribution
 multfn, cost = algorithms.symmetric_multfn(q) # cost is 6
 intpart = utils.intpart_from_multfn(multfn) # intpart is [10]
+
+# which differs from that computed using the IID approximation
+m_iid = models.IIDModel(10, m.prevalence())
+multfn_iid, _ = algorithms.symmetric_multfn(np.exp(m_iid.log_q()))
+intpart_iid = utils.intpart_from_multfn(multfn_iid) # is [4, 3, 3]
+
+utils.ECost(q, multfn) # 6
+utils.ECost(q, multfn_iid) # 6.63
 ```
```

