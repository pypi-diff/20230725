# Comparing `tmp/bilirpc-1.1.tar.gz` & `tmp/bilirpc-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilirpc-1.1.tar", max compression
+gzip compressed data, was "bilirpc-1.2.tar", max compression
```

## Comparing `bilirpc-1.1.tar` & `bilirpc-1.2.tar`

### file list

```diff
@@ -1,373 +1,373 @@
--rw-r--r--   0        0        0        0 2023-07-25 12:46:23.607515 bilirpc-1.1/README.md
--rw-r--r--   0        0        0      174 2023-07-24 13:18:16.061240 bilirpc-1.1/bilirpc/__init__.py
--rw-r--r--   0        0        0     2985 2023-07-25 12:45:54.735334 bilirpc-1.1/bilirpc/api.py
--rw-r--r--   0        0        0        0 2023-07-24 14:30:21.919272 bilirpc-1.1/bilirpc/bilibili/__init__.py
--rw-r--r--   0        0        0      140 2023-07-24 14:30:40.423299 bilirpc-1.1/bilirpc/bilibili/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1150 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/account/fission/v1/fission.proto
--rw-r--r--   0        0        0     2663 2023-07-24 13:51:03.340765 bilirpc-1.1/bilirpc/bilibili/account/fission/v1/fission_pb2.py
--rw-r--r--   0        0        0     6044 2023-07-24 13:51:03.340765 bilirpc-1.1/bilirpc/bilibili/account/fission/v1/fission_pb2_grpc.py
--rw-r--r--   0        0        0    19936 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/ad/v1/ad.proto
--rw-r--r--   0        0        0    25729 2023-07-24 13:51:41.504880 bilirpc-1.1/bilirpc/bilibili/ad/v1/ad_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:51:41.504880 bilirpc-1.1/bilirpc/bilibili/ad/v1/ad_pb2_grpc.py
--rw-r--r--   0        0        0     1308 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/api/player/v1/player.proto
--rw-r--r--   0        0        0     2587 2023-07-24 13:52:06.044955 bilirpc-1.1/bilirpc/bilibili/api/player/v1/player_pb2.py
--rw-r--r--   0        0        0     2572 2023-07-24 13:52:06.044955 bilirpc-1.1/bilirpc/bilibili/api/player/v1/player_pb2_grpc.py
--rw-r--r--   0        0        0     3131 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/api/probe/v1/probe.proto
--rw-r--r--   0        0        0     7021 2023-07-24 13:52:42.613071 bilirpc-1.1/bilirpc/bilibili/api/probe/v1/probe_pb2.py
--rw-r--r--   0        0        0    16584 2023-07-24 13:52:42.613071 bilirpc-1.1/bilirpc/bilibili/api/probe/v1/probe_pb2_grpc.py
--rw-r--r--   0        0        0     1040 2023-07-24 15:00:59.453756 bilirpc-1.1/bilirpc/bilibili/app/archive/middleware/v1/__pycache__/preload_pb2.cpython-310.pyc
--rw-r--r--   0        0        0      394 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/archive/middleware/v1/preload.proto
--rw-r--r--   0        0        0     1277 2023-07-24 13:53:50.333291 bilirpc-1.1/bilirpc/bilibili/app/archive/middleware/v1/preload_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:53:50.333291 bilirpc-1.1/bilirpc/bilibili/app/archive/middleware/v1/preload_pb2_grpc.py
--rw-r--r--   0        0        0     3869 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/archive/v1/archive.proto
--rw-r--r--   0        0        0     5206 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/archive/v1/archive_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/archive/v1/archive_pb2_grpc.py
--rw-r--r--   0        0        0      982 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/card/v1/ad.proto
--rw-r--r--   0        0        0     2256 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/ad_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/ad_pb2_grpc.py
--rw-r--r--   0        0        0      777 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/card/v1/card.proto
--rw-r--r--   0        0        0     2150 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/card_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/card_pb2_grpc.py
--rw-r--r--   0        0        0     5488 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/card/v1/common.proto
--rw-r--r--   0        0        0     9216 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/common_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     6786 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/card/v1/double.proto
--rw-r--r--   0        0        0    12871 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/double_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/double_pb2_grpc.py
--rw-r--r--   0        0        0     6404 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/card/v1/single.proto
--rw-r--r--   0        0        0    10607 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/single_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/card/v1/single_pb2_grpc.py
--rw-r--r--   0        0        0     1746 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/click/v1/heartbeat.proto
--rw-r--r--   0        0        0     3956 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/click/v1/heartbeat_pb2.py
--rw-r--r--   0        0        0      876 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/click/v1/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0      263 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/download.proto
--rw-r--r--   0        0        0     1411 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/download_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/download_pb2_grpc.py
--rw-r--r--   0        0        0      321 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/dynamic.proto
--rw-r--r--   0        0        0     1607 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/dynamic_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/dynamic_pb2_grpc.py
--rw-r--r--   0        0        0     1729 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/experimental.proto
--rw-r--r--   0        0        0     3644 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/experimental_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/experimental_pb2_grpc.py
--rw-r--r--   0        0        0      263 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/internaldevice.proto
--rw-r--r--   0        0        0     1412 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/internaldevice_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/internaldevice_pb2_grpc.py
--rw-r--r--   0        0        0      253 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/night.proto
--rw-r--r--   0        0        0     1381 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/night_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/night_pb2_grpc.py
--rw-r--r--   0        0        0      818 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/other.proto
--rw-r--r--   0        0        0     2071 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/other_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/other_pb2_grpc.py
--rw-r--r--   0        0        0      936 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/pegasus.proto
--rw-r--r--   0        0        0     2657 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/pegasus_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/pegasus_pb2_grpc.py
--rw-r--r--   0        0        0     1961 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/play.proto
--rw-r--r--   0        0        0     3444 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/play_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/play_pb2_grpc.py
--rw-r--r--   0        0        0      465 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/privacy.proto
--rw-r--r--   0        0        0     1741 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/privacy_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/privacy_pb2_grpc.py
--rw-r--r--   0        0        0      399 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/search.proto
--rw-r--r--   0        0        0     1711 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/search_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/search_pb2_grpc.py
--rw-r--r--   0        0        0     2721 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/distribution/v1/distribution.proto
--rw-r--r--   0        0        0     6193 2023-07-24 14:08:26.245264 bilirpc-1.1/bilirpc/bilibili/app/distribution/v1/distribution_pb2.py
--rw-r--r--   0        0        0     6610 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/distribution/v1/distribution_pb2_grpc.py
--rw-r--r--   0        0        0      293 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/dynamic/common/dynamic.proto
--rw-r--r--   0        0        0     1419 2023-07-24 13:57:43.678110 bilirpc-1.1/bilirpc/bilibili/app/dynamic/common/dynamic_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:57:43.678110 bilirpc-1.1/bilirpc/bilibili/app/dynamic/common/dynamic_pb2_grpc.py
--rw-r--r--   0        0        0    21326 2023-07-24 15:00:59.449756 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     8807 2023-07-24 15:00:59.453756 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0    29817 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/dynamic.proto
--rw-r--r--   0        0        0    37877 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2.py
--rw-r--r--   0        0        0    23606 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2_grpc.py
--rw-r--r--   0        0        0   100695 2023-07-24 14:30:40.431299 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    31191 2023-07-24 14:30:40.451299 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0     1282 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/campus.proto
--rw-r--r--   0        0        0     3927 2023-07-24 13:58:26.402268 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/campus_pb2.py
--rw-r--r--   0        0        0     2728 2023-07-24 13:58:26.402268 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/campus_pb2_grpc.py
--rw-r--r--   0        0        0   117183 2023-07-24 13:04:02.811851 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/dynamic.proto
--rw-r--r--   0        0        0   172974 2023-07-24 13:58:26.402268 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2.py
--rw-r--r--   0        0        0    99325 2023-07-24 13:58:26.402268 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2_grpc.py
--rw-r--r--   0        0        0      962 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/opus.proto
--rw-r--r--   0        0        0     2908 2023-07-24 13:58:26.402268 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/opus_pb2.py
--rw-r--r--   0        0        0     2659 2023-07-24 13:58:26.402268 bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/opus_pb2_grpc.py
--rw-r--r--   0        0        0     8157 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/history.proto
--rw-r--r--   0        0        0    11002 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/history_pb2.py
--rw-r--r--   0        0        0    12971 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/history_pb2_grpc.py
--rw-r--r--   0        0        0     4599 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/media.proto
--rw-r--r--   0        0        0    10030 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/media_pb2.py
--rw-r--r--   0        0        0     9477 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/media_pb2_grpc.py
--rw-r--r--   0        0        0     3565 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/search.proto
--rw-r--r--   0        0        0     5394 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/search_pb2.py
--rw-r--r--   0        0        0     6746 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/search_pb2_grpc.py
--rw-r--r--   0        0        0     1612 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/space.proto
--rw-r--r--   0        0        0     4295 2023-07-24 14:08:26.249264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/space_pb2.py
--rw-r--r--   0        0        0     6061 2023-07-24 14:08:26.297264 bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/space_pb2_grpc.py
--rw-r--r--   0        0        0    19736 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/listener/v1/listener.proto
--rw-r--r--   0        0        0    40528 2023-07-24 14:08:26.297264 bilirpc-1.1/bilirpc/bilibili/app/listener/v1/listener_pb2.py
--rw-r--r--   0        0        0    58680 2023-07-24 14:08:26.297264 bilirpc-1.1/bilirpc/bilibili/app/listener/v1/listener_pb2_grpc.py
--rw-r--r--   0        0        0    28703 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/nativeact/v1/nativeact.proto
--rw-r--r--   0        0        0    51641 2023-07-24 14:08:26.297264 bilirpc-1.1/bilirpc/bilibili/app/nativeact/v1/nativeact_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/nativeact/v1/nativeact_pb2_grpc.py
--rw-r--r--   0        0        0     1200 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/playeronline/v1/playeronline.proto
--rw-r--r--   0        0        0     2911 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2.py
--rw-r--r--   0        0        0     6366 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2_grpc.py
--rw-r--r--   0        0        0      482 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel.proto
--rw-r--r--   0        0        0     1741 2023-07-24 14:00:45.226794 bilirpc-1.1/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:00:45.226794 bilirpc-1.1/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel_pb2_grpc.py
--rw-r--r--   0        0        0      471 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel.proto
--rw-r--r--   0        0        0     2046 2023-07-24 14:01:01.518857 bilirpc-1.1/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:01:01.518857 bilirpc-1.1/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel_pb2_grpc.py
--rw-r--r--   0        0        0     1171 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/playerunite/v1/playerunite.proto
--rw-r--r--   0        0        0     2969 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2.py
--rw-r--r--   0        0        0     2723 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2_grpc.py
--rw-r--r--   0        0        0    15390 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/playurl/v1/playurl.proto
--rw-r--r--   0        0        0    22028 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/playurl/v1/playurl_pb2.py
--rw-r--r--   0        0        0     9424 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/playurl/v1/playurl_pb2_grpc.py
--rw-r--r--   0        0        0     1170 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/resource/privacy/v1/api.proto
--rw-r--r--   0        0        0     3009 2023-07-24 14:02:05.011104 bilirpc-1.1/bilirpc/bilibili/app/resource/privacy/v1/api_pb2.py
--rw-r--r--   0        0        0     4565 2023-07-24 14:02:05.011104 bilirpc-1.1/bilirpc/bilibili/app/resource/privacy/v1/api_pb2_grpc.py
--rw-r--r--   0        0        0     1941 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/resource/v1/module.proto
--rw-r--r--   0        0        0     4261 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/resource/v1/module_pb2.py
--rw-r--r--   0        0        0     2472 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/resource/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1692 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/search/v2/search.proto
--rw-r--r--   0        0        0     4015 2023-07-24 14:06:08.586608 bilirpc-1.1/bilirpc/bilibili/app/search/v2/search_pb2.py
--rw-r--r--   0        0        0     8029 2023-07-24 14:06:08.586608 bilirpc-1.1/bilirpc/bilibili/app/search/v2/search_pb2_grpc.py
--rw-r--r--   0        0        0      546 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/show/gateway/v1/service.proto
--rw-r--r--   0        0        0     1804 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/gateway/v1/service_pb2.py
--rw-r--r--   0        0        0     2716 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/gateway/v1/service_pb2_grpc.py
--rw-r--r--   0        0        0      754 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/show/mixture/v1/mixture.proto
--rw-r--r--   0        0        0     2216 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2.py
--rw-r--r--   0        0        0     2589 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2_grpc.py
--rw-r--r--   0        0        0     2470 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/show/popular/v1/popular.proto
--rw-r--r--   0        0        0     3741 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/popular/v1/popular_pb2.py
--rw-r--r--   0        0        0     2608 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/popular/v1/popular_pb2_grpc.py
--rw-r--r--   0        0        0     2478 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/show/rank/v1/rank.proto
--rw-r--r--   0        0        0     3522 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/rank/v1/rank_pb2.py
--rw-r--r--   0        0        0     4316 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/rank/v1/rank_pb2_grpc.py
--rw-r--r--   0        0        0      734 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/show/region/v1/region.proto
--rw-r--r--   0        0        0     2301 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/region/v1/region_pb2.py
--rw-r--r--   0        0        0     2559 2023-07-24 14:07:39.765669 bilirpc-1.1/bilirpc/bilibili/app/show/region/v1/region_pb2_grpc.py
--rw-r--r--   0        0        0     1504 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/space/v1/space.proto
--rw-r--r--   0        0        0     3424 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/space/v1/space_pb2.py
--rw-r--r--   0        0        0     2463 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/space/v1/space_pb2_grpc.py
--rw-r--r--   0        0        0     2031 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/splash/v1/splash.proto
--rw-r--r--   0        0        0     3833 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/splash/v1/splash_pb2.py
--rw-r--r--   0        0        0     2462 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/splash/v1/splash_pb2_grpc.py
--rw-r--r--   0        0        0     9159 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/topic/v1/topic.proto
--rw-r--r--   0        0        0    17394 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/topic/v1/topic_pb2.py
--rw-r--r--   0        0        0     6076 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/topic/v1/topic_pb2_grpc.py
--rw-r--r--   0        0        0    49304 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/view/v1/view.proto
--rw-r--r--   0        0        0    72369 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/view/v1/view_pb2.py
--rw-r--r--   0        0        0    35019 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/view/v1/view_pb2_grpc.py
--rw-r--r--   0        0        0      170 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/viewunite/pgcanymodel.proto
--rw-r--r--   0        0        0     1144 2023-07-24 14:08:44.349119 bilirpc-1.1/bilirpc/bilibili/app/viewunite/pgcanymodel_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:44.349119 bilirpc-1.1/bilirpc/bilibili/app/viewunite/pgcanymodel_pb2_grpc.py
--rw-r--r--   0        0        0      110 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/viewunite/ugcanymodel.proto
--rw-r--r--   0        0        0     1061 2023-07-24 14:08:44.349119 bilirpc-1.1/bilirpc/bilibili/app/viewunite/ugcanymodel_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:08:44.349119 bilirpc-1.1/bilirpc/bilibili/app/viewunite/ugcanymodel_pb2_grpc.py
--rw-r--r--   0        0        0     8800 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/viewunite/v1/viewunite.proto
--rw-r--r--   0        0        0    15661 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2.py
--rw-r--r--   0        0        0     4369 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2_grpc.py
--rw-r--r--   0        0        0      831 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/app/wall/v1/wall.proto
--rw-r--r--   0        0        0     2301 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/wall/v1/wall_pb2.py
--rw-r--r--   0        0        0     2501 2023-07-24 14:08:26.301264 bilirpc-1.1/bilirpc/bilibili/app/wall/v1/wall_pb2_grpc.py
--rw-r--r--   0        0        0      644 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/editor/notify.proto
--rw-r--r--   0        0        0     1745 2023-07-24 14:11:23.684094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/editor/notify_pb2.py
--rw-r--r--   0        0        0     2694 2023-07-24 14:11:23.684094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/editor/notify_pb2_grpc.py
--rw-r--r--   0        0        0      114 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/esports/notify.proto
--rw-r--r--   0        0        0     1114 2023-07-24 14:11:23.684094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/esports/notify_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/esports/notify_pb2_grpc.py
--rw-r--r--   0        0        0      320 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/fission/notify.proto
--rw-r--r--   0        0        0     1505 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/fission/notify_pb2.py
--rw-r--r--   0        0        0     2638 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/fission/notify_pb2_grpc.py
--rw-r--r--   0        0        0     2001 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/im/notify.proto
--rw-r--r--   0        0        0     3351 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/im/notify_pb2.py
--rw-r--r--   0        0        0     2580 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/im/notify_pb2_grpc.py
--rw-r--r--   0        0        0     1239 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/dm.proto
--rw-r--r--   0        0        0     2245 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/dm_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/dm_pb2_grpc.py
--rw-r--r--   0        0        0      668 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/native.proto
--rw-r--r--   0        0        0     1882 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/native_pb2.py
--rw-r--r--   0        0        0     2642 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/native_pb2_grpc.py
--rw-r--r--   0        0        0     1262 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/resource.proto
--rw-r--r--   0        0        0     2476 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/resource_pb2.py
--rw-r--r--   0        0        0     2641 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/resource_pb2_grpc.py
--rw-r--r--   0        0        0      529 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/search.proto
--rw-r--r--   0        0        0     1974 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/search_pb2.py
--rw-r--r--   0        0        0     2820 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/search_pb2_grpc.py
--rw-r--r--   0        0        0      162 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/note/sync.proto
--rw-r--r--   0        0        0     1124 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/note/sync_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/note/sync_pb2_grpc.py
--rw-r--r--   0        0        0     4914 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/freya.proto
--rw-r--r--   0        0        0     7508 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/freya_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/freya_pb2_grpc.py
--rw-r--r--   0        0        0     1004 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/live.proto
--rw-r--r--   0        0        0     2170 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/live_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/live_pb2_grpc.py
--rw-r--r--   0        0        0      306 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ticket/activitygame.proto
--rw-r--r--   0        0        0     1417 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ticket/activitygame_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/ticket/activitygame_pb2_grpc.py
--rw-r--r--   0        0        0     1727 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/message/tv/proj.proto
--rw-r--r--   0        0        0     2948 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/tv/proj_pb2.py
--rw-r--r--   0        0        0     9106 2023-07-24 14:11:23.688094 bilirpc-1.1/bilirpc/bilibili/broadcast/message/tv/proj_pb2_grpc.py
--rw-r--r--   0        0        0     3051 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/broadcast.proto
--rw-r--r--   0        0        0     3962 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/broadcast_pb2.py
--rw-r--r--   0        0        0    11798 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/broadcast_pb2_grpc.py
--rw-r--r--   0        0        0      380 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/laser.proto
--rw-r--r--   0        0        0     1456 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/laser_pb2.py
--rw-r--r--   0        0        0     2604 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/laser_pb2_grpc.py
--rw-r--r--   0        0        0      446 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/mod.proto
--rw-r--r--   0        0        0     1630 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/mod_pb2.py
--rw-r--r--   0        0        0     2575 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/mod_pb2_grpc.py
--rw-r--r--   0        0        0     2721 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/push.proto
--rw-r--r--   0        0        0     4288 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/push_pb2.py
--rw-r--r--   0        0        0     2560 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/push_pb2_grpc.py
--rw-r--r--   0        0        0     1148 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/room.proto
--rw-r--r--   0        0        0     3331 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/room_pb2.py
--rw-r--r--   0        0        0     2481 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/room_pb2_grpc.py
--rw-r--r--   0        0        0      821 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/test.proto
--rw-r--r--   0        0        0     2112 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/test_pb2.py
--rw-r--r--   0        0        0     5149 2023-07-24 14:11:40.856007 bilirpc-1.1/bilirpc/bilibili/broadcast/v1/test_pb2_grpc.py
--rw-r--r--   0        0        0      410 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/broadcast/v2/laser.proto
--rw-r--r--   0        0        0     1467 2023-07-24 14:11:48.583970 bilirpc-1.1/bilirpc/bilibili/broadcast/v2/laser_pb2.py
--rw-r--r--   0        0        0     2528 2023-07-24 14:11:48.583970 bilirpc-1.1/bilirpc/bilibili/broadcast/v2/laser_pb2_grpc.py
--rw-r--r--   0        0        0     3543 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/cheese/gateway/player/v1/playurl.proto
--rw-r--r--   0        0        0     4658 2023-07-24 14:12:20.327824 bilirpc-1.1/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2.py
--rw-r--r--   0        0        0     4518 2023-07-24 14:12:20.327824 bilirpc-1.1/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2_grpc.py
--rw-r--r--   0        0        0       27 2023-07-24 14:13:36.579526 bilirpc-1.1/bilirpc/bilibili/community/interfacess/biligram/v1/biligram.proto
--rw-r--r--   0        0        0      960 2023-07-24 14:13:42.411506 bilirpc-1.1/bilirpc/bilibili/community/interfacess/biligram/v1/biligram_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:13:42.411506 bilirpc-1.1/bilirpc/bilibili/community/interfacess/biligram/v1/biligram_pb2_grpc.py
--rw-r--r--   0        0        0    22984 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/community/service/dm/v1/dm.proto
--rw-r--r--   0        0        0    34431 2023-07-24 14:14:18.771390 bilirpc-1.1/bilirpc/bilibili/community/service/dm/v1/dm_pb2.py
--rw-r--r--   0        0        0    11551 2023-07-24 14:14:18.771390 bilirpc-1.1/bilirpc/bilibili/community/service/dm/v1/dm_pb2_grpc.py
--rw-r--r--   0        0        0      537 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/community/service/govern/v1/govern.proto
--rw-r--r--   0        0        0     1942 2023-07-24 14:14:40.611326 bilirpc-1.1/bilirpc/bilibili/community/service/govern/v1/govern_pb2.py
--rw-r--r--   0        0        0     2623 2023-07-24 14:14:40.611326 bilirpc-1.1/bilirpc/bilibili/community/service/govern/v1/govern_pb2_grpc.py
--rw-r--r--   0        0        0     2915 2023-07-24 14:30:40.439299 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/__pycache__/common_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1595 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/common.proto
--rw-r--r--   0        0        0     4397 2023-07-24 13:24:12.339667 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/common_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:24:12.339667 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/common_pb2_grpc.py
--rw-r--r--   0        0        0     4023 2023-07-24 14:30:40.439299 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/avatar_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2710 2023-07-24 14:30:40.439299 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/plugin_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2193 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/avatar.proto
--rw-r--r--   0        0        0     5838 2023-07-24 13:23:36.695422 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/avatar_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:23:36.695422 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/avatar_pb2_grpc.py
--rw-r--r--   0        0        0     1399 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/plugin.proto
--rw-r--r--   0        0        0     3935 2023-07-24 13:23:36.695422 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/plugin_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 13:23:36.695422 bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/plugin_pb2_grpc.py
--rw-r--r--   0        0        0    21995 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dynamic/common/dynamic.proto
--rw-r--r--   0        0        0    24391 2023-07-24 14:15:24.615213 bilirpc-1.1/bilirpc/bilibili/dynamic/common/dynamic_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:15:24.615213 bilirpc-1.1/bilirpc/bilibili/dynamic/common/dynamic_pb2_grpc.py
--rw-r--r--   0        0        0    63946 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dynamic/gw/gateway.proto
--rw-r--r--   0        0        0    79164 2023-07-24 14:15:24.615213 bilirpc-1.1/bilirpc/bilibili/dynamic/gw/gateway_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:15:24.615213 bilirpc-1.1/bilirpc/bilibili/dynamic/gw/gateway_pb2_grpc.py
--rw-r--r--   0        0        0        7 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/campus/v1/api.proto
--rw-r--r--   0        0        0     4742 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/feed/v1/api.proto
--rw-r--r--   0        0        0     9280 2023-07-24 14:16:00.899133 bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2.py
--rw-r--r--   0        0        0    24463 2023-07-24 14:16:00.899133 bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2_grpc.py
--rw-r--r--   0        0        0     4076 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/gaia/gw/gw_api.proto
--rw-r--r--   0        0        0     3986 2023-07-24 14:16:22.399090 bilirpc-1.1/bilirpc/bilibili/gaia/gw/gw_api_pb2.py
--rw-r--r--   0        0        0     4284 2023-07-24 14:16:22.399090 bilirpc-1.1/bilirpc/bilibili/gaia/gw/gw_api_pb2_grpc.py
--rw-r--r--   0        0        0      554 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/im/interfaces/inner-interface/v1/api.proto
--rw-r--r--   0        0        0     1925 2023-07-24 14:17:58.690944 bilirpc-1.1/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2.py
--rw-r--r--   0        0        0     2822 2023-07-24 14:17:58.690944 bilirpc-1.1/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2_grpc.py
--rw-r--r--   0        0        0    11343 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/im/interfaces/v1/im.proto
--rw-r--r--   0        0        0    19413 2023-07-24 14:18:45.198897 bilirpc-1.1/bilirpc/bilibili/im/interfaces/v1/im_pb2.py
--rw-r--r--   0        0        0    46195 2023-07-24 14:18:45.198897 bilirpc-1.1/bilirpc/bilibili/im/interfaces/v1/im_pb2_grpc.py
--rw-r--r--   0        0        0    11779 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/im/type/im.proto
--rw-r--r--   0        0        0    12171 2023-07-24 14:19:41.938856 bilirpc-1.1/bilirpc/bilibili/im/type/im_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:19:41.938856 bilirpc-1.1/bilirpc/bilibili/im/type/im_pb2_grpc.py
--rw-r--r--   0        0        0      826 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/live/app/room/v1/room.proto
--rw-r--r--   0        0        0     2527 2023-07-24 14:20:13.722842 bilirpc-1.1/bilirpc/bilibili/live/app/room/v1/room_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:20:13.722842 bilirpc-1.1/bilirpc/bilibili/live/app/room/v1/room_pb2_grpc.py
--rw-r--r--   0        0        0      934 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/live/general/interfaces/v1/interfaces.proto
--rw-r--r--   0        0        0     2520 2023-07-24 14:20:40.202833 bilirpc-1.1/bilirpc/bilibili/live/general/interfaces/v1/interfaces_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:20:40.202833 bilirpc-1.1/bilirpc/bilibili/live/general/interfaces/v1/interfaces_pb2_grpc.py
--rw-r--r--   0        0        0      767 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/main/common/arch/doll/v1/doll.proto
--rw-r--r--   0        0        0     2582 2023-07-24 14:21:11.734828 bilirpc-1.1/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2.py
--rw-r--r--   0        0        0     6142 2023-07-24 14:21:11.734828 bilirpc-1.1/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2_grpc.py
--rw-r--r--   0        0        0    26735 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/main/community/reply/v1/reply.proto
--rw-r--r--   0        0        0    39031 2023-07-24 14:21:33.830827 bilirpc-1.1/bilirpc/bilibili/main/community/reply/v1/reply_pb2.py
--rw-r--r--   0        0        0    21080 2023-07-24 14:21:33.830827 bilirpc-1.1/bilirpc/bilibili/main/community/reply/v1/reply_pb2_grpc.py
--rw-r--r--   0        0        0     1006 2023-07-24 14:31:00.259329 bilirpc-1.1/bilirpc/bilibili/metadata/__pycache__/metadata_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1149 2023-07-24 14:31:00.255329 bilirpc-1.1/bilirpc/bilibili/metadata/device/__pycache__/device_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1104 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/device/device.proto
--rw-r--r--   0        0        0     1611 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/device/device_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/device/device_pb2_grpc.py
--rw-r--r--   0        0        0      545 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/fawkes/fawkes.proto
--rw-r--r--   0        0        0     1352 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/fawkes/fawkes_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/fawkes/fawkes_pb2_grpc.py
--rw-r--r--   0        0        0     1160 2023-07-24 14:31:00.259329 bilirpc-1.1/bilirpc/bilibili/metadata/locale/__pycache__/locale_pb2.cpython-310.pyc
--rw-r--r--   0        0        0      749 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/locale/locale.proto
--rw-r--r--   0        0        0     1499 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/locale/locale_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/locale/locale_pb2_grpc.py
--rw-r--r--   0        0        0      509 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/metadata.proto
--rw-r--r--   0        0        0     1296 2023-07-24 14:22:20.566831 bilirpc-1.1/bilirpc/bilibili/metadata/metadata_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:20.566831 bilirpc-1.1/bilirpc/bilibili/metadata/metadata_pb2_grpc.py
--rw-r--r--   0        0        0     1309 2023-07-24 14:31:00.259329 bilirpc-1.1/bilirpc/bilibili/metadata/network/__pycache__/network_pb2.cpython-310.pyc
--rw-r--r--   0        0        0      754 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/network/network.proto
--rw-r--r--   0        0        0     1818 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/network/network_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/network/network_pb2_grpc.py
--rw-r--r--   0        0        0      183 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/parabox/parabox.proto
--rw-r--r--   0        0        0     1282 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/parabox/parabox_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/parabox/parabox_pb2_grpc.py
--rw-r--r--   0        0        0      545 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/metadata/restriction/restriction.proto
--rw-r--r--   0        0        0     1539 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/restriction/restriction_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.1/bilirpc/bilibili/metadata/restriction/restriction_pb2_grpc.py
--rw-r--r--   0        0        0      546 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/pagination/pagination.proto
--rw-r--r--   0        0        0     1838 2023-07-24 14:22:46.330838 bilirpc-1.1/bilirpc/bilibili/pagination/pagination_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:22:46.330838 bilirpc-1.1/bilirpc/bilibili/pagination/pagination_pb2_grpc.py
--rw-r--r--   0        0        0     3673 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/gallery.proto
--rw-r--r--   0        0        0     7936 2023-07-24 14:23:06.978845 bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2.py
--rw-r--r--   0        0        0    14838 2023-07-24 14:23:06.978845 bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2_grpc.py
--rw-r--r--   0        0        0        7 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/openplatform/apiserver/v1alpha1/api.proto
--rw-r--r--   0        0        0     6966 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v1/playurl.proto
--rw-r--r--   0        0        0     8395 2023-07-24 14:23:51.366865 bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2.py
--rw-r--r--   0        0        0     6300 2023-07-24 14:23:51.366865 bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2_grpc.py
--rw-r--r--   0        0        0    24837 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v2/playurl.proto
--rw-r--r--   0        0        0    37508 2023-07-24 14:23:59.398869 bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2.py
--rw-r--r--   0        0        0     4484 2023-07-24 14:23:59.398869 bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2_grpc.py
--rw-r--r--   0        0        0      831 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/pgc/service/premiere/v1/premiere.proto
--rw-r--r--   0        0        0     1798 2023-07-24 14:24:19.326881 bilirpc-1.1/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2.py
--rw-r--r--   0        0        0     2746 2023-07-24 14:24:19.326881 bilirpc-1.1/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2_grpc.py
--rw-r--r--   0        0        0     9874 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/playershared/playershared.proto
--rw-r--r--   0        0        0    15413 2023-07-24 14:24:39.446894 bilirpc-1.1/bilirpc/bilibili/playershared/playershared_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:24:39.446894 bilirpc-1.1/bilirpc/bilibili/playershared/playershared_pb2_grpc.py
--rw-r--r--   0        0        0    36287 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/polymer/app/search/v1/search.proto
--rw-r--r--   0        0        0    66042 2023-07-24 14:25:00.242909 bilirpc-1.1/bilirpc/bilibili/polymer/app/search/v1/search_pb2.py
--rw-r--r--   0        0        0     6355 2023-07-24 14:25:00.242909 bilirpc-1.1/bilirpc/bilibili/polymer/app/search/v1/search_pb2_grpc.py
--rw-r--r--   0        0        0     1775 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/polymer/community/govern/v1/govern.proto
--rw-r--r--   0        0        0     4486 2023-07-24 14:25:22.398926 bilirpc-1.1/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2.py
--rw-r--r--   0        0        0     5094 2023-07-24 14:25:22.398926 bilirpc-1.1/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2_grpc.py
--rw-r--r--   0        0        0     1361 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/polymer/contract/v1/contract.proto
--rw-r--r--   0        0        0     3522 2023-07-24 14:25:42.850943 bilirpc-1.1/bilirpc/bilibili/polymer/contract/v1/contract_pb2.py
--rw-r--r--   0        0        0     6231 2023-07-24 14:25:42.850943 bilirpc-1.1/bilirpc/bilibili/polymer/contract/v1/contract_pb2_grpc.py
--rw-r--r--   0        0        0      596 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/polymer/list/v1/list.proto
--rw-r--r--   0        0        0     2242 2023-07-24 14:26:26.630983 bilirpc-1.1/bilirpc/bilibili/polymer/list/v1/list_pb2.py
--rw-r--r--   0        0        0     4258 2023-07-24 14:26:26.630983 bilirpc-1.1/bilirpc/bilibili/polymer/list/v1/list_pb2_grpc.py
--rw-r--r--   0        0        0      783 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/relation/interfaces/api.proto
--rw-r--r--   0        0        0     2173 2023-07-24 14:26:47.439004 bilirpc-1.1/bilirpc/bilibili/relation/interfaces/api_pb2.py
--rw-r--r--   0        0        0     2798 2023-07-24 14:26:47.439004 bilirpc-1.1/bilirpc/bilibili/relation/interfaces/api_pb2_grpc.py
--rw-r--r--   0        0        0      251 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/render/render.proto
--rw-r--r--   0        0        0     1287 2023-07-24 14:27:15.919034 bilirpc-1.1/bilirpc/bilibili/render/render_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:27:15.919034 bilirpc-1.1/bilirpc/bilibili/render/render_pb2_grpc.py
--rw-r--r--   0        0        0      426 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/rpc/status.proto
--rw-r--r--   0        0        0     1244 2023-07-24 14:27:38.599060 bilirpc-1.1/bilirpc/bilibili/rpc/status_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:27:38.599060 bilirpc-1.1/bilirpc/bilibili/rpc/status_pb2_grpc.py
--rw-r--r--   0        0        0     9169 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/tv/interfaces/dm/v1/dm.proto
--rw-r--r--   0        0        0    11291 2023-07-24 14:27:59.255084 bilirpc-1.1/bilirpc/bilibili/tv/interfaces/dm/v1/dm_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:27:59.255084 bilirpc-1.1/bilirpc/bilibili/tv/interfaces/dm/v1/dm_pb2_grpc.py
--rw-r--r--   0        0        0      536 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/vega/deneb/v1/deneb.proto
--rw-r--r--   0        0        0     1887 2023-07-24 14:28:19.751108 bilirpc-1.1/bilirpc/bilibili/vega/deneb/v1/deneb_pb2.py
--rw-r--r--   0        0        0     2588 2023-07-24 14:28:19.755108 bilirpc-1.1/bilirpc/bilibili/vega/deneb/v1/deneb_pb2_grpc.py
--rw-r--r--   0        0        0    19322 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/web/interfaces/v1/interfaces.proto
--rw-r--r--   0        0        0    34870 2023-07-24 14:28:48.807145 bilirpc-1.1/bilirpc/bilibili/web/interfaces/v1/interfaces_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:28:48.807145 bilirpc-1.1/bilirpc/bilibili/web/interfaces/v1/interfaces_pb2_grpc.py
--rw-r--r--   0        0        0     3505 2023-07-22 13:13:29.000000 bilirpc-1.1/bilirpc/bilibili/web/space/v1/space.proto
--rw-r--r--   0        0        0     8294 2023-07-24 14:29:13.335177 bilirpc-1.1/bilirpc/bilibili/web/space/v1/space_pb2.py
--rw-r--r--   0        0        0      159 2023-07-24 14:29:13.335177 bilirpc-1.1/bilirpc/bilibili/web/space/v1/space_pb2_grpc.py
--rw-r--r--   0        0        0     1692 2023-07-24 15:51:36.313264 bilirpc-1.1/bilirpc/tools.py
--rw-r--r--   0        0        0      359 2023-07-25 12:49:52.792825 bilirpc-1.1/pyproject.toml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 bilirpc-1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-25 12:46:23.607515 bilirpc-1.2/README.md
+-rw-r--r--   0        0        0      174 2023-07-24 13:18:16.061240 bilirpc-1.2/bilirpc/__init__.py
+-rw-r--r--   0        0        0     2902 2023-07-25 12:53:17.618106 bilirpc-1.2/bilirpc/api.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:30:21.919272 bilirpc-1.2/bilirpc/bilibili/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-24 14:30:40.423299 bilirpc-1.2/bilirpc/bilibili/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1150 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/account/fission/v1/fission.proto
+-rw-r--r--   0        0        0     2663 2023-07-24 13:51:03.340765 bilirpc-1.2/bilirpc/bilibili/account/fission/v1/fission_pb2.py
+-rw-r--r--   0        0        0     6046 2023-07-25 12:53:37.730232 bilirpc-1.2/bilirpc/bilibili/account/fission/v1/fission_pb2_grpc.py
+-rw-r--r--   0        0        0    19936 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/ad/v1/ad.proto
+-rw-r--r--   0        0        0    25729 2023-07-24 13:51:41.504880 bilirpc-1.2/bilirpc/bilibili/ad/v1/ad_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:51:41.504880 bilirpc-1.2/bilirpc/bilibili/ad/v1/ad_pb2_grpc.py
+-rw-r--r--   0        0        0     1308 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/api/player/v1/player.proto
+-rw-r--r--   0        0        0     2587 2023-07-24 13:52:06.044955 bilirpc-1.2/bilirpc/bilibili/api/player/v1/player_pb2.py
+-rw-r--r--   0        0        0     2580 2023-07-25 12:54:35.678594 bilirpc-1.2/bilirpc/bilibili/api/player/v1/player_pb2_grpc.py
+-rw-r--r--   0        0        0     3131 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/api/probe/v1/probe.proto
+-rw-r--r--   0        0        0     7021 2023-07-24 13:52:42.613071 bilirpc-1.2/bilirpc/bilibili/api/probe/v1/probe_pb2.py
+-rw-r--r--   0        0        0    16577 2023-07-25 12:53:58.874364 bilirpc-1.2/bilirpc/bilibili/api/probe/v1/probe_pb2_grpc.py
+-rw-r--r--   0        0        0     1040 2023-07-24 15:00:59.453756 bilirpc-1.2/bilirpc/bilibili/app/archive/middleware/v1/__pycache__/preload_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0      394 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/archive/middleware/v1/preload.proto
+-rw-r--r--   0        0        0     1277 2023-07-24 13:53:50.333291 bilirpc-1.2/bilirpc/bilibili/app/archive/middleware/v1/preload_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:53:50.333291 bilirpc-1.2/bilirpc/bilibili/app/archive/middleware/v1/preload_pb2_grpc.py
+-rw-r--r--   0        0        0     3869 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/archive/v1/archive.proto
+-rw-r--r--   0        0        0     5206 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/archive/v1/archive_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/archive/v1/archive_pb2_grpc.py
+-rw-r--r--   0        0        0      982 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/card/v1/ad.proto
+-rw-r--r--   0        0        0     2256 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/ad_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/ad_pb2_grpc.py
+-rw-r--r--   0        0        0      777 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/card/v1/card.proto
+-rw-r--r--   0        0        0     2150 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/card_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/card_pb2_grpc.py
+-rw-r--r--   0        0        0     5488 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/card/v1/common.proto
+-rw-r--r--   0        0        0     9224 2023-07-25 12:55:14.810838 bilirpc-1.2/bilirpc/bilibili/app/card/v1/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     6786 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/card/v1/double.proto
+-rw-r--r--   0        0        0    12879 2023-07-25 12:55:22.338885 bilirpc-1.2/bilirpc/bilibili/app/card/v1/double_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/double_pb2_grpc.py
+-rw-r--r--   0        0        0     6404 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/card/v1/single.proto
+-rw-r--r--   0        0        0    10615 2023-07-25 12:55:27.058915 bilirpc-1.2/bilirpc/bilibili/app/card/v1/single_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/card/v1/single_pb2_grpc.py
+-rw-r--r--   0        0        0     1746 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/click/v1/heartbeat.proto
+-rw-r--r--   0        0        0     3956 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/click/v1/heartbeat_pb2.py
+-rw-r--r--   0        0        0      876 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/click/v1/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0      263 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/download.proto
+-rw-r--r--   0        0        0     1419 2023-07-25 12:55:48.283047 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/download_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/download_pb2_grpc.py
+-rw-r--r--   0        0        0      321 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/dynamic.proto
+-rw-r--r--   0        0        0     1615 2023-07-25 12:55:52.651075 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/dynamic_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/dynamic_pb2_grpc.py
+-rw-r--r--   0        0        0     1729 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/experimental.proto
+-rw-r--r--   0        0        0     3652 2023-07-25 12:55:56.691100 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/experimental_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/experimental_pb2_grpc.py
+-rw-r--r--   0        0        0      263 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/internaldevice.proto
+-rw-r--r--   0        0        0     1420 2023-07-25 12:56:00.919126 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/internaldevice_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/internaldevice_pb2_grpc.py
+-rw-r--r--   0        0        0      253 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/night.proto
+-rw-r--r--   0        0        0     1389 2023-07-25 12:56:03.671143 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/night_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/night_pb2_grpc.py
+-rw-r--r--   0        0        0      818 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/other.proto
+-rw-r--r--   0        0        0     2079 2023-07-25 12:56:07.299166 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/other_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/other_pb2_grpc.py
+-rw-r--r--   0        0        0      936 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/pegasus.proto
+-rw-r--r--   0        0        0     2665 2023-07-25 12:56:11.627193 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/pegasus_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/pegasus_pb2_grpc.py
+-rw-r--r--   0        0        0     1961 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/play.proto
+-rw-r--r--   0        0        0     3452 2023-07-25 12:56:14.867213 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/play_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/play_pb2_grpc.py
+-rw-r--r--   0        0        0      465 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/privacy.proto
+-rw-r--r--   0        0        0     1749 2023-07-25 12:56:18.427236 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/privacy_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/privacy_pb2_grpc.py
+-rw-r--r--   0        0        0      399 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/search.proto
+-rw-r--r--   0        0        0     1719 2023-07-25 12:56:23.639268 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/search_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:56:53.589928 bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/search_pb2_grpc.py
+-rw-r--r--   0        0        0     2721 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/distribution/v1/distribution.proto
+-rw-r--r--   0        0        0     6193 2023-07-24 14:08:26.245264 bilirpc-1.2/bilirpc/bilibili/app/distribution/v1/distribution_pb2.py
+-rw-r--r--   0        0        0     6612 2023-07-25 12:56:36.023346 bilirpc-1.2/bilirpc/bilibili/app/distribution/v1/distribution_pb2_grpc.py
+-rw-r--r--   0        0        0      293 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/dynamic/common/dynamic.proto
+-rw-r--r--   0        0        0     1419 2023-07-24 13:57:43.678110 bilirpc-1.2/bilirpc/bilibili/app/dynamic/common/dynamic_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:57:43.678110 bilirpc-1.2/bilirpc/bilibili/app/dynamic/common/dynamic_pb2_grpc.py
+-rw-r--r--   0        0        0    21326 2023-07-24 15:00:59.449756 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     8807 2023-07-24 15:00:59.453756 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0    29817 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/dynamic.proto
+-rw-r--r--   0        0        0    37885 2023-07-25 12:57:08.879400 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2.py
+-rw-r--r--   0        0        0    23614 2023-07-25 12:57:14.731214 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2_grpc.py
+-rw-r--r--   0        0        0   100695 2023-07-24 14:30:40.431299 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    31191 2023-07-24 14:30:40.451299 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0     1282 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/campus.proto
+-rw-r--r--   0        0        0     3959 2023-07-25 12:57:28.618782 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/campus_pb2.py
+-rw-r--r--   0        0        0     2736 2023-07-25 12:57:18.967081 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/campus_pb2_grpc.py
+-rw-r--r--   0        0        0   117183 2023-07-24 13:04:02.811851 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/dynamic.proto
+-rw-r--r--   0        0        0   172974 2023-07-24 13:58:26.402268 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2.py
+-rw-r--r--   0        0        0    99333 2023-07-25 12:57:42.274370 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2_grpc.py
+-rw-r--r--   0        0        0      962 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/opus.proto
+-rw-r--r--   0        0        0     2924 2023-07-25 12:57:53.146050 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/opus_pb2.py
+-rw-r--r--   0        0        0     2667 2023-07-25 12:57:46.730238 bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/opus_pb2_grpc.py
+-rw-r--r--   0        0        0     8157 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/history.proto
+-rw-r--r--   0        0        0    11010 2023-07-25 12:57:58.813886 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/history_pb2.py
+-rw-r--r--   0        0        0    12971 2023-07-24 14:08:26.249264 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/history_pb2_grpc.py
+-rw-r--r--   0        0        0     4599 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/media.proto
+-rw-r--r--   0        0        0    10030 2023-07-24 14:08:26.249264 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/media_pb2.py
+-rw-r--r--   0        0        0     9485 2023-07-25 12:58:01.101820 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/media_pb2_grpc.py
+-rw-r--r--   0        0        0     3565 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/search.proto
+-rw-r--r--   0        0        0     5394 2023-07-24 14:08:26.249264 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/search_pb2.py
+-rw-r--r--   0        0        0     6754 2023-07-25 12:58:13.557468 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/search_pb2_grpc.py
+-rw-r--r--   0        0        0     1612 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/space.proto
+-rw-r--r--   0        0        0     4319 2023-07-25 12:58:23.337198 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/space_pb2.py
+-rw-r--r--   0        0        0     6069 2023-07-25 12:58:16.333391 bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/space_pb2_grpc.py
+-rw-r--r--   0        0        0    19736 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/listener/v1/listener.proto
+-rw-r--r--   0        0        0    40544 2023-07-25 12:58:36.852834 bilirpc-1.2/bilirpc/bilibili/app/listener/v1/listener_pb2.py
+-rw-r--r--   0        0        0    58680 2023-07-24 14:08:26.297264 bilirpc-1.2/bilirpc/bilibili/app/listener/v1/listener_pb2_grpc.py
+-rw-r--r--   0        0        0    28703 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/nativeact/v1/nativeact.proto
+-rw-r--r--   0        0        0    51657 2023-07-25 12:58:46.800572 bilirpc-1.2/bilirpc/bilibili/app/nativeact/v1/nativeact_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/nativeact/v1/nativeact_pb2_grpc.py
+-rw-r--r--   0        0        0     1200 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/playeronline/v1/playeronline.proto
+-rw-r--r--   0        0        0     2911 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2.py
+-rw-r--r--   0        0        0     6374 2023-07-25 12:58:54.396376 bilirpc-1.2/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2_grpc.py
+-rw-r--r--   0        0        0      482 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel.proto
+-rw-r--r--   0        0        0     1749 2023-07-25 12:58:59.620243 bilirpc-1.2/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:00:45.226794 bilirpc-1.2/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel_pb2_grpc.py
+-rw-r--r--   0        0        0      471 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel.proto
+-rw-r--r--   0        0        0     2046 2023-07-24 14:01:01.518857 bilirpc-1.2/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:01:01.518857 bilirpc-1.2/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel_pb2_grpc.py
+-rw-r--r--   0        0        0     1171 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/playerunite/v1/playerunite.proto
+-rw-r--r--   0        0        0     2977 2023-07-25 12:59:10.507970 bilirpc-1.2/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2.py
+-rw-r--r--   0        0        0     2727 2023-07-25 12:59:14.807864 bilirpc-1.2/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2_grpc.py
+-rw-r--r--   0        0        0    15390 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/playurl/v1/playurl.proto
+-rw-r--r--   0        0        0    22028 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/playurl/v1/playurl_pb2.py
+-rw-r--r--   0        0        0     9424 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/playurl/v1/playurl_pb2_grpc.py
+-rw-r--r--   0        0        0     1170 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/resource/privacy/v1/api.proto
+-rw-r--r--   0        0        0     3009 2023-07-24 14:02:05.011104 bilirpc-1.2/bilirpc/bilibili/app/resource/privacy/v1/api_pb2.py
+-rw-r--r--   0        0        0     4573 2023-07-25 12:59:27.355561 bilirpc-1.2/bilirpc/bilibili/app/resource/privacy/v1/api_pb2_grpc.py
+-rw-r--r--   0        0        0     1941 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/resource/v1/module.proto
+-rw-r--r--   0        0        0     4261 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/resource/v1/module_pb2.py
+-rw-r--r--   0        0        0     2480 2023-07-25 12:59:33.063425 bilirpc-1.2/bilirpc/bilibili/app/resource/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1692 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/search/v2/search.proto
+-rw-r--r--   0        0        0     4023 2023-07-25 12:59:37.371324 bilirpc-1.2/bilirpc/bilibili/app/search/v2/search_pb2.py
+-rw-r--r--   0        0        0     8045 2023-07-25 12:59:47.631086 bilirpc-1.2/bilirpc/bilibili/app/search/v2/search_pb2_grpc.py
+-rw-r--r--   0        0        0      546 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/show/gateway/v1/service.proto
+-rw-r--r--   0        0        0     1804 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/gateway/v1/service_pb2.py
+-rw-r--r--   0        0        0     2716 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/gateway/v1/service_pb2_grpc.py
+-rw-r--r--   0        0        0      754 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/show/mixture/v1/mixture.proto
+-rw-r--r--   0        0        0     2216 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2.py
+-rw-r--r--   0        0        0     2589 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2_grpc.py
+-rw-r--r--   0        0        0     2470 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/show/popular/v1/popular.proto
+-rw-r--r--   0        0        0     3741 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/popular/v1/popular_pb2.py
+-rw-r--r--   0        0        0     2608 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/popular/v1/popular_pb2_grpc.py
+-rw-r--r--   0        0        0     2478 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/show/rank/v1/rank.proto
+-rw-r--r--   0        0        0     3522 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/rank/v1/rank_pb2.py
+-rw-r--r--   0        0        0     4316 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/rank/v1/rank_pb2_grpc.py
+-rw-r--r--   0        0        0      734 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/show/region/v1/region.proto
+-rw-r--r--   0        0        0     2301 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/region/v1/region_pb2.py
+-rw-r--r--   0        0        0     2559 2023-07-24 14:07:39.765669 bilirpc-1.2/bilirpc/bilibili/app/show/region/v1/region_pb2_grpc.py
+-rw-r--r--   0        0        0     1504 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/space/v1/space.proto
+-rw-r--r--   0        0        0     3424 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/space/v1/space_pb2.py
+-rw-r--r--   0        0        0     2463 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/space/v1/space_pb2_grpc.py
+-rw-r--r--   0        0        0     2031 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/splash/v1/splash.proto
+-rw-r--r--   0        0        0     3833 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/splash/v1/splash_pb2.py
+-rw-r--r--   0        0        0     2462 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/splash/v1/splash_pb2_grpc.py
+-rw-r--r--   0        0        0     9159 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/topic/v1/topic.proto
+-rw-r--r--   0        0        0    17394 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/topic/v1/topic_pb2.py
+-rw-r--r--   0        0        0     6076 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/topic/v1/topic_pb2_grpc.py
+-rw-r--r--   0        0        0    49304 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/view/v1/view.proto
+-rw-r--r--   0        0        0    72369 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/view/v1/view_pb2.py
+-rw-r--r--   0        0        0    35019 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/view/v1/view_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/viewunite/pgcanymodel.proto
+-rw-r--r--   0        0        0     1144 2023-07-24 14:08:44.349119 bilirpc-1.2/bilirpc/bilibili/app/viewunite/pgcanymodel_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:44.349119 bilirpc-1.2/bilirpc/bilibili/app/viewunite/pgcanymodel_pb2_grpc.py
+-rw-r--r--   0        0        0      110 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/viewunite/ugcanymodel.proto
+-rw-r--r--   0        0        0     1061 2023-07-24 14:08:44.349119 bilirpc-1.2/bilirpc/bilibili/app/viewunite/ugcanymodel_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:08:44.349119 bilirpc-1.2/bilirpc/bilibili/app/viewunite/ugcanymodel_pb2_grpc.py
+-rw-r--r--   0        0        0     8800 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/viewunite/v1/viewunite.proto
+-rw-r--r--   0        0        0    15661 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2.py
+-rw-r--r--   0        0        0     4369 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2_grpc.py
+-rw-r--r--   0        0        0      831 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/app/wall/v1/wall.proto
+-rw-r--r--   0        0        0     2301 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/wall/v1/wall_pb2.py
+-rw-r--r--   0        0        0     2501 2023-07-24 14:08:26.301264 bilirpc-1.2/bilirpc/bilibili/app/wall/v1/wall_pb2_grpc.py
+-rw-r--r--   0        0        0      644 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/editor/notify.proto
+-rw-r--r--   0        0        0     1745 2023-07-24 14:11:23.684094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/editor/notify_pb2.py
+-rw-r--r--   0        0        0     2694 2023-07-24 14:11:23.684094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/editor/notify_pb2_grpc.py
+-rw-r--r--   0        0        0      114 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/esports/notify.proto
+-rw-r--r--   0        0        0     1114 2023-07-24 14:11:23.684094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/esports/notify_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/esports/notify_pb2_grpc.py
+-rw-r--r--   0        0        0      320 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/fission/notify.proto
+-rw-r--r--   0        0        0     1505 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/fission/notify_pb2.py
+-rw-r--r--   0        0        0     2638 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/fission/notify_pb2_grpc.py
+-rw-r--r--   0        0        0     2001 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/im/notify.proto
+-rw-r--r--   0        0        0     3351 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/im/notify_pb2.py
+-rw-r--r--   0        0        0     2580 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/im/notify_pb2_grpc.py
+-rw-r--r--   0        0        0     1239 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/dm.proto
+-rw-r--r--   0        0        0     2245 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/dm_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/dm_pb2_grpc.py
+-rw-r--r--   0        0        0      668 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/native.proto
+-rw-r--r--   0        0        0     1882 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/native_pb2.py
+-rw-r--r--   0        0        0     2642 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/native_pb2_grpc.py
+-rw-r--r--   0        0        0     1262 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/resource.proto
+-rw-r--r--   0        0        0     2476 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/resource_pb2.py
+-rw-r--r--   0        0        0     2641 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/resource_pb2_grpc.py
+-rw-r--r--   0        0        0      529 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/search.proto
+-rw-r--r--   0        0        0     1974 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/search_pb2.py
+-rw-r--r--   0        0        0     2820 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/search_pb2_grpc.py
+-rw-r--r--   0        0        0      162 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/note/sync.proto
+-rw-r--r--   0        0        0     1124 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/note/sync_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/note/sync_pb2_grpc.py
+-rw-r--r--   0        0        0     4914 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/freya.proto
+-rw-r--r--   0        0        0     7508 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/freya_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/freya_pb2_grpc.py
+-rw-r--r--   0        0        0     1004 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/live.proto
+-rw-r--r--   0        0        0     2170 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/live_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/live_pb2_grpc.py
+-rw-r--r--   0        0        0      306 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ticket/activitygame.proto
+-rw-r--r--   0        0        0     1417 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ticket/activitygame_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/ticket/activitygame_pb2_grpc.py
+-rw-r--r--   0        0        0     1727 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/message/tv/proj.proto
+-rw-r--r--   0        0        0     2948 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/tv/proj_pb2.py
+-rw-r--r--   0        0        0     9106 2023-07-24 14:11:23.688094 bilirpc-1.2/bilirpc/bilibili/broadcast/message/tv/proj_pb2_grpc.py
+-rw-r--r--   0        0        0     3051 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/broadcast.proto
+-rw-r--r--   0        0        0     3962 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/broadcast_pb2.py
+-rw-r--r--   0        0        0    11798 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/broadcast_pb2_grpc.py
+-rw-r--r--   0        0        0      380 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/laser.proto
+-rw-r--r--   0        0        0     1456 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/laser_pb2.py
+-rw-r--r--   0        0        0     2604 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/laser_pb2_grpc.py
+-rw-r--r--   0        0        0      446 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/mod.proto
+-rw-r--r--   0        0        0     1630 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/mod_pb2.py
+-rw-r--r--   0        0        0     2575 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/mod_pb2_grpc.py
+-rw-r--r--   0        0        0     2721 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/push.proto
+-rw-r--r--   0        0        0     4288 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/push_pb2.py
+-rw-r--r--   0        0        0     2560 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/push_pb2_grpc.py
+-rw-r--r--   0        0        0     1148 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/room.proto
+-rw-r--r--   0        0        0     3331 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/room_pb2.py
+-rw-r--r--   0        0        0     2481 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/room_pb2_grpc.py
+-rw-r--r--   0        0        0      821 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/test.proto
+-rw-r--r--   0        0        0     2112 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/test_pb2.py
+-rw-r--r--   0        0        0     5149 2023-07-24 14:11:40.856007 bilirpc-1.2/bilirpc/bilibili/broadcast/v1/test_pb2_grpc.py
+-rw-r--r--   0        0        0      410 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/broadcast/v2/laser.proto
+-rw-r--r--   0        0        0     1467 2023-07-24 14:11:48.583970 bilirpc-1.2/bilirpc/bilibili/broadcast/v2/laser_pb2.py
+-rw-r--r--   0        0        0     2528 2023-07-24 14:11:48.583970 bilirpc-1.2/bilirpc/bilibili/broadcast/v2/laser_pb2_grpc.py
+-rw-r--r--   0        0        0     3543 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/cheese/gateway/player/v1/playurl.proto
+-rw-r--r--   0        0        0     4658 2023-07-24 14:12:20.327824 bilirpc-1.2/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2.py
+-rw-r--r--   0        0        0     4518 2023-07-24 14:12:20.327824 bilirpc-1.2/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2_grpc.py
+-rw-r--r--   0        0        0       27 2023-07-24 14:13:36.579526 bilirpc-1.2/bilirpc/bilibili/community/interfacess/biligram/v1/biligram.proto
+-rw-r--r--   0        0        0      960 2023-07-24 14:13:42.411506 bilirpc-1.2/bilirpc/bilibili/community/interfacess/biligram/v1/biligram_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:13:42.411506 bilirpc-1.2/bilirpc/bilibili/community/interfacess/biligram/v1/biligram_pb2_grpc.py
+-rw-r--r--   0        0        0    22984 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/community/service/dm/v1/dm.proto
+-rw-r--r--   0        0        0    34431 2023-07-24 14:14:18.771390 bilirpc-1.2/bilirpc/bilibili/community/service/dm/v1/dm_pb2.py
+-rw-r--r--   0        0        0    11551 2023-07-24 14:14:18.771390 bilirpc-1.2/bilirpc/bilibili/community/service/dm/v1/dm_pb2_grpc.py
+-rw-r--r--   0        0        0      537 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/community/service/govern/v1/govern.proto
+-rw-r--r--   0        0        0     1942 2023-07-24 14:14:40.611326 bilirpc-1.2/bilirpc/bilibili/community/service/govern/v1/govern_pb2.py
+-rw-r--r--   0        0        0     2623 2023-07-24 14:14:40.611326 bilirpc-1.2/bilirpc/bilibili/community/service/govern/v1/govern_pb2_grpc.py
+-rw-r--r--   0        0        0     2915 2023-07-24 14:30:40.439299 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/__pycache__/common_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1595 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/common.proto
+-rw-r--r--   0        0        0     4397 2023-07-24 13:24:12.339667 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:24:12.339667 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/common_pb2_grpc.py
+-rw-r--r--   0        0        0     4023 2023-07-24 14:30:40.439299 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/avatar_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2710 2023-07-24 14:30:40.439299 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/plugin_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2193 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/avatar.proto
+-rw-r--r--   0        0        0     5838 2023-07-24 13:23:36.695422 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/avatar_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:23:36.695422 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/avatar_pb2_grpc.py
+-rw-r--r--   0        0        0     1399 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/plugin.proto
+-rw-r--r--   0        0        0     3935 2023-07-24 13:23:36.695422 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/plugin_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 13:23:36.695422 bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/plugin_pb2_grpc.py
+-rw-r--r--   0        0        0    21995 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dynamic/common/dynamic.proto
+-rw-r--r--   0        0        0    24391 2023-07-24 14:15:24.615213 bilirpc-1.2/bilirpc/bilibili/dynamic/common/dynamic_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:15:24.615213 bilirpc-1.2/bilirpc/bilibili/dynamic/common/dynamic_pb2_grpc.py
+-rw-r--r--   0        0        0    63946 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dynamic/gw/gateway.proto
+-rw-r--r--   0        0        0    79164 2023-07-24 14:15:24.615213 bilirpc-1.2/bilirpc/bilibili/dynamic/gw/gateway_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:15:24.615213 bilirpc-1.2/bilirpc/bilibili/dynamic/gw/gateway_pb2_grpc.py
+-rw-r--r--   0        0        0        7 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/campus/v1/api.proto
+-rw-r--r--   0        0        0     4742 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/feed/v1/api.proto
+-rw-r--r--   0        0        0     9280 2023-07-24 14:16:00.899133 bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2.py
+-rw-r--r--   0        0        0    24463 2023-07-24 14:16:00.899133 bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2_grpc.py
+-rw-r--r--   0        0        0     4076 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/gaia/gw/gw_api.proto
+-rw-r--r--   0        0        0     3986 2023-07-24 14:16:22.399090 bilirpc-1.2/bilirpc/bilibili/gaia/gw/gw_api_pb2.py
+-rw-r--r--   0        0        0     4284 2023-07-24 14:16:22.399090 bilirpc-1.2/bilirpc/bilibili/gaia/gw/gw_api_pb2_grpc.py
+-rw-r--r--   0        0        0      554 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/im/interfaces/inner-interface/v1/api.proto
+-rw-r--r--   0        0        0     1925 2023-07-24 14:17:58.690944 bilirpc-1.2/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2.py
+-rw-r--r--   0        0        0     2822 2023-07-24 14:17:58.690944 bilirpc-1.2/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2_grpc.py
+-rw-r--r--   0        0        0    11343 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/im/interfaces/v1/im.proto
+-rw-r--r--   0        0        0    19413 2023-07-24 14:18:45.198897 bilirpc-1.2/bilirpc/bilibili/im/interfaces/v1/im_pb2.py
+-rw-r--r--   0        0        0    46195 2023-07-24 14:18:45.198897 bilirpc-1.2/bilirpc/bilibili/im/interfaces/v1/im_pb2_grpc.py
+-rw-r--r--   0        0        0    11779 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/im/type/im.proto
+-rw-r--r--   0        0        0    12171 2023-07-24 14:19:41.938856 bilirpc-1.2/bilirpc/bilibili/im/type/im_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:19:41.938856 bilirpc-1.2/bilirpc/bilibili/im/type/im_pb2_grpc.py
+-rw-r--r--   0        0        0      826 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/live/app/room/v1/room.proto
+-rw-r--r--   0        0        0     2527 2023-07-24 14:20:13.722842 bilirpc-1.2/bilirpc/bilibili/live/app/room/v1/room_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:20:13.722842 bilirpc-1.2/bilirpc/bilibili/live/app/room/v1/room_pb2_grpc.py
+-rw-r--r--   0        0        0      934 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/live/general/interfaces/v1/interfaces.proto
+-rw-r--r--   0        0        0     2520 2023-07-24 14:20:40.202833 bilirpc-1.2/bilirpc/bilibili/live/general/interfaces/v1/interfaces_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:20:40.202833 bilirpc-1.2/bilirpc/bilibili/live/general/interfaces/v1/interfaces_pb2_grpc.py
+-rw-r--r--   0        0        0      767 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/main/common/arch/doll/v1/doll.proto
+-rw-r--r--   0        0        0     2582 2023-07-24 14:21:11.734828 bilirpc-1.2/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2.py
+-rw-r--r--   0        0        0     6142 2023-07-24 14:21:11.734828 bilirpc-1.2/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2_grpc.py
+-rw-r--r--   0        0        0    26735 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/main/community/reply/v1/reply.proto
+-rw-r--r--   0        0        0    39031 2023-07-24 14:21:33.830827 bilirpc-1.2/bilirpc/bilibili/main/community/reply/v1/reply_pb2.py
+-rw-r--r--   0        0        0    21080 2023-07-24 14:21:33.830827 bilirpc-1.2/bilirpc/bilibili/main/community/reply/v1/reply_pb2_grpc.py
+-rw-r--r--   0        0        0     1006 2023-07-24 14:31:00.259329 bilirpc-1.2/bilirpc/bilibili/metadata/__pycache__/metadata_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1149 2023-07-24 14:31:00.255329 bilirpc-1.2/bilirpc/bilibili/metadata/device/__pycache__/device_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1104 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/device/device.proto
+-rw-r--r--   0        0        0     1611 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/device/device_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/device/device_pb2_grpc.py
+-rw-r--r--   0        0        0      545 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/fawkes/fawkes.proto
+-rw-r--r--   0        0        0     1352 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/fawkes/fawkes_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/fawkes/fawkes_pb2_grpc.py
+-rw-r--r--   0        0        0     1160 2023-07-24 14:31:00.259329 bilirpc-1.2/bilirpc/bilibili/metadata/locale/__pycache__/locale_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0      749 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/locale/locale.proto
+-rw-r--r--   0        0        0     1499 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/locale/locale_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/locale/locale_pb2_grpc.py
+-rw-r--r--   0        0        0      509 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/metadata.proto
+-rw-r--r--   0        0        0     1296 2023-07-24 14:22:20.566831 bilirpc-1.2/bilirpc/bilibili/metadata/metadata_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:20.566831 bilirpc-1.2/bilirpc/bilibili/metadata/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0     1309 2023-07-24 14:31:00.259329 bilirpc-1.2/bilirpc/bilibili/metadata/network/__pycache__/network_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0      754 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/network/network.proto
+-rw-r--r--   0        0        0     1818 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/network/network_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/network/network_pb2_grpc.py
+-rw-r--r--   0        0        0      183 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/parabox/parabox.proto
+-rw-r--r--   0        0        0     1282 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/parabox/parabox_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/parabox/parabox_pb2_grpc.py
+-rw-r--r--   0        0        0      545 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/metadata/restriction/restriction.proto
+-rw-r--r--   0        0        0     1539 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/restriction/restriction_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:15.374830 bilirpc-1.2/bilirpc/bilibili/metadata/restriction/restriction_pb2_grpc.py
+-rw-r--r--   0        0        0      546 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/pagination/pagination.proto
+-rw-r--r--   0        0        0     1838 2023-07-24 14:22:46.330838 bilirpc-1.2/bilirpc/bilibili/pagination/pagination_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:22:46.330838 bilirpc-1.2/bilirpc/bilibili/pagination/pagination_pb2_grpc.py
+-rw-r--r--   0        0        0     3673 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/gallery.proto
+-rw-r--r--   0        0        0     7936 2023-07-24 14:23:06.978845 bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2.py
+-rw-r--r--   0        0        0    14838 2023-07-24 14:23:06.978845 bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2_grpc.py
+-rw-r--r--   0        0        0        7 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/openplatform/apiserver/v1alpha1/api.proto
+-rw-r--r--   0        0        0     6966 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v1/playurl.proto
+-rw-r--r--   0        0        0     8395 2023-07-24 14:23:51.366865 bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2.py
+-rw-r--r--   0        0        0     6300 2023-07-24 14:23:51.366865 bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2_grpc.py
+-rw-r--r--   0        0        0    24837 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v2/playurl.proto
+-rw-r--r--   0        0        0    37508 2023-07-24 14:23:59.398869 bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2.py
+-rw-r--r--   0        0        0     4484 2023-07-24 14:23:59.398869 bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2_grpc.py
+-rw-r--r--   0        0        0      831 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/pgc/service/premiere/v1/premiere.proto
+-rw-r--r--   0        0        0     1798 2023-07-24 14:24:19.326881 bilirpc-1.2/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2.py
+-rw-r--r--   0        0        0     2746 2023-07-24 14:24:19.326881 bilirpc-1.2/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2_grpc.py
+-rw-r--r--   0        0        0     9874 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/playershared/playershared.proto
+-rw-r--r--   0        0        0    15413 2023-07-24 14:24:39.446894 bilirpc-1.2/bilirpc/bilibili/playershared/playershared_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:24:39.446894 bilirpc-1.2/bilirpc/bilibili/playershared/playershared_pb2_grpc.py
+-rw-r--r--   0        0        0    36287 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/polymer/app/search/v1/search.proto
+-rw-r--r--   0        0        0    66042 2023-07-24 14:25:00.242909 bilirpc-1.2/bilirpc/bilibili/polymer/app/search/v1/search_pb2.py
+-rw-r--r--   0        0        0     6355 2023-07-24 14:25:00.242909 bilirpc-1.2/bilirpc/bilibili/polymer/app/search/v1/search_pb2_grpc.py
+-rw-r--r--   0        0        0     1775 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/polymer/community/govern/v1/govern.proto
+-rw-r--r--   0        0        0     4486 2023-07-24 14:25:22.398926 bilirpc-1.2/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2.py
+-rw-r--r--   0        0        0     5094 2023-07-24 14:25:22.398926 bilirpc-1.2/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2_grpc.py
+-rw-r--r--   0        0        0     1361 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/polymer/contract/v1/contract.proto
+-rw-r--r--   0        0        0     3522 2023-07-24 14:25:42.850943 bilirpc-1.2/bilirpc/bilibili/polymer/contract/v1/contract_pb2.py
+-rw-r--r--   0        0        0     6231 2023-07-24 14:25:42.850943 bilirpc-1.2/bilirpc/bilibili/polymer/contract/v1/contract_pb2_grpc.py
+-rw-r--r--   0        0        0      596 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/polymer/list/v1/list.proto
+-rw-r--r--   0        0        0     2242 2023-07-24 14:26:26.630983 bilirpc-1.2/bilirpc/bilibili/polymer/list/v1/list_pb2.py
+-rw-r--r--   0        0        0     4258 2023-07-24 14:26:26.630983 bilirpc-1.2/bilirpc/bilibili/polymer/list/v1/list_pb2_grpc.py
+-rw-r--r--   0        0        0      783 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/relation/interfaces/api.proto
+-rw-r--r--   0        0        0     2173 2023-07-24 14:26:47.439004 bilirpc-1.2/bilirpc/bilibili/relation/interfaces/api_pb2.py
+-rw-r--r--   0        0        0     2798 2023-07-24 14:26:47.439004 bilirpc-1.2/bilirpc/bilibili/relation/interfaces/api_pb2_grpc.py
+-rw-r--r--   0        0        0      251 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/render/render.proto
+-rw-r--r--   0        0        0     1287 2023-07-24 14:27:15.919034 bilirpc-1.2/bilirpc/bilibili/render/render_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:27:15.919034 bilirpc-1.2/bilirpc/bilibili/render/render_pb2_grpc.py
+-rw-r--r--   0        0        0      426 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/rpc/status.proto
+-rw-r--r--   0        0        0     1244 2023-07-24 14:27:38.599060 bilirpc-1.2/bilirpc/bilibili/rpc/status_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:27:38.599060 bilirpc-1.2/bilirpc/bilibili/rpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0     9169 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/tv/interfaces/dm/v1/dm.proto
+-rw-r--r--   0        0        0    11291 2023-07-24 14:27:59.255084 bilirpc-1.2/bilirpc/bilibili/tv/interfaces/dm/v1/dm_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:27:59.255084 bilirpc-1.2/bilirpc/bilibili/tv/interfaces/dm/v1/dm_pb2_grpc.py
+-rw-r--r--   0        0        0      536 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/vega/deneb/v1/deneb.proto
+-rw-r--r--   0        0        0     1887 2023-07-24 14:28:19.751108 bilirpc-1.2/bilirpc/bilibili/vega/deneb/v1/deneb_pb2.py
+-rw-r--r--   0        0        0     2588 2023-07-24 14:28:19.755108 bilirpc-1.2/bilirpc/bilibili/vega/deneb/v1/deneb_pb2_grpc.py
+-rw-r--r--   0        0        0    19322 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/web/interfaces/v1/interfaces.proto
+-rw-r--r--   0        0        0    34870 2023-07-24 14:28:48.807145 bilirpc-1.2/bilirpc/bilibili/web/interfaces/v1/interfaces_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:28:48.807145 bilirpc-1.2/bilirpc/bilibili/web/interfaces/v1/interfaces_pb2_grpc.py
+-rw-r--r--   0        0        0     3505 2023-07-22 13:13:29.000000 bilirpc-1.2/bilirpc/bilibili/web/space/v1/space.proto
+-rw-r--r--   0        0        0     8294 2023-07-24 14:29:13.335177 bilirpc-1.2/bilirpc/bilibili/web/space/v1/space_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-24 14:29:13.335177 bilirpc-1.2/bilirpc/bilibili/web/space/v1/space_pb2_grpc.py
+-rw-r--r--   0        0        0     1724 2023-07-25 12:53:25.318154 bilirpc-1.2/bilirpc/tools.py
+-rw-r--r--   0        0        0      359 2023-07-25 13:00:01.802767 bilirpc-1.2/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 bilirpc-1.2/PKG-INFO
```

### Comparing `bilirpc-1.1/bilirpc/api.py` & `bilirpc-1.2/bilirpc/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 @Time    :   2022/9/23 17:34
 @Author  :   DMC ,
 """
 from typing import Optional
 
 import grpc
 
-from bilibili.app.dynamic.v2.dynamic_pb2 import (
+from bilirpc.bilibili.app.dynamic.v2.dynamic_pb2 import (
     DynAllReq,
     DynamicType,
     DynSpaceReq,
     DynDetailReq,
-    RepostListReq,
-    PlayerArgs
 )
 from loguru import logger
-from google.protobuf.json_format import MessageToJson
 
 from bilibili.app.dynamic.v2.dynamic_pb2_grpc import DynamicStub
 from bilirpc.tools import fakebuvid, make_metadata
 
 
 async def get_follow_dynamic(update_baseline: Optional[str] = None, access_token: str = None):
     try:
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/account/fission/v1/fission.proto` & `bilirpc-1.2/bilirpc/bilibili/account/fission/v1/fission.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/account/fission/v1/fission_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/account/fission/v1/fission_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/account/fission/v1/fission_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/account/fission/v1/fission_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.account.fission.v1 import fission_pb2 as bilibili_dot_account_dot_fission_dot_v1_dot_fission__pb2
+from bilirpc.bilibili.account.fission.v1 import fission_pb2 as bilibili_dot_account_dot_fission_dot_v1_dot_fission__pb2
 
 
 class FissionStub(object):
-    """Fission裂变
+    """Fission裂变
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -29,33 +29,33 @@
                 '/bilibili.account.fission.v1.Fission/Privacy',
                 request_serializer=bilibili_dot_account_dot_fission_dot_v1_dot_fission__pb2.PrivacyReq.SerializeToString,
                 response_deserializer=bilibili_dot_account_dot_fission_dot_v1_dot_fission__pb2.PrivacyReply.FromString,
                 )
 
 
 class FissionServicer(object):
-    """Fission裂变
+    """Fission裂变
     """
 
     def Entrance(self, request, context):
-        """活动入口
+        """活动入口
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Window(self, request, context):
-        """首页弹窗
+        """首页弹窗
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Privacy(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_FissionServicer_to_server(servicer, server):
@@ -79,15 +79,15 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bilibili.account.fission.v1.Fission', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Fission(object):
-    """Fission裂变
+    """Fission裂变
     """
 
     @staticmethod
     def Entrance(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/ad/v1/ad.proto` & `bilirpc-1.2/bilirpc/bilibili/ad/v1/ad.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/ad/v1/ad_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/ad/v1/ad_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/api/player/v1/player.proto` & `bilirpc-1.2/bilirpc/bilibili/api/player/v1/player.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/api/player/v1/player_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/api/player/v1/player_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/api/player/v1/player_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/api/player/v1/player_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.api.player.v1 import player_pb2 as bilibili_dot_api_dot_player_dot_v1_dot_player__pb2
+from bilirpc.bilibili.api.player.v1 import player_pb2 as bilibili_dot_api_dot_player_dot_v1_dot_player__pb2
 
 
 class HeartbeatStub(object):
     """心跳上报
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/api/probe/v1/probe.proto` & `bilirpc-1.2/bilirpc/bilibili/api/probe/v1/probe.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/api/probe/v1/probe_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/api/probe/v1/probe_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/api/probe/v1/probe_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/api/probe/v1/probe_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.api.probe.v1 import probe_pb2 as bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2
+from bilirpc.bilibili.api.probe.v1 import probe_pb2 as bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2
 
 
 class ProbeStub(object):
-    """服务可用性探针
+    """服务可用性探针
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -34,40 +34,40 @@
                 '/bilibili.api.probe.v1.Probe/TestSub',
                 request_serializer=bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2.ProbeSubReq.SerializeToString,
                 response_deserializer=bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2.ProbeSubReply.FromString,
                 )
 
 
 class ProbeServicer(object):
-    """服务可用性探针
+    """服务可用性探针
     """
 
     def TestCode(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def TestReq(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def TestStream(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def TestSub(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ProbeServicer_to_server(servicer, server):
@@ -96,15 +96,15 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bilibili.api.probe.v1.Probe', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Probe(object):
-    """服务可用性探针
+    """服务可用性探针
     """
 
     @staticmethod
     def TestCode(request,
             target,
             options=(),
             channel_credentials=None,
@@ -169,15 +169,15 @@
             bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2.ProbeSubReq.SerializeToString,
             bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2.ProbeSubReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class ProbeServiceStub(object):
-    """服务可用性探针
+    """服务可用性探针
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -206,47 +206,47 @@
                 '/bilibili.api.probe.v1.ProbeService/EchoPatch',
                 request_serializer=bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2.DynamicMessageUpdate.SerializeToString,
                 response_deserializer=bilibili_dot_api_dot_probe_dot_v1_dot_probe__pb2.DynamicMessageUpdate.FromString,
                 )
 
 
 class ProbeServiceServicer(object):
-    """服务可用性探针
+    """服务可用性探针
     """
 
     def Echo(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def EchoBody(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def EchoDelete(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def EchoError(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def EchoPatch(self, request, context):
-        """
+        """
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ProbeServiceServicer_to_server(servicer, server):
@@ -280,15 +280,15 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bilibili.api.probe.v1.ProbeService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class ProbeService(object):
-    """服务可用性探针
+    """服务可用性探针
     """
 
     @staticmethod
     def Echo(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/archive/middleware/v1/__pycache__/preload_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/app/archive/middleware/v1/__pycache__/preload_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/archive/middleware/v1/preload_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/archive/middleware/v1/preload_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/archive/v1/archive.proto` & `bilirpc-1.2/bilirpc/bilibili/app/archive/v1/archive.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/archive/v1/archive_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/archive/v1/archive_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/ad.proto` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/ad.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/ad_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/ad_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/card.proto` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/card.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/card_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/card_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/common.proto` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/common.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/common_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/common_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.card.v1 import ad_pb2 as bilibili_dot_app_dot_card_dot_v1_dot_ad__pb2
+from bilirpc.bilibili.app.card.v1 import ad_pb2 as bilibili_dot_app_dot_card_dot_v1_dot_ad__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bilibili/app/card/v1/common.proto\x12\x14\x62ilibili.app.card.v1\x1a\x1d\x62ilibili/app/card/v1/ad.proto\"\xb1\x01\n\x04\x41rgs\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\r\n\x05up_id\x18\x02 \x01(\x03\x12\x0f\n\x07up_name\x18\x03 \x01(\t\x12\x0b\n\x03rid\x18\x04 \x01(\x05\x12\r\n\x05rname\x18\x05 \x01(\t\x12\x0b\n\x03tid\x18\x06 \x01(\x03\x12\r\n\x05tname\x18\x07 \x01(\t\x12\x10\n\x08track_id\x18\x08 \x01(\t\x12\r\n\x05state\x18\t \x01(\t\x12\x15\n\rconverge_type\x18\n \x01(\x05\x12\x0b\n\x03\x61id\x18\x0b \x01(\x03\"x\n\x06\x41vatar\x12\r\n\x05\x63over\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x65vent\x18\x05 \x01(\t\x12\x10\n\x08\x65vent_v2\x18\x06 \x01(\t\x12\x15\n\rdefalut_cover\x18\x07 \x01(\x05\"\x9b\x05\n\x04\x42\x61se\x12\x11\n\tcard_type\x18\x01 \x01(\t\x12\x11\n\tcard_goto\x18\x02 \x01(\t\x12\x0c\n\x04goto\x18\x03 \x01(\t\x12\r\n\x05param\x18\x04 \x01(\t\x12\r\n\x05\x63over\x18\x05 \x01(\t\x12\r\n\x05title\x18\x06 \x01(\t\x12\x0b\n\x03uri\x18\x07 \x01(\t\x12\x35\n\x0bthree_point\x18\x08 \x01(\x0b\x32 .bilibili.app.card.v1.ThreePoint\x12(\n\x04\x61rgs\x18\t \x01(\x0b\x32\x1a.bilibili.app.card.v1.Args\x12\x35\n\x0bplayer_args\x18\n \x01(\x0b\x32 .bilibili.app.card.v1.PlayerArgs\x12\x0b\n\x03idx\x18\x0b \x01(\x03\x12-\n\x07\x61\x64_info\x18\x0c \x01(\x0b\x32\x1c.bilibili.app.card.v1.AdInfo\x12(\n\x04mask\x18\r \x01(\x0b\x32\x1a.bilibili.app.card.v1.Mask\x12\x11\n\tfrom_type\x18\x0e \x01(\t\x12:\n\x0ethree_point_v2\x18\x0f \x03(\x0b\x32\".bilibili.app.card.v1.ThreePointV2\x12:\n\x0ethree_point_v3\x18\x10 \x03(\x0b\x32\".bilibili.app.card.v1.ThreePointV3\x12\x31\n\x0b\x64\x65sc_button\x18\x11 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Button\x12:\n\x0ethree_point_v4\x18\x12 \x01(\x0b\x32\".bilibili.app.card.v1.ThreePointV4\x12-\n\x07up_args\x18\x13 \x01(\x0b\x32\x1c.bilibili.app.card.v1.UpArgs\"\xa5\x01\n\x06\x42utton\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\r\n\x05param\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\r\n\x05\x65vent\x18\x04 \x01(\t\x12\x10\n\x08selected\x18\x05 \x01(\x05\x12\x0c\n\x04type\x18\x06 \x01(\x05\x12\x10\n\x08\x65vent_v2\x18\x07 \x01(\t\x12\x30\n\x08relation\x18\x08 \x01(\x0b\x32\x1e.bilibili.app.card.v1.Relation\")\n\rDislikeReason\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\"o\n\nLikeButton\x12\x0b\n\x03\x41id\x18\x01 \x01(\x03\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\x12\x12\n\nshow_count\x18\x03 \x01(\x08\x12\r\n\x05\x65vent\x18\x04 \x01(\t\x12\x10\n\x08selected\x18\x05 \x01(\x05\x12\x10\n\x08\x65vent_v2\x18\x06 \x01(\t\"b\n\x04Mask\x12,\n\x06\x61vatar\x18\x01 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12,\n\x06\x62utton\x18\x02 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Button\"\xb0\x01\n\nPlayerArgs\x12\x0f\n\x07is_live\x18\x01 \x01(\x05\x12\x0b\n\x03\x61id\x18\x02 \x01(\x03\x12\x0b\n\x03\x63id\x18\x03 \x01(\x03\x12\x10\n\x08sub_type\x18\x04 \x01(\x05\x12\x0f\n\x07room_id\x18\x05 \x01(\x03\x12\r\n\x05\x65p_id\x18\x07 \x01(\x03\x12\x12\n\nis_preview\x18\x08 \x01(\x05\x12\x0c\n\x04type\x18\t \x01(\t\x12\x10\n\x08\x64uration\x18\n \x01(\x03\x12\x11\n\tseason_id\x18\x0b \x01(\x03\"\xd5\x02\n\x0bReasonStyle\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x12\n\ntext_color\x18\x02 \x01(\t\x12\x10\n\x08\x62g_color\x18\x03 \x01(\t\x12\x14\n\x0c\x62order_color\x18\x04 \x01(\t\x12\x10\n\x08icon_url\x18\x05 \x01(\t\x12\x18\n\x10text_color_night\x18\x06 \x01(\t\x12\x16\n\x0e\x62g_color_night\x18\x07 \x01(\t\x12\x1a\n\x12\x62order_color_night\x18\x08 \x01(\t\x12\x16\n\x0eicon_night_url\x18\t \x01(\t\x12\x10\n\x08\x62g_style\x18\n \x01(\x05\x12\x0b\n\x03uri\x18\x0b \x01(\t\x12\x13\n\x0bicon_bg_url\x18\x0c \x01(\t\x12\r\n\x05\x65vent\x18\r \x01(\t\x12\x10\n\x08\x65vent_v2\x18\x0e \x01(\t\x12\x17\n\x0fright_icon_type\x18\x0f \x01(\x05\x12\x16\n\x0eleft_icon_type\x18\x10 \x01(\t\"B\n\x08Relation\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x11\n\tis_follow\x18\x02 \x01(\x05\x12\x13\n\x0bis_followed\x18\x03 \x01(\x05\"\xbb\x02\n\nSharePlane\x12\r\n\x05title\x18\x01 \x01(\t\x12\x16\n\x0eshare_subtitle\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\r\n\x05\x63over\x18\x04 \x01(\t\x12\x0b\n\x03\x61id\x18\x05 \x01(\x03\x12\x0c\n\x04\x62vid\x18\x06 \x01(\t\x12?\n\x08share_to\x18\x07 \x03(\x0b\x32-.bilibili.app.card.v1.SharePlane.ShareToEntry\x12\x0e\n\x06\x61uthor\x18\x08 \x01(\t\x12\x11\n\tauthor_id\x18\t \x01(\x03\x12\x12\n\nshort_link\x18\n \x01(\t\x12\x13\n\x0bplay_number\x18\x0b \x01(\t\x12\x11\n\tfirst_cid\x18\x0c \x01(\x03\x1a.\n\x0cShareToEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"\x97\x01\n\nThreePoint\x12<\n\x0f\x64islike_reasons\x18\x01 \x03(\x0b\x32#.bilibili.app.card.v1.DislikeReason\x12\x36\n\tfeedbacks\x18\x02 \x03(\x0b\x32#.bilibili.app.card.v1.DislikeReason\x12\x13\n\x0bwatch_later\x18\x03 \x01(\x05\"\x7f\n\x0cThreePointV2\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x34\n\x07reasons\x18\x03 \x03(\x0b\x32#.bilibili.app.card.v1.DislikeReason\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\n\n\x02id\x18\x05 \x01(\x03\"\xef\x01\n\x0cThreePointV3\x12\r\n\x05title\x18\x01 \x01(\t\x12\x16\n\x0eselected_title\x18\x02 \x01(\t\x12\x10\n\x08subtitle\x18\x03 \x01(\t\x12\x34\n\x07reasons\x18\x04 \x03(\x0b\x32#.bilibili.app.card.v1.DislikeReason\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\n\n\x02id\x18\x06 \x01(\x03\x12\x10\n\x08selected\x18\x07 \x01(\x05\x12\x0c\n\x04icon\x18\x08 \x01(\t\x12\x15\n\rselected_icon\x18\t \x01(\t\x12\x0b\n\x03url\x18\n \x01(\t\x12\x12\n\ndefault_id\x18\x0b \x01(\x05\"|\n\x0cThreePointV4\x12\x35\n\x0bshare_plane\x18\x01 \x01(\x0b\x32 .bilibili.app.card.v1.SharePlane\x12\x35\n\x0bwatch_later\x18\x02 \x01(\x0b\x32 .bilibili.app.card.v1.WatchLater\"\xb9\x01\n\x02Up\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12,\n\x06\x61vatar\x18\x04 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12\x15\n\rofficial_icon\x18\x05 \x01(\x05\x12\x31\n\x0b\x64\x65sc_button\x18\x06 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Button\x12\x13\n\x0b\x63ooperation\x18\x07 \x01(\t\"K\n\x06UpArgs\x12\r\n\x05up_id\x18\x01 \x01(\x03\x12\x0f\n\x07up_name\x18\x02 \x01(\t\x12\x0f\n\x07up_face\x18\x03 \x01(\t\x12\x10\n\x08selected\x18\x04 \x01(\x03\"\'\n\nWatchLater\x12\x0b\n\x03\x61id\x18\x01 \x01(\x03\x12\x0c\n\x04\x62vid\x18\x02 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.card.v1.common_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/double.proto` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/double.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/double_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/double_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.card.v1 import common_pb2 as bilibili_dot_app_dot_card_dot_v1_dot_common__pb2
+from bilirpc.bilibili.app.card.v1 import common_pb2 as bilibili_dot_app_dot_card_dot_v1_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bilibili/app/card/v1/double.proto\x12\x14\x62ilibili.app.card.v1\x1a!bilibili/app/card/v1/common.proto\"\xc3\x01\n\x0b\x44oubleCards\x12<\n\x0esmall_cover_v2\x18\x01 \x01(\x0b\x32\".bilibili.app.card.v1.SmallCoverV2H\x00\x12\x34\n\none_pic_v2\x18\x02 \x01(\x0b\x32\x1e.bilibili.app.card.v1.OnePicV2H\x00\x12\x38\n\x0cthree_pic_v2\x18\x03 \x01(\x0b\x32 .bilibili.app.card.v1.ThreePicV2H\x00\x42\x06\n\x04\x43\x61rd\"\xf6\x04\n\x0cSmallCoverV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x11\n\tcover_gif\x18\x02 \x01(\t\x12\x12\n\ncover_blur\x18\x03 \x01(\x05\x12\x19\n\x11\x63over_left_text_1\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x05 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x06 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x07 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\x08 \x01(\t\x12\x18\n\x10\x63over_right_icon\x18\t \x01(\x05\x12$\n\x1c\x63over_right_background_color\x18\n \x01(\t\x12\x10\n\x08subtitle\x18\x0b \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x0c \x01(\t\x12\x13\n\x0brcmd_reason\x18\r \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x0e \x01(\t\x12,\n\x06\x61vatar\x18\x0f \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12\x15\n\rofficial_icon\x18\x10 \x01(\x05\x12\x10\n\x08\x63\x61n_play\x18\x11 \x01(\x05\x12<\n\x11rcmd_reason_style\x18\x12 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12?\n\x14rcmd_reason_style_v2\x18\x13 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x35\n\x0blike_button\x18\x14 \x01(\x0b\x32 .bilibili.app.card.v1.LikeButton\"\xc3\x02\n\x0cSmallCoverV3\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12,\n\x06\x61vatar\x18\x02 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12\x17\n\x0f\x63over_left_text\x18\x03 \x01(\t\x12\x38\n\x12\x63over_right_button\x18\x04 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Button\x12\x13\n\x0brcmd_reason\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x06 \x01(\t\x12\x15\n\rofficial_icon\x18\x07 \x01(\x05\x12\x10\n\x08\x63\x61n_play\x18\x08 \x01(\x05\x12<\n\x11rcmd_reason_style\x18\t \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"e\n\rMiddleCoverV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\r\n\x05ratio\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x04 \x01(\t\"\xbe\x03\n\x0cLargeCoverV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12,\n\x06\x61vatar\x18\x02 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12\r\n\x05\x62\x61\x64ge\x18\x03 \x01(\t\x12\x38\n\x12\x63over_right_button\x18\x04 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Button\x12\x19\n\x11\x63over_left_text_1\x18\x05 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x06 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x07 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x08 \x01(\x05\x12\x13\n\x0brcmd_reason\x18\t \x01(\t\x12\x15\n\rofficial_icon\x18\n \x01(\x05\x12\x10\n\x08\x63\x61n_play\x18\x0b \x01(\x05\x12<\n\x11rcmd_reason_style\x18\x0c \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x10\n\x08show_top\x18\r \x01(\x05\x12\x13\n\x0bshow_bottom\x18\x0e \x01(\x05\"\xa6\x01\n\x0bThreeItemV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x12\n\ntitle_icon\x18\x02 \x01(\x05\x12\x10\n\x08more_uri\x18\x03 \x01(\t\x12\x11\n\tmore_text\x18\x04 \x01(\t\x12\x34\n\x05items\x18\x05 \x03(\x0b\x32%.bilibili.app.card.v1.ThreeItemV2Item\"\xb7\x01\n\x0fThreeItemV2Item\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x17\n\x0f\x63over_left_icon\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65sc_text_1\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65sc_icon_1\x18\x04 \x01(\x05\x12\x13\n\x0b\x64\x65sc_text_2\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65sc_icon_2\x18\x06 \x01(\x05\x12\r\n\x05\x62\x61\x64ge\x18\x07 \x01(\t\"\x8e\x01\n\x0cSmallCoverV4\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x13\n\x0b\x63over_badge\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x18\n\x10title_right_text\x18\x04 \x01(\t\x12\x17\n\x0ftitle_right_pic\x18\x05 \x01(\x05\"i\n\tTwoItemV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x32\n\x05items\x18\x02 \x03(\x0b\x32#.bilibili.app.card.v1.TwoItemV2Item\"~\n\rTwoItemV2Item\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\r\n\x05\x62\x61\x64ge\x18\x02 \x01(\t\x12\x19\n\x11\x63over_left_text_1\x18\x03 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x04 \x01(\x05\"\x8c\x01\n\tMultiItem\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x10\n\x08more_uri\x18\x02 \x01(\t\x12\x11\n\tmore_text\x18\x03 \x01(\t\x12\x30\n\x05items\x18\x04 \x03(\x0b\x32!.bilibili.app.card.v1.DoubleCards\"\xdc\x03\n\nThreePicV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x12\n\nleft_cover\x18\x02 \x01(\t\x12\x15\n\rright_cover_1\x18\x03 \x01(\t\x12\x15\n\rright_cover_2\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_text_1\x18\x05 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x06 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x07 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x08 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\t \x01(\t\x12\x18\n\x10\x63over_right_icon\x18\n \x01(\x05\x12$\n\x1c\x63over_right_background_color\x18\x0b \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x0c \x01(\t\x12\x13\n\x0brcmd_reason\x18\r \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x0e \x01(\t\x12,\n\x06\x61vatar\x18\x0f \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12<\n\x11rcmd_reason_style\x18\x10 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\xd4\x02\n\x08OnePicV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x19\n\x11\x63over_left_icon_1\x18\x02 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x03 \x01(\t\x12\x18\n\x10\x63over_right_text\x18\x04 \x01(\t\x12\x18\n\x10\x63over_right_icon\x18\x05 \x01(\x05\x12$\n\x1c\x63over_right_background_color\x18\x06 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x07 \x01(\t\x12\x13\n\x0brcmd_reason\x18\x08 \x01(\t\x12,\n\x06\x61vatar\x18\t \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12<\n\x11rcmd_reason_style\x18\n \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\xab\x03\n\x0cLargeCoverV3\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x11\n\tcover_gif\x18\x02 \x01(\t\x12,\n\x06\x61vatar\x18\x03 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12@\n\x15top_rcmd_reason_style\x18\x04 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x43\n\x18\x62ottom_rcmd_reason_style\x18\x05 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x19\n\x11\x63over_left_text_1\x18\x06 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x07 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x08 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\t \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\n \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x0b \x01(\t\x12\x15\n\rofficial_icon\x18\x0c \x01(\x05\"\x8b\x03\n\nThreePicV3\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x12\n\nleft_cover\x18\x02 \x01(\t\x12\x15\n\rright_cover_1\x18\x03 \x01(\t\x12\x15\n\rright_cover_2\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_text_1\x18\x05 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x06 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x07 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x08 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\t \x01(\t\x12\x18\n\x10\x63over_right_icon\x18\n \x01(\x05\x12$\n\x1c\x63over_right_background_color\x18\x0b \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x0c \x01(\t\x12<\n\x11rcmd_reason_style\x18\r \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\x91\x02\n\x08OnePicV3\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x19\n\x11\x63over_left_text_1\x18\x02 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x03 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\x04 \x01(\t\x12\x18\n\x10\x63over_right_icon\x18\x05 \x01(\x05\x12$\n\x1c\x63over_right_background_color\x18\x06 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x07 \x01(\t\x12<\n\x11rcmd_reason_style\x18\x08 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"F\n\x0cSmallCoverV7\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\"\xdb\x03\n\x0cSmallCoverV9\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x19\n\x11\x63over_left_text_1\x18\x02 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x03 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x05 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\x06 \x01(\t\x12\x18\n\x10\x63over_right_icon\x18\x07 \x01(\x05\x12\x10\n\x08\x63\x61n_play\x18\x08 \x01(\x05\x12<\n\x11rcmd_reason_style\x18\t \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12$\n\x02up\x18\n \x01(\x0b\x32\x18.bilibili.app.card.v1.Up\x12\x41\n\x16left_cover_badge_style\x18\x0b \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12H\n\x1dleft_bottom_rcmd_reason_style\x18\x0c \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\xe3\x02\n\x14SmallCoverConvergeV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x19\n\x11\x63over_left_text_1\x18\x02 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x03 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x05 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\x06 \x01(\t\x12\x1c\n\x14\x63over_right_top_text\x18\x07 \x01(\t\x12<\n\x11rcmd_reason_style\x18\x08 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12?\n\x14rcmd_reason_style_v2\x18\t \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\xc0\x01\n\x13SmallChannelSpecial\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x10\n\x08\x62g_cover\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65sc_1\x18\x03 \x01(\t\x12\x0e\n\x06\x64\x65sc_2\x18\x04 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x05 \x01(\t\x12>\n\x13rcmd_reason_style_2\x18\x06 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyleb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.card.v1.double_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/single.proto` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/single.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/card/v1/single_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/card/v1/single_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.card.v1 import common_pb2 as bilibili_dot_app_dot_card_dot_v1_dot_common__pb2
+from bilirpc.bilibili.app.card.v1 import common_pb2 as bilibili_dot_app_dot_card_dot_v1_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bilibili/app/card/v1/single.proto\x12\x14\x62ilibili.app.card.v1\x1a!bilibili/app/card/v1/common.proto\"\xbc\x04\n\x0cSmallCoverV5\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x11\n\tcover_gif\x18\x02 \x01(\t\x12$\n\x02up\x18\x03 \x01(\x0b\x32\x18.bilibili.app.card.v1.Up\x12\x1a\n\x12\x63over_right_text_1\x18\x04 \x01(\t\x12\x14\n\x0cright_desc_1\x18\x05 \x01(\t\x12\x14\n\x0cright_desc_2\x18\x06 \x01(\t\x12<\n\x11rcmd_reason_style\x18\x07 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12?\n\x10hotword_entrance\x18\x08 \x01(\x0b\x32%.bilibili.app.card.v1.HotwordEntrance\x12<\n\x11\x63orner_mark_style\x18\t \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x14\n\x0cright_icon_1\x18\n \x01(\x05\x12\x14\n\x0cright_icon_2\x18\x0b \x01(\x05\x12\x41\n\x16left_corner_mark_style\x18\x0c \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12,\n$cover_right_text_content_description\x18\r \x01(\t\x12\'\n\x1fright_desc1_content_description\x18\x0e \x01(\t\"\xb9\x04\n\x0eSmallCoverV5Ad\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x11\n\tcover_gif\x18\x02 \x01(\t\x12$\n\x02up\x18\x03 \x01(\x0b\x32\x18.bilibili.app.card.v1.Up\x12\x19\n\x11\x63over_right_text1\x18\x04 \x01(\t\x12\x13\n\x0bright_desc1\x18\x05 \x01(\t\x12\x13\n\x0bright_desc2\x18\x06 \x01(\t\x12<\n\x11rcmd_reason_style\x18\x07 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12?\n\x10hotword_entrance\x18\x08 \x01(\x0b\x32%.bilibili.app.card.v1.HotwordEntrance\x12<\n\x11\x63orner_mark_style\x18\t \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x13\n\x0bright_icon1\x18\n \x01(\x05\x12\x13\n\x0bright_icon2\x18\x0b \x01(\x05\x12\x41\n\x16left_corner_mark_style\x18\x0c \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12,\n$cover_right_text_content_description\x18\r \x01(\t\x12\'\n\x1fright_desc1_content_description\x18\x0e \x01(\t\"U\n\x0fHotwordEntrance\x12\x12\n\nhotword_id\x18\x01 \x01(\x03\x12\x10\n\x08hot_text\x18\x02 \x01(\t\x12\x0e\n\x06h5_url\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\"\x9d\x06\n\x0cLargeCoverV1\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x11\n\tcover_gif\x18\x02 \x01(\t\x12,\n\x06\x61vatar\x18\x03 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Avatar\x12\x19\n\x11\x63over_left_text_1\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_text_2\x18\x05 \x01(\t\x12\x19\n\x11\x63over_left_text_3\x18\x06 \x01(\t\x12\x13\n\x0b\x63over_badge\x18\x07 \x01(\t\x12\x17\n\x0ftop_rcmd_reason\x18\x08 \x01(\t\x12\x1a\n\x12\x62ottom_rcmd_reason\x18\t \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\n \x01(\t\x12\x15\n\rofficial_icon\x18\x0b \x01(\x05\x12\x10\n\x08\x63\x61n_play\x18\x0c \x01(\x05\x12@\n\x15top_rcmd_reason_style\x18\r \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x43\n\x18\x62ottom_rcmd_reason_style\x18\x0e \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12?\n\x14rcmd_reason_style_v2\x18\x0f \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x41\n\x16left_cover_badge_style\x18\x10 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x42\n\x17right_cover_badge_style\x18\x11 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x15\n\rcover_badge_2\x18\x12 \x01(\t\x12\x35\n\x0blike_button\x18\x13 \x01(\x0b\x32 .bilibili.app.card.v1.LikeButton\x12\x19\n\x11title_single_line\x18\x14 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\x15 \x01(\t\"\xb0\x01\n\x0eThreeItemAllV2\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12@\n\x15top_rcmd_reason_style\x18\x02 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x32\n\x04item\x18\x03 \x03(\x0b\x32$.bilibili.app.card.v1.TwoItemHV1Item\"\xd2\x01\n\x0eTwoItemHV1Item\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\r\n\x05param\x18\x04 \x01(\t\x12(\n\x04\x61rgs\x18\x05 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Args\x12\x0c\n\x04goto\x18\x06 \x01(\t\x12\x19\n\x11\x63over_left_text_1\x18\x07 \x01(\t\x12\x19\n\x11\x63over_left_icon_1\x18\x08 \x01(\x05\x12\x18\n\x10\x63over_right_text\x18\t \x01(\t\"\xae\x01\n\x0bRcmdOneItem\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12=\n\x12topRcmdReasonStyle\x18\x02 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\x12\x36\n\x04item\x18\x03 \x01(\x0b\x32(.bilibili.app.card.v1.SmallCoverRcmdItem\"\xae\x02\n\x12SmallCoverRcmdItem\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\r\n\x05param\x18\x04 \x01(\t\x12\x0c\n\x04goto\x18\x05 \x01(\t\x12\x17\n\x0f\x63overRightText1\x18\x06 \x01(\t\x12\x12\n\nrightDesc1\x18\x07 \x01(\t\x12\x12\n\nrightDesc2\x18\x08 \x01(\t\x12\x10\n\x08\x63overGif\x18\t \x01(\t\x12\x12\n\nrightIcon1\x18\n \x01(\x05\x12\x12\n\nrightIcon2\x18\x0b \x01(\x05\x12,\n$cover_right_text_content_description\x18\x0c \x01(\t\x12\'\n\x1fright_desc1_content_description\x18\r \x01(\t\"\xa3\x01\n\x0bThreeItemV1\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x11\n\ttitleIcon\x18\x02 \x01(\x05\x12\x0f\n\x07moreUri\x18\x03 \x01(\t\x12\x10\n\x08moreText\x18\x04 \x01(\t\x12\x34\n\x05items\x18\x05 \x03(\x0b\x32%.bilibili.app.card.v1.ThreeItemV1Item\"\x96\x01\n\x0fThreeItemV1Item\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x15\n\rcoverLeftText\x18\x02 \x01(\t\x12\x15\n\rcoverLeftIcon\x18\x03 \x01(\x05\x12\r\n\x05\x64\x65sc1\x18\x04 \x01(\t\x12\r\n\x05\x64\x65sc2\x18\x05 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x06 \x01(\t\"G\n\x0cHotTopicItem\x12\r\n\x05\x63over\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\r\n\x05param\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\"u\n\x08HotTopic\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x31\n\x05items\x18\x03 \x03(\x0b\x32\".bilibili.app.card.v1.HotTopicItem\"\xfd\x01\n\nDynamicHot\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x16\n\x0etop_left_title\x18\x02 \x01(\t\x12\r\n\x05\x64\x65sc1\x18\x03 \x01(\t\x12\r\n\x05\x64\x65sc2\x18\x04 \x01(\t\x12\x10\n\x08more_uri\x18\x05 \x01(\t\x12\x11\n\tmore_text\x18\x06 \x01(\t\x12\x0e\n\x06\x63overs\x18\x07 \x03(\t\x12\x18\n\x10\x63over_right_text\x18\x08 \x01(\t\x12@\n\x15top_rcmd_reason_style\x18\t \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\x95\x01\n\rMiddleCoverV3\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\r\n\x05\x64\x65sc1\x18\x02 \x01(\t\x12\r\n\x05\x64\x65sc2\x18\x03 \x01(\t\x12<\n\x11\x63over_badge_style\x18\x04 \x01(\x0b\x32!.bilibili.app.card.v1.ReasonStyle\"\xb8\x02\n\x0cLargeCoverV4\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x19\n\x11\x63over_left_text_1\x18\x02 \x01(\t\x12\x19\n\x11\x63over_left_text_2\x18\x03 \x01(\t\x12\x19\n\x11\x63over_left_text_3\x18\x04 \x01(\t\x12\x13\n\x0b\x63over_badge\x18\x05 \x01(\t\x12\x10\n\x08\x63\x61n_play\x18\x06 \x01(\x05\x12$\n\x02up\x18\x07 \x01(\x0b\x32\x18.bilibili.app.card.v1.Up\x12\x12\n\nshort_link\x18\x08 \x01(\t\x12\x16\n\x0eshare_subtitle\x18\t \x01(\t\x12\x13\n\x0bplay_number\x18\n \x01(\t\x12\x0c\n\x04\x62vid\x18\x0b \x01(\t\x12\x11\n\tsub_param\x18\x0c \x01(\t\"q\n\x12PopularTopEntrance\x12(\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1a.bilibili.app.card.v1.Base\x12\x31\n\x05items\x18\x02 \x03(\x0b\x32\".bilibili.app.card.v1.EntranceItem\"\xb3\x01\n\x0c\x45ntranceItem\x12\x0c\n\x04goto\x18\x01 \x01(\t\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\x11\n\tmodule_id\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\x12\x13\n\x0b\x65ntrance_id\x18\x06 \x01(\x03\x12,\n\x06\x62ubble\x18\x07 \x01(\x0b\x32\x1c.bilibili.app.card.v1.Bubble\x12\x15\n\rentrance_type\x18\x08 \x01(\x05\"@\n\x06\x42ubble\x12\x16\n\x0e\x62ubble_content\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\r\n\x05stime\x18\x03 \x01(\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.card.v1.single_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/click/v1/heartbeat.proto` & `bilirpc-1.2/bilirpc/bilibili/app/click/v1/heartbeat.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/click/v1/heartbeat_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/click/v1/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/click/v1/heartbeat_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/click/v1/heartbeat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/download_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/download_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0bilibili/app/distribution/setting/download.proto\x12*bilibili.app.distribution.setting.download\x1a/bilibili/app/distribution/v1/distribution.proto\"e\n\x16\x44ownloadSettingsConfig\x12K\n\x1a\x65nable_download_auto_start\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.download_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/dynamic_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/dynamic_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/bilibili/app/distribution/setting/dynamic.proto\x12)bilibili.app.distribution.setting.dynamic\x1a/bilibili/app/distribution/v1/distribution.proto\"J\n\x0f\x44ynamicAutoPlay\x12\x37\n\x05value\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\"d\n\x13\x44ynamicDeviceConfig\x12M\n\tauto_play\x18\x01 \x01(\x0b\x32:.bilibili.app.distribution.setting.dynamic.DynamicAutoPlayb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.dynamic_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/experimental.proto` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/experimental.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/experimental_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/experimental_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4bilibili/app/distribution/setting/experimental.proto\x12.bilibili.app.distribution.setting.experimental\x1a/bilibili/app/distribution/v1/distribution.proto\"F\n\rDynamicSelect\x12\x35\n\x04\x66old\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"u\n\x03\x45xp\x12\x34\n\x02id\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12\x38\n\x06\x62ucket\x18\x02 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int32Value\"\x90\x01\n\x12\x45xperimentalConfig\x12\x37\n\x04\x66lag\x18\x01 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12\x41\n\x04\x65xps\x18\x02 \x03(\x0b\x32\x33.bilibili.app.distribution.setting.experimental.Exp\"\xb5\x01\n\x11MultipleTusConfig\x12I\n\x08top_left\x18\x01 \x01(\x0b\x32\x37.bilibili.app.distribution.setting.experimental.TopLeft\x12U\n\x0e\x64ynamic_select\x18\x02 \x01(\x0b\x32=.bilibili.app.distribution.setting.experimental.DynamicSelect\"\x96\x07\n\x07TopLeft\x12\x36\n\x03url\x18\x01 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12I\n\x16story_foreground_image\x18\x02 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12I\n\x16story_background_image\x18\x03 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12J\n\x17listen_foreground_image\x18\x04 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12J\n\x17listen_background_image\x18\x05 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12M\n\x1aios_story_foreground_image\x18\x06 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12M\n\x1aios_story_background_image\x18\x07 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12N\n\x1bios_listen_foreground_image\x18\x08 \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12N\n\x1bios_listen_background_image\x18\t \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12\x37\n\x04goto\x18\n \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12\x39\n\x06url_v2\x18\x0b \x01(\x0b\x32).bilibili.app.distribution.v1.StringValue\x12\x39\n\x07goto_v2\x18\x0c \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12\x38\n\x05\x62\x61\x64ge\x18\r \x01(\x0b\x32).bilibili.app.distribution.v1.StringValueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.experimental_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/internaldevice_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/internaldevice_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6bilibili/app/distribution/setting/internaldevice.proto\x12\x30\x62ilibili.app.distribution.setting.internaldevice\x1a/bilibili/app/distribution/v1/distribution.proto\"M\n\x14InternalDeviceConfig\x12\x35\n\x03\x66ts\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Valueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.internaldevice_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/night_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/night_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-bilibili/app/distribution/setting/night.proto\x12\'bilibili.app.distribution.setting.night\x1a/bilibili/app/distribution/v1/distribution.proto\"^\n\x13NightSettingsConfig\x12G\n\x16is_night_follow_system\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.night_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/other.proto` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/other.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/other_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/other_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-bilibili/app/distribution/setting/other.proto\x12\'bilibili.app.distribution.setting.other\x1a/bilibili/app/distribution/v1/distribution.proto\"\xdb\x04\n\x13OtherSettingsConfig\x12@\n\x0ewatermark_type\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12H\n\x16web_image_quality_type\x18\x02 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12G\n\x16\x65nable_read_pasteboard\x18\x03 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12@\n\x0fpaste_auto_jump\x18\x04 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12K\n\x1amini_screen_play_when_back\x18\x05 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x46\n\x15\x65nable_resume_playing\x18\x06 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12H\n\x17\x65nable_wifi_auto_update\x18\x07 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12N\n\x1d\x65nable_guide_screenshot_share\x18\x08 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.other_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/pegasus.proto` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/pegasus.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/pegasus_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/pegasus_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/bilibili/app/distribution/setting/pegasus.proto\x12)bilibili.app.distribution.setting.pegasus\x1a/bilibili/app/distribution/v1/distribution.proto\"H\n\rFeedModeValue\x12\x37\n\x05value\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\"\xa7\x02\n\x0fPegasusAutoPlay\x12\x38\n\x06single\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12\x38\n\x06\x64ouble\x18\x02 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12O\n\x1esingle_affected_by_server_side\x18\x03 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12O\n\x1e\x64ouble_affected_by_server_side\x18\x04 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"\x97\x01\n\x12PegasusColumnValue\x12\x37\n\x05value\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12H\n\x17\x61\x66\x66\x65\x63ted_by_server_side\x18\x02 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"\xfb\x01\n\x13PegasusDeviceConfig\x12M\n\x06\x63olumn\x18\x01 \x01(\x0b\x32=.bilibili.app.distribution.setting.pegasus.PegasusColumnValue\x12\x46\n\x04mode\x18\x02 \x01(\x0b\x32\x38.bilibili.app.distribution.setting.pegasus.FeedModeValue\x12M\n\tauto_play\x18\x03 \x01(\x0b\x32:.bilibili.app.distribution.setting.pegasus.PegasusAutoPlayb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.pegasus_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/play.proto` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/play.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/play_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/play_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,bilibili/app/distribution/setting/play.proto\x12&bilibili.app.distribution.setting.play\x1a/bilibili/app/distribution/v1/distribution.proto\"\xd8\x02\n\x0f\x43loudPlayConfig\x12@\n\x0f\x65nable_panorama\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12=\n\x0c\x65nable_dolby\x18\x02 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12=\n\x0c\x65nable_shake\x18\x03 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x42\n\x11\x65nable_background\x18\x04 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x41\n\x10\x65nable_loss_less\x18\x05 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"\xec\x07\n\nPlayConfig\x12\x41\n\x10should_auto_play\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12G\n\x16should_auto_fullscreen\x18\x02 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x45\n\x14\x65nable_playurl_https\x18\x03 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12K\n\x1a\x65nable_danmaku_interaction\x18\x04 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x45\n\x13small_screen_status\x18\x05 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12G\n\x15player_codec_mode_key\x18\x06 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12M\n\x1c\x65nable_gravity_rotate_screen\x18\x07 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12J\n\x19\x65nable_danmaku_monospaced\x18\x08 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x45\n\x14\x65nable_edit_subtitle\x18\t \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12@\n\x0f\x65nable_subtitle\x18\n \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12>\n\x0c\x63olor_filter\x18\x0b \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12\x42\n\x11should_auto_story\x18\x0c \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12\x45\n\x14landscape_auto_story\x18\r \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12?\n\x0evolume_balance\x18\x0e \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"_\n\x12SpecificPlayConfig\x12I\n\x18\x65nable_segmented_section\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.play_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/privacy_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/privacy_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/bilibili/app/distribution/setting/privacy.proto\x12)bilibili.app.distribution.setting.privacy\x1a/bilibili/app/distribution/v1/distribution.proto\"_\n\x18MidPrivacySettingsConfig\x12\x43\n\x12recommend_to_known\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"\x9c\x01\n\x15PrivacySettingsConfig\x12\x43\n\x12\x61\x64_recommand_store\x18\x01 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\x12>\n\rsensor_access\x18\x02 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValueb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.privacy_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/setting/search_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/setting/search_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.bilibili/app/distribution/setting/search.proto\x12(bilibili.app.distribution.setting.search\x1a/bilibili/app/distribution/v1/distribution.proto\"\x93\x01\n\x0eSearchAutoPlay\x12\x37\n\x05value\x18\x01 \x01(\x0b\x32(.bilibili.app.distribution.v1.Int64Value\x12H\n\x17\x61\x66\x66\x65\x63ted_by_server_side\x18\x02 \x01(\x0b\x32\'.bilibili.app.distribution.v1.BoolValue\"a\n\x12SearchDeviceConfig\x12K\n\tauto_play\x18\x01 \x01(\x0b\x32\x38.bilibili.app.distribution.setting.search.SearchAutoPlayb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.distribution.setting.search_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/v1/distribution.proto` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/v1/distribution.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/v1/distribution_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/v1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/distribution/v1/distribution_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/distribution/v1/distribution_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
+from bilirpc.bilibili.app.distribution.v1 import distribution_pb2 as bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2
 
 
 class DistributionStub(object):
-    """APP配置
+    """APP配置
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -29,33 +29,33 @@
                 '/bilibili.app.distribution.v1.Distribution/UserPreference',
                 request_serializer=bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2.UserPreferenceReq.SerializeToString,
                 response_deserializer=bilibili_dot_app_dot_distribution_dot_v1_dot_distribution__pb2.UserPreferenceReply.FromString,
                 )
 
 
 class DistributionServicer(object):
-    """APP配置
+    """APP配置
     """
 
     def GetUserPreference(self, request, context):
-        """获取云端储存的用户偏好
+        """获取云端储存的用户偏好
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetUserPreference(self, request, context):
-        """设定用户偏好
+        """设定用户偏好
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UserPreference(self, request, context):
-        """获取云控配置
+        """获取云控配置
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_DistributionServicer_to_server(servicer, server):
@@ -79,15 +79,15 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bilibili.app.distribution.v1.Distribution', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Distribution(object):
-    """APP配置
+    """APP配置
     """
 
     @staticmethod
     def GetUserPreference(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/common/dynamic_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/common/dynamic_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2_grpc.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/__pycache__/dynamic_pb2_grpc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/dynamic.proto` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/dynamic.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%bilibili/app/dynamic/v1/dynamic.proto\x12\x17\x62ilibili.app.dynamic.v1\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\"{\n\x10\x41\x64\x64ressComponent\x12\x0e\n\x06nation\x18\x01 \x01(\t\x12\x10\n\x08province\x18\x02 \x01(\t\x12\x0c\n\x04\x63ity\x18\x03 \x01(\t\x12\x10\n\x08\x64istrict\x18\x04 \x01(\t\x12\x0e\n\x06street\x18\x05 \x01(\t\x12\x15\n\rstreet_number\x18\x06 \x01(\t\"y\n\x06\x41\x64Info\x12\x13\n\x0bnation_code\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x64\x63ode\x18\x02 \x01(\t\x12\x11\n\tcity_code\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x03gps\x18\x05 \x01(\x0b\x32\x1c.bilibili.app.dynamic.v1.Gps\"\x8e\x01\n\rCardCurrBatch\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x0e\n\x06text_1\x18\x04 \x01(\t\x12\x0e\n\x06text_2\x18\x05 \x01(\t\x12\x32\n\x05\x62\x61\x64ge\x18\x06 \x01(\x0b\x32#.bilibili.app.dynamic.v1.VideoBadge\"\x8d\x01\n\x0e\x43\x61rdCurrSeason\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x0e\n\x06text_1\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x05 \x01(\t\x12\x32\n\x05\x62\x61\x64ge\x18\x06 \x01(\x0b\x32#.bilibili.app.dynamic.v1.VideoBadge\"\xf6\x03\n\x07\x43\x61rdPGC\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x19\n\x11\x63over_left_text_1\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_text_2\x18\x05 \x01(\t\x12\x19\n\x11\x63over_left_text_3\x18\x06 \x01(\t\x12\x0b\n\x03\x63id\x18\x07 \x01(\x03\x12\x11\n\tseason_id\x18\x08 \x01(\x03\x12\x0c\n\x04\x65pid\x18\t \x01(\x03\x12\x0b\n\x03\x61id\x18\n \x01(\x03\x12\x36\n\nmedia_type\x18\x0b \x01(\x0e\x32\".bilibili.app.dynamic.v1.MediaType\x12\x37\n\x08sub_type\x18\x0c \x01(\x0e\x32%.bilibili.app.dynamic.v1.VideoSubType\x12\x12\n\nis_preview\x18\r \x01(\x05\x12\x35\n\tdimension\x18\x0e \x01(\x0b\x32\".bilibili.app.dynamic.v1.Dimension\x12\x32\n\x05\x62\x61\x64ge\x18\x0f \x03(\x0b\x32#.bilibili.app.dynamic.v1.VideoBadge\x12\x10\n\x08\x63\x61n_play\x18\x10 \x01(\x05\x12\x32\n\x06season\x18\x11 \x01(\x0b\x32\".bilibili.app.dynamic.v1.PGCSeason\"\xd5\x02\n\x07\x43\x61rdUGC\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x19\n\x11\x63over_left_text_1\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_text_2\x18\x05 \x01(\t\x12\x19\n\x11\x63over_left_text_3\x18\x06 \x01(\t\x12\x0c\n\x04\x61vid\x18\x07 \x01(\x03\x12\x0b\n\x03\x63id\x18\x08 \x01(\x03\x12\x36\n\nmedia_type\x18\t \x01(\x0e\x32\".bilibili.app.dynamic.v1.MediaType\x12\x35\n\tdimension\x18\n \x01(\x0b\x32\".bilibili.app.dynamic.v1.Dimension\x12\x32\n\x05\x62\x61\x64ge\x18\x0b \x03(\x0b\x32#.bilibili.app.dynamic.v1.VideoBadge\x12\x10\n\x08\x63\x61n_play\x18\x0c \x01(\x05\"<\n\x0b\x44\x65\x63oCardFan\x12\x0e\n\x06is_fan\x18\x01 \x01(\x05\x12\x0e\n\x06number\x18\x02 \x01(\x05\x12\r\n\x05\x63olor\x18\x03 \x01(\t\"q\n\x0c\x44\x65\x63orateCard\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x63\x61rd_url\x18\x02 \x01(\t\x12\x10\n\x08jump_url\x18\x03 \x01(\t\x12\x31\n\x03\x66\x61n\x18\x04 \x01(\x0b\x32$.bilibili.app.dynamic.v1.DecoCardFan\"^\n\x0b\x44\x65scription\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x12\n\nemoji_type\x18\x04 \x01(\t\x12\x12\n\ngoods_type\x18\x05 \x01(\t\":\n\tDimension\x12\x0e\n\x06height\x18\x01 \x01(\x03\x12\r\n\x05width\x18\x02 \x01(\x03\x12\x0e\n\x06rotate\x18\x03 \x01(\x03\"\xb4\x01\n\x0b\x44ynamicItem\x12\x11\n\tcard_type\x18\x01 \x01(\t\x12\x11\n\titem_type\x18\x02 \x01(\t\x12\x30\n\x07modules\x18\x03 \x03(\x0b\x32\x1f.bilibili.app.dynamic.v1.Module\x12\x12\n\ndyn_id_str\x18\x04 \x01(\t\x12\x17\n\x0forig_dyn_id_str\x18\x05 \x01(\t\x12\x0e\n\x06r_type\x18\x06 \x01(\x05\x12\x10\n\x08has_fold\x18\x07 \x01(\x05\"E\n\x0f\x44ynDetailsReply\x12\x32\n\x04list\x18\x01 \x03(\x0b\x32$.bilibili.app.dynamic.v1.DynamicItem\"\x89\x01\n\rDynDetailsReq\x12\x16\n\x0eteenagers_mode\x18\x01 \x01(\x05\x12\x13\n\x0b\x64ynamic_ids\x18\x02 \x01(\t\x12\n\n\x02qn\x18\x03 \x01(\x05\x12\r\n\x05\x66nver\x18\x04 \x01(\x05\x12\r\n\x05\x66nval\x18\x05 \x01(\x05\x12\x12\n\nforce_host\x18\x06 \x01(\x05\x12\r\n\x05\x66ourk\x18\x07 \x01(\x05\"P\n\x17\x44ynMixUpListSearchReply\x12\x35\n\x05items\x18\x01 \x03(\x0b\x32&.bilibili.app.dynamic.v1.MixUpListItem\"%\n\x15\x44ynMixUpListSearchReq\x12\x0c\n\x04name\x18\x01 \x01(\t\"o\n\x19\x44ynMixUpListViewMoreReply\x12\x35\n\x05items\x18\x01 \x03(\x0b\x32&.bilibili.app.dynamic.v1.MixUpListItem\x12\x1b\n\x13search_default_text\x18\x02 \x01(\t\"\x9d\x01\n\x0e\x44ynOurCityItem\x12\x11\n\tcard_type\x18\x01 \x01(\t\x12\x0e\n\x06\x64yn_id\x18\x02 \x01(\x03\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12:\n\x07modules\x18\x04 \x03(\x0b\x32).bilibili.app.dynamic.v1.DynOurCityModule\x12\x0b\n\x03rid\x18\x05 \x01(\x03\x12\x12\n\ndebug_info\x18\x06 \x01(\t\"\xd8\x02\n\x10\x44ynOurCityModule\x12\x13\n\x0bmodule_type\x18\x01 \x01(\t\x12\x46\n\x0cmodule_cover\x18\x02 \x01(\x0b\x32..bilibili.app.dynamic.v1.DynOurCityModuleCoverH\x00\x12\x44\n\x0bmodule_desc\x18\x03 \x01(\x0b\x32-.bilibili.app.dynamic.v1.DynOurCityModuleDescH\x00\x12H\n\rmodule_author\x18\x04 \x01(\x0b\x32/.bilibili.app.dynamic.v1.DynOurCityModuleAuthorH\x00\x12H\n\rmodule_extend\x18\x05 \x01(\x0b\x32/.bilibili.app.dynamic.v1.DynOurCityModuleExtendH\x00\x42\r\n\x0bmodule_item\"N\n\x16\x44ynOurCityModuleAuthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x66\x61\x63\x65\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\"\xf1\x01\n\x15\x44ynOurCityModuleCover\x12\x0e\n\x06\x63overs\x18\x01 \x03(\t\x12\r\n\x05style\x18\x02 \x01(\x05\x12\x19\n\x11\x63over_left_icon_1\x18\x03 \x01(\x05\x12\x19\n\x11\x63over_left_text_1\x18\x04 \x01(\t\x12\x19\n\x11\x63over_left_icon_2\x18\x05 \x01(\x05\x12\x19\n\x11\x63over_left_text_2\x18\x06 \x01(\t\x12\x19\n\x11\x63over_left_text_3\x18\x07 \x01(\t\x12\x32\n\x05\x62\x61\x64ge\x18\x08 \x03(\x0b\x32#.bilibili.app.dynamic.v1.VideoBadge\"$\n\x14\x44ynOurCityModuleDesc\x12\x0c\n\x04\x64\x65sc\x18\x01 \x01(\t\"z\n\x16\x44ynOurCityModuleExtend\x12\x0c\n\x04type\x18\x01 \x01(\t\x12H\n\nextend_lbs\x18\x02 \x01(\x0b\x32\x32.bilibili.app.dynamic.v1.DynOurCityModuleExtendLBSH\x00\x42\x08\n\x06\x65xtend\"W\n\x19\x44ynOurCityModuleExtendLBS\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x10\n\x08poi_type\x18\x04 \x01(\x05\"\xca\x01\n\x0f\x44ynOurCityReply\x12\x0e\n\x06offset\x18\x01 \x01(\t\x12\x10\n\x08has_more\x18\x02 \x01(\x05\x12\r\n\x05style\x18\x03 \x01(\x05\x12\x11\n\ttop_label\x18\x04 \x01(\t\x12\x35\n\x04list\x18\x05 \x03(\x0b\x32\'.bilibili.app.dynamic.v1.DynOurCityItem\x12\x18\n\x10top_button_label\x18\x06 \x01(\t\x12\x0f\n\x07\x63ity_id\x18\x07 \x01(\x05\x12\x11\n\tcity_name\x18\x08 \x01(\t\"\x8b\x03\n\rDynOurCityReq\x12\x0f\n\x07\x63ity_id\x18\x01 \x01(\x03\x12\x0b\n\x03lat\x18\x02 \x01(\x01\x12\x0b\n\x03lng\x18\x03 \x01(\x01\x12\x0e\n\x06offset\x18\x04 \x01(\t\x12\x11\n\tpage_size\x18\x05 \x01(\x05\x12\x16\n\x0eteenagers_mode\x18\x06 \x01(\x05\x12\n\n\x02qn\x18\x07 \x01(\x05\x12\r\n\x05\x66nver\x18\x08 \x01(\x05\x12\r\n\x05\x66nval\x18\t \x01(\x05\x12\x12\n\nforce_host\x18\n \x01(\x05\x12\r\n\x05\x66ourk\x18\x0b \x01(\x05\x12\x11\n\tlbs_state\x18\x0c \x01(\x05\x12\x14\n\x0crefresh_city\x18\r \x01(\r\x12\x32\n\x08\x65xp_conf\x18\x0e \x01(\x0b\x32 .bilibili.app.dynamic.v1.ExpConf\x12\x43\n\x0bplayer_args\x18\x0f \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x11\n\tcity_code\x18\x10 \x01(\x03\x12\x12\n\nbuild_time\x18\x11 \x01(\x03\"%\n\x13\x44ynOurCitySwitchReq\x12\x0e\n\x06switch\x18\x01 \x01(\x05\"\x1b\n\nDynRedItem\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xa8\x01\n\x0b\x44ynRedReply\x12\x10\n\x08red_type\x18\x01 \x01(\t\x12\x39\n\x0c\x64yn_red_item\x18\x02 \x01(\x0b\x32#.bilibili.app.dynamic.v1.DynRedItem\x12\x13\n\x0b\x64\x65\x66\x61ult_tab\x18\x03 \x01(\t\x12\x37\n\tred_style\x18\x04 \x01(\x0b\x32$.bilibili.app.dynamic.v1.DynRedStyle\"C\n\tDynRedReq\x12\x36\n\ntab_offset\x18\x01 \x03(\x0b\x32\".bilibili.app.dynamic.v1.TabOffset\"\xa0\x01\n\x0b\x44ynRedStyle\x12\x0f\n\x07\x62g_type\x18\x01 \x01(\x05\x12\x13\n\x0b\x63orner_type\x18\x02 \x01(\x05\x12\x14\n\x0c\x64isplay_time\x18\x03 \x01(\x05\x12\x13\n\x0b\x63orner_mark\x18\x04 \x01(\t\x12\x32\n\x02up\x18\x05 \x01(\x0b\x32&.bilibili.app.dynamic.v1.DynRedStyleUp\x12\x0c\n\x04type\x18\x06 \x01(\x05\"*\n\rDynRedStyleUp\x12\x0b\n\x03uid\x18\x01 \x01(\x03\x12\x0c\n\x04\x66\x61\x63\x65\x18\x02 \x01(\t\"\xe7\x01\n\x06\x44ynTab\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0e\n\x06\x62ubble\x18\x03 \x01(\t\x12\x11\n\tred_point\x18\x04 \x01(\x05\x12\x0f\n\x07\x63ity_id\x18\x05 \x01(\x03\x12\x10\n\x08is_popup\x18\x06 \x01(\x05\x12-\n\x05popup\x18\x07 \x01(\x0b\x32\x1e.bilibili.app.dynamic.v1.Popup\x12\x12\n\ndefaultTab\x18\x08 \x01(\x08\x12\x11\n\tsub_title\x18\t \x01(\t\x12\x0e\n\x06\x61nchor\x18\n \x01(\t\x12\x15\n\rinternal_test\x18\x0b \x01(\t\"?\n\x0b\x44ynTabReply\x12\x30\n\x07\x64yn_tab\x18\x01 \x03(\x0b\x32\x1f.bilibili.app.dynamic.v1.DynTab\"#\n\tDynTabReq\x12\x16\n\x0eteenagers_mode\x18\x01 \x01(\x05\"8\n\x0f\x44ynUpdOffsetReq\x12\x10\n\x08host_uid\x18\x01 \x01(\x03\x12\x13\n\x0bread_offset\x18\x02 \x01(\t\"\x82\x01\n\x15\x44ynVideoPersonalReply\x12\x32\n\x04list\x18\x01 \x03(\x0b\x32$.bilibili.app.dynamic.v1.DynamicItem\x12\x0e\n\x06offset\x18\x02 \x01(\t\x12\x10\n\x08has_more\x18\x03 \x01(\x05\x12\x13\n\x0bread_offset\x18\x04 \x01(\t\"\xbe\x01\n\x13\x44ynVideoPersonalReq\x12\x16\n\x0eteenagers_mode\x18\x01 \x01(\x05\x12\x10\n\x08host_uid\x18\x02 \x01(\x03\x12\x0e\n\x06offset\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\x05\x12\x12\n\nis_preload\x18\x05 \x01(\x05\x12\n\n\x02qn\x18\x06 \x01(\x05\x12\r\n\x05\x66nver\x18\x07 \x01(\x05\x12\r\n\x05\x66nval\x18\x08 \x01(\x05\x12\x12\n\nforce_host\x18\t \x01(\x05\x12\r\n\x05\x66ourk\x18\n \x01(\x05\"\xbf\x01\n\x0b\x44ynVideoReq\x12\x16\n\x0eteenagers_mode\x18\x01 \x01(\x05\x12\x17\n\x0fupdate_baseline\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\x05\x12\x14\n\x0crefresh_type\x18\x05 \x01(\x05\x12\n\n\x02qn\x18\x06 \x01(\x05\x12\r\n\x05\x66nver\x18\x07 \x01(\x05\x12\r\n\x05\x66nval\x18\x08 \x01(\x05\x12\x12\n\nforce_host\x18\t \x01(\x05\x12\r\n\x05\x66ourk\x18\n \x01(\x05\"\x9d\x01\n\x10\x44ynVideoReqReply\x12\x32\n\x04list\x18\x01 \x03(\x0b\x32$.bilibili.app.dynamic.v1.DynamicItem\x12\x12\n\nupdate_num\x18\x02 \x01(\x05\x12\x16\n\x0ehistory_offset\x18\x03 \x01(\t\x12\x17\n\x0fupdate_baseline\x18\x04 \x01(\t\x12\x10\n\x08has_more\x18\x05 \x01(\x05\"*\n\x03\x45xp\x12\x10\n\x08\x65xp_name\x18\x01 \x01(\t\x12\x11\n\texp_group\x18\x02 \x01(\t\"I\n\x07\x45xpConf\x12\x12\n\nexp_enable\x18\x01 \x01(\x05\x12*\n\x04\x65xps\x18\x02 \x03(\x0b\x32\x1c.bilibili.app.dynamic.v1.Exp\"\x9a\x02\n\x06\x45xtend\x12\x0c\n\x04type\x18\x01 \x01(\t\x12?\n\x0e\x65xt_info_topic\x18\x02 \x01(\x0b\x32%.bilibili.app.dynamic.v1.ExtInfoTopicH\x00\x12;\n\x0c\x65xt_info_lbs\x18\x03 \x01(\x0b\x32#.bilibili.app.dynamic.v1.ExtInfoLBSH\x00\x12;\n\x0c\x65xt_info_hot\x18\x04 \x01(\x0b\x32#.bilibili.app.dynamic.v1.ExtInfoHotH\x00\x12=\n\rext_info_game\x18\x05 \x01(\x0b\x32$.bilibili.app.dynamic.v1.ExtInfoGameH\x00\x42\x08\n\x06\x65xtend\"7\n\x0b\x45xtInfoGame\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\"6\n\nExtInfoHot\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\"H\n\nExtInfoLBS\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x10\n\x08poi_type\x18\x04 \x01(\x05\"8\n\x0c\x45xtInfoTopic\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\"~\n\x0e\x46ollowListItem\x12\x11\n\tseason_id\x18\x01 \x01(\x05\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63over\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12.\n\x06new_ep\x18\x05 \x01(\x0b\x32\x1e.bilibili.app.dynamic.v1.NewEP\"\x98\x01\n\rGeoCoderReply\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x44\n\x11\x61\x64\x64ress_component\x18\x02 \x01(\x0b\x32).bilibili.app.dynamic.v1.AddressComponent\x12\x30\n\x07\x61\x64_info\x18\x03 \x01(\x0b\x32\x1f.bilibili.app.dynamic.v1.AdInfo\"5\n\x0bGeoCoderReq\x12\x0b\n\x03lat\x18\x01 \x01(\x01\x12\x0b\n\x03lng\x18\x02 \x01(\x01\x12\x0c\n\x04\x66rom\x18\x03 \x01(\t\"\x1f\n\x03Gps\x12\x0b\n\x03lat\x18\x01 \x01(\x01\x12\x0b\n\x03lng\x18\x02 \x01(\x01\"O\n\rLikeAnimation\x12\r\n\x05\x62\x65gin\x18\x01 \x01(\t\x12\x0c\n\x04proc\x18\x02 \x01(\t\x12\x0b\n\x03\x65nd\x18\x03 \x01(\t\x12\x14\n\x0clike_icon_id\x18\x04 \x01(\x03\"V\n\x08LikeInfo\x12\x39\n\tanimation\x18\x01 \x01(\x0b\x32&.bilibili.app.dynamic.v1.LikeAnimation\x12\x0f\n\x07is_like\x18\x02 \x01(\x05\"3\n\x08LikeUser\x12\x0b\n\x03uid\x18\x01 \x01(\x03\x12\r\n\x05uname\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\"*\n\x08LiveInfo\x12\x11\n\tis_living\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\"\xec\x02\n\rMixUpListItem\x12\x0b\n\x03uid\x18\x01 \x01(\x03\x12\x19\n\x11special_attention\x18\x02 \x01(\x05\x12\x14\n\x0creddot_state\x18\x03 \x01(\x05\x12=\n\tlive_info\x18\x04 \x01(\x0b\x32*.bilibili.app.dynamic.v1.MixUpListLiveItem\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x0c\n\x04\x66\x61\x63\x65\x18\x06 \x01(\t\x12\x39\n\x08official\x18\x07 \x01(\x0b\x32\'.bilibili.app.dynamic.v1.OfficialVerify\x12-\n\x03vip\x18\x08 \x01(\x0b\x32 .bilibili.app.dynamic.v1.VipInfo\x12\x33\n\x08relation\x18\t \x01(\x0b\x32!.bilibili.app.dynamic.v1.Relation\x12\x16\n\x0epremiere_state\x18\n \x01(\x05\x12\x0b\n\x03uri\x18\x0b \x01(\t\"A\n\x11MixUpListLiveItem\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0f\n\x07room_id\x18\x02 \x01(\x03\x12\x0b\n\x03uri\x18\x03 \x01(\t\"\xf7\x05\n\x06Module\x12\x13\n\x0bmodule_type\x18\x01 \x01(\t\x12:\n\x0bmodule_fold\x18\x02 \x01(\x0b\x32#.bilibili.app.dynamic.v1.ModuleFoldH\x00\x12>\n\rmodule_author\x18\x03 \x01(\x0b\x32%.bilibili.app.dynamic.v1.ModuleAuthorH\x00\x12@\n\x0emodule_dynamic\x18\x04 \x01(\x0b\x32&.bilibili.app.dynamic.v1.ModuleDynamicH\x00\x12<\n\x0cmodule_state\x18\x05 \x01(\x0b\x32$.bilibili.app.dynamic.v1.ModuleStateH\x00\x12@\n\x0emodule_forward\x18\x06 \x01(\x0b\x32&.bilibili.app.dynamic.v1.ModuleForwardH\x00\x12>\n\rmodule_extend\x18\x07 \x01(\x0b\x32%.bilibili.app.dynamic.v1.ModuleExtendH\x00\x12@\n\x0emodule_dispute\x18\x08 \x01(\x0b\x32&.bilibili.app.dynamic.v1.ModuleDisputeH\x00\x12:\n\x0bmodule_desc\x18\t \x01(\x0b\x32#.bilibili.app.dynamic.v1.ModuleDescH\x00\x12\x42\n\x0fmodule_likeUser\x18\n \x01(\x0b\x32\'.bilibili.app.dynamic.v1.ModuleLikeUserH\x00\x12\x41\n\rmodule_upList\x18\x0b \x01(\x0b\x32(.bilibili.app.dynamic.v1.ModuleDynUpListH\x00\x12\x46\n\x11module_followList\x18\x0c \x01(\x0b\x32).bilibili.app.dynamic.v1.ModuleFollowListH\x00\x42\r\n\x0bmodule_item\"\xa5\x01\n\x0cModuleAuthor\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x18\n\x10ptime_label_text\x18\x02 \x01(\t\x12\x31\n\x06\x61uthor\x18\x03 \x01(\x0b\x32!.bilibili.app.dynamic.v1.UserInfo\x12<\n\rdecorate_card\x18\x04 \x01(\x0b\x32%.bilibili.app.dynamic.v1.DecorateCard\"@\n\nModuleDesc\x12\x32\n\x04\x64\x65sc\x18\x01 \x03(\x0b\x32$.bilibili.app.dynamic.v1.Description\"9\n\rModuleDispute\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\"\x9e\x02\n\rModuleDynamic\x12\x11\n\tcard_type\x18\x01 \x01(\t\x12\x34\n\x08\x63\x61rd_ugc\x18\x02 \x01(\x0b\x32 .bilibili.app.dynamic.v1.CardUGCH\x00\x12\x34\n\x08\x63\x61rd_pgc\x18\x03 \x01(\x0b\x32 .bilibili.app.dynamic.v1.CardPGCH\x00\x12\x43\n\x10\x63\x61rd_curr_season\x18\x04 \x01(\x0b\x32\'.bilibili.app.dynamic.v1.CardCurrSeasonH\x00\x12\x41\n\x0f\x63\x61rd_curr_batch\x18\x05 \x01(\x0b\x32&.bilibili.app.dynamic.v1.CardCurrBatchH\x00\x42\x06\n\x04\x63\x61rd\"l\n\x0fModuleDynUpList\x12\x14\n\x0cmodule_title\x18\x01 \x01(\t\x12\x10\n\x08show_all\x18\x02 \x01(\t\x12\x31\n\x04list\x18\x03 \x03(\x0b\x32#.bilibili.app.dynamic.v1.UpListItem\"?\n\x0cModuleExtend\x12/\n\x06\x65xtend\x18\x01 \x03(\x0b\x32\x1f.bilibili.app.dynamic.v1.Extend\"\xaf\x01\n\nModuleFold\x12\x11\n\tfold_type\x18\x01 \x01(\x05\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x10\n\x08\x66old_ids\x18\x03 \x01(\t\x12\x35\n\nfold_users\x18\x04 \x03(\x0b\x32!.bilibili.app.dynamic.v1.UserInfo\x12\x37\n\x0c\x66old_type_v2\x18\x05 \x01(\x0e\x32!.bilibili.app.dynamic.v1.FoldType\"`\n\x10ModuleFollowList\x12\x15\n\rview_all_link\x18\x01 \x01(\t\x12\x35\n\x04list\x18\x02 \x03(\x0b\x32\'.bilibili.app.dynamic.v1.FollowListItem\"T\n\rModuleForward\x12\x11\n\tcard_type\x18\x01 \x01(\t\x12\x30\n\x07modules\x18\x02 \x03(\x0b\x32\x1f.bilibili.app.dynamic.v1.Module\"]\n\x0eModuleLikeUser\x12\x35\n\nlike_users\x18\x01 \x03(\x0b\x32!.bilibili.app.dynamic.v1.LikeUser\x12\x14\n\x0c\x64isplay_text\x18\x02 \x01(\t\"\x98\x01\n\x0bModuleState\x12\x0e\n\x06repost\x18\x01 \x01(\x05\x12\x0c\n\x04like\x18\x02 \x01(\x05\x12\r\n\x05reply\x18\x03 \x01(\x05\x12\x34\n\tlike_info\x18\x04 \x01(\x0b\x32!.bilibili.app.dynamic.v1.LikeInfo\x12\x12\n\nno_comment\x18\x05 \x01(\x08\x12\x12\n\nno_forward\x18\x06 \x01(\x08\"l\n\tNameplate\x12\x0b\n\x03nid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05image\x18\x03 \x01(\t\x12\x13\n\x0bimage_small\x18\x04 \x01(\t\x12\r\n\x05level\x18\x05 \x01(\t\x12\x11\n\tcondition\x18\x06 \x01(\t\"6\n\x05NewEP\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\nindex_show\x18\x02 \x01(\t\x12\r\n\x05\x63over\x18\x03 \x01(\t\"\t\n\x07NoReply\"\x07\n\x05NoReq\">\n\x0eOfficialVerify\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x10\n\x08is_atten\x18\x03 \x01(\x05\"\x19\n\x17OurCityClickReportReply\"V\n\x15OurCityClickReportReq\x12\x12\n\ndynamic_id\x18\x01 \x01(\t\x12\x0f\n\x07\x63ity_id\x18\x02 \x01(\x03\x12\x0b\n\x03lat\x18\x03 \x01(\x01\x12\x0b\n\x03lng\x18\x04 \x01(\x01\";\n\tPGCSeason\x12\x11\n\tis_finish\x18\x01 \x01(\x05\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\x05\"b\n\x13PlayerPreloadParams\x12\n\n\x02qn\x18\x01 \x01(\x05\x12\r\n\x05\x66nver\x18\x02 \x01(\x05\x12\r\n\x05\x66nval\x18\x03 \x01(\x05\x12\x12\n\nforce_host\x18\x04 \x01(\x05\x12\r\n\x05\x66ourk\x18\x05 \x01(\x05\"1\n\x05Popup\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\"z\n\x08Relation\x12\x37\n\x06status\x18\x01 \x01(\x0e\x32\'.bilibili.app.dynamic.v1.RelationStatus\x12\x11\n\tis_follow\x18\x02 \x01(\x05\x12\x13\n\x0bis_followed\x18\x03 \x01(\x05\x12\r\n\x05title\x18\x04 \x01(\t\"q\n\tShareInfo\x12\x0b\n\x03\x61id\x18\x01 \x01(\x03\x12\x0c\n\x04\x62vid\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\x10\n\x08subtitle\x18\x04 \x01(\t\x12\r\n\x05\x63over\x18\x05 \x01(\t\x12\x0b\n\x03mid\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\x07 \x01(\t\"z\n\nSVideoItem\x12\x11\n\tcard_type\x18\x01 \x01(\t\x12\x36\n\x07modules\x18\x02 \x03(\x0b\x32%.bilibili.app.dynamic.v1.SVideoModule\x12\x12\n\ndyn_id_str\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x03\"\xc2\x02\n\x0cSVideoModule\x12\x13\n\x0bmodule_type\x18\x01 \x01(\t\x12\x44\n\rmodule_author\x18\x02 \x01(\x0b\x32+.bilibili.app.dynamic.v1.SVideoModuleAuthorH\x00\x12\x44\n\rmodule_player\x18\x03 \x01(\x0b\x32+.bilibili.app.dynamic.v1.SVideoModulePlayerH\x00\x12@\n\x0bmodule_desc\x18\x04 \x01(\x0b\x32).bilibili.app.dynamic.v1.SVideoModuleDescH\x00\x12@\n\x0bmodule_stat\x18\x05 \x01(\x0b\x32).bilibili.app.dynamic.v1.SVideoModuleStatH\x00\x42\r\n\x0bmodule_item\"r\n\x12SVideoModuleAuthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x66\x61\x63\x65\x18\x03 \x01(\t\x12\x10\n\x08pub_desc\x18\x04 \x01(\t\x12\x14\n\x0cis_attention\x18\x05 \x01(\x05\x12\x0b\n\x03uri\x18\x06 \x01(\t\"-\n\x10SVideoModuleDesc\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\"\xa2\x01\n\x12SVideoModulePlayer\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x0b\n\x03\x61id\x18\x04 \x01(\x03\x12\x0b\n\x03\x63id\x18\x05 \x01(\x03\x12\x10\n\x08\x64uration\x18\x06 \x01(\x03\x12\x35\n\tdimension\x18\x07 \x01(\x0b\x32\".bilibili.app.dynamic.v1.Dimension\"\x86\x01\n\x10SVideoModuleStat\x12:\n\tstat_info\x18\x01 \x03(\x0b\x32\'.bilibili.app.dynamic.v1.SVideoStatInfo\x12\x36\n\nshare_info\x18\x02 \x01(\x0b\x32\".bilibili.app.dynamic.v1.ShareInfo\"\x93\x01\n\x0bSVideoReply\x12\x31\n\x04list\x18\x01 \x03(\x0b\x32#.bilibili.app.dynamic.v1.SVideoItem\x12\x0e\n\x06offset\x18\x02 \x01(\t\x12\x10\n\x08has_more\x18\x03 \x01(\x05\x12/\n\x03top\x18\x04 \x01(\x0b\x32\".bilibili.app.dynamic.v1.SVideoTop\"\xe9\x02\n\tSVideoReq\x12\x0b\n\x03oid\x18\x01 \x01(\x03\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.bilibili.app.dynamic.v1.SVideoType\x12\x0e\n\x06offset\x18\x03 \x01(\t\x12\n\n\x02qn\x18\x04 \x01(\x05\x12\r\n\x05\x66nver\x18\x05 \x01(\x05\x12\r\n\x05\x66nval\x18\x06 \x01(\x05\x12\x12\n\nforce_host\x18\x07 \x01(\x05\x12\r\n\x05\x66ourk\x18\x08 \x01(\x05\x12\r\n\x05spmid\x18\t \x01(\t\x12\x12\n\nfrom_spmid\x18\n \x01(\t\x12\x44\n\x0eplayer_preload\x18\x0b \x01(\x0b\x32,.bilibili.app.dynamic.v1.PlayerPreloadParams\x12\x11\n\tfocus_aid\x18\x0c \x01(\x03\x12\x43\n\x0bplayer_args\x18\r \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"J\n\x0eSVideoStatInfo\x12\x0c\n\x04icon\x18\x01 \x01(\x05\x12\x0b\n\x03num\x18\x02 \x01(\x03\x12\x10\n\x08selected\x18\x03 \x01(\x05\x12\x0b\n\x03uri\x18\x04 \x01(\t\"(\n\tSVideoTop\x12\r\n\x05Title\x18\x01 \x01(\t\x12\x0c\n\x04\x44\x65sc\x18\x02 \x01(\t\"(\n\tTabOffset\x12\x0b\n\x03tab\x18\x01 \x01(\x05\x12\x0e\n\x06offset\x18\x02 \x01(\t\"I\n\nUpListItem\x12\x12\n\nhas_update\x18\x01 \x01(\x05\x12\x0c\n\x04\x66\x61\x63\x65\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0b\n\x03uid\x18\x04 \x01(\x03\"\xc9\x02\n\x08UserInfo\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x66\x61\x63\x65\x18\x03 \x01(\t\x12\x39\n\x08official\x18\x04 \x01(\x0b\x32\'.bilibili.app.dynamic.v1.OfficialVerify\x12-\n\x03vip\x18\x05 \x01(\x0b\x32 .bilibili.app.dynamic.v1.VipInfo\x12/\n\x04live\x18\x06 \x01(\x0b\x32!.bilibili.app.dynamic.v1.LiveInfo\x12\x0b\n\x03uri\x18\x07 \x01(\t\x12\x35\n\x07pendant\x18\x08 \x01(\x0b\x32$.bilibili.app.dynamic.v1.UserPendant\x12\x35\n\tnameplate\x18\t \x01(\x0b\x32\".bilibili.app.dynamic.v1.Nameplate\"G\n\x0bUserPendant\x12\x0b\n\x03pid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05image\x18\x03 \x01(\t\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\x03\"\xb6\x01\n\nVideoBadge\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x12\n\ntext_color\x18\x02 \x01(\t\x12\x18\n\x10text_color_night\x18\x03 \x01(\t\x12\x10\n\x08\x62g_color\x18\x04 \x01(\t\x12\x16\n\x0e\x62g_color_night\x18\x05 \x01(\t\x12\x14\n\x0c\x62order_color\x18\x06 \x01(\t\x12\x1a\n\x12\x62order_color_night\x18\x07 \x01(\t\x12\x10\n\x08\x62g_style\x18\x08 \x01(\x05\"\x7f\n\x07VipInfo\x12\x0c\n\x04Type\x18\x01 \x01(\x05\x12\x0e\n\x06status\x18\x02 \x01(\x05\x12\x10\n\x08\x64ue_date\x18\x03 \x01(\x03\x12\x30\n\x05label\x18\x04 \x01(\x0b\x32!.bilibili.app.dynamic.v1.VipLabel\x12\x12\n\ntheme_type\x18\x05 \x01(\x05\"\x18\n\x08VipLabel\x12\x0c\n\x04path\x18\x01 \x01(\t*/\n\x06\x42gType\x12\x13\n\x0f\x62g_type_default\x10\x00\x12\x10\n\x0c\x62g_type_face\x10\x01*S\n\nCornerType\x12\x14\n\x10\x63orner_type_none\x10\x00\x12\x14\n\x10\x63orner_type_text\x10\x01\x12\x19\n\x15\x63orner_type_animation\x10\x02*m\n\x08\x46oldType\x12\x10\n\x0c\x46oldTypeZero\x10\x00\x12\x13\n\x0f\x46oldTypePublish\x10\x01\x12\x14\n\x10\x46oldTypeFrequent\x10\x02\x12\x11\n\rFoldTypeUnite\x10\x03\x12\x11\n\rFoldTypeLimit\x10\x04*g\n\tMediaType\x12\x11\n\rMediaTypeNone\x10\x00\x12\x10\n\x0cMediaTypeUGC\x10\x01\x12\x10\n\x0cMediaTypePGC\x10\x02\x12\x11\n\rMediaTypeLive\x10\x03\x12\x10\n\x0cMediaTypeVCS\x10\x04*\xc3\x01\n\x0eRelationStatus\x12\x18\n\x14relation_status_none\x10\x00\x12\x1c\n\x18relation_status_nofollow\x10\x01\x12\x1a\n\x16relation_status_follow\x10\x02\x12\x1c\n\x18relation_status_followed\x10\x03\x12\"\n\x1erelation_status_mutual_concern\x10\x04\x12\x1b\n\x17relation_status_special\x10\x05*L\n\tStyleType\x12\x13\n\x0fSTYLE_TYPE_NONE\x10\x00\x12\x13\n\x0fSTYLE_TYPE_LIVE\x10\x01\x12\x15\n\x11STYLE_TYPE_DYN_UP\x10\x02*Y\n\nSVideoType\x12\x0c\n\x08TypeNone\x10\x00\x12\x0f\n\x0bTypeDynamic\x10\x01\x12\x14\n\x10TypePopularIndex\x10\x02\x12\x16\n\x12TypePopularHotword\x10\x03*\xa5\x01\n\x0cVideoSubType\x12\x14\n\x10VideoSubTypeNone\x10\x00\x12\x17\n\x13VideoSubTypeBangumi\x10\x01\x12\x15\n\x11VideoSubTypeMovie\x10\x02\x12\x1b\n\x17VideoSubTypeDocumentary\x10\x03\x12\x18\n\x14VideoSubTypeDomestic\x10\x04\x12\x18\n\x14VideoSubTypeTeleplay\x10\x05\x32\x8a\n\n\x07\x44ynamic\x12[\n\x08\x44ynVideo\x12$.bilibili.app.dynamic.v1.DynVideoReq\x1a).bilibili.app.dynamic.v1.DynVideoReqReply\x12^\n\nDynDetails\x12&.bilibili.app.dynamic.v1.DynDetailsReq\x1a(.bilibili.app.dynamic.v1.DynDetailsReply\x12R\n\x06SVideo\x12\".bilibili.app.dynamic.v1.SVideoReq\x1a$.bilibili.app.dynamic.v1.SVideoReply\x12R\n\x06\x44ynTab\x12\".bilibili.app.dynamic.v1.DynTabReq\x1a$.bilibili.app.dynamic.v1.DynTabReply\x12\x62\n\x10\x44ynOurCitySwitch\x12,.bilibili.app.dynamic.v1.DynOurCitySwitchReq\x1a .bilibili.app.dynamic.v1.NoReply\x12^\n\nDynOurCity\x12&.bilibili.app.dynamic.v1.DynOurCityReq\x1a(.bilibili.app.dynamic.v1.DynOurCityReply\x12p\n\x10\x44ynVideoPersonal\x12,.bilibili.app.dynamic.v1.DynVideoPersonalReq\x1a..bilibili.app.dynamic.v1.DynVideoPersonalReply\x12Z\n\x0c\x44ynUpdOffset\x12(.bilibili.app.dynamic.v1.DynUpdOffsetReq\x1a .bilibili.app.dynamic.v1.NoReply\x12R\n\x06\x44ynRed\x12\".bilibili.app.dynamic.v1.DynRedReq\x1a$.bilibili.app.dynamic.v1.DynRedReply\x12j\n\x14\x44ynMixUpListViewMore\x12\x1e.bilibili.app.dynamic.v1.NoReq\x1a\x32.bilibili.app.dynamic.v1.DynMixUpListViewMoreReply\x12v\n\x12\x44ynMixUpListSearch\x12..bilibili.app.dynamic.v1.DynMixUpListSearchReq\x1a\x30.bilibili.app.dynamic.v1.DynMixUpListSearchReply\x12v\n\x12OurCityClickReport\x12..bilibili.app.dynamic.v1.OurCityClickReportReq\x1a\x30.bilibili.app.dynamic.v1.OurCityClickReportReply\x12X\n\x08GeoCoder\x12$.bilibili.app.dynamic.v1.GeoCoderReq\x1a&.bilibili.app.dynamic.v1.GeoCoderReplyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.dynamic.v1.dynamic_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v1/dynamic_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.dynamic.v1 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v1_dot_dynamic__pb2
+from bilirpc.bilibili.app.dynamic.v1 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v1_dot_dynamic__pb2
 
 
 class DynamicStub(object):
     """v1动态
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2_grpc.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/__pycache__/dynamic_pb2_grpc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/campus.proto` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/campus.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/campus_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/campus_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
-from bilibili.pagination import pagination_pb2 as bilibili_dot_pagination_dot_pagination__pb2
-from bilibili.app.dynamic.common import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_common_dot_dynamic__pb2
-from bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.pagination import pagination_pb2 as bilibili_dot_pagination_dot_pagination__pb2
+from bilirpc.bilibili.app.dynamic.common import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_common_dot_dynamic__pb2
+from bilirpc.bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bilibili/app/dynamic/v2/campus.proto\x12\x17\x62ilibili.app.dynamic.v2\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\x1a$bilibili/pagination/pagination.proto\x1a)bilibili/app/dynamic/common/dynamic.proto\x1a%bilibili/app/dynamic/v2/dynamic.proto\"\xac\x01\n\x13\x43\x61mpusWaterFlowItem\x12\x11\n\titem_type\x18\x01 \x01(\x05\x12:\n\x08wh_ratio\x18\x02 \x01(\x0b\x32(.bilibili.app.dynamic.common.ItemWHRatio\x12>\n\x0citem_default\x18\x03 \x01(\x0b\x32&.bilibili.app.dynamic.v2.WFItemDefaultH\x00\x42\x06\n\x04item\"\xb2\x01\n\x10WaterFlowRcmdReq\x12\x11\n\tcampus_id\x18\x01 \x01(\x03\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x43\n\x0bplayer_args\x18\x03 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x38\n\x04\x66rom\x18\x04 \x01(\x0e\x32*.bilibili.app.dynamic.v2.CampusRcmdReqFrom\"\x8a\x01\n\x11WaterFlowRcmdResp\x12;\n\x05items\x18\x01 \x03(\x0b\x32,.bilibili.app.dynamic.v2.CampusWaterFlowItem\x12\x38\n\x06offset\x18\x02 \x01(\x0b\x32(.bilibili.pagination.FeedPaginationReply\"\xc0\x03\n\rWFItemDefault\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x41\n\rbottom_left_1\x18\x03 \x01(\x0b\x32*.bilibili.app.dynamic.v2.CoverIconWithText\x12\x41\n\rbottom_left_2\x18\x04 \x01(\x0b\x32*.bilibili.app.dynamic.v2.CoverIconWithText\x12\x42\n\x0e\x62ottom_right_1\x18\x05 \x01(\x0b\x32*.bilibili.app.dynamic.v2.CoverIconWithText\x12\x0b\n\x03uri\x18\x06 \x01(\t\x12\x38\n\x0brcmd_reason\x18\x07 \x01(\x0b\x32#.bilibili.app.dynamic.v2.RcmdReason\x12L\n\x0b\x61nnotations\x18\x08 \x03(\x0b\x32\x37.bilibili.app.dynamic.v2.WFItemDefault.AnnotationsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x32p\n\x06\x43\x61mpus\x12\x66\n\rWaterFlowRcmd\x12).bilibili.app.dynamic.v2.WaterFlowRcmdReq\x1a*.bilibili.app.dynamic.v2.WaterFlowRcmdRespb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.dynamic.v2.campus_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/campus_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/campus_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.dynamic.v2 import campus_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_campus__pb2
+from bilirpc.bilibili.app.dynamic.v2 import campus_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_campus__pb2
 
 
 class CampusStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/dynamic.proto` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/dynamic.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/dynamic_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
+from bilirpc.bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
 
 
 class DynamicStub(object):
     """v2动态, rpc 按字母顺序排列
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/opus.proto` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/opus.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/opus_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/opus_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
-from bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"bilibili/app/dynamic/v2/opus.proto\x12\x17\x62ilibili.app.dynamic.v2\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\x1a%bilibili/app/dynamic/v2/dynamic.proto\"\x94\x02\n\rOpusDetailReq\x12\x34\n\topus_type\x18\x01 \x01(\x0e\x32!.bilibili.app.dynamic.v2.OpusType\x12\x0b\n\x03oid\x18\x02 \x01(\x03\x12\x10\n\x08\x64yn_type\x18\x03 \x01(\x03\x12\x10\n\x08share_id\x18\x04 \x01(\t\x12\x12\n\nshare_mode\x18\t \x01(\x05\x12\x12\n\nlocal_time\x18\n \x01(\x05\x12\x43\n\x0bplayer_args\x18\x0b \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12/\n\x06\x63onfig\x18\x0c \x01(\x0b\x32\x1f.bilibili.app.dynamic.v2.Config\"F\n\x0eOpusDetailResp\x12\x34\n\topus_item\x18\x01 \x01(\x0b\x32!.bilibili.app.dynamic.v2.OpusItem\"\xc1\x01\n\x08OpusItem\x12\x0f\n\x07opus_id\x18\x01 \x01(\x03\x12\x34\n\topus_type\x18\x02 \x01(\x0e\x32!.bilibili.app.dynamic.v2.OpusType\x12\x0b\n\x03oid\x18\x03 \x01(\x03\x12\x30\n\x07modules\x18\x04 \x03(\x0b\x32\x1f.bilibili.app.dynamic.v2.Module\x12/\n\x06\x65xtend\x18\x05 \x01(\x0b\x32\x1f.bilibili.app.dynamic.v2.Extend*\\\n\x08OpusType\x12\x11\n\rOPUS_TYPE_DYN\x10\x00\x12\x15\n\x11OPUS_TYPE_ARTICLE\x10\x01\x12\x12\n\x0eOPUS_TYPE_NOTE\x10\x02\x12\x12\n\x0eOPUS_TYPE_WORD\x10\x03\x32\x65\n\x04Opus\x12]\n\nOpusDetail\x12&.bilibili.app.dynamic.v2.OpusDetailReq\x1a\'.bilibili.app.dynamic.v2.OpusDetailRespb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.dynamic.v2.opus_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/dynamic/v2/opus_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/dynamic/v2/opus_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.dynamic.v2 import opus_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_opus__pb2
+from bilirpc.bilibili.app.dynamic.v2 import opus_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_opus__pb2
 
 
 class OpusStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/history.proto` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/history.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/history_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/history_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bilibili/app/interfaces/v1/history.proto\x12\x19\x62ilibili.app.interface.v1\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\"\x98\x01\n\x0b\x43\x61rdArticle\x12\x0e\n\x06\x63overs\x18\x01 \x03(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03mid\x18\x03 \x01(\x03\x12\x18\n\x10\x64isplayAttention\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61\x64ge\x18\x05 \x01(\t\x12\x35\n\x08relation\x18\x06 \x01(\x0b\x32#.bilibili.app.interface.v1.Relation\"`\n\nCardCheese\x12\r\n\x05\x63over\x18\x01 \x01(\t\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x10\n\x08\x64uration\x18\x03 \x01(\x03\x12\x10\n\x08subtitle\x18\x04 \x01(\t\x12\r\n\x05state\x18\x05 \x01(\x03\"\xa3\x01\n\x08\x43\x61rdLive\x12\r\n\x05\x63over\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03mid\x18\x03 \x01(\x03\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\x0e\n\x06ststus\x18\x05 \x01(\x05\x12\x19\n\x11\x64isplay_attention\x18\x06 \x01(\x08\x12\x35\n\x08relation\x18\x07 \x01(\x0b\x32#.bilibili.app.interface.v1.Relation\"l\n\x07\x43\x61rdOGV\x12\r\n\x05\x63over\x18\x01 \x01(\t\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x10\n\x08\x64uration\x18\x03 \x01(\x03\x12\x10\n\x08subtitle\x18\x04 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\x03\"\xbd\x02\n\x07\x43\x61rdUGC\x12\r\n\x05\x63over\x18\x01 \x01(\t\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x10\n\x08\x64uration\x18\x03 \x01(\x03\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0b\n\x03mid\x18\x05 \x01(\x03\x12\x19\n\x11\x64isplay_attention\x18\x06 \x01(\x08\x12\x0b\n\x03\x63id\x18\x07 \x01(\x03\x12\x0c\n\x04page\x18\x08 \x01(\x05\x12\x10\n\x08subtitle\x18\t \x01(\t\x12\x35\n\x08relation\x18\n \x01(\x0b\x32#.bilibili.app.interface.v1.Relation\x12\x0c\n\x04\x62vid\x18\x0b \x01(\t\x12\x0e\n\x06videos\x18\x0c \x01(\x03\x12\x12\n\nshort_link\x18\r \x01(\t\x12\x16\n\x0eshare_subtitle\x18\x0e \x01(\t\x12\x0c\n\x04view\x18\x0f \x01(\x03\x12\r\n\x05state\x18\x10 \x01(\x03\"\x1c\n\x08\x43learReq\x12\x10\n\x08\x62usiness\x18\x01 \x01(\t\"$\n\x06\x43ursor\x12\x0b\n\x03max\x18\x01 \x01(\x03\x12\r\n\x05maxTp\x18\x02 \x01(\x05\"\xeb\x03\n\nCursorItem\x12\x36\n\x08\x63\x61rd_ugc\x18\x01 \x01(\x0b\x32\".bilibili.app.interface.v1.CardUGCH\x00\x12\x36\n\x08\x63\x61rd_ogv\x18\x02 \x01(\x0b\x32\".bilibili.app.interface.v1.CardOGVH\x00\x12>\n\x0c\x63\x61rd_article\x18\x03 \x01(\x0b\x32&.bilibili.app.interface.v1.CardArticleH\x00\x12\x38\n\tcard_live\x18\x04 \x01(\x0b\x32#.bilibili.app.interface.v1.CardLiveH\x00\x12<\n\x0b\x63\x61rd_cheese\x18\x05 \x01(\x0b\x32%.bilibili.app.interface.v1.CardCheeseH\x00\x12\r\n\x05title\x18\x06 \x01(\t\x12\x0b\n\x03uri\x18\x07 \x01(\t\x12\x0e\n\x06viewAt\x18\x08 \x01(\x03\x12\x0b\n\x03kid\x18\t \x01(\x03\x12\x0b\n\x03oid\x18\n \x01(\x03\x12\x10\n\x08\x62usiness\x18\x0b \x01(\t\x12\n\n\x02tp\x18\x0c \x01(\x05\x12\x31\n\x02\x64t\x18\r \x01(\x0b\x32%.bilibili.app.interface.v1.DeviceType\x12\x11\n\thas_share\x18\x0e \x01(\x08\x42\x0b\n\tcard_item\"\xba\x01\n\x0b\x43ursorReply\x12\x34\n\x05items\x18\x01 \x03(\x0b\x32%.bilibili.app.interface.v1.CursorItem\x12\x31\n\x03tab\x18\x02 \x03(\x0b\x32$.bilibili.app.interface.v1.CursorTab\x12\x31\n\x06\x63ursor\x18\x03 \x01(\x0b\x32!.bilibili.app.interface.v1.Cursor\x12\x0f\n\x07hasMore\x18\x04 \x01(\x08\"\xdd\x01\n\tCursorReq\x12\x31\n\x06\x63ursor\x18\x01 \x01(\x0b\x32!.bilibili.app.interface.v1.Cursor\x12\x10\n\x08\x62usiness\x18\x02 \x01(\t\x12\x46\n\x0eplayer_preload\x18\x03 \x01(\x0b\x32..bilibili.app.interface.v1.PlayerPreloadParams\x12\x43\n\x0bplayer_args\x18\x04 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"J\n\tCursorTab\x12\x10\n\x08\x62usiness\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06router\x18\x03 \x01(\t\x12\r\n\x05\x66ocus\x18\x04 \x01(\x08\"\x9d\x01\n\rCursorV2Reply\x12\x34\n\x05items\x18\x01 \x03(\x0b\x32%.bilibili.app.interface.v1.CursorItem\x12\x31\n\x06\x63ursor\x18\x02 \x01(\x0b\x32!.bilibili.app.interface.v1.Cursor\x12\x0f\n\x07hasMore\x18\x03 \x01(\x08\x12\x12\n\nempty_link\x18\x04 \x01(\t\"\xf1\x01\n\x0b\x43ursorV2Req\x12\x31\n\x06\x63ursor\x18\x01 \x01(\x0b\x32!.bilibili.app.interface.v1.Cursor\x12\x10\n\x08\x62usiness\x18\x02 \x01(\t\x12\x46\n\x0eplayer_preload\x18\x03 \x01(\x0b\x32..bilibili.app.interface.v1.PlayerPreloadParams\x12\x43\n\x0bplayer_args\x18\x04 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x10\n\x08is_local\x18\x05 \x01(\x08\"A\n\tDeleteReq\x12\x34\n\x08his_info\x18\x01 \x01(\x0b\x32\".bilibili.app.interface.v1.HisInfo\"G\n\nDeviceType\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1d.bilibili.app.interface.v1.DT\x12\x0c\n\x04icon\x18\x02 \x01(\t\"(\n\x07HisInfo\x12\x10\n\x08\x62usiness\x18\x01 \x01(\t\x12\x0b\n\x03kid\x18\x02 \x01(\x03\"D\n\x0fHistoryTabReply\x12\x31\n\x03tab\x18\x01 \x03(\x0b\x32$.bilibili.app.interface.v1.CursorTab\"l\n\rHistoryTabReq\x12\x10\n\x08\x62usiness\x18\x01 \x01(\t\x12\x38\n\x06source\x18\x02 \x01(\x0e\x32(.bilibili.app.interface.v1.HistorySource\x12\x0f\n\x07keyword\x18\x03 \x01(\t\"v\n\x12LatestHistoryReply\x12\x34\n\x05items\x18\x01 \x01(\x0b\x32%.bilibili.app.interface.v1.CursorItem\x12\r\n\x05scene\x18\x02 \x01(\t\x12\r\n\x05rtime\x18\x03 \x01(\x03\x12\x0c\n\x04\x66lag\x18\x04 \x01(\t\"l\n\x10LatestHistoryReq\x12\x10\n\x08\x62usiness\x18\x01 \x01(\t\x12\x46\n\x0eplayer_preload\x18\x02 \x01(\x0b\x32..bilibili.app.interface.v1.PlayerPreloadParams\"\t\n\x07NoReply\"!\n\x04Page\x12\n\n\x02pn\x18\x01 \x01(\x03\x12\r\n\x05total\x18\x02 \x01(\x03\"a\n\x13PlayerPreloadParams\x12\n\n\x02qn\x18\x01 \x01(\x03\x12\r\n\x05\x66nver\x18\x02 \x01(\x03\x12\r\n\x05\x66nval\x18\x03 \x01(\x03\x12\x11\n\tforceHost\x18\x04 \x01(\x03\x12\r\n\x05\x66ourk\x18\x05 \x01(\x03\"B\n\x08Relation\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x11\n\tis_follow\x18\x02 \x01(\x05\x12\x13\n\x0bis_followed\x18\x03 \x01(\x05\"\x83\x01\n\x0bSearchReply\x12\x34\n\x05items\x18\x01 \x03(\x0b\x32%.bilibili.app.interface.v1.CursorItem\x12\x0f\n\x07hasMore\x18\x02 \x01(\x08\x12-\n\x04page\x18\x03 \x01(\x0b\x32\x1f.bilibili.app.interface.v1.Page\":\n\tSearchReq\x12\x0f\n\x07keyword\x18\x01 \x01(\t\x12\n\n\x02pn\x18\x02 \x01(\x03\x12\x10\n\x08\x62usiness\x18\x03 \x01(\t*S\n\x02\x44T\x12\x0b\n\x07Unknown\x10\x00\x12\t\n\x05Phone\x10\x01\x12\x07\n\x03Pad\x10\x02\x12\x06\n\x02PC\x10\x03\x12\x06\n\x02TV\x10\x04\x12\x07\n\x03\x43\x61r\x10\x05\x12\x07\n\x03Iot\x10\x06\x12\n\n\x06\x41ndPad\x10\x07*6\n\rHistorySource\x12\x11\n\rhistory_VALUE\x10\x00\x12\x12\n\x0eshopping_VALUE\x10\x01\x32\x8e\x05\n\x07History\x12\x62\n\nHistoryTab\x12(.bilibili.app.interface.v1.HistoryTabReq\x1a*.bilibili.app.interface.v1.HistoryTabReply\x12V\n\x06\x43ursor\x12$.bilibili.app.interface.v1.CursorReq\x1a&.bilibili.app.interface.v1.CursorReply\x12\\\n\x08\x43ursorV2\x12&.bilibili.app.interface.v1.CursorV2Req\x1a(.bilibili.app.interface.v1.CursorV2Reply\x12R\n\x06\x44\x65lete\x12$.bilibili.app.interface.v1.DeleteReq\x1a\".bilibili.app.interface.v1.NoReply\x12V\n\x06Search\x12$.bilibili.app.interface.v1.SearchReq\x1a&.bilibili.app.interface.v1.SearchReply\x12P\n\x05\x43lear\x12#.bilibili.app.interface.v1.ClearReq\x1a\".bilibili.app.interface.v1.NoReply\x12k\n\rLatestHistory\x12+.bilibili.app.interface.v1.LatestHistoryReq\x1a-.bilibili.app.interface.v1.LatestHistoryReplyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.interfaces.v1.history_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/history_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/media.proto` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/media.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/media_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/media_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/media_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/media_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.interfaces.v1 import media_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_media__pb2
+from bilirpc.bilibili.app.interfaces.v1 import media_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_media__pb2
 
 
 class MediaStub(object):
     """
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/search.proto` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/search.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/search_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/search_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/search_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.interfaces.v1 import search_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_search__pb2
+from bilirpc.bilibili.app.interfaces.v1 import search_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_search__pb2
 
 
 class SearchStub(object):
     """搜索
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/space.proto` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/space.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/space_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/space_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
-from bilibili.app.archive.v1 import archive_pb2 as bilibili_dot_app_dot_archive_dot_v1_dot_archive__pb2
-from bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.app.archive.v1 import archive_pb2 as bilibili_dot_app_dot_archive_dot_v1_dot_archive__pb2
+from bilirpc.bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&bilibili/app/interfaces/v1/space.proto\x12\x19\x62ilibili.app.interface.v1\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\x1a%bilibili/app/archive/v1/archive.proto\x1a%bilibili/app/dynamic/v2/dynamic.proto\"A\n\x03\x41rc\x12-\n\x07\x61rchive\x18\x01 \x01(\x0b\x32\x1c.bilibili.app.archive.v1.Arc\x12\x0b\n\x03uri\x18\x02 \x01(\t\"@\n\x07\x44ynamic\x12\x35\n\x07\x64ynamic\x18\x01 \x01(\x0b\x32$.bilibili.app.dynamic.v2.DynamicItem\"M\n\x0eSearchTabReply\x12\r\n\x05\x66ocus\x18\x01 \x01(\x03\x12,\n\x04tabs\x18\x02 \x03(\x0b\x32\x1e.bilibili.app.interface.v1.Tab\":\n\x0cSearchTabReq\x12\x0f\n\x07keyword\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\x03\x12\x0c\n\x04\x66rom\x18\x03 \x01(\x05\"U\n\x12SearchArchiveReply\x12\x30\n\x08\x61rchives\x18\x01 \x03(\x0b\x32\x1e.bilibili.app.interface.v1.Arc\x12\r\n\x05total\x18\x02 \x01(\x03\"\x8d\x01\n\x10SearchArchiveReq\x12\x0f\n\x07keyword\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\x03\x12\n\n\x02pn\x18\x03 \x01(\x03\x12\n\n\x02ps\x18\x04 \x01(\x03\x12\x43\n\x0bplayer_args\x18\x05 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"Y\n\x12SearchDynamicReply\x12\x34\n\x08\x64ynamics\x18\x01 \x03(\x0b\x32\".bilibili.app.interface.v1.Dynamic\x12\r\n\x05total\x18\x02 \x01(\x03\"\x8d\x01\n\x10SearchDynamicReq\x12\x0f\n\x07keyword\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\x03\x12\n\n\x02pn\x18\x03 \x01(\x03\x12\n\n\x02ps\x18\x04 \x01(\x03\x12\x43\n\x0bplayer_args\x18\x05 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"!\n\x03Tab\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t*&\n\x04\x46rom\x12\x0e\n\nArchiveTab\x10\x00\x12\x0e\n\nDynamicTab\x10\x01\x32\xc2\x02\n\x05Space\x12_\n\tSearchTab\x12\'.bilibili.app.interface.v1.SearchTabReq\x1a).bilibili.app.interface.v1.SearchTabReply\x12k\n\rSearchArchive\x12+.bilibili.app.interface.v1.SearchArchiveReq\x1a-.bilibili.app.interface.v1.SearchArchiveReply\x12k\n\rSearchDynamic\x12+.bilibili.app.interface.v1.SearchDynamicReq\x1a-.bilibili.app.interface.v1.SearchDynamicReplyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.interfaces.v1.space_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/interfaces/v1/space_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/interfaces/v1/space_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.interfaces.v1 import space_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_space__pb2
+from bilirpc.bilibili.app.interfaces.v1 import space_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_space__pb2
 
 
 class SpaceStub(object):
     """
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/listener/v1/listener.proto` & `bilirpc-1.2/bilirpc/bilibili/app/listener/v1/listener.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/listener/v1/listener_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/listener/v1/listener_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
-from bilibili.app.interfaces.v1 import history_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_history__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.app.interfaces.v1 import history_pb2 as bilibili_dot_app_dot_interfaces_dot_v1_dot_history__pb2
 from bilibili.app.playurl.v1 import playurl_pb2 as bilibili_dot_app_dot_playurl_dot_v1_dot_playurl__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bilibili/app/listener/v1/listener.proto\x12\x18\x62ilibili.app.listener.v1\x1a\x1bgoogle/protobuf/empty.proto\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\x1a(bilibili/app/interfaces/v1/history.proto\x1a%bilibili/app/playurl/v1/playurl.proto\"o\n\x06\x41uthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x03 \x01(\t\x12:\n\x08relation\x18\x04 \x01(\x0b\x32(.bilibili.app.listener.v1.FollowRelation\"\x88\x01\n\x0f\x42KArcDetailsReq\x12\x31\n\x05items\x18\x01 \x03(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x42\n\nplayerArgs\x18\x02 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"F\n\x10\x42KArcDetailsResp\x12\x32\n\x04list\x18\x01 \x03(\x0b\x32$.bilibili.app.listener.v1.DetailItem\"\xe4\x01\n\tBKArchive\x12\x0b\n\x03oid\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63over\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\x12\x10\n\x08\x64uration\x18\x05 \x01(\x03\x12\x0b\n\x03rid\x18\x06 \x01(\x05\x12\r\n\x05rname\x18\x07 \x01(\t\x12\x0f\n\x07publish\x18\x08 \x01(\x03\x12\x15\n\rdisplayed_oid\x18\t \x01(\t\x12\x11\n\tcopyright\x18\n \x01(\x05\x12\x35\n\x06rights\x18\x0b \x01(\x0b\x32%.bilibili.app.listener.v1.BKArcRights\"W\n\tBKArcPart\x12\x0b\n\x03oid\x18\x01 \x01(\x03\x12\x0e\n\x06sub_id\x18\x02 \x01(\x03\x12\r\n\x05title\x18\x03 \x01(\t\x12\x10\n\x08\x64uration\x18\x04 \x01(\x03\x12\x0c\n\x04page\x18\x05 \x01(\x05\"!\n\x0b\x42KArcRights\x12\x12\n\nno_reprint\x18\x01 \x01(\x05\"\x98\x01\n\x06\x42KStat\x12\x0c\n\x04like\x18\x01 \x01(\x05\x12\x0c\n\x04\x63oin\x18\x02 \x01(\x05\x12\x11\n\tfavourite\x18\x03 \x01(\x05\x12\r\n\x05reply\x18\x04 \x01(\x05\x12\r\n\x05share\x18\x05 \x01(\x05\x12\x0c\n\x04view\x18\x06 \x01(\x05\x12\x10\n\x08has_like\x18\x07 \x01(\x08\x12\x10\n\x08has_coin\x18\x08 \x01(\x08\x12\x0f\n\x07has_fav\x18\t \x01(\x08\"\xee\x01\n\nCardModule\x12\x13\n\x0bmodule_type\x18\x01 \x01(\x05\x12=\n\rmodule_header\x18\x02 \x01(\x0b\x32$.bilibili.app.listener.v1.PkcmHeaderH\x00\x12?\n\x0emodule_archive\x18\x03 \x01(\x0b\x32%.bilibili.app.listener.v1.PkcmArchiveH\x00\x12\x41\n\x0bmodule_cbtn\x18\x04 \x01(\x0b\x32*.bilibili.app.listener.v1.PkcmCenterButtonH\x00\x42\x08\n\x06module\"\'\n\x08\x43lickReq\x12\x0b\n\x03sid\x18\x01 \x01(\x03\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\"\x0b\n\tClickResp\"]\n\nCoinAddReq\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12\x10\n\x08thumb_up\x18\x03 \x01(\x08\"\x1e\n\x0b\x43oinAddResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"\xdf\x01\n\x08\x44\x61shItem\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08\x62\x61se_url\x18\x02 \x01(\t\x12\x12\n\nbackup_url\x18\x03 \x03(\t\x12\x11\n\tbandwidth\x18\x04 \x01(\x05\x12\x11\n\tmime_type\x18\x05 \x01(\t\x12\x0e\n\x06\x63odecs\x18\x06 \x01(\t\x12?\n\x0csegment_base\x18\x0c \x01(\x0b\x32).bilibili.app.listener.v1.DashSegmentBase\x12\x0f\n\x07\x63odecid\x18\r \x01(\x05\x12\x0b\n\x03md5\x18\x0e \x01(\t\x12\x0c\n\x04size\x18\x0f \x01(\x03\">\n\x0f\x44\x61shSegmentBase\x12\x16\n\x0einitialization\x18\x01 \x01(\t\x12\x13\n\x0bindex_range\x18\x02 \x01(\t\"\xd3\x05\n\nDetailItem\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x30\n\x03\x61rc\x18\x02 \x01(\x0b\x32#.bilibili.app.listener.v1.BKArchive\x12\x32\n\x05parts\x18\x03 \x03(\x0b\x32#.bilibili.app.listener.v1.BKArcPart\x12/\n\x05owner\x18\x04 \x01(\x0b\x32 .bilibili.app.listener.v1.Author\x12.\n\x04stat\x18\x05 \x01(\x0b\x32 .bilibili.app.listener.v1.BKStat\x12\x11\n\tlast_part\x18\x06 \x01(\x03\x12\x10\n\x08progress\x18\x07 \x01(\x03\x12\x10\n\x08playable\x18\x08 \x01(\x05\x12\x0f\n\x07message\x18\t \x01(\t\x12I\n\x0bplayer_info\x18\n \x03(\x0b\x32\x34.bilibili.app.listener.v1.DetailItem.PlayerInfoEntry\x12;\n\x0f\x61ssociated_item\x18\x0b \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x16\n\x0elast_play_time\x18\x0c \x01(\x03\x12\x13\n\x0bhistory_tag\x18\r \x01(\t\x12:\n\x0b\x64\x65vice_type\x18\x0e \x01(\x0b\x32%.bilibili.app.interface.v1.DeviceType\x12<\n\x0fugc_season_info\x18\x0f \x01(\x0b\x32#.bilibili.app.listener.v1.FavFolder\x1aU\n\x0fPlayerInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayInfo:\x02\x38\x01\"P\n\x08\x45ventReq\x12\x12\n\nevent_type\x18\x01 \x01(\x05\x12\x30\n\x04item\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\"\x0b\n\tEventResp\"~\n\rEventTracking\x12\x10\n\x08operator\x18\x01 \x01(\t\x12\r\n\x05\x62\x61tch\x18\x02 \x01(\t\x12\x10\n\x08track_id\x18\x03 \x01(\t\x12\x13\n\x0b\x65ntity_type\x18\x04 \x01(\t\x12\x11\n\tentity_id\x18\x05 \x01(\t\x12\x12\n\ntrack_json\x18\x06 \x01(\t\"\xf4\x02\n\tFavFolder\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\x12\x38\n\x05owner\x18\x03 \x01(\x0b\x32).bilibili.app.listener.v1.FavFolderAuthor\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\r\n\x05\x63over\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x06 \x01(\t\x12\r\n\x05\x63ount\x18\x07 \x01(\x05\x12\x0c\n\x04\x61ttr\x18\x08 \x01(\x05\x12\r\n\x05state\x18\t \x01(\x05\x12\x0f\n\x07\x66\x61vored\x18\n \x01(\x05\x12\r\n\x05\x63time\x18\x0b \x01(\x03\x12\r\n\x05mtime\x18\x0c \x01(\x03\x12\x14\n\x0cstat_fav_cnt\x18\r \x01(\x05\x12\x16\n\x0estat_share_cnt\x18\x0e \x01(\x05\x12\x15\n\rstat_like_cnt\x18\x0f \x01(\x05\x12\x15\n\rstat_Play_cnt\x18\x10 \x01(\x05\x12\x16\n\x0estat_reply_cnt\x18\x11 \x01(\x05\x12\x11\n\tfav_state\x18\x12 \x01(\x05\"C\n\x0f\x46\x61vFolderAction\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\x05\",\n\x0f\x46\x61vFolderAuthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\"U\n\x12\x46\x61vFolderCreateReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x0e\n\x06public\x18\x03 \x01(\x05\x12\x13\n\x0b\x66older_type\x18\x04 \x01(\x05\"H\n\x13\x46\x61vFolderCreateResp\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\x12\x0f\n\x07message\x18\x03 \x01(\t\"6\n\x12\x46\x61vFolderDeleteReq\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\"&\n\x13\x46\x61vFolderDeleteResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"\xaa\x01\n\x12\x46\x61vFolderDetailReq\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\x12\x0f\n\x07\x66\x61v_mid\x18\x03 \x01(\x03\x12\x34\n\tlast_item\x18\x04 \x01(\x0b\x32!.bilibili.app.listener.v1.FavItem\x12\x11\n\tpage_size\x18\x05 \x01(\x05\x12\x18\n\x10need_folder_info\x18\x06 \x01(\x08\"\xa8\x01\n\x13\x46\x61vFolderDetailResp\x12\r\n\x05total\x18\x01 \x01(\x05\x12\x11\n\treach_end\x18\x02 \x01(\x08\x12\x35\n\x04list\x18\x03 \x03(\x0b\x32\'.bilibili.app.listener.v1.FavItemDetail\x12\x38\n\x0b\x66older_info\x18\x04 \x01(\x0b\x32#.bilibili.app.listener.v1.FavFolder\"Z\n\x10\x46\x61vFolderListReq\x12\x14\n\x0c\x66older_types\x18\x01 \x03(\x05\x12\x30\n\x04item\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\"F\n\x11\x46\x61vFolderListResp\x12\x31\n\x04list\x18\x01 \x03(\x0b\x32#.bilibili.app.listener.v1.FavFolder\"1\n\rFavFolderMeta\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\"\x96\x01\n\x07\x46\x61vItem\x12\x11\n\titem_type\x18\x01 \x01(\x05\x12\x0b\n\x03oid\x18\x02 \x01(\x03\x12\x0b\n\x03\x66id\x18\x03 \x01(\x03\x12\x0b\n\x03mid\x18\x04 \x01(\x03\x12\r\n\x05mtime\x18\x05 \x01(\x03\x12\r\n\x05\x63time\x18\x06 \x01(\x03\x12\x33\n\x02\x65t\x18\x07 \x01(\x0b\x32\'.bilibili.app.listener.v1.EventTracking\"\x9f\x01\n\rFavItemAddReq\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\x12\x32\n\x04play\x18\x03 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItemH\x00\x12\x30\n\x03\x66\x61v\x18\x04 \x01(\x0b\x32!.bilibili.app.listener.v1.FavItemH\x00\x42\x06\n\x04item\"!\n\x0e\x46\x61vItemAddResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"*\n\rFavItemAuthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xbb\x01\n\x0f\x46\x61vItemBatchReq\x12:\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32).bilibili.app.listener.v1.FavFolderAction\x12\x32\n\x04play\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItemH\x00\x12\x30\n\x03\x66\x61v\x18\x03 \x01(\x0b\x32!.bilibili.app.listener.v1.FavItemH\x00\x42\x06\n\x04item\"#\n\x10\x46\x61vItemBatchResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"\x9f\x01\n\rFavItemDelReq\x12\x0b\n\x03\x66id\x18\x01 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x02 \x01(\x05\x12\x32\n\x04play\x18\x03 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItemH\x00\x12\x30\n\x03\x66\x61v\x18\x04 \x01(\x0b\x32!.bilibili.app.listener.v1.FavItemH\x00\x42\x06\n\x04item\"!\n\x0e\x46\x61vItemDelResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"\x8b\x02\n\rFavItemDetail\x12/\n\x04item\x18\x01 \x01(\x0b\x32!.bilibili.app.listener.v1.FavItem\x12\x36\n\x05owner\x18\x02 \x01(\x0b\x32\'.bilibili.app.listener.v1.FavItemAuthor\x12\x33\n\x04stat\x18\x03 \x01(\x0b\x32%.bilibili.app.listener.v1.FavItemStat\x12\r\n\x05\x63over\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x10\n\x08\x64uration\x18\x06 \x01(\x03\x12\r\n\x05state\x18\x07 \x01(\x05\x12\x0f\n\x07message\x18\x08 \x01(\t\x12\r\n\x05parts\x18\t \x01(\x05\"*\n\x0b\x46\x61vItemStat\x12\x0c\n\x04view\x18\x01 \x01(\x05\x12\r\n\x05reply\x18\x02 \x01(\x05\"`\n\x16\x46\x61voredInAnyFoldersReq\x12\x14\n\x0c\x66older_types\x18\x01 \x03(\x05\x12\x30\n\x04item\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\"\x85\x01\n\x17\x46\x61voredInAnyFoldersResp\x12\x38\n\x07\x66olders\x18\x01 \x03(\x0b\x32\'.bilibili.app.listener.v1.FavFolderMeta\x12\x30\n\x04item\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\"\x1c\n\rFavTabShowReq\x12\x0b\n\x03mid\x18\x01 \x01(\x03\"#\n\x0e\x46\x61vTabShowResp\x12\x11\n\tshow_menu\x18\x01 \x01(\x08\" \n\x0e\x46ollowRelation\x12\x0e\n\x06status\x18\x01 \x01(\x05\"t\n\x11\x46ormatDescription\x12\x0f\n\x07quality\x18\x01 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0c\x64isplay_desc\x18\x04 \x01(\t\x12\x13\n\x0bsuperscript\x18\x05 \x01(\t\";\n\x17MainFavMusicMenuListReq\x12\x10\n\x08tab_type\x18\x01 \x01(\x05\x12\x0e\n\x06offset\x18\x02 \x01(\t\"\x86\x01\n\x18MainFavMusicMenuListResp\x12\x10\n\x08tab_type\x18\x01 \x01(\x05\x12\x36\n\tmenu_list\x18\x02 \x03(\x0b\x32#.bilibili.app.listener.v1.MusicMenu\x12\x10\n\x08has_more\x18\x03 \x01(\x08\x12\x0e\n\x06offset\x18\x04 \x01(\t\"\x1b\n\x19MainFavMusicSubTabListReq\"\xe7\x02\n\x1aMainFavMusicSubTabListResp\x12\x33\n\x04tabs\x18\x01 \x03(\x0b\x32%.bilibili.app.listener.v1.MusicSubTab\x12K\n\x0f\x64\x65\x66\x61ult_tab_res\x18\x02 \x01(\x0b\x32\x32.bilibili.app.listener.v1.MainFavMusicMenuListResp\x12^\n\x0e\x66irst_page_res\x18\x03 \x03(\x0b\x32\x46.bilibili.app.listener.v1.MainFavMusicSubTabListResp.FirstPageResEntry\x1ag\n\x11\x46irstPageResEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\x41\n\x05value\x18\x02 \x01(\x0b\x32\x32.bilibili.app.listener.v1.MainFavMusicMenuListResp:\x02\x38\x01\"\xe8\x01\n\rMedialistItem\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\r\n\x05title\x18\x02 \x01(\t\x12\r\n\x05\x63over\x18\x03 \x01(\t\x12\x10\n\x08\x64uration\x18\x04 \x01(\x03\x12\r\n\x05parts\x18\x05 \x01(\x05\x12\x0e\n\x06up_mid\x18\x06 \x01(\x03\x12\x0f\n\x07up_name\x18\x07 \x01(\t\x12\r\n\x05state\x18\x08 \x01(\x05\x12\x0f\n\x07message\x18\t \x01(\t\x12\x11\n\tstat_view\x18\n \x01(\x03\x12\x12\n\nstat_reply\x18\x0b \x01(\x03\"A\n\x0cMedialistReq\x12\x11\n\tlist_type\x18\x01 \x01(\x03\x12\x0e\n\x06\x62iz_id\x18\x02 \x01(\x03\x12\x0e\n\x06offset\x18\x03 \x01(\t\"\xb4\x01\n\rMedialistResp\x12\r\n\x05total\x18\x01 \x01(\x03\x12\x10\n\x08has_more\x18\x02 \x01(\x08\x12\x0e\n\x06offset\x18\x03 \x01(\t\x12\x36\n\x05items\x18\x04 \x03(\x0b\x32\'.bilibili.app.listener.v1.MedialistItem\x12:\n\x07up_info\x18\x05 \x01(\x0b\x32).bilibili.app.listener.v1.MedialistUpInfo\"J\n\x0fMedialistUpInfo\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0e\n\x06\x61vatar\x18\x02 \x01(\t\x12\x0c\n\x04\x66\x61ns\x18\x03 \x01(\x03\x12\x0c\n\x04name\x18\x04 \x01(\t\"\x1b\n\rMenuDeleteReq\x12\n\n\x02id\x18\x01 \x01(\x03\"!\n\x0eMenuDeleteResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"I\n\x0bMenuEditReq\x12\n\n\x02id\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x11\n\tis_public\x18\x04 \x01(\x05\"\x1f\n\x0cMenuEditResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"5\n\x10MenuSubscribeReq\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\x05\x12\x11\n\ttarget_id\x18\x02 \x01(\x03\"$\n\x11MenuSubscribeResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"\x8f\x02\n\tMusicMenu\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x11\n\tmenu_type\x18\x02 \x01(\x05\x12\r\n\x05title\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\x12\r\n\x05\x63over\x18\x05 \x01(\t\x12\x38\n\x05owner\x18\x06 \x01(\x0b\x32).bilibili.app.listener.v1.MusicMenuAuthor\x12\r\n\x05state\x18\x07 \x01(\x05\x12\x0c\n\x04\x61ttr\x18\x08 \x01(\x03\x12\x35\n\x04stat\x18\t \x01(\x0b\x32\'.bilibili.app.listener.v1.MusicMenuStat\x12\r\n\x05total\x18\n \x01(\x03\x12\r\n\x05\x63time\x18\x0b \x01(\x03\x12\x0b\n\x03uri\x18\x0c \x01(\t\"<\n\x0fMusicMenuAuthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x03 \x01(\t\",\n\rMusicMenuStat\x12\x0c\n\x04play\x18\x01 \x01(\x03\x12\r\n\x05reply\x18\x02 \x01(\x03\"<\n\x0bMusicSubTab\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08tab_type\x18\x02 \x01(\x05\x12\r\n\x05total\x18\x03 \x01(\x03\"i\n\nPageOption\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x11\n\tdirection\x18\x02 \x01(\x05\x12\x35\n\tlast_item\x18\x03 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\"\x81\x02\n\x0bPickArchive\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\r\n\x05title\x18\x02 \x01(\t\x12:\n\x05owner\x18\x03 \x01(\x0b\x32+.bilibili.app.listener.v1.PickArchiveAuthor\x12\r\n\x05\x63over\x18\x04 \x01(\t\x12\x10\n\x08\x64uration\x18\x05 \x01(\x03\x12\r\n\x05parts\x18\x06 \x01(\x05\x12\x11\n\tstat_view\x18\x07 \x01(\x05\x12\x12\n\nstat_reply\x18\x08 \x01(\x05\x12\r\n\x05state\x18\t \x01(\x05\x12\x0f\n\x07message\x18\n \x01(\t\".\n\x11PickArchiveAuthor\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\"v\n\x08PickCard\x12\x0f\n\x07pick_id\x18\x01 \x01(\x03\x12\x0f\n\x07\x63\x61rd_id\x18\x02 \x01(\x03\x12\x11\n\tcard_name\x18\x03 \x01(\t\x12\x35\n\x07modules\x18\x04 \x03(\x0b\x32$.bilibili.app.listener.v1.CardModule\"5\n\x11PickCardDetailReq\x12\x0f\n\x07\x63\x61rd_id\x18\x01 \x01(\x03\x12\x0f\n\x07pick_id\x18\x02 \x01(\x03\"m\n\x12PickCardDetailResp\x12\x0f\n\x07\x63\x61rd_id\x18\x01 \x01(\x03\x12\x0f\n\x07pick_id\x18\x02 \x01(\x03\x12\x35\n\x07modules\x18\x03 \x03(\x0b\x32$.bilibili.app.listener.v1.CardModule\"\x1d\n\x0bPickFeedReq\x12\x0e\n\x06offset\x18\x01 \x01(\x03\"Q\n\x0cPickFeedResp\x12\x0e\n\x06offset\x18\x01 \x01(\x03\x12\x31\n\x05\x63\x61rds\x18\x02 \x03(\x0b\x32\".bilibili.app.listener.v1.PickCard\"V\n\x0bPkcmArchive\x12\x32\n\x03\x61rc\x18\x01 \x01(\x0b\x32%.bilibili.app.listener.v1.PickArchive\x12\x13\n\x0bpick_reason\x18\x02 \x01(\t\"T\n\x10PkcmCenterButton\x12\x11\n\ticon_head\x18\x01 \x01(\t\x12\x11\n\ticon_tail\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\"^\n\nPkcmHeader\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x10\n\x08\x62tn_icon\x18\x03 \x01(\t\x12\x10\n\x08\x62tn_text\x18\x04 \x01(\t\x12\x0f\n\x07\x62tn_uri\x18\x05 \x01(\t\"[\n\x13PlayActionReportReq\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x12\n\nfrom_spmid\x18\x02 \x01(\t\"h\n\x08PlayDASH\x12\x10\n\x08\x64uration\x18\x01 \x01(\x05\x12\x17\n\x0fmin_buffer_time\x18\x02 \x01(\x02\x12\x31\n\x05\x61udio\x18\x03 \x03(\x0b\x32\".bilibili.app.listener.v1.DashItem\"}\n\x11PlayHistoryAddReq\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x10\n\x08\x64uration\x18\x03 \x01(\x03\x12\x12\n\nplay_style\x18\x04 \x01(\x05\"X\n\x11PlayHistoryDelReq\x12\x31\n\x05items\x18\x01 \x03(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x10\n\x08truncate\x18\x02 \x01(\x08\"b\n\x0ePlayHistoryReq\x12\x36\n\x08page_opt\x18\x01 \x01(\x0b\x32$.bilibili.app.listener.v1.PageOption\x12\x18\n\x10local_today_zero\x18\x02 \x01(\x03\"g\n\x0fPlayHistoryResp\x12\r\n\x05total\x18\x01 \x01(\x05\x12\x11\n\treach_end\x18\x02 \x01(\x08\x12\x32\n\x04list\x18\x03 \x03(\x0b\x32$.bilibili.app.listener.v1.DetailItem\"\xee\x02\n\x08PlayInfo\x12\n\n\x02qn\x18\x01 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\x12\x0f\n\x07qn_type\x18\x03 \x01(\x05\x12\x35\n\x08play_url\x18\x04 \x01(\x0b\x32!.bilibili.app.listener.v1.PlayURLH\x00\x12\x37\n\tplay_dash\x18\x05 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayDASHH\x00\x12\r\n\x05\x66nver\x18\x06 \x01(\x05\x12\r\n\x05\x66nval\x18\x07 \x01(\x05\x12\x0f\n\x07\x66ormats\x18\x08 \x03(\x05\x12\x15\n\rvideo_codecid\x18\t \x01(\x05\x12\x0e\n\x06length\x18\n \x01(\x03\x12\x0c\n\x04\x63ode\x18\x0b \x01(\x05\x12\x0f\n\x07message\x18\x0c \x01(\t\x12\x13\n\x0b\x65xpire_time\x18\r \x01(\x03\x12\x33\n\x06volume\x18\x0e \x01(\x0b\x32#.bilibili.app.playurl.v1.VolumeInfoB\x06\n\x04info\"o\n\x08PlayItem\x12\x11\n\titem_type\x18\x01 \x01(\x05\x12\x0b\n\x03oid\x18\x03 \x01(\x03\x12\x0e\n\x06sub_id\x18\x04 \x03(\x03\x12\x33\n\x02\x65t\x18\x05 \x01(\x0b\x32\'.bilibili.app.listener.v1.EventTracking\"\x9f\x01\n\x0ePlaylistAddReq\x12\x31\n\x05items\x18\x01 \x03(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x33\n\x05\x61\x66ter\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItemH\x00\x12\x0e\n\x04head\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04tail\x18\x04 \x01(\x08H\x00\x42\x05\n\x03pos\"U\n\x0ePlaylistDelReq\x12\x31\n\x05items\x18\x01 \x03(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x10\n\x08truncate\x18\x02 \x01(\x08\"\xa2\x02\n\x0bPlaylistReq\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x32\n\x06\x61nchor\x18\x03 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x36\n\x08page_opt\x18\x04 \x01(\x0b\x32$.bilibili.app.listener.v1.PageOption\x12\x43\n\x0bplayer_args\x18\x05 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x10\n\x08\x65xtra_id\x18\x06 \x01(\x03\x12\x36\n\x08sort_opt\x18\x07 \x01(\x0b\x32$.bilibili.app.listener.v1.SortOption\"\xc7\x01\n\x0cPlaylistResp\x12\r\n\x05total\x18\x01 \x01(\x05\x12\x13\n\x0breach_start\x18\x02 \x01(\x08\x12\x11\n\treach_end\x18\x03 \x01(\x08\x12\x32\n\x04list\x18\x04 \x03(\x0b\x32$.bilibili.app.listener.v1.DetailItem\x12\x35\n\tlast_play\x18\x05 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x15\n\rlast_progress\x18\x06 \x01(\x03\">\n\x07PlayURL\x12\x33\n\x04\x64url\x18\x01 \x03(\x0b\x32%.bilibili.app.listener.v1.ResponseUrl\"\x83\x01\n\nPlayURLReq\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x43\n\x0bplayer_args\x18\x02 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"\x84\x02\n\x0bPlayURLResp\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x10\n\x08playable\x18\x02 \x01(\x05\x12\x0f\n\x07message\x18\x03 \x01(\t\x12I\n\nplayerInfo\x18\x04 \x03(\x0b\x32\x35.bilibili.app.listener.v1.PlayURLResp.PlayerInfoEntry\x1aU\n\x0fPlayerInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayInfo:\x02\x38\x01\"\x9e\x01\n\x0fRcmdPlaylistReq\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x14\n\x0cneed_history\x18\x03 \x01(\x08\x12\x16\n\x0eneed_top_cards\x18\x04 \x01(\x08\x12\x43\n\x0bplayer_args\x18\x05 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\"\x91\x01\n\x10RcmdPlaylistResp\x12\x32\n\x04list\x18\x01 \x03(\x0b\x32$.bilibili.app.listener.v1.DetailItem\x12\x13\n\x0bhistory_len\x18\x02 \x01(\x03\x12\x34\n\ttop_cards\x18\x03 \x03(\x0b\x32!.bilibili.app.listener.v1.TopCard\"\x86\x01\n\x0bResponseUrl\x12\r\n\x05order\x18\x01 \x01(\x05\x12\x0e\n\x06length\x18\x02 \x01(\x03\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\r\n\x05\x61head\x18\x04 \x01(\t\x12\r\n\x05vhead\x18\x05 \x01(\t\x12\x0b\n\x03url\x18\x06 \x01(\t\x12\x12\n\nbackup_url\x18\x07 \x03(\t\x12\x0b\n\x03md5\x18\x08 \x01(\t\"/\n\nSortOption\x12\r\n\x05order\x18\x01 \x01(\x05\x12\x12\n\nsort_field\x18\x02 \x01(\x05\"N\n\nThumbUpReq\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\"\x1e\n\x0bThumbUpResp\x12\x0f\n\x07message\x18\x01 \x01(\t\"\xe4\x02\n\x07TopCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x12\n\nplay_style\x18\x02 \x01(\x05\x12\x11\n\tcard_type\x18\x03 \x01(\x05\x12?\n\x0elisten_history\x18\x04 \x01(\x0b\x32%.bilibili.app.listener.v1.TpcdHistoryH\x00\x12=\n\nfav_folder\x18\x05 \x01(\x0b\x32\'.bilibili.app.listener.v1.TpcdFavFolderH\x00\x12;\n\tup_recall\x18\x06 \x01(\x0b\x32&.bilibili.app.listener.v1.TpcdUpRecallH\x00\x12=\n\npick_today\x18\x07 \x01(\x0b\x32\'.bilibili.app.listener.v1.TpcdPickTodayH\x00\x12\x0b\n\x03pos\x18\x08 \x01(\x03\x12\x12\n\ntitle_icon\x18\t \x01(\tB\x06\n\x04\x63\x61rd\"\x80\x01\n\rTpcdFavFolder\x12\x32\n\x04item\x18\x01 \x01(\x0b\x32$.bilibili.app.listener.v1.DetailItem\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0b\n\x03pic\x18\x03 \x01(\t\x12\x0b\n\x03\x66id\x18\x04 \x01(\x03\x12\x13\n\x0b\x66older_type\x18\x05 \x01(\x05\"\\\n\x0bTpcdHistory\x12\x32\n\x04item\x18\x01 \x01(\x0b\x32$.bilibili.app.listener.v1.DetailItem\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0b\n\x03pic\x18\x03 \x01(\t\"\x85\x01\n\rTpcdPickToday\x12\x32\n\x04item\x18\x01 \x01(\x0b\x32$.bilibili.app.listener.v1.DetailItem\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0b\n\x03pic\x18\x03 \x01(\t\x12\x0f\n\x07pick_id\x18\x04 \x01(\x03\x12\x14\n\x0cpick_card_id\x18\x05 \x01(\x03\"\xa2\x01\n\x0cTpcdUpRecall\x12\x0e\n\x06up_mid\x18\x01 \x01(\x03\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0e\n\x06\x61vatar\x18\x03 \x01(\t\x12\x16\n\x0emedialist_type\x18\x04 \x01(\x03\x12\x18\n\x10medialist_biz_id\x18\x05 \x01(\x03\x12\x32\n\x04item\x18\x06 \x01(\x0b\x32$.bilibili.app.listener.v1.DetailItem\"A\n\rTripleLikeReq\x12\x30\n\x04item\x18\x01 \x01(\x0b\x32\".bilibili.app.listener.v1.PlayItem\"T\n\x0eTripleLikeResp\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x10\n\x08thumb_ok\x18\x02 \x01(\x08\x12\x0f\n\x07\x63oin_ok\x18\x03 \x01(\x08\x12\x0e\n\x06\x66\x61v_ok\x18\x04 \x01(\x08*\\\n\x0e\x43\x61rdModuleType\x12\x12\n\x0eModule_invalid\x10\x00\x12\x11\n\rModule_header\x10\x01\x12\x12\n\x0eModule_archive\x10\x02\x12\x0f\n\x0bModule_cbtn\x10\x03*P\n\tListOrder\x12\x0c\n\x08NO_ORDER\x10\x00\x12\x10\n\x0cORDER_NORMAL\x10\x01\x12\x11\n\rORDER_REVERSE\x10\x02\x12\x10\n\x0cORDER_RANDOM\x10\x03*O\n\rListSortField\x12\x0b\n\x07NO_SORT\x10\x00\x12\x0e\n\nSORT_CTIME\x10\x01\x12\x10\n\x0cSORT_VIEWCNT\x10\x02\x12\x0f\n\x0bSORT_FAVCNT\x10\x03*\xa6\x01\n\x0ePlaylistSource\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\r\n\tMEM_SPACE\x10\x01\x12\x14\n\x10\x41UDIO_COLLECTION\x10\x02\x12\x0e\n\nAUDIO_CARD\x10\x03\x12\x12\n\x0eUSER_FAVOURITE\x10\x04\x12\x0e\n\nUP_ARCHIVE\x10\x05\x12\x0f\n\x0b\x41UDIO_CACHE\x10\x06\x12\r\n\tPICK_CARD\x10\x07\x12\x0e\n\nMEDIA_LIST\x10\x08*f\n\x0bTopCardType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x12\n\x0eLISTEN_HISTORY\x10\x01\x12\x13\n\x0f\x46\x41VORITE_FOLDER\x10\x02\x12\r\n\tUP_RECALL\x10\x03\x12\x0e\n\nPICK_TODAY\x10\x04\x32\xba\x13\n\x08Listener\x12\x36\n\x04Ping\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\x12V\n\x07PlayUrl\x12$.bilibili.app.listener.v1.PlayURLReq\x1a%.bilibili.app.listener.v1.PlayURLResp\x12\x65\n\x0c\x42karcDetails\x12).bilibili.app.listener.v1.BKArcDetailsReq\x1a*.bilibili.app.listener.v1.BKArcDetailsResp\x12Y\n\x08Playlist\x12%.bilibili.app.listener.v1.PlaylistReq\x1a&.bilibili.app.listener.v1.PlaylistResp\x12O\n\x0bPlaylistAdd\x12(.bilibili.app.listener.v1.PlaylistAddReq\x1a\x16.google.protobuf.Empty\x12O\n\x0bPlaylistDel\x12(.bilibili.app.listener.v1.PlaylistDelReq\x1a\x16.google.protobuf.Empty\x12\x65\n\x0cRcmdPlaylist\x12).bilibili.app.listener.v1.RcmdPlaylistReq\x1a*.bilibili.app.listener.v1.RcmdPlaylistResp\x12\x62\n\x0bPlayHistory\x12(.bilibili.app.listener.v1.PlayHistoryReq\x1a).bilibili.app.listener.v1.PlayHistoryResp\x12U\n\x0ePlayHistoryAdd\x12+.bilibili.app.listener.v1.PlayHistoryAddReq\x1a\x16.google.protobuf.Empty\x12U\n\x0ePlayHistoryDel\x12+.bilibili.app.listener.v1.PlayHistoryDelReq\x1a\x16.google.protobuf.Empty\x12Y\n\x10PlayActionReport\x12-.bilibili.app.listener.v1.PlayActionReportReq\x1a\x16.google.protobuf.Empty\x12_\n\nTripleLike\x12\'.bilibili.app.listener.v1.TripleLikeReq\x1a(.bilibili.app.listener.v1.TripleLikeResp\x12V\n\x07ThumbUp\x12$.bilibili.app.listener.v1.ThumbUpReq\x1a%.bilibili.app.listener.v1.ThumbUpResp\x12V\n\x07\x43oinAdd\x12$.bilibili.app.listener.v1.CoinAddReq\x1a%.bilibili.app.listener.v1.CoinAddResp\x12_\n\nFavItemAdd\x12\'.bilibili.app.listener.v1.FavItemAddReq\x1a(.bilibili.app.listener.v1.FavItemAddResp\x12_\n\nFavItemDel\x12\'.bilibili.app.listener.v1.FavItemDelReq\x1a(.bilibili.app.listener.v1.FavItemDelResp\x12\x65\n\x0c\x46\x61vItemBatch\x12).bilibili.app.listener.v1.FavItemBatchReq\x1a*.bilibili.app.listener.v1.FavItemBatchResp\x12z\n\x13\x46\x61voredInAnyFolders\x12\x30.bilibili.app.listener.v1.FavoredInAnyFoldersReq\x1a\x31.bilibili.app.listener.v1.FavoredInAnyFoldersResp\x12h\n\rFavFolderList\x12*.bilibili.app.listener.v1.FavFolderListReq\x1a+.bilibili.app.listener.v1.FavFolderListResp\x12n\n\x0f\x46\x61vFolderDetail\x12,.bilibili.app.listener.v1.FavFolderDetailReq\x1a-.bilibili.app.listener.v1.FavFolderDetailResp\x12n\n\x0f\x46\x61vFolderCreate\x12,.bilibili.app.listener.v1.FavFolderCreateReq\x1a-.bilibili.app.listener.v1.FavFolderCreateResp\x12n\n\x0f\x46\x61vFolderDelete\x12,.bilibili.app.listener.v1.FavFolderDeleteReq\x1a-.bilibili.app.listener.v1.FavFolderDeleteResp\x12Y\n\x08PickFeed\x12%.bilibili.app.listener.v1.PickFeedReq\x1a&.bilibili.app.listener.v1.PickFeedResp\x12k\n\x0ePickCardDetail\x12+.bilibili.app.listener.v1.PickCardDetailReq\x1a,.bilibili.app.listener.v1.PickCardDetailResp\x12\\\n\tMedialist\x12&.bilibili.app.listener.v1.MedialistReq\x1a\'.bilibili.app.listener.v1.MedialistResp\x12P\n\x05\x45vent\x12\".bilibili.app.listener.v1.EventReq\x1a#.bilibili.app.listener.v1.EventResp2\xe5\x05\n\x05Music\x12_\n\nFavTabShow\x12\'.bilibili.app.listener.v1.FavTabShowReq\x1a(.bilibili.app.listener.v1.FavTabShowResp\x12\x83\x01\n\x16MainFavMusicSubTabList\x12\x33.bilibili.app.listener.v1.MainFavMusicSubTabListReq\x1a\x34.bilibili.app.listener.v1.MainFavMusicSubTabListResp\x12}\n\x14MainFavMusicMenuList\x12\x31.bilibili.app.listener.v1.MainFavMusicMenuListReq\x1a\x32.bilibili.app.listener.v1.MainFavMusicMenuListResp\x12Y\n\x08MenuEdit\x12%.bilibili.app.listener.v1.MenuEditReq\x1a&.bilibili.app.listener.v1.MenuEditResp\x12_\n\nMenuDelete\x12\'.bilibili.app.listener.v1.MenuDeleteReq\x1a(.bilibili.app.listener.v1.MenuDeleteResp\x12h\n\rMenuSubscribe\x12*.bilibili.app.listener.v1.MenuSubscribeReq\x1a+.bilibili.app.listener.v1.MenuSubscribeResp\x12P\n\x05\x43lick\x12\".bilibili.app.listener.v1.ClickReq\x1a#.bilibili.app.listener.v1.ClickRespb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/listener/v1/listener_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/listener/v1/listener_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/nativeact/v1/nativeact.proto` & `bilirpc-1.2/bilirpc/bilibili/app/nativeact/v1/nativeact.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/nativeact/v1/nativeact_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/nativeact/v1/nativeact_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
-from bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
-from bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
+from bilirpc.bilibili.app.dynamic.v2 import dynamic_pb2 as bilibili_dot_app_dot_dynamic_dot_v2_dot_dynamic__pb2
+from bilirpc.bilibili.app.archive.middleware.v1 import preload_pb2 as bilibili_dot_app_dot_archive_dot_middleware_dot_v1_dot_preload__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)bilibili/app/nativeact/v1/nativeact.proto\x12\x19\x62ilibili.app.nativeact.v1\x1a\x19google/protobuf/any.proto\x1a%bilibili/app/dynamic/v2/dynamic.proto\x1a\x30\x62ilibili/app/archive/middleware/v1/preload.proto\"I\n\x04\x41rea\x12\x0e\n\x06height\x18\x01 \x01(\x03\x12\r\n\x05width\x18\x02 \x01(\x03\x12\t\n\x01x\x18\x03 \x01(\x03\x12\t\n\x01y\x18\x04 \x01(\x03\x12\x0c\n\x04ukey\x18\x05 \x01(\t\"?\n\x05\x42\x61\x64ge\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08\x62g_color\x18\x02 \x01(\t\x12\x16\n\x0e\x62g_color_night\x18\x03 \x01(\t\"d\n\x0f\x43\x61rouselImgCard\x12\x15\n\rcontent_style\x18\x01 \x01(\x03\x12:\n\x06images\x18\x02 \x03(\x0b\x32*.bilibili.app.nativeact.v1.CarouselImgItem\"\x90\x01\n\x0f\x43\x61rouselImgItem\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0e\n\x06length\x18\x03 \x01(\x03\x12\r\n\x05width\x18\x04 \x01(\x03\x12\x32\n\x07top_tab\x18\x05 \x01(\x0b\x32!.bilibili.app.nativeact.v1.TopTab\x12\x0e\n\x06height\x18\x06 \x01(\x03\"z\n\x10\x43\x61rouselWordCard\x12\x15\n\rcontent_style\x18\x01 \x01(\x03\x12\x13\n\x0bscroll_type\x18\x02 \x01(\x03\x12:\n\x05words\x18\x03 \x03(\x0b\x32+.bilibili.app.nativeact.v1.CarouselWordItem\"#\n\x10\x43\x61rouselWordItem\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\"\x91\x06\n\x05\x43olor\x12\x10\n\x08\x62g_color\x18\x01 \x01(\t\x12\x13\n\x0btitle_color\x18\x02 \x01(\t\x12\x16\n\x0etop_font_color\x18\x03 \x01(\t\x12\x19\n\x11\x62ottom_font_color\x18\x04 \x01(\t\x12\x12\n\nfont_color\x18\x05 \x01(\t\x12\x1d\n\x15text_title_font_color\x18\x06 \x01(\t\x12\x17\n\x0findicator_color\x18\x07 \x01(\t\x12\x15\n\rcard_bg_color\x18\x08 \x01(\t\x12\x1d\n\x15\x63\x61rd_title_font_color\x18\t \x01(\t\x12\x1b\n\x13\x63\x61rd_title_bg_color\x18\n \x01(\t\x12\x1c\n\x14view_more_font_color\x18\x0b \x01(\t\x12\x1a\n\x12view_more_bg_color\x18\x0c \x01(\t\x12\x16\n\x0etimeline_color\x18\r \x01(\t\x12\x17\n\x0frcmd_font_color\x18\x0e \x01(\t\x12\x1b\n\x13subtitle_font_color\x18\x0f \x01(\t\x12\x1b\n\x13selected_font_color\x18\x10 \x01(\t\x12\x19\n\x11selected_bg_color\x18\x11 \x01(\t\x12\x1d\n\x15unselected_font_color\x18\x12 \x01(\t\x12\x1b\n\x13unselected_bg_color\x18\x13 \x01(\t\x12\x1e\n\x16nt_selected_font_color\x18\x14 \x01(\t\x12\x1c\n\x14nt_selected_bg_color\x18\x15 \x01(\t\x12 \n\x18nt_unselected_font_color\x18\x16 \x01(\t\x12\x1e\n\x16nt_unselected_bg_color\x18\x17 \x01(\t\x12\x1a\n\x12progress_bar_color\x18\x18 \x01(\t\x12\x16\n\x0epanel_bg_color\x18\x19 \x01(\t\x12\x1a\n\x12panel_select_color\x18\x1a \x01(\t\x12\x1f\n\x17panel_select_font_color\x18\x1b \x01(\t\x12\"\n\x1apanel_nt_select_font_color\x18\x1c \x01(\t\"m\n\x12\x44ynamicActMoreCard\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12<\n\x0csubpage_data\x18\x03 \x01(\x0b\x32&.bilibili.app.nativeact.v1.SubpageData\"D\n\x0b\x44ynamicCard\x12\x35\n\x07\x64ynamic\x18\x01 \x01(\x0b\x32$.bilibili.app.dynamic.v2.DynamicItem\"j\n\x0f\x44ynamicMoreCard\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12<\n\x0csubpage_data\x18\x03 \x01(\x0b\x32&.bilibili.app.nativeact.v1.SubpageData\"\x84\x01\n\rDynamicParams\x12)\n\x0b\x66\x65\x65\x64_offset\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0e\n\x06offset\x18\x02 \x01(\x03\x12\x12\n\nlast_group\x18\x03 \x01(\x03\x12\x11\n\tmodule_id\x18\x04 \x01(\x03\x12\x11\n\tsort_type\x18\x05 \x01(\x03\"\xf7\x01\n\nDynamicReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x38\n\x06params\x18\x02 \x01(\x0b\x32(.bilibili.app.nativeact.v1.DynamicParams\x12\x12\n\nfrom_spmid\x18\x03 \x01(\t\x12\x43\n\x0bplayer_args\x18\x04 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x12\n\nlocal_time\x18\x05 \x01(\x05\x12\x15\n\ris_cold_start\x18\x06 \x01(\x08\x12\x17\n\x0fprimary_page_id\x18\x07 \x01(\x03\"@\n\x0b\x44ynamicResp\x12\x31\n\x06module\x18\x01 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\"1\n\x0c\x45\x64itorParams\x12\x0e\n\x06offset\x18\x01 \x01(\x03\x12\x11\n\tmodule_id\x18\x02 \x01(\x03\"\xfa\x03\n\x13\x45\x64itorRecommendCard\x12\x10\n\x08top_icon\x18\x01 \x01(\t\x12\x13\n\x0btop_content\x18\x02 \x01(\t\x12\x13\n\x0b\x62ottom_icon\x18\x03 \x01(\t\x12\x16\n\x0e\x62ottom_content\x18\x04 \x01(\t\x12\x17\n\x0f\x63over_image_uri\x18\x05 \x01(\t\x12\r\n\x05title\x18\x06 \x01(\t\x12\x0b\n\x03uri\x18\x07 \x01(\t\x12\x11\n\tposition1\x18\x08 \x01(\t\x12\x11\n\tposition2\x18\t \x01(\t\x12\x11\n\tposition3\x18\n \x01(\t\x12\x11\n\tposition4\x18\x0b \x01(\t\x12\x11\n\tposition5\x18\x0c \x01(\t\x12/\n\x05share\x18\r \x01(\x0b\x32 .bilibili.app.nativeact.v1.Share\x12/\n\x05\x62\x61\x64ge\x18\x0e \x01(\x0b\x32 .bilibili.app.nativeact.v1.Badge\x12\x38\n\nreport_dic\x18\x0f \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReportDic\x12\x33\n\x07setting\x18\x10 \x01(\x0b\x32\".bilibili.app.nativeact.v1.Setting\x12\x13\n\x0bmiddle_icon\x18\x11 \x01(\t\x12\x15\n\rresource_type\x18\x12 \x01(\t\"q\n\tEditorReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x37\n\x06params\x18\x02 \x01(\x0b\x32\'.bilibili.app.nativeact.v1.EditorParams\x12\x17\n\x0fprimary_page_id\x18\x03 \x01(\x03\"?\n\nEditorResp\x12\x31\n\x06module\x18\x01 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\"[\n\x0f\x46ollowOgvParams\x12\x35\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32%.bilibili.app.nativeact.v1.ActionType\x12\x11\n\tseason_id\x18\x02 \x01(\x05\"^\n\x0c\x46ollowOgvReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12:\n\x06params\x18\x02 \x01(\x0b\x32*.bilibili.app.nativeact.v1.FollowOgvParams\"%\n\x0c\x46ollowOgvRly\x12\x15\n\rfollow_params\x18\x01 \x01(\t\"X\n\x08GameCard\x12\r\n\x05image\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x10\n\x08subtitle\x18\x04 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x05 \x01(\t\"\xd7\x01\n\nHeaderCard\x12\x12\n\nuser_image\x18\x01 \x01(\t\x12\x11\n\tuser_name\x18\x02 \x01(\t\x12\x17\n\x0fsponsor_content\x18\x03 \x01(\t\x12\x18\n\x10high_light_image\x18\x04 \x01(\t\x12\x17\n\x0flow_light_image\x18\x05 \x01(\t\x12\x0b\n\x03uri\x18\x06 \x01(\t\x12\x10\n\x08view_num\x18\x07 \x01(\t\x12\x13\n\x0b\x64iscuss_num\x18\x08 \x01(\t\x12\x15\n\ris_subscribed\x18\t \x01(\x08\x12\x0b\n\x03mid\x18\n \x01(\x03\">\n\x08IconCard\x12\x32\n\x05items\x18\x01 \x03(\x0b\x32#.bilibili.app.nativeact.v1.IconItem\"5\n\x08IconItem\x12\r\n\x05title\x18\x01 \x01(\t\x12\r\n\x05image\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\"\x1f\n\x0eImageTitleCard\x12\r\n\x05image\x18\x01 \x01(\t\"\xde\x02\n\x08IndexReq\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\x15\n\ractivity_from\x18\x02 \x01(\t\x12\x12\n\ndynamic_id\x18\x03 \x01(\x03\x12\x14\n\x0cshare_origin\x18\x04 \x01(\t\x12\x0e\n\x06tab_id\x18\x05 \x01(\x03\x12\x15\n\rtab_module_id\x18\x06 \x01(\x03\x12\x15\n\rhttps_url_req\x18\x07 \x01(\x05\x12\x12\n\nfrom_spmid\x18\x08 \x01(\t\x12\x13\n\x0b\x63urrent_tab\x18\t \x01(\t\x12\x43\n\x0bplayer_args\x18\n \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x12\n\nlocal_time\x18\x0b \x01(\x05\x12\x15\n\ris_cold_start\x18\x0c \x01(\x08\x12\x17\n\x0fprimary_page_id\x18\r \x01(\x03\x12\x10\n\x08tab_from\x18\x0e \x01(\t\"\xbc\x01\n\x0eInlineIndexReq\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\x15\n\rhttps_url_req\x18\x02 \x01(\x05\x12\x12\n\nfrom_spmid\x18\x03 \x01(\t\x12\x43\n\x0bplayer_args\x18\x04 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x12\n\nlocal_time\x18\x05 \x01(\x05\x12\x15\n\ris_cold_start\x18\x06 \x01(\x08\"T\n\x0cLayerDynamic\x12\r\n\x05title\x18\x01 \x01(\t\x12\x35\n\x07\x64ynamic\x18\x02 \x01(\x0b\x32$.bilibili.app.dynamic.v2.DynamicItem\"R\n\x08LiveCard\x12\x10\n\x08has_live\x18\x01 \x01(\x05\x12\x34\n\x07\x63ontent\x18\x02 \x01(\x0b\x32#.bilibili.app.nativeact.v1.LiveItem\"\xf9\x02\n\x08LiveItem\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x0b\n\x03uid\x18\x02 \x01(\x03\x12\x13\n\x0blive_status\x18\x03 \x01(\x03\x12\x11\n\troom_type\x18\x04 \x01(\x03\x12\x11\n\tplay_type\x18\x05 \x01(\x03\x12\r\n\x05title\x18\x06 \x01(\t\x12\r\n\x05\x63over\x18\x07 \x01(\t\x12\x0e\n\x06online\x18\x08 \x01(\x03\x12\x0f\n\x07\x61rea_id\x18\t \x01(\x03\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x16\n\x0eparent_area_id\x18\x0b \x01(\x03\x12\x18\n\x10parent_area_name\x18\x0c \x01(\t\x12\x18\n\x10live_screen_type\x18\r \x01(\x03\x12\x15\n\rlast_end_time\x18\x0e \x01(\x03\x12\x0c\n\x04link\x18\x0f \x01(\t\x12\x0f\n\x07live_id\x18\x10 \x01(\x03\x12@\n\x0cwatched_show\x18\x11 \x01(\x0b\x32*.bilibili.app.nativeact.v1.LiveWatchedShow\"{\n\x0fLiveWatchedShow\x12\x0e\n\x06switch\x18\x01 \x01(\x08\x12\x0b\n\x03num\x18\x02 \x01(\x03\x12\x12\n\ntext_small\x18\x03 \x01(\t\x12\x12\n\ntext_large\x18\x04 \x01(\t\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\x15\n\ricon_location\x18\x06 \x01(\t\"\xba\x01\n\nMessageBox\x12\x11\n\talert_msg\x18\x01 \x01(\t\x12\x1b\n\x13\x63onfirm_button_text\x18\x02 \x01(\t\x12\x1a\n\x12\x63\x61ncel_button_text\x18\x03 \x01(\t\x12\x13\n\x0b\x63onfirm_msg\x18\x04 \x01(\t\x12\x12\n\ncancel_msg\x18\x05 \x01(\t\x12\x37\n\x04type\x18\x06 \x01(\x0e\x32).bilibili.app.nativeact.v1.MessageBoxType\"\xb1\x02\n\x06Module\x12\x13\n\x0bmodule_type\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\x03\x12\x36\n\x0cmodule_color\x18\x03 \x01(\x0b\x32 .bilibili.app.nativeact.v1.Color\x12:\n\x0emodule_setting\x18\x04 \x01(\x0b\x32\".bilibili.app.nativeact.v1.Setting\x12;\n\x0cmodule_items\x18\x05 \x03(\x0b\x32%.bilibili.app.nativeact.v1.ModuleItem\x12\x16\n\x0esubpage_params\x18\x06 \x01(\t\x12\x13\n\x0bmodule_ukey\x18\x07 \x01(\t\x12\x10\n\x08has_more\x18\x08 \x01(\x08\x12\x0f\n\x07is_feed\x18\t \x01(\x08\"\x9c \n\nModuleItem\x12G\n\tcard_type\x18\x01 \x01(\x0e\x32\x34.bilibili.app.nativeact.v1.ModuleItem.CardDetailCase\x12\x0f\n\x07\x63\x61rd_id\x18\x02 \x01(\t\x12O\n\x15\x65\x64itor_recommend_card\x18\n \x01(\x0b\x32..bilibili.app.nativeact.v1.EditorRecommendCardH\x00\x12J\n\x12participation_card\x18\x0b \x01(\x0b\x32,.bilibili.app.nativeact.v1.ParticipationCardH\x00\x12<\n\x0bheader_card\x18\x0c \x01(\x0b\x32%.bilibili.app.nativeact.v1.HeaderCardH\x00\x12>\n\x0c\x64ynamic_card\x18\r \x01(\x0b\x32&.bilibili.app.nativeact.v1.DynamicCardH\x00\x12\x38\n\ttext_card\x18\x0e \x01(\x0b\x32#.bilibili.app.nativeact.v1.TextCardH\x00\x12\x43\n\x0ftext_title_card\x18\x0f \x01(\x0b\x32(.bilibili.app.nativeact.v1.TextTitleCardH\x00\x12\x45\n\x10image_title_card\x18\x10 \x01(\x0b\x32).bilibili.app.nativeact.v1.ImageTitleCardH\x00\x12G\n\x11\x64ynamic_more_card\x18\x11 \x01(\x0b\x32*.bilibili.app.nativeact.v1.DynamicMoreCardH\x00\x12N\n\x15\x64ynamic_act_more_card\x18\x12 \x01(\x0b\x32-.bilibili.app.nativeact.v1.DynamicActMoreCardH\x00\x12\x38\n\tlive_card\x18\x13 \x01(\x0b\x32#.bilibili.app.nativeact.v1.LiveCardH\x00\x12G\n\x11\x63\x61rousel_img_card\x18\x14 \x01(\x0b\x32*.bilibili.app.nativeact.v1.CarouselImgCardH\x00\x12I\n\x12\x63\x61rousel_word_card\x18\x15 \x01(\x0b\x32+.bilibili.app.nativeact.v1.CarouselWordCardH\x00\x12@\n\rresource_card\x18\x16 \x01(\x0b\x32\'.bilibili.app.nativeact.v1.ResourceCardH\x00\x12I\n\x12resource_more_card\x18\x17 \x01(\x0b\x32+.bilibili.app.nativeact.v1.ResourceMoreCardH\x00\x12\x38\n\tgame_card\x18\x18 \x01(\x0b\x32#.bilibili.app.nativeact.v1.GameCardH\x00\x12:\n\nvideo_card\x18\x19 \x01(\x0b\x32$.bilibili.app.nativeact.v1.VideoCardH\x00\x12\x43\n\x0fvideo_more_card\x18\x1a \x01(\x0b\x32(.bilibili.app.nativeact.v1.VideoMoreCardH\x00\x12=\n\x0erecommend_card\x18\x1b \x01(\x0b\x32#.bilibili.app.nativeact.v1.RcmdCardH\x00\x12N\n\x17recommend_vertical_card\x18\x1c \x01(\x0b\x32+.bilibili.app.nativeact.v1.RcmdVerticalCardH\x00\x12\x46\n\x10relativeact_card\x18\x1d \x01(\x0b\x32*.bilibili.app.nativeact.v1.RelativeactCardH\x00\x12U\n\x18relativeact_capsule_card\x18\x1e \x01(\x0b\x32\x31.bilibili.app.nativeact.v1.RelativeactCapsuleCardH\x00\x12\x42\n\x0estatement_card\x18\x1f \x01(\x0b\x32(.bilibili.app.nativeact.v1.StatementCardH\x00\x12\x38\n\ticon_card\x18  \x01(\x0b\x32#.bilibili.app.nativeact.v1.IconCardH\x00\x12\x38\n\tvote_card\x18! \x01(\x0b\x32#.bilibili.app.nativeact.v1.VoteCardH\x00\x12>\n\x0creserve_card\x18\" \x01(\x0b\x32&.bilibili.app.nativeact.v1.ReserveCardH\x00\x12I\n\x12timeline_head_card\x18# \x01(\x0b\x32+.bilibili.app.nativeact.v1.TimelineHeadCardH\x00\x12T\n\x18timeline_event_text_card\x18$ \x01(\x0b\x32\x30.bilibili.app.nativeact.v1.TimelineEventTextCardH\x00\x12V\n\x19timeline_event_image_card\x18% \x01(\x0b\x32\x31.bilibili.app.nativeact.v1.TimelineEventImageCardH\x00\x12^\n\x1dtimeline_event_imagetext_card\x18& \x01(\x0b\x32\x35.bilibili.app.nativeact.v1.TimelineEventImagetextCardH\x00\x12\\\n\x1ctimeline_event_resource_card\x18\' \x01(\x0b\x32\x34.bilibili.app.nativeact.v1.TimelineEventResourceCardH\x00\x12I\n\x12timeline_more_card\x18( \x01(\x0b\x32+.bilibili.app.nativeact.v1.TimelineMoreCardH\x00\x12M\n\x14timeline_unfold_card\x18) \x01(\x0b\x32-.bilibili.app.nativeact.v1.TimelineUnfoldCardH\x00\x12=\n\x0cogv_one_card\x18* \x01(\x0b\x32%.bilibili.app.nativeact.v1.OgvOneCardH\x00\x12\x41\n\x0eogv_three_card\x18+ \x01(\x0b\x32\'.bilibili.app.nativeact.v1.OgvThreeCardH\x00\x12?\n\rogv_more_card\x18, \x01(\x0b\x32&.bilibili.app.nativeact.v1.OgvMoreCardH\x00\x12\x44\n\x0fnavigation_card\x18- \x01(\x0b\x32).bilibili.app.nativeact.v1.NavigationCardH\x00\x12:\n\nreply_card\x18. \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReplyCardH\x00\x12\x36\n\x08tab_card\x18/ \x01(\x0b\x32\".bilibili.app.nativeact.v1.TabCardH\x00\x12@\n\rnewact_header\x18\x30 \x01(\x0b\x32\'.bilibili.app.nativeact.v1.NewactHeaderH\x00\x12>\n\x0cnewact_award\x18\x31 \x01(\x0b\x32&.bilibili.app.nativeact.v1.NewactAwardH\x00\x12\x46\n\x10newact_statement\x18\x32 \x01(\x0b\x32*.bilibili.app.nativeact.v1.NewactStatementH\x00\x12@\n\rprogress_card\x18\x33 \x01(\x0b\x32\'.bilibili.app.nativeact.v1.ProgressCardH\x00\x12<\n\x0bselect_card\x18\x34 \x01(\x0b\x32%.bilibili.app.nativeact.v1.SelectCardH\x00\"\xd6\x07\n\x0e\x43\x61rdDetailCase\x12\x16\n\x12\x43\x41RDDETAIL_NOT_SET\x10\x00\x12\x19\n\x15\x45\x44ITOR_RECOMMEND_CARD\x10\n\x12\x16\n\x12PARTICIPATION_CARD\x10\x0b\x12\x0f\n\x0bHEADER_CARD\x10\x0c\x12\x10\n\x0c\x44YNAMIC_CARD\x10\r\x12\r\n\tTEXT_CARD\x10\x0e\x12\x13\n\x0fTEXT_TITLE_CARD\x10\x0f\x12\x14\n\x10IMAGE_TITLE_CARD\x10\x10\x12\x15\n\x11\x44YNAMIC_MORE_CARD\x10\x11\x12\x19\n\x15\x44YNAMIC_ACT_MORE_CARD\x10\x12\x12\r\n\tLIVE_CARD\x10\x13\x12\x15\n\x11\x43\x41ROUSEL_IMG_CARD\x10\x14\x12\x16\n\x12\x43\x41ROUSEL_WORD_CARD\x10\x15\x12\x11\n\rRESOURCE_CARD\x10\x16\x12\x16\n\x12RESOURCE_MORE_CARD\x10\x17\x12\r\n\tGAME_CARD\x10\x18\x12\x0e\n\nVIDEO_CARD\x10\x19\x12\x13\n\x0fVIDEO_MORE_CARD\x10\x1a\x12\x12\n\x0eRECOMMEND_CARD\x10\x1b\x12\x1b\n\x17RECOMMEND_VERTICAL_CARD\x10\x1c\x12\x14\n\x10RELATIVEACT_CARD\x10\x1d\x12\x1c\n\x18RELATIVEACT_CAPSULE_CARD\x10\x1e\x12\x12\n\x0eSTATEMENT_CARD\x10\x1f\x12\r\n\tICON_CARD\x10 \x12\r\n\tVOTE_CARD\x10!\x12\x10\n\x0cRESERVE_CARD\x10\"\x12\x16\n\x12TIMELINE_HEAD_CARD\x10#\x12\x1c\n\x18TIMELINE_EVENT_TEXT_CARD\x10$\x12\x1d\n\x19TIMELINE_EVENT_IMAGE_CARD\x10%\x12!\n\x1dTIMELINE_EVENT_IMAGETEXT_CARD\x10&\x12 \n\x1cTIMELINE_EVENT_RESOURCE_CARD\x10\'\x12\x16\n\x12TIMELINE_MORE_CARD\x10(\x12\x18\n\x14TIMELINE_UNFOLD_CARD\x10)\x12\x10\n\x0cOGV_ONE_CARD\x10*\x12\x12\n\x0eOGV_THREE_CARD\x10+\x12\x11\n\rOGV_MORE_CARD\x10,\x12\x13\n\x0fNAVIGATION_CARD\x10-\x12\x0e\n\nREPLY_CARD\x10.\x12\x0c\n\x08TAB_CARD\x10/\x12\x16\n\x12NEWACT_HEADER_CARD\x10\x30\x12\x15\n\x11NEWACT_AWARD_CARD\x10\x31\x12\x19\n\x15NEWACT_STATEMENT_CARD\x10\x32\x12\x11\n\rPROGRESS_CARD\x10\x33\x12\x0f\n\x0bSELECT_CARD\x10\x34\x42\r\n\x0b\x63\x61rd_detail\"J\n\x0eNavigationCard\x12\x38\n\x05items\x18\x01 \x03(\x0b\x32).bilibili.app.nativeact.v1.NavigationItem\"2\n\x0eNavigationItem\x12\x11\n\tmodule_id\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\"W\n\x0bNewactAward\x12\r\n\x05title\x18\x01 \x01(\t\x12\x39\n\x05items\x18\x02 \x03(\x0b\x32*.bilibili.app.nativeact.v1.NewactAwardItem\"1\n\x0fNewactAwardItem\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"3\n\rNewactFeature\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x62order_color\x18\x02 \x01(\t\"\xd2\x01\n\x0cNewactHeader\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\t\x12\r\n\x05image\x18\x03 \x01(\t\x12\x15\n\rsponsor_title\x18\x04 \x01(\t\x12\x0b\n\x03mid\x18\x05 \x01(\x03\x12\x11\n\tuser_name\x18\x06 \x01(\t\x12\x11\n\tuser_face\x18\x07 \x01(\t\x12\x10\n\x08user_url\x18\x08 \x01(\t\x12:\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32(.bilibili.app.nativeact.v1.NewactFeature\"5\n\x13NewactStatementItem\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\"_\n\x0fNewactStatement\x12\r\n\x05title\x18\x01 \x01(\t\x12=\n\x05items\x18\x02 \x03(\x0b\x32..bilibili.app.nativeact.v1.NewactStatementItem\"G\n\x0cOfficialInfo\x12\x0c\n\x04role\x18\x01 \x01(\x05\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\"\x95\x01\n\x0fOgvFollowButton\x12\x13\n\x0bis_followed\x18\x01 \x01(\x08\x12\x13\n\x0b\x66ollow_text\x18\x02 \x01(\t\x12\x13\n\x0b\x66ollow_icon\x18\x03 \x01(\t\x12\x15\n\runfollow_text\x18\x04 \x01(\t\x12\x15\n\runfollow_icon\x18\x05 \x01(\t\x12\x15\n\rfollow_params\x18\x06 \x01(\t\"M\n\x0bOgvMoreCard\x12\x13\n\x0b\x62utton_text\x18\x01 \x01(\t\x12\x19\n\x11supernatant_title\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\t\"\x94\x03\n\nOgvOneCard\x12\x11\n\tposition1\x18\x01 \x01(\t\x12\x11\n\tposition2\x18\x02 \x01(\t\x12\x11\n\tposition3\x18\x03 \x01(\t\x12\x19\n\x11\x63over_right_text1\x18\x04 \x01(\t\x12\x19\n\x11\x63over_right_text2\x18\x05 \x01(\t\x12\x14\n\x0crcmd_content\x18\x06 \x01(\t\x12\x11\n\trcmd_icon\x18\x07 \x01(\t\x12\x41\n\rfollow_button\x18\x08 \x01(\x0b\x32*.bilibili.app.nativeact.v1.OgvFollowButton\x12\r\n\x05image\x18\r \x01(\t\x12/\n\x05\x62\x61\x64ge\x18\x0e \x01(\x0b\x32 .bilibili.app.nativeact.v1.Badge\x12\r\n\x05title\x18\x0f \x01(\t\x12\x38\n\nreport_dic\x18\x10 \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReportDic\x12\x0b\n\x03url\x18\x11 \x01(\t\x12\x15\n\rresource_type\x18\x12 \x01(\t\"M\n\x14OgvSupernatantParams\x12\x12\n\nlast_index\x18\x01 \x01(\x03\x12\x0e\n\x06offset\x18\x02 \x01(\x03\x12\x11\n\tmodule_id\x18\x03 \x01(\x03\"\x81\x01\n\x11OgvSupernatantReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12?\n\x06params\x18\x02 \x01(\x0b\x32/.bilibili.app.nativeact.v1.OgvSupernatantParams\x12\x17\n\x0fprimary_page_id\x18\x03 \x01(\x03\"[\n\x12OgvSupernatantResp\x12\x31\n\x06module\x18\x01 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\x12\x12\n\nlast_index\x18\x02 \x01(\x03\"\xaa\x02\n\x0cOgvThreeCard\x12\x18\n\x10\x63over_left_text1\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x41\n\rfollow_button\x18\x03 \x01(\x0b\x32*.bilibili.app.nativeact.v1.OgvFollowButton\x12\r\n\x05image\x18\x04 \x01(\t\x12/\n\x05\x62\x61\x64ge\x18\x05 \x01(\x0b\x32 .bilibili.app.nativeact.v1.Badge\x12\r\n\x05title\x18\x06 \x01(\t\x12\x38\n\nreport_dic\x18\x07 \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReportDic\x12\x0b\n\x03url\x18\x08 \x01(\t\x12\x15\n\rresource_type\x18\t \x01(\t\"\x91\x04\n\x08PageResp\x12\x11\n\tis_online\x18\x01 \x01(\x08\x12\x1d\n\x15ignore_app_dark_theme\x18\x02 \x01(\x08\x12\x34\n\npage_color\x18\x03 \x01(\x0b\x32 .bilibili.app.nativeact.v1.Color\x12\x38\n\npage_share\x18\x04 \x01(\x0b\x32$.bilibili.app.nativeact.v1.PageShare\x12\x36\n\x0bpage_header\x18\x05 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\x12\x38\n\rparticipation\x18\x06 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\x12\x36\n\x0bmodule_list\x18\x07 \x03(\x0b\x32!.bilibili.app.nativeact.v1.Module\x12\x17\n\x0fis_dynamic_feed\x18\x08 \x01(\x08\x12>\n\rlayer_dynamic\x18\t \x01(\x0b\x32\'.bilibili.app.nativeact.v1.LayerDynamic\x12\x16\n\x0eis_editor_feed\x18\n \x01(\x08\x12\x14\n\x0csponsor_type\x18\x0b \x01(\x03\x12\x32\n\x07top_tab\x18\x0c \x01(\x0b\x32!.bilibili.app.nativeact.v1.TopTab\"\xc5\x01\n\tPageShare\x12\x0c\n\x04type\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\r\n\x05image\x18\x04 \x01(\t\x12\x12\n\ninside_uri\x18\x05 \x01(\t\x12\x13\n\x0boutside_uri\x18\x06 \x01(\t\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x0b\n\x03sid\x18\x08 \x01(\t\x12\x16\n\x0espace_page_url\x18\t \x01(\t\x12 \n\x18space_exclusive_page_url\x18\n \x01(\t\"{\n\x11ParticipationCard\x12\r\n\x05image\x18\x01 \x01(\t\x12\x16\n\x0eselected_image\x18\x02 \x01(\t\x12?\n\x05items\x18\x03 \x03(\x0b\x32\x30.bilibili.app.nativeact.v1.ParticipationCardItem\"P\n\x15ParticipationCardItem\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\r\n\x05title\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\"@\n\x0fPlayerDimension\x12\r\n\x05width\x18\x01 \x01(\x03\x12\x0e\n\x06height\x18\x02 \x01(\x03\x12\x0e\n\x06rotate\x18\x03 \x01(\x08\"\xae\x02\n\x0cProgressCard\x12\x37\n\x05style\x18\x01 \x01(\x0e\x32(.bilibili.app.nativeact.v1.ProgressStyle\x12:\n\tslot_type\x18\x02 \x01(\x0e\x32\'.bilibili.app.nativeact.v1.ProgressSlot\x12\x38\n\x08\x62\x61r_type\x18\x03 \x01(\x0e\x32&.bilibili.app.nativeact.v1.ProgressBar\x12\x15\n\rtexture_image\x18\x04 \x01(\t\x12\x0b\n\x03num\x18\x05 \x01(\x03\x12\x13\n\x0b\x64isplay_num\x18\x06 \x01(\t\x12\x36\n\x05nodes\x18\x07 \x03(\x0b\x32\'.bilibili.app.nativeact.v1.ProgressNode\"]\n\rProgressEvent\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12;\n\x05items\x18\x02 \x03(\x0b\x32,.bilibili.app.nativeact.v1.ProgressEventItem\"x\n\x11ProgressEventItem\x12\x0f\n\x07item_id\x18\x01 \x01(\x03\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03num\x18\x03 \x01(\x03\x12\x13\n\x0b\x64isplay_num\x18\x04 \x01(\t\x12\x0f\n\x07web_key\x18\x05 \x01(\t\x12\x11\n\tdimension\x18\x06 \x01(\x03\">\n\x0cProgressNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03num\x18\x02 \x01(\x03\x12\x13\n\x0b\x64isplay_num\x18\x03 \x01(\t\"\x1e\n\x0bProgressReq\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\"F\n\x0bProgressRly\x12\x37\n\x05\x65vent\x18\x01 \x01(\x0b\x32(.bilibili.app.nativeact.v1.ProgressEvent\"\xa4\x02\n\x08RcmdCard\x12\x0b\n\x03mid\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x66\x61\x63\x65\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x13\n\x0bis_followed\x18\x06 \x01(\x08\x12\x39\n\x08official\x18\x07 \x01(\x0b\x32\'.bilibili.app.nativeact.v1.OfficialInfo\x12/\n\x03vip\x18\x08 \x01(\x0b\x32\".bilibili.app.nativeact.v1.VipInfo\x12\x11\n\trank_icon\x18\t \x01(\t\x12>\n\rredirect_type\x18\n \x01(\x0e\x32\'.bilibili.app.nativeact.v1.RedirectType\"F\n\x10RcmdVerticalCard\x12\x32\n\x05items\x18\x01 \x03(\x0b\x32#.bilibili.app.nativeact.v1.RcmdCard\"i\n\x16RelativeactCapsuleCard\x12\r\n\x05title\x18\x01 \x01(\t\x12@\n\x05items\x18\x02 \x03(\x0b\x32\x31.bilibili.app.nativeact.v1.RelativeactCapsuleItem\"E\n\x16RelativeactCapsuleItem\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\"J\n\x0fRelativeactCard\x12\r\n\x05image\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\"+\n\tReplyCard\x12\x10\n\x08reply_id\x18\x01 \x01(\x03\x12\x0c\n\x04type\x18\x02 \x01(\x03\"\xa9\x01\n\tReportDic\x12\x10\n\x08\x62iz_type\x18\x01 \x01(\t\x12\x13\n\x0bseason_type\x18\x02 \x01(\t\x12\x0b\n\x03\x61id\x18\x03 \x01(\x03\x12\x0b\n\x03\x63id\x18\x04 \x01(\x03\x12\x10\n\x08sub_type\x18\x05 \x01(\x05\x12\r\n\x05\x65p_id\x18\x06 \x01(\x03\x12\x12\n\nis_preview\x18\x07 \x01(\x05\x12\x11\n\tseason_id\x18\x08 \x01(\x03\x12\x13\n\x0b\x61uthor_name\x18\t \x01(\t\"\x84\x02\n\rReserveButton\x12\x34\n\x04goto\x18\x01 \x01(\x0e\x32&.bilibili.app.nativeact.v1.ReserveGoto\x12:\n\x0bmessage_box\x18\x02 \x01(\x0b\x32%.bilibili.app.nativeact.v1.MessageBox\x12\x16\n\x0ereserve_params\x18\x03 \x01(\t\x12\x10\n\x08has_done\x18\x04 \x01(\x08\x12\x11\n\tdone_text\x18\x05 \x01(\t\x12\x13\n\x0bundone_text\x18\x06 \x01(\t\x12\x0c\n\x04icon\x18\x07 \x01(\t\x12\x14\n\x0cis_highlight\x18\x08 \x01(\x08\x12\x0b\n\x03url\x18\t \x01(\t\"\xe3\x01\n\x0bReserveCard\x12\x0b\n\x03sid\x18\x01 \x01(\x03\x12\x0b\n\x03mid\x18\x02 \x01(\x03\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x66\x61\x63\x65\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\x12\r\n\x05title\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0b\n\x03num\x18\x08 \x01(\x03\x12\x10\n\x08subtitle\x18\t \x01(\t\x12\x38\n\x06\x62utton\x18\n \x01(\x0b\x32(.bilibili.app.nativeact.v1.ReserveButton\x12\x18\n\x10hide_reserve_num\x18\x0b \x01(\x08\",\n\rReserveParams\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\x05\x12\x0b\n\x03sid\x18\x02 \x01(\x03\"Z\n\nReserveReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x38\n\x06params\x18\x02 \x01(\x0b\x32(.bilibili.app.nativeact.v1.ReserveParams\"$\n\nReserveRly\x12\x16\n\x0ereserve_params\x18\x01 \x01(\t\"\xc7\x02\n\x0cResourceCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x17\n\x0f\x63over_image_uri\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x18\n\x10\x63over_right_text\x18\x04 \x01(\t\x12\x18\n\x10\x63over_left_text1\x18\x05 \x01(\t\x12\x18\n\x10\x63over_left_icon1\x18\x06 \x01(\x03\x12\x18\n\x10\x63over_left_text2\x18\x07 \x01(\t\x12\x18\n\x10\x63over_left_icon2\x18\x08 \x01(\x03\x12/\n\x05\x62\x61\x64ge\x18\t \x01(\x0b\x32 .bilibili.app.nativeact.v1.Badge\x12\x38\n\nreport_dic\x18\n \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReportDic\x12\x15\n\rresource_type\x18\x0b \x01(\t\"k\n\x10ResourceMoreCard\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12<\n\x0csubpage_data\x18\x03 \x01(\x0b\x32&.bilibili.app.nativeact.v1.SubpageData\"\\\n\x0eResourceParams\x12\x0e\n\x06offset\x18\x01 \x01(\x03\x12\x14\n\x0ctopic_offset\x18\x02 \x01(\t\x12\x11\n\tmodule_id\x18\x03 \x01(\x03\x12\x11\n\tsort_type\x18\x04 \x01(\x03\"u\n\x0bResourceReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x39\n\x06params\x18\x02 \x01(\x0b\x32).bilibili.app.nativeact.v1.ResourceParams\x12\x17\n\x0fprimary_page_id\x18\x03 \x01(\x03\"A\n\x0cResourceResp\x12\x31\n\x06module\x18\x01 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\"W\n\nSelectCard\x12\x13\n\x0b\x63urrent_tab\x18\x01 \x01(\x03\x12\x34\n\x05items\x18\x02 \x03(\x0b\x32%.bilibili.app.nativeact.v1.SelectItem\"f\n\nSelectItem\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\x12\x38\n\npage_share\x18\x03 \x01(\x0b\x32$.bilibili.app.nativeact.v1.PageShare\"\xf3\x02\n\x07Setting\x12\x1b\n\x13\x64isplay_more_button\x18\x01 \x01(\x08\x12\x15\n\rdisplay_title\x18\x02 \x01(\x08\x12\x15\n\rauto_carousel\x18\x03 \x01(\x08\x12\x1a\n\x12top_tab_follow_img\x18\x04 \x01(\x08\x12\x19\n\x11top_tab_fade_away\x18\x05 \x01(\x08\x12\x11\n\tauto_play\x18\x06 \x01(\x08\x12\x1d\n\x15\x64isplay_unfold_button\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isplay_num\x18\x08 \x01(\x08\x12\x18\n\x10\x64isplay_view_num\x18\t \x01(\x08\x12\x1d\n\x15\x64isplay_subscribe_btn\x18\n \x01(\x08\x12\x13\n\x0bunfold_rest\x18\x0b \x01(\x08\x12\x1c\n\x14\x64isplay_progress_num\x18\x0c \x01(\x08\x12\x18\n\x10\x64isplay_node_num\x18\r \x01(\x08\x12\x19\n\x11\x64isplay_node_desc\x18\x0e \x01(\x08\"U\n\x05Share\x12\x15\n\rdisplay_later\x18\x01 \x01(\x08\x12\x0b\n\x03oid\x18\x02 \x01(\x03\x12\x14\n\x0cshare_origin\x18\x03 \x01(\t\x12\x12\n\nshare_type\x18\x04 \x01(\x03\"9\n\tSizeImage\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0e\n\x06height\x18\x02 \x01(\x03\x12\r\n\x05width\x18\x03 \x01(\x03\" \n\rStatementCard\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\"a\n\x0bSubpageData\x12\r\n\x05title\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\x33\n\x04tabs\x18\x03 \x03(\x0b\x32%.bilibili.app.nativeact.v1.SubpageTab\"*\n\nSubpageTab\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\"\xbd\x01\n\x07TabCard\x12\x13\n\x0b\x63urrent_tab\x18\x01 \x01(\x03\x12\x32\n\x05style\x18\x02 \x01(\x0e\x32#.bilibili.app.nativeact.v1.TabStyle\x12\x31\n\x05items\x18\x03 \x03(\x0b\x32\".bilibili.app.nativeact.v1.TabItem\x12\x36\n\x08\x62g_image\x18\x04 \x01(\x0b\x32$.bilibili.app.nativeact.v1.SizeImage\"\xd2\x01\n\x0bTabIndexReq\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\x15\n\rhttps_url_req\x18\x02 \x01(\x05\x12\x12\n\nfrom_spmid\x18\x03 \x01(\t\x12\x43\n\x0bplayer_args\x18\x04 \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x17\n\x0fprimary_page_id\x18\x05 \x01(\x03\x12\x12\n\nlocal_time\x18\x06 \x01(\x05\x12\x15\n\ris_cold_start\x18\x07 \x01(\x08\"\xdb\x01\n\x07TabItem\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\r\n\x05title\x18\x02 \x01(\t\x12\x15\n\rdisable_click\x18\x03 \x01(\x08\x12\x1b\n\x13\x64isable_click_toast\x18\x04 \x01(\t\x12<\n\x0eselected_image\x18\x05 \x01(\x0b\x32$.bilibili.app.nativeact.v1.SizeImage\x12>\n\x10unselected_image\x18\x06 \x01(\x0b\x32$.bilibili.app.nativeact.v1.SizeImage\"\x18\n\x08TextCard\x12\x0c\n\x04text\x18\x01 \x01(\t\"\x1e\n\rTextTitleCard\x12\r\n\x05title\x18\x01 \x01(\t\"i\n\x16TimelineEventImageCard\x12\x33\n\x05image\x18\x01 \x01(\x0b\x32$.bilibili.app.nativeact.v1.SizeImage\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\"j\n\x1aTimelineEventImagetextCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\x12\r\n\x05image\x18\x04 \x01(\t\x12\x0b\n\x03uri\x18\x05 \x01(\t\"\xf8\x01\n\x19TimelineEventResourceCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x17\n\x0f\x63over_image_uri\x18\x02 \x01(\t\x12\x0b\n\x03uri\x18\x03 \x01(\t\x12\x11\n\tposition1\x18\x04 \x01(\t\x12\x11\n\tposition2\x18\x05 \x01(\t\x12/\n\x05\x62\x61\x64ge\x18\x06 \x01(\x0b\x32 .bilibili.app.nativeact.v1.Badge\x12\x38\n\nreport_dic\x18\x07 \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReportDic\x12\x15\n\rresource_type\x18\x08 \x01(\t\"V\n\x15TimelineEventTextCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\"!\n\x10TimelineHeadCard\x12\r\n\x05stage\x18\x01 \x01(\t\"R\n\x10TimelineMoreCard\x12\x13\n\x0b\x62utton_text\x18\x01 \x01(\t\x12\x19\n\x11supernatant_title\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\t\"R\n\x19TimelineSupernatantParams\x12\x12\n\nlast_index\x18\x01 \x01(\x03\x12\x0e\n\x06offset\x18\x02 \x01(\x03\x12\x11\n\tmodule_id\x18\x03 \x01(\x03\"\x8b\x01\n\x16TimelineSupernatantReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x44\n\x06params\x18\x02 \x01(\x0b\x32\x34.bilibili.app.nativeact.v1.TimelineSupernatantParams\x12\x17\n\x0fprimary_page_id\x18\x03 \x01(\x03\"`\n\x17TimelineSupernatantResp\x12\x31\n\x06module\x18\x01 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\x12\x12\n\nlast_index\x18\x02 \x01(\x03\"\xce\x04\n\x12TimelineUnfoldCard\x12\x13\n\x0bunfold_text\x18\x01 \x01(\t\x12\x11\n\tfold_text\x18\x02 \x01(\t\x12\x41\n\x05\x63\x61rds\x18\x03 \x03(\x0b\x32\x32.bilibili.app.nativeact.v1.TimelineUnfoldCard.Card\x1a\xcc\x03\n\x04\x43\x61rd\x12I\n\x12timeline_head_card\x18\x01 \x01(\x0b\x32+.bilibili.app.nativeact.v1.TimelineHeadCardH\x00\x12T\n\x18timeline_event_text_card\x18\x02 \x01(\x0b\x32\x30.bilibili.app.nativeact.v1.TimelineEventTextCardH\x00\x12V\n\x19timeline_event_image_card\x18\x03 \x01(\x0b\x32\x31.bilibili.app.nativeact.v1.TimelineEventImageCardH\x00\x12^\n\x1dtimeline_event_imagetext_card\x18\x04 \x01(\x0b\x32\x35.bilibili.app.nativeact.v1.TimelineEventImagetextCardH\x00\x12\\\n\x1ctimeline_event_resource_card\x18\x05 \x01(\x0b\x32\x34.bilibili.app.nativeact.v1.TimelineEventResourceCardH\x00\x42\r\n\x0b\x63\x61rd_detail\"\xb8\x02\n\rTopicIndexReq\x12\x0f\n\x07page_id\x18\x01 \x01(\x03\x12\x15\n\ractivity_from\x18\x02 \x01(\t\x12\x12\n\ndynamic_id\x18\x03 \x01(\x03\x12\x14\n\x0cshare_origin\x18\x04 \x01(\t\x12\x0e\n\x06tab_id\x18\x05 \x01(\x03\x12\x15\n\rtab_module_id\x18\x06 \x01(\x03\x12\x15\n\rhttps_url_req\x18\x07 \x01(\x05\x12\x12\n\nfrom_spmid\x18\x08 \x01(\t\x12\x13\n\x0b\x63urrent_tab\x18\t \x01(\t\x12\x43\n\x0bplayer_args\x18\n \x01(\x0b\x32..bilibili.app.archive.middleware.v1.PlayerArgs\x12\x12\n\nlocal_time\x18\x0b \x01(\x05\x12\x15\n\ris_cold_start\x18\x0c \x01(\x08\"\x9f\x01\n\x06TopTab\x12\x11\n\tbg_image1\x18\x01 \x01(\t\x12\x11\n\tbg_image2\x18\x02 \x01(\t\x12\x15\n\rtab_top_color\x18\x03 \x01(\t\x12\x18\n\x10tab_middle_color\x18\x04 \x01(\t\x12\x18\n\x10tab_bottom_color\x18\x05 \x01(\t\x12\x12\n\nfont_color\x18\x06 \x01(\t\x12\x10\n\x08\x62\x61r_type\x18\x07 \x01(\x03\"\x87\x03\n\tVideoCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x17\n\x0f\x63over_image_uri\x18\x02 \x01(\t\x12\x18\n\x10\x63over_left_text1\x18\x03 \x01(\t\x12\x18\n\x10\x63over_left_text2\x18\x04 \x01(\t\x12\x18\n\x10\x63over_left_text3\x18\x05 \x01(\t\x12\x0b\n\x03uri\x18\x06 \x01(\t\x12/\n\x05\x62\x61\x64ge\x18\x07 \x01(\x0b\x32 .bilibili.app.nativeact.v1.Badge\x12\x36\n\x06rights\x18\x08 \x01(\x0b\x32&.bilibili.app.nativeact.v1.VideoRights\x12=\n\tdimension\x18\t \x01(\x0b\x32*.bilibili.app.nativeact.v1.PlayerDimension\x12\x38\n\nreport_dic\x18\n \x01(\x0b\x32$.bilibili.app.nativeact.v1.ReportDic\x12\x15\n\rresource_type\x18\x0b \x01(\t\"h\n\rVideoMoreCard\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12<\n\x0csubpage_data\x18\x03 \x01(\x0b\x32&.bilibili.app.nativeact.v1.SubpageData\"Y\n\x0bVideoParams\x12\x0e\n\x06offset\x18\x01 \x01(\x03\x12\x14\n\x0ctopic_offset\x18\x02 \x01(\t\x12\x11\n\tmodule_id\x18\x03 \x01(\x03\x12\x11\n\tsort_type\x18\x04 \x01(\x03\"o\n\x08VideoReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x36\n\x06params\x18\x02 \x01(\x0b\x32&.bilibili.app.nativeact.v1.VideoParams\x12\x17\n\x0fprimary_page_id\x18\x03 \x01(\x03\">\n\tVideoResp\x12\x31\n\x06module\x18\x01 \x01(\x0b\x32!.bilibili.app.nativeact.v1.Module\"F\n\x0bVideoRights\x12\x0f\n\x07ugc_pay\x18\x01 \x01(\x08\x12\x16\n\x0eis_cooperation\x18\x02 \x01(\x08\x12\x0e\n\x06is_pgc\x18\x03 \x01(\x08\"\xf5\x01\n\x07VipInfo\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0e\n\x06status\x18\x02 \x01(\x05\x12\x10\n\x08\x64ue_date\x18\x03 \x01(\x03\x12\x14\n\x0cvip_pay_type\x18\x04 \x01(\x05\x12\x12\n\ntheme_type\x18\x05 \x01(\x05\x12\x32\n\x05label\x18\x06 \x01(\x0b\x32#.bilibili.app.nativeact.v1.VipLabel\x12\x18\n\x10\x61vatar_subscript\x18\x07 \x01(\x05\x12\x16\n\x0enickname_color\x18\x08 \x01(\t\x12\x0c\n\x04role\x18\t \x01(\x03\x12\x1c\n\x14\x61vatar_subscript_url\x18\n \x01(\t\"\x89\x01\n\x08VipLabel\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x03 \x01(\t\x12\x13\n\x0blabel_theme\x18\x04 \x01(\t\x12\x12\n\ntext_color\x18\x05 \x01(\t\x12\x10\n\x08\x62g_style\x18\x06 \x01(\x05\x12\x10\n\x08\x62g_color\x18\x07 \x01(\t\x12\x14\n\x0c\x62order_color\x18\x08 \x01(\t\"\xe1\x01\n\nVoteButton\x12-\n\x04\x61rea\x18\x01 \x01(\x0b\x32\x1f.bilibili.app.nativeact.v1.Area\x12\x12\n\ndone_image\x18\x02 \x01(\t\x12\x14\n\x0cundone_image\x18\x03 \x01(\t\x12\x11\n\thas_voted\x18\x04 \x01(\x08\x12:\n\x0bmessage_box\x18\x05 \x01(\x0b\x32%.bilibili.app.nativeact.v1.MessageBox\x12\x13\n\x0bvote_params\x18\x06 \x01(\t\x12\x16\n\x0esource_item_id\x18\x07 \x01(\x03\"\xff\x01\n\x08VoteCard\x12\x36\n\x08\x62g_image\x18\x01 \x01(\x0b\x32$.bilibili.app.nativeact.v1.SizeImage\x12\x12\n\noption_num\x18\x02 \x01(\x03\x12\x36\n\x07\x62uttons\x18\x03 \x03(\x0b\x32%.bilibili.app.nativeact.v1.VoteButton\x12\x34\n\x08left_num\x18\x04 \x01(\x0b\x32\".bilibili.app.nativeact.v1.VoteNum\x12\x39\n\x08progress\x18\x05 \x01(\x0b\x32\'.bilibili.app.nativeact.v1.VoteProgress\"E\n\x07VoteNum\x12-\n\x04\x61rea\x18\x01 \x01(\x0b\x32\x1f.bilibili.app.nativeact.v1.Area\x12\x0b\n\x03num\x18\x02 \x01(\x03\"\\\n\nVoteParams\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\x05\x12\x0b\n\x03sid\x18\x02 \x01(\x03\x12\x0b\n\x03gid\x18\x03 \x01(\x03\x12\x16\n\x0esource_item_id\x18\x04 \x01(\x03\x12\x0c\n\x04type\x18\x05 \x01(\t\"\x8b\x02\n\x0cVoteProgress\x12-\n\x04\x61rea\x18\x01 \x01(\x0b\x32\x1f.bilibili.app.nativeact.v1.Area\x12;\n\x05style\x18\x02 \x01(\x0e\x32,.bilibili.app.nativeact.v1.VoteProgressStyle\x12G\n\x05items\x18\x03 \x03(\x0b\x32\x38.bilibili.app.nativeact.v1.VoteProgress.VoteProgressItem\x1a\x46\n\x10VoteProgressItem\x12\r\n\x05\x63olor\x18\x01 \x01(\t\x12\x0b\n\x03num\x18\x02 \x01(\x03\x12\x16\n\x0esource_item_id\x18\x03 \x01(\x03\"T\n\x07VoteReq\x12\x12\n\nraw_params\x18\x01 \x01(\t\x12\x35\n\x06params\x18\x02 \x01(\x0b\x32%.bilibili.app.nativeact.v1.VoteParams\"G\n\x08VoteResp\x12\x13\n\x0bvote_params\x18\x01 \x01(\t\x12\x10\n\x08left_num\x18\x02 \x01(\x03\x12\x14\n\x0c\x63\x61n_vote_num\x18\x03 \x01(\x03*+\n\nActionType\x12\x0b\n\x07\x44\x65\x66\x61ult\x10\x00\x12\x06\n\x02\x44o\x10\x01\x12\x08\n\x04Undo\x10\x02*\'\n\x0eMessageBoxType\x12\n\n\x06\x44ialog\x10\x00\x12\t\n\x05Toast\x10\x01*>\n\x0bProgressBar\x12\x0f\n\x0bPBarDefault\x10\x00\x12\r\n\tPBarColor\x10\x01\x12\x0f\n\x0bPBarTexture\x10\x02*A\n\x0cProgressSlot\x12\x10\n\x0cPSlotDefault\x10\x00\x12\x10\n\x0cPSlotOutline\x10\x01\x12\r\n\tPSlotFill\x10\x02*X\n\rProgressStyle\x12\x11\n\rPStyleDefault\x10\x00\x12\x0f\n\x0bPStyleRound\x10\x01\x12\x13\n\x0fPStyleRectangle\x10\x02\x12\x0e\n\nPStyleNode\x10\x03*A\n\x0cRedirectType\x12\x11\n\rRtTypeDefault\x10\x00\x12\x0f\n\x0bRtTypeSpace\x10\x01\x12\r\n\tRtTypeUri\x10\x02*4\n\x0bReserveGoto\x12\x0b\n\x07Reserve\x10\x00\x12\x0c\n\x08Redirect\x10\x01\x12\n\n\x06Unable\x10\x02*E\n\x08TabStyle\x12\x13\n\x0fTabStyleDefault\x10\x00\x12\x11\n\rTabStyleColor\x10\x01\x12\x11\n\rTabStyleImage\x10\x02*M\n\x11VoteProgressStyle\x12\x12\n\x0eVPStyleDefault\x10\x00\x12\x11\n\rVPStyleCircle\x10\x01\x12\x11\n\rVPStyleSquare\x10\x02\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.nativeact.v1.nativeact_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playeronline/v1/playeronline.proto` & `bilirpc-1.2/bilirpc/bilibili/app/playeronline/v1/playeronline.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/playeronline/v1/playeronline_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.playeronline.v1 import playeronline_pb2 as bilibili_dot_app_dot_playeronline_dot_v1_dot_playeronline__pb2
+from bilirpc.bilibili.app.playeronline.v1 import playeronline_pb2 as bilibili_dot_app_dot_playeronline_dot_v1_dot_playeronline__pb2
 
 
 class PlayerOnlineStub(object):
     """在线人数
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/playerunite/pgcanymodel/pgcanymodel_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.pgc.gateway.player.v2 import playurl_pb2 as bilibili_dot_pgc_dot_gateway_dot_player_dot_v2_dot_playurl__pb2
+from bilirpc.bilibili.pgc.gateway.player.v2 import playurl_pb2 as bilibili_dot_pgc_dot_gateway_dot_player_dot_v2_dot_playurl__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6bilibili/app/playerunite/pgcanymodel/pgcanymodel.proto\x12$bilibili.app.playerunite.pgcanymodel\x1a,bilibili/pgc/gateway/player/v2/playurl.proto\"\xd7\x02\n\x0bPGCAnyModel\x12\x46\n\x08\x62usiness\x18\x03 \x01(\x0b\x32\x34.bilibili.pgc.gateway.player.v2.PlayViewBusinessInfo\x12\x34\n\x05\x65vent\x18\x04 \x01(\x0b\x32%.bilibili.pgc.gateway.player.v2.Event\x12;\n\tview_info\x18\x05 \x01(\x0b\x32(.bilibili.pgc.gateway.player.v2.ViewInfo\x12I\n\rplay_ext_conf\x18\x06 \x01(\x0b\x32\x32.bilibili.pgc.gateway.player.v2.PlayAbilityExtConf\x12\x42\n\rplay_ext_info\x18\x07 \x01(\x0b\x32+.bilibili.pgc.gateway.player.v2.PlayExtInfob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.playerunite.pgcanymodel.pgcanymodel_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/playerunite/ugcanymodel/ugcanymodel_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playerunite/v1/playerunite.proto` & `bilirpc-1.2/bilirpc/bilibili/app/playerunite/v1/playerunite.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.playershared import playershared_pb2 as bilibili_dot_playershared_dot_playershared__pb2
+from bilirpc.bilibili.playershared import playershared_pb2 as bilibili_dot_playershared_dot_playershared__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-bilibili/app/playerunite/v1/playerunite.proto\x12\x1b\x62ilibili.app.playerunite.v1\x1a(bilibili/playershared/playershared.proto\x1a\x19google/protobuf/any.proto\"\xf0\x01\n\x10PlayViewUniteReq\x12,\n\x03vod\x18\x01 \x01(\x0b\x32\x1f.bilibili.playershared.VideoVod\x12\r\n\x05spmid\x18\x02 \x01(\t\x12\x12\n\nfrom_spmid\x18\x03 \x01(\t\x12V\n\rextra_content\x18\x04 \x03(\x0b\x32?.bilibili.app.playerunite.v1.PlayViewUniteReq.ExtraContentEntry\x1a\x33\n\x11\x45xtraContentEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb7\x03\n\x12PlayViewUniteReply\x12\x30\n\x08vod_info\x18\x01 \x01(\x0b\x32\x1e.bilibili.playershared.VodInfo\x12\x39\n\rplay_arc_conf\x18\x02 \x01(\x0b\x32\".bilibili.playershared.PlayArcConf\x12?\n\x10play_device_conf\x18\x03 \x01(\x0b\x32%.bilibili.playershared.PlayDeviceConf\x12+\n\x05\x65vent\x18\x04 \x01(\x0b\x32\x1c.bilibili.playershared.Event\x12(\n\nsupplement\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x30\n\x08play_arc\x18\x06 \x01(\x0b\x32\x1e.bilibili.playershared.PlayArc\x12\x39\n\rqn_trial_info\x18\x07 \x01(\x0b\x32\".bilibili.playershared.QnTrialInfo\x12/\n\x07history\x18\x08 \x01(\x0b\x32\x1e.bilibili.playershared.History2y\n\x06Player\x12o\n\rPlayViewUnite\x12-.bilibili.app.playerunite.v1.PlayViewUniteReq\x1a/.bilibili.app.playerunite.v1.PlayViewUniteReplyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/playerunite/v1/playerunite_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.playerunite.v1 import playerunite_pb2 as bilibili_dot_app_dot_playerunite_dot_v1_dot_playerunite__pb2
+from bilirpc.bilibili.app.playerunite.v1 import playerunite_pb2 as bilibili_dot_app_dot_playerunite_dot_v1_dot_playerunite__pb2
 
 
 class PlayerStub(object):
-    """统一视频url
+    """统一视频url
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -19,19 +19,19 @@
                 '/bilibili.app.playerunite.v1.Player/PlayViewUnite',
                 request_serializer=bilibili_dot_app_dot_playerunite_dot_v1_dot_playerunite__pb2.PlayViewUniteReq.SerializeToString,
                 response_deserializer=bilibili_dot_app_dot_playerunite_dot_v1_dot_playerunite__pb2.PlayViewUniteReply.FromString,
                 )
 
 
 class PlayerServicer(object):
-    """统一视频url
+    """统一视频url
     """
 
     def PlayViewUnite(self, request, context):
-        """视频地址
+        """视频地址
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_PlayerServicer_to_server(servicer, server):
@@ -45,15 +45,15 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bilibili.app.playerunite.v1.Player', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Player(object):
-    """统一视频url
+    """统一视频url
     """
 
     @staticmethod
     def PlayViewUnite(request,
             target,
             options=(),
             channel_credentials=None,
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playurl/v1/playurl.proto` & `bilirpc-1.2/bilirpc/bilibili/app/playurl/v1/playurl.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playurl/v1/playurl_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/playurl/v1/playurl_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/playurl/v1/playurl_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/playurl/v1/playurl_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/resource/privacy/v1/api.proto` & `bilirpc-1.2/bilirpc/bilibili/app/resource/privacy/v1/api.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/resource/privacy/v1/api_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/resource/privacy/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/resource/privacy/v1/api_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/resource/privacy/v1/api_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.resource.privacy.v1 import api_pb2 as bilibili_dot_app_dot_resource_dot_privacy_dot_v1_dot_api__pb2
+from bilirpc.bilibili.app.resource.privacy.v1 import api_pb2 as bilibili_dot_app_dot_resource_dot_privacy_dot_v1_dot_api__pb2
 
 
 class PrivacyStub(object):
     """隐私
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/resource/v1/module.proto` & `bilirpc-1.2/bilirpc/bilibili/app/resource/v1/module.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/resource/v1/module_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/resource/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/resource/v1/module_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/resource/v1/module_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.resource.v1 import module_pb2 as bilibili_dot_app_dot_resource_dot_v1_dot_module__pb2
+from bilirpc.bilibili.app.resource.v1 import module_pb2 as bilibili_dot_app_dot_resource_dot_v1_dot_module__pb2
 
 
 class ModuleStub(object):
     """
     """
 
     def __init__(self, channel):
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/search/v2/search.proto` & `bilirpc-1.2/bilirpc/bilibili/app/search/v2/search.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/search/v2/search_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/search/v2/search_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from bilibili.broadcast.message.main import search_pb2 as bilibili_dot_broadcast_dot_message_dot_main_dot_search__pb2
+from bilirpc.bilibili.broadcast.message.main import search_pb2 as bilibili_dot_broadcast_dot_message_dot_main_dot_search__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#bilibili/app/search/v2/search.proto\x12\x16\x62ilibili.app.search.v2\x1a,bilibili/broadcast/message/main/search.proto\"<\n\x11\x43\x61ncelChatTaskReq\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x13\n\x0b\x66rom_source\x18\x02 \x01(\t\"#\n\x13\x43\x61ncelChatTaskReply\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\"J\n\x10GetChatResultReq\x12\r\n\x05query\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x13\n\x0b\x66rom_source\x18\x03 \x01(\t\"\xf2\x01\n\rSearchEggInfo\x12\x10\n\x08\x65gg_type\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x15\n\ris_commercial\x18\x03 \x01(\x05\x12\x12\n\nmask_color\x18\x04 \x01(\t\x12\x19\n\x11mask_transparency\x18\x05 \x01(\x03\x12\x0b\n\x03md5\x18\x06 \x01(\t\x12\x0f\n\x07re_type\x18\x07 \x01(\x05\x12\x0e\n\x06re_url\x18\x08 \x01(\t\x12\x10\n\x08re_value\x18\t \x01(\t\x12\x12\n\nshow_count\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x03\x12\x0e\n\x06source\x18\x0c \x01(\x03\x12\x0b\n\x03url\x18\r \x01(\t\"I\n\x0eSearchEggInfos\x12\x37\n\x08\x65gg_info\x18\x01 \x03(\x0b\x32%.bilibili.app.search.v2.SearchEggInfo\"d\n\x0eSearchEggReply\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0c\n\x04seid\x18\x02 \x01(\t\x12\x36\n\x06result\x18\x03 \x01(\x0b\x32&.bilibili.app.search.v2.SearchEggInfos\"\x0e\n\x0cSearchEggReq\"7\n\x13SubmitChatTaskReply\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x12\n\nsession_id\x18\x02 \x01(\t\"I\n\x11SubmitChatTaskReq\x12\r\n\x05query\x18\x01 \x01(\t\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12\x13\n\x0b\x66rom_source\x18\x03 \x01(\t2\x9f\x03\n\x06Search\x12h\n\x0e\x43\x61ncelChatTask\x12).bilibili.app.search.v2.CancelChatTaskReq\x1a+.bilibili.app.search.v2.CancelChatTaskReply\x12\x66\n\rGetChatResult\x12(.bilibili.app.search.v2.GetChatResultReq\x1a+.bilibili.broadcast.message.main.ChatResult\x12Y\n\tSearchEgg\x12$.bilibili.app.search.v2.SearchEggReq\x1a&.bilibili.app.search.v2.SearchEggReply\x12h\n\x0eSubmitChatTask\x12).bilibili.app.search.v2.SubmitChatTaskReq\x1a+.bilibili.app.search.v2.SubmitChatTaskReplyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'bilibili.app.search.v2.search_pb2', _globals)
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/search/v2/search_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/search/v2/search_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from bilibili.app.search.v2 import search_pb2 as bilibili_dot_app_dot_search_dot_v2_dot_search__pb2
-from bilibili.broadcast.message.main import search_pb2 as bilibili_dot_broadcast_dot_message_dot_main_dot_search__pb2
+from bilirpc.bilibili.app.search.v2 import search_pb2 as bilibili_dot_app_dot_search_dot_v2_dot_search__pb2
+from bilirpc.bilibili.broadcast.message.main import search_pb2 as bilibili_dot_broadcast_dot_message_dot_main_dot_search__pb2
 
 
 class SearchStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/gateway/v1/service.proto` & `bilirpc-1.2/bilirpc/bilibili/app/show/gateway/v1/service.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/gateway/v1/service_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/gateway/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/gateway/v1/service_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/gateway/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/mixture/v1/mixture.proto` & `bilirpc-1.2/bilirpc/bilibili/app/show/mixture/v1/mixture.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/mixture/v1/mixture_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/popular/v1/popular.proto` & `bilirpc-1.2/bilirpc/bilibili/app/show/popular/v1/popular.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/popular/v1/popular_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/popular/v1/popular_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/popular/v1/popular_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/popular/v1/popular_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/rank/v1/rank.proto` & `bilirpc-1.2/bilirpc/bilibili/app/show/rank/v1/rank.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/rank/v1/rank_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/rank/v1/rank_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/rank/v1/rank_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/rank/v1/rank_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/region/v1/region.proto` & `bilirpc-1.2/bilirpc/bilibili/app/show/region/v1/region.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/region/v1/region_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/region/v1/region_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/show/region/v1/region_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/show/region/v1/region_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/space/v1/space.proto` & `bilirpc-1.2/bilirpc/bilibili/app/space/v1/space.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/space/v1/space_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/space/v1/space_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/space/v1/space_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/space/v1/space_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/splash/v1/splash.proto` & `bilirpc-1.2/bilirpc/bilibili/app/splash/v1/splash.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/splash/v1/splash_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/splash/v1/splash_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/splash/v1/splash_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/splash/v1/splash_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/topic/v1/topic.proto` & `bilirpc-1.2/bilirpc/bilibili/app/topic/v1/topic.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/topic/v1/topic_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/topic/v1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/topic/v1/topic_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/topic/v1/topic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/view/v1/view.proto` & `bilirpc-1.2/bilirpc/bilibili/app/view/v1/view.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/view/v1/view_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/view/v1/view_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/view/v1/view_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/view/v1/view_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/viewunite/pgcanymodel_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/viewunite/pgcanymodel_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/viewunite/ugcanymodel_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/viewunite/ugcanymodel_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/viewunite/v1/viewunite.proto` & `bilirpc-1.2/bilirpc/bilibili/app/viewunite/v1/viewunite.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/viewunite/v1/viewunite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/wall/v1/wall.proto` & `bilirpc-1.2/bilirpc/bilibili/app/wall/v1/wall.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/wall/v1/wall_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/app/wall/v1/wall_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/app/wall/v1/wall_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/app/wall/v1/wall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/editor/notify.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/editor/notify.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/editor/notify_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/editor/notify_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/editor/notify_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/editor/notify_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/esports/notify_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/esports/notify_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/fission/notify_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/fission/notify_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/fission/notify_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/fission/notify_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/im/notify.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/im/notify.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/im/notify_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/im/notify_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/im/notify_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/im/notify_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/dm.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/dm.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/dm_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/dm_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/native.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/native.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/native_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/native_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/native_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/native_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/resource.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/resource.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/resource_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/resource_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/resource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/search.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/search.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/search_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/search_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/main/search_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/main/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/note/sync_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/note/sync_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/freya.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/freya.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/freya_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/freya_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/live.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/live.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/ogv/live_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/ogv/live_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/ticket/activitygame_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/ticket/activitygame_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/tv/proj.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/tv/proj.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/tv/proj_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/tv/proj_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/message/tv/proj_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/message/tv/proj_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/broadcast.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/broadcast.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/broadcast_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/broadcast_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/broadcast_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/laser_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/laser_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/laser_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/laser_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/mod_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/mod_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/mod_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/mod_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/push.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/push.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/push_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/push_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/push_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/push_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/room.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/room.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/room_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/room_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/room_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/room_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/test.proto` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/test.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/test_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/test_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v1/test_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v1/test_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v2/laser_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v2/laser_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/broadcast/v2/laser_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/broadcast/v2/laser_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/cheese/gateway/player/v1/playurl.proto` & `bilirpc-1.2/bilirpc/bilibili/cheese/gateway/player/v1/playurl.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/cheese/gateway/player/v1/playurl_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/interfacess/biligram/v1/biligram_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/community/interfacess/biligram/v1/biligram_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/service/dm/v1/dm.proto` & `bilirpc-1.2/bilirpc/bilibili/community/service/dm/v1/dm.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/service/dm/v1/dm_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/community/service/dm/v1/dm_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/service/dm/v1/dm_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/community/service/dm/v1/dm_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/service/govern/v1/govern.proto` & `bilirpc-1.2/bilirpc/bilibili/community/service/govern/v1/govern.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/service/govern/v1/govern_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/community/service/govern/v1/govern_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/community/service/govern/v1/govern_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/community/service/govern/v1/govern_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/__pycache__/common_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/__pycache__/common_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/common.proto` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/common.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/common/common_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/avatar_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/avatar_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/plugin_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/__pycache__/plugin_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/avatar.proto` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/avatar.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/avatar_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/avatar_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/plugin.proto` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/plugin.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dagw/component/avatar/v1/plugin_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/dagw/component/avatar/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/common/dynamic.proto` & `bilirpc-1.2/bilirpc/bilibili/dynamic/common/dynamic.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/common/dynamic_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/dynamic/common/dynamic_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/gw/gateway.proto` & `bilirpc-1.2/bilirpc/bilibili/dynamic/gw/gateway.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/gw/gateway_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/dynamic/gw/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/feed/v1/api.proto` & `bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/feed/v1/api.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/dynamic/interfaces/feed/v1/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/gaia/gw/gw_api.proto` & `bilirpc-1.2/bilirpc/bilibili/gaia/gw/gw_api.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/gaia/gw/gw_api_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/gaia/gw/gw_api_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/gaia/gw/gw_api_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/gaia/gw/gw_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/interfaces/inner-interface/v1/api.proto` & `bilirpc-1.2/bilirpc/bilibili/im/interfaces/inner-interface/v1/api.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/im/interfaces/inner-interface/v1/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/interfaces/v1/im.proto` & `bilirpc-1.2/bilirpc/bilibili/im/interfaces/v1/im.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/interfaces/v1/im_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/im/interfaces/v1/im_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/interfaces/v1/im_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/im/interfaces/v1/im_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/type/im.proto` & `bilirpc-1.2/bilirpc/bilibili/im/type/im.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/im/type/im_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/im/type/im_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/live/app/room/v1/room.proto` & `bilirpc-1.2/bilirpc/bilibili/live/app/room/v1/room.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/live/app/room/v1/room_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/live/app/room/v1/room_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/live/general/interfaces/v1/interfaces.proto` & `bilirpc-1.2/bilirpc/bilibili/live/general/interfaces/v1/interfaces.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/live/general/interfaces/v1/interfaces_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/live/general/interfaces/v1/interfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/main/common/arch/doll/v1/doll.proto` & `bilirpc-1.2/bilirpc/bilibili/main/common/arch/doll/v1/doll.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/main/common/arch/doll/v1/doll_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/main/community/reply/v1/reply.proto` & `bilirpc-1.2/bilirpc/bilibili/main/community/reply/v1/reply.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/main/community/reply/v1/reply_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/main/community/reply/v1/reply_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/main/community/reply/v1/reply_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/main/community/reply/v1/reply_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/__pycache__/metadata_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/metadata/__pycache__/metadata_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/device/__pycache__/device_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/metadata/device/__pycache__/device_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/device/device.proto` & `bilirpc-1.2/bilirpc/bilibili/metadata/device/device.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/device/device_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/device/device_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/fawkes/fawkes.proto` & `bilirpc-1.2/bilirpc/bilibili/metadata/fawkes/fawkes.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/fawkes/fawkes_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/fawkes/fawkes_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/locale/__pycache__/locale_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/metadata/locale/__pycache__/locale_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/locale/locale.proto` & `bilirpc-1.2/bilirpc/bilibili/metadata/locale/locale.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/locale/locale_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/locale/locale_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/metadata_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/network/__pycache__/network_pb2.cpython-310.pyc` & `bilirpc-1.2/bilirpc/bilibili/metadata/network/__pycache__/network_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/network/network.proto` & `bilirpc-1.2/bilirpc/bilibili/metadata/network/network.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/network/network_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/network/network_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/parabox/parabox_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/parabox/parabox_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/restriction/restriction.proto` & `bilirpc-1.2/bilirpc/bilibili/metadata/restriction/restriction.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/metadata/restriction/restriction_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/metadata/restriction/restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pagination/pagination.proto` & `bilirpc-1.2/bilirpc/bilibili/pagination/pagination.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pagination/pagination_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/pagination/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/gallery.proto` & `bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/gallery.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/pangu/gallery/v1/gallery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v1/playurl.proto` & `bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v1/playurl.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v1/playurl_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v2/playurl.proto` & `bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v2/playurl.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/pgc/gateway/player/v2/playurl_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/service/premiere/v1/premiere.proto` & `bilirpc-1.2/bilirpc/bilibili/pgc/service/premiere/v1/premiere.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/pgc/service/premiere/v1/premiere_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/playershared/playershared.proto` & `bilirpc-1.2/bilirpc/bilibili/playershared/playershared.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/playershared/playershared_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/playershared/playershared_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/app/search/v1/search.proto` & `bilirpc-1.2/bilirpc/bilibili/polymer/app/search/v1/search.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/app/search/v1/search_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/app/search/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/app/search/v1/search_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/app/search/v1/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/community/govern/v1/govern.proto` & `bilirpc-1.2/bilirpc/bilibili/polymer/community/govern/v1/govern.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/community/govern/v1/govern_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/contract/v1/contract.proto` & `bilirpc-1.2/bilirpc/bilibili/polymer/contract/v1/contract.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/contract/v1/contract_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/contract/v1/contract_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/contract/v1/contract_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/contract/v1/contract_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/list/v1/list.proto` & `bilirpc-1.2/bilirpc/bilibili/polymer/list/v1/list.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/list/v1/list_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/list/v1/list_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/polymer/list/v1/list_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/polymer/list/v1/list_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/relation/interfaces/api.proto` & `bilirpc-1.2/bilirpc/bilibili/relation/interfaces/api.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/relation/interfaces/api_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/relation/interfaces/api_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/relation/interfaces/api_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/relation/interfaces/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/render/render_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/render/render_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/rpc/status_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/tv/interfaces/dm/v1/dm.proto` & `bilirpc-1.2/bilirpc/bilibili/tv/interfaces/dm/v1/dm.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/tv/interfaces/dm/v1/dm_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/tv/interfaces/dm/v1/dm_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/vega/deneb/v1/deneb.proto` & `bilirpc-1.2/bilirpc/bilibili/vega/deneb/v1/deneb.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/vega/deneb/v1/deneb_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/vega/deneb/v1/deneb_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/vega/deneb/v1/deneb_pb2_grpc.py` & `bilirpc-1.2/bilirpc/bilibili/vega/deneb/v1/deneb_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/web/interfaces/v1/interfaces.proto` & `bilirpc-1.2/bilirpc/bilibili/web/interfaces/v1/interfaces.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/web/interfaces/v1/interfaces_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/web/interfaces/v1/interfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/web/space/v1/space.proto` & `bilirpc-1.2/bilirpc/bilibili/web/space/v1/space.proto`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/bilibili/web/space/v1/space_pb2.py` & `bilirpc-1.2/bilirpc/bilibili/web/space/v1/space_pb2.py`

 * *Files identical despite different names*

### Comparing `bilirpc-1.1/bilirpc/tools.py` & `bilirpc-1.2/bilirpc/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 @IDE     :   PyCharm
 @Time    :   2022/9/23 17:37
 @Author  :   DMC ,
 """
 import hashlib
 import random
 from typing import Optional
-from bilibili.metadata.device.device_pb2 import Device
-from bilibili.metadata.locale.locale_pb2 import Locale
-from bilibili.metadata.network.network_pb2 import Network, NetworkType
-from bilibili.metadata.metadata_pb2 import Metadata
+from bilirpc.bilibili.metadata.device.device_pb2 import Device
+from bilirpc.bilibili.metadata.locale.locale_pb2 import Locale
+from bilirpc.bilibili.metadata.network.network_pb2 import Network, NetworkType
+from bilirpc.bilibili.metadata.metadata_pb2 import Metadata
 
 def fakebuvid():
     mac_list = []
     for _ in range(1, 7):
         rand_str = "".join(random.sample("0123456789abcdef", 2))
         mac_list.append(rand_str)
     rand_mac = ":".join(mac_list)
```

### Comparing `bilirpc-1.1/PKG-INFO` & `bilirpc-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilirpc
-Version: 1.1
+Version: 1.2
 Summary: B站grpc请求2
 License: MIT
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

