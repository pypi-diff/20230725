# Comparing `tmp/pytorch-metric-learning-2.2.0.tar.gz` & `tmp/pytorch-metric-learning-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-metric-learning-2.2.0.tar", last modified: Sun Jun 18 18:02:42 2023, max compression
+gzip compressed data, was "pytorch-metric-learning-2.3.0.tar", last modified: Tue Jul 25 14:55:38 2023, max compression
```

## Comparing `pytorch-metric-learning-2.2.0.tar` & `pytorch-metric-learning-2.3.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.458103 pytorch-metric-learning-2.2.0/
--rw-r--r--   0 kevin      (501) staff       (20)     1090 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/LICENSE
--rw-r--r--   0 kevin      (501) staff       (20)    15727 2023-06-18 18:02:42.457936 pytorch-metric-learning-2.2.0/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)    15109 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/README.md
--rw-r--r--   0 kevin      (501) staff       (20)       38 2023-06-18 18:02:42.458140 pytorch-metric-learning-2.2.0/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)     1507 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/setup.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.442916 pytorch-metric-learning-2.2.0/src/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.443979 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/
--rw-r--r--   0 kevin      (501) staff       (20)       22 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.445503 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/
--rw-r--r--   0 kevin      (501) staff       (20)      265 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     3508 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/base_distance.py
--rw-r--r--   0 kevin      (501) staff       (20)      755 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/batched_distance.py
--rw-r--r--   0 kevin      (501) staff       (20)      274 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/cosine_similarity.py
--rw-r--r--   0 kevin      (501) staff       (20)      424 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/dot_product_similarity.py
--rw-r--r--   0 kevin      (501) staff       (20)     1042 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/lp_distance.py
--rw-r--r--   0 kevin      (501) staff       (20)      714 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/snr_distance.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.450231 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/
--rw-r--r--   0 kevin      (501) staff       (20)     1696 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     3061 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/angular_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1386 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/arcface_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)      391 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/base_loss_wrapper.py
--rw-r--r--   0 kevin      (501) staff       (20)     2456 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py
--rw-r--r--   0 kevin      (501) staff       (20)     2832 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/circle_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2005 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/contrastive_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)      939 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cosface_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     5333 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cross_batch_memory.py
--rw-r--r--   0 kevin      (501) staff       (20)     2833 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/fast_ap_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1492 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/generic_pair_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1689 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/instance_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2047 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     5674 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     3034 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     4731 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/manifold_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     3288 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/margin_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2863 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/mixins.py
--rw-r--r--   0 kevin      (501) staff       (20)     1558 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2351 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multiple_losses.py
--rw-r--r--   0 kevin      (501) staff       (20)     1463 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/n_pairs_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1957 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/nca_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2173 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1778 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/ntxent_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2635 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/p2s_grad_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     3506 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/pnp_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     3469 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1376 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_losses.py
--rw-r--r--   0 kevin      (501) staff       (20)     2269 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/self_supervised_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)      373 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
--rw-r--r--   0 kevin      (501) staff       (20)     3230 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/soft_triple_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)      360 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/sphereface_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2600 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     1715 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/supcon_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2290 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     2049 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
--rw-r--r--   0 kevin      (501) staff       (20)     3374 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/vicreg_loss.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.451826 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/
--rw-r--r--   0 kevin      (501) staff       (20)      569 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     2874 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/angular_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     2201 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/base_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     8131 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)      404 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/batch_hard_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     2066 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)      493 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
--rw-r--r--   0 kevin      (501) staff       (20)     2192 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/hdc_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     2315 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     1742 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/pair_margin_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     2461 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py
--rw-r--r--   0 kevin      (501) staff       (20)     2303 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.453175 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/
--rw-r--r--   0 kevin      (501) staff       (20)      459 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      169 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)     3816 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/base_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)     1130 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)     1551 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/divisor_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)      156 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)      473 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/mean_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/multiple_reducers.py
--rw-r--r--   0 kevin      (501) staff       (20)     2149 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)      182 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/sum_reducer.py
--rw-r--r--   0 kevin      (501) staff       (20)     2211 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/threshold_reducer.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.453962 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/
--rw-r--r--   0 kevin      (501) staff       (20)      338 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      499 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/base_regularizer.py
--rw-r--r--   0 kevin      (501) staff       (20)      871 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
--rw-r--r--   0 kevin      (501) staff       (20)      723 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py
--rw-r--r--   0 kevin      (501) staff       (20)     1229 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
--rw-r--r--   0 kevin      (501) staff       (20)     2697 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
--rw-r--r--   0 kevin      (501) staff       (20)      432 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.454567 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/
--rw-r--r--   0 kevin      (501) staff       (20)      220 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     2132 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
--rw-r--r--   0 kevin      (501) staff       (20)     3843 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
--rw-r--r--   0 kevin      (501) staff       (20)     2555 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
--rw-r--r--   0 kevin      (501) staff       (20)     1696 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.455483 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/
--rw-r--r--   0 kevin      (501) staff       (20)      243 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)    12495 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/base_tester.py
--rw-r--r--   0 kevin      (501) staff       (20)     1371 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_embedding_space.py
--rw-r--r--   0 kevin      (501) staff       (20)     2820 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
--rw-r--r--   0 kevin      (501) staff       (20)     2791 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/with_same_parent_label.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.456350 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/
--rw-r--r--   0 kevin      (501) staff       (20)      321 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)    11599 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/base_trainer.py
--rw-r--r--   0 kevin      (501) staff       (20)     3002 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
--rw-r--r--   0 kevin      (501) staff       (20)     6807 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
--rw-r--r--   0 kevin      (501) staff       (20)      625 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/metric_loss_only.py
--rw-r--r--   0 kevin      (501) staff       (20)     1224 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/train_with_classifier.py
--rw-r--r--   0 kevin      (501) staff       (20)     2295 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.457752 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)    18488 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/accuracy_calculator.py
--rw-r--r--   0 kevin      (501) staff       (20)    15447 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/common_functions.py
--rw-r--r--   0 kevin      (501) staff       (20)     6399 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/distributed.py
--rw-r--r--   0 kevin      (501) staff       (20)    11776 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/inference.py
--rw-r--r--   0 kevin      (501) staff       (20)     1801 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/key_checker.py
--rw-r--r--   0 kevin      (501) staff       (20)    15836 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/logging_presets.py
--rw-r--r--   0 kevin      (501) staff       (20)     9444 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
--rw-r--r--   0 kevin      (501) staff       (20)     1078 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_tracker.py
--rw-r--r--   0 kevin      (501) staff       (20)      661 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records.py
--rw-r--r--   0 kevin      (501) staff       (20)     1624 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.444579 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)    15727 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     6089 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)      226 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)       24 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/top_level.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.803415 pytorch-metric-learning-2.3.0/
+-rw-r--r--   0 kevin      (501) staff       (20)     1090 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/LICENSE
+-rw-r--r--   0 kevin      (501) staff       (20)    16399 2023-07-25 14:55:38.803117 pytorch-metric-learning-2.3.0/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)    15781 2023-07-21 19:43:14.000000 pytorch-metric-learning-2.3.0/README.md
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-07-25 14:55:38.803477 pytorch-metric-learning-2.3.0/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     1507 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.782919 pytorch-metric-learning-2.3.0/src/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.784314 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/
+-rw-r--r--   0 kevin      (501) staff       (20)       22 2023-07-25 14:55:02.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.786713 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/
+-rw-r--r--   0 kevin      (501) staff       (20)      265 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3508 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/base_distance.py
+-rw-r--r--   0 kevin      (501) staff       (20)      755 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/batched_distance.py
+-rw-r--r--   0 kevin      (501) staff       (20)      274 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/cosine_similarity.py
+-rw-r--r--   0 kevin      (501) staff       (20)      424 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/dot_product_similarity.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1042 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/lp_distance.py
+-rw-r--r--   0 kevin      (501) staff       (20)      714 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/snr_distance.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.792747 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/
+-rw-r--r--   0 kevin      (501) staff       (20)     1738 2023-07-25 14:55:02.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3061 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/angular_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1386 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/arcface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      391 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/base_loss_wrapper.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2456 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2832 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/circle_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2005 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/contrastive_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      939 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/cosface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5333 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/cross_batch_memory.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2833 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/fast_ap_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1492 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/generic_pair_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3184 2023-07-25 14:55:02.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/histogram_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1689 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/instance_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2047 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5674 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3034 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4731 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/manifold_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3288 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/margin_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2863 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/mixins.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1558 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2351 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/multiple_losses.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1463 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/n_pairs_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1957 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/nca_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2173 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1778 2023-07-21 21:59:36.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/ntxent_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2635 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/p2s_grad_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3506 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/pnp_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3469 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1376 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/proxy_losses.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2269 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/self_supervised_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      373 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3230 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/soft_triple_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      360 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/sphereface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2600 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1715 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/supcon_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2290 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2049 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3374 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/vicreg_loss.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.794793 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/
+-rw-r--r--   0 kevin      (501) staff       (20)      569 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2874 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/angular_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2201 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/base_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     8131 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)      404 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/batch_hard_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2066 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)      493 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2192 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/hdc_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2315 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1742 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/pair_margin_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2461 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2303 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.796619 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/
+-rw-r--r--   0 kevin      (501) staff       (20)      459 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      169 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3816 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/base_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1130 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1551 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/divisor_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      156 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      473 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/mean_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/multiple_reducers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2149 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      182 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/sum_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2211 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/threshold_reducer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.797816 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/
+-rw-r--r--   0 kevin      (501) staff       (20)      338 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      499 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/base_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      871 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      723 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1229 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2697 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      432 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.798740 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/
+-rw-r--r--   0 kevin      (501) staff       (20)      220 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2132 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3843 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2555 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1696 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.799563 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/
+-rw-r--r--   0 kevin      (501) staff       (20)      243 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12495 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/base_tester.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1371 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/global_embedding_space.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2820 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2791 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/with_same_parent_label.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.800765 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/
+-rw-r--r--   0 kevin      (501) staff       (20)      321 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11599 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/base_trainer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3002 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6807 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
+-rw-r--r--   0 kevin      (501) staff       (20)      625 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/metric_loss_only.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1224 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/train_with_classifier.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2295 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.802803 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    18489 2023-07-25 14:55:02.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/accuracy_calculator.py
+-rw-r--r--   0 kevin      (501) staff       (20)    15447 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/common_functions.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6399 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/distributed.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11776 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/inference.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1801 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/key_checker.py
+-rw-r--r--   0 kevin      (501) staff       (20)    15836 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/logging_presets.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9444 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1078 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/loss_tracker.py
+-rw-r--r--   0 kevin      (501) staff       (20)      661 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/module_with_records.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1624 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-25 14:55:38.785026 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)    16399 2023-07-25 14:55:38.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     6142 2023-07-25 14:55:38.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-07-25 14:55:38.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)      226 2023-07-25 14:55:38.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       24 2023-07-25 14:55:38.000000 pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/top_level.txt
```

### Comparing `pytorch-metric-learning-2.2.0/LICENSE` & `pytorch-metric-learning-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/PKG-INFO` & `pytorch-metric-learning-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-metric-learning
-Version: 2.2.0
+Version: 2.3.0
 Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
 Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
 Author: Kevin Musgrave
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
@@ -31,21 +31,23 @@
  <a href="https://anaconda.org/conda-forge/pytorch-metric-learning">
      <img alt="Anaconda version" src="https://img.shields.io/conda/v/conda-forge/pytorch-metric-learning?color=bright-green">
  </a>
 </p>
 
 ## News
 
+**June 18**: v2.2.0
+- Added [ManifoldLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) and [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#p2sgradloss).
+- Added a `symmetric` flag to [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss).
+- See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.2.0).
+- Thank you [domenicoMuscill0](https://github.com/domenicoMuscill0).
+
 **April 5**: v2.1.0
 - Added [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss)
-- Thanks to contributor [interestingzhuo](https://github.com/interestingzhuo).
-
-**January 29**: v2.0.0
-- Added SelfSupervisedLoss, plus various API improvements. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.0.0).
-- Thanks to contributor [cwkeam](https://github.com/cwkeam).
+- Thanks you [interestingzhuo](https://github.com/interestingzhuo).
 
 
 ## Documentation
 - [**View the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-learning/)
 - [**View the installation instructions here**](https://github.com/KevinMusgrave/pytorch-metric-learning#installation)
 - [**View the available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/CONTENTS.md) 
 
@@ -238,14 +240,15 @@
 ## Acknowledgements
 
 ### Contributors
 Thanks to the contributors who made pull requests!
 
 | Contributor | Highlights |
 | -- | -- |
+|[domenicoMuscill0](https://github.com/domenicoMuscill0)| - [ManifoldLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) <br/> - [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#p2sgradloss) 
 |[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any combination of query and reference sets <br/> - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) work with arbitrary label comparisons |
 |[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss) <br/> - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) <br/> - BaseLossWrapper|
 |[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer) <br/> - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/#twostreammetricloss) <br/> - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester) <br/> - [Example using trainers.TwoStreamMetricLoss](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/TwoStreamMetricLoss.ipynb) |
 | [chingisooinar](https://github.com/chingisooinar) | [SubCenterArcFaceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#subcenterarcfaceloss) |
 | [elias-ramzi](https://github.com/elias-ramzi) | [HierarchicalSampler](https://kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler) |
 | [fjsj](https://github.com/fjsj) | [SupConLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) |
 | [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) |
@@ -256,14 +259,15 @@
 | [Hummer12007](https://github.com/Hummer12007) | ```utils.key_checker``` |
 | [vltanh](https://github.com/vltanh) | Made ```InferenceModel.train_indexer``` accept datasets |
 | [btseytlin](https://github.com/btseytlin) | ```get_nearest_neighbors``` in [InferenceModel](https://kevinmusgrave.github.io/pytorch-metric-learning/inference_models) |
 | [mlw214](https://github.com/mlw214) | Added ```return_per_class``` to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
 | [layumi](https://github.com/layumi) | [InstanceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#instanceloss) |
 | [NoTody](https://github.com/NoTody) | Helped add `ref_emb` and `ref_labels` to the distributed wrappers. |
 | [ElisonSherton](https://github.com/ElisonSherton) | Fixed an edge case in ArcFaceLoss. |
+| [stompsjo](https://github.com/stompsjo) | Improved documentation for NTXentLoss |
 | [z1w](https://github.com/z1w) | |
 | [thinline72](https://github.com/thinline72) | |
 | [tpanum](https://github.com/tpanum) | |
 | [fralik](https://github.com/fralik) | |
 | [joaqo](https://github.com/joaqo) | |
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
@@ -286,14 +290,15 @@
 - https://github.com/facebookresearch/deepcluster
 - https://github.com/geonm/proxy-anchor-loss
 - https://github.com/idstcv/SoftTriple
 - https://github.com/kunhe/FastAP-metric-learning
 - https://github.com/ronekko/deep_metric_learning
 - https://github.com/tjddus9597/Proxy-Anchor-CVPR2020
 - http://kaizhao.net/regularface
+- https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts
 
 ### Logo
 Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing the logo.
 
 ## Citing this library
 If you'd like to cite pytorch-metric-learning in your paper, you can use this bibtex:
 ```latex
```

#### html2text {}

```diff
@@ -1,62 +1,66 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.2.0 Summary: The
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.3.0 Summary: The
 easiest way to use deep metric learning in your application. Modular, flexible,
 and extensible. Written in PyTorch. Home-page: https://github.com/
 KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.0
 Description-Content-Type: text/markdown Provides-Extra: with-hooks Provides-
 Extra: with-hooks-cpu Provides-Extra: docs Provides-Extra: dev License-File:
 LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
-## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
-pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
-[interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
-Added SelfSupervisedLoss, plus various API improvements. See the [release
-notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
-v2.0.0). - Thanks to contributor [cwkeam](https://github.com/cwkeam). ##
-Documentation - [**View the documentation here**](https://
-kevinmusgrave.github.io/pytorch-metric-learning/) - [**View the installation
-instructions here**](https://github.com/KevinMusgrave/pytorch-metric-
-learning#installation) - [**View the available losses, miners etc. here**]
-(https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
-CONTENTS.md) ## Google Colab Examples See the [examples folder](https://
-github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
-README.md) for notebooks you can download or run on Google Colab. ## PyTorch
-Metric Learning Overview This library contains 9 modules, each of which can be
-used independently within your existing codebase, or combined together for a
-complete train/test workflow. ![high_level_module_overview](docs/imgs/
-high_level_module_overview.png) ## How loss functions work ### Using losses and
-miners in your training loop Letâs initialize a plain [TripletMarginLoss]
-(https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
-#tripletmarginloss): ```python from pytorch_metric_learning import losses
-loss_func = losses.TripletMarginLoss() ``` To compute the loss in your training
-loop, pass in the embeddings computed by your model, and the corresponding
-labels. The embeddings should have size (N, embedding_size), and the labels
-should have size (N), where N is the batch size. ```python # your training loop
-for i, (data, labels) in enumerate(dataloader): optimizer.zero_grad()
-embeddings = model(data) loss = loss_func(embeddings, labels) loss.backward()
-optimizer.step() ``` The TripletMarginLoss computes all possible triplets
-within the batch, based on the labels you pass into it. Anchor-positive pairs
-are formed by embeddings that share the same label, and anchor-negative pairs
-are formed by embeddings that have different labels. Sometimes it can help to
-add a mining function: ```python from pytorch_metric_learning import miners,
-losses miner = miners.MultiSimilarityMiner() loss_func =
-losses.TripletMarginLoss() # your training loop for i, (data, labels) in
-enumerate(dataloader): optimizer.zero_grad() embeddings = model(data)
-hard_pairs = miner(embeddings, labels) loss = loss_func(embeddings, labels,
-hard_pairs) loss.backward() optimizer.step() ``` In the above code, the miner
-finds positive and negative pairs that it thinks are particularly difficult.
-Note that even though the TripletMarginLoss operates on triplets, itâs still
-possible to pass in pairs. This is because the library automatically converts
-pairs to triplets and triplets to pairs, when necessary. ### Customizing loss
-functions Loss functions can be customized using [distances](https://
-kevinmusgrave.github.io/pytorch-metric-learning/distances/), [reducers](https:/
-/kevinmusgrave.github.io/pytorch-metric-learning/reducers/), and [regularizers]
+## News **June 18**: v2.2.0 - Added [ManifoldLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) and
+[P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#p2sgradloss). - Added a `symmetric` flag to [SelfSupervisedLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss). -
+See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-
+learning/releases/tag/v2.2.0). - Thank you [domenicoMuscill0](https://
+github.com/domenicoMuscill0). **April 5**: v2.1.0 - Added [PNPLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) - Thanks you
+[interestingzhuo](https://github.com/interestingzhuo). ## Documentation -
+[**View the documentation here**](https://kevinmusgrave.github.io/pytorch-
+metric-learning/) - [**View the installation instructions here**](https://
+github.com/KevinMusgrave/pytorch-metric-learning#installation) - [**View the
+available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-
+metric-learning/blob/master/CONTENTS.md) ## Google Colab Examples See the
+[examples folder](https://github.com/KevinMusgrave/pytorch-metric-learning/
+blob/master/examples/README.md) for notebooks you can download or run on Google
+Colab. ## PyTorch Metric Learning Overview This library contains 9 modules,
+each of which can be used independently within your existing codebase, or
+combined together for a complete train/test workflow. !
+[high_level_module_overview](docs/imgs/high_level_module_overview.png) ## How
+loss functions work ### Using losses and miners in your training loop Letâs
+initialize a plain [TripletMarginLoss](https://kevinmusgrave.github.io/pytorch-
+metric-learning/losses/#tripletmarginloss): ```python from
+pytorch_metric_learning import losses loss_func = losses.TripletMarginLoss()
+``` To compute the loss in your training loop, pass in the embeddings computed
+by your model, and the corresponding labels. The embeddings should have size
+(N, embedding_size), and the labels should have size (N), where N is the batch
+size. ```python # your training loop for i, (data, labels) in enumerate
+(dataloader): optimizer.zero_grad() embeddings = model(data) loss = loss_func
+(embeddings, labels) loss.backward() optimizer.step() ``` The TripletMarginLoss
+computes all possible triplets within the batch, based on the labels you pass
+into it. Anchor-positive pairs are formed by embeddings that share the same
+label, and anchor-negative pairs are formed by embeddings that have different
+labels. Sometimes it can help to add a mining function: ```python from
+pytorch_metric_learning import miners, losses miner =
+miners.MultiSimilarityMiner() loss_func = losses.TripletMarginLoss() # your
+training loop for i, (data, labels) in enumerate(dataloader):
+optimizer.zero_grad() embeddings = model(data) hard_pairs = miner(embeddings,
+labels) loss = loss_func(embeddings, labels, hard_pairs) loss.backward()
+optimizer.step() ``` In the above code, the miner finds positive and negative
+pairs that it thinks are particularly difficult. Note that even though the
+TripletMarginLoss operates on triplets, itâs still possible to pass in pairs.
+This is because the library automatically converts pairs to triplets and
+triplets to pairs, when necessary. ### Customizing loss functions Loss
+functions can be customized using [distances](https://kevinmusgrave.github.io/
+pytorch-metric-learning/distances/), [reducers](https://
+kevinmusgrave.github.io/pytorch-metric-learning/reducers/), and [regularizers]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/regularizers/). In the
 diagram below, a miner finds the indices of hard pairs within a batch. These
 are used to index into the distance matrix, computed by the distance object.
 For this diagram, the loss function is pair-based, so it computes a loss per
 pair. In addition, a regularizer has been supplied, so a regularization loss is
 computed for each embedding in the batch. The per-pair and per-element losses
 are passed to the reducer, which (in this diagram) only keeps losses with a
@@ -121,18 +125,21 @@
 datatypes and test device as environment variables. For example, to test using
 float32 and float64 on the CPU: ```bash TEST_DTYPES=float32,float64
 TEST_DEVICE=cpu python -m unittest discover ``` To run a single test file
 instead of the entire test suite, specify the file name: ```bash python -
 m unittest tests/losses/test_angular_loss.py ``` Code is formatted using
 ```black``` and ```isort```: ```bash pip install black isort ./format_code.sh
 ``` ## Acknowledgements ### Contributors Thanks to the contributors who made
-pull requests! | Contributor | Highlights | | -- | -- | |[mlopezantequera]
-(https://github.com/mlopezantequera) | - Made the [testers](https://
-kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
-combination of query and reference sets
+pull requests! | Contributor | Highlights | | -- | -- | |[domenicoMuscill0]
+(https://github.com/domenicoMuscill0)| - [ManifoldLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss)
+- [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#p2sgradloss) |[mlopezantequera](https://github.com/mlopezantequera) | - Made
+the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers)
+work on any combination of query and reference sets
 - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-
 learning/accuracy_calculation/) work with arbitrary label comparisons | |
 [cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss)
 - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
 #vicregloss)
 - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://
@@ -171,15 +178,16 @@
 kevinmusgrave.github.io/pytorch-metric-learning/inference_models) | | [mlw214]
 (https://github.com/mlw214) | Added ```return_per_class``` to
 [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/
 accuracy_calculation/) | | [layumi](https://github.com/layumi) | [InstanceLoss]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#instanceloss)
 | | [NoTody](https://github.com/NoTody) | Helped add `ref_emb` and `ref_labels`
 to the distributed wrappers. | | [ElisonSherton](https://github.com/
-ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [z1w](https://
+ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [stompsjo](https://
+github.com/stompsjo) | Improved documentation for NTXentLoss | | [z1w](https://
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
 [michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
@@ -196,13 +204,14 @@
 that has been adapted and modified from the following great open-source repos:
 - https://github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/
 incubator-mxnet/blob/master/example/gluon/embedding_learning - https://
 github.com/facebookresearch/deepcluster - https://github.com/geonm/proxy-
 anchor-loss - https://github.com/idstcv/SoftTriple - https://github.com/kunhe/
 FastAP-metric-learning - https://github.com/ronekko/deep_metric_learning -
 https://github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/
-regularface ### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/
-) for designing the logo. ## Citing this library If you'd like to cite pytorch-
-metric-learning in your paper, you can use this bibtex: ```latex @article
+regularface - https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts
+### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing
+the logo. ## Citing this library If you'd like to cite pytorch-metric-learning
+in your paper, you can use this bibtex: ```latex @article
 {Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
 and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
 {abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.2.0/README.md` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pytorch-metric-learning
+Version: 2.3.0
+Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
+Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
+Author: Kevin Musgrave
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+Provides-Extra: with-hooks
+Provides-Extra: with-hooks-cpu
+Provides-Extra: docs
+Provides-Extra: dev
+License-File: LICENSE
+
 <h1>
 <a href="https://github.com/KevinMusgrave/pytorch-metric-learning">
 <img alt="PyTorch Metric Learning" src="https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/docs/imgs/Logo2.png">
 </a>
 </h1>
 
 <p align="center">
@@ -14,21 +31,23 @@
  <a href="https://anaconda.org/conda-forge/pytorch-metric-learning">
      <img alt="Anaconda version" src="https://img.shields.io/conda/v/conda-forge/pytorch-metric-learning?color=bright-green">
  </a>
 </p>
 
 ## News
 
+**June 18**: v2.2.0
+- Added [ManifoldLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) and [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#p2sgradloss).
+- Added a `symmetric` flag to [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss).
+- See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.2.0).
+- Thank you [domenicoMuscill0](https://github.com/domenicoMuscill0).
+
 **April 5**: v2.1.0
 - Added [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss)
-- Thanks to contributor [interestingzhuo](https://github.com/interestingzhuo).
-
-**January 29**: v2.0.0
-- Added SelfSupervisedLoss, plus various API improvements. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.0.0).
-- Thanks to contributor [cwkeam](https://github.com/cwkeam).
+- Thanks you [interestingzhuo](https://github.com/interestingzhuo).
 
 
 ## Documentation
 - [**View the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-learning/)
 - [**View the installation instructions here**](https://github.com/KevinMusgrave/pytorch-metric-learning#installation)
 - [**View the available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/CONTENTS.md) 
 
@@ -221,14 +240,15 @@
 ## Acknowledgements
 
 ### Contributors
 Thanks to the contributors who made pull requests!
 
 | Contributor | Highlights |
 | -- | -- |
+|[domenicoMuscill0](https://github.com/domenicoMuscill0)| - [ManifoldLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) <br/> - [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#p2sgradloss) 
 |[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any combination of query and reference sets <br/> - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) work with arbitrary label comparisons |
 |[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss) <br/> - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) <br/> - BaseLossWrapper|
 |[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer) <br/> - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/#twostreammetricloss) <br/> - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester) <br/> - [Example using trainers.TwoStreamMetricLoss](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/TwoStreamMetricLoss.ipynb) |
 | [chingisooinar](https://github.com/chingisooinar) | [SubCenterArcFaceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#subcenterarcfaceloss) |
 | [elias-ramzi](https://github.com/elias-ramzi) | [HierarchicalSampler](https://kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler) |
 | [fjsj](https://github.com/fjsj) | [SupConLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) |
 | [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) |
@@ -239,14 +259,15 @@
 | [Hummer12007](https://github.com/Hummer12007) | ```utils.key_checker``` |
 | [vltanh](https://github.com/vltanh) | Made ```InferenceModel.train_indexer``` accept datasets |
 | [btseytlin](https://github.com/btseytlin) | ```get_nearest_neighbors``` in [InferenceModel](https://kevinmusgrave.github.io/pytorch-metric-learning/inference_models) |
 | [mlw214](https://github.com/mlw214) | Added ```return_per_class``` to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
 | [layumi](https://github.com/layumi) | [InstanceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#instanceloss) |
 | [NoTody](https://github.com/NoTody) | Helped add `ref_emb` and `ref_labels` to the distributed wrappers. |
 | [ElisonSherton](https://github.com/ElisonSherton) | Fixed an edge case in ArcFaceLoss. |
+| [stompsjo](https://github.com/stompsjo) | Improved documentation for NTXentLoss |
 | [z1w](https://github.com/z1w) | |
 | [thinline72](https://github.com/thinline72) | |
 | [tpanum](https://github.com/tpanum) | |
 | [fralik](https://github.com/fralik) | |
 | [joaqo](https://github.com/joaqo) | |
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
@@ -269,14 +290,15 @@
 - https://github.com/facebookresearch/deepcluster
 - https://github.com/geonm/proxy-anchor-loss
 - https://github.com/idstcv/SoftTriple
 - https://github.com/kunhe/FastAP-metric-learning
 - https://github.com/ronekko/deep_metric_learning
 - https://github.com/tjddus9597/Proxy-Anchor-CVPR2020
 - http://kaizhao.net/regularface
+- https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts
 
 ### Logo
 Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing the logo.
 
 ## Citing this library
 If you'd like to cite pytorch-metric-learning in your paper, you can use this bibtex:
 ```latex
```

#### html2text {}

```diff
@@ -1,53 +1,66 @@
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.3.0 Summary: The
+easiest way to use deep metric learning in your application. Modular, flexible,
+and extensible. Written in PyTorch. Home-page: https://github.com/
+KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.0
+Description-Content-Type: text/markdown Provides-Extra: with-hooks Provides-
+Extra: with-hooks-cpu Provides-Extra: docs Provides-Extra: dev License-File:
+LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
-## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
-pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
-[interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
-Added SelfSupervisedLoss, plus various API improvements. See the [release
-notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
-v2.0.0). - Thanks to contributor [cwkeam](https://github.com/cwkeam). ##
-Documentation - [**View the documentation here**](https://
-kevinmusgrave.github.io/pytorch-metric-learning/) - [**View the installation
-instructions here**](https://github.com/KevinMusgrave/pytorch-metric-
-learning#installation) - [**View the available losses, miners etc. here**]
-(https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
-CONTENTS.md) ## Google Colab Examples See the [examples folder](https://
-github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
-README.md) for notebooks you can download or run on Google Colab. ## PyTorch
-Metric Learning Overview This library contains 9 modules, each of which can be
-used independently within your existing codebase, or combined together for a
-complete train/test workflow. ![high_level_module_overview](docs/imgs/
-high_level_module_overview.png) ## How loss functions work ### Using losses and
-miners in your training loop Letâs initialize a plain [TripletMarginLoss]
-(https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
-#tripletmarginloss): ```python from pytorch_metric_learning import losses
-loss_func = losses.TripletMarginLoss() ``` To compute the loss in your training
-loop, pass in the embeddings computed by your model, and the corresponding
-labels. The embeddings should have size (N, embedding_size), and the labels
-should have size (N), where N is the batch size. ```python # your training loop
-for i, (data, labels) in enumerate(dataloader): optimizer.zero_grad()
-embeddings = model(data) loss = loss_func(embeddings, labels) loss.backward()
-optimizer.step() ``` The TripletMarginLoss computes all possible triplets
-within the batch, based on the labels you pass into it. Anchor-positive pairs
-are formed by embeddings that share the same label, and anchor-negative pairs
-are formed by embeddings that have different labels. Sometimes it can help to
-add a mining function: ```python from pytorch_metric_learning import miners,
-losses miner = miners.MultiSimilarityMiner() loss_func =
-losses.TripletMarginLoss() # your training loop for i, (data, labels) in
-enumerate(dataloader): optimizer.zero_grad() embeddings = model(data)
-hard_pairs = miner(embeddings, labels) loss = loss_func(embeddings, labels,
-hard_pairs) loss.backward() optimizer.step() ``` In the above code, the miner
-finds positive and negative pairs that it thinks are particularly difficult.
-Note that even though the TripletMarginLoss operates on triplets, itâs still
-possible to pass in pairs. This is because the library automatically converts
-pairs to triplets and triplets to pairs, when necessary. ### Customizing loss
-functions Loss functions can be customized using [distances](https://
-kevinmusgrave.github.io/pytorch-metric-learning/distances/), [reducers](https:/
-/kevinmusgrave.github.io/pytorch-metric-learning/reducers/), and [regularizers]
+## News **June 18**: v2.2.0 - Added [ManifoldLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) and
+[P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#p2sgradloss). - Added a `symmetric` flag to [SelfSupervisedLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss). -
+See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-
+learning/releases/tag/v2.2.0). - Thank you [domenicoMuscill0](https://
+github.com/domenicoMuscill0). **April 5**: v2.1.0 - Added [PNPLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) - Thanks you
+[interestingzhuo](https://github.com/interestingzhuo). ## Documentation -
+[**View the documentation here**](https://kevinmusgrave.github.io/pytorch-
+metric-learning/) - [**View the installation instructions here**](https://
+github.com/KevinMusgrave/pytorch-metric-learning#installation) - [**View the
+available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-
+metric-learning/blob/master/CONTENTS.md) ## Google Colab Examples See the
+[examples folder](https://github.com/KevinMusgrave/pytorch-metric-learning/
+blob/master/examples/README.md) for notebooks you can download or run on Google
+Colab. ## PyTorch Metric Learning Overview This library contains 9 modules,
+each of which can be used independently within your existing codebase, or
+combined together for a complete train/test workflow. !
+[high_level_module_overview](docs/imgs/high_level_module_overview.png) ## How
+loss functions work ### Using losses and miners in your training loop Letâs
+initialize a plain [TripletMarginLoss](https://kevinmusgrave.github.io/pytorch-
+metric-learning/losses/#tripletmarginloss): ```python from
+pytorch_metric_learning import losses loss_func = losses.TripletMarginLoss()
+``` To compute the loss in your training loop, pass in the embeddings computed
+by your model, and the corresponding labels. The embeddings should have size
+(N, embedding_size), and the labels should have size (N), where N is the batch
+size. ```python # your training loop for i, (data, labels) in enumerate
+(dataloader): optimizer.zero_grad() embeddings = model(data) loss = loss_func
+(embeddings, labels) loss.backward() optimizer.step() ``` The TripletMarginLoss
+computes all possible triplets within the batch, based on the labels you pass
+into it. Anchor-positive pairs are formed by embeddings that share the same
+label, and anchor-negative pairs are formed by embeddings that have different
+labels. Sometimes it can help to add a mining function: ```python from
+pytorch_metric_learning import miners, losses miner =
+miners.MultiSimilarityMiner() loss_func = losses.TripletMarginLoss() # your
+training loop for i, (data, labels) in enumerate(dataloader):
+optimizer.zero_grad() embeddings = model(data) hard_pairs = miner(embeddings,
+labels) loss = loss_func(embeddings, labels, hard_pairs) loss.backward()
+optimizer.step() ``` In the above code, the miner finds positive and negative
+pairs that it thinks are particularly difficult. Note that even though the
+TripletMarginLoss operates on triplets, itâs still possible to pass in pairs.
+This is because the library automatically converts pairs to triplets and
+triplets to pairs, when necessary. ### Customizing loss functions Loss
+functions can be customized using [distances](https://kevinmusgrave.github.io/
+pytorch-metric-learning/distances/), [reducers](https://
+kevinmusgrave.github.io/pytorch-metric-learning/reducers/), and [regularizers]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/regularizers/). In the
 diagram below, a miner finds the indices of hard pairs within a batch. These
 are used to index into the distance matrix, computed by the distance object.
 For this diagram, the loss function is pair-based, so it computes a loss per
 pair. In addition, a regularizer has been supplied, so a regularization loss is
 computed for each embedding in the batch. The per-pair and per-element losses
 are passed to the reducer, which (in this diagram) only keeps losses with a
@@ -112,18 +125,21 @@
 datatypes and test device as environment variables. For example, to test using
 float32 and float64 on the CPU: ```bash TEST_DTYPES=float32,float64
 TEST_DEVICE=cpu python -m unittest discover ``` To run a single test file
 instead of the entire test suite, specify the file name: ```bash python -
 m unittest tests/losses/test_angular_loss.py ``` Code is formatted using
 ```black``` and ```isort```: ```bash pip install black isort ./format_code.sh
 ``` ## Acknowledgements ### Contributors Thanks to the contributors who made
-pull requests! | Contributor | Highlights | | -- | -- | |[mlopezantequera]
-(https://github.com/mlopezantequera) | - Made the [testers](https://
-kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
-combination of query and reference sets
+pull requests! | Contributor | Highlights | | -- | -- | |[domenicoMuscill0]
+(https://github.com/domenicoMuscill0)| - [ManifoldLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss)
+- [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#p2sgradloss) |[mlopezantequera](https://github.com/mlopezantequera) | - Made
+the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers)
+work on any combination of query and reference sets
 - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-
 learning/accuracy_calculation/) work with arbitrary label comparisons | |
 [cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss)
 - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
 #vicregloss)
 - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://
@@ -162,15 +178,16 @@
 kevinmusgrave.github.io/pytorch-metric-learning/inference_models) | | [mlw214]
 (https://github.com/mlw214) | Added ```return_per_class``` to
 [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/
 accuracy_calculation/) | | [layumi](https://github.com/layumi) | [InstanceLoss]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#instanceloss)
 | | [NoTody](https://github.com/NoTody) | Helped add `ref_emb` and `ref_labels`
 to the distributed wrappers. | | [ElisonSherton](https://github.com/
-ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [z1w](https://
+ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [stompsjo](https://
+github.com/stompsjo) | Improved documentation for NTXentLoss | | [z1w](https://
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
 [michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
@@ -187,13 +204,14 @@
 that has been adapted and modified from the following great open-source repos:
 - https://github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/
 incubator-mxnet/blob/master/example/gluon/embedding_learning - https://
 github.com/facebookresearch/deepcluster - https://github.com/geonm/proxy-
 anchor-loss - https://github.com/idstcv/SoftTriple - https://github.com/kunhe/
 FastAP-metric-learning - https://github.com/ronekko/deep_metric_learning -
 https://github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/
-regularface ### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/
-) for designing the logo. ## Citing this library If you'd like to cite pytorch-
-metric-learning in your paper, you can use this bibtex: ```latex @article
+regularface - https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts
+### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing
+the logo. ## Citing this library If you'd like to cite pytorch-metric-learning
+in your paper, you can use this bibtex: ```latex @article
 {Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
 and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
 {abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.2.0/setup.py` & `pytorch-metric-learning-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/base_distance.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/base_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/batched_distance.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/batched_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/lp_distance.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/lp_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/snr_distance.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/distances/snr_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/__init__.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .base_metric_loss_function import BaseMetricLossFunction
 from .circle_loss import CircleLoss
 from .contrastive_loss import ContrastiveLoss
 from .cosface_loss import CosFaceLoss
 from .cross_batch_memory import CrossBatchMemory
 from .fast_ap_loss import FastAPLoss
 from .generic_pair_loss import GenericPairLoss
+from .histogram_loss import HistogramLoss
 from .instance_loss import InstanceLoss
 from .intra_pair_variance_loss import IntraPairVarianceLoss
 from .large_margin_softmax_loss import LargeMarginSoftmaxLoss
 from .lifted_structure_loss import GeneralizedLiftedStructureLoss, LiftedStructureLoss
 from .manifold_loss import ManifoldLoss
 from .margin_loss import MarginLoss
 from .mixins import EmbeddingRegularizerMixin, WeightRegularizerMixin
```

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/angular_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/angular_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/arcface_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/circle_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/contrastive_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cosface_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/cosface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cross_batch_memory.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/cross_batch_memory.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/fast_ap_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/fast_ap_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/generic_pair_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/generic_pair_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/instance_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/instance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/manifold_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/manifold_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/margin_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/mixins.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multiple_losses.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/multiple_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/n_pairs_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/n_pairs_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/nca_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/nca_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/ntxent_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/ntxent_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/p2s_grad_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/p2s_grad_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/pnp_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/pnp_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_losses.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/proxy_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/self_supervised_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/self_supervised_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/soft_triple_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/soft_triple_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/supcon_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/supcon_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/vicreg_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/losses/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/__init__.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/angular_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/angular_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/base_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/base_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/hdc_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/hdc_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/pair_margin_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/pair_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/base_reducer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/base_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/divisor_reducer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/divisor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/multiple_reducers.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/multiple_reducers.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/threshold_reducer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/reducers/threshold_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/base_tester.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/base_tester.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_embedding_space.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/global_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/with_same_parent_label.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/testers/with_same_parent_label.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/base_trainer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/base_trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/metric_loss_only.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/metric_loss_only.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/train_with_classifier.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/train_with_classifier.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/accuracy_calculator.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/accuracy_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
 
         if ref_includes_query and not (
             torch.allclose(query, reference[: len(query)])
             and torch.allclose(query_labels, reference_labels[: len(query)])
         ):
             raise ValueError(
                 "When ref_includes_query is True, the first len(query) elements of reference must be equal to query.\n"
-                "Likewise, the first len(query_labels) elements of reference_lbels must be equal to query_labels.\n"
+                "Likewise, the first len(query_labels) elements of reference_labels must be equal to query_labels.\n"
             )
 
         self.curr_function_dict = self.get_function_dict(include, exclude)
 
         kwargs = {
             "query": query,
             "reference": reference,
```

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/common_functions.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/distributed.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/inference.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/inference.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/key_checker.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/key_checker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/logging_presets.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/logging_presets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_tracker.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/loss_tracker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/module_with_records.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/PKG-INFO` & `pytorch-metric-learning-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pytorch-metric-learning
-Version: 2.2.0
-Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
-Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
-Author: Kevin Musgrave
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-Provides-Extra: with-hooks
-Provides-Extra: with-hooks-cpu
-Provides-Extra: docs
-Provides-Extra: dev
-License-File: LICENSE
-
 <h1>
 <a href="https://github.com/KevinMusgrave/pytorch-metric-learning">
 <img alt="PyTorch Metric Learning" src="https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/docs/imgs/Logo2.png">
 </a>
 </h1>
 
 <p align="center">
@@ -31,21 +14,23 @@
  <a href="https://anaconda.org/conda-forge/pytorch-metric-learning">
      <img alt="Anaconda version" src="https://img.shields.io/conda/v/conda-forge/pytorch-metric-learning?color=bright-green">
  </a>
 </p>
 
 ## News
 
+**June 18**: v2.2.0
+- Added [ManifoldLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) and [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#p2sgradloss).
+- Added a `symmetric` flag to [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss).
+- See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.2.0).
+- Thank you [domenicoMuscill0](https://github.com/domenicoMuscill0).
+
 **April 5**: v2.1.0
 - Added [PNPLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss)
-- Thanks to contributor [interestingzhuo](https://github.com/interestingzhuo).
-
-**January 29**: v2.0.0
-- Added SelfSupervisedLoss, plus various API improvements. See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/v2.0.0).
-- Thanks to contributor [cwkeam](https://github.com/cwkeam).
+- Thanks you [interestingzhuo](https://github.com/interestingzhuo).
 
 
 ## Documentation
 - [**View the documentation here**](https://kevinmusgrave.github.io/pytorch-metric-learning/)
 - [**View the installation instructions here**](https://github.com/KevinMusgrave/pytorch-metric-learning#installation)
 - [**View the available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/CONTENTS.md) 
 
@@ -238,14 +223,15 @@
 ## Acknowledgements
 
 ### Contributors
 Thanks to the contributors who made pull requests!
 
 | Contributor | Highlights |
 | -- | -- |
+|[domenicoMuscill0](https://github.com/domenicoMuscill0)| - [ManifoldLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) <br/> - [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#p2sgradloss) 
 |[mlopezantequera](https://github.com/mlopezantequera) | - Made the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any combination of query and reference sets <br/> - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) work with arbitrary label comparisons |
 |[cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss) <br/> - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#vicregloss) <br/> - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) <br/> - BaseLossWrapper|
 |[marijnl](https://github.com/marijnl)| - [BatchEasyHardMiner](https://kevinmusgrave.github.io/pytorch-metric-learning/miners/#batcheasyhardminer) <br/> - [TwoStreamMetricLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/trainers/#twostreammetricloss) <br/> - [GlobalTwoStreamEmbeddingSpaceTester](https://kevinmusgrave.github.io/pytorch-metric-learning/testers/#globaltwostreamembeddingspacetester) <br/> - [Example using trainers.TwoStreamMetricLoss](https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/notebooks/TwoStreamMetricLoss.ipynb) |
 | [chingisooinar](https://github.com/chingisooinar) | [SubCenterArcFaceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#subcenterarcfaceloss) |
 | [elias-ramzi](https://github.com/elias-ramzi) | [HierarchicalSampler](https://kevinmusgrave.github.io/pytorch-metric-learning/samplers/#hierarchicalsampler) |
 | [fjsj](https://github.com/fjsj) | [SupConLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#supconloss) |
 | [AlenUbuntu](https://github.com/AlenUbuntu) | [CircleLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#circleloss) |
@@ -256,14 +242,15 @@
 | [Hummer12007](https://github.com/Hummer12007) | ```utils.key_checker``` |
 | [vltanh](https://github.com/vltanh) | Made ```InferenceModel.train_indexer``` accept datasets |
 | [btseytlin](https://github.com/btseytlin) | ```get_nearest_neighbors``` in [InferenceModel](https://kevinmusgrave.github.io/pytorch-metric-learning/inference_models) |
 | [mlw214](https://github.com/mlw214) | Added ```return_per_class``` to [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/accuracy_calculation/) |
 | [layumi](https://github.com/layumi) | [InstanceLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#instanceloss) |
 | [NoTody](https://github.com/NoTody) | Helped add `ref_emb` and `ref_labels` to the distributed wrappers. |
 | [ElisonSherton](https://github.com/ElisonSherton) | Fixed an edge case in ArcFaceLoss. |
+| [stompsjo](https://github.com/stompsjo) | Improved documentation for NTXentLoss |
 | [z1w](https://github.com/z1w) | |
 | [thinline72](https://github.com/thinline72) | |
 | [tpanum](https://github.com/tpanum) | |
 | [fralik](https://github.com/fralik) | |
 | [joaqo](https://github.com/joaqo) | |
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
@@ -286,14 +273,15 @@
 - https://github.com/facebookresearch/deepcluster
 - https://github.com/geonm/proxy-anchor-loss
 - https://github.com/idstcv/SoftTriple
 - https://github.com/kunhe/FastAP-metric-learning
 - https://github.com/ronekko/deep_metric_learning
 - https://github.com/tjddus9597/Proxy-Anchor-CVPR2020
 - http://kaizhao.net/regularface
+- https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts
 
 ### Logo
 Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing the logo.
 
 ## Citing this library
 If you'd like to cite pytorch-metric-learning in your paper, you can use this bibtex:
 ```latex
```

#### html2text {}

```diff
@@ -1,62 +1,57 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.2.0 Summary: The
-easiest way to use deep metric learning in your application. Modular, flexible,
-and extensible. Written in PyTorch. Home-page: https://github.com/
-KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.0
-Description-Content-Type: text/markdown Provides-Extra: with-hooks Provides-
-Extra: with-hooks-cpu Provides-Extra: docs Provides-Extra: dev License-File:
-LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
-## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
-pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
-[interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
-Added SelfSupervisedLoss, plus various API improvements. See the [release
-notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
-v2.0.0). - Thanks to contributor [cwkeam](https://github.com/cwkeam). ##
-Documentation - [**View the documentation here**](https://
-kevinmusgrave.github.io/pytorch-metric-learning/) - [**View the installation
-instructions here**](https://github.com/KevinMusgrave/pytorch-metric-
-learning#installation) - [**View the available losses, miners etc. here**]
-(https://github.com/KevinMusgrave/pytorch-metric-learning/blob/master/
-CONTENTS.md) ## Google Colab Examples See the [examples folder](https://
-github.com/KevinMusgrave/pytorch-metric-learning/blob/master/examples/
-README.md) for notebooks you can download or run on Google Colab. ## PyTorch
-Metric Learning Overview This library contains 9 modules, each of which can be
-used independently within your existing codebase, or combined together for a
-complete train/test workflow. ![high_level_module_overview](docs/imgs/
-high_level_module_overview.png) ## How loss functions work ### Using losses and
-miners in your training loop Letâs initialize a plain [TripletMarginLoss]
-(https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
-#tripletmarginloss): ```python from pytorch_metric_learning import losses
-loss_func = losses.TripletMarginLoss() ``` To compute the loss in your training
-loop, pass in the embeddings computed by your model, and the corresponding
-labels. The embeddings should have size (N, embedding_size), and the labels
-should have size (N), where N is the batch size. ```python # your training loop
-for i, (data, labels) in enumerate(dataloader): optimizer.zero_grad()
-embeddings = model(data) loss = loss_func(embeddings, labels) loss.backward()
-optimizer.step() ``` The TripletMarginLoss computes all possible triplets
-within the batch, based on the labels you pass into it. Anchor-positive pairs
-are formed by embeddings that share the same label, and anchor-negative pairs
-are formed by embeddings that have different labels. Sometimes it can help to
-add a mining function: ```python from pytorch_metric_learning import miners,
-losses miner = miners.MultiSimilarityMiner() loss_func =
-losses.TripletMarginLoss() # your training loop for i, (data, labels) in
-enumerate(dataloader): optimizer.zero_grad() embeddings = model(data)
-hard_pairs = miner(embeddings, labels) loss = loss_func(embeddings, labels,
-hard_pairs) loss.backward() optimizer.step() ``` In the above code, the miner
-finds positive and negative pairs that it thinks are particularly difficult.
-Note that even though the TripletMarginLoss operates on triplets, itâs still
-possible to pass in pairs. This is because the library automatically converts
-pairs to triplets and triplets to pairs, when necessary. ### Customizing loss
-functions Loss functions can be customized using [distances](https://
-kevinmusgrave.github.io/pytorch-metric-learning/distances/), [reducers](https:/
-/kevinmusgrave.github.io/pytorch-metric-learning/reducers/), and [regularizers]
+## News **June 18**: v2.2.0 - Added [ManifoldLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss) and
+[P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#p2sgradloss). - Added a `symmetric` flag to [SelfSupervisedLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss). -
+See the [release notes](https://github.com/KevinMusgrave/pytorch-metric-
+learning/releases/tag/v2.2.0). - Thank you [domenicoMuscill0](https://
+github.com/domenicoMuscill0). **April 5**: v2.1.0 - Added [PNPLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#pnploss) - Thanks you
+[interestingzhuo](https://github.com/interestingzhuo). ## Documentation -
+[**View the documentation here**](https://kevinmusgrave.github.io/pytorch-
+metric-learning/) - [**View the installation instructions here**](https://
+github.com/KevinMusgrave/pytorch-metric-learning#installation) - [**View the
+available losses, miners etc. here**](https://github.com/KevinMusgrave/pytorch-
+metric-learning/blob/master/CONTENTS.md) ## Google Colab Examples See the
+[examples folder](https://github.com/KevinMusgrave/pytorch-metric-learning/
+blob/master/examples/README.md) for notebooks you can download or run on Google
+Colab. ## PyTorch Metric Learning Overview This library contains 9 modules,
+each of which can be used independently within your existing codebase, or
+combined together for a complete train/test workflow. !
+[high_level_module_overview](docs/imgs/high_level_module_overview.png) ## How
+loss functions work ### Using losses and miners in your training loop Letâs
+initialize a plain [TripletMarginLoss](https://kevinmusgrave.github.io/pytorch-
+metric-learning/losses/#tripletmarginloss): ```python from
+pytorch_metric_learning import losses loss_func = losses.TripletMarginLoss()
+``` To compute the loss in your training loop, pass in the embeddings computed
+by your model, and the corresponding labels. The embeddings should have size
+(N, embedding_size), and the labels should have size (N), where N is the batch
+size. ```python # your training loop for i, (data, labels) in enumerate
+(dataloader): optimizer.zero_grad() embeddings = model(data) loss = loss_func
+(embeddings, labels) loss.backward() optimizer.step() ``` The TripletMarginLoss
+computes all possible triplets within the batch, based on the labels you pass
+into it. Anchor-positive pairs are formed by embeddings that share the same
+label, and anchor-negative pairs are formed by embeddings that have different
+labels. Sometimes it can help to add a mining function: ```python from
+pytorch_metric_learning import miners, losses miner =
+miners.MultiSimilarityMiner() loss_func = losses.TripletMarginLoss() # your
+training loop for i, (data, labels) in enumerate(dataloader):
+optimizer.zero_grad() embeddings = model(data) hard_pairs = miner(embeddings,
+labels) loss = loss_func(embeddings, labels, hard_pairs) loss.backward()
+optimizer.step() ``` In the above code, the miner finds positive and negative
+pairs that it thinks are particularly difficult. Note that even though the
+TripletMarginLoss operates on triplets, itâs still possible to pass in pairs.
+This is because the library automatically converts pairs to triplets and
+triplets to pairs, when necessary. ### Customizing loss functions Loss
+functions can be customized using [distances](https://kevinmusgrave.github.io/
+pytorch-metric-learning/distances/), [reducers](https://
+kevinmusgrave.github.io/pytorch-metric-learning/reducers/), and [regularizers]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/regularizers/). In the
 diagram below, a miner finds the indices of hard pairs within a batch. These
 are used to index into the distance matrix, computed by the distance object.
 For this diagram, the loss function is pair-based, so it computes a loss per
 pair. In addition, a regularizer has been supplied, so a regularization loss is
 computed for each embedding in the batch. The per-pair and per-element losses
 are passed to the reducer, which (in this diagram) only keeps losses with a
@@ -121,18 +116,21 @@
 datatypes and test device as environment variables. For example, to test using
 float32 and float64 on the CPU: ```bash TEST_DTYPES=float32,float64
 TEST_DEVICE=cpu python -m unittest discover ``` To run a single test file
 instead of the entire test suite, specify the file name: ```bash python -
 m unittest tests/losses/test_angular_loss.py ``` Code is formatted using
 ```black``` and ```isort```: ```bash pip install black isort ./format_code.sh
 ``` ## Acknowledgements ### Contributors Thanks to the contributors who made
-pull requests! | Contributor | Highlights | | -- | -- | |[mlopezantequera]
-(https://github.com/mlopezantequera) | - Made the [testers](https://
-kevinmusgrave.github.io/pytorch-metric-learning/testers) work on any
-combination of query and reference sets
+pull requests! | Contributor | Highlights | | -- | -- | |[domenicoMuscill0]
+(https://github.com/domenicoMuscill0)| - [ManifoldLoss](https://
+kevinmusgrave.github.io/pytorch-metric-learning/losses/#manifoldloss)
+- [P2SGradLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
+#p2sgradloss) |[mlopezantequera](https://github.com/mlopezantequera) | - Made
+the [testers](https://kevinmusgrave.github.io/pytorch-metric-learning/testers)
+work on any combination of query and reference sets
 - Made [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-
 learning/accuracy_calculation/) work with arbitrary label comparisons | |
 [cwkeam](https://github.com/cwkeam) | - [SelfSupervisedLoss](https://
 kevinmusgrave.github.io/pytorch-metric-learning/losses/#selfsupervisedloss)
 - [VICRegLoss](https://kevinmusgrave.github.io/pytorch-metric-learning/losses/
 #vicregloss)
 - Added mean reciprocal rank accuracy to [AccuracyCalculator](https://
@@ -171,15 +169,16 @@
 kevinmusgrave.github.io/pytorch-metric-learning/inference_models) | | [mlw214]
 (https://github.com/mlw214) | Added ```return_per_class``` to
 [AccuracyCalculator](https://kevinmusgrave.github.io/pytorch-metric-learning/
 accuracy_calculation/) | | [layumi](https://github.com/layumi) | [InstanceLoss]
 (https://kevinmusgrave.github.io/pytorch-metric-learning/losses/#instanceloss)
 | | [NoTody](https://github.com/NoTody) | Helped add `ref_emb` and `ref_labels`
 to the distributed wrappers. | | [ElisonSherton](https://github.com/
-ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [z1w](https://
+ElisonSherton) | Fixed an edge case in ArcFaceLoss. | | [stompsjo](https://
+github.com/stompsjo) | Improved documentation for NTXentLoss | | [z1w](https://
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
 [michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
@@ -196,13 +195,14 @@
 that has been adapted and modified from the following great open-source repos:
 - https://github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/
 incubator-mxnet/blob/master/example/gluon/embedding_learning - https://
 github.com/facebookresearch/deepcluster - https://github.com/geonm/proxy-
 anchor-loss - https://github.com/idstcv/SoftTriple - https://github.com/kunhe/
 FastAP-metric-learning - https://github.com/ronekko/deep_metric_learning -
 https://github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/
-regularface ### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/
-) for designing the logo. ## Citing this library If you'd like to cite pytorch-
-metric-learning in your paper, you can use this bibtex: ```latex @article
+regularface - https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts
+### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/) for designing
+the logo. ## Citing this library If you'd like to cite pytorch-metric-learning
+in your paper, you can use this bibtex: ```latex @article
 {Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
 and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
 {abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/SOURCES.txt` & `pytorch-metric-learning-2.3.0/src/pytorch_metric_learning.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/pytorch_metric_learning/losses/base_metric_loss_function.py
 src/pytorch_metric_learning/losses/circle_loss.py
 src/pytorch_metric_learning/losses/contrastive_loss.py
 src/pytorch_metric_learning/losses/cosface_loss.py
 src/pytorch_metric_learning/losses/cross_batch_memory.py
 src/pytorch_metric_learning/losses/fast_ap_loss.py
 src/pytorch_metric_learning/losses/generic_pair_loss.py
+src/pytorch_metric_learning/losses/histogram_loss.py
 src/pytorch_metric_learning/losses/instance_loss.py
 src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
 src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
 src/pytorch_metric_learning/losses/lifted_structure_loss.py
 src/pytorch_metric_learning/losses/manifold_loss.py
 src/pytorch_metric_learning/losses/margin_loss.py
 src/pytorch_metric_learning/losses/mixins.py
```

