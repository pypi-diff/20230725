# Comparing `tmp/actnova-yolo-1.0.7.tar.gz` & `tmp/actnova-yolo-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actnova-yolo-1.0.7.tar", last modified: Tue Jul 25 09:43:18 2023, max compression
+gzip compressed data, was "actnova-yolo-1.0.8.tar", last modified: Tue Jul 25 09:46:41 2023, max compression
```

## Comparing `actnova-yolo-1.0.7.tar` & `actnova-yolo-1.0.8.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.192414 actnova-yolo-1.0.7/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5625 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/CONTRIBUTING.md
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    34523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/LICENSE
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      213 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/MANIFEST.in
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26768 2023-07-25 09:43:18.192618 actnova-yolo-1.0.7/PKG-INFO
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    25155 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/README.md
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24156 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/README.zh-CN.md
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.145115 actnova-yolo-1.0.7/actnova_yolo.egg-info/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26768 2023-07-25 09:43:18.000000 actnova-yolo-1.0.7/actnova_yolo.egg-info/PKG-INFO
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6102 2023-07-25 09:43:18.000000 actnova-yolo-1.0.7/actnova_yolo.egg-info/SOURCES.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        1 2023-07-25 09:43:18.000000 actnova-yolo-1.0.7/actnova_yolo.egg-info/dependency_links.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       93 2023-07-25 09:43:18.000000 actnova-yolo-1.0.7/actnova_yolo.egg-info/entry_points.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      394 2023-07-25 09:43:18.000000 actnova-yolo-1.0.7/actnova_yolo.egg-info/requires.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       12 2023-07-25 09:43:18.000000 actnova-yolo-1.0.7/actnova_yolo.egg-info/top_level.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/requirements.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      682 2023-07-25 09:43:18.193142 actnova-yolo-1.0.7/setup.cfg
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3098 2023-07-25 09:16:57.000000 actnova-yolo-1.0.7/setup.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.146020 actnova-yolo-1.0.7/tests/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/tests/test_cli.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4344 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/tests/test_engine.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7216 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/tests/test_python.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.146395 actnova-yolo-1.0.7/ultralytics/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      564 2023-07-25 09:43:10.000000 actnova-yolo-1.0.7/ultralytics/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.147829 actnova-yolo-1.0.7/ultralytics/assets/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)   137419 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/assets/bus.jpg
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    50427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.148896 actnova-yolo-1.0.7/ultralytics/cfg/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18847 2023-07-25 09:03:15.000000 actnova-yolo-1.0.7/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.152449 actnova-yolo-1.0.7/ultralytics/cfg/datasets/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2746 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1981 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9255 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3507 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3007 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1542 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1862 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1846 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      895 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1777 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7173 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.136006 actnova-yolo-1.0.7/ultralytics/cfg/models/
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.152903 actnova-yolo-1.0.7/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1970 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2177 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.153586 actnova-yolo-1.0.7/ultralytics/cfg/models/v3/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1537 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.154018 actnova-yolo-1.0.7/ultralytics/cfg/models/v5/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1923 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.154246 actnova-yolo-1.0.7/ultralytics/cfg/models/v6/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1735 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.156054 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1946 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1580 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1490 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1913 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.156607 actnova-yolo-1.0.7/ultralytics/cfg/trackers/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      694 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.159188 actnova-yolo-1.0.7/ultralytics/data/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      389 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1830 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/annotator.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/augment.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12660 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/base.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6562 2023-07-25 09:40:23.000000 actnova-yolo-1.0.7/ultralytics/data/build.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9180 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/converter.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.159663 actnova-yolo-1.0.7/ultralytics/data/dataloaders/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:42:31.000000 actnova-yolo-1.0.7/ultralytics/data/dataloaders/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13378 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/dataset.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/data/loaders.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26075 2023-07-25 09:42:08.000000 actnova-yolo-1.0.7/ultralytics/data/utils.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.161880 actnova-yolo-1.0.7/ultralytics/engine/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/engine/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    44686 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/engine/exporter.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19444 2023-07-25 09:06:02.000000 actnova-yolo-1.0.7/ultralytics/engine/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16516 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/engine/predictor.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24667 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/engine/results.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    31186 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/engine/trainer.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11754 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/engine/validator.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.163114 actnova-yolo-1.0.7/ultralytics/hub/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4393 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/hub/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/hub/auth.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8469 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/hub/session.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9425 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/hub/utils.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.163364 actnova-yolo-1.0.7/ultralytics/models/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       99 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.165160 actnova-yolo-1.0.7/ultralytics/models/fastsam/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      254 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4557 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/fastsam/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16752 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1986 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12414 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.166122 actnova-yolo-1.0.7/ultralytics/models/nas/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      179 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/nas/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5206 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/nas/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1445 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/nas/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      947 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/nas/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.167272 actnova-yolo-1.0.7/ultralytics/models/rtdetr/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      197 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7384 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2949 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6561 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.168441 actnova-yolo-1.0.7/ultralytics/models/sam/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      176 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13296 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/amg.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4822 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/build.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2522 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/model.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.170590 actnova-yolo-1.0.7/ultralytics/models/sam/modules/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6372 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    22545 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7309 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    21760 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8532 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18948 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.171249 actnova-yolo-1.0.7/ultralytics/models/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/utils/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13157 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/utils/loss.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12990 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.171751 actnova-yolo-1.0.7/ultralytics/models/yolo/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      182 2023-07-25 09:06:47.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.173129 actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      264 2023-07-25 08:46:18.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2375 2023-07-25 08:46:08.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2809 2023-07-25 08:46:07.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10917 2023-07-25 08:46:05.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.175460 actnova-yolo-1.0.7/ultralytics/models/yolo/classify/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1914 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4651 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.176367 actnova-yolo-1.0.7/ultralytics/models/yolo/detect/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      277 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5780 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/detect/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.177276 actnova-yolo-1.0.7/ultralytics/models/yolo/pose/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      247 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2369 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2788 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10911 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.178351 actnova-yolo-1.0.7/ultralytics/models/yolo/segment/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      295 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2833 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2497 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.179220 actnova-yolo-1.0.7/ultralytics/nn/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      586 2023-07-25 06:35:22.000000 actnova-yolo-1.0.7/ultralytics/nn/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26042 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.181684 actnova-yolo-1.0.7/ultralytics/nn/modules/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1587 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11841 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/modules/block.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/modules/conv.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16098 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/modules/head.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    15934 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3244 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/nn/modules/utils.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37093 2023-07-25 09:00:06.000000 actnova-yolo-1.0.7/ultralytics/nn/tasks.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.182964 actnova-yolo-1.0.7/ultralytics/trackers/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      227 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1609 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/basetrack.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5681 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14446 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2324 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/track.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.183882 actnova-yolo-1.0.7/ultralytics/trackers/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12209 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18420 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8749 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.188562 actnova-yolo-1.0.7/ultralytics/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    30200 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3864 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/autobatch.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16087 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.191020 actnova-yolo-1.0.7/ultralytics/utils/callbacks/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      214 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5593 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5974 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13115 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4386 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3363 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2701 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      608 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1716 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19224 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/checks.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2591 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/dist.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12818 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/downloads.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      312 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/errors.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5450 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/files.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/instance.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19144 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/loss.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42325 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/metrics.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    29212 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/ops.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1246 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/patches.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24845 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/plotting.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/tal.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    23082 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/torch_utils.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/utils/tuner.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.191242 actnova-yolo-1.0.7/ultralytics/yolo/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       94 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.191435 actnova-yolo-1.0.7/ultralytics/yolo/cfg/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      373 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/yolo/cfg/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.191630 actnova-yolo-1.0.7/ultralytics/yolo/data/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      823 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/yolo/data/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.191838 actnova-yolo-1.0.7/ultralytics/yolo/engine/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      385 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/yolo/engine/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.192027 actnova-yolo-1.0.7/ultralytics/yolo/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/yolo/utils/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:43:18.192211 actnova-yolo-1.0.7/ultralytics/yolo/v8/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      387 2023-07-25 05:23:34.000000 actnova-yolo-1.0.7/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.124180 actnova-yolo-1.0.8/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5625 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    34523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/LICENSE
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      213 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/MANIFEST.in
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26768 2023-07-25 09:46:41.124417 actnova-yolo-1.0.8/PKG-INFO
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    25155 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/README.md
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24156 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/README.zh-CN.md
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.080465 actnova-yolo-1.0.8/actnova_yolo.egg-info/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26768 2023-07-25 09:46:41.000000 actnova-yolo-1.0.8/actnova_yolo.egg-info/PKG-INFO
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6102 2023-07-25 09:46:41.000000 actnova-yolo-1.0.8/actnova_yolo.egg-info/SOURCES.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        1 2023-07-25 09:46:41.000000 actnova-yolo-1.0.8/actnova_yolo.egg-info/dependency_links.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       93 2023-07-25 09:46:41.000000 actnova-yolo-1.0.8/actnova_yolo.egg-info/entry_points.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      394 2023-07-25 09:46:41.000000 actnova-yolo-1.0.8/actnova_yolo.egg-info/requires.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       12 2023-07-25 09:46:41.000000 actnova-yolo-1.0.8/actnova_yolo.egg-info/top_level.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/requirements.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      682 2023-07-25 09:46:41.124985 actnova-yolo-1.0.8/setup.cfg
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3098 2023-07-25 09:16:57.000000 actnova-yolo-1.0.8/setup.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.081649 actnova-yolo-1.0.8/tests/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/tests/test_cli.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4344 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/tests/test_engine.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7216 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/tests/test_python.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.081967 actnova-yolo-1.0.8/ultralytics/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      564 2023-07-25 09:46:21.000000 actnova-yolo-1.0.8/ultralytics/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.083085 actnova-yolo-1.0.8/ultralytics/assets/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)   137419 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/assets/bus.jpg
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    50427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.083954 actnova-yolo-1.0.8/ultralytics/cfg/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18847 2023-07-25 09:03:15.000000 actnova-yolo-1.0.8/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.087388 actnova-yolo-1.0.8/ultralytics/cfg/datasets/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2746 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1981 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9255 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3507 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3007 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1542 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1862 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1846 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      895 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1777 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7173 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.073660 actnova-yolo-1.0.8/ultralytics/cfg/models/
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.087856 actnova-yolo-1.0.8/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1970 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2177 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.088549 actnova-yolo-1.0.8/ultralytics/cfg/models/v3/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1537 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.088981 actnova-yolo-1.0.8/ultralytics/cfg/models/v5/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1923 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.089183 actnova-yolo-1.0.8/ultralytics/cfg/models/v6/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1735 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.090810 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1946 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1580 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1490 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1913 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.091225 actnova-yolo-1.0.8/ultralytics/cfg/trackers/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      694 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.093474 actnova-yolo-1.0.8/ultralytics/data/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      389 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1830 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/annotator.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/augment.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12660 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/base.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6545 2023-07-25 09:45:32.000000 actnova-yolo-1.0.8/ultralytics/data/build.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9180 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/converter.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.093890 actnova-yolo-1.0.8/ultralytics/data/dataloaders/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:42:31.000000 actnova-yolo-1.0.8/ultralytics/data/dataloaders/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13378 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/dataset.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/data/loaders.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26075 2023-07-25 09:42:08.000000 actnova-yolo-1.0.8/ultralytics/data/utils.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.096250 actnova-yolo-1.0.8/ultralytics/engine/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/engine/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    44686 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/engine/exporter.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19444 2023-07-25 09:06:02.000000 actnova-yolo-1.0.8/ultralytics/engine/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16516 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/engine/predictor.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24667 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/engine/results.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    31186 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/engine/trainer.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11754 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/engine/validator.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.097173 actnova-yolo-1.0.8/ultralytics/hub/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4393 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/hub/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/hub/auth.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8469 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/hub/session.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9425 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/hub/utils.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.097386 actnova-yolo-1.0.8/ultralytics/models/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       99 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.098989 actnova-yolo-1.0.8/ultralytics/models/fastsam/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      254 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4557 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16752 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1986 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12414 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.099958 actnova-yolo-1.0.8/ultralytics/models/nas/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      179 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5206 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/nas/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1445 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/nas/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      947 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/nas/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.101009 actnova-yolo-1.0.8/ultralytics/models/rtdetr/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      197 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7384 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2949 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6561 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.101982 actnova-yolo-1.0.8/ultralytics/models/sam/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      176 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13296 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/amg.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4822 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/build.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2522 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/model.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.103969 actnova-yolo-1.0.8/ultralytics/models/sam/modules/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6372 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    22545 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7309 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    21760 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8532 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18948 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.104575 actnova-yolo-1.0.8/ultralytics/models/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13157 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/utils/loss.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12990 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.104798 actnova-yolo-1.0.8/ultralytics/models/yolo/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      182 2023-07-25 09:06:47.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.105974 actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      264 2023-07-25 08:46:18.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2375 2023-07-25 08:46:08.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2809 2023-07-25 08:46:07.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10917 2023-07-25 08:46:05.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.106835 actnova-yolo-1.0.8/ultralytics/models/yolo/classify/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1914 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4651 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.107700 actnova-yolo-1.0.8/ultralytics/models/yolo/detect/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      277 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5780 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/detect/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.108554 actnova-yolo-1.0.8/ultralytics/models/yolo/pose/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      247 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2369 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2788 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10911 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.109581 actnova-yolo-1.0.8/ultralytics/models/yolo/segment/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      295 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2833 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2497 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.110208 actnova-yolo-1.0.8/ultralytics/nn/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      586 2023-07-25 06:35:22.000000 actnova-yolo-1.0.8/ultralytics/nn/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26042 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.111857 actnova-yolo-1.0.8/ultralytics/nn/modules/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1587 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11841 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/modules/block.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16098 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/modules/head.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    15934 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3244 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37093 2023-07-25 09:00:06.000000 actnova-yolo-1.0.8/ultralytics/nn/tasks.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.112867 actnova-yolo-1.0.8/ultralytics/trackers/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      227 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1609 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5681 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14446 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2324 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/track.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.113709 actnova-yolo-1.0.8/ultralytics/trackers/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12209 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18420 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8749 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.119493 actnova-yolo-1.0.8/ultralytics/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    30200 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3864 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/autobatch.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16087 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.122396 actnova-yolo-1.0.8/ultralytics/utils/callbacks/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      214 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5593 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5974 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13115 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4386 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3363 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2701 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      608 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1716 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19224 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/checks.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2591 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/dist.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12818 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/downloads.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      312 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/errors.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5450 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/files.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/instance.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19144 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/loss.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42325 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/metrics.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    29212 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/ops.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1246 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/patches.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24845 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/plotting.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/tal.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    23082 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/utils/tuner.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.122786 actnova-yolo-1.0.8/ultralytics/yolo/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       94 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.123080 actnova-yolo-1.0.8/ultralytics/yolo/cfg/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      373 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/yolo/cfg/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.123316 actnova-yolo-1.0.8/ultralytics/yolo/data/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      823 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/yolo/data/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.123535 actnova-yolo-1.0.8/ultralytics/yolo/engine/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      385 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/yolo/engine/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.123739 actnova-yolo-1.0.8/ultralytics/yolo/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/yolo/utils/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:46:41.123947 actnova-yolo-1.0.8/ultralytics/yolo/v8/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      387 2023-07-25 05:23:34.000000 actnova-yolo-1.0.8/ultralytics/yolo/v8/__init__.py
```

### Comparing `actnova-yolo-1.0.7/CONTRIBUTING.md` & `actnova-yolo-1.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/LICENSE` & `actnova-yolo-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/PKG-INFO` & `actnova-yolo-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actnova-yolo
-Version: 1.0.7
+Version: 1.0.8
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification. modified for Actnova by HahmDY
 Home-page: https://github.com/HahmActnova/actnova_yolo
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Source, https://github.com/HahmActnova/actnova_yolo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.7 Summary: Ultralytics
+Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.8 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. modified for Actnova by HahmDY Home-
 page: https://github.com/HahmActnova/actnova_yolo Author: Ultralytics Author-
 email: hello@ultralytics.com License: AGPL-3.0 Project-URL: Bug Reports, https:
 //github.com/ultralytics/ultralytics/issues Project-URL: Source, https://
 github.com/HahmActnova/actnova_yolo Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
```

### Comparing `actnova-yolo-1.0.7/README.md` & `actnova-yolo-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/README.zh-CN.md` & `actnova-yolo-1.0.8/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/actnova_yolo.egg-info/PKG-INFO` & `actnova-yolo-1.0.8/actnova_yolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actnova-yolo
-Version: 1.0.7
+Version: 1.0.8
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification. modified for Actnova by HahmDY
 Home-page: https://github.com/HahmActnova/actnova_yolo
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Source, https://github.com/HahmActnova/actnova_yolo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.7 Summary: Ultralytics
+Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.8 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. modified for Actnova by HahmDY Home-
 page: https://github.com/HahmActnova/actnova_yolo Author: Ultralytics Author-
 email: hello@ultralytics.com License: AGPL-3.0 Project-URL: Bug Reports, https:
 //github.com/ultralytics/ultralytics/issues Project-URL: Source, https://
 github.com/HahmActnova/actnova_yolo Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
```

### Comparing `actnova-yolo-1.0.7/actnova_yolo.egg-info/SOURCES.txt` & `actnova-yolo-1.0.8/actnova_yolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/requirements.txt` & `actnova-yolo-1.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/setup.cfg` & `actnova-yolo-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/setup.py` & `actnova-yolo-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/tests/test_cli.py` & `actnova-yolo-1.0.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/tests/test_engine.py` & `actnova-yolo-1.0.8/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/tests/test_python.py` & `actnova-yolo-1.0.8/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/__init__.py` & `actnova-yolo-1.0.8/ultralytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 
 from ultralytics.engine.model import YOLO
 from ultralytics.hub import start
 from ultralytics.models import RTDETR, SAM
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import SETTINGS as settings
```

### Comparing `actnova-yolo-1.0.7/ultralytics/assets/bus.jpg` & `actnova-yolo-1.0.8/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/assets/zidane.jpg` & `actnova-yolo-1.0.8/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/__init__.py` & `actnova-yolo-1.0.8/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/Argoverse.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/ImageNet.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/Objects365.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/SKU-110K.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/VOC.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/VisDrone.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco-pose.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco128-seg.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco128.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco8-pose.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco8-seg.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/coco8.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/datasets/xView.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/default.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v3/yolov3.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v5/yolov5.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v6/yolov6.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/models/v8/yolov8.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/trackers/botsort.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/cfg/trackers/bytetrack.yaml` & `actnova-yolo-1.0.8/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/annotator.py` & `actnova-yolo-1.0.8/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/augment.py` & `actnova-yolo-1.0.8/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/base.py` & `actnova-yolo-1.0.8/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/build.py` & `actnova-yolo-1.0.8/ultralytics/data/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         rect=cfg.rect or rect,  # rectangular batches
         cache=cfg.cache or None,
         single_cls=cfg.single_cls or False,
         stride=int(stride),
         pad=0.0 if mode == 'train' else 0.5,
         prefix=colorstr(f'{mode}: '),
         use_segments=cfg.task == 'segment',
-        use_keypoints= (cfg.task == 'pose') AND (cfg.task == 'actnova'),
+        use_keypoints= cfg.task in ['pose', 'actnova'],
         classes=cfg.classes,
         data=data,
         fraction=cfg.fraction if mode == 'train' else 1.0)
 
 
 def build_dataloader(dataset, batch, workers, shuffle=True, rank=-1):
     """Return an InfiniteDataLoader or DataLoader for training or validation set."""
```

### Comparing `actnova-yolo-1.0.7/ultralytics/data/converter.py` & `actnova-yolo-1.0.8/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/dataset.py` & `actnova-yolo-1.0.8/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/loaders.py` & `actnova-yolo-1.0.8/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/data/utils.py` & `actnova-yolo-1.0.8/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/engine/exporter.py` & `actnova-yolo-1.0.8/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/engine/model.py` & `actnova-yolo-1.0.8/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/engine/predictor.py` & `actnova-yolo-1.0.8/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/engine/results.py` & `actnova-yolo-1.0.8/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/engine/trainer.py` & `actnova-yolo-1.0.8/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/engine/validator.py` & `actnova-yolo-1.0.8/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/hub/__init__.py` & `actnova-yolo-1.0.8/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/hub/auth.py` & `actnova-yolo-1.0.8/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/hub/session.py` & `actnova-yolo-1.0.8/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/hub/utils.py` & `actnova-yolo-1.0.8/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/fastsam/model.py` & `actnova-yolo-1.0.8/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/fastsam/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/fastsam/prompt.py` & `actnova-yolo-1.0.8/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/fastsam/utils.py` & `actnova-yolo-1.0.8/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/fastsam/val.py` & `actnova-yolo-1.0.8/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/nas/model.py` & `actnova-yolo-1.0.8/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/nas/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/nas/val.py` & `actnova-yolo-1.0.8/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/rtdetr/model.py` & `actnova-yolo-1.0.8/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/rtdetr/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/rtdetr/train.py` & `actnova-yolo-1.0.8/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/rtdetr/val.py` & `actnova-yolo-1.0.8/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/amg.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/build.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/model.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/modules/decoders.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/modules/encoders.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/modules/sam.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/modules/tiny_encoder.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/modules/transformer.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/sam/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/utils/loss.py` & `actnova-yolo-1.0.8/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/utils/ops.py` & `actnova-yolo-1.0.8/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/train.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/actnova/val.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/actnova/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/classify/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/classify/train.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/classify/val.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/detect/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/detect/train.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/detect/val.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/pose/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/pose/train.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/pose/val.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/segment/predict.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/segment/train.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/models/yolo/segment/val.py` & `actnova-yolo-1.0.8/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/__init__.py` & `actnova-yolo-1.0.8/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/autobackend.py` & `actnova-yolo-1.0.8/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/modules/__init__.py` & `actnova-yolo-1.0.8/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/modules/block.py` & `actnova-yolo-1.0.8/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/modules/conv.py` & `actnova-yolo-1.0.8/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/modules/head.py` & `actnova-yolo-1.0.8/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/modules/transformer.py` & `actnova-yolo-1.0.8/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/modules/utils.py` & `actnova-yolo-1.0.8/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/nn/tasks.py` & `actnova-yolo-1.0.8/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/basetrack.py` & `actnova-yolo-1.0.8/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/bot_sort.py` & `actnova-yolo-1.0.8/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/byte_tracker.py` & `actnova-yolo-1.0.8/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/track.py` & `actnova-yolo-1.0.8/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/utils/gmc.py` & `actnova-yolo-1.0.8/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/utils/kalman_filter.py` & `actnova-yolo-1.0.8/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/trackers/utils/matching.py` & `actnova-yolo-1.0.8/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/__init__.py` & `actnova-yolo-1.0.8/ultralytics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/autobatch.py` & `actnova-yolo-1.0.8/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/benchmarks.py` & `actnova-yolo-1.0.8/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/base.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/clearml.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/comet.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/dvc.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/hub.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/mlflow.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/neptune.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/raytune.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/tensorboard.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/callbacks/wb.py` & `actnova-yolo-1.0.8/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/checks.py` & `actnova-yolo-1.0.8/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/dist.py` & `actnova-yolo-1.0.8/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/downloads.py` & `actnova-yolo-1.0.8/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/files.py` & `actnova-yolo-1.0.8/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/instance.py` & `actnova-yolo-1.0.8/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/loss.py` & `actnova-yolo-1.0.8/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/metrics.py` & `actnova-yolo-1.0.8/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/ops.py` & `actnova-yolo-1.0.8/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/patches.py` & `actnova-yolo-1.0.8/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/plotting.py` & `actnova-yolo-1.0.8/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/tal.py` & `actnova-yolo-1.0.8/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/torch_utils.py` & `actnova-yolo-1.0.8/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/utils/tuner.py` & `actnova-yolo-1.0.8/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/yolo/data/__init__.py` & `actnova-yolo-1.0.8/ultralytics/yolo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.7/ultralytics/yolo/utils/__init__.py` & `actnova-yolo-1.0.8/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

