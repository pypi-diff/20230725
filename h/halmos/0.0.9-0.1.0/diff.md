# Comparing `tmp/halmos-0.0.9.tar.gz` & `tmp/halmos-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmos-0.0.9.tar", last modified: Mon Jul 10 05:12:16 2023, max compression
+gzip compressed data, was "halmos-0.1.0.tar", last modified: Tue Jul 25 01:35:05 2023, max compression
```

## Comparing `halmos-0.0.9.tar` & `halmos-0.1.0.tar`

### file list

```diff
@@ -1,69 +1,129 @@
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.079452 halmos-0.0.9/
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.071124 halmos-0.0.9/.github/
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.072952 halmos-0.0.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 dpark      (502) wheel        (0)      468 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 dpark      (502) wheel        (0)      604 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073341 halmos-0.0.9/.github/workflows/
--rw-r--r--   0 dpark      (502) wheel        (0)     2945 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/workflows/codeql.yml
--rw-r--r--   0 dpark      (502) wheel        (0)      439 2023-07-10 04:56:56.000000 halmos-0.0.9/.github/workflows/publish.yml
--rw-r--r--   0 dpark      (502) wheel        (0)      873 2023-07-10 04:57:15.000000 halmos-0.0.9/.github/workflows/test.yml
--rw-r--r--   0 dpark      (502) wheel        (0)      219 2023-07-10 04:56:56.000000 halmos-0.0.9/.gitignore
--rw-r--r--   0 dpark      (502) wheel        (0)      109 2023-07-10 04:56:56.000000 halmos-0.0.9/.gitmodules
--rw-r--r--   0 dpark      (502) wheel        (0)    34523 2023-07-10 04:56:56.000000 halmos-0.0.9/LICENSE
--rw-r--r--   0 dpark      (502) wheel        (0)     4542 2023-07-10 05:12:16.079294 halmos-0.0.9/PKG-INFO
--rw-r--r--   0 dpark      (502) wheel        (0)     4075 2023-07-10 04:57:15.000000 halmos-0.0.9/README.md
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073480 halmos-0.0.9/examples/
--rw-r--r--   0 dpark      (502) wheel        (0)      141 2023-07-10 04:56:56.000000 halmos-0.0.9/examples/foundry.toml
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073606 halmos-0.0.9/examples/src/
--rw-r--r--   0 dpark      (502) wheel        (0)     1030 2023-07-10 04:56:56.000000 halmos-0.0.9/examples/src/Example.sol
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.073751 halmos-0.0.9/examples/test/
--rw-r--r--   0 dpark      (502) wheel        (0)     1587 2023-07-10 04:56:56.000000 halmos-0.0.9/examples/test/Example.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      733 2023-07-10 04:56:56.000000 halmos-0.0.9/pyproject.toml
--rw-r--r--   0 dpark      (502) wheel        (0)       43 2023-07-10 04:56:56.000000 halmos-0.0.9/requirements.txt
--rw-r--r--   0 dpark      (502) wheel        (0)       38 2023-07-10 05:12:16.079489 halmos-0.0.9/setup.cfg
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.071638 halmos-0.0.9/src/
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.074585 halmos-0.0.9/src/halmos/
--rw-r--r--   0 dpark      (502) wheel        (0)       36 2023-07-10 04:56:56.000000 halmos-0.0.9/src/halmos/__init__.py
--rw-r--r--   0 dpark      (502) wheel        (0)    23618 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/__main__.py
--rw-r--r--   0 dpark      (502) wheel        (0)     1724 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/byte2op.py
--rw-r--r--   0 dpark      (502) wheel        (0)     3010 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/cheatcodes.py
--rw-r--r--   0 dpark      (502) wheel        (0)    59143 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/sevm.py
--rw-r--r--   0 dpark      (502) wheel        (0)    28892 2023-07-10 04:57:15.000000 halmos-0.0.9/src/halmos/utils.py
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.075398 halmos-0.0.9/src/halmos.egg-info/
--rw-r--r--   0 dpark      (502) wheel        (0)     4542 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/PKG-INFO
--rw-r--r--   0 dpark      (502) wheel        (0)     1290 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/SOURCES.txt
--rw-r--r--   0 dpark      (502) wheel        (0)        1 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/dependency_links.txt
--rw-r--r--   0 dpark      (502) wheel        (0)       48 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/entry_points.txt
--rw-r--r--   0 dpark      (502) wheel        (0)       39 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/requires.txt
--rw-r--r--   0 dpark      (502) wheel        (0)        7 2023-07-10 05:12:16.000000 halmos-0.0.9/src/halmos.egg-info/top_level.txt
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.075803 halmos-0.0.9/tests/
--rw-r--r--   0 dpark      (502) wheel        (0)      140 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/foundry.toml
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.076580 halmos-0.0.9/tests/src/
--rw-r--r--   0 dpark      (502) wheel        (0)      126 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Const.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1581 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Counter.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      334 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Create.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      405 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/List.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      184 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/SignExtend.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      905 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/src/Storage.sol
-drwxr-xr-x   0 dpark      (502) wheel        (0)        0 2023-07-10 05:12:16.079078 halmos-0.0.9/tests/test/
--rw-r--r--   0 dpark      (502) wheel        (0)     1092 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Arith.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      785 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Block.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      345 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Const.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     3155 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Counter.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      748 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Create.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      867 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Deal.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      732 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test/Foundry.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      691 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Invalid.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      594 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Library.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1648 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/List.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1319 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test/Opcode.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     3450 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Prank.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1832 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Send.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      650 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Setup.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1986 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test/SetupPlus.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      294 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/SignExtend.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1139 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Storage.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)      274 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Struct.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     1363 2023-07-10 04:56:56.000000 halmos-0.0.9/tests/test/Warp.t.sol
--rw-r--r--   0 dpark      (502) wheel        (0)     6085 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test_cli.py
--rw-r--r--   0 dpark      (502) wheel        (0)     6151 2023-07-10 04:57:15.000000 halmos-0.0.9/tests/test_sevm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.270598 halmos-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 01:34:56.000000 halmos-0.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.242597 halmos-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/test-external.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/test-long.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-25 01:34:56.000000 halmos-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 01:34:56.000000 halmos-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 01:34:56.000000 halmos-0.1.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 01:34:56.000000 halmos-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 01:34:56.000000 halmos-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-25 01:35:05.270598 halmos-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-25 01:34:56.000000 halmos-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/benchmarks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-25 01:34:56.000000 halmos-0.1.0/benchmarks/baolean.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.246598 halmos-0.1.0/examples/tokens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/examples/tokens/ERC20/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.250598 halmos-0.1.0/examples/tokens/ERC20/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/src/SolmateERC20.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC20/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/DEIStablecoin.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    27482 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/DEIStablecoin.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/ERC20Test.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC20/test/SolmateERC20.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC721/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC721/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/src/SolmateERC721.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/tokens/ERC721/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/test/ERC721Test.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/tokens/ERC721/test/SolmateERC721.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/toy/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/toy/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/toy/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/toy/src/Example.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.254598 halmos-0.1.0/examples/toy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-25 01:34:56.000000 halmos-0.1.0/examples/toy/test/Example.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 01:34:56.000000 halmos-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 01:34:56.000000 halmos-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 01:34:56.000000 halmos-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:35:05.270598 halmos-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.246598 halmos-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/src/halmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35162 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/cheatcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85996 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/sevm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 01:34:56.000000 halmos-0.1.0/src/halmos/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/src/halmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 01:35:05.000000 halmos-0.1.0/src/halmos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.258598 halmos-0.1.0/tests/expected/
+-rw-r--r--   0 runner    (1001) docker     (123)    34018 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/erc20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/erc721.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/expected/toy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.262598 halmos-0.1.0/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Const.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Counter.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Create.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/List.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/SignExtend.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/src/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:35:05.270598 halmos-0.1.0/tests/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Arith.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/AssertTest.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Block.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Byte.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Console.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Const.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Counter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Create.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Deal.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Foundry.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Getter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/HalmosCheatCode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Invalid.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Library.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/LibraryLinking.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/List.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Math.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Natspec.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Opcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Prank.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Proxy.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Reset.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Revert.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Send.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Setup.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/SetupPlus.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/SetupSymbolic.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/SignExtend.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Solver.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Storage.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Store.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Struct.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/TestConstructor.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Token.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/UnsupportedOpcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test/Warp.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_halmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-25 01:34:56.000000 halmos-0.1.0/tests/test_sevm.py
```

### Comparing `halmos-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md` & `halmos-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `halmos-0.0.9/.github/workflows/codeql.yml` & `halmos-0.1.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.0.9/.github/workflows/test.yml` & `halmos-0.1.0/.github/workflows/test-long.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-name: Test
+name: Test long
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
   test:
-    runs-on: ubuntu-latest
+    runs-on: macos-latest
 
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11", "3.8.13", "3.9.13", "3.10.6"]
+        include:
+        - testname: "examples/tokens/ERC20"
+        - testname: "examples/tokens/ERC721"
 
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: recursive
 
       - name: Install Foundry
         uses: foundry-rs/foundry-toolchain@v1
 
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: "3.11"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pytest
 
       - name: Install Halmos
         run: pip install -e .
 
       - name: Run pytest
-        run: pytest
-
-      - name: Test Halmos
-        run: halmos tests --solver-axioms
+        run: pytest -v tests/test_halmos.py -k ${{ matrix.testname }} --halmos-options="-v -st --error-unknown --test-parallel --solver-parallel --solver-timeout-assertion 0"
```

### Comparing `halmos-0.0.9/LICENSE` & `halmos-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `halmos-0.0.9/PKG-INFO` & `halmos-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.0.9
+Version: 0.1.0
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: Daejun Park
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -33,40 +33,45 @@
 
 ## Installation
 
 ```
 $ pip install halmos
 ```
 
+Or, if you want to try the latest dev version:
+```
+$ pip install git+https://github.com/a16z/halmos
+```
+
 ## Usage
 
 ```
 $ cd /path/to/src
 $ halmos
 ```
 
 For more details:
 ```
 $ halmos --help
 ```
 
 ## Examples
 
-Given a contract, [Example.sol](examples/src/Example.sol):
+Given a contract, [Example.sol](examples/toy/src/Example.sol):
 ```solidity
 contract Example {
     function totalPriceBuggy(uint96 price, uint32 quantity) public pure returns (uint128) {
         unchecked {
             return uint120(price) * quantity; // buggy type casting: uint120 vs uint128
         }
     }
 }
 ```
 
-You write some **property-based tests** (in Solidity), [Example.t.sol](examples/test/Example.t.sol):
+You write some **property-based tests** (in Solidity), [Example.t.sol](examples/toy/test/Example.t.sol):
 ```solidity
 contract ExampleTest is Example {
     function testTotalPriceBuggy(uint96 price, uint32 quantity) public pure {
         uint128 total = totalPriceBuggy(price, quantity);
         assert(quantity == 0 || total >= price);
     }
 }
@@ -83,10 +88,41 @@
 $ halmos
 [FAIL] testTotalPriceBuggy(uint96,uint32) (paths: 6, time: 0.10s, bounds: [])
 Counterexample: [p_price_uint96 = 39614081294025656978550816768, p_quantity_uint32 = 1073741824]
 ```
 
 _(In this specific example, Halmos discovered an input that violated the assertion, which was missed by the fuzzer!)_
 
+## Develop
+
+```sh
+# if you want to submit a pull request, fork the repository:
+
+gh repo fork a16z/halmos
+
+# or if you just want to develop locally, clone it
+# git clone git@github.com:a16z/halmos.git
+
+# create and activate a virtual environment
+
+python3.11 -m venv .venv
+source .venv/bin/activate
+
+# install the dependencies
+
+python -m pip install -r requirements.txt
+python -m pip install -r requirements-dev.txt
+
+# install and run the git hook scripts
+
+pre-commit install
+pre-commit run --all-files
+
+# we recommend enabling the black formatter in your editor
+# but you can run it manually if needed:
+
+python -m black .
+```
+
 ## Disclaimer
 
 _These smart contracts and code are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts and code. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions or loss of transmitted information. THE SMART CONTRACTS AND CODE CONTAINED HEREIN ARE FURNISHED AS IS, WHERE IS, WITH ALL FAULTS AND WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING ANY WARRANTY OF MERCHANTABILITY, NON-INFRINGEMENT OR FITNESS FOR ANY PARTICULAR PURPOSE. Further, use of any of these smart contracts and code may be restricted or prohibited under applicable law, including securities laws, and it is therefore strongly advised for you to contact a reputable attorney in any jurisdiction where these smart contracts and code may be accessible for any questions or concerns with respect thereto. Further, no information provided in this repo should be construed as investment advice or legal advice for any particular facts or circumstances, and is not meant to replace competent counsel. a16z is not liable for any use of the foregoing, and users should proceed with caution and use at their own risk. See a16z.com/disclosures for more info._
```

### Comparing `halmos-0.0.9/README.md` & `halmos-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,40 +20,45 @@
 
 ## Installation
 
 ```
 $ pip install halmos
 ```
 
+Or, if you want to try the latest dev version:
+```
+$ pip install git+https://github.com/a16z/halmos
+```
+
 ## Usage
 
 ```
 $ cd /path/to/src
 $ halmos
 ```
 
 For more details:
 ```
 $ halmos --help
 ```
 
 ## Examples
 
-Given a contract, [Example.sol](examples/src/Example.sol):
+Given a contract, [Example.sol](examples/toy/src/Example.sol):
 ```solidity
 contract Example {
     function totalPriceBuggy(uint96 price, uint32 quantity) public pure returns (uint128) {
         unchecked {
             return uint120(price) * quantity; // buggy type casting: uint120 vs uint128
         }
     }
 }
 ```
 
-You write some **property-based tests** (in Solidity), [Example.t.sol](examples/test/Example.t.sol):
+You write some **property-based tests** (in Solidity), [Example.t.sol](examples/toy/test/Example.t.sol):
 ```solidity
 contract ExampleTest is Example {
     function testTotalPriceBuggy(uint96 price, uint32 quantity) public pure {
         uint128 total = totalPriceBuggy(price, quantity);
         assert(quantity == 0 || total >= price);
     }
 }
@@ -70,10 +75,41 @@
 $ halmos
 [FAIL] testTotalPriceBuggy(uint96,uint32) (paths: 6, time: 0.10s, bounds: [])
 Counterexample: [p_price_uint96 = 39614081294025656978550816768, p_quantity_uint32 = 1073741824]
 ```
 
 _(In this specific example, Halmos discovered an input that violated the assertion, which was missed by the fuzzer!)_
 
+## Develop
+
+```sh
+# if you want to submit a pull request, fork the repository:
+
+gh repo fork a16z/halmos
+
+# or if you just want to develop locally, clone it
+# git clone git@github.com:a16z/halmos.git
+
+# create and activate a virtual environment
+
+python3.11 -m venv .venv
+source .venv/bin/activate
+
+# install the dependencies
+
+python -m pip install -r requirements.txt
+python -m pip install -r requirements-dev.txt
+
+# install and run the git hook scripts
+
+pre-commit install
+pre-commit run --all-files
+
+# we recommend enabling the black formatter in your editor
+# but you can run it manually if needed:
+
+python -m black .
+```
+
 ## Disclaimer
 
 _These smart contracts and code are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts and code. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions or loss of transmitted information. THE SMART CONTRACTS AND CODE CONTAINED HEREIN ARE FURNISHED AS IS, WHERE IS, WITH ALL FAULTS AND WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING ANY WARRANTY OF MERCHANTABILITY, NON-INFRINGEMENT OR FITNESS FOR ANY PARTICULAR PURPOSE. Further, use of any of these smart contracts and code may be restricted or prohibited under applicable law, including securities laws, and it is therefore strongly advised for you to contact a reputable attorney in any jurisdiction where these smart contracts and code may be accessible for any questions or concerns with respect thereto. Further, no information provided in this repo should be construed as investment advice or legal advice for any particular facts or circumstances, and is not meant to replace competent counsel. a16z is not liable for any use of the foregoing, and users should proceed with caution and use at their own risk. See a16z.com/disclosures for more info._
```

### Comparing `halmos-0.0.9/examples/src/Example.sol` & `halmos-0.1.0/examples/toy/src/Example.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.9/examples/test/Example.t.sol` & `halmos-0.1.0/examples/toy/test/Example.t.sol`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity >=0.8.0 <0.9.0;
 
 import "../src/Example.sol";
 
+/// @custom:halmos --solver-timeout-assertion 0
 contract ExampleTest is Example {
 
     function testTotalPriceBuggy(uint96 price, uint32 quantity) public pure {
         uint128 total = totalPriceBuggy(price, quantity);
         assert(quantity == 0 || total >= price);
     }
 
@@ -23,26 +24,28 @@
 
     function testIsPowerOfTwo(uint8 x) public pure {
         bool result1 = isPowerOfTwo(x);
         bool result2 = x == 1 || x == 2 || x == 4 || x == 8 || x == 16 || x == 32 || x == 64 || x == 128;
         assert(result1 == result2);
     }
 
+    /// @custom:halmos --loop 256
     function testIsPowerOfTwo(uint256 x) public pure {
         bool result1 = isPowerOfTwo(x);
         bool result2 = false;
         for (uint i = 0; i < 256; i++) { // NOTE: `--loop 256` option needed for complete verification
             if (x == 2**i) {
                 result2 = true;
                 break;
             }
         }
         assert(result1 == result2);
     }
 
+    /// @custom:halmos --loop 256
     function testIsPowerOfTwoEq(uint x) public pure {
         bool result1 = isPowerOfTwo(x);
         bool result2 = isPowerOfTwoIter(x);
         assert(result1 == result2);
     }
 
 }
```

### Comparing `halmos-0.0.9/pyproject.toml` & `halmos-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2", "black"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [project]
 name = "halmos"
 description = "Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode"
@@ -14,17 +14,19 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "crytic-compile >= 0.3.0, < 0.3.2",
     "z3-solver",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 halmos = "halmos.__main__:main"
 
 [project.urls]
 "Homepage" = "https://github.com/a16z/halmos"
+
+[tool.black]
+target-versions = ["py38", "py39", "py310", "py311"]
```

### Comparing `halmos-0.0.9/src/halmos/sevm.py` & `halmos-0.1.0/src/halmos/sevm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,878 +1,1697 @@
 # SPDX-License-Identifier: AGPL-3.0
 
 import json
 import math
+import re
 
 from copy import deepcopy
 from collections import defaultdict
-from typing import List, Dict, Set, Tuple, Any
+from typing import List, Dict, Union as UnionType, Tuple, Any, Optional
 from functools import reduce
 
 from z3 import *
-from .byte2op import Opcode, decode, concat, mnemonic
-from .utils import EVM, color_good, color_warn, sha3_inv
-from .cheatcodes import hevm_cheat_code, Prank
-
-Word = Any # z3 expression (including constants)
-Byte = Any # z3 expression (including constants)
-Bytes = Any # z3 expression (including constants)
+from .utils import (
+    EVM,
+    sha3_inv,
+    restore_precomputed_hashes,
+    str_opcode,
+    assert_address,
+    assert_uint256,
+    con_addr,
+    bv_value_to_bytes,
+    hexify,
+)
+from .cheatcodes import halmos_cheat_code, hevm_cheat_code, console, Prank
+
+Word = Any  # z3 expression (including constants)
+Byte = Any  # z3 expression (including constants)
+Bytes = Any  # z3 expression (including constants)
+Address = BitVecRef  # 160-bitvector
 
-Steps = Dict[int,Dict[str,Any]] # execution tree
+Steps = Dict[int, Dict[str, Any]]  # execution tree
 
 # symbolic states
-f_calldataload = Function('calldataload', BitVecSort(256), BitVecSort(256)) # index
-f_calldatasize = Function('calldatasize', BitVecSort(256))
-f_extcodesize  = Function('extcodesize' , BitVecSort(256), BitVecSort(256)) # target address
-f_extcodehash  = Function('extcodehash' , BitVecSort(256), BitVecSort(256)) # target address
-f_blockhash    = Function('blockhash'   , BitVecSort(256), BitVecSort(256)) # block number
-f_gas          = Function('gas'         , BitVecSort(256), BitVecSort(256)) # cnt
-f_gasprice     = Function('gasprice'    , BitVecSort(256))
-f_origin       = Function('origin'      , BitVecSort(256))
+# calldataload(index)
+f_calldataload = Function("calldataload", BitVecSort(256), BitVecSort(256))
+# calldatasize()
+f_calldatasize = Function("calldatasize", BitVecSort(256))
+# extcodesize(target address)
+f_extcodesize = Function("extcodesize", BitVecSort(160), BitVecSort(256))
+# extcodehash(target address)
+f_extcodehash = Function("extcodehash", BitVecSort(160), BitVecSort(256))
+# blockhash(block number)
+f_blockhash = Function("blockhash", BitVecSort(256), BitVecSort(256))
+# gas(cnt)
+f_gas = Function("gas", BitVecSort(256), BitVecSort(256))
+# gasprice()
+f_gasprice = Function("gasprice", BitVecSort(256))
+# origin()
+f_origin = Function("origin", BitVecSort(160))
 
 # uninterpreted arithmetic
-f_add  = Function('evm_add' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_sub  = Function('evm_sub' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_mul  = Function('evm_mul' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_div  = Function('evm_div' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_mod  = Function('evm_mod' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_sdiv = Function('evm_sdiv', BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_smod = Function('evm_smod', BitVecSort(256), BitVecSort(256), BitVecSort(256))
-f_exp  = Function('evm_exp' , BitVecSort(256), BitVecSort(256), BitVecSort(256))
-
-def con(n: int) -> Word:
-    return BitVecVal(n, 256)
-
-def wextend(mem: List[Byte], loc: int, size: int) -> None:
-    if len(mem) < loc + size:
-        mem.extend([BitVecVal(0, 8) for _ in range(loc + size - len(mem))])
+f_add = {
+    256: Function("evm_bvadd", BitVecSort(256), BitVecSort(256), BitVecSort(256)),
+    264: Function("evm_bvadd_264", BitVecSort(264), BitVecSort(264), BitVecSort(264)),
+}
+f_sub = Function("evm_bvsub", BitVecSort(256), BitVecSort(256), BitVecSort(256))
+f_mul = {
+    256: Function("evm_bvmul", BitVecSort(256), BitVecSort(256), BitVecSort(256)),
+    512: Function("evm_bvmul_512", BitVecSort(512), BitVecSort(512), BitVecSort(512)),
+}
+f_div = Function("evm_bvudiv", BitVecSort(256), BitVecSort(256), BitVecSort(256))
+f_mod = {
+    256: Function("evm_bvurem", BitVecSort(256), BitVecSort(256), BitVecSort(256)),
+    264: Function("evm_bvurem_264", BitVecSort(264), BitVecSort(264), BitVecSort(264)),
+    512: Function("evm_bvurem_512", BitVecSort(512), BitVecSort(512), BitVecSort(512)),
+}
+f_sdiv = Function("evm_bvsdiv", BitVecSort(256), BitVecSort(256), BitVecSort(256))
+f_smod = Function("evm_bvsrem", BitVecSort(256), BitVecSort(256), BitVecSort(256))
+f_exp = Function("evm_exp", BitVecSort(256), BitVecSort(256), BitVecSort(256))
+
+magic_address: int = 0xAAAA0000
+
+new_address_offset: int = 1
+
+
+def id_str(x: Any) -> str:
+    return hexify(x).replace(" ", "")
 
-def wload(mem: List[Byte], loc: int, size: int) -> Bytes:
+
+def name_of(x: str) -> str:
+    return re.sub(r"\s+", "_", x)
+
+
+class Instruction:
+    pc: int
+    opcode: int
+    operand: Optional[UnionType[bytes, BitVecRef]]
+
+    def __init__(self, opcode, **kwargs) -> None:
+        self.opcode = opcode
+
+        self.pc = kwargs.get("pc", -1)
+        self.operand = kwargs.get("operand", None)
+
+    def __str__(self) -> str:
+        operand_str = ""
+        if self.operand is not None:
+            operand = self.operand
+            if isinstance(operand, bytes):
+                operand = BitVecVal(
+                    int.from_bytes(self.operand, "big"), len(self.operand) * 8
+                )
+
+            expected_operand_length = instruction_length(self.opcode) - 1
+            actual_operand_length = operand.size() // 8
+            if expected_operand_length != actual_operand_length:
+                operand_str = f" ERROR {operand} ({expected_operand_length - actual_operand_length} bytes missed)"
+            else:
+                operand_str = " " + str(operand)
+
+        return f"{mnemonic(self.opcode)}{operand_str}"
+
+    def __repr__(self) -> str:
+        return f"Instruction({mnemonic(self.opcode)}, pc={self.pc}, operand={repr(self.operand)})"
+
+    def __len__(self) -> int:
+        return instruction_length(self.opcode)
+
+
+class NotConcreteError(Exception):
+    pass
+
+
+def unbox_int(x: Any) -> Any:
+    """Convert int-like objects to int"""
+    if isinstance(x, bytes):
+        return int.from_bytes(x, "big")
+
+    if is_bv_value(x):
+        return x.as_long()
+
+    return x
+
+
+def int_of(x: Any, err: str = "expected concrete value but got") -> int:
+    res = unbox_int(x)
+
+    if isinstance(res, int):
+        return res
+
+    raise NotConcreteError(f"{err}: {x}")
+
+
+def iter_bytes(x: Any, _byte_length: int = -1):
+    """Return an iterable over the bytes of x (concrete or symbolic)"""
+
+    if isinstance(x, bytes):
+        return x
+
+    if isinstance(x, int):
+        # the byte length must be passed explicitly for ints, or this will fail
+        return x.to_bytes(_byte_length, "big")
+
+    if is_bv_value(x):
+        return bv_value_to_bytes(x)
+
+    if is_bv(x):
+        if x.size() % 8 != 0:
+            raise ValueError(x)
+
+        # size in bytes
+        size = x.size() // 8
+        return [
+            simplify(Extract((size - 1 - i) * 8 + 7, (size - 1 - i) * 8, x))
+            for i in range(size)
+        ]
+
+    raise ValueError(x)
+
+
+def is_concrete(x: Any) -> bool:
+    return isinstance(x, int) or isinstance(x, bytes) or is_bv_value(x)
+
+
+def mnemonic(opcode) -> str:
+    if is_concrete(opcode):
+        opcode = int_of(opcode)
+        return str_opcode.get(opcode, hex(opcode))
+    else:
+        return str(opcode)
+
+
+def concat(args):
+    if len(args) > 1:
+        return Concat(args)
+    else:
+        return args[0]
+
+
+def uint256(x: BitVecRef) -> BitVecRef:
+    bitsize = x.size()
+    if bitsize > 256:
+        raise ValueError(x)
+    if bitsize == 256:
+        return x
+    return simplify(ZeroExt(256 - bitsize, x))
+
+
+def uint160(x: BitVecRef) -> BitVecRef:
+    bitsize = x.size()
+    if bitsize > 256:
+        raise ValueError(x)
+    if bitsize == 160:
+        return x
+    if bitsize > 160:
+        return simplify(Extract(159, 0, x))
+    else:
+        return simplify(ZeroExt(160 - bitsize, x))
+
+
+def con(n: int, size_bits=256) -> Word:
+    return BitVecVal(n, size_bits)
+
+
+def byte_length(x: Any) -> int:
+    if is_bv(x):
+        if x.size() % 8 != 0:
+            raise ValueError(x)
+        return x.size() >> 3
+
+    if isinstance(x, bytes):
+        return len(x)
+
+    raise ValueError(x)
+
+
+def instruction_length(opcode: Any) -> int:
+    opcode = int_of(opcode)
+    return (opcode - EVM.PUSH0 + 1) if EVM.PUSH1 <= opcode <= EVM.PUSH32 else 1
+
+
+def wextend(mem: List[UnionType[int, BitVecRef]], loc: int, size: int) -> None:
+    mem.extend([0] * (loc + size - len(mem)))
+
+
+def wload(
+    mem: List[UnionType[int, BitVecRef]], loc: int, size: int, prefer_concrete=False
+) -> UnionType[bytes, Bytes]:
     wextend(mem, loc, size)
-    return simplify(Concat(mem[loc:loc+size])) # BitVecSort(size * 8)
 
-def wstore(mem: List[Byte], loc: int, size: int, val: Bytes) -> None:
-    if not eq(val.sort(), BitVecSort(size*8)): raise ValueError(val)
+    memslice = mem[loc : loc + size]
+
+    # runtime sanity check: mem should only contain ints or BitVecs (not bytes)
+    all_concrete = True
+    for i in memslice:
+        if isinstance(i, int):
+            if not i in range(0, 256):
+                raise ValueError(i)
+            continue
+
+        if is_bv(i):
+            if not is_bv_value(i):
+                all_concrete = False
+            continue
+
+        raise ValueError(i)
+
+    if prefer_concrete and all_concrete:
+        # will raise an error if any i is not in range(0, 256)
+        return bytes([int_of(i) for i in memslice])
+
+    # wrap concrete bytes in BitVecs
+    # this would truncate the upper bits if the value didn't fit in 8 bits
+    # therefore we rely on the value range check above to raise an error
+    wrapped = [BitVecVal(i, 8) if not is_bv(i) else i for i in memslice]
+
+    # BitVecSort(size * 8)
+    return simplify(concat(wrapped))
+
+
+def wstore(
+    mem: List[UnionType[int, BitVecRef]], loc: int, size: int, val: Bytes
+) -> None:
+    if not eq(val.sort(), BitVecSort(size * 8)):
+        raise ValueError(val)
     wextend(mem, loc, size)
     for i in range(size):
-        mem[loc + i] = simplify(Extract((size-1 - i)*8+7, (size-1 - i)*8, val))
+        mem[loc + i] = simplify(
+            Extract((size - 1 - i) * 8 + 7, (size - 1 - i) * 8, val)
+        )
 
-def wstore_partial(mem: List[Byte], loc: int, offset: int, size: int, data: Bytes, datasize: int) -> None:
-    if size > 0:
-        if not datasize >= offset + size: raise ValueError(datasize, offset, size)
-        sub_data = Extract((datasize-1 - offset)*8+7, (datasize - offset - size)*8, data)
+
+def wstore_partial(
+    mem: List[UnionType[int, BitVecRef]],
+    loc: int,
+    offset: int,
+    size: int,
+    data: UnionType[bytes, Bytes],
+    datasize: int,
+) -> None:
+    if size <= 0:
+        return
+
+    if not datasize >= offset + size:
+        raise ValueError(datasize, offset, size)
+
+    if is_bv(data):
+        sub_data = Extract(
+            (datasize - 1 - offset) * 8 + 7, (datasize - offset - size) * 8, data
+        )
         wstore(mem, loc, size, sub_data)
+    elif isinstance(data, bytes):
+        sub_data = data[offset : offset + size]
+        mem[loc : loc + size] = sub_data
+    else:
+        raise ValueError(data)
+
 
-def wstore_bytes(mem: List[Byte], loc: int, size: int, arr: List[Byte]) -> None:
-    if not size == len(arr): raise ValueError(size, arr)
+def wstore_bytes(
+    mem: List[UnionType[int, BitVecRef]], loc: int, size: int, arr: List[Byte]
+) -> None:
+    if not size == len(arr):
+        raise ValueError(size, arr)
     wextend(mem, loc, size)
     for i in range(size):
-        if not eq(arr[i].sort(), BitVecSort(8)): raise ValueError(arr)
+        if not eq(arr[i].sort(), BitVecSort(8)):
+            raise ValueError(arr)
         mem[loc + i] = arr[i]
 
-def create_address(cnt: int) -> Word:
-    return con(0x220E + cnt)
 
-def valid_jump_destinations(pgm: List[Opcode]) -> Set[int]:
-    jumpdests = set()
-    i = 0
-    while i < len(pgm):
-        opcode = pgm[i].op[0]
-        if is_bv_value(opcode):
-            opcode = opcode.as_long()
-            if opcode == EVM.JUMPDEST:
-                jumpdests.add(i)
-            elif EVM.PUSH1 <= opcode <= EVM.PUSH32:
-                i += opcode - EVM.PUSH1 + 1
-        i += 1
-    return jumpdests
+def extract_bytes(data: BitVecRef, byte_offset: int, size_bytes: int) -> BitVecRef:
+    """Extract bytes from calldata. Zero-pad if out of bounds."""
+    n = data.size()
+    if n % 8 != 0:
+        raise ValueError(n)
+
+    # will extract hi - lo + 1 bits
+    hi = n - 1 - byte_offset * 8
+    lo = n - byte_offset * 8 - size_bytes * 8
+    lo = 0 if lo < 0 else lo
+
+    val = simplify(Extract(hi, lo, data))
+
+    zero_padding = size_bytes * 8 - val.size()
+    if zero_padding < 0:
+        raise ValueError(val)
+    if zero_padding > 0:
+        val = simplify(Concat(val, con(0, zero_padding)))
+
+    return val
+
+
+def extract_funsig(calldata: BitVecRef):
+    """Extracts the function signature (first 4 bytes) from calldata"""
+    n = calldata.size()
+    # return simplify(Extract(n-1, n-32, calldata))
+    return extract_bytes(calldata, 0, 4)
+
+
+def extract_string_argument(calldata: BitVecRef, arg_idx: int):
+    """Extracts idx-th argument of string from calldata"""
+    string_offset = int_of(
+        extract_bytes(calldata, 4 + arg_idx * 32, 32),
+        "symbolic offset for string argument",
+    )
+    string_length = int_of(
+        extract_bytes(calldata, 4 + string_offset, 32),
+        "symbolic size for string argument",
+    )
+    if string_length == 0:
+        return ""
+    string_value = int_of(
+        extract_bytes(calldata, 4 + string_offset + 32, string_length),
+        "symbolic string argument",
+    )
+    string_bytes = string_value.to_bytes(string_length, "big")
+    return string_bytes.decode("utf-8")
+
 
 class State:
     stack: List[Word]
     memory: List[Byte]
 
     def __init__(self) -> None:
         self.stack: List[Word] = []
         self.memory: List[Byte] = []
 
-    def __deepcopy__(self, memo): # -> State:
+    def __deepcopy__(self, memo):  # -> State:
         st = State()
         st.stack = deepcopy(self.stack)
         st.memory = deepcopy(self.memory)
         return st
 
     def __str__(self) -> str:
-        return ''.join([
-            'Stack: ', str(self.stack), '\n',
-            self.str_memory(),
-        ])
+        return "".join(
+            [
+                f"Stack: {str(self.stack)}\n",
+                # self.str_memory(),
+            ]
+        )
 
     def str_memory(self) -> str:
         idx: int = 0
-        ret: str = 'Memory:'
+        ret: str = "Memory:"
         size: int = len(self.memory)
         while idx < size:
-            ret = ret + '\n' + '- ' + str(hex(idx)) + ': ' + str(self.memory[idx:min(idx+32,size)])
-            idx = idx + 32
-        return ret + '\n'
+            ret += f"\n- {hex(idx)}: {self.memory[idx : min(idx + 32, size)]}"
+            idx += 32
+        return ret + "\n"
 
     def push(self, v: Word) -> None:
-        if not (eq(v.sort(), BitVecSort(256)) or is_bool(v)): raise ValueError(v)
+        if not (eq(v.sort(), BitVecSort(256)) or is_bool(v)):
+            raise ValueError(v)
         self.stack.insert(0, simplify(v))
 
     def pop(self) -> Word:
         v = self.stack[0]
         del self.stack[0]
         return v
 
     def dup(self, n: int) -> None:
-        self.push(self.stack[n-1])
+        self.push(self.stack[n - 1])
 
     def swap(self, n: int) -> None:
         tmp = self.stack[0]
         self.stack[0] = self.stack[n]
         self.stack[n] = tmp
 
     def mloc(self) -> int:
-        loc: int = int(str(self.pop())) # loc must be concrete
+        loc: int = int_of(self.pop(), "symbolic memory offset")
         return loc
 
     def mstore(self, full: bool) -> None:
         loc: int = self.mloc()
         val: Word = self.pop()
         if is_bool(val):
             val = If(val, con(1), con(0))
         if full:
             wstore(self.memory, loc, 32, val)
-        else: # mstore8
+        else:  # mstore8
             wstore_bytes(self.memory, loc, 1, [simplify(Extract(7, 0, val))])
 
     def mload(self) -> None:
         loc: int = self.mloc()
         self.push(wload(self.memory, loc, 32))
 
     def ret(self) -> Bytes:
         loc: int = self.mloc()
-        size: int = int(str(self.pop())) # size (in bytes) must be concrete
+        size: int = int_of(self.pop(), "symbolic return data size")  # size in bytes
         if size > 0:
-            return wload(self.memory, loc, size)
+            return wload(self.memory, loc, size, prefer_concrete=True)
         else:
             return None
 
+
 class Block:
-    basefee: Any
-    chainid: Any
-    coinbase: Any
-    difficulty: Any # prevrandao
-    gaslimit: Any
-    number: Any
-    timestamp: Any
+    basefee: BitVecRef
+    chainid: BitVecRef
+    coinbase: Address
+    difficulty: BitVecRef  # prevrandao
+    gaslimit: BitVecRef
+    number: BitVecRef
+    timestamp: BitVecRef
 
     def __init__(self, **kwargs) -> None:
-        self.basefee    = kwargs['basefee']
-        self.chainid    = kwargs['chainid']
-        self.coinbase   = kwargs['coinbase']
-        self.difficulty = kwargs['difficulty']
-        self.gaslimit   = kwargs['gaslimit']
-        self.number     = kwargs['number']
-        self.timestamp  = kwargs['timestamp']
+        self.basefee = kwargs["basefee"]
+        self.chainid = kwargs["chainid"]
+        self.coinbase = kwargs["coinbase"]
+        self.difficulty = kwargs["difficulty"]
+        self.gaslimit = kwargs["gaslimit"]
+        self.number = kwargs["number"]
+        self.timestamp = kwargs["timestamp"]
+
+        assert_address(self.coinbase)
+
+
+class Contract:
+    """Abstraction over contract bytecode. Can include concrete and symbolic elements."""
+
+    # for completely concrete code: _rawcode is a bytes object
+    # for completely or partially symbolic code: _rawcode is a single BitVec element
+    #    (typically a Concat() of concrete and symbolic values)
+    _rawcode: UnionType[bytes, BitVecRef]
+
+    def __init__(self, rawcode: UnionType[bytes, BitVecRef]) -> None:
+        if is_bv_value(rawcode):
+            if rawcode.size() % 8 != 0:
+                raise ValueError(rawcode)
+            rawcode = rawcode.as_long().to_bytes(rawcode.size() // 8, "big")
+        self._rawcode = rawcode
+
+    def __init_jumpdests(self):
+        self.jumpdests = set()
+
+        for insn in iter(self):
+            if insn.opcode == EVM.JUMPDEST:
+                self.jumpdests.add(insn.pc)
+
+    def __iter__(self):
+        return CodeIterator(self)
+
+    def from_hexcode(hexcode: str):
+        """Create a contract from a hexcode string, e.g. "aabbccdd" """
+        if not isinstance(hexcode, str):
+            raise ValueError(hexcode)
+
+        if len(hexcode) % 2 != 0:
+            raise ValueError(hexcode)
+
+        if hexcode.startswith("0x"):
+            hexcode = hexcode[2:]
+
+        return Contract(bytes.fromhex(hexcode))
+
+    def decode_instruction(self, pc: int) -> Instruction:
+        opcode = int_of(self[pc])
+
+        if EVM.PUSH1 <= opcode <= EVM.PUSH32:
+            operand = self[pc + 1 : pc + opcode - EVM.PUSH0 + 1]
+            return Instruction(opcode, pc=pc, operand=operand)
+
+        return Instruction(opcode, pc=pc)
+
+    def next_pc(self, pc):
+        opcode = self[pc]
+        return pc + instruction_length(opcode)
+
+    def __getslice__(self, slice):
+        step = 1 if slice.step is None else slice.step
+        if step != 1:
+            return ValueError(f"slice step must be 1 but got {slice}")
+
+        # symbolic
+        if is_bv(self._rawcode):
+            extracted = extract_bytes(
+                self._rawcode, slice.start, slice.stop - slice.start
+            )
+
+            # check if that part of the code is concrete
+            if is_bv_value(extracted):
+                return bv_value_to_bytes(extracted)
+
+            else:
+                return extracted
+
+        # concrete
+        return self._rawcode[slice.start : slice.stop]
+
+    def __getitem__(self, key) -> UnionType[int, BitVecRef]:
+        """Returns the byte at the given offset."""
+        if isinstance(key, slice):
+            return self.__getslice__(key)
+
+        offset = int_of(key, "symbolic index into contract bytecode")
+
+        # support for negative indexing, e.g. contract[-1]
+        if offset < 0:
+            return self[len(self) + offset]
+
+        # in the EVM, this is defined as returning 0
+        if offset >= len(self):
+            return 0
+
+        # symbolic
+        if is_bv(self._rawcode):
+            extracted = extract_bytes(self._rawcode, offset, 1)
+
+            # return as concrete if possible
+            return unbox_int(extracted)
+
+        # concrete
+        return self._rawcode[offset]
+
+    def __len__(self) -> int:
+        """Returns the length of the bytecode in bytes."""
+        return byte_length(self._rawcode)
+
+    def valid_jump_destinations(self) -> set:
+        """Returns the set of valid jump destinations."""
+        if not hasattr(self, "jumpdests"):
+            self.__init_jumpdests()
+
+        return self.jumpdests
+
+
+class CodeIterator:
+    def __init__(self, contract: Contract):
+        self.contract = contract
+        self.pc = 0
+        self.is_symbolic = is_bv(contract._rawcode)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self) -> Instruction:
+        """Returns a tuple of (pc, opcode)"""
+        if self.pc >= len(self.contract):
+            raise StopIteration
+
+        insn = self.contract.decode_instruction(self.pc)
+        self.pc += len(insn)
 
-class Exec: # an execution path
+        return insn
+
+
+class Exec:  # an execution path
     # network
-    pgm: Dict[Any,List[Opcode]] # address -> { opcode map: pc -> opcode }
-    code: Dict[Any,List[Any]] # address -> opcode sequence
-    storage: Dict[Any,Dict[int,Any]] # address -> { storage slot -> value }
-    balance: Any # address -> balance
+    code: Dict[Address, Contract]
+    storage: Dict[Address, Dict[int, Any]]  # address -> { storage slot -> value }
+    balance: Any  # address -> balance
     # block
     block: Block
     # tx
-    calldata: List[Byte] # msg.data
-    callvalue: Word # msg.value
-    caller: Word # msg.sender
-    this: Word # current account address
+    calldata: List[Byte]  # msg.data
+    callvalue: Word  # msg.value
+    caller: Address  # msg.sender
+    this: Address  # current account address
     # vm state
     pc: int
-    st: State # stack and memory
-    jumpis: Dict[str,Dict[bool,int]] # for loop detection
-    output: Any # returndata
-    symbolic: bool # symbolic or concrete storage
+    st: State  # stack and memory
+    jumpis: Dict[str, Dict[bool, int]]  # for loop detection
+    output: Any  # returndata
+    symbolic: bool  # symbolic or concrete storage
     prank: Prank
     # path
     solver: Solver
-    path: List[Any] # path conditions
+    path: List[Any]  # path conditions
     # logs
-    log: List[Tuple[List[Word], Any]] # event logs emitted
-    cnts: Dict[int,int] # opcode -> frequency
-    sha3s: List[Tuple[Word,Word]] # sha3 hashes generated
-    storages: Dict[Any,Any] # storage updates
-    balances: Dict[Any,Any] # balance updates
-    calls: List[Any] # external calls
+    log: List[Tuple[List[Word], Any]]  # event logs emitted
+    cnts: Dict[str, Dict[int, int]]  # opcode -> frequency; counters
+    sha3s: List[Tuple[Word, Word]]  # sha3 hashes generated
+    storages: Dict[Any, Any]  # storage updates
+    balances: Dict[Any, Any]  # balance updates
+    calls: List[Any]  # external calls
     failed: bool
     error: str
 
     def __init__(self, **kwargs) -> None:
-        self.pgm      = kwargs['pgm']
-        self.code     = kwargs['code']
-        self.storage  = kwargs['storage']
-        self.balance  = kwargs['balance']
+        self.code = kwargs["code"]
+        self.storage = kwargs["storage"]
+        self.balance = kwargs["balance"]
         #
-        self.block    = kwargs['block']
+        self.block = kwargs["block"]
         #
-        self.calldata = kwargs['calldata']
-        self.callvalue= kwargs['callvalue']
-        self.caller   = kwargs['caller']
-        self.this     = kwargs['this']
+        self.calldata = kwargs["calldata"]
+        self.callvalue = kwargs["callvalue"]
+        self.caller = kwargs["caller"]
+        self.this = kwargs["this"]
         #
-        self.pc       = kwargs['pc']
-        self.st       = kwargs['st']
-        self.jumpis   = kwargs['jumpis']
-        self.output   = kwargs['output']
-        self.symbolic = kwargs['symbolic']
-        self.prank    = kwargs['prank']
+        self.pc = kwargs["pc"]
+        self.st = kwargs["st"]
+        self.jumpis = kwargs["jumpis"]
+        self.output = kwargs["output"]
+        self.symbolic = kwargs["symbolic"]
+        self.prank = kwargs["prank"]
         #
-        self.solver   = kwargs['solver']
-        self.path     = kwargs['path']
+        self.solver = kwargs["solver"]
+        self.path = kwargs["path"]
         #
-        self.log      = kwargs['log']
-        self.cnts     = kwargs['cnts']
-        self.sha3s    = kwargs['sha3s']
-        self.storages = kwargs['storages']
-        self.balances = kwargs['balances']
-        self.calls    = kwargs['calls']
-        self.failed   = kwargs['failed']
-        self.error    = kwargs['error']
+        self.log = kwargs["log"]
+        self.cnts = kwargs["cnts"]
+        self.sha3s = kwargs["sha3s"]
+        self.storages = kwargs["storages"]
+        self.balances = kwargs["balances"]
+        self.calls = kwargs["calls"]
+        self.failed = kwargs["failed"]
+        self.error = kwargs["error"]
+
+        assert_address(self.caller)
+        assert_address(self.this)
+
+    def current_opcode(self) -> UnionType[int, BitVecRef]:
+        return unbox_int(self.code[self.this][self.pc])
+
+    def current_instruction(self) -> Instruction:
+        return self.code[self.this].decode_instruction(self.pc)
 
     def str_cnts(self) -> str:
-        return ''.join([f'{x[0]}: {x[1]}\n' for x in sorted(self.cnts.items(), key=lambda x: x[0])])
+        return "".join(
+            [
+                f"{x[0]}: {x[1]}\n"
+                for x in sorted(self.cnts["opcode"].items(), key=lambda x: x[0])
+            ]
+        )
 
     def str_solver(self) -> str:
-        return '\n'.join([str(cond) for cond in self.solver.assertions()])
+        return "\n".join([str(cond) for cond in self.solver.assertions()])
 
     def str_path(self) -> str:
-        return ''.join(map(lambda x: '- ' + str(x) + '\n', filter(lambda x: str(x) != 'True', self.path)))
+        return "".join(
+            map(
+                lambda x: "- " + str(x) + "\n",
+                filter(lambda x: str(x) != "True", self.path),
+            )
+        )
 
     def __str__(self) -> str:
-        return ''.join([
-            'PC: '              , str(self.this), ' ', str(self.pc), ' ', str(self.pgm[self.this][self.pc]), '\n',
-            str(self.st),
-            'Balance: '         , str(self.balance), '\n',
-            'Storage:\n'        , ''.join(map(lambda x: '- ' + str(x) + ': ' + str(self.storage[x]) + '\n', self.storage)),
-        #   'Solver:\n'         , self.str_solver(), '\n',
-            'Path:\n'           , self.str_path(),
-            'Output: '          , str(self.output) , '\n',
-            'Log: '             , str(self.log)    , '\n',
-        #   'Opcodes:\n'        , self.str_cnts(),
-        #   'Memsize: '         , str(len(self.st.memory)), '\n',
-            'Balance updates:\n', ''.join(map(lambda x: '- ' + str(x) + '\n', sorted(self.balances.items(), key=lambda x: str(x[0])))),
-            'Storage updates:\n', ''.join(map(lambda x: '- ' + str(x) + '\n', sorted(self.storages.items(), key=lambda x: str(x[0])))),
-            'SHA3 hashes:\n'    , ''.join(map(lambda x: '- ' + str(x) + '\n', self.sha3s)),
-            'External calls:\n' , ''.join(map(lambda x: '- ' + str(x) + '\n', self.calls)),
-        #   'Calldata: '        , str(self.calldata), '\n',
-        ])
+        return hexify(
+            "".join(
+                [
+                    f"PC: {self.this} {self.pc} {mnemonic(self.current_opcode())}\n",
+                    str(self.st),
+                    f"Balance: {self.balance}\n",
+                    f"Storage:\n",
+                    "".join(
+                        map(
+                            lambda x: f"- {x}: {self.storage[x]}\n",
+                            self.storage,
+                        )
+                    ),
+                    # f"Solver:\n{self.str_solver()}\n",
+                    f"Path:\n{self.str_path()}",
+                    f"Output: {self.output.hex() if isinstance(self.output, bytes) else self.output}\n",
+                    f"Log: {self.log}\n",
+                    # f"Opcodes:\n{self.str_cnts()}",
+                    # f"Memsize: {len(self.st.memory)}\n",
+                    f"Balance updates:\n",
+                    "".join(
+                        map(
+                            lambda x: f"- {x}\n",
+                            sorted(self.balances.items(), key=lambda x: str(x[0])),
+                        )
+                    ),
+                    f"Storage updates:\n",
+                    "".join(
+                        map(
+                            lambda x: f"- {x}\n",
+                            sorted(self.storages.items(), key=lambda x: str(x[0])),
+                        )
+                    ),
+                    f"SHA3 hashes:\n",
+                    "".join(map(lambda x: f"- {x}\n", self.sha3s)),
+                    f"External calls:\n",
+                    "".join(map(lambda x: f"- {x}\n", self.calls)),
+                    # f"Calldata: {self.calldata}\n",
+                ]
+            )
+        )
 
     def next_pc(self) -> None:
-        self.pc += 1
-        while self.pgm[self.this][self.pc] is None:
-            self.pc += 1
+        self.pc = self.code[self.this].next_pc(self.pc)
 
     def check(self, cond: Any) -> Any:
         self.solver.push()
         self.solver.add(simplify(cond))
         result = self.solver.check()
         self.solver.pop()
         return result
 
     def select(self, array: Any, key: Word, arrays: Dict) -> Word:
         if array in arrays:
             store = arrays[array]
-            if store.decl().name() == 'store' and store.num_args() == 3:
+            if store.decl().name() == "store" and store.num_args() == 3:
                 base = store.arg(0)
                 key0 = store.arg(1)
                 val0 = store.arg(2)
-                if eq(key, key0): # structural equality
+                if eq(key, key0):  # structural equality
                     return val0
-                if self.check(key == key0) == unsat: # key != key0
+                if self.check(key == key0) == unsat:  # key != key0
                     return self.select(base, key, arrays)
-                if self.check(key != key0) == unsat: # key == key0
+                if self.check(key != key0) == unsat:  # key == key0
                     return val0
+        # empty array
+        elif not self.symbolic and re.search(r"^storage_.+_00$", str(array)):
+            # note: simplifying empty array access might have a negative impact on solver performance
+            return con(0)
         return Select(array, key)
 
     def balance_of(self, addr: Word) -> Word:
+        assert_address(addr)
         value = self.select(self.balance, addr, self.balances)
-        self.solver.add(ULT(value, con(2**96))) # practical assumption on the max balance per account
+        # practical assumption on the max balance per account
+        self.solver.add(ULT(value, con(2**96)))
         return value
 
     def balance_update(self, addr: Word, value: Word):
-        new_balance_var = Array(f'balance{1+len(self.balances)}', BitVecSort(256), BitVecSort(256))
+        assert_address(addr)
+        assert_uint256(value)
+        new_balance_var = Array(
+            f"balance_{1+len(self.balances):>02}", BitVecSort(160), BitVecSort(256)
+        )
         new_balance = Store(self.balance, addr, value)
         self.solver.add(new_balance_var == new_balance)
         self.balance = new_balance_var
         self.balances[new_balance_var] = new_balance
 
-    def sinit(self, slot: int, keys) -> None:
-        if slot not in self.storage[self.this]:
-            self.storage[self.this][slot] = {}
-        if len(keys) not in self.storage[self.this][slot]:
+    def empty_storage_of(self, addr: BitVecRef, slot: int, len_keys: int) -> ArrayRef:
+        return Array(
+            f"storage_{id_str(addr)}_{slot}_{len_keys}_00",
+            BitVecSort(len_keys * 256),
+            BitVecSort(256),
+        )
+
+    def sinit(self, addr: Any, slot: int, keys) -> None:
+        assert_address(addr)
+        if slot not in self.storage[addr]:
+            self.storage[addr][slot] = {}
+        if len(keys) not in self.storage[addr][slot]:
             if len(keys) == 0:
                 if self.symbolic:
-                    self.storage[self.this][slot][len(keys)] = BitVec(f'storage_slot_{str(slot)}_{str(len(keys))}', 256)
+                    self.storage[addr][slot][len(keys)] = BitVec(
+                        f"storage_{id_str(addr)}_{slot}_{len(keys)}_00", 256
+                    )
                 else:
-                    self.storage[self.this][slot][len(keys)] = con(0)
+                    self.storage[addr][slot][len(keys)] = con(0)
             else:
-                if self.symbolic:
-                    self.storage[self.this][slot][len(keys)] = Array(f'storage_slot_{str(slot)}_{str(len(keys))}', BitVecSort(len(keys)*256), BitVecSort(256))
-                else:
-                    self.storage[self.this][slot][len(keys)] = K(BitVecSort(len(keys)*256), con(0))
+                # do not use z3 const array `K(BitVecSort(len(keys)*256), con(0))` when not self.symbolic
+                # instead use normal smt array, and generate emptyness axiom; see sload()
+                self.storage[addr][slot][len(keys)] = self.empty_storage_of(
+                    addr, slot, len(keys)
+                )
 
-    def sload(self, loc: Word) -> Word:
+    def sload(self, addr: Any, loc: Word) -> Word:
         offsets = self.decode_storage_loc(loc)
-        if not len(offsets) > 0: raise ValueError(offsets)
-        slot, keys = int(str(offsets[0])), offsets[1:]
-        self.sinit(slot, keys)
+        if not len(offsets) > 0:
+            raise ValueError(offsets)
+        slot, keys = int_of(offsets[0], "symbolic storage base slot"), offsets[1:]
+        self.sinit(addr, slot, keys)
         if len(keys) == 0:
-            return self.storage[self.this][slot][0]
+            return self.storage[addr][slot][0]
         else:
-            return self.select(self.storage[self.this][slot][len(keys)], concat(keys), self.storages)
+            if not self.symbolic:
+                # generate emptyness axiom for each array index, instead of using quantified formula; see sinit()
+                self.solver.add(
+                    Select(self.empty_storage_of(addr, slot, len(keys)), concat(keys))
+                    == con(0)
+                )
+            return self.select(
+                self.storage[addr][slot][len(keys)], concat(keys), self.storages
+            )
 
-    def sstore(self, loc: Any, val: Any) -> None:
+    def sstore(self, addr: Any, loc: Any, val: Any) -> None:
         offsets = self.decode_storage_loc(loc)
-        if not len(offsets) > 0: raise ValueError(offsets)
-        slot, keys = int(str(offsets[0])), offsets[1:]
-        self.sinit(slot, keys)
+        if not len(offsets) > 0:
+            raise ValueError(offsets)
+        slot, keys = int_of(offsets[0], "symbolic storage base slot"), offsets[1:]
+        self.sinit(addr, slot, keys)
         if len(keys) == 0:
-            self.storage[self.this][slot][0] = val
+            self.storage[addr][slot][0] = val
         else:
-            new_storage_var = Array(f'storage{self.cnt_sstore()}', BitVecSort(len(keys)*256), BitVecSort(256))
-            new_storage = Store(self.storage[self.this][slot][len(keys)], concat(keys), val)
+            new_storage_var = Array(
+                f"storage_{id_str(addr)}_{slot}_{len(keys)}_{1+len(self.storages):>02}",
+                BitVecSort(len(keys) * 256),
+                BitVecSort(256),
+            )
+            new_storage = Store(self.storage[addr][slot][len(keys)], concat(keys), val)
             self.solver.add(new_storage_var == new_storage)
-            self.storage[self.this][slot][len(keys)] = new_storage_var
+            self.storage[addr][slot][len(keys)] = new_storage_var
             self.storages[new_storage_var] = new_storage
 
     def decode_storage_loc(self, loc: Any) -> Any:
         def normalize(expr: Any) -> Any:
             # Concat(Extract(255, 8, bvadd(x, y)), bvadd(Extract(7, 0, x), Extract(7, 0, y))) => x + y
-            if expr.decl().name() == 'concat' and expr.num_args() == 2:
-                arg0 = expr.arg(0) # Extract(255, 8, bvadd(x, y))
-                arg1 = expr.arg(1) # bvadd(Extract(7, 0, x), Extract(7, 0, y))
-                if arg0.decl().name() == 'extract' and arg0.num_args() == 1 and arg0.params() == [255, 8]:
-                    arg00 = arg0.arg(0) # bvadd(x, y)
-                    if arg00.decl().name() == 'bvadd':
+            if expr.decl().name() == "concat" and expr.num_args() == 2:
+                arg0 = expr.arg(0)  # Extract(255, 8, bvadd(x, y))
+                arg1 = expr.arg(1)  # bvadd(Extract(7, 0, x), Extract(7, 0, y))
+                if (
+                    arg0.decl().name() == "extract"
+                    and arg0.num_args() == 1
+                    and arg0.params() == [255, 8]
+                ):
+                    arg00 = arg0.arg(0)  # bvadd(x, y)
+                    if arg00.decl().name() == "bvadd":
                         x = arg00.arg(0)
                         y = arg00.arg(1)
-                        if arg1.decl().name() == 'bvadd' and arg1.num_args() == 2:
-                            if arg1.arg(0) == Extract(7, 0, x) and arg1.arg(1) == Extract(7, 0, y):
+                        if arg1.decl().name() == "bvadd" and arg1.num_args() == 2:
+                            if eq(arg1.arg(0), simplify(Extract(7, 0, x))) and eq(
+                                arg1.arg(1), simplify(Extract(7, 0, y))
+                            ):
                                 return x + y
             return expr
+
         loc = normalize(loc)
 
-        if loc.decl().name() == 'sha3_512': # m[k] : hash(k.m)
+        if loc.decl().name() == "sha3_512":  # m[k] : hash(k.m)
             args = loc.arg(0)
-            offset, base = simplify(Extract(511, 256, args)), simplify(Extract(255, 0, args))
-            return self.decode_storage_loc(base) + (offset,con(0))
-        elif loc.decl().name() == 'sha3_256': # a[i] : hash(a)+i
+            offset, base = simplify(Extract(511, 256, args)), simplify(
+                Extract(255, 0, args)
+            )
+            return self.decode_storage_loc(base) + (offset, con(0))
+        elif loc.decl().name() == "sha3_256":  # a[i] : hash(a)+i
             base = loc.arg(0)
             return self.decode_storage_loc(base) + (con(0),)
-        elif loc.decl().name() == 'bvadd':
-        #   # when len(args) == 2
-        #   arg0 = self.decode_storage_loc(loc.arg(0))
-        #   arg1 = self.decode_storage_loc(loc.arg(1))
-        #   if len(arg0) == 1 and len(arg1) > 1: # i + hash(x)
-        #       return arg1[0:-1] + (arg1[-1] + arg0[0],)
-        #   elif len(arg0) > 1 and len(arg1) == 1: # hash(x) + i
-        #       return arg0[0:-1] + (arg0[-1] + arg1[0],)
-        #   elif len(arg0) == 1 and len(arg1) == 1: # i + j
-        #       return (arg0[0] + arg1[0],)
-        #   else: # hash(x) + hash(y) # ambiguous
-        #       raise ValueError(loc)
+        elif loc.decl().name() == "bvadd":
+            #   # when len(args) == 2
+            #   arg0 = self.decode_storage_loc(loc.arg(0))
+            #   arg1 = self.decode_storage_loc(loc.arg(1))
+            #   if len(arg0) == 1 and len(arg1) > 1: # i + hash(x)
+            #       return arg1[0:-1] + (arg1[-1] + arg0[0],)
+            #   elif len(arg0) > 1 and len(arg1) == 1: # hash(x) + i
+            #       return arg0[0:-1] + (arg0[-1] + arg1[0],)
+            #   elif len(arg0) == 1 and len(arg1) == 1: # i + j
+            #       return (arg0[0] + arg1[0],)
+            #   else: # hash(x) + hash(y) # ambiguous
+            #       raise ValueError(loc)
             # when len(args) >= 2
             args = loc.children()
-            if len(args) < 2: raise ValueError(loc)
-            args = sorted(map(self.decode_storage_loc, args), key=lambda x: len(x), reverse=True)
-            if len(args[1]) > 1: raise ValueError(loc) # only args[0]'s length >= 1, the others must be 1
-            return args[0][0:-1] + (reduce(lambda r, x: r + x[0], args[1:], args[0][-1]),)
-        elif is_bv_value(loc) and int(str(loc)) in sha3_inv:
-            return (con(sha3_inv[int(str(loc))]), con(0))
+            if len(args) < 2:
+                raise ValueError(loc)
+            args = sorted(
+                map(self.decode_storage_loc, args), key=lambda x: len(x), reverse=True
+            )
+            if len(args[1]) > 1:
+                # only args[0]'s length >= 1, the others must be 1
+                raise ValueError(loc)
+            return args[0][0:-1] + (
+                reduce(lambda r, x: r + x[0], args[1:], args[0][-1]),
+            )
+        elif is_bv_value(loc):
+            (preimage, delta) = restore_precomputed_hashes(loc.as_long())
+            if preimage:  # loc == hash(preimage) + delta
+                return (con(preimage), con(delta))
+            else:
+                return (loc,)
         elif is_bv(loc):
             return (loc,)
         else:
             raise ValueError(loc)
 
     def sha3(self) -> None:
         loc: int = self.st.mloc()
-        size: int = int(str(self.st.pop())) # size (in bytes) must be concrete
+        size: int = int_of(self.st.pop(), "symbolic SHA3 data size")
         self.sha3_data(wload(self.st.memory, loc, size), size)
 
     def sha3_data(self, data: Bytes, size: int) -> None:
-        f_sha3 = Function('sha3_'+str(size*8), BitVecSort(size*8), BitVecSort(256))
+        f_sha3 = Function(
+            "sha3_" + str(size * 8), BitVecSort(size * 8), BitVecSort(256)
+        )
         sha3 = f_sha3(data)
-        sha3_var = BitVec(f'sha3_var{self.cnt_sha3()}', 256)
+        sha3_var = BitVec(f"sha3_var_{len(self.sha3s):>02}", 256)
         self.solver.add(sha3_var == sha3)
-        self.solver.add(ULE(sha3_var, con(2**256 - 2**64))) # assume hash values are sufficiently smaller than the uint max
+        # assume hash values are sufficiently smaller than the uint max
+        self.solver.add(ULE(sha3_var, con(2**256 - 2**64)))
         self.assume_sha3_distinct(sha3_var, sha3)
-        if size == 64 or size == 32: # for storage hashed location
+        if size == 64 or size == 32:  # for storage hashed location
             self.st.push(sha3)
         else:
             self.st.push(sha3_var)
 
     def assume_sha3_distinct(self, sha3_var, sha3) -> None:
-        for (v,s) in self.sha3s:
-            if s.decl().name() == sha3.decl().name(): # same size
-            #   self.solver.add(Implies(sha3_var == v, sha3.arg(0) == s.arg(0)))
+        for v, s in self.sha3s:
+            if s.decl().name() == sha3.decl().name():  # same size
+                # self.solver.add(Implies(sha3_var == v, sha3.arg(0) == s.arg(0)))
                 self.solver.add(Implies(sha3.arg(0) != s.arg(0), sha3_var != v))
             else:
                 self.solver.add(sha3_var != v)
         self.solver.add(sha3_var != con(0))
         self.sha3s.append((sha3_var, sha3))
 
-    def cnt_call(self) -> int:
-        return self.cnts[EVM.CALL] + self.cnts[EVM.STATICCALL]
-    def cnt_sstore(self) -> int:
-        return self.cnts[EVM.SSTORE]
-    def cnt_gas(self) -> int:
-        return self.cnts[EVM.GAS]
-    def cnt_balance(self) -> int:
-        return self.cnts[EVM.BALANCE]
-    def cnt_sha3(self) -> int:
-        return self.cnts[EVM.SHA3]
-    def cnt_create(self) -> int:
-        return self.cnts[EVM.CREATE]
+    def new_gas_id(self) -> int:
+        self.cnts["fresh"]["gas"] += 1
+        return self.cnts["fresh"]["gas"]
+
+    def new_address(self) -> Address:
+        self.cnts["fresh"]["address"] += 1
+        return con_addr(
+            magic_address + new_address_offset + self.cnts["fresh"]["address"]
+        )
+
+    def new_symbol_id(self) -> int:
+        self.cnts["fresh"]["symbol"] += 1
+        return self.cnts["fresh"]["symbol"]
 
     def returndatasize(self) -> int:
-        if self.output is None:
-            return 0
-        else:
-            size: int = self.output.size()
-            if not size % 8 == 0: raise ValueError(size)
-            return int(size / 8)
-
-    def read_code(self, idx: int) -> Byte:
-        if idx < len(self.code[self.this]):
-            return self.code[self.this][idx]
-        else:
-            return BitVecVal(0, 8)
+        return 0 if self.output is None else byte_length(self.output)
 
     def is_jumpdest(self, x: Word) -> bool:
-        if not is_bv_value(x): return False
-        pc: int = int(str(x))
-        if pc < 0 or pc >= len(self.pgm[self.this]): return False
-        if self.pgm[self.this][pc] is None: return False
-        opcode = self.pgm[self.this][pc].op[0]
-        return is_bv_value(opcode) and opcode.as_long() == EVM.JUMPDEST
+        if not is_concrete(x):
+            return False
+
+        pc: int = int_of(x)
+        if pc < 0:
+            raise ValueError(pc)
+
+        opcode = unbox_int(self.code[self.this][pc])
+        return opcode == EVM.JUMPDEST
 
     def jumpi_id(self) -> str:
-        return f'{self.pc}:' + ','.join(map(lambda x: str(x) if self.is_jumpdest(x) else '', self.st.stack))
+        return f"{self.pc}:" + ",".join(
+            map(lambda x: str(x) if self.is_jumpdest(x) else "", self.st.stack)
+        )
 
-# convert opcode list to opcode map
-def ops_to_pgm(ops: List[Opcode]) -> List[Opcode]:
-    pgm: List[Opcode] = [None for _ in range(ops[-1].pc + 1)]
-    for o in ops:
-        pgm[o.pc] = o
-    return pgm
 
 #             x  == b   if sort(x) = bool
 # int_to_bool(x) == b   if sort(x) = int
 def test(x: Word, b: bool) -> Word:
     if is_bool(x):
         if b:
             return x
         else:
             return Not(x)
     elif is_bv(x):
         if b:
-            return (x != con(0))
+            return x != con(0)
         else:
-            return (x == con(0))
+            return x == con(0)
     else:
         raise ValueError(x)
 
+
 def is_non_zero(x: Word) -> Word:
     return test(x, True)
 
+
 def is_zero(x: Word) -> Word:
     return test(x, False)
 
+
 def and_or(x: Word, y: Word, is_and: bool) -> Word:
     if is_bool(x) and is_bool(y):
         if is_and:
             return And(x, y)
         else:
             return Or(x, y)
     elif is_bv(x) and is_bv(y):
         if is_and:
-            return (x & y)
+            return x & y
         else:
-            return (x | y)
+            return x | y
     elif is_bool(x) and is_bv(y):
         return and_or(If(x, con(1), con(0)), y, is_and)
     elif is_bv(x) and is_bool(y):
         return and_or(x, If(y, con(1), con(0)), is_and)
     else:
         raise ValueError(x, y, is_and)
 
+
 def and_of(x: Word, y: Word) -> Word:
     return and_or(x, y, True)
 
+
 def or_of(x: Word, y: Word) -> Word:
     return and_or(x, y, False)
 
+
 def b2i(w: Word) -> Word:
     if is_true(w):
         return con(1)
     if is_false(w):
         return con(0)
     if is_bool(w):
         return If(w, con(1), con(0))
     else:
         return w
 
+
 def is_power_of_two(x: int) -> bool:
     if x > 0:
         return not (x & (x - 1))
     else:
         return False
 
+
 class SEVM:
     options: Dict
 
     def __init__(self, options: Dict) -> None:
         self.options = options
 
     def div_xy_y(self, w1: Word, w2: Word) -> Word:
         # return the number of bits required to represent the given value. default = 256
         def bitsize(w: Word) -> int:
-            if w.decl().name() == 'concat' and is_bv_value(w.arg(0)) and int(str(w.arg(0))) == 0:
+            if (
+                w.decl().name() == "concat"
+                and is_bv_value(w.arg(0))
+                and int(str(w.arg(0))) == 0
+            ):
                 return 256 - w.arg(0).size()
             return 256
-        if w1.decl().name() == 'bvmul' and w1.num_args() == 2:
+
+        if w1.decl().name() == "bvmul" and w1.num_args() == 2:
             x = w1.arg(0)
             y = w1.arg(1)
-            if w2 == x or w2 == y: # xy/x or xy/y
+            if eq(w2, x) or eq(w2, y):  # xy/x or xy/y
                 size_x = bitsize(x)
                 size_y = bitsize(y)
                 if size_x + size_y <= 256:
-                    if w2 == x: # xy/x == y
+                    if eq(w2, x):  # xy/x == y
                         return y
-                    else: # xy/y == x
+                    else:  # xy/y == x
                         return x
         return None
 
-    def arith(self, op: int, w1: Word, w2: Word) -> Word:
+    def mk_add(self, x: Any, y: Any) -> Any:
+        f_add[x.size()](x, y)
+
+    def mk_mul(self, x: Any, y: Any) -> Any:
+        f_mul[x.size()](x, y)
+
+    def mk_div(self, ex: Exec, x: Any, y: Any) -> Any:
+        term = f_div(x, y)
+        ex.solver.add(ULE(term, x))  # (x / y) <= x
+        return term
+
+    def mk_mod(self, ex: Exec, x: Any, y: Any) -> Any:
+        term = f_mod[x.size()](x, y)
+        ex.solver.add(ULE(term, y))  # (x % y) <= y
+        # ex.solver.add(Or(y == con(0), ULT(term, y))) # (x % y) < y if y != 0
+        return term
+
+    def arith(self, ex: Exec, op: int, w1: Word, w2: Word) -> Word:
         w1 = b2i(w1)
         w2 = b2i(w2)
         if op == EVM.ADD:
-            if self.options.get('add'):
+            if self.options.get("add"):
                 return w1 + w2
             if is_bv_value(w1) and is_bv_value(w2):
                 return w1 + w2
             else:
-                return f_add(w1, w2)
+                return self.mk_add(w1, w2)
         elif op == EVM.SUB:
-            if self.options.get('sub'):
+            if self.options.get("sub"):
                 return w1 - w2
             if is_bv_value(w1) and is_bv_value(w2):
                 return w1 - w2
             else:
                 return f_sub(w1, w2)
         elif op == EVM.MUL:
-            if self.options.get('mul'):
+            if self.options.get("mul"):
                 return w1 * w2
             if is_bv_value(w1) and is_bv_value(w2):
                 return w1 * w2
             elif is_bv_value(w1):
-                i1: int = int(str(w1)) # must be concrete
+                i1: int = int(str(w1))  # must be concrete
                 if i1 == 0:
-                    return con(0)
+                    return w1
                 elif is_power_of_two(i1):
-                    return w2 << int(math.log(i1,2))
+                    return w2 << int(math.log(i1, 2))
                 else:
-                    return f_mul(w1, w2)
+                    return self.mk_mul(w1, w2)
             elif is_bv_value(w2):
-                i2: int = int(str(w2)) # must be concrete
+                i2: int = int(str(w2))  # must be concrete
                 if i2 == 0:
-                    return con(0)
+                    return w2
                 elif is_power_of_two(i2):
-                    return w1 << int(math.log(i2,2))
+                    return w1 << int(math.log(i2, 2))
                 else:
-                    return f_mul(w1, w2)
+                    return self.mk_mul(w1, w2)
             else:
-                return f_mul(w1, w2)
+                return self.mk_mul(w1, w2)
         elif op == EVM.DIV:
             div_for_overflow_check = self.div_xy_y(w1, w2)
-            if div_for_overflow_check is not None: # xy/x or xy/y
+            if div_for_overflow_check is not None:  # xy/x or xy/y
                 return div_for_overflow_check
-            if self.options.get('div'):
-                return UDiv(w1, w2) # unsigned div (bvudiv)
+            if self.options.get("div"):
+                return UDiv(w1, w2)  # unsigned div (bvudiv)
             if is_bv_value(w1) and is_bv_value(w2):
                 return UDiv(w1, w2)
             elif is_bv_value(w2):
-                i2: int = int(str(w2)) # must be concrete
+                i2: int = int(str(w2))  # must be concrete
                 if i2 == 0:
-                    return con(0)
+                    return w2
                 elif i2 == 1:
                     return w1
                 elif is_power_of_two(i2):
-                    return LShR(w1, int(math.log(i2,2)))
-                elif self.options.get('divByConst'):
+                    return LShR(w1, int(math.log(i2, 2)))
+                elif self.options.get("divByConst"):
                     return UDiv(w1, w2)
                 else:
-                    return f_div(w1, w2)
+                    return self.mk_div(ex, w1, w2)
             else:
-                return f_div(w1, w2)
+                return self.mk_div(ex, w1, w2)
         elif op == EVM.MOD:
+            if self.options.get("mod"):
+                return URem(w1, w2)
             if is_bv_value(w1) and is_bv_value(w2):
-                return URem(w1, w2) # bvurem
+                return URem(w1, w2)  # bvurem
             elif is_bv_value(w2):
                 i2: int = int(str(w2))
                 if i2 == 0 or i2 == 1:
-                    return con(0)
+                    return con(0, w2.size())
                 elif is_power_of_two(i2):
-                    bitsize = int(math.log(i2,2))
-                    return ZeroExt(256-bitsize, Extract(bitsize-1, 0, w1))
-                elif self.options.get('modByConst'):
+                    bitsize = int(math.log(i2, 2))
+                    return ZeroExt(w2.size() - bitsize, Extract(bitsize - 1, 0, w1))
+                elif self.options.get("modByConst"):
                     return URem(w1, w2)
                 else:
-                    return f_mod(w1, w2)
+                    return self.mk_mod(ex, w1, w2)
             else:
-                return f_mod(w1, w2)
+                return self.mk_mod(ex, w1, w2)
         elif op == EVM.SDIV:
             if is_bv_value(w1) and is_bv_value(w2):
-                return w1 / w2 # bvsdiv
+                return w1 / w2  # bvsdiv
             else:
                 return f_sdiv(w1, w2)
         elif op == EVM.SMOD:
             if is_bv_value(w1) and is_bv_value(w2):
-                return SRem(w1, w2) # bvsrem  # vs: w1 % w2 (bvsmod w1 w2)
+                return SRem(w1, w2)  # bvsrem  # vs: w1 % w2 (bvsmod w1 w2)
             else:
                 return f_smod(w1, w2)
         elif op == EVM.EXP:
             if is_bv_value(w1) and is_bv_value(w2):
-                i1: int = int(str(w1)) # must be concrete
-                i2: int = int(str(w2)) # must be concrete
-                return con(i1 ** i2)
+                i1: int = int(str(w1))  # must be concrete
+                i2: int = int(str(w2))  # must be concrete
+                return con(i1**i2)
             elif is_bv_value(w2):
                 i2: int = int(str(w2))
                 if i2 == 0:
                     return con(1)
                 elif i2 == 1:
                     return w1
-                elif i2 <= self.options.get('expByConst'):
+                elif i2 <= self.options.get("expByConst"):
                     exp = w1
                     for _ in range(i2 - 1):
                         exp = exp * w1
                     return exp
                 else:
                     return f_exp(w1, w2)
             else:
                 return f_exp(w1, w2)
         else:
             raise ValueError(op)
 
-    def call(self, ex: Exec, op: int, stack: List[Tuple[Exec,int]], step_id: int, out: List[Exec]) -> None:
+    def arith2(self, ex: Exec, op: int, w1: Word, w2: Word, w3: Word) -> Word:
+        w1 = b2i(w1)
+        w2 = b2i(w2)
+        w3 = b2i(w3)
+        if op == EVM.ADDMOD:
+            # to avoid add overflow; and to be a multiple of 8-bit
+            r1 = self.arith(
+                ex, EVM.ADD, simplify(ZeroExt(8, w1)), simplify(ZeroExt(8, w2))
+            )
+            r2 = self.arith(ex, EVM.MOD, simplify(r1), simplify(ZeroExt(8, w3)))
+            if r1.size() != 264:
+                raise ValueError(r1)
+            if r2.size() != 264:
+                raise ValueError(r2)
+            return Extract(255, 0, r2)
+        elif op == EVM.MULMOD:
+            # to avoid mul overflow
+            r1 = self.arith(
+                ex, EVM.MUL, simplify(ZeroExt(256, w1)), simplify(ZeroExt(256, w2))
+            )
+            r2 = self.arith(ex, EVM.MOD, simplify(r1), simplify(ZeroExt(256, w3)))
+            if r1.size() != 512:
+                raise ValueError(r1)
+            if r2.size() != 512:
+                raise ValueError(r2)
+            return Extract(255, 0, r2)
+        else:
+            raise ValueError(op)
+
+    def call(
+        self,
+        ex: Exec,
+        op: int,
+        stack: List[Tuple[Exec, int]],
+        step_id: int,
+        out: List[Exec],
+        bounded_loops: List[str],
+    ) -> None:
         gas = ex.st.pop()
-        to = ex.st.pop()
+
+        to = uint160(ex.st.pop())
+
         if op == EVM.STATICCALL:
             fund = con(0)
         else:
             fund = ex.st.pop()
         arg_loc: int = ex.st.mloc()
-        arg_size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
+        # size (in bytes)
+        arg_size: int = int_of(ex.st.pop(), "symbolic CALL input data size")
         ret_loc: int = ex.st.mloc()
-        ret_size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
+        # size (in bytes)
+        ret_size: int = int_of(ex.st.pop(), "symbolic CALL return data size")
 
-        if not arg_size >= 0: raise ValueError(arg_size)
-        if not ret_size >= 0: raise ValueError(ret_size)
+        if not arg_size >= 0:
+            raise ValueError(arg_size)
+        if not ret_size >= 0:
+            raise ValueError(ret_size)
 
         caller = ex.prank.lookup(ex.this, to)
 
+        orig_code = ex.code.copy()
+        orig_storage = deepcopy(ex.storage)
+        orig_balance = deepcopy(ex.balance)
+        orig_log = deepcopy(ex.log)
+
         if not (is_bv_value(fund) and fund.as_long() == 0):
-            ex.balance_update(caller, self.arith(EVM.SUB, ex.balance_of(caller), fund))
-            ex.balance_update(to,     self.arith(EVM.ADD, ex.balance_of(to),     fund))
+            ex.balance_update(
+                caller, self.arith(ex, EVM.SUB, ex.balance_of(caller), fund)
+            )
+            ex.balance_update(to, self.arith(ex, EVM.ADD, ex.balance_of(to), fund))
 
         def call_known() -> None:
             calldata = [None] * arg_size
             wextend(ex.st.memory, arg_loc, arg_size)
-            wstore_bytes(calldata, 0, arg_size, ex.st.memory[arg_loc:arg_loc+arg_size])
+            wstore_bytes(
+                calldata, 0, arg_size, ex.st.memory[arg_loc : arg_loc + arg_size]
+            )
 
             # execute external calls
-            (new_exs, new_steps) = self.run(Exec(
-                pgm       = ex.pgm,
-                code      = ex.code,
-                storage   = ex.storage,
-                balance   = ex.balance,
-                #
-                block     = ex.block,
-                #
-                calldata  = calldata,
-                callvalue = fund,
-                caller    = caller,
-                this      = to,
-                #
-                pc        = 0,
-                st        = State(),
-                jumpis    = {},
-                output    = None,
-                symbolic  = ex.symbolic,
-                prank     = Prank(),
-                #
-                solver    = ex.solver,
-                path      = ex.path,
-                #
-                log       = ex.log,
-                cnts      = ex.cnts,
-                sha3s     = ex.sha3s,
-                storages  = ex.storages,
-                balances  = ex.balances,
-                calls     = ex.calls,
-                failed    = ex.failed,
-                error     = ex.error,
-            ))
+            (new_exs, new_steps, new_bounded_loops) = self.run(
+                Exec(
+                    code=ex.code,
+                    storage=ex.storage,
+                    balance=ex.balance,
+                    #
+                    block=ex.block,
+                    #
+                    calldata=calldata,
+                    callvalue=fund,
+                    caller=caller,
+                    this=to,
+                    #
+                    pc=0,
+                    st=State(),
+                    jumpis={},
+                    output=None,
+                    symbolic=ex.symbolic,
+                    prank=Prank(),
+                    #
+                    solver=ex.solver,
+                    path=ex.path,
+                    #
+                    log=ex.log,
+                    cnts=ex.cnts,
+                    sha3s=ex.sha3s,
+                    storages=ex.storages,
+                    balances=ex.balances,
+                    calls=ex.calls,
+                    failed=ex.failed,
+                    error=ex.error,
+                )
+            )
+
+            bounded_loops.extend(new_bounded_loops)
 
             # process result
             for idx, new_ex in enumerate(new_exs):
-                opcode = new_ex.pgm[new_ex.this][new_ex.pc].op[0]
+                opcode = new_ex.current_opcode()
 
                 # restore tx msg
-                new_ex.calldata  = ex.calldata
+                new_ex.calldata = ex.calldata
                 new_ex.callvalue = ex.callvalue
-                new_ex.caller    = ex.caller
-                new_ex.this      = ex.this
+                new_ex.caller = ex.caller
+                new_ex.this = ex.this
 
                 # restore vm state
                 new_ex.pc = ex.pc
                 new_ex.st = deepcopy(ex.st)
                 new_ex.jumpis = deepcopy(ex.jumpis)
                 # new_ex.output is passed into the caller
                 new_ex.symbolic = ex.symbolic
                 new_ex.prank = ex.prank
 
                 # set return data (in memory)
-                wstore_partial(new_ex.st.memory, ret_loc, 0, min(ret_size, new_ex.returndatasize()), new_ex.output, new_ex.returndatasize())
+                actual_ret_size = new_ex.returndatasize()
+                wstore_partial(
+                    new_ex.st.memory,
+                    ret_loc,
+                    0,
+                    min(ret_size, actual_ret_size),
+                    new_ex.output,
+                    actual_ret_size,
+                )
 
                 # set status code (in stack)
-                if is_bv_value(opcode) and opcode.as_long() in [EVM.STOP, EVM.RETURN, EVM.REVERT, EVM.INVALID]:
-                    if opcode.as_long() in [EVM.STOP, EVM.RETURN]:
+                if opcode in [EVM.STOP, EVM.RETURN, EVM.REVERT, EVM.INVALID]:
+                    if opcode in [EVM.STOP, EVM.RETURN]:
                         new_ex.st.push(con(1))
                     else:
                         new_ex.st.push(con(0))
 
+                        # revert network states
+                        new_ex.code = orig_code
+                        new_ex.storage = orig_storage
+                        new_ex.balance = orig_balance
+                        new_ex.log = orig_log
+
                     # add to worklist even if it reverted during the external call
                     new_ex.next_pc()
                     stack.append((new_ex, step_id))
                 else:
                     # got stuck during external call
-                    new_ex.error = f'external call stuck: {mnemonic(opcode)}'
+                    new_ex.error = f"External call encountered an issue at {mnemonic(opcode)}: {new_ex.error}"
                     out.append(new_ex)
 
         def call_unknown() -> None:
+            call_id = len(ex.calls)
+
             # push exit code
             if arg_size > 0:
                 arg = wload(ex.st.memory, arg_loc, arg_size)
-                f_call = Function('call_'+str(arg_size*8), BitVecSort(256), BitVecSort(256), BitVecSort(256), BitVecSort(256), BitVecSort(arg_size*8), BitVecSort(256))
-                exit_code = f_call(con(ex.cnt_call()), gas, to, fund, arg)
+                f_call = Function(
+                    "call_" + str(arg_size * 8),
+                    BitVecSort(256),  # cnt
+                    BitVecSort(256),  # gas
+                    BitVecSort(160),  # to
+                    BitVecSort(256),  # value
+                    BitVecSort(arg_size * 8),  # args
+                    BitVecSort(256),
+                )
+                exit_code = f_call(con(call_id), gas, to, fund, arg)
             else:
-                f_call = Function('call_'+str(arg_size*8), BitVecSort(256), BitVecSort(256), BitVecSort(256), BitVecSort(256),                         BitVecSort(256))
-                exit_code = f_call(con(ex.cnt_call()), gas, to, fund)
-            exit_code_var = BitVec(f'call{ex.cnt_call()}', 256)
+                f_call = Function(
+                    "call_" + str(arg_size * 8),
+                    BitVecSort(256),  # cnt
+                    BitVecSort(256),  # gas
+                    BitVecSort(160),  # to
+                    BitVecSort(256),  # value
+                    BitVecSort(256),
+                )
+                exit_code = f_call(con(call_id), gas, to, fund)
+            exit_code_var = BitVec(f"call_exit_code_{call_id:>02}", 256)
             ex.solver.add(exit_code_var == exit_code)
             ex.st.push(exit_code_var)
 
             ret = None
-            if ret_size > 0: # TODO: handle inconsistent return sizes for unknown functions
-                f_ret = Function('ret_'+str(ret_size*8), BitVecSort(256), BitVecSort(ret_size*8))
+            # TODO: handle inconsistent return sizes for unknown functions
+            if ret_size > 0:
+                f_ret = Function(
+                    "ret_" + str(ret_size * 8),
+                    BitVecSort(256),
+                    BitVecSort(ret_size * 8),
+                )
                 ret = f_ret(exit_code_var)
 
             # TODO: cover other precompiled
-            if to == con(1): # ecrecover exit code is always 1
+            if eq(to, con_addr(1)):  # ecrecover exit code is always 1
+                ex.solver.add(exit_code_var != con(0))
+
+            # halmos cheat code
+            if eq(to, halmos_cheat_code.address):
                 ex.solver.add(exit_code_var != con(0))
 
+                funsig: int = int_of(
+                    extract_funsig(arg), "symbolic halmos cheatcode function selector"
+                )
+
+                # createUint(uint256,string) returns (uint256)
+                if funsig == halmos_cheat_code.create_uint:
+                    bit_size = int_of(
+                        extract_bytes(arg, 4, 32),
+                        "symbolic bit size for halmos.createUint()",
+                    )
+                    label = name_of(extract_string_argument(arg, 1))
+                    if bit_size <= 256:
+                        ret = uint256(
+                            BitVec(
+                                f"halmos_{label}_uint{bit_size}_{ex.new_symbol_id():>02}",
+                                bit_size,
+                            )
+                        )
+                    else:
+                        ex.error = f"bitsize larger than 256: {bit_size}"
+                        out.append(ex)
+                        return
+
+                # createBytes(uint256,string) returns (bytes)
+                elif funsig == halmos_cheat_code.create_bytes:
+                    byte_size = int_of(
+                        extract_bytes(arg, 4, 32),
+                        "symbolic byte size for halmos.createBytes()",
+                    )
+                    label = name_of(extract_string_argument(arg, 1))
+                    symbolic_bytes = BitVec(
+                        f"halmos_{label}_bytes_{ex.new_symbol_id():>02}", byte_size * 8
+                    )
+                    ret = Concat(
+                        BitVecVal(32, 256), BitVecVal(byte_size, 256), symbolic_bytes
+                    )
+
+                # createUint256(string) returns (uint256)
+                elif funsig == halmos_cheat_code.create_uint256:
+                    label = name_of(extract_string_argument(arg, 0))
+                    ret = BitVec(
+                        f"halmos_{label}_uint256_{ex.new_symbol_id():>02}", 256
+                    )
+
+                # createBytes32(string) returns (bytes32)
+                elif funsig == halmos_cheat_code.create_bytes32:
+                    label = name_of(extract_string_argument(arg, 0))
+                    ret = BitVec(
+                        f"halmos_{label}_bytes32_{ex.new_symbol_id():>02}", 256
+                    )
+
+                # createAddress(string) returns (address)
+                elif funsig == halmos_cheat_code.create_address:
+                    label = name_of(extract_string_argument(arg, 0))
+                    ret = uint256(
+                        BitVec(f"halmos_{label}_address_{ex.new_symbol_id():>02}", 160)
+                    )
+
+                # createBool(string) returns (bool)
+                elif funsig == halmos_cheat_code.create_bool:
+                    label = name_of(extract_string_argument(arg, 0))
+                    ret = uint256(
+                        BitVec(f"halmos_{label}_bool_{ex.new_symbol_id():>02}", 1)
+                    )
+
+                else:
+                    ex.error = f"Unknown halmos cheat code: function selector = 0x{funsig:0>8x}, calldata = {hexify(arg)}"
+                    out.append(ex)
+                    return
+
             # vm cheat code
-            if to == con(hevm_cheat_code.address):
+            if eq(to, hevm_cheat_code.address):
                 ex.solver.add(exit_code_var != con(0))
                 # vm.fail()
-                if arg == hevm_cheat_code.fail_payload: # BitVecVal(hevm_cheat_code.fail_payload, 800)
+                # BitVecVal(hevm_cheat_code.fail_payload, 800)
+                if arg == hevm_cheat_code.fail_payload:
                     ex.failed = True
+                    out.append(ex)
+                    return
                 # vm.assume(bool)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.assume_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.assume_sig
+                ):
                     assume_cond = simplify(is_non_zero(Extract(255, 0, arg)))
                     ex.solver.add(assume_cond)
                     ex.path.append(str(assume_cond))
                 # vm.getCode(string)
-                elif simplify(Extract(arg_size*8-1, arg_size*8-32, arg)) == hevm_cheat_code.get_code_sig:
+                elif (
+                    simplify(Extract(arg_size * 8 - 1, arg_size * 8 - 32, arg))
+                    == hevm_cheat_code.get_code_sig
+                ):
                     calldata = bytes.fromhex(hex(arg.as_long())[2:])
-                    path_len = int.from_bytes(calldata[36:68], 'big')
-                    path = calldata[68:68+path_len].decode('utf-8')
+                    path_len = int.from_bytes(calldata[36:68], "big")
+                    path = calldata[68 : 68 + path_len].decode("utf-8")
+
+                    if ":" in path:
+                        [filename, contract_name] = path.split(":")
+                        path = "out/" + filename + "/" + contract_name + ".json"
+
+                    target = self.options["target"].rstrip("/")
+                    path = target + "/" + path
 
-                    if ':' in path:
-                        [filename, contract_name] = path.split(':')
-                        path = 'out/' + filename + '/' + contract_name + '.json'
-
-                    target = self.options['target'].rstrip('/')
-                    path = target + '/' + path
-                    
                     with open(path) as f:
                         artifact = json.loads(f.read())
-                    
-                    if artifact['bytecode']['object']:
-                        bytecode = artifact['bytecode']['object'].replace('0x', '')
+
+                    if artifact["bytecode"]["object"]:
+                        bytecode = artifact["bytecode"]["object"].replace("0x", "")
                     else:
-                        bytecode = artifact['bytecode'].replace('0x', '')
+                        bytecode = artifact["bytecode"].replace("0x", "")
 
                     bytecode_len = (len(bytecode) + 1) // 2
-                    bytecode_len_enc = hex(bytecode_len).replace('0x', '').rjust(64, '0')
+                    bytecode_len_enc = (
+                        hex(bytecode_len).replace("0x", "").rjust(64, "0")
+                    )
 
                     bytecode_len_ceil = (bytecode_len + 31) // 32 * 32
 
-                    ret_bytes = '00' * 31 + '20' + bytecode_len_enc + bytecode.ljust(bytecode_len_ceil*2, '0')
+                    ret_bytes = (
+                        "00" * 31
+                        + "20"
+                        + bytecode_len_enc
+                        + bytecode.ljust(bytecode_len_ceil * 2, "0")
+                    )
                     ret_len = len(ret_bytes) // 2
                     ret_bytes = bytes.fromhex(ret_bytes)
 
-                    ret = BitVecVal(int.from_bytes(ret_bytes, 'big'), ret_len * 8)
+                    ret = BitVecVal(int.from_bytes(ret_bytes, "big"), ret_len * 8)
                 # vm.prank(address)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.prank_sig:
-                    result = ex.prank.prank(simplify(Extract(255, 0, arg)))
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.prank_sig
+                ):
+                    result = ex.prank.prank(uint160(Extract(255, 0, arg)))
                     if not result:
-                        ex.error = 'You have an active prank already.'
+                        ex.error = "You have an active prank already."
                         out.append(ex)
                         return
                 # vm.startPrank(address)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.start_prank_sig:
-                    result = ex.prank.startPrank(simplify(Extract(255, 0, arg)))
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg))
+                    == hevm_cheat_code.start_prank_sig
+                ):
+                    result = ex.prank.startPrank(uint160(Extract(255, 0, arg)))
                     if not result:
-                        ex.error = 'You have an active prank already.'
+                        ex.error = "You have an active prank already."
                         out.append(ex)
                         return
                 # vm.stopPrank()
-                elif eq(arg.sort(), BitVecSort((4)*8)) and simplify(Extract(31, 0, arg)) == hevm_cheat_code.stop_prank_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4) * 8))
+                    and simplify(Extract(31, 0, arg)) == hevm_cheat_code.stop_prank_sig
+                ):
                     ex.prank.stopPrank()
                 # vm.deal(address,uint256)
-                elif eq(arg.sort(), BitVecSort((4+32*2)*8)) and simplify(Extract(543, 512, arg)) == hevm_cheat_code.deal_sig:
-                    who = simplify(Extract(511, 256, arg))
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32 * 2) * 8))
+                    and simplify(Extract(543, 512, arg)) == hevm_cheat_code.deal_sig
+                ):
+                    who = uint160(Extract(511, 256, arg))
                     amount = simplify(Extract(255, 0, arg))
                     ex.balance_update(who, amount)
+                # vm.store(address,bytes32,bytes32)
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32 * 3) * 8))
+                    and simplify(Extract(799, 768, arg)) == hevm_cheat_code.store_sig
+                ):
+                    store_account = uint160(Extract(767, 512, arg))
+                    store_slot = simplify(Extract(511, 256, arg))
+                    store_value = simplify(Extract(255, 0, arg))
+                    if store_account in ex.storage:
+                        ex.sstore(store_account, store_slot, store_value)
+                    else:
+                        ex.error = f"uninitialized account: {store_account}"
+                        out.append(ex)
+                        return
+                # vm.load(address,bytes32)
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32 * 2) * 8))
+                    and simplify(Extract(543, 512, arg)) == hevm_cheat_code.load_sig
+                ):
+                    load_account = uint160(Extract(511, 256, arg))
+                    load_slot = simplify(Extract(255, 0, arg))
+                    if load_account in ex.storage:
+                        ret = ex.sload(load_account, load_slot)
+                    else:
+                        ex.error = f"uninitialized account: {load_account}"
+                        out.append(ex)
+                        return
                 # vm.fee(uint256)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.fee_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.fee_sig
+                ):
                     ex.block.basefee = simplify(Extract(255, 0, arg))
                 # vm.chainId(uint256)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.chainid_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.chainid_sig
+                ):
                     ex.block.chainid = simplify(Extract(255, 0, arg))
                 # vm.coinbase(address)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.coinbase_sig:
-                    ex.block.coinbase = simplify(Extract(255, 0, arg))
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.coinbase_sig
+                ):
+                    ex.block.coinbase = uint160(Extract(255, 0, arg))
                 # vm.difficulty(uint256)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.difficulty_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg))
+                    == hevm_cheat_code.difficulty_sig
+                ):
                     ex.block.difficulty = simplify(Extract(255, 0, arg))
                 # vm.roll(uint256)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.roll_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.roll_sig
+                ):
                     ex.block.number = simplify(Extract(255, 0, arg))
                 # vm.warp(uint256)
-                elif eq(arg.sort(), BitVecSort((4+32)*8)) and simplify(Extract(287, 256, arg)) == hevm_cheat_code.warp_sig:
+                elif (
+                    eq(arg.sort(), BitVecSort((4 + 32) * 8))
+                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.warp_sig
+                ):
                     ex.block.timestamp = simplify(Extract(255, 0, arg))
+                # vm.etch(address,bytes)
+                elif extract_funsig(arg) == hevm_cheat_code.etch_sig:
+                    who = extract_bytes(arg, 4 + 12, 20)
+
+                    # who must be concrete
+                    if not is_bv_value(who):
+                        ex.error = f"vm.etch(address who, bytes code) must have concrete argument `who` but received {who}"
+                        out.append(ex)
+                        return
+
+                    # code must be concrete
+                    try:
+                        code_offset = int_of(extract_bytes(arg, 4 + 32, 32))
+                        code_length = int_of(extract_bytes(arg, 4 + code_offset, 32))
+                        code_int = int_of(
+                            extract_bytes(arg, 4 + code_offset + 32, code_length)
+                        )
+                        code_bytes = code_int.to_bytes(code_length, "big")
+
+                        ex.code[who] = Contract(code_bytes)
+                    except Exception as e:
+                        ex.error = f"vm.etch(address who, bytes code) must have concrete argument `code` but received calldata {arg}"
+                        out.append(ex)
+                        return
+
                 else:
                     # TODO: support other cheat codes
-                    ex.error = str('Unsupported cheat code: calldata: ' + str(arg))
+                    ex.error = f"Unsupported cheat code: calldata = {hexify(arg)}"
+                    out.append(ex)
+                    return
+
+            # console
+            if eq(to, console.address):
+                ex.solver.add(exit_code_var != con(0))
+
+                funsig: int = int_of(
+                    extract_funsig(arg), "symbolic console function selector"
+                )
+
+                if funsig == console.log_uint:
+                    print(extract_bytes(arg, 4, 32))
+
+                # elif funsig == console.log_string:
+
+                else:
+                    # TODO: support other console functions
+                    ex.error = f"Unsupported console function: function selector = 0x{funsig:0>8x}, calldata = {hexify(arg)}"
                     out.append(ex)
                     return
 
             # store return value
             if ret_size > 0:
                 wstore(ex.st.memory, ret_loc, ret_size, ret)
 
@@ -881,261 +1700,320 @@
 
             ex.calls.append((exit_code_var, exit_code, ex.output))
 
             ex.next_pc()
             stack.append((ex, step_id))
 
         # separately handle known / unknown external calls
-        if to in ex.pgm:
+
+        # TODO: avoid relying directly on dict membership here
+        # it is based on hashing of the z3 expr objects rather than equivalence
+        if to in ex.code:
             call_known()
         else:
             call_unknown()
 
-    def create(self, ex: Exec, stack: List[Tuple[Exec,int]], step_id: int, out: List[Exec]) -> None:
+    def create(
+        self,
+        ex: Exec,
+        stack: List[Tuple[Exec, int]],
+        step_id: int,
+        out: List[Exec],
+        bounded_loops: List[str],
+    ) -> None:
         value: Word = ex.st.pop()
-        loc: int = int(str(ex.st.pop()))
-        size: int = int(str(ex.st.pop()))
+        loc: int = int_of(ex.st.pop(), "symbolic CREATE offset")
+        size: int = int_of(ex.st.pop(), "symbolic CREATE size")
 
         # contract creation code
-        create_hexcode = wload(ex.st.memory, loc, size)
-        (create_ops, create_code) = decode(create_hexcode)
-        create_pgm = ops_to_pgm(create_ops)
+        create_hexcode = wload(ex.st.memory, loc, size, prefer_concrete=True)
+        create_code = Contract(create_hexcode)
 
         # new account address
-        new_addr = create_address(ex.cnt_create())
-        for addr in ex.pgm:
-            ex.solver.add(new_addr != addr) # ensure new address is fresh
+        new_addr = ex.new_address()
+
+        for addr in ex.code:
+            ex.solver.add(new_addr != addr)  # ensure new address is fresh
 
         # setup new account
-        ex.pgm[new_addr] = create_pgm   # existing pgm must be empty
-        ex.code[new_addr] = create_code # existing code must be empty
-        ex.storage[new_addr] = {}       # existing storage may not be empty and reset here
+        ex.code[new_addr] = create_code  # existing code must be empty
+        ex.storage[new_addr] = {}  # existing storage may not be empty and reset here
 
         # lookup prank
         caller = ex.prank.lookup(ex.this, new_addr)
 
         # transfer value
-        ex.solver.add(UGE(ex.balance_of(caller), value)) # assume balance is enough; otherwise ignore this path
+        # assume balance is enough; otherwise ignore this path
+        ex.solver.add(UGE(ex.balance_of(caller), value))
         if not (is_bv_value(value) and value.as_long() == 0):
-            ex.balance_update(caller,   self.arith(EVM.SUB, ex.balance_of(caller),   value))
-            ex.balance_update(new_addr, self.arith(EVM.ADD, ex.balance_of(new_addr), value))
+            ex.balance_update(
+                caller, self.arith(ex, EVM.SUB, ex.balance_of(caller), value)
+            )
+            ex.balance_update(
+                new_addr, self.arith(ex, EVM.ADD, ex.balance_of(new_addr), value)
+            )
 
         # execute contract creation code
-        (new_exs, new_steps) = self.run(Exec(
-            pgm       = ex.pgm,
-            code      = ex.code,
-            storage   = ex.storage,
-            balance   = ex.balance,
-            #
-            block     = ex.block,
-            #
-            calldata  = [],
-            callvalue = value,
-            caller    = ex.this,
-            this      = new_addr,
-            #
-            pc        = 0,
-            st        = State(),
-            jumpis    = {},
-            output    = None,
-            symbolic  = False,
-            prank     = Prank(),
-            #
-            solver    = ex.solver,
-            path      = ex.path,
-            #
-            log       = ex.log,
-            cnts      = ex.cnts,
-            sha3s     = ex.sha3s,
-            storages  = ex.storages,
-            balances  = ex.balances,
-            calls     = ex.calls,
-            failed    = ex.failed,
-            error     = ex.error,
-        ))
+        (new_exs, new_steps, new_bounded_loops) = self.run(
+            Exec(
+                code=ex.code,
+                storage=ex.storage,
+                balance=ex.balance,
+                #
+                block=ex.block,
+                #
+                calldata=[],
+                callvalue=value,
+                caller=caller,
+                this=new_addr,
+                #
+                pc=0,
+                st=State(),
+                jumpis={},
+                output=None,
+                symbolic=False,
+                prank=Prank(),
+                #
+                solver=ex.solver,
+                path=ex.path,
+                #
+                log=ex.log,
+                cnts=ex.cnts,
+                sha3s=ex.sha3s,
+                storages=ex.storages,
+                balances=ex.balances,
+                calls=ex.calls,
+                failed=ex.failed,
+                error=ex.error,
+            )
+        )
+
+        bounded_loops.extend(new_bounded_loops)
 
         # process result
         for idx, new_ex in enumerate(new_exs):
             # sanity checks
-            if new_ex.failed: raise ValueError(new_ex)
+            if new_ex.failed:
+                raise ValueError(new_ex)
 
-            opcode = new_ex.pgm[new_ex.this][new_ex.pc].op[0]
-            if is_bv_value(opcode) and opcode.as_long() in [EVM.STOP, EVM.RETURN]:
+            opcode = new_ex.current_opcode()
+            if opcode in [EVM.STOP, EVM.RETURN]:
                 # new contract code
-                new_hexcode = new_ex.output
-                (new_ops, new_code) = decode(new_hexcode)
-                new_pgm = ops_to_pgm(new_ops)
-
-                # set new contract code
-                new_ex.pgm[new_addr] = new_pgm
-                new_ex.code[new_addr] = new_code
+                new_ex.code[new_addr] = Contract(new_ex.output)
 
                 # restore tx msg
-                new_ex.calldata  = ex.calldata
+                new_ex.calldata = ex.calldata
                 new_ex.callvalue = ex.callvalue
-                new_ex.caller    = ex.caller
-                new_ex.this      = ex.this
+                new_ex.caller = ex.caller
+                new_ex.this = ex.this
 
                 # restore vm state
                 new_ex.pc = ex.pc
                 new_ex.st = deepcopy(ex.st)
                 new_ex.jumpis = deepcopy(ex.jumpis)
-                new_ex.output = None # output is reset, not restored
+                new_ex.output = None  # output is reset, not restored
                 new_ex.symbolic = ex.symbolic
                 new_ex.prank = ex.prank
 
                 # push new address to stack
-                new_ex.st.push(new_addr)
+                new_ex.st.push(uint256(new_addr))
 
                 # add to worklist
                 new_ex.next_pc()
                 stack.append((new_ex, step_id))
             else:
                 # creation failed
                 out.append(new_ex)
 
-    def jumpi(self, ex: Exec, stack: List[Tuple[Exec,int]], step_id: int) -> None:
+    def jumpi(
+        self,
+        ex: Exec,
+        stack: List[Tuple[Exec, int]],
+        step_id: int,
+        bounded_loops: List[str],
+    ) -> None:
         jid = ex.jumpi_id()
 
         source: int = ex.pc
-        target: int = int(str(ex.st.pop())) # target must be concrete
+        target: int = int_of(ex.st.pop(), "symbolic JUMPI target")
         cond: Word = ex.st.pop()
 
         visited = ex.jumpis.get(jid, {True: 0, False: 0})
 
+        cond_true = simplify(is_non_zero(cond))
+        cond_false = simplify(is_zero(cond))
+
+        potential_true: bool = ex.check(cond_true) != unsat
+        potential_false: bool = ex.check(cond_false) != unsat
+
+        # note: both may be false if the previous path condition was considered unknown but turns out to be unsat later
+
+        follow_true = False
+        follow_false = False
+
+        if potential_true and potential_false:
+            # for loop unrolling
+            follow_true = visited[True] < self.options["max_loop"]
+            follow_false = visited[False] < self.options["max_loop"]
+            if not (follow_true and follow_false):
+                bounded_loops.append(jid)
+        else:
+            # for constant-bounded loops
+            follow_true = potential_true
+            follow_false = potential_false
+
         new_ex_true = None
         new_ex_false = None
 
-        ex.solver.push()
-        cond_true = simplify(is_non_zero(cond))
-        ex.solver.add(cond_true)
-        if ex.solver.check() != unsat: # jump
-            new_ex_true = self.create_branch(ex, str(cond_true), target)
-        ex.solver.pop()
+        if follow_true:
+            if follow_false:
+                new_ex_true = self.create_branch(ex, cond_true, target)
+            else:
+                new_ex_true = ex
+                new_ex_true.solver.add(cond_true)
+                new_ex_true.path.append(str(cond_true))
+                new_ex_true.pc = target
 
-        cond_false = simplify(is_zero(cond))
-        ex.solver.add(cond_false)
-        if ex.solver.check() != unsat:
-            ex.path.append(str(cond_false))
-            ex.next_pc()
+        if follow_false:
             new_ex_false = ex
-
-        if new_ex_true and new_ex_false: # for loop unrolling
-            if visited[True] < self.options['max_loop']: # or source < target:
-                new_ex_true.jumpis[jid] = {True: visited[True] + 1, False: visited[False]}
-                stack.append((new_ex_true, step_id))
-            if visited[False] < self.options['max_loop']: # or source < target:
-                new_ex_false.jumpis[jid] = {True: visited[True], False: visited[False] + 1}
-                stack.append((new_ex_false, step_id))
-        elif new_ex_true: # for constant-bounded loops
+            new_ex_false.solver.add(cond_false)
+            new_ex_false.path.append(str(cond_false))
+            new_ex_false.next_pc()
+
+        if new_ex_true:
+            if potential_true and potential_false:
+                new_ex_true.jumpis[jid] = {
+                    True: visited[True] + 1,
+                    False: visited[False],
+                }
             stack.append((new_ex_true, step_id))
-        elif new_ex_false:
+
+        if new_ex_false:
+            if potential_true and potential_false:
+                new_ex_false.jumpis[jid] = {
+                    True: visited[True],
+                    False: visited[False] + 1,
+                }
             stack.append((new_ex_false, step_id))
-        else:
-            pass # this may happen if the previous path condition was considered unknown but turns out to be unsat later
 
-    def jump(self, ex: Exec, stack: List[Tuple[Exec,int]], step_id: int) -> None:
+    def jump(self, ex: Exec, stack: List[Tuple[Exec, int]], step_id: int) -> None:
         dst = ex.st.pop()
 
         # if dst is concrete, just jump
-        if is_bv_value(dst):
-            ex.pc = int(str(dst))
+        if is_concrete(dst):
+            ex.pc = int_of(dst)
             stack.append((ex, step_id))
 
         # otherwise, create a new execution for feasible targets
-        elif self.options['sym_jump']:
-            for target in valid_jump_destinations(ex.pgm[ex.this]):
-                ex.solver.push()
+        elif self.options["sym_jump"]:
+            for target in ex.code[ex.this].valid_jump_destinations():
                 target_reachable = simplify(dst == target)
-                ex.solver.add(target_reachable)
-                if ex.solver.check() != unsat: # jump
-                    if self.options.get('debug'):
-                        print(f'we can jump to {target} with model {ex.solver.model()}')
-                    new_ex = self.create_branch(ex, str(target_reachable), target)
+                if ex.check(target_reachable) != unsat:  # jump
+                    if self.options.get("debug"):
+                        print(f"We can jump to {target} with model {ex.solver.model()}")
+                    new_ex = self.create_branch(ex, target_reachable, target)
                     stack.append((new_ex, step_id))
-                ex.solver.pop()
-
         else:
-            raise ValueError(dst)
+            raise NotConcreteError(f"symbolic JUMP target: {dst}")
 
-    def create_branch(self, ex: Exec, cond: str, target: int) -> Exec:
-        new_solver = SolverFor('QF_AUFBV')
-        new_solver.set(timeout=self.options['timeout'])
+    def create_branch(self, ex: Exec, cond: BitVecRef, target: int) -> Exec:
+        new_solver = SolverFor("QF_AUFBV")
+        new_solver.set(timeout=self.options["timeout"])
         new_solver.add(ex.solver.assertions())
+        new_solver.add(cond)
         new_path = deepcopy(ex.path)
-        new_path.append(cond)
+        new_path.append(str(cond))
         new_ex = Exec(
-            pgm      = ex.pgm.copy(), # shallow copy for potential new contract creation; existing code doesn't change
-            code     = ex.code.copy(), # shallow copy
-            storage  = deepcopy(ex.storage),
-            balance  = deepcopy(ex.balance),
+            code=ex.code.copy(),  # shallow copy for potential new contract creation; existing code doesn't change
+            storage=deepcopy(ex.storage),
+            balance=deepcopy(ex.balance),
             #
-            block    = deepcopy(ex.block),
+            block=deepcopy(ex.block),
             #
-            calldata = ex.calldata,
-            callvalue= ex.callvalue,
-            caller   = ex.caller,
-            this     = ex.this,
+            calldata=ex.calldata,
+            callvalue=ex.callvalue,
+            caller=ex.caller,
+            this=ex.this,
             #
-            pc       = target,
-            st       = deepcopy(ex.st),
-            jumpis   = deepcopy(ex.jumpis),
-            output   = deepcopy(ex.output),
-            symbolic = ex.symbolic,
-            prank    = deepcopy(ex.prank),
+            pc=target,
+            st=deepcopy(ex.st),
+            jumpis=deepcopy(ex.jumpis),
+            output=deepcopy(ex.output),
+            symbolic=ex.symbolic,
+            prank=deepcopy(ex.prank),
             #
-            solver   = new_solver,
-            path     = new_path,
+            solver=new_solver,
+            path=new_path,
             #
-            log      = deepcopy(ex.log),
-            cnts     = deepcopy(ex.cnts),
-            sha3s    = deepcopy(ex.sha3s),
-            storages = deepcopy(ex.storages),
-            balances = deepcopy(ex.balances),
-            calls    = deepcopy(ex.calls),
-            failed   = ex.failed,
-            error    = ex.error,
+            log=deepcopy(ex.log),
+            cnts=deepcopy(ex.cnts),
+            sha3s=deepcopy(ex.sha3s),
+            storages=deepcopy(ex.storages),
+            balances=deepcopy(ex.balances),
+            calls=deepcopy(ex.calls),
+            failed=ex.failed,
+            error=ex.error,
         )
         return new_ex
 
+    def sym_byte_of(self, idx: BitVecRef, w: BitVecRef) -> BitVecRef:
+        """generate symbolic BYTE opcode result using 32 nested ite"""
+
+        def gen_nested_ite(curr: int) -> BitVecRef:
+            if curr < 32:
+                return If(
+                    idx == con(curr),
+                    Extract((31 - curr) * 8 + 7, (31 - curr) * 8, w),
+                    gen_nested_ite(curr + 1),
+                )
+            else:
+                return con(0, 8)
+
+        # If(idx == 0, Extract(255, 248, w), If(idx == 1, Extract(247, 240, w), ..., If(idx == 31, Extract(7, 0, w), 0)...))
+        return ZeroExt(248, gen_nested_ite(0))
+
     def run(self, ex0: Exec) -> Tuple[List[Exec], Steps]:
         out: List[Exec] = []
+        bounded_loops: List[str] = []
         steps: Steps = {}
         step_id: int = 0
 
-        stack: List[Tuple[Exec,int]] = [(ex0, 0)]
+        stack: List[Tuple[Exec, int]] = [(ex0, 0)]
         while stack:
             try:
-                if 'max_width' in self.options and len(out) >= self.options['max_width']: break
+                if (
+                    "max_width" in self.options
+                    and len(out) >= self.options["max_width"]
+                ):
+                    break
 
                 (ex, prev_step_id) = stack.pop()
                 step_id += 1
 
-                o = ex.pgm[ex.this][ex.pc]
-                opcode = o.op[0]
-                if is_bv_value(opcode):
-                    opcode = int(str(opcode))
-                else:
-                    out.append(ex)
+                insn = ex.current_instruction()
+                opcode = insn.opcode
+                ex.cnts["opcode"][opcode] += 1
+
+                if (
+                    "max_depth" in self.options
+                    and sum(ex.cnts["opcode"].values()) > self.options["max_depth"]
+                ):
                     continue
-                ex.cnts[opcode] += 1
 
-                if 'max_depth' in self.options and sum(ex.cnts.values()) > self.options['max_depth']:
-                    continue
-
-                if self.options.get('log'):
+                if self.options.get("log"):
                     if opcode == EVM.JUMPI:
-                        steps[step_id] = {'parent': prev_step_id, 'exec': str(ex)}
-                #   elif opcode == EVM.CALL:
-                #       steps[step_id] = {'parent': prev_step_id, 'exec': str(ex) + ex.st.str_memory() + '\n'}
+                        steps[step_id] = {"parent": prev_step_id, "exec": str(ex)}
+                    # elif opcode == EVM.CALL:
+                    #     steps[step_id] = {'parent': prev_step_id, 'exec': str(ex) + ex.st.str_memory() + '\n'}
                     else:
-                    #   steps[step_id] = {'parent': prev_step_id, 'exec': ex.summary()}
-                        steps[step_id] = {'parent': prev_step_id, 'exec': str(ex)}
-                    if self.options.get('verbose', 0) >= 3:
-                        print(ex)
+                        # steps[step_id] = {'parent': prev_step_id, 'exec': ex.summary()}
+                        steps[step_id] = {"parent": prev_step_id, "exec": str(ex)}
+
+                if self.options.get("print_steps"):
+                    print(ex)
 
                 if opcode == EVM.STOP:
                     ex.output = None
                     out.append(ex)
                     continue
 
                 elif opcode == EVM.INVALID:
@@ -1150,140 +2028,150 @@
 
                 elif opcode == EVM.RETURN:
                     ex.output = ex.st.ret()
                     out.append(ex)
                     continue
 
                 elif opcode == EVM.JUMPI:
-                    self.jumpi(ex, stack, step_id)
+                    self.jumpi(ex, stack, step_id, bounded_loops)
                     continue
 
                 elif opcode == EVM.JUMP:
                     self.jump(ex, stack, step_id)
                     continue
 
                 elif opcode == EVM.JUMPDEST:
                     pass
 
-                elif EVM.ADD <= opcode <= EVM.SMOD: # ADD MUL SUB DIV SDIV MOD SMOD
-                    ex.st.push(self.arith(opcode, ex.st.pop(), ex.st.pop()))
+                elif EVM.ADD <= opcode <= EVM.SMOD:  # ADD MUL SUB DIV SDIV MOD SMOD
+                    ex.st.push(self.arith(ex, opcode, ex.st.pop(), ex.st.pop()))
+
+                elif EVM.ADDMOD <= opcode <= EVM.MULMOD:  # ADDMOD MULMOD
+                    ex.st.push(
+                        self.arith2(ex, opcode, ex.st.pop(), ex.st.pop(), ex.st.pop())
+                    )
 
                 elif opcode == EVM.EXP:
-                    ex.st.push(self.arith(opcode, ex.st.pop(), ex.st.pop()))
+                    ex.st.push(self.arith(ex, opcode, ex.st.pop(), ex.st.pop()))
 
                 elif opcode == EVM.LT:
                     w1 = b2i(ex.st.pop())
                     w2 = b2i(ex.st.pop())
-                    ex.st.push(ULT(w1, w2)) # bvult
+                    ex.st.push(ULT(w1, w2))  # bvult
                 elif opcode == EVM.GT:
                     w1 = b2i(ex.st.pop())
                     w2 = b2i(ex.st.pop())
-                    ex.st.push(UGT(w1, w2)) # bvugt
+                    ex.st.push(UGT(w1, w2))  # bvugt
                 elif opcode == EVM.SLT:
                     w1 = b2i(ex.st.pop())
                     w2 = b2i(ex.st.pop())
-                    ex.st.push(w1 < w2) # bvslt
+                    ex.st.push(w1 < w2)  # bvslt
                 elif opcode == EVM.SGT:
                     w1 = b2i(ex.st.pop())
                     w2 = b2i(ex.st.pop())
-                    ex.st.push(w1 > w2) # bvsgt
+                    ex.st.push(w1 > w2)  # bvsgt
 
                 elif opcode == EVM.EQ:
                     w1 = ex.st.pop()
                     w2 = ex.st.pop()
                     if eq(w1.sort(), w2.sort()):
                         ex.st.push(w1 == w2)
                     else:
                         if is_bool(w1):
-                            if not is_bv(w2): raise ValueError(w2)
+                            if not is_bv(w2):
+                                raise ValueError(w2)
                             ex.st.push(If(w1, con(1), con(0)) == w2)
                         else:
-                            if not is_bv(w1): raise ValueError(w1)
-                            if not is_bool(w2): raise ValueError(w2)
+                            if not is_bv(w1):
+                                raise ValueError(w1)
+                            if not is_bool(w2):
+                                raise ValueError(w2)
                             ex.st.push(w1 == If(w2, con(1), con(0)))
                 elif opcode == EVM.ISZERO:
                     ex.st.push(is_zero(ex.st.pop()))
 
                 elif opcode == EVM.AND:
                     ex.st.push(and_of(ex.st.pop(), ex.st.pop()))
                 elif opcode == EVM.OR:
                     ex.st.push(or_of(ex.st.pop(), ex.st.pop()))
                 elif opcode == EVM.NOT:
-                    ex.st.push(~ ex.st.pop()) # bvnot
+                    ex.st.push(~ex.st.pop())  # bvnot
                 elif opcode == EVM.SHL:
                     w = ex.st.pop()
-                    ex.st.push(b2i(ex.st.pop()) << b2i(w)) # bvshl
+                    ex.st.push(b2i(ex.st.pop()) << b2i(w))  # bvshl
                 elif opcode == EVM.SAR:
                     w = ex.st.pop()
-                    ex.st.push(ex.st.pop() >> w) # bvashr
+                    ex.st.push(ex.st.pop() >> w)  # bvashr
                 elif opcode == EVM.SHR:
                     w = ex.st.pop()
-                    ex.st.push(LShR(ex.st.pop(), w)) # bvlshr
+                    ex.st.push(LShR(ex.st.pop(), w))  # bvlshr
 
                 elif opcode == EVM.SIGNEXTEND:
-                    w = ex.st.pop()
-                    if not is_bv_value(w): raise ValueError(w)
-
-                    w = int(str(w))
-                    if w <= 30: # if w == 31, result is SignExt(0, value) == value
+                    w = int_of(ex.st.pop(), "symbolic SIGNEXTEND size")
+                    if w <= 30:  # if w == 31, result is SignExt(0, value) == value
                         bl = (w + 1) * 8
                         ex.st.push(SignExt(256 - bl, Extract(bl - 1, 0, ex.st.pop())))
 
                 elif opcode == EVM.XOR:
-                    ex.st.push(ex.st.pop() ^ ex.st.pop()) # bvxor
+                    ex.st.push(ex.st.pop() ^ ex.st.pop())  # bvxor
 
                 elif opcode == EVM.CALLDATALOAD:
                     if ex.calldata is None:
                         ex.st.push(f_calldataload(ex.st.pop()))
                     else:
-                        offset: int = int(str(ex.st.pop()))
-                        ex.st.push(Concat((ex.calldata + [BitVecVal(0, 8)] * 32)[offset:offset+32]))
-                    #   try:
-                    #       offset: int = int(str(ex.st.pop()))
-                    #       ex.st.push(Concat(ex.calldata[offset:offset+32]))
-                    #   except:
-                    #       ex.st.push(f_calldataload(ex.st.pop()))
+                        offset: int = int_of(
+                            ex.st.pop(), "symbolic CALLDATALOAD offset"
+                        )
+                        ex.st.push(
+                            Concat(
+                                (ex.calldata + [BitVecVal(0, 8)] * 32)[
+                                    offset : offset + 32
+                                ]
+                            )
+                        )
                 elif opcode == EVM.CALLDATASIZE:
                     if ex.calldata is None:
                         ex.st.push(f_calldatasize())
                     else:
                         ex.st.push(con(len(ex.calldata)))
                 elif opcode == EVM.CALLVALUE:
                     ex.st.push(ex.callvalue)
                 elif opcode == EVM.CALLER:
-                    ex.st.push(ex.caller)
+                    ex.st.push(uint256(ex.caller))
                 elif opcode == EVM.ORIGIN:
-                    ex.st.push(f_origin())
-                    ex.solver.add(Extract(255, 160, f_origin()) == BitVecVal(0, 96))
+                    ex.st.push(uint256(f_origin()))
                 elif opcode == EVM.ADDRESS:
-                    ex.st.push(ex.this)
+                    ex.st.push(uint256(ex.this))
                 elif opcode == EVM.EXTCODESIZE:
-                    address = ex.st.pop()
+                    address = uint160(ex.st.pop())
                     if address in ex.code:
                         codesize = con(len(ex.code[address]))
                     else:
                         codesize = f_extcodesize(address)
-                        if address == con(hevm_cheat_code.address):
+                        if (
+                            address == hevm_cheat_code.address
+                            or address == halmos_cheat_code.address
+                        ):
                             ex.solver.add(codesize > 0)
                     ex.st.push(codesize)
                 elif opcode == EVM.EXTCODEHASH:
                     ex.st.push(f_extcodehash(ex.st.pop()))
                 elif opcode == EVM.CODESIZE:
                     ex.st.push(con(len(ex.code[ex.this])))
                 elif opcode == EVM.GAS:
-                    ex.st.push(f_gas(con(ex.cnt_gas())))
+                    ex.st.push(f_gas(con(ex.new_gas_id())))
                 elif opcode == EVM.GASPRICE:
                     ex.st.push(f_gasprice())
 
                 elif opcode == EVM.BASEFEE:
                     ex.st.push(ex.block.basefee)
                 elif opcode == EVM.CHAINID:
                     ex.st.push(ex.block.chainid)
                 elif opcode == EVM.COINBASE:
-                    ex.st.push(ex.block.coinbase)
+                    ex.st.push(uint256(ex.block.coinbase))
                 elif opcode == EVM.DIFFICULTY:
                     ex.st.push(ex.block.difficulty)
                 elif opcode == EVM.GASLIMIT:
                     ex.st.push(ex.block.gaslimit)
                 elif opcode == EVM.NUMBER:
                     ex.st.push(ex.block.number)
                 elif opcode == EVM.TIMESTAMP:
@@ -1292,189 +2180,234 @@
                 elif opcode == EVM.PC:
                     ex.st.push(con(ex.pc))
 
                 elif opcode == EVM.BLOCKHASH:
                     ex.st.push(f_blockhash(ex.st.pop()))
 
                 elif opcode == EVM.BALANCE:
-                    ex.st.push(ex.balance_of(ex.st.pop()))
+                    ex.st.push(ex.balance_of(uint160(ex.st.pop())))
                 elif opcode == EVM.SELFBALANCE:
                     ex.st.push(ex.balance_of(ex.this))
 
                 elif opcode == EVM.CALL or opcode == EVM.STATICCALL:
-                    self.call(ex, opcode, stack, step_id, out)
+                    self.call(ex, opcode, stack, step_id, out, bounded_loops)
                     continue
 
                 elif opcode == EVM.SHA3:
                     ex.sha3()
 
                 elif opcode == EVM.CREATE:
-                    self.create(ex, stack, step_id, out)
+                    self.create(ex, stack, step_id, out, bounded_loops)
                     continue
 
                 elif opcode == EVM.POP:
                     ex.st.pop()
                 elif opcode == EVM.MLOAD:
                     ex.st.mload()
                 elif opcode == EVM.MSTORE:
                     ex.st.mstore(True)
                 elif opcode == EVM.MSTORE8:
                     ex.st.mstore(False)
 
                 elif opcode == EVM.MSIZE:
                     size: int = len(ex.st.memory)
-                    size = ((size + 31) // 32) * 32 # round up to the next multiple of 32
+                    # round up to the next multiple of 32
+                    size = ((size + 31) // 32) * 32
                     ex.st.push(con(size))
 
                 elif opcode == EVM.SLOAD:
-                    ex.st.push(ex.sload(ex.st.pop()))
+                    ex.st.push(ex.sload(ex.this, ex.st.pop()))
                 elif opcode == EVM.SSTORE:
-                    ex.sstore(ex.st.pop(), ex.st.pop())
+                    ex.sstore(ex.this, ex.st.pop(), ex.st.pop())
 
                 elif opcode == EVM.RETURNDATASIZE:
                     ex.st.push(con(ex.returndatasize()))
                 elif opcode == EVM.RETURNDATACOPY:
                     loc: int = ex.st.mloc()
-                    offset: int = int(str(ex.st.pop())) # offset must be concrete
-                    size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
-                    wstore_partial(ex.st.memory, loc, offset, size, ex.output, ex.returndatasize())
+                    offset: int = int_of(ex.st.pop(), "symbolic RETURNDATACOPY offset")
+                    # size (in bytes)
+                    size: int = int_of(ex.st.pop(), "symbolic RETURNDATACOPY size")
+                    wstore_partial(
+                        ex.st.memory, loc, offset, size, ex.output, ex.returndatasize()
+                    )
 
                 elif opcode == EVM.CALLDATACOPY:
                     loc: int = ex.st.mloc()
-                    offset: int = int(str(ex.st.pop())) # offset must be concrete
-                    size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
+                    offset: int = int_of(ex.st.pop(), "symbolic CALLDATACOPY offset")
+                    # size (in bytes)
+                    size: int = int_of(ex.st.pop(), "symbolic CALLDATACOPY size")
                     if size > 0:
                         if ex.calldata is None:
-                            f_calldatacopy = Function('calldatacopy_'+str(size*8), BitVecSort(256), BitVecSort(size*8))
+                            f_calldatacopy = Function(
+                                "calldatacopy_" + str(size * 8),
+                                BitVecSort(256),
+                                BitVecSort(size * 8),
+                            )
                             data = f_calldatacopy(offset)
                             wstore(ex.st.memory, loc, size, data)
                         else:
                             if offset + size <= len(ex.calldata):
-                                wstore_bytes(ex.st.memory, loc, size, ex.calldata[offset:offset+size])
-                            elif offset == len(ex.calldata): # copy zero bytes
-                                wstore_bytes(ex.st.memory, loc, size, [BitVecVal(0, 8) for _ in range(size)])
+                                wstore_bytes(
+                                    ex.st.memory,
+                                    loc,
+                                    size,
+                                    ex.calldata[offset : offset + size],
+                                )
+                            elif offset == len(ex.calldata):
+                                # copy zero bytes
+                                wstore_bytes(
+                                    ex.st.memory,
+                                    loc,
+                                    size,
+                                    [BitVecVal(0, 8) for _ in range(size)],
+                                )
                             else:
                                 raise ValueError(offset, size, len(ex.calldata))
 
                 elif opcode == EVM.CODECOPY:
                     loc: int = ex.st.mloc()
-                    pc: int = int(str(ex.st.pop())) # pc must be concrete
-                    size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
+                    offset: int = int_of(ex.st.pop(), "symbolic CODECOPY offset")
+                    # size (in bytes)
+                    size: int = int_of(ex.st.pop(), "symbolic CODECOPY size")
                     wextend(ex.st.memory, loc, size)
-                    for i in range(size):
-                        ex.st.memory[loc + i] = ex.read_code(pc + i)
+
+                    codeslice = ex.code[ex.this][offset : offset + size]
+                    ex.st.memory[loc : loc + size] = iter_bytes(codeslice)
 
                 elif opcode == EVM.BYTE:
-                    idx: int = int(str(ex.st.pop())) # index must be concrete
-                    if idx < 0: raise ValueError(idx)
+                    idx = ex.st.pop()
                     w = ex.st.pop()
-                    if idx >= 32:
-                        ex.st.push(con(0))
+                    if is_bv_value(idx):
+                        idx = idx.as_long()
+                        if idx < 0:
+                            raise ValueError(idx)
+                        if idx >= 32:
+                            ex.st.push(con(0))
+                        else:
+                            ex.st.push(
+                                ZeroExt(
+                                    248, Extract((31 - idx) * 8 + 7, (31 - idx) * 8, w)
+                                )
+                            )
                     else:
-                        ex.st.push(ZeroExt(248, Extract((31-idx)*8+7, (31-idx)*8, w)))
+                        if self.options["debug"]:
+                            print(
+                                f"Warning: the use of symbolic BYTE indexing may potentially impact the performance of symbolic reasoning: BYTE {idx} {w}"
+                            )
+                        ex.st.push(self.sym_byte_of(idx, w))
 
                 elif EVM.LOG0 <= opcode <= EVM.LOG4:
                     num_keys: int = opcode - EVM.LOG0
                     loc: int = ex.st.mloc()
-                    size: int = int(str(ex.st.pop())) # size (in bytes) must be concrete
+                    # size (in bytes)
+                    size: int = int_of(ex.st.pop(), "symbolic LOG data size")
                     keys = []
                     for _ in range(num_keys):
                         keys.append(ex.st.pop())
-                    ex.log.append((keys, wload(ex.st.memory, loc, size) if size > 0 else None))
+                    ex.log.append(
+                        (keys, wload(ex.st.memory, loc, size) if size > 0 else None)
+                    )
+
+                elif opcode == EVM.PUSH0:
+                    ex.st.push(con(0))
 
                 elif EVM.PUSH1 <= opcode <= EVM.PUSH32:
-                    if is_bv_value(o.op[1]):
-                        val = int(str(o.op[1]))
-                        if opcode == EVM.PUSH32 and val in sha3_inv: # restore precomputed hashes
+                    if is_concrete(insn.operand):
+                        val = int_of(insn.operand)
+                        if opcode == EVM.PUSH32 and val in sha3_inv:
+                            # restore precomputed hashes
                             ex.sha3_data(con(sha3_inv[val]), 32)
                         else:
                             ex.st.push(con(val))
                     else:
                         if opcode == EVM.PUSH32:
-                            ex.st.push(o.op[1])
+                            ex.st.push(insn.operand)
                         else:
-                            ex.st.push(ZeroExt((EVM.PUSH32 - opcode)*8, o.op[1]))
+                            ex.st.push(ZeroExt((EVM.PUSH32 - opcode) * 8, insn.operand))
                 elif EVM.DUP1 <= opcode <= EVM.DUP16:
                     ex.st.dup(opcode - EVM.DUP1 + 1)
                 elif EVM.SWAP1 <= opcode <= EVM.SWAP16:
                     ex.st.swap(opcode - EVM.SWAP1 + 1)
 
                 else:
                     out.append(ex)
                     continue
 
                 ex.next_pc()
                 stack.append((ex, step_id))
 
+            except NotConcreteError as err:
+                ex.error = f"{err}"
+                out.append(ex)
+                continue
+
             except Exception as err:
-                if self.options['debug']:
+                if self.options["debug"]:
                     print(ex)
                 raise
 
-        return (out, steps)
+        return (out, steps, bounded_loops)
 
     def mk_exec(
         self,
         #
-        pgm,
         code,
         storage,
         balance,
         #
         block,
         #
         calldata,
         callvalue,
         caller,
         this,
         #
-    #   pc,
-    #   st,
-    #   jumpis,
-    #   output,
+        # pc,
+        # st,
+        # jumpis,
+        # output,
         symbolic,
-    #   prank,
+        # prank,
         #
         solver,
-    #   path,
+        # path,
         #
-    #   log,
-    #   cnts,
-    #   sha3s,
-    #   storages,
-    #   balances,
-    #   calls,
-    #   failed,
-    #   error,
+        # log,
+        # cnts,
+        # sha3s,
+        # storages,
+        # balances,
+        # calls,
+        # failed,
+        # error,
     ) -> Exec:
         return Exec(
-            pgm      = pgm,
-            code     = code,
-            storage  = storage,
-            balance  = balance,
+            code=code,
+            storage=storage,
+            balance=balance,
             #
-            block    = block,
+            block=block,
             #
-            calldata = calldata,
-            callvalue= callvalue,
-            caller   = caller,
-            this     = this,
+            calldata=calldata,
+            callvalue=callvalue,
+            caller=caller,
+            this=this,
             #
-            pc       = 0,
-            st       = State(),
-            jumpis   = {},
-            output   = None,
-            symbolic = symbolic,
-            prank    = Prank(),
+            pc=0,
+            st=State(),
+            jumpis={},
+            output=None,
+            symbolic=symbolic,
+            prank=Prank(),
             #
-            solver   = solver,
-            path     = [],
+            solver=solver,
+            path=[],
             #
-            log      = [],
-            cnts     = defaultdict(int),
-            sha3s    = [],
-            storages = {},
-            balances = {},
-            calls    = [],
-            failed   = False,
-            error    = '',
+            log=[],
+            cnts=defaultdict(lambda: defaultdict(int)),
+            sha3s=[],
+            storages={},
+            balances={},
+            calls=[],
+            failed=False,
+            error="",
         )
```

### Comparing `halmos-0.0.9/src/halmos.egg-info/PKG-INFO` & `halmos-0.1.0/src/halmos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.0.9
+Version: 0.1.0
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: Daejun Park
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -33,40 +33,45 @@
 
 ## Installation
 
 ```
 $ pip install halmos
 ```
 
+Or, if you want to try the latest dev version:
+```
+$ pip install git+https://github.com/a16z/halmos
+```
+
 ## Usage
 
 ```
 $ cd /path/to/src
 $ halmos
 ```
 
 For more details:
 ```
 $ halmos --help
 ```
 
 ## Examples
 
-Given a contract, [Example.sol](examples/src/Example.sol):
+Given a contract, [Example.sol](examples/toy/src/Example.sol):
 ```solidity
 contract Example {
     function totalPriceBuggy(uint96 price, uint32 quantity) public pure returns (uint128) {
         unchecked {
             return uint120(price) * quantity; // buggy type casting: uint120 vs uint128
         }
     }
 }
 ```
 
-You write some **property-based tests** (in Solidity), [Example.t.sol](examples/test/Example.t.sol):
+You write some **property-based tests** (in Solidity), [Example.t.sol](examples/toy/test/Example.t.sol):
 ```solidity
 contract ExampleTest is Example {
     function testTotalPriceBuggy(uint96 price, uint32 quantity) public pure {
         uint128 total = totalPriceBuggy(price, quantity);
         assert(quantity == 0 || total >= price);
     }
 }
@@ -83,10 +88,41 @@
 $ halmos
 [FAIL] testTotalPriceBuggy(uint96,uint32) (paths: 6, time: 0.10s, bounds: [])
 Counterexample: [p_price_uint96 = 39614081294025656978550816768, p_quantity_uint32 = 1073741824]
 ```
 
 _(In this specific example, Halmos discovered an input that violated the assertion, which was missed by the fuzzer!)_
 
+## Develop
+
+```sh
+# if you want to submit a pull request, fork the repository:
+
+gh repo fork a16z/halmos
+
+# or if you just want to develop locally, clone it
+# git clone git@github.com:a16z/halmos.git
+
+# create and activate a virtual environment
+
+python3.11 -m venv .venv
+source .venv/bin/activate
+
+# install the dependencies
+
+python -m pip install -r requirements.txt
+python -m pip install -r requirements-dev.txt
+
+# install and run the git hook scripts
+
+pre-commit install
+pre-commit run --all-files
+
+# we recommend enabling the black formatter in your editor
+# but you can run it manually if needed:
+
+python -m black .
+```
+
 ## Disclaimer
 
 _These smart contracts and code are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts and code. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions or loss of transmitted information. THE SMART CONTRACTS AND CODE CONTAINED HEREIN ARE FURNISHED AS IS, WHERE IS, WITH ALL FAULTS AND WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING ANY WARRANTY OF MERCHANTABILITY, NON-INFRINGEMENT OR FITNESS FOR ANY PARTICULAR PURPOSE. Further, use of any of these smart contracts and code may be restricted or prohibited under applicable law, including securities laws, and it is therefore strongly advised for you to contact a reputable attorney in any jurisdiction where these smart contracts and code may be accessible for any questions or concerns with respect thereto. Further, no information provided in this repo should be construed as investment advice or legal advice for any particular facts or circumstances, and is not meant to replace competent counsel. a16z is not liable for any use of the foregoing, and users should proceed with caution and use at their own risk. See a16z.com/disclosures for more info._
```

### Comparing `halmos-0.0.9/tests/src/Counter.sol` & `halmos-0.1.0/tests/src/Counter.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.9/tests/src/Storage.sol` & `halmos-0.1.0/tests/src/Storage.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.0.9/tests/test/Counter.t.sol` & `halmos-0.1.0/tests/test/Counter.t.sol`

 * *Files 6% similar despite different names*

```diff
@@ -1,129 +1,130 @@
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity >=0.8.0 <0.9.0;
 
 import "../src/Counter.sol";
 
+/// @custom:halmos --loop 4 --symbolic-storage
 contract CounterTest is Counter {
-    function testSet(uint n) public {
+    function check_set(uint n) public {
         set(n);
         assert(cnt == n);
     }
 
-    function testInc() public {
+    function check_inc() public {
         uint oldCnt = cnt;
         inc();
         assert(cnt > oldCnt);
         assert(cnt == oldCnt + 1);
     }
 
-    function testIncOpt() public {
+    function check_incOpt() public {
         uint oldCnt = cnt;
         require(cnt < type(uint).max);
         incOpt();
         assert(cnt > oldCnt);
         assert(cnt == oldCnt + 1);
     }
 
-    function testIncBy(uint n) public {
+    function check_incBy(uint n) public {
         uint oldCnt = cnt;
         incBy(n);
         assert(cnt < oldCnt || cnt == oldCnt + n); // cnt >= oldCnt ==> cnt == oldCnt + n
     }
 
     function specLoopFor(uint n) public {
         uint oldCnt = cnt;
         loopFor(n);
         assert(cnt >= oldCnt);
         assert(cnt == oldCnt + n);
     }
-    function testLoopFor(uint8 k) public {
+    function check_loopFor(uint8 k) public {
         specLoopFor(k);
     }
 
     function specLoopWhile(uint n) public {
         uint oldCnt = cnt;
         loopWhile(n);
         assert(cnt >= oldCnt);
         assert(cnt == oldCnt + n);
     }
-    function testLoopWhile(uint8 k) public {
+    function check_loopWhile(uint8 k) public {
         specLoopWhile(k);
     }
 
     function specLoopDoWhile(uint n) public {
         uint oldCnt = cnt;
         loopDoWhile(n);
         assert(cnt > oldCnt);
         if (n == 0) assert(cnt == oldCnt + 1);
         else assert(cnt == oldCnt + n);
     }
-    function testLoopDoWhile(uint8 k) public {
+    function check_loopDoWhile(uint8 k) public {
         specLoopDoWhile(k);
     }
 
-    function testLoopConst() public {
+    function check_loopConst() public {
         uint oldCnt = cnt;
         loopConst();
         assert(cnt >= oldCnt);
         assert(cnt == oldCnt + 2);
     }
 
-    function testLoopConstIf() public {
+    function check_loopConstIf() public {
         uint oldCnt = cnt;
         loopConstIf();
         assert(cnt >= oldCnt);
         assert(cnt <= oldCnt + 4);
     }
 
     function specSetSum(uint[2] memory arr) public {
         setSum(arr);
         assert(cnt == arr[0] + arr[1]);
     }
-    function testSetSum(uint248 a, uint248 b) public {
+    function check_setSum(uint248 a, uint248 b) public {
         specSetSum([uint(a), b]);
     }
 
-    function testSetString(uint, string memory s, uint, string memory r, uint) public {
+    function check_setString(uint, string memory s, uint, string memory r, uint) public {
         uint oldCnt = cnt;
         setString(s);
         setString(r);
         assert(cnt == oldCnt + bytes(s).length + bytes(r).length);
     }
 
-    function testFoo(uint a, uint b, uint c, uint d) public {
+    function check_foo(uint a, uint b, uint c, uint d) public {
         uint oldCnt = cnt;
         foo(a, b, c, d);
         assert(cnt == oldCnt + 4);
     }
 
-    function testDiv1(uint x, uint y) public pure {
+    function check_div_1(uint x, uint y) public pure {
         if (y > 0) {
             assert(x / y <= x);
         }
     }
 
-    function testDiv2(uint x, uint y) public pure {
+    function check_div_2(uint x, uint y) public pure {
         if (y > 0) {
             assert(x / y == x / y);
         }
     }
 
-    function testMulDiv(uint x, uint y) public pure {
+    function check_mulDiv(uint x, uint y) public pure {
         unchecked {
             if (x > 0 && y > 0) {
                 uint z = x * y;
                 if (z / x == y) {
                     assert(z / x == y);
                   //assert(z / y == x); // smt failed to solve
                 }
             }
         }
     }
 
-    /* TODO: support testFail prefix
-    function testFail() public pure {
+    /* TODO: support checkFail prefix
+    function checkFail() public pure {
         require(false);
         // deadcode
     }
     */
 }
```

### Comparing `halmos-0.0.9/tests/test/Create.t.sol` & `halmos-0.1.0/tests/test/Create.t.sol`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 contract CreateTest is Test {
     Create public create;
 
     function setUp() public {
         create = new Create(0x220E);
     }
 
-    /* TODO: support testFail prefix
-    function testFailSetUp() public {
+    /* TODO: support checkFail prefix
+    function checkFail_setUp() public {
         assertEq(create.value(), 0);
     }
     */
 
-    function testSet(uint x) public {
+    function check_set(uint x) public {
         create.set(x);
         assertEq(create.value(), x);
     }
 
-    function testImmutable() public {
+    function check_immutable() public {
         assertEq(create.halmos(), 0x220E);
     }
 
-    function testInitialized() public {
+    function check_initialized() public {
         assertEq(create.initialized(), 7);
     }
 
-    function testConst() public {
+    function check_const() public {
         assertEq(create.const(), 11);
     }
 }
```

### Comparing `halmos-0.0.9/tests/test/Deal.t.sol` & `halmos-0.1.0/tests/test/Deal.t.sol`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 pragma solidity >=0.8.0 <0.9.0;
 
 import "forge-std/Test.sol";
 
 contract DealTest is Test {
     C c;
 
-    function testDeal1(address payable receiver, uint amount) public {
+    function check_deal_1(address payable receiver, uint amount) public {
         vm.deal(receiver, amount);
         assert(receiver.balance == amount);
     }
 
-    function testDeal2(address payable receiver, uint amount1, uint amount2) public {
+    function check_deal_2(address payable receiver, uint amount1, uint amount2) public {
         vm.deal(receiver, amount1);
         vm.deal(receiver, amount2); // reset the balance, not increasing
         assert(receiver.balance == amount2);
     }
 
-    function testDealNew() public {
+    function check_deal_new() public {
         vm.deal(address(this), 3 ether);
 
         c = new C{value: 3 ether}();
 
         assertGe(address(c).balance, 3 ether); // it is possible to send ether to c before it is created
         assert(address(this).balance == 0 ether);
     }
```

### Comparing `halmos-0.0.9/tests/test/Invalid.t.sol` & `halmos-0.1.0/tests/test/Invalid.t.sol`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity ^0.5.2;
 
 contract OldCompilerTest {
 
-    function testAssert(uint x) public {
+    function check_assert(uint x) public pure {
         if (x == 0) return;
         assert(false); // old compiler versions don't revert with panic; instead, they run invalid opcode, which halmos ignores, resulting in no error here.
-    //myAssert(false); // you can use your own assertion that panic-reverts if assertion fails, when using halmos for old version code.
     }
 
-    function myAssert(bool cond) internal {
+    function check_myAssert(uint x) public pure {
+        if (x == 0) return;
+        myAssert(false); // you can use your own assertion that panic-reverts if assertion fails, when using halmos for old version code.
+    }
+
+    function myAssert(bool cond) internal pure {
         if (!cond) {
             assembly {
                 mstore(0x00, 0x4e487b71)
                 mstore(0x20, 0x01)
                 revert(0x1c, 0x24)
             }
         }
```

### Comparing `halmos-0.0.9/tests/test/Library.t.sol` & `halmos-0.1.0/tests/test/Library.t.sol`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         unchecked {
             return x + y;
         }
     }
 }
 
 contract LibraryTest {
-    function testAdd(uint x, uint y) public pure {
+    function check_add(uint x, uint y) public pure {
         unchecked {
             assert(Math._add(x,y) == x+y);
             /* TODO: support public library functions (library linking)
             assert(Math.add(x,y) == x+y);
             */
         }
     }
```

### Comparing `halmos-0.0.9/tests/test/List.t.sol` & `halmos-0.1.0/tests/test/List.t.sol`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity >=0.8.0 <0.9.0;
 
 import "forge-std/Test.sol";
 import "../src/List.sol";
 
+/// @custom:halmos --symbolic-storage
 contract ListTest is Test, List {
-    function testAdd(uint x) public {
+    function check_add(uint x) public {
         uint oldSize = arr.length;
         vm.assume(oldSize < type(uint).max);
         add(x);
         uint newSize = arr.length;
         assert(oldSize < newSize);
         assert(oldSize + 1 == newSize);
         assert(arr[newSize-1] == x);
     }
 
-    function testRemove() public {
+    function check_remove() public {
         uint oldSize = arr.length;
         vm.assume(oldSize > 0);
         remove();
         uint newSize = arr.length;
         assert(oldSize > newSize);
         assert(oldSize == newSize + 1);
     }
 
-    function testSet(uint i, uint x) public {
+    function check_set(uint i, uint x) public {
         vm.assume(i < arr.length);
         set(i, x);
         assert(arr[i] == x);
     }
 }
 
+/// @custom:halmos --symbolic-storage
 contract ListTestTest is Test {
     List list;
 
     function setUp() public {
         list = new List();
         list.add(1);
     }
 
-    function testAdd(uint x) public {
+    function check_add(uint x) public {
         uint oldSize = list.size();
         vm.assume(oldSize < type(uint).max);
         list.add(x);
         uint newSize = list.size();
         assert(oldSize < newSize);
         assert(oldSize + 1 == newSize);
         assert(list.arr(newSize-1) == x);
     }
 
-    function testRemove() public {
+    function check_remove() public {
         uint oldSize = list.size();
         vm.assume(oldSize > 0);
         list.remove();
         uint newSize = list.size();
         assert(oldSize > newSize);
         assert(oldSize == newSize + 1);
     }
 
-    function testSet(uint i, uint x) public {
+    function check_set(uint i, uint x) public {
         vm.assume(i < list.size());
         list.set(i, x);
         assert(list.arr(i) == x);
     }
 }
```

### Comparing `halmos-0.0.9/tests/test/Prank.t.sol` & `halmos-0.1.0/tests/test/Prank.t.sol`

 * *Files 27% similar despite different names*

```diff
@@ -13,29 +13,37 @@
     }
 
     function recordCaller() public {
         caller = msg.sender;
     }
 }
 
+contract ConstructorRecorder {
+    address public caller;
+
+    constructor() {
+        caller = msg.sender;
+    }
+}
+
 contract Ext is Test {
     function prank(address user) public {
         vm.prank(user);
     }
 }
 
 contract PrankSetUpTest is Test {
     Target target;
 
     function setUp() public {
         target = new Target();
         vm.prank(address(target)); // prank is reset after setUp()
     }
 
-    function testPrank(address user) public {
+    function check_prank(address user) public {
         vm.prank(user);
         target.recordCaller();
         assert(target.caller() == user);
     }
 }
 
 contract PrankTest is Test {
@@ -48,24 +56,24 @@
         ext = new Ext();
     }
 
     function prank(address user) public {
         vm.prank(user);
     }
 
-    function testPrank(address user) public {
+    function check_prank(address user) public {
         vm.prank(user);
         target.recordCaller();
         assert(target.caller() == user);
 
         target.recordCaller();
         assert(target.caller() == address(this));
     }
 
-    function testStartPrank(address user) public {
+    function check_startPrank(address user) public {
         vm.startPrank(user);
 
         target.recordCaller();
         assert(target.caller() == user);
 
         target.setCaller(address(this));
         assert(target.caller() == address(this));
@@ -75,60 +83,73 @@
 
         vm.stopPrank();
 
         target.recordCaller();
         assert(target.caller() == address(this));
     }
 
-    function testPrankInternal(address user) public {
+    function check_prank_Internal(address user) public {
         prank(user); // indirect prank
         target.recordCaller();
         assert(target.caller() == user);
     }
 
-    function testPrankExternal(address user) public {
+    function check_prank_External(address user) public {
         ext.prank(user); // prank isn't propagated beyond the vm boundry
         target.recordCaller();
         assert(target.caller() == address(this));
     }
 
-    function testPrankExternalSelf(address user) public {
+    function check_prank_ExternalSelf(address user) public {
         this.prank(user); // prank isn't propagated beyond the vm boundry
         target.recordCaller();
         assert(target.caller() == address(this));
     }
 
-    function testPrankNew(address user) public {
+    function check_prank_New(address user) public {
         vm.prank(user);
         dummy = new Dummy(); // contract creation also consumes prank
         vm.prank(user);
         target.recordCaller();
         assert(target.caller() == user);
     }
 
-    function testPrankReset1(address user) public {
+    function check_prank_Reset1(address user) public {
     //  vm.prank(address(target)); // overwriting active prank is not allowed
         vm.prank(user);
         target.recordCaller();
         assert(target.caller() == user);
     }
 
-    function testPrankReset2(address user) public {
+    function check_prank_Reset2(address user) public {
     //  vm.prank(address(target)); // overwriting active prank is not allowed
         vm.startPrank(user);
         target.recordCaller();
         assert(target.caller() == user);
     }
 
-    function testStopPrank1(address user) public {
+    function check_stopPrank_1(address user) public {
         vm.prank(user);
         vm.stopPrank(); // stopPrank can be used to disable both startPrank() and prank()
         target.recordCaller();
         assert(target.caller() == address(this));
     }
 
-    function testStopPrank2() public {
+    function check_stopPrank_2() public {
         vm.stopPrank(); // stopPrank is allowed even when no active prank exists!
         target.recordCaller();
         assert(target.caller() == address(this));
     }
+
+    function check_prank_Constructor(address user) public {
+        vm.prank(user);
+        ConstructorRecorder recorder = new ConstructorRecorder();
+        assert(recorder.caller() == user);
+    }
+
+    // TODO: uncomment when we add CREATE2 support
+    // function check_prank_ConstructorCreate2(address user, bytes32 salt) public {
+    //     vm.prank(user);
+    //     ConstructorRecorder recorder = new ConstructorRecorder{salt:salt}();
+    //     assert(recorder.caller() == user);
+    // }
 }
```

### Comparing `halmos-0.0.9/tests/test/Send.t.sol` & `halmos-0.1.0/tests/test/Send.t.sol`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity >=0.8.0 <0.9.0;
 
 contract SendTest {
 
-    function testSend(address payable receiver, uint amount, address others) public {
+    function check_Send(address payable receiver, uint amount, address others) public {
         require(others != address(this) && others != receiver);
 
         require(address(this) != receiver);
 
         uint oldBalanceSender = address(this).balance;
         uint oldBalanceReceiver = receiver.balance;
         uint oldBalanceOthers = others.balance;
@@ -22,15 +22,15 @@
             assert(newBalanceSender == oldBalanceSender - amount);
             assert(newBalanceReceiver == oldBalanceReceiver + amount);
             assert(oldBalanceSender + oldBalanceReceiver == newBalanceSender + newBalanceReceiver);
             assert(oldBalanceOthers == newBalanceOthers);
         }
     }
 
-    function testSendSelf(address payable receiver, uint amount, address others) public {
+    function check_SendSelf(address payable receiver, uint amount, address others) public {
         require(others != address(this) && others != receiver);
 
         require(address(this) == receiver);
 
         uint oldBalanceSender = address(this).balance;
         uint oldBalanceReceiver = receiver.balance;
         uint oldBalanceOthers = others.balance;
```

### Comparing `halmos-0.0.9/tests/test/Setup.t.sol` & `halmos-0.1.0/tests/test/Setup.t.sol`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
         users = new address[](size);
         users[0] = address(bytes20(keccak256("test")));
         for (uint256 i = 1; i < size - 1; i++) {
             users[i] = address(uint160(users[i - 1]) + 1);
         }
     }
 
-    function testTrue() public {
+    function check_True() public {
         assertEq(users[0], address(bytes20(keccak256("test"))));
         assertEq(users[1], address(uint160(users[0]) + 1));
         assertEq(users[2], address(0));
     }
 }
```

### Comparing `halmos-0.0.9/tests/test/SetupPlus.t.sol` & `halmos-0.1.0/tests/test/SetupPlus.t.sol`

 * *Files 17% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 contract SetupPlusTest {
     A a;
 
     function setUp() public {
         a = new A(11, 200);
     }
 
-    // if setUpPlus() is provided, Halmos uses setUpPlus() instead of setUp().
-    // setUpPlus() is symbolically executed.
+    // if setUpSymbolic() is provided, Halmos uses setUpSymbolic() instead of setUp().
+    // setUpSymbolic() is symbolically executed.
 
-    // if multiple setUpPlus() functions are provided, the last one in the lexicographical order will be used.
-    // e.g., setUpPlus(uint256,uint256) is used instead of setUpPlus(uint256).
+    // if multiple setUpSymbolic() functions are provided, the last one in the lexicographical order will be used.
+    // e.g., setUpSymbolic(uint256,uint256) is used instead of setUpSymbolic(uint256).
 
-    function setUpPlus(uint x, uint y) public {
+    function setUpSymbolic(uint x, uint y) public {
         require(x > 10);
         require(y > 100);
         a = new A(x, y);
     }
 
-    function setUpPlus(uint x) public {
+    function setUpSymbolic(uint x) public {
         a = new A(x, x);
     }
 
-    function testSetup() public {
+    function check_Setup() public view {
         assert(a.x() > 10);
         assert(a.y() > 100);
     }
 }
 
 contract B {
     uint public x1;
@@ -75,22 +75,22 @@
         init[0] = 10;
         init[1] = 20;
         init[2] = 30;
         init[3] = 40;
         mk();
     }
 
-    function setUpPlus(uint[4] memory _init) public {
+    function setUpSymbolic(uint[4] memory _init) public {
         init[0] = _init[0];
         init[1] = _init[1];
         init[2] = _init[2];
         init[3] = _init[3];
         mk();
     }
 
-    function testSetup() public {
+    function check_Setup() public view {
         assert(b.x1() == init[0]);
         assert(b.y1() == init[1]);
         assert(b.x2() == init[2]);
         assert(b.y2() == init[3]);
     }
 }
```

### Comparing `halmos-0.0.9/tests/test/Storage.t.sol` & `halmos-0.1.0/tests/test/Storage.t.sol`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 // SPDX-License-Identifier: AGPL-3.0
 pragma solidity >=0.8.0 <0.9.0;
 
 import "forge-std/Test.sol";
 import "../src/Storage.sol";
 
+/// @custom:halmos --symbolic-storage
 contract StorageTest is Storage {
-    function testSetMap1(uint k, uint v) public {
+    function check_setMap1(uint k, uint v) public {
         setMap1(k, v);
         assert(map1[k] == v);
     }
 
-    function testSetMap2(uint k1, uint k2, uint v) public {
+    function check_setMap2(uint k1, uint k2, uint v) public {
         setMap2(k1, k2, v);
         assert(map2[k1][k2] == v);
     }
 
-    function testSetMap3(uint k1, uint k2, uint k3, uint v) public {
+    function check_setMap3(uint k1, uint k2, uint k3, uint v) public {
         setMap3(k1, k2, k3, v);
         assert(map3[k1][k2][k3] == v);
     }
 
-    function testAddArr1(uint v) public {
+    function check_addArr1(uint v) public {
         uint size = arr1.length;
         addArr1(v);
         assert(arr1.length == size + 1);
         assert(arr1[size] == v);
     }
 
-    function testAddArr2(uint i, uint v) public {
+    function check_addArr2(uint i, uint v) public {
         uint size = arr2[i].length;
         addArr2(i, v);
         assert(arr2[i].length == size + 1);
         assert(arr2[i][size] == v);
     }
 
-    function testAddMap1Arr1(uint k, uint v) public {
+    function check_addMap1Arr1(uint k, uint v) public {
         uint size = map1Arr1[k].length;
         addMap1Arr1(k, v);
         assert(map1Arr1[k].length == size + 1);
         assert(map1Arr1[k][size] == v);
     }
 }
```

### Comparing `halmos-0.0.9/tests/test/Warp.t.sol` & `halmos-0.1.0/tests/test/Warp.t.sol`

 * *Files 9% similar despite different names*

```diff
@@ -24,43 +24,43 @@
         vm.warp(1000);
     }
 
     function warp(uint time) public {
         vm.warp(time);
     }
 
-    function testWarp(uint time) public {
+    function check_warp(uint time) public {
         vm.warp(time);
         assert(block.timestamp == time);
     }
 
-    function testWarpInternal(uint time) public {
+    function check_warp_Internal(uint time) public {
         warp(time);
         assert(block.timestamp == time);
     }
 
-    function testWarpExternal(uint time) public {
+    function check_warp_External(uint time) public {
         ext.warp(time);
         assert(block.timestamp == time);
     }
 
-    function testWarpExternalSelf(uint time) public {
+    function check_warp_ExternalSelf(uint time) public {
         this.warp(time);
         assert(block.timestamp == time);
     }
 
-    function testWarpNew(uint time) public {
+    function check_warp_New(uint time) public {
         c = new C(time);
         assert(block.timestamp == time);
     }
 
-    function testWarpReset(uint time1, uint time2) public {
+    function check_warp_Reset(uint time1, uint time2) public {
         vm.warp(time1);
         assert(block.timestamp == time1);
         vm.warp(time2);
         assert(block.timestamp == time2);
     }
 
-    function testWarpSetUp() public {
+    function check_warp_SetUp() public view {
         assert(block.timestamp == 1000);
     }
 }
```

