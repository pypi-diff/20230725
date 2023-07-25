# Comparing `tmp/aac-metrics-0.4.2.tar.gz` & `tmp/aac-metrics-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aac-metrics-0.4.2.tar", last modified: Wed Apr 19 15:14:38 2023, max compression
+gzip compressed data, was "aac-metrics-0.4.3.tar", last modified: Tue Jul 25 16:55:38 2023, max compression
```

## Comparing `aac-metrics-0.4.2.tar` & `aac-metrics-0.4.3.tar`

### file list

```diff
@@ -1,106 +1,102 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.317355 aac-metrics-0.4.2/.github/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/.github/workflows/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1958 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/.github/workflows/python-package-pip.yaml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.2/LICENCE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      147 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/MANIFEST.in
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12241 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11103 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/README.md
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/data/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/data/example_1.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/data/example_2.csv
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/examples/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2023-04-19 15:13:33.000000 aac-metrics-0.4.2/examples/example_1.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2023-04-19 15:13:33.000000 aac-metrics-0.4.2/examples/example_2.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-04-19 15:13:33.000000 aac-metrics-0.4.2/install_spice.sh
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1954 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/src/aac_metrics/__main__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics/classes/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2023-03-16 14:40:20.000000 aac-metrics-0.4.2/src/aac_metrics/classes/base.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/fluerr.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/classes/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/sbert_sim.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spider_fl.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/classes/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7642 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7466 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/evaluate.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9592 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9590 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/fluerr.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/mult_cands.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/sbert_sim.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spider_fl.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.2/src/aac_metrics/functional/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/src/aac_metrics/info.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1559 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/install_spice.sh
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/src/aac_metrics/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.2/src/aac_metrics/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3807 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/src/aac_metrics/utils/checks.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.2/src/aac_metrics/utils/collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.2/src/aac_metrics/utils/imports.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7678 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/src/aac_metrics/utils/tokenization.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.325355 aac-metrics-0.4.2/src/aac_metrics.egg-info/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12241 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4122 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-04-19 15:14:38.000000 aac-metrics-0.4.2/src/aac_metrics.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.329355 aac-metrics-0.4.2/tests/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-19 15:14:38.321355 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.2/tests/caption-evaluation-tools/eval_metrics.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/tests/test_bleu_tchmet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4271 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/tests/test_compare_cet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3886 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/tests/test_compare_fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.2/tests/test_pickable.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1763 2023-04-19 15:13:37.000000 aac-metrics-0.4.2/tests/test_utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.464243 aac-metrics-0.4.3/.github/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.464243 aac-metrics-0.4.3/.github/workflows/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2106 2023-07-21 17:28:20.000000 aac-metrics-0.4.3/.github/workflows/python-package-pip.yaml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.3/LICENCE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      147 2023-04-19 15:13:37.000000 aac-metrics-0.4.3/MANIFEST.in
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11925 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10787 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/README.md
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/data/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2023-04-19 15:13:37.000000 aac-metrics-0.4.3/data/example_1.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2023-04-19 15:13:37.000000 aac-metrics-0.4.3/data/example_2.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1980 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.3/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.464243 aac-metrics-0.4.3/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/src/aac_metrics/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.3/src/aac_metrics/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/src/aac_metrics/classes/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1013 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/base.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/classes/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7642 2023-04-19 15:13:37.000000 aac-metrics-0.4.3/src/aac_metrics/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7550 2023-06-15 09:01:14.000000 aac-metrics-0.4.3/src/aac_metrics/evaluate.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/src/aac_metrics/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/src/aac_metrics/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9699 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9553 2023-06-15 09:01:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/src/aac_metrics/functional/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/src/aac_metrics/functional/mult_cands.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/src/aac_metrics/functional/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/src/aac_metrics/functional/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/functional/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.3/src/aac_metrics/functional/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2023-07-25 16:55:14.000000 aac-metrics-0.4.3/src/aac_metrics/info.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1559 2023-04-19 15:13:37.000000 aac-metrics-0.4.3/src/aac_metrics/install_spice.sh
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/src/aac_metrics/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.3/src/aac_metrics/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3773 2023-06-15 09:01:14.000000 aac-metrics-0.4.3/src/aac_metrics/utils/checks.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.3/src/aac_metrics/utils/collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.3/src/aac_metrics/utils/imports.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7698 2023-06-15 09:01:14.000000 aac-metrics-0.4.3/src/aac_metrics/utils/tokenization.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/src/aac_metrics.egg-info/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11925 2023-07-25 16:55:38.000000 aac-metrics-0.4.3/src/aac_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4059 2023-07-25 16:55:38.000000 aac-metrics-0.4.3/src/aac_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-07-25 16:55:38.000000 aac-metrics-0.4.3/src/aac_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-07-25 16:55:38.000000 aac-metrics-0.4.3/src/aac_metrics.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      189 2023-07-25 16:55:38.000000 aac-metrics-0.4.3/src/aac_metrics.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-07-25 16:55:38.000000 aac-metrics-0.4.3/src/aac_metrics.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.476243 aac-metrics-0.4.3/tests/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.468243 aac-metrics-0.4.3/tests/caption-evaluation-tools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.468243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.468243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.468243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.468243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.468243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-07-25 16:55:38.472243 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocotools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.3/tests/caption-evaluation-tools/eval_metrics.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/tests/test_bleu_tchmet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4271 2023-05-23 13:08:54.000000 aac-metrics-0.4.3/tests/test_compare_cet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3886 2023-04-19 15:13:37.000000 aac-metrics-0.4.3/tests/test_compare_fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.3/tests/test_pickable.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1823 2023-06-15 09:01:14.000000 aac-metrics-0.4.3/tests/test_utils.py
```

### Comparing `aac-metrics-0.4.2/.github/workflows/python-package-pip.yaml` & `aac-metrics-0.4.3/.github/workflows/python-package-pip.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -22,40 +22,45 @@
     # --- INSTALLATIONS ---
     - name: Checkout repository
       uses: actions/checkout@v2
       with:
         submodules: recursive
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
   
     - name: Set up Java ${{ matrix.java-version }}
       uses: actions/setup-java@v2
       with:
         distribution: 'temurin'
         java-version: ${{ matrix.java-version }}
         java-package: jre
 
     - name: Install package
+      # note: ${GITHUB_REF##*/} gives the branch name
       run: |
-        python -m pip install "aac-metrics[dev] @ git+https://github.com/Labbeti/aac-metrics@dev"
+        python -m pip install "aac-metrics[dev] @ git+https://github.com/Labbeti/aac-metrics@${GITHUB_REF##*/}"
   
     - name: Load cache of external code and data
       uses: actions/cache@master
       id: cache_external
       with:
         path: /home/runner/.cache/aac-metrics/*
         key: ${{ runner.os }}-${{ hashFiles('src/aac_metrics/download.py') }}
         restore-keys: |
           ${{ runner.os }}-
 
     # --- TESTS ---
+    - name: Compile python files
+      run: |
+        python -m compileall src
+
     - name: Lint with flake8
       run: |
         python -m flake8 --config .flake8 --exit-zero --show-source --statistics src
 
     - name: Check format with Black
       run: |
         python -m black --check --diff src
```

### Comparing `aac-metrics-0.4.2/LICENCE` & `aac-metrics-0.4.3/LICENCE`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/PKG-INFO` & `aac-metrics-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.4.2
+Version: 0.4.3
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
-Project-URL: homepage, https://pypi.org/project/aac-metrics/
-Project-URL: documentation, https://aac-metrics.readthedocs.io/
-Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
-Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
+Project-URL: Homepage, https://pypi.org/project/aac-metrics/
+Project-URL: Documentation, https://aac-metrics.readthedocs.io/
+Project-URL: Repository, https://github.com//Labbeti/aac-metrics.git
+Project-URL: Changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
 Keywords: audio,metrics,text,captioning,audio-captioning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -158,18 +158,14 @@
 ## Additional notes
 ### CIDEr or CIDEr-D ?
 The CIDEr metric differs from CIDEr-D because it applies a stemmer to each word before computing the n-grams of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 
 ### Does metrics work on multi-GPU ?
 No. Most of these metrics use numpy or external java programs to run, which prevents multi-GPU testing for now.
 
-### Is torchmetrics needed for this package ?
-No. But if torchmetrics is installed, all metrics classes will inherit from the base class `torchmetrics.Metric`.
-It is because most of the metrics does not use PyTorch tensors to compute scores and numpy and strings cannot be added to states of `torchmetrics.Metric`.
-
 ## SPIDEr-max metric
 SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model. For more detail, please see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/stable/spider_max.html).
 
 ## References
 #### BLEU
 [1] K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, “BLEU: a
 method for automatic evaluation of machine translation,” in Proceed-
@@ -236,18 +232,18 @@
 
 If you use this software, please consider cite it as below :
 ```
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
-    month = {4},
+    month = {6},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.2},
+    version = {0.4.3},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.2 Summary: Metrics for
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.3 Summary: Metrics for
 evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
 email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
-pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
-Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
-repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
+pub@gmail.com> Project-URL: Homepage, https://pypi.org/project/aac-metrics/
+Project-URL: Documentation, https://aac-metrics.readthedocs.io/ Project-URL:
+Repository, https://github.com//Labbeti/aac-metrics.git Project-URL: Changelog,
 https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
 audio,metrics,text,captioning,audio-captioning Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -86,19 +86,15 @@
 specify a java executable path with `java_path` argument. - `unzip` command to
 extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
 CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
 before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
 reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
 audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 ### Does metrics work on multi-GPU ? No. Most of these metrics use numpy or
-external java programs to run, which prevents multi-GPU testing for now. ### Is
-torchmetrics needed for this package ? No. But if torchmetrics is installed,
-all metrics classes will inherit from the base class `torchmetrics.Metric`. It
-is because most of the metrics does not use PyTorch tensors to compute scores
-and numpy and strings cannot be added to states of `torchmetrics.Metric`. ##
+external java programs to run, which prevents multi-GPU testing for now. ##
 SPIDEr-max metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr
 that takes into account multiple candidates for the same audio. It computes the
 maximum of the SPIDEr scores for each candidate to balance the high sensitivity
 to the frequency of the words generated by the model. For more detail, please
 see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/
 stable/spider_max.html). ## References #### BLEU [1] K. Papineni, S. Roukos, T.
 Ward, and W.-J. Zhu, âBLEU: a method for automatic evaluation of machine
@@ -138,10 +134,10 @@
 Pellegrini, Thomas and Pinquier, Julien}, URL = {https://hal.archives-
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
-license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.2}, year = {2023}, } ``` ##
+license = {MIT}, month = {6}, title = {{aac-metrics}}, url = {https://
+github.com/Labbeti/aac-metrics/}, version = {0.4.3}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.2/README.md` & `aac-metrics-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -134,18 +134,14 @@
 ## Additional notes
 ### CIDEr or CIDEr-D ?
 The CIDEr metric differs from CIDEr-D because it applies a stemmer to each word before computing the n-grams of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 
 ### Does metrics work on multi-GPU ?
 No. Most of these metrics use numpy or external java programs to run, which prevents multi-GPU testing for now.
 
-### Is torchmetrics needed for this package ?
-No. But if torchmetrics is installed, all metrics classes will inherit from the base class `torchmetrics.Metric`.
-It is because most of the metrics does not use PyTorch tensors to compute scores and numpy and strings cannot be added to states of `torchmetrics.Metric`.
-
 ## SPIDEr-max metric
 SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model. For more detail, please see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/stable/spider_max.html).
 
 ## References
 #### BLEU
 [1] K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, “BLEU: a
 method for automatic evaluation of machine translation,” in Proceed-
@@ -212,18 +208,18 @@
 
 If you use this software, please consider cite it as below :
 ```
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
-    month = {4},
+    month = {6},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.2},
+    version = {0.4.3},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -70,19 +70,15 @@
 specify a java executable path with `java_path` argument. - `unzip` command to
 extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
 CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
 before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
 reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
 audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 ### Does metrics work on multi-GPU ? No. Most of these metrics use numpy or
-external java programs to run, which prevents multi-GPU testing for now. ### Is
-torchmetrics needed for this package ? No. But if torchmetrics is installed,
-all metrics classes will inherit from the base class `torchmetrics.Metric`. It
-is because most of the metrics does not use PyTorch tensors to compute scores
-and numpy and strings cannot be added to states of `torchmetrics.Metric`. ##
+external java programs to run, which prevents multi-GPU testing for now. ##
 SPIDEr-max metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr
 that takes into account multiple candidates for the same audio. It computes the
 maximum of the SPIDEr scores for each candidate to balance the high sensitivity
 to the frequency of the words generated by the model. For more detail, please
 see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/
 stable/spider_max.html). ## References #### BLEU [1] K. Papineni, S. Roukos, T.
 Ward, and W.-J. Zhu, âBLEU: a method for automatic evaluation of machine
@@ -122,10 +118,10 @@
 Pellegrini, Thomas and Pinquier, Julien}, URL = {https://hal.archives-
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
-license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.2}, year = {2023}, } ``` ##
+license = {MIT}, month = {6}, title = {{aac-metrics}}, url = {https://
+github.com/Labbeti/aac-metrics/}, version = {0.4.3}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.2/data/example_1.csv` & `aac-metrics-0.4.3/data/example_1.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/data/example_2.csv` & `aac-metrics-0.4.3/data/example_2.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/install_spice.sh` & `aac-metrics-0.4.3/src/aac_metrics/install_spice.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/bash
 
-DEFAULT_SPICE_ROOT="."
+DEFAULT_SPICE_ROOT="$HOME/.cache/aac-metrics/spice"
 
 if [ "$1" = "-h" ] || [ "$1" = "--help" ]; then
     echo "Install all files for running the java SPICE program in the SPICE_ROOT directory."
     echo "The default spice root path is \"${DEFAULT_SPICE_ROOT}\"."
     echo "Usage: $0 [SPICE_ROOT]"
     exit 0
 fi
```

### Comparing `aac-metrics-0.4.2/pyproject.toml` & `aac-metrics-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,33 @@
     "pyyaml>=6.0",
     "tqdm>=4.64.0",
     "sentence-transformers>=2.2.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "https://pypi.org/project/aac-metrics/"
-documentation = "https://aac-metrics.readthedocs.io/"
-repository = "https://github.com//Labbeti/aac-metrics.git"
-changelog = "https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md"
+Homepage = "https://pypi.org/project/aac-metrics/"
+Documentation = "https://aac-metrics.readthedocs.io/"
+Repository = "https://github.com//Labbeti/aac-metrics.git"
+Changelog = "https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md"
 
 [project.scripts]
 aac-metrics = "aac_metrics.__main__:_print_usage"
 aac-metrics-download = "aac_metrics.download:_main_download"
 aac-metrics-evaluate = "aac_metrics.evaluate:_main_evaluate"
 aac-metrics-info = "aac_metrics.info:print_install_info"
 
 [project.optional-dependencies]
 dev = [
     "pytest==7.1.2",
     "flake8==4.0.1",
     "black==22.8.0",
     "scikit-image==0.19.2",
     "matplotlib==3.5.2",
+    "torchmetrics>=0.10",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["aac_metrics*"]  # package names should match these glob patterns (["*"] by default)
 
 [tool.setuptools.dynamic]
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/__init__.py` & `aac-metrics-0.4.3/src/aac_metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __name__ = "aac-metrics"
 __author__ = "Etienne Labbé (Labbeti)"
 __author_email__ = "labbeti.pub@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "Etienne Labbé (Labbeti)"
 __status__ = "Development"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 
 from .classes.base import AACMetric
 from .classes.bleu import BLEU
 from .classes.cider_d import CIDErD
 from .classes.evaluate import AACEvaluate, _get_metric_factory_classes
 from .classes.fense import FENSE
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/__main__.py` & `aac-metrics-0.4.3/src/aac_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/__init__.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/base.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Any, Optional
 
-from aac_metrics.utils.imports import _TORCHMETRICS_AVAILABLE
+from torch import nn
 
 
-if _TORCHMETRICS_AVAILABLE:
-    from torchmetrics import Metric as __BaseMetric  # type: ignore
+class AACMetric(nn.Module):
+    """Base Metric module used when torchmetrics is not installed."""
 
-    class AACMetric(__BaseMetric):  # type: ignore
-        # The theorical minimal value of the main global score of the metric.
-        min_value: Optional[float] = None
-        # The theorical maximal value of the main global score of the metric.
-        max_value: Optional[float] = None
+    # Global values
+    full_state_update: Optional[bool] = False
+    higher_is_better: Optional[bool] = None
+    is_differentiable: Optional[bool] = False
 
-else:
-    from torch import nn
+    # The theorical minimal value of the main global score of the metric.
+    min_value: Optional[float] = None
+    # The theorical maximal value of the main global score of the metric.
+    max_value: Optional[float] = None
 
-    class AACMetric(nn.Module):
-        """Base Metric module used when torchmetrics is not installed."""
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
 
-        # Global values
-        full_state_update: Optional[bool] = False
-        higher_is_better: Optional[bool] = None
-        is_differentiable: Optional[bool] = False
+    # Public methods
+    def compute(self) -> Any:
+        return None
 
-        # The theorical minimal value of the main global score of the metric.
-        min_value: Optional[float] = None
-        # The theorical maximal value of the main global score of the metric.
-        max_value: Optional[float] = None
+    def forward(self, *args: Any, **kwargs: Any) -> Any:
+        self.update(*args, **kwargs)
+        output = self.compute()
+        self.reset()
+        return output
 
-        # Public methods
-        def compute(self) -> Any:
-            return None
+    def reset(self) -> None:
+        pass
 
-        def forward(self, *args: Any, **kwargs: Any) -> Any:
-            self.update(*args, **kwargs)
-            output = self.compute()
-            self.reset()
-            return output
-
-        def reset(self) -> None:
-            pass
-
-        def update(self, *args, **kwargs) -> None:
-            pass
+    def update(self, *args, **kwargs) -> None:
+        pass
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/bleu.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/cider_d.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/cider_d.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/evaluate.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from aac_metrics.classes.spider_fl import SPIDErFL
 from aac_metrics.functional.evaluate import METRICS_SETS, evaluate
 
 
 pylog = logging.getLogger(__name__)
 
 
-class Evaluate(AACMetric, list[AACMetric]):
+class Evaluate(list[AACMetric], AACMetric):
     """Evaluate candidates with multiple references with custom metrics.
 
     For more information, see :func:`~aac_metrics.functional.evaluate.evaluate`.
     """
 
     full_state_update = False
     higher_is_better = None
@@ -51,16 +51,16 @@
             cache_path,
             java_path,
             tmp_path,
             device,
             verbose,
         )
 
-        AACMetric.__init__(self)
         list.__init__(self, metrics)
+        AACMetric.__init__(self)
         self._preprocess = preprocess
         self._cache_path = cache_path
         self._java_path = java_path
         self._tmp_path = tmp_path
         self._device = device
         self._verbose = verbose
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/fense.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/fense.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             self._verbose,
         )
 
     def extra_repr(self) -> str:
         return f"error_threshold={self._error_threshold}, penalty={self._penalty}, device={self._device}, batch_size={self._batch_size}"
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("sbert.sim", "fluerr", "fense") + tuple(
+        return ("sbert_sim", "fluerr", "fense") + tuple(
             f"fluerr.{name}_prob" for name in ERROR_NAMES
         )
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/fluerr.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/fluerr.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/meteor.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/rouge_l.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/sbert_sim.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/sbert_sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             self._verbose,
         )
 
     def extra_repr(self) -> str:
         return f"device={self._device}, batch_size={self._batch_size}"
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("sbert.sim",)
+        return ("sbert_sim",)
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
 
     def update(
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/spice.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/spider.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/spider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/spider_fl.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/spider_fl.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/classes/spider_max.py` & `aac-metrics-0.4.3/src/aac_metrics/classes/spider_max.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/download.py` & `aac-metrics-0.4.3/src/aac_metrics/download.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/evaluate.py` & `aac-metrics-0.4.3/src/aac_metrics/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,22 +206,22 @@
     refs_lens = list(map(len, mult_references))
     if args.verbose >= 1:
         pylog.info(
             f"Found {len(candidates)} candidates, {len(mult_references)} references and [{min(refs_lens)}, {max(refs_lens)}] references per candidate."
         )
 
     corpus_scores, _sents_scores = evaluate(
-        candidates,
-        mult_references,
-        True,
-        args.metrics_set_name,
-        args.cache_path,
-        args.java_path,
-        args.tmp_path,
-        args.verbose,
+        candidates=candidates,
+        mult_references=mult_references,
+        preprocess=True,
+        metrics=args.metrics_set_name,
+        cache_path=args.cache_path,
+        java_path=args.java_path,
+        tmp_path=args.tmp_path,
+        verbose=args.verbose,
     )
 
     corpus_scores = {k: v.item() for k, v in corpus_scores.items()}
     pylog.info(f"Global scores:\n{yaml.dump(corpus_scores, sort_keys=False)}")
 
 
 if __name__ == "__main__":
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/__init__.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/bleu.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/bleu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import logging
 import math
 
 from collections import Counter
 from typing import Any, Callable, Optional, Union
 
 import torch
 
 from torch import Tensor
 
 
+pylog = logging.getLogger(__name__)
+
 BLEU_OPTIONS = ("shortest", "average", "closest")
 
 
 def bleu(
     candidates: list[str],
     mult_references: list[list[str]],
     return_all_scores: bool = True,
@@ -161,26 +164,26 @@
     needs to know about them."""
 
     reflen = []
     maxcounts = {}
     for ref in refs:
         rl, counts = __cook_sentence(ref, n, tokenizer)
         reflen.append(rl)
-        for (ngram, count) in counts.items():
+        for ngram, count in counts.items():
             maxcounts[ngram] = max(maxcounts.get(ngram, 0), count)
 
     # Calculate effective reference sentence length.
     if eff == "shortest":
         reflen = min(reflen)
     elif eff == "average":
         reflen = float(sum(reflen)) / len(reflen)
 
     # lhuang: N.B.: leave reflen computaiton to the very end!!
     # lhuang: N.B.: in case of "closest", keep a list of reflens!! (bad design)
-    return (reflen, maxcounts)
+    return reflen, maxcounts
 
 
 def __cook_candidate(
     test: str,
     reflen_refmaxcounts: tuple[Any, dict[tuple[str, ...], int]],
     eff: Optional[None],
     n: int,
@@ -199,15 +202,15 @@
     else:  # i.e., "average" or "shortest" or None
         result["reflen"] = reflen
 
     result["testlen"] = testlen
     result["guess"] = [max(0, testlen - k + 1) for k in range(1, n + 1)]
     result["correct"] = [0] * n
 
-    for (ngram, count) in counts.items():
+    for ngram, count in counts.items():
         result["correct"][len(ngram) - 1] += min(refmaxcounts.get(ngram, 0), count)
 
     return result
 
 
 def __compute_bleu_score(
     cooked_cands: list,
@@ -217,15 +220,18 @@
     verbose: int = 0,
 ) -> tuple[list[float], list[list[float]]]:
     SMALL = 1e-9
     TINY = 1e-15  # so that if guess is 0 still return 0
     bleu_list = [[] for _ in range(n)]
 
     if option is None:
-        option = "average" if len(cooked_mrefs) == 1 else "closest"
+        if len(cooked_mrefs) == 1:
+            option = "average"
+        else:
+            option = "closest"
 
     global_cands_len = 0
     global_mrefs_len = 0
     totalcomps = {"testlen": 0, "reflen": 0, "guess": [0] * n, "correct": [0] * n}
 
     # for each sentence
     for comps in cooked_cands:
@@ -250,16 +256,16 @@
 
         # N.B.: avoid zero division
         ratio = (testlen + TINY) / (reflen + SMALL)
         if ratio < 1:
             for k in range(n):
                 bleu_list[k][-1] *= math.exp(1 - 1 / ratio)
 
-        if verbose > 1:
-            print(comps, reflen)
+        if verbose > 2:
+            pylog.debug(comps, reflen)
 
     totalcomps["reflen"] = global_mrefs_len
     totalcomps["testlen"] = global_cands_len
 
     bleus = []
     bleu = 1.0
     for k in range(n):
@@ -270,17 +276,17 @@
     ratio = (global_cands_len + TINY) / (
         global_mrefs_len + SMALL
     )  # N.B.: avoid zero division
     if ratio < 1:
         for k in range(n):
             bleus[k] *= math.exp(1 - 1 / ratio)
 
-    if verbose > 0:
-        print(totalcomps)
-        print("ratio:", ratio)
+    if verbose > 2:
+        pylog.debug(totalcomps)
+        pylog.debug("ratio:", ratio)
 
     return bleus, bleu_list
 
 
 def __single_reflen(
     reflens: list[int],
     option: Optional[str] = None,
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/cider_d.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/cider_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     :param cnts:
     :return: tf-idf of n-grams (array of n dict[tuple, float]), norm (array of n floats) (norms for n-grams), length (int) (number of distinct n-grams from 1 to n)
     """
     vec = [defaultdict(float) for _ in range(n)]
     length = 0
     norm = np.zeros((n,))
 
-    for (ngram, term_freq) in counters.items():
+    for ngram, term_freq in counters.items():
         if isinstance(doc_frequencies, Mapping):
             count = doc_frequencies[ngram]
         else:
             count = doc_frequencies(ngram)
 
         # give ngram count 1 if it doesn't appear in reference corpus
         log_df = np.log(max(1.0, count))
@@ -229,15 +229,15 @@
     """
     delta = float(cand_len - ref_len)
     # measure consine similarity
     similarities = np.zeros((n,))
 
     for ni in range(n):
         # ngram
-        for (ngram, count) in cand_vec[ni].items():
+        for ngram, count in cand_vec[ni].items():
             # vrama91 : added clipping
             similarities[ni] += min(count, ref_vec[ni][ngram]) * ref_vec[ni][ngram]
 
         if (cand_norm[ni] != 0) and (ref_norm[ni] != 0):
             similarities[ni] /= cand_norm[ni] * ref_norm[ni]
 
         # vrama91: added a length based gaussian penalty
@@ -251,37 +251,32 @@
     cooked_mrefs: list[list[Counter]],
     doc_frequencies: Union[Counter[tuple], Callable[[tuple], int]],
     log_n_refs: float,
     n: int,
     sigma: float,
     scale: float,
 ) -> tuple[np.ndarray, list[tuple[list, list]]]:
-
     scores = np.empty((len(cooked_cands),))
     tfidf_lst = []
 
     for i, (cand, refs) in enumerate(zip(cooked_cands, cooked_mrefs)):
         # compute vector for test captions
         vec, norm, length = __counter_to_vec(cand, log_n_refs, n, doc_frequencies)
         # compute vector for ref captions
-        ngrams_scores = np.zeros((n,))
+        ngrams_scores = np.zeros((len(refs), n))
         vec_refs = []
-        for ref in refs:
+        for j, ref in enumerate(refs):
             vec_ref, norm_ref, length_ref = __counter_to_vec(
                 ref, log_n_refs, n, doc_frequencies
             )
             vec_refs.append(vec_ref)
-            ngrams_scores += __similarity(
+            ngrams_scores[j] = __similarity(
                 vec, vec_ref, norm, norm_ref, length, length_ref, n, sigma
             )
-        # change by vrama91 - mean of ngram scores, instead of sum
-        score_avg = np.mean(ngrams_scores)
-        # divide by number of references
-        score_avg /= len(refs)
-        # multiply score by 10
-        score_avg *= scale
-        # append score of an image to the score list
-        scores[i] = score_avg
 
+        # Use this weird mean calculation instead of ".mean()" because it can give slight differences compared to the original implementation
+        score_avg = ngrams_scores.sum(axis=0).mean() / len(refs)
+        scores[i] = score_avg
         tfidf_lst.append((vec, vec_refs))
 
+    scores = scores * scale
     return scores, tfidf_lst
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/evaluate.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/fense.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/fluerr.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/fluerr.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/meteor.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/mult_cands.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/mult_cands.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/rouge_l.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/sbert_sim.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/sbert_sim.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/spice.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/spider.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/spider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/spider_fl.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/spider_fl.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/functional/spider_max.py` & `aac-metrics-0.4.3/src/aac_metrics/functional/spider_max.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/info.py` & `aac-metrics-0.4.3/src/aac_metrics/info.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/utils/checks.py` & `aac-metrics-0.4.3/src/aac_metrics/utils/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import re
 import subprocess
 
-from dataclasses import dataclass
 from functools import cache
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Any, Union
 
 
 pylog = logging.getLogger(__name__)
 
 VERSION_PATTERN = r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+).*"
 MIN_JAVA_MAJOR_VERSION = 8
-MAX_JAVA_MAJOR_VERSION = 11
+MAX_JAVA_MAJOR_VERSION = 13
 
 
 def check_metric_inputs(
     candidates: Any,
     mult_references: Any,
 ) -> None:
     """Raises ValueError if candidates and mult_references does not have a valid type and size."""
@@ -50,14 +49,28 @@
         pylog.error(
             f"Using Java version {version} is not officially supported by aac-metrics package and will not work for METEOR and SPICE metrics."
             f"(expected major version in range [{MIN_JAVA_MAJOR_VERSION}, {MAX_JAVA_MAJOR_VERSION}])"
         )
     return valid
 
 
+def is_mono_sents(sents: Any) -> bool:
+    """Returns True if input is list[str]."""
+    return isinstance(sents, list) and all(isinstance(sent, str) for sent in sents)
+
+
+def is_mult_sents(mult_sents: Any) -> bool:
+    """Returns True if input is list[list[str]]."""
+    return (
+        isinstance(mult_sents, list)
+        and all(isinstance(sents, list) for sents in mult_sents)
+        and all(isinstance(sent, str) for sents in mult_sents for sent in sents)
+    )
+
+
 def _get_java_version(java_path: str) -> str:
     """Returns True if the java path is valid."""
     if not isinstance(java_path, str):
         raise TypeError(f"Invalid argument type {type(java_path)=}. (expected str)")
 
     output = "INVALID"
     try:
@@ -97,24 +110,10 @@
         major_version == 1 and minor_version <= 8
     ):  # java <= 8 use versioning "1.MAJOR.MINOR" and > 8 use "MAJOR.MINOR.PATCH"
         major_version = minor_version
 
     return min_major <= major_version <= max_major
 
 
-def is_mono_sents(sents: Any) -> bool:
-    """Returns True if input is list[str]."""
-    return isinstance(sents, list) and all(isinstance(sent, str) for sent in sents)
-
-
-def is_mult_sents(mult_sents: Any) -> bool:
-    """Returns True if input is list[list[str]]."""
-    return (
-        isinstance(mult_sents, list)
-        and all(isinstance(sents, list) for sents in mult_sents)
-        and all(isinstance(sent, str) for sents in mult_sents for sent in sents)
-    )
-
-
 @cache
 def _warn_once(msg: str) -> None:
     pylog.warning(msg)
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics/utils/collections.py` & `aac-metrics-0.4.3/src/aac_metrics/utils/collections.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/src/aac_metrics/utils/tokenization.py` & `aac-metrics-0.4.3/src/aac_metrics/utils/tokenization.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,24 +56,25 @@
 
     :param sentences: The sentences to tokenize.
     :param audio_ids: The optional audio names. None will use the audio index as name. defaults to None.
     :param cache_path: The path to the external directory containing the JAR program. defaults to "$HOME/.cache".
     :param java_path: The path to the java executable. defaults to "java".
     :param tmp_path: The path to a temporary directory. defaults to "/tmp".
     :param verbose: The verbose level. defaults to 0.
-    :returns: The sentences tokenized.
+    :returns: The sentences tokenized as list[list[str]].
     """
+    sentences = list(sentences)
+    if len(sentences) == 0:
+        return []
+
     cache_path = osp.expandvars(cache_path)
     java_path = osp.expandvars(java_path)
     tmp_path = osp.expandvars(tmp_path)
 
     # Based on https://github.com/audio-captioning/caption-evaluation-tools/blob/c1798df4c91e29fe689b1ccd4ce45439ec966417/caption/pycocoevalcap/tokenizer/ptbtokenizer.py#L30
-    sentences = list(sentences)
-    if len(sentences) == 0:
-        return []
 
     stanford_fpath = osp.join(cache_path, FNAME_STANFORD_CORENLP_3_4_1_JAR)
 
     # Sanity checks
     if __debug__:
         if not osp.isdir(cache_path):
             raise RuntimeError(f"Cannot find cache directory at {cache_path=}.")
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics.egg-info/PKG-INFO` & `aac-metrics-0.4.3/src/aac_metrics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.4.2
+Version: 0.4.3
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
-Project-URL: homepage, https://pypi.org/project/aac-metrics/
-Project-URL: documentation, https://aac-metrics.readthedocs.io/
-Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
-Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
+Project-URL: Homepage, https://pypi.org/project/aac-metrics/
+Project-URL: Documentation, https://aac-metrics.readthedocs.io/
+Project-URL: Repository, https://github.com//Labbeti/aac-metrics.git
+Project-URL: Changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
 Keywords: audio,metrics,text,captioning,audio-captioning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -158,18 +158,14 @@
 ## Additional notes
 ### CIDEr or CIDEr-D ?
 The CIDEr metric differs from CIDEr-D because it applies a stemmer to each word before computing the n-grams of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 
 ### Does metrics work on multi-GPU ?
 No. Most of these metrics use numpy or external java programs to run, which prevents multi-GPU testing for now.
 
-### Is torchmetrics needed for this package ?
-No. But if torchmetrics is installed, all metrics classes will inherit from the base class `torchmetrics.Metric`.
-It is because most of the metrics does not use PyTorch tensors to compute scores and numpy and strings cannot be added to states of `torchmetrics.Metric`.
-
 ## SPIDEr-max metric
 SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model. For more detail, please see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/stable/spider_max.html).
 
 ## References
 #### BLEU
 [1] K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, “BLEU: a
 method for automatic evaluation of machine translation,” in Proceed-
@@ -236,18 +232,18 @@
 
 If you use this software, please consider cite it as below :
 ```
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
-    month = {4},
+    month = {6},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.2},
+    version = {0.4.3},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.2 Summary: Metrics for
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.3 Summary: Metrics for
 evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
 email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
-pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
-Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
-repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
+pub@gmail.com> Project-URL: Homepage, https://pypi.org/project/aac-metrics/
+Project-URL: Documentation, https://aac-metrics.readthedocs.io/ Project-URL:
+Repository, https://github.com//Labbeti/aac-metrics.git Project-URL: Changelog,
 https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
 audio,metrics,text,captioning,audio-captioning Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -86,19 +86,15 @@
 specify a java executable path with `java_path` argument. - `unzip` command to
 extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
 CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
 before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
 reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
 audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 ### Does metrics work on multi-GPU ? No. Most of these metrics use numpy or
-external java programs to run, which prevents multi-GPU testing for now. ### Is
-torchmetrics needed for this package ? No. But if torchmetrics is installed,
-all metrics classes will inherit from the base class `torchmetrics.Metric`. It
-is because most of the metrics does not use PyTorch tensors to compute scores
-and numpy and strings cannot be added to states of `torchmetrics.Metric`. ##
+external java programs to run, which prevents multi-GPU testing for now. ##
 SPIDEr-max metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr
 that takes into account multiple candidates for the same audio. It computes the
 maximum of the SPIDEr scores for each candidate to balance the high sensitivity
 to the frequency of the words generated by the model. For more detail, please
 see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/
 stable/spider_max.html). ## References #### BLEU [1] K. Papineni, S. Roukos, T.
 Ward, and W.-J. Zhu, âBLEU: a method for automatic evaluation of machine
@@ -138,10 +134,10 @@
 Pellegrini, Thomas and Pinquier, Julien}, URL = {https://hal.archives-
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
-license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.2}, year = {2023}, } ``` ##
+license = {MIT}, month = {6}, title = {{aac-metrics}}, url = {https://
+github.com/Labbeti/aac-metrics/}, version = {0.4.3}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.2/src/aac_metrics.egg-info/SOURCES.txt` & `aac-metrics-0.4.3/src/aac_metrics.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENCE
 MANIFEST.in
 README.md
-install_spice.sh
 pyproject.toml
 setup.py
 ./setup.py
 ./.github/workflows/python-package-pip.yaml
 ./src/aac_metrics/__init__.py
 ./src/aac_metrics/__main__.py
 ./src/aac_metrics/download.py
@@ -44,16 +43,14 @@
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
 ./tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
 ./tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
 ./tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
 data/example_1.csv
 data/example_2.csv
-examples/example_1.csv
-examples/example_2.csv
 src/aac_metrics/__init__.py
 src/aac_metrics/__main__.py
 src/aac_metrics/download.py
 src/aac_metrics/evaluate.py
 src/aac_metrics/info.py
 src/aac_metrics/install_spice.sh
 src/aac_metrics.egg-info/PKG-INFO
```

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/caption-evaluation-tools/eval_metrics.py` & `aac-metrics-0.4.3/tests/caption-evaluation-tools/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/test_bleu_tchmet.py` & `aac-metrics-0.4.3/tests/test_bleu_tchmet.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/test_compare_cet.py` & `aac-metrics-0.4.3/tests/test_compare_cet.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/test_compare_fense.py` & `aac-metrics-0.4.3/tests/test_compare_fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/test_pickable.py` & `aac-metrics-0.4.3/tests/test_pickable.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.2/tests/test_utils.py` & `aac-metrics-0.4.3/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,17 @@
             ("1.7.0", False),
             ("1.8.0", True),
             ("1.9.0", False),
             ("1.10.0", False),
             ("9.0.0", True),
             ("10.0.0", True),
             ("11.0.0", True),
-            ("12.0.0", False),
+            ("12.0.0", True),
+            ("13.0.0", True),
+            ("14.0.0", False),
             ("17.0.0", False),
             ("20.0.0", False),
         ]
         for version, expected in test_set:
             output = _check_java_version(
                 version, MIN_JAVA_MAJOR_VERSION, MAX_JAVA_MAJOR_VERSION
             )
```

