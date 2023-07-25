# Comparing `tmp/flumine-2.4.0.tar.gz` & `tmp/flumine-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flumine-2.4.0.tar", last modified: Mon Jul 24 10:17:30 2023, max compression
+gzip compressed data, was "dist/flumine-2.4.1.tar", last modified: Tue Jul 25 07:29:30 2023, max compression
```

## Comparing `flumine-2.4.0.tar` & `flumine-2.4.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 10:17:30.000000 flumine-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-24 10:17:12.000000 flumine-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/baseflumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/betconnectclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/betfairclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/clients/simulatedclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/controls/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/controls/tradingcontrols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/baseexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/betfairexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/simulatedexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/execution/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/flumine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/markets/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/order/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/strategy/runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/strategy/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/basestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/historicalstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/marketstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/orderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/simulatedorderstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/sportsdatastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-24 10:17:12.000000 flumine-2.4.0/flumine/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 10:17:30.000000 flumine-2.4.0/flumine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:17:30.000000 flumine-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 10:17:12.000000 flumine-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:30.000000 flumine-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_baseflumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_blotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_clientcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_flumine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_fluminesimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_loggingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_orderpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_ordertype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_runnercontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_simulated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    61695 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_simulatedorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_tradingcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-24 10:17:12.000000 flumine-2.4.0/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-25 07:29:30.000000 flumine-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-25 07:29:04.000000 flumine-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/baseflumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/betconnectclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/betfairclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/clients/simulatedclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/controls/tradingcontrols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/baseexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/betfairexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/simulatedexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/execution/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/flumine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14302 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/markets/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/order/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/strategy/runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/strategy/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/basestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/historicalstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/marketstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/orderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/simulatedorderstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/sportsdatastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-25 07:29:04.000000 flumine-2.4.1/flumine/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 07:29:30.000000 flumine-2.4.1/flumine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:29:30.000000 flumine-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 07:29:04.000000 flumine-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:30.000000 flumine-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_baseflumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_blotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_clientcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63899 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_flumine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_fluminesimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_loggingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_orderpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_ordertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_runnercontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_simulated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61695 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_simulatedorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40617 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_tradingcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-25 07:29:04.000000 flumine-2.4.1/tests/test_worker.py
```

### Comparing `flumine-2.4.0/PKG-INFO` & `flumine-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.4.0
+Version: 2.4.1
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.4.0 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.4.1 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.4.0/README.md` & `flumine-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/__init__.py` & `flumine-2.4.1/flumine/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/baseflumine.py` & `flumine-2.4.1/flumine/baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/clients/baseclient.py` & `flumine-2.4.1/flumine/clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/clients/betconnectclient.py` & `flumine-2.4.1/flumine/clients/betconnectclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/clients/betfairclient.py` & `flumine-2.4.1/flumine/clients/betfairclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/clients/clients.py` & `flumine-2.4.1/flumine/clients/clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/clients/simulatedclient.py` & `flumine-2.4.1/flumine/clients/simulatedclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/config.py` & `flumine-2.4.1/flumine/config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/controls/__init__.py` & `flumine-2.4.1/flumine/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/controls/clientcontrols.py` & `flumine-2.4.1/flumine/controls/clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/controls/loggingcontrols.py` & `flumine-2.4.1/flumine/controls/loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/controls/tradingcontrols.py` & `flumine-2.4.1/flumine/controls/tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/events/events.py` & `flumine-2.4.1/flumine/events/events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/exceptions.py` & `flumine-2.4.1/flumine/exceptions.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/execution/baseexecution.py` & `flumine-2.4.1/flumine/execution/baseexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/execution/betfairexecution.py` & `flumine-2.4.1/flumine/execution/betfairexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/execution/simulatedexecution.py` & `flumine-2.4.1/flumine/execution/simulatedexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/execution/transaction.py` & `flumine-2.4.1/flumine/execution/transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/flumine.py` & `flumine-2.4.1/flumine/flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/markets/blotter.py` & `flumine-2.4.1/flumine/markets/blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/markets/market.py` & `flumine-2.4.1/flumine/markets/market.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/markets/markets.py` & `flumine-2.4.1/flumine/markets/markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/markets/middleware.py` & `flumine-2.4.1/flumine/markets/middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/order/order.py` & `flumine-2.4.1/flumine/order/order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/order/orderpackage.py` & `flumine-2.4.1/flumine/order/orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/order/ordertype.py` & `flumine-2.4.1/flumine/order/ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/order/process.py` & `flumine-2.4.1/flumine/order/process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/order/responses.py` & `flumine-2.4.1/flumine/order/responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/order/trade.py` & `flumine-2.4.1/flumine/order/trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/patching.py` & `flumine-2.4.1/flumine/patching.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/simulation/simulatedorder.py` & `flumine-2.4.1/flumine/simulation/simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/simulation/simulation.py` & `flumine-2.4.1/flumine/simulation/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
 
             if market_book.status == "CLOSED":
                 self._process_close_market(event=events.CloseMarketEvent(market_book))
                 continue
 
             # get market
             market = self.markets.markets.get(market_id)
-            if market is None:
+            market_is_new = market is None
+            if market_is_new:
                 market = self._add_market(market_id, market_book)
                 self.log_control(events.MarketEvent(market))
             elif market.closed:
                 self.markets.add_market(market_id, market)
 
             # process market
             market(market_book)
@@ -136,14 +137,18 @@
                 utils.call_middleware_error_handling(middleware, market)
 
             # process current orders
             if market.blotter.active:
                 self._process_simulated_orders(market)
 
             for strategy in self.strategies:
+                if market_is_new:
+                    utils.call_strategy_error_handling(
+                        strategy.process_new_market, market, market_book
+                    )
                 if utils.call_strategy_error_handling(
                     strategy.check_market, market, market_book
                 ):
                     utils.call_strategy_error_handling(
                         strategy.process_market_book, market, market_book
                     )
```

### Comparing `flumine-2.4.0/flumine/simulation/utils.py` & `flumine-2.4.1/flumine/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/strategy/runnercontext.py` & `flumine-2.4.1/flumine/strategy/runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/strategy/strategy.py` & `flumine-2.4.1/flumine/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/basestream.py` & `flumine-2.4.1/flumine/streams/basestream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/datastream.py` & `flumine-2.4.1/flumine/streams/datastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/historicalstream.py` & `flumine-2.4.1/flumine/streams/historicalstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/marketstream.py` & `flumine-2.4.1/flumine/streams/marketstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/orderstream.py` & `flumine-2.4.1/flumine/streams/orderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/simulatedorderstream.py` & `flumine-2.4.1/flumine/streams/simulatedorderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/sportsdatastream.py` & `flumine-2.4.1/flumine/streams/sportsdatastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/streams/streams.py` & `flumine-2.4.1/flumine/streams/streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/utils.py` & `flumine-2.4.1/flumine/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine/worker.py` & `flumine-2.4.1/flumine/worker.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/flumine.egg-info/PKG-INFO` & `flumine-2.4.1/flumine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flumine
-Version: 2.4.0
+Version: 2.4.1
 Summary: Betting trading framework
 Home-page: https://github.com/betcode-org/flumine
 Author: Liam Pauling
 Author-email: a@unknown.com
 License: MIT
 Description: <p align="center">
           <a href="https://github.com/betcode-org">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flumine Version: 2.4.0 Summary: Betting trading
+Metadata-Version: 2.1 Name: flumine Version: 2.4.1 Summary: Betting trading
 framework Home-page: https://github.com/betcode-org/flumine Author: Liam
 Pauling Author-email: a@unknown.com License: MIT Description:
                           [docs/images/logo-full.png]
 # flÅ«mine ![Build Status](https://github.com/betcode-org/flumine/actions/
 workflows/test.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/
 github/liampauling/flumine/badge.svg?branch=master)](https://coveralls.io/
 github/liampauling/flumine?branch=master) [![PyPI version](https://
```

### Comparing `flumine-2.4.0/flumine.egg-info/SOURCES.txt` & `flumine-2.4.1/flumine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/setup.py` & `flumine-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_baseflumine.py` & `flumine-2.4.1/tests/test_baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_blotter.py` & `flumine-2.4.1/tests/test_blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_clientcontrols.py` & `flumine-2.4.1/tests/test_clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_clients.py` & `flumine-2.4.1/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_config.py` & `flumine-2.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_events.py` & `flumine-2.4.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_execution.py` & `flumine-2.4.1/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_flumine.py` & `flumine-2.4.1/tests/test_flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_fluminesimulation.py` & `flumine-2.4.1/tests/test_fluminesimulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from flumine.clients import ExchangeType
 from flumine.order.orderpackage import OrderPackageType
 from flumine import config
 from flumine.exceptions import RunError
 from flumine.order.trade import TradeStatus
 from flumine.markets.blotter import Blotter
 from flumine.order.order import OrderTypes
+from flumine.markets.market import Market
 
 
 class FlumineSimulationTest(unittest.TestCase):
     def setUp(self):
         self.mock_client = mock.Mock(EXCHANGE=ExchangeType.SIMULATED)
         self.flumine = FlumineSimulation(self.mock_client)
 
@@ -88,14 +89,34 @@
         mock_market.blotter.live_orders = []
         self.flumine.markets._markets = {"1.23": mock_market}
         mock_event.event = [mock_market_book]
         self.flumine._process_market_books(mock_event)
         mock__check_pending_packages.assert_called_with("1.23")
         mock__process_simulated_orders.assert_called_with(mock_market)
 
+    def test__process_market_books_new_market(self):
+        mock_strategy = mock.Mock()
+        self.flumine.add_strategy(mock_strategy)
+        mock_market_book = mock.Mock(market_id="1.23")
+        mock_market_book.runners = []
+        mock_event = mock.Mock()
+        mock_event.event = [mock_market_book]
+        for call_count in range(1, 5):
+            # process_new_market must be called only once, the first time
+            with self.subTest(call_count=call_count):
+                self.flumine._process_market_books(mock_event)
+                mock_strategy.process_new_market.assert_called_once()
+                self.assertEqual(
+                    mock_strategy.process_market_book.call_count, call_count
+                )
+        market, market_book = mock_strategy.process_new_market.call_args[0]
+        self.assertIs(market_book, mock_market_book)
+        self.assertIsInstance(market, Market)
+        self.assertIs(market.market_book, mock_market_book)
+
     def test_process_order_package(self):
         mock_order_package = mock.Mock()
         self.flumine.process_order_package(mock_order_package)
         self.assertEqual(self.flumine.handler_queue, [mock_order_package])
 
     def test__process_simulated_orders(self):
         mock_market = mock.Mock(context={})
```

### Comparing `flumine-2.4.0/tests/test_integration.py` & `flumine-2.4.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_loggingcontrols.py` & `flumine-2.4.1/tests/test_loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_markets.py` & `flumine-2.4.1/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_middleware.py` & `flumine-2.4.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_order.py` & `flumine-2.4.1/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_orderpackage.py` & `flumine-2.4.1/tests/test_orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_ordertype.py` & `flumine-2.4.1/tests/test_ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_process.py` & `flumine-2.4.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_responses.py` & `flumine-2.4.1/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_runnercontext.py` & `flumine-2.4.1/tests/test_runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_simulated_utils.py` & `flumine-2.4.1/tests/test_simulated_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_simulatedorder.py` & `flumine-2.4.1/tests/test_simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_strategy.py` & `flumine-2.4.1/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_streams.py` & `flumine-2.4.1/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_trade.py` & `flumine-2.4.1/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_tradingcontrols.py` & `flumine-2.4.1/tests/test_tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_transaction.py` & `flumine-2.4.1/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_utils.py` & `flumine-2.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.4.0/tests/test_worker.py` & `flumine-2.4.1/tests/test_worker.py`

 * *Files identical despite different names*

