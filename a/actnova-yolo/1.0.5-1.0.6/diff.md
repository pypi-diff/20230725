# Comparing `tmp/actnova-yolo-1.0.5.tar.gz` & `tmp/actnova-yolo-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actnova-yolo-1.0.5.tar", last modified: Tue Jul 25 08:48:05 2023, max compression
+gzip compressed data, was "actnova-yolo-1.0.6.tar", last modified: Tue Jul 25 09:18:39 2023, max compression
```

## Comparing `actnova-yolo-1.0.5.tar` & `actnova-yolo-1.0.6.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.949215 actnova-yolo-1.0.5/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5625 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/CONTRIBUTING.md
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    34523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/LICENSE
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      213 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/MANIFEST.in
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26780 2023-07-25 08:48:05.949424 actnova-yolo-1.0.5/PKG-INFO
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    25155 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/README.md
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24156 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/README.zh-CN.md
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.909249 actnova-yolo-1.0.5/actnova_yolo.egg-info/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26780 2023-07-25 08:48:05.000000 actnova-yolo-1.0.5/actnova_yolo.egg-info/PKG-INFO
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6102 2023-07-25 08:48:05.000000 actnova-yolo-1.0.5/actnova_yolo.egg-info/SOURCES.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        1 2023-07-25 08:48:05.000000 actnova-yolo-1.0.5/actnova_yolo.egg-info/dependency_links.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       93 2023-07-25 08:48:05.000000 actnova-yolo-1.0.5/actnova_yolo.egg-info/entry_points.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      394 2023-07-25 08:48:05.000000 actnova-yolo-1.0.5/actnova_yolo.egg-info/requires.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       12 2023-07-25 08:48:05.000000 actnova-yolo-1.0.5/actnova_yolo.egg-info/top_level.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/requirements.txt
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      682 2023-07-25 08:48:05.950220 actnova-yolo-1.0.5/setup.cfg
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3110 2023-07-25 08:29:02.000000 actnova-yolo-1.0.5/setup.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.909952 actnova-yolo-1.0.5/tests/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/tests/test_cli.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4344 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/tests/test_engine.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7216 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/tests/test_python.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.910148 actnova-yolo-1.0.5/ultralytics/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      564 2023-07-25 08:48:03.000000 actnova-yolo-1.0.5/ultralytics/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.911179 actnova-yolo-1.0.5/ultralytics/assets/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)   137419 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/assets/bus.jpg
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    50427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.911867 actnova-yolo-1.0.5/ultralytics/cfg/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18735 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.915262 actnova-yolo-1.0.5/ultralytics/cfg/datasets/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2746 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1981 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9255 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3507 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3007 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1542 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1862 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1846 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      895 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1777 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7173 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.903095 actnova-yolo-1.0.5/ultralytics/cfg/models/
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.915654 actnova-yolo-1.0.5/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1970 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2177 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.916412 actnova-yolo-1.0.5/ultralytics/cfg/models/v3/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1537 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.917071 actnova-yolo-1.0.5/ultralytics/cfg/models/v5/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1923 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.917318 actnova-yolo-1.0.5/ultralytics/cfg/models/v6/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1735 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.919215 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1946 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1580 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1490 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1913 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.919733 actnova-yolo-1.0.5/ultralytics/cfg/trackers/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      694 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.921990 actnova-yolo-1.0.5/ultralytics/data/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      389 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1830 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/annotator.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/augment.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12660 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/base.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6531 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/build.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9180 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/converter.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.922246 actnova-yolo-1.0.5/ultralytics/data/dataloaders/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/dataloaders/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13378 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/dataset.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/loaders.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    25868 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/data/utils.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.924006 actnova-yolo-1.0.5/ultralytics/engine/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/engine/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    44686 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/engine/exporter.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19444 2023-07-25 08:47:06.000000 actnova-yolo-1.0.5/ultralytics/engine/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16516 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/engine/predictor.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24667 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/engine/results.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    31186 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/engine/trainer.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11754 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/engine/validator.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.924895 actnova-yolo-1.0.5/ultralytics/hub/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4393 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/hub/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/hub/auth.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8469 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/hub/session.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9425 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/hub/utils.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.925099 actnova-yolo-1.0.5/ultralytics/models/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       99 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.926392 actnova-yolo-1.0.5/ultralytics/models/fastsam/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      254 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4557 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/fastsam/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16752 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1986 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12414 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.927274 actnova-yolo-1.0.5/ultralytics/models/nas/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      179 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/nas/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5206 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/nas/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1445 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/nas/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      947 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/nas/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.928378 actnova-yolo-1.0.5/ultralytics/models/rtdetr/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      197 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7384 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2949 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6561 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.929475 actnova-yolo-1.0.5/ultralytics/models/sam/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      176 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13296 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/amg.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4822 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/build.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2522 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/model.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.931193 actnova-yolo-1.0.5/ultralytics/models/sam/modules/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6372 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    22545 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7309 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    21760 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8532 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18948 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.931803 actnova-yolo-1.0.5/ultralytics/models/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/utils/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13157 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/utils/loss.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12990 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.932028 actnova-yolo-1.0.5/ultralytics/models/yolo/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      182 2023-07-25 08:33:18.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.933318 actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      264 2023-07-25 08:46:18.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2375 2023-07-25 08:46:08.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2809 2023-07-25 08:46:07.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10917 2023-07-25 08:46:05.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.934412 actnova-yolo-1.0.5/ultralytics/models/yolo/classify/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1914 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4651 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.935258 actnova-yolo-1.0.5/ultralytics/models/yolo/detect/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      277 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5780 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/detect/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.936093 actnova-yolo-1.0.5/ultralytics/models/yolo/pose/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      247 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2369 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2788 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10911 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.937126 actnova-yolo-1.0.5/ultralytics/models/yolo/segment/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      295 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2833 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2497 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.937878 actnova-yolo-1.0.5/ultralytics/nn/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      586 2023-07-25 06:35:22.000000 actnova-yolo-1.0.5/ultralytics/nn/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26042 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.939262 actnova-yolo-1.0.5/ultralytics/nn/modules/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1587 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11841 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/modules/block.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/modules/conv.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16098 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/modules/head.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    15934 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3244 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/nn/modules/utils.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37028 2023-07-25 06:25:22.000000 actnova-yolo-1.0.5/ultralytics/nn/tasks.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.940371 actnova-yolo-1.0.5/ultralytics/trackers/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      227 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1609 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/basetrack.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5681 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14446 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2324 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/track.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.941172 actnova-yolo-1.0.5/ultralytics/trackers/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12209 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18420 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8749 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.945306 actnova-yolo-1.0.5/ultralytics/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    30200 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3864 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/autobatch.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16087 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.947626 actnova-yolo-1.0.5/ultralytics/utils/callbacks/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      214 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5593 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5974 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13115 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4386 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3363 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2701 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      608 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1716 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19224 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/checks.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2591 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/dist.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12818 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/downloads.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      312 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/errors.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5450 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/files.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/instance.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19144 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/loss.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42325 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/metrics.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    29212 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/ops.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1246 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/patches.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24845 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/plotting.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/tal.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)    23082 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/torch_utils.py
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/utils/tuner.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.947869 actnova-yolo-1.0.5/ultralytics/yolo/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)       94 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.948118 actnova-yolo-1.0.5/ultralytics/yolo/cfg/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      373 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/yolo/cfg/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.948377 actnova-yolo-1.0.5/ultralytics/yolo/data/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      823 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/yolo/data/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.948608 actnova-yolo-1.0.5/ultralytics/yolo/engine/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      385 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/yolo/engine/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.948820 actnova-yolo-1.0.5/ultralytics/yolo/utils/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/yolo/utils/__init__.py
-drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 08:48:05.949037 actnova-yolo-1.0.5/ultralytics/yolo/v8/
--rw-r--r--   0 dongyoonhahm   (501) staff       (20)      387 2023-07-25 05:23:34.000000 actnova-yolo-1.0.5/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.004945 actnova-yolo-1.0.6/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5625 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/CONTRIBUTING.md
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    34523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/LICENSE
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      213 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/MANIFEST.in
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26768 2023-07-25 09:18:39.005314 actnova-yolo-1.0.6/PKG-INFO
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    25155 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/README.md
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24156 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/README.zh-CN.md
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.962008 actnova-yolo-1.0.6/actnova_yolo.egg-info/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26768 2023-07-25 09:18:38.000000 actnova-yolo-1.0.6/actnova_yolo.egg-info/PKG-INFO
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6102 2023-07-25 09:18:38.000000 actnova-yolo-1.0.6/actnova_yolo.egg-info/SOURCES.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        1 2023-07-25 09:18:38.000000 actnova-yolo-1.0.6/actnova_yolo.egg-info/dependency_links.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       93 2023-07-25 09:18:38.000000 actnova-yolo-1.0.6/actnova_yolo.egg-info/entry_points.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      394 2023-07-25 09:18:38.000000 actnova-yolo-1.0.6/actnova_yolo.egg-info/requires.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       12 2023-07-25 09:18:38.000000 actnova-yolo-1.0.6/actnova_yolo.egg-info/top_level.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/requirements.txt
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      682 2023-07-25 09:18:39.006123 actnova-yolo-1.0.6/setup.cfg
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3098 2023-07-25 09:16:57.000000 actnova-yolo-1.0.6/setup.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.962723 actnova-yolo-1.0.6/tests/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/tests/test_cli.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4344 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/tests/test_engine.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7216 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/tests/test_python.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.963021 actnova-yolo-1.0.6/ultralytics/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      564 2023-07-25 09:17:51.000000 actnova-yolo-1.0.6/ultralytics/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.964144 actnova-yolo-1.0.6/ultralytics/assets/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)   137419 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/assets/bus.jpg
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    50427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.964759 actnova-yolo-1.0.6/ultralytics/cfg/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18847 2023-07-25 09:03:15.000000 actnova-yolo-1.0.6/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.968178 actnova-yolo-1.0.6/ultralytics/cfg/datasets/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2746 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1981 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9255 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2427 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3507 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3007 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1542 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1862 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1846 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      895 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1777 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5153 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7173 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.955214 actnova-yolo-1.0.6/ultralytics/cfg/models/
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.968605 actnova-yolo-1.0.6/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1970 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2177 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.969224 actnova-yolo-1.0.6/ultralytics/cfg/models/v3/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1537 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.969646 actnova-yolo-1.0.6/ultralytics/cfg/models/v5/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1923 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1550 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.969839 actnova-yolo-1.0.6/ultralytics/cfg/models/v6/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1735 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.971487 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1946 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1580 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1920 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1490 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1913 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.971909 actnova-yolo-1.0.6/ultralytics/cfg/trackers/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      694 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.974605 actnova-yolo-1.0.6/ultralytics/data/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      389 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1830 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/annotator.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37439 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/augment.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12660 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/base.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6531 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/build.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9180 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/converter.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.974892 actnova-yolo-1.0.6/ultralytics/data/dataloaders/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/dataloaders/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13378 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/dataset.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16523 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/loaders.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    25868 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/data/utils.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.976771 actnova-yolo-1.0.6/ultralytics/engine/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/engine/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    44686 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/engine/exporter.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19444 2023-07-25 09:06:02.000000 actnova-yolo-1.0.6/ultralytics/engine/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16516 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/engine/predictor.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24667 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/engine/results.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    31186 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/engine/trainer.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11754 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/engine/validator.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.977753 actnova-yolo-1.0.6/ultralytics/hub/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4393 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/hub/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5193 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/hub/auth.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8469 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/hub/session.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     9425 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/hub/utils.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.977955 actnova-yolo-1.0.6/ultralytics/models/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       99 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.979273 actnova-yolo-1.0.6/ultralytics/models/fastsam/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      254 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4557 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2797 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16752 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1986 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12414 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.980108 actnova-yolo-1.0.6/ultralytics/models/nas/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      179 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5206 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/nas/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1445 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/nas/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      947 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/nas/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.981182 actnova-yolo-1.0.6/ultralytics/models/rtdetr/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      197 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7384 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2949 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6561 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.982153 actnova-yolo-1.0.6/ultralytics/models/sam/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      176 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13296 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/amg.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4822 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/build.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2522 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/model.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.983923 actnova-yolo-1.0.6/ultralytics/models/sam/modules/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6372 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    22545 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     7309 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    21760 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8532 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18948 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.984562 actnova-yolo-1.0.6/ultralytics/models/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       42 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13157 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/utils/loss.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12990 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.984774 actnova-yolo-1.0.6/ultralytics/models/yolo/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      182 2023-07-25 09:06:47.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.985919 actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      264 2023-07-25 08:46:18.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2375 2023-07-25 08:46:08.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2809 2023-07-25 08:46:07.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10917 2023-07-25 08:46:05.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.986912 actnova-yolo-1.0.6/ultralytics/models/yolo/classify/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1914 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     6856 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4651 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.987803 actnova-yolo-1.0.6/ultralytics/models/yolo/detect/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      277 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1839 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5780 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13521 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/detect/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.988725 actnova-yolo-1.0.6/ultralytics/models/yolo/pose/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      247 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2369 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2788 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    10911 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.989730 actnova-yolo-1.0.6/ultralytics/models/yolo/segment/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      295 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2833 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2497 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12890 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.990471 actnova-yolo-1.0.6/ultralytics/nn/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      586 2023-07-25 06:35:22.000000 actnova-yolo-1.0.6/ultralytics/nn/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    26042 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.992128 actnova-yolo-1.0.6/ultralytics/nn/modules/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1587 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11841 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/modules/block.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    11647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16098 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/modules/head.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    15934 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3244 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    37093 2023-07-25 09:00:06.000000 actnova-yolo-1.0.6/ultralytics/nn/tasks.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.993596 actnova-yolo-1.0.6/ultralytics/trackers/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      227 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1609 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5681 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14446 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2324 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/track.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:38.994575 actnova-yolo-1.0.6/ultralytics/trackers/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12209 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    18420 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     8749 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.000260 actnova-yolo-1.0.6/ultralytics/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    30200 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3864 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/autobatch.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    16087 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.002898 actnova-yolo-1.0.6/ultralytics/utils/callbacks/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      214 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5593 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5974 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13115 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     4386 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3363 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2701 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     3751 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      608 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1716 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2252 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19224 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/checks.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     2591 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/dist.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    12818 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/downloads.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      312 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/errors.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5450 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/files.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    14645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/instance.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    19144 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/loss.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    42325 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/metrics.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    29212 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/ops.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     1246 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/patches.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    24845 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/plotting.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    13645 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/tal.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)    23082 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)     5403 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/utils/tuner.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.003222 actnova-yolo-1.0.6/ultralytics/yolo/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)       94 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.003586 actnova-yolo-1.0.6/ultralytics/yolo/cfg/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      373 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/yolo/cfg/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.003891 actnova-yolo-1.0.6/ultralytics/yolo/data/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      823 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/yolo/data/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.004161 actnova-yolo-1.0.6/ultralytics/yolo/engine/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      385 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/yolo/engine/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.004420 actnova-yolo-1.0.6/ultralytics/yolo/utils/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      647 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/yolo/utils/__init__.py
+drwxr-xr-x   0 dongyoonhahm   (501) staff       (20)        0 2023-07-25 09:18:39.004635 actnova-yolo-1.0.6/ultralytics/yolo/v8/
+-rw-r--r--   0 dongyoonhahm   (501) staff       (20)      387 2023-07-25 05:23:34.000000 actnova-yolo-1.0.6/ultralytics/yolo/v8/__init__.py
```

### Comparing `actnova-yolo-1.0.5/CONTRIBUTING.md` & `actnova-yolo-1.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/LICENSE` & `actnova-yolo-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/PKG-INFO` & `actnova-yolo-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: actnova-yolo
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification. modified for Actnova by HahmDY
 Home-page: https://github.com/HahmActnova/actnova_yolo
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
-Project-URL: Source, https://github.com/HahmActnova/actnova_yolo/ultralytics
+Project-URL: Source, https://github.com/HahmActnova/actnova_yolo
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.5 Summary: Ultralytics
+Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.6 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. modified for Actnova by HahmDY Home-
 page: https://github.com/HahmActnova/actnova_yolo Author: Ultralytics Author-
 email: hello@ultralytics.com License: AGPL-3.0 Project-URL: Bug Reports, https:
 //github.com/ultralytics/ultralytics/issues Project-URL: Source, https://
-github.com/HahmActnova/actnova_yolo/ultralytics Keywords: machine-
-learning,deep-
+github.com/HahmActnova/actnova_yolo Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `actnova-yolo-1.0.5/README.md` & `actnova-yolo-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/README.zh-CN.md` & `actnova-yolo-1.0.6/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/actnova_yolo.egg-info/PKG-INFO` & `actnova-yolo-1.0.6/actnova_yolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: actnova-yolo
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification. modified for Actnova by HahmDY
 Home-page: https://github.com/HahmActnova/actnova_yolo
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
-Project-URL: Source, https://github.com/HahmActnova/actnova_yolo/ultralytics
+Project-URL: Source, https://github.com/HahmActnova/actnova_yolo
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.5 Summary: Ultralytics
+Metadata-Version: 2.1 Name: actnova-yolo Version: 1.0.6 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. modified for Actnova by HahmDY Home-
 page: https://github.com/HahmActnova/actnova_yolo Author: Ultralytics Author-
 email: hello@ultralytics.com License: AGPL-3.0 Project-URL: Bug Reports, https:
 //github.com/ultralytics/ultralytics/issues Project-URL: Source, https://
-github.com/HahmActnova/actnova_yolo/ultralytics Keywords: machine-
-learning,deep-
+github.com/HahmActnova/actnova_yolo Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `actnova-yolo-1.0.5/actnova_yolo.egg-info/SOURCES.txt` & `actnova-yolo-1.0.6/actnova_yolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/requirements.txt` & `actnova-yolo-1.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/setup.cfg` & `actnova-yolo-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/setup.py` & `actnova-yolo-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     description=('Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, '
                  'pose estimation and image classification. modified for Actnova by HahmDY'),
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/HahmActnova/actnova_yolo',
     project_urls={
         'Bug Reports': 'https://github.com/ultralytics/ultralytics/issues',
-        'Source': 'https://github.com/HahmActnova/actnova_yolo/ultralytics'},
+        'Source': 'https://github.com/HahmActnova/actnova_yolo'},
     author='Ultralytics',
     author_email='hello@ultralytics.com',
     packages=find_packages(),  # required
     include_package_data=True,
     install_requires=REQUIREMENTS,
     extras_require={
         'dev': [
```

### Comparing `actnova-yolo-1.0.5/tests/test_cli.py` & `actnova-yolo-1.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/tests/test_engine.py` & `actnova-yolo-1.0.6/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/tests/test_python.py` & `actnova-yolo-1.0.6/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/__init__.py` & `actnova-yolo-1.0.6/ultralytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = '1.0.5'
+__version__ = '1.0.6'
 
 from ultralytics.engine.model import YOLO
 from ultralytics.hub import start
 from ultralytics.models import RTDETR, SAM
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import SETTINGS as settings
```

### Comparing `actnova-yolo-1.0.5/ultralytics/assets/bus.jpg` & `actnova-yolo-1.0.6/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/assets/zidane.jpg` & `actnova-yolo-1.0.6/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/__init__.py` & `actnova-yolo-1.0.6/ultralytics/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 
 from ultralytics.utils import (DEFAULT_CFG, DEFAULT_CFG_DICT, DEFAULT_CFG_PATH, LOGGER, ROOT, SETTINGS, SETTINGS_YAML,
                                IterableSimpleNamespace, __version__, checks, colorstr, deprecation_warn, yaml_load,
                                yaml_print)
 
 # Define valid tasks and modes
 MODES = 'train', 'val', 'predict', 'export', 'track', 'benchmark'
-TASKS = 'detect', 'segment', 'classify', 'pose'
-TASK2DATA = {'detect': 'coco8.yaml', 'segment': 'coco8-seg.yaml', 'classify': 'imagenet100', 'pose': 'coco8-pose.yaml'}
+TASKS = 'detect', 'segment', 'classify', 'pose', 'actnova'
+TASK2DATA = {'detect': 'coco8.yaml', 'segment': 'coco8-seg.yaml', 'classify': 'imagenet100', 'pose': 'coco8-pose.yaml','actnova': 'coco8-pose.yaml'}
 TASK2MODEL = {
     'detect': 'yolov8n.pt',
     'segment': 'yolov8n-seg.pt',
     'classify': 'yolov8n-cls.pt',
-    'pose': 'yolov8n-pose.pt'}
+    'pose': 'yolov8n-pose.pt',
+    'actnova': 'yolov8n-pose.pt'}
 TASK2METRIC = {
     'detect': 'metrics/mAP50-95(B)',
     'segment': 'metrics/mAP50-95(M)',
     'classify': 'metrics/accuracy_top1',
-    'pose': 'metrics/mAP50-95(P)'}
+    'pose': 'metrics/mAP50-95(P)',
+    'actnova': 'metrics/mAP50-95(P)'}
 
 CLI_HELP_MSG = \
     f"""
     Arguments received: {str(['yolo'] + sys.argv[1:])}. Ultralytics 'yolo' commands use the following syntax:
 
         yolo TASK MODE ARGS
```

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/Argoverse.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/ImageNet.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/Objects365.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/SKU-110K.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/VOC.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/VisDrone.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco-pose.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco128-seg.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco128.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco8-pose.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco8-seg.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/coco8.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/datasets/xView.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/default.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v3/yolov3.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v5/yolov5.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v6/yolov6.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/models/v8/yolov8.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/trackers/botsort.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/cfg/trackers/bytetrack.yaml` & `actnova-yolo-1.0.6/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/annotator.py` & `actnova-yolo-1.0.6/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/augment.py` & `actnova-yolo-1.0.6/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/base.py` & `actnova-yolo-1.0.6/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/build.py` & `actnova-yolo-1.0.6/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/converter.py` & `actnova-yolo-1.0.6/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/dataset.py` & `actnova-yolo-1.0.6/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/loaders.py` & `actnova-yolo-1.0.6/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/data/utils.py` & `actnova-yolo-1.0.6/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/engine/exporter.py` & `actnova-yolo-1.0.6/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/engine/model.py` & `actnova-yolo-1.0.6/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/engine/predictor.py` & `actnova-yolo-1.0.6/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/engine/results.py` & `actnova-yolo-1.0.6/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/engine/trainer.py` & `actnova-yolo-1.0.6/ultralytics/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/engine/validator.py` & `actnova-yolo-1.0.6/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/hub/__init__.py` & `actnova-yolo-1.0.6/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/hub/auth.py` & `actnova-yolo-1.0.6/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/hub/session.py` & `actnova-yolo-1.0.6/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/hub/utils.py` & `actnova-yolo-1.0.6/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/fastsam/model.py` & `actnova-yolo-1.0.6/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/fastsam/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/fastsam/prompt.py` & `actnova-yolo-1.0.6/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/fastsam/utils.py` & `actnova-yolo-1.0.6/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/fastsam/val.py` & `actnova-yolo-1.0.6/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/nas/model.py` & `actnova-yolo-1.0.6/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/nas/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/nas/val.py` & `actnova-yolo-1.0.6/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/rtdetr/model.py` & `actnova-yolo-1.0.6/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/rtdetr/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/rtdetr/train.py` & `actnova-yolo-1.0.6/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/rtdetr/val.py` & `actnova-yolo-1.0.6/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/amg.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/build.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/model.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/modules/decoders.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/modules/encoders.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/modules/sam.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/modules/tiny_encoder.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/modules/transformer.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/sam/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/utils/loss.py` & `actnova-yolo-1.0.6/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/utils/ops.py` & `actnova-yolo-1.0.6/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/train.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/actnova/val.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/actnova/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/classify/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/classify/train.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/classify/val.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/detect/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/detect/train.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/detect/val.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/pose/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/pose/train.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/pose/val.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/segment/predict.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/segment/train.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/models/yolo/segment/val.py` & `actnova-yolo-1.0.6/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/__init__.py` & `actnova-yolo-1.0.6/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/autobackend.py` & `actnova-yolo-1.0.6/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/modules/__init__.py` & `actnova-yolo-1.0.6/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/modules/block.py` & `actnova-yolo-1.0.6/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/modules/conv.py` & `actnova-yolo-1.0.6/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/modules/head.py` & `actnova-yolo-1.0.6/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/modules/transformer.py` & `actnova-yolo-1.0.6/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/modules/utils.py` & `actnova-yolo-1.0.6/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/nn/tasks.py` & `actnova-yolo-1.0.6/ultralytics/nn/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -801,14 +801,17 @@
             return 'classify'
         if m == 'detect':
             return 'detect'
         if m == 'segment':
             return 'segment'
         if m == 'pose':
             return 'pose'
+        if m == 'actnova':
+            return 'actnova'
+        
 
     # Guess from model cfg
     if isinstance(model, dict):
         with contextlib.suppress(Exception):
             return cfg2task(model)
 
     # Guess from PyTorch model
```

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/basetrack.py` & `actnova-yolo-1.0.6/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/bot_sort.py` & `actnova-yolo-1.0.6/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/byte_tracker.py` & `actnova-yolo-1.0.6/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/track.py` & `actnova-yolo-1.0.6/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/utils/gmc.py` & `actnova-yolo-1.0.6/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/utils/kalman_filter.py` & `actnova-yolo-1.0.6/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/trackers/utils/matching.py` & `actnova-yolo-1.0.6/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/__init__.py` & `actnova-yolo-1.0.6/ultralytics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/autobatch.py` & `actnova-yolo-1.0.6/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/benchmarks.py` & `actnova-yolo-1.0.6/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/base.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/clearml.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/comet.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/dvc.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/hub.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/mlflow.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/neptune.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/raytune.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/tensorboard.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/callbacks/wb.py` & `actnova-yolo-1.0.6/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/checks.py` & `actnova-yolo-1.0.6/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/dist.py` & `actnova-yolo-1.0.6/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/downloads.py` & `actnova-yolo-1.0.6/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/files.py` & `actnova-yolo-1.0.6/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/instance.py` & `actnova-yolo-1.0.6/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/loss.py` & `actnova-yolo-1.0.6/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/metrics.py` & `actnova-yolo-1.0.6/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/ops.py` & `actnova-yolo-1.0.6/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/patches.py` & `actnova-yolo-1.0.6/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/plotting.py` & `actnova-yolo-1.0.6/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/tal.py` & `actnova-yolo-1.0.6/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/torch_utils.py` & `actnova-yolo-1.0.6/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/utils/tuner.py` & `actnova-yolo-1.0.6/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/yolo/data/__init__.py` & `actnova-yolo-1.0.6/ultralytics/yolo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `actnova-yolo-1.0.5/ultralytics/yolo/utils/__init__.py` & `actnova-yolo-1.0.6/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

