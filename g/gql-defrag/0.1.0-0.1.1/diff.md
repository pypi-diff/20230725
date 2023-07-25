# Comparing `tmp/gql_defrag-0.1.0.tar.gz` & `tmp/gql_defrag-0.1.1.tar.gz`

## Comparing `gql_defrag-0.1.0.tar` & `gql_defrag-0.1.1.tar`

### file list

```diff
@@ -1,128 +1,16 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.flake8
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.prettierrc.yaml
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.github/workflows/pyanalyze.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180394 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52426 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18253 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   149860 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60702 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137646 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130438 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123343 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109230 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    57771 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0    90149 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22414 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85363 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    26823 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87490 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44419 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75223 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167571 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28506 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49767 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   162190 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   142478 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/test.data.json
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/test.meta.json
--rw-r--r--   0        0        0   239658 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432428 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57892 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89080 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   408014 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129009 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25099 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79296 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30883 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/__init__.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/__init__.meta.json
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/__main__.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/__main__.meta.json
--rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/defrag.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/defrag.meta.json
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/finder.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/gql_defrag/finder.meta.json
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70605 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64597 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91145 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   322647 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/gql_defrag/__init__.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/gql_defrag/__main__.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/gql_defrag/defrag.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/gql_defrag/finder.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/tests/test.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/.gitignore
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 gql_defrag-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.flake8
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.prettierrc.yaml
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.github/workflows/pyanalyze.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/gql_defrag/__init__.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/gql_defrag/__main__.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/gql_defrag/defrag.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/gql_defrag/finder.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/tests/test.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/.gitignore
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 gql_defrag-0.1.1/PKG-INFO
```

### Comparing `gql_defrag-0.1.0/.pre-commit-config.yaml` & `gql_defrag-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gql_defrag-0.1.0/gql_defrag/__main__.py` & `gql_defrag-0.1.1/gql_defrag/__main__.py`

 * *Files identical despite different names*

### Comparing `gql_defrag-0.1.0/gql_defrag/defrag.py` & `gql_defrag-0.1.1/gql_defrag/defrag.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 query.selection_set, source=query_name if add_source else None
             ),
             loc=query.loc,
         )
         new_doc = ast.Document(definitions=[new_query])
         return print_ast(new_doc)
 
-    def defragment_all(self, add_source: bool = True) -> Iterable[tuple[str, str]]:
+    def defragment_all(self, *, add_source: bool = True) -> Iterable[tuple[str, str]]:
         for query_name in self.query_to_defn:
             yield query_name, self.defragment(query_name, add_source=add_source)
 
     def _defragment_selection_set(
         self, selection_set: ast.SelectionSet, source: Optional[str]
     ) -> ast.SelectionSet:
         new_selections, final_list = self._parse_selection_set(
```

### Comparing `gql_defrag-0.1.0/gql_defrag/finder.py` & `gql_defrag-0.1.1/gql_defrag/finder.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def extract_from_js(source_dir: Path) -> Iterable[str]:
     """Extract GraphQL from JavaScript files."""
     for path in get_files(source_dir, {".js", ".jsx", ".ts", ".tsx"}):
         contents = path.read_text()
         for doc in re.findall(r"(?:graphql|gql)`([^`]+)`", contents):
-            yield doc.replace("null", '"null"')
+            yield clean_gql(doc)
 
 
 def extract_from_standalone_files(source_dir: Path, extension: str = ".graphql"):
     """Extract GraphQL from standalone files."""
     for path in get_files(source_dir, {extension}):
         yield path.read_text()
 
@@ -38,8 +38,13 @@
     """Extract GraphQL from Relay files."""
     for path in get_files(source_dir, {".ts"}):
         if not path.name.endswith(".graphql.ts"):
             continue
         contents = path.read_text()
         for doc in re.findall(r'"text": ("(?:\\"|[^"])+")', contents):
             doc = ast.literal_eval(doc)
-            yield doc.replace("null", '"null"')
+            yield clean_gql(doc)
+
+
+def clean_gql(gql: str) -> str:
+    # Our parser doesn't like 'null', so replace it with a string
+    return re.sub(r"\b(?<!\")null(?!\")\b", '"null"', gql)
```

### Comparing `gql_defrag-0.1.0/tests/test.py` & `gql_defrag-0.1.1/tests/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from gql_defrag import Defragmenter
+from gql_defrag.finder import clean_gql
 
 DOCUMENT = """
 query SomeQuery {
     field
     name
     ...SomeFragment
 }
@@ -21,7 +22,15 @@
 }
 """
 
 
 def test_basic() -> None:
     defragmenter = Defragmenter([DOCUMENT])
     assert defragmenter.defragment("SomeQuery").strip() == EXPECTED.strip()
+
+
+def test_null() -> None:
+    query = 'query SomeQuery { nullableField(arg: null, arg2: "null") }'
+    assert (
+        clean_gql(query).strip()
+        == 'query SomeQuery { nullableField(arg: "null", arg2: "null") }'
+    )
```

### Comparing `gql_defrag-0.1.0/README.md` & `gql_defrag-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,10 +88,14 @@
 `<query name>.graphql`.
 
 If `--include-source` is given, `@gql_defrag_source` are added with precise source
 information for each field.
 
 ## Changelog
 
+### Version 0.1.1 (July 25, 2023)
+
+- Fix bug with handling of fields that contain "null" in their name
+
 ### Version 0.1.0 (May 3, 2023)
 
 Initial public release.
```

### Comparing `gql_defrag-0.1.0/pyproject.toml` & `gql_defrag-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gql_defrag"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jelle Zijlstra", email="jelle@quora.com" },
 ]
 description = "Merge GraphQL fragments into the parent query"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `gql_defrag-0.1.0/PKG-INFO` & `gql_defrag-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql_defrag
-Version: 0.1.0
+Version: 0.1.1
 Summary: Merge GraphQL fragments into the parent query
 Project-URL: Homepage, https://github.com/JelleZijlstra/gql-defrag
 Author-email: Jelle Zijlstra <jelle@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -101,10 +101,14 @@
 `<query name>.graphql`.
 
 If `--include-source` is given, `@gql_defrag_source` are added with precise source
 information for each field.
 
 ## Changelog
 
+### Version 0.1.1 (July 25, 2023)
+
+- Fix bug with handling of fields that contain "null" in their name
+
 ### Version 0.1.0 (May 3, 2023)
 
 Initial public release.
```

