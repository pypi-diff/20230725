# Comparing `tmp/kingsoftcloud-sdk-python-1.1.5.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.1.5.tar", last modified: Wed Jul 19 02:15:54 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.6.tar", last modified: Tue Jul 25 11:59:15 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.1.5.tar` & `kingsoftcloud-sdk-python-1.1.6.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.158770 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 02:15:54.000000 kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.162770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80297 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   123172 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.166770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.170770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 02:15:54.174770 kingsoftcloud-sdk-python-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-19 02:15:42.000000 kingsoftcloud-sdk-python-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 11:59:15.000000 kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.499125 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51841 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45896 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85663 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126047 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.503126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.507126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.511126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 11:59:15.515126 kingsoftcloud-sdk-python-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 11:59:03.000000 kingsoftcloud-sdk-python-1.1.6/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/LICENSE` & `kingsoftcloud-sdk-python-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.5
+Version: 1.1.6
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/README.rst` & `kingsoftcloud-sdk-python-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.5
+Version: 1.1.6
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.6/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.1.5'
+__version__ = '1.1.6'
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,37 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def DetachUserPolicy(self, request):
+        """解绑IAM用户策略
+        :param request: Request instance for DetachUserPolicy.
+        :type request: :class:`ksyun.client.iam.v20151101.models.DetachUserPolicyRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DetachUserPolicy", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def ListAttachedUserPolicies(self, request):
         """查询用户附加策略列表
         :param request: Request instance for ListAttachedUserPolicies.
         :type request: :class:`ksyun.client.iam.v20151101.models.ListAttachedUserPoliciesRequest`
         """
         try:
             params = request._serialize()
@@ -1284,14 +1307,60 @@
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def InsertInstanceToES(self, request):
+        """非标实例插入es
+        :param request: Request instance for InsertInstanceToES.
+        :type request: :class:`ksyun.client.iam.v20151101.models.InsertInstanceToESRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("InsertInstanceToES", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DelInstanceFromES(self, request):
+        """删除非标实例
+        :param request: Request instance for DelInstanceFromES.
+        :type request: :class:`ksyun.client.iam.v20151101.models.DelInstanceFromESRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DelInstanceFromES", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
                 raise KsyunSDKException(code, message, req_id)
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/iam/v20151101/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,36 @@
         self.UserName = None
 
     def _deserialize(self, params):
         if params.get("UserName"):
             self.UserName = params.get("UserName")
 
 
+class DetachUserPolicyRequest(AbstractModel):
+    """DetachUserPolicy请求参数结构体
+    """
+
+    def __init__(self):
+        r"""解绑IAM用户策略
+        :param PolicyKrn: 需要解绑的策略的krn标识
+格式：krn:ksc:iam::account-id:policy/policy-name
+        :type PathPrefix: String
+        :param UserName: 需要解绑的策略的目标用户名
+        :type PathPrefix: String
+        """
+        self.PolicyKrn = None
+        self.UserName = None
+
+    def _deserialize(self, params):
+        if params.get("PolicyKrn"):
+            self.PolicyKrn = params.get("PolicyKrn")
+        if params.get("UserName"):
+            self.UserName = params.get("UserName")
+
+
 class ListAttachedUserPoliciesRequest(AbstractModel):
     """ListAttachedUserPolicies请求参数结构体
     """
 
     def __init__(self):
         r"""查询用户附加策略列表
         :param UserName: 待查询策略列表的目标用户名
@@ -507,20 +529,25 @@
     """GetLoginProfile请求参数结构体
     """
 
     def __init__(self):
         r"""查询登录配置信息
         :param UserName: 要查询的IAM子用户名称
         :type PathPrefix: String
+        :param NotCheckPassword: 
+        :type PathPrefix: Int
         """
         self.UserName = None
+        self.NotCheckPassword = None
 
     def _deserialize(self, params):
         if params.get("UserName"):
             self.UserName = params.get("UserName")
+        if params.get("NotCheckPassword"):
+            self.NotCheckPassword = params.get("NotCheckPassword")
 
 
 class CreateAccessKeyRequest(AbstractModel):
     """CreateAccessKey请求参数结构体
     """
 
     def __init__(self):
@@ -1319,7 +1346,74 @@
         r"""获取子用户ak最后使用时间
         """
 
     def _deserialize(self, params):
         return
 
 
+class InsertInstanceToESRequest(AbstractModel):
+    """InsertInstanceToES请求参数结构体
+    """
+
+    def __init__(self):
+        r"""非标实例插入es
+        :param ProjectId: 
+        :type PathPrefix: Int
+        :param ProductLine: 
+        :type PathPrefix: String
+        :param ProductGroup: 
+        :type PathPrefix: Int
+        :param ResourceType: 
+        :type PathPrefix: String
+        :param InstanceId: 
+        :type PathPrefix: String
+        :param RegionEn: 
+        :type PathPrefix: String
+        :param InstanceName: 
+        :type PathPrefix: String
+        """
+        self.ProjectId = None
+        self.ProductLine = None
+        self.ProductGroup = None
+        self.ResourceType = None
+        self.InstanceId = None
+        self.RegionEn = None
+        self.InstanceName = None
+
+    def _deserialize(self, params):
+        if params.get("ProjectId"):
+            self.ProjectId = params.get("ProjectId")
+        if params.get("ProductLine"):
+            self.ProductLine = params.get("ProductLine")
+        if params.get("ProductGroup"):
+            self.ProductGroup = params.get("ProductGroup")
+        if params.get("ResourceType"):
+            self.ResourceType = params.get("ResourceType")
+        if params.get("InstanceId"):
+            self.InstanceId = params.get("InstanceId")
+        if params.get("RegionEn"):
+            self.RegionEn = params.get("RegionEn")
+        if params.get("InstanceName"):
+            self.InstanceName = params.get("InstanceName")
+
+
+class DelInstanceFromESRequest(AbstractModel):
+    """DelInstanceFromES请求参数结构体
+    """
+
+    def __init__(self):
+        r"""删除非标实例
+        :param ProductLine: 
+        :type PathPrefix: String
+        :param InstanceId: 
+        :type PathPrefix: String
+        """
+        self.ProductLine = None
+        self.InstanceId = None
+
+    def _deserialize(self, params):
+        if params.get("ProductLine"):
+            self.ProductLine = params.get("ProductLine")
+        if params.get("InstanceId"):
+            self.InstanceId = params.get("InstanceId")
+
+
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -648,14 +648,37 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def DeleteDedicatedHost(self, request):
+        """删除专属宿主机
+        :param request: Request instance for DeleteDedicatedHost.
+        :type request: :class:`ksyun.client.kec.v20160304.models.DeleteDedicatedHostRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DeleteDedicatedHost", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def RenameDedicatedHost(self, request):
         """修改专属宿主机名称
         :param request: Request instance for RenameDedicatedHost.
         :type request: :class:`ksyun.client.kec.v20160304.models.RenameDedicatedHostRequest`
         """
         try:
             params = request._serialize()
@@ -1338,14 +1361,60 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def DescribeImageSharePermission(self, request):
+        """镜像共享的账户列表
+        :param request: Request instance for DescribeImageSharePermission.
+        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeImageSharePermissionRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DescribeImageSharePermission", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DescribeRegions(self, request):
+        """用户有权限机房
+        :param request: Request instance for DescribeRegions.
+        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeRegionsRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DescribeRegions", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def AttachKey(self, request):
         """主机绑定密钥
         :param request: Request instance for AttachKey.
         :type request: :class:`ksyun.client.kec.v20160304.models.AttachKeyRequest`
         """
         try:
             params = request._serialize()
@@ -1384,14 +1453,37 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def DescribeAvailabilityZones(self, request):
+        """查询可用区列表
+        :param request: Request instance for DescribeAvailabilityZones.
+        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeAvailabilityZonesRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DescribeAvailabilityZones", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def DescribeInstanceTypeConfigs(self, request):
         """查询机型套餐配置信息
         :param request: Request instance for DescribeInstanceTypeConfigs.
         :type request: :class:`ksyun.client.kec.v20160304.models.DescribeInstanceTypeConfigsRequest`
         """
         try:
             params = request._serialize()
@@ -1821,14 +1913,37 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def InstanceMigrate(self, request):
+        """专属虚机迁移
+        :param request: Request instance for InstanceMigrate.
+        :type request: :class:`ksyun.client.kec.v20160304.models.InstanceMigrateRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("InstanceMigrate", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def ModifyInstanceAutoDeleteTime(self, request):
         """实例定时删除
         :param request: Request instance for ModifyInstanceAutoDeleteTime.
         :type request: :class:`ksyun.client.kec.v20160304.models.ModifyInstanceAutoDeleteTimeRequest`
         """
         try:
             params = request._serialize()
@@ -2066,14 +2181,37 @@
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DescribeMinFlavorCount(self, request):
+        """DescribeMinFlavorCount
+        :param request: Request instance for DescribeMinFlavorCount.
+        :type request: :class:`ksyun.client.kec.v20160304.models.DescribeMinFlavorCountRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call("DescribeMinFlavorCount", params)
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
                 raise KsyunSDKException(code, message, req_id)
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kec/v20160304/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -963,14 +963,35 @@
             self.InstanceNameSuffix = params.get("InstanceNameSuffix")
         if params.get("DedicatedClusterId"):
             self.DedicatedClusterId = params.get("DedicatedClusterId")
         if params.get("Tag"):
             self.Tag = params.get("Tag")
 
 
+class DeleteDedicatedHostRequest(AbstractModel):
+    """DeleteDedicatedHost请求参数结构体
+    """
+
+    def __init__(self):
+        r"""删除专属宿主机
+        :param DedicatedHostId: 专属宿主机id
+        :type PathPrefix: Filter
+        :param IsRefund: 是否退订(默认true）
+        :type PathPrefix: Boolean
+        """
+        self.DedicatedHostId = None
+        self.IsRefund = None
+
+    def _deserialize(self, params):
+        if params.get("DedicatedHostId"):
+            self.DedicatedHostId = params.get("DedicatedHostId")
+        if params.get("IsRefund"):
+            self.IsRefund = params.get("IsRefund")
+
+
 class RenameDedicatedHostRequest(AbstractModel):
     """RenameDedicatedHost请求参数结构体
     """
 
     def __init__(self):
         r"""修改专属宿主机名称
         :param DedicatedHostId: 专属宿主机id
@@ -2097,14 +2118,43 @@
             self.ImageId = params.get("ImageId")
         if params.get("AccountId"):
             self.AccountId = params.get("AccountId")
         if params.get("Permission"):
             self.Permission = params.get("Permission")
 
 
+class DescribeImageSharePermissionRequest(AbstractModel):
+    """DescribeImageSharePermission请求参数结构体
+    """
+
+    def __init__(self):
+        r"""镜像共享的账户列表
+        :param ImageId: 共享的镜像ID。
+标准UUID格式，形如^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$
+        :type PathPrefix: String
+        """
+        self.ImageId = None
+
+    def _deserialize(self, params):
+        if params.get("ImageId"):
+            self.ImageId = params.get("ImageId")
+
+
+class DescribeRegionsRequest(AbstractModel):
+    """DescribeRegions请求参数结构体
+    """
+
+    def __init__(self):
+        r"""用户有权限机房
+        """
+
+    def _deserialize(self, params):
+        return
+
+
 class AttachKeyRequest(AbstractModel):
     """AttachKey请求参数结构体
     """
 
     def __init__(self):
         r"""主机绑定密钥
         :param Action: 动作
@@ -2153,14 +2203,26 @@
             self.Action = params.get("Action")
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
         if params.get("KeyId"):
             self.KeyId = params.get("KeyId")
 
 
+class DescribeAvailabilityZonesRequest(AbstractModel):
+    """DescribeAvailabilityZones请求参数结构体
+    """
+
+    def __init__(self):
+        r"""查询可用区列表
+        """
+
+    def _deserialize(self, params):
+        return
+
+
 class DescribeInstanceTypeConfigsRequest(AbstractModel):
     """DescribeInstanceTypeConfigs请求参数结构体
     """
 
     def __init__(self):
         r"""查询机型套餐配置信息
         """
@@ -2693,14 +2755,45 @@
     def _deserialize(self, params):
         if params.get("DedicatedClusterId"):
             self.DedicatedClusterId = params.get("DedicatedClusterId")
         if params.get("DedicatedClusterName"):
             self.DedicatedClusterName = params.get("DedicatedClusterName")
 
 
+class InstanceMigrateRequest(AbstractModel):
+    """InstanceMigrate请求参数结构体
+    """
+
+    def __init__(self):
+        r"""专属虚机迁移
+        :param DedicatedHostId: 专属宿主机id
+        :type PathPrefix: String
+        :param InstanceId: 虚拟机ID
+        :type PathPrefix: String
+        :param InstanceType: 套餐类型
+        :type PathPrefix: String
+        :param DataDisk: 数据盘id
+        :type PathPrefix: Filter
+        """
+        self.DedicatedHostId = None
+        self.InstanceId = None
+        self.InstanceType = None
+        self.DataDisk = None
+
+    def _deserialize(self, params):
+        if params.get("DedicatedHostId"):
+            self.DedicatedHostId = params.get("DedicatedHostId")
+        if params.get("InstanceId"):
+            self.InstanceId = params.get("InstanceId")
+        if params.get("InstanceType"):
+            self.InstanceType = params.get("InstanceType")
+        if params.get("DataDisk"):
+            self.DataDisk = params.get("DataDisk")
+
+
 class ModifyInstanceAutoDeleteTimeRequest(AbstractModel):
     """ModifyInstanceAutoDeleteTime请求参数结构体
     """
 
     def __init__(self):
         r"""实例定时删除
         :param InstanceId: 待重启实例ID列表，N的范围为1-100
@@ -3106,7 +3199,19 @@
         self.InstanceId = None
 
     def _deserialize(self, params):
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
 
 
+class DescribeMinFlavorCountRequest(AbstractModel):
+    """DescribeMinFlavorCount请求参数结构体
+    """
+
+    def __init__(self):
+        r"""DescribeMinFlavorCount
+        """
+
+    def _deserialize(self, params):
+        return
+
+
```

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/kls/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/kls/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20100525/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20100525/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20210101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20210101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/monitor/v20220101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/monitor/v20220101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/slb/v20171210/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/slb/v20171210/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.6/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.5/setup.py` & `kingsoftcloud-sdk-python-1.1.6/setup.py`

 * *Files identical despite different names*

