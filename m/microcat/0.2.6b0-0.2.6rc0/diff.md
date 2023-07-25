# Comparing `tmp/microcat-0.2.6b0.tar.gz` & `tmp/microcat-0.2.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.2.6b0.tar", last modified: Tue Jul 25 08:48:11 2023, max compression
+gzip compressed data, was "microcat-0.2.6rc0.tar", last modified: Tue Jul 25 12:48:54 2023, max compression
```

## Comparing `microcat-0.2.6b0.tar` & `microcat-0.2.6rc0.tar`

### file list

```diff
@@ -1,80 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.230221 microcat-0.2.6b0/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.6b0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 03:24:51.000000 microcat-0.2.6b0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-25 08:48:11.230221 microcat-0.2.6b0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.6b0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.222221 microcat-0.2.6b0/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       74 2023-07-25 08:48:09.000000 microcat-0.2.6b0/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 12:02:38.000000 microcat-0.2.6b0/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.222221 microcat-0.2.6b0/microcat/bulk_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/bulk_wf/config/
--rw-r--r--   0 root         (0) root         (0)     3575 2023-07-23 14:44:49.000000 microcat-0.2.6b0/microcat/bulk_wf/config/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/bulk_wf/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.6b0/microcat/bulk_wf/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.6b0/microcat/chemistry_defs.json
--rw-r--r--   0 root         (0) root         (0)    43444 2023-07-25 08:44:25.000000 microcat-0.2.6b0/microcat/cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9780 2023-07-25 03:11:48.000000 microcat-0.2.6b0/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)     5099 2023-07-24 15:17:06.000000 microcat-0.2.6b0/microcat/prepare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.222221 microcat-0.2.6b0/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/profiles/generic/
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/cluster_config.yaml
--rw-r--r--   0 root         (0) root         (0)      408 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/config.yaml
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/key_mapping.yaml
--rwxr-xr-x   0 root         (0) root         (0)      430 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)      747 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/pbs_status.py
--rwxr-xr-x   0 root         (0) root         (0)      869 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/pbspro_status.py
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/queues.tsv.example
--rwxr-xr-x   0 root         (0) root         (0)     4928 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/scheduler.py
--rwxr-xr-x   0 root         (0) root         (0)     1755 2023-07-25 08:32:33.000000 microcat-0.2.6b0/microcat/profiles/generic/slurm_status.py
--rwxr-xr-x   0 root         (0) root         (0)    12352 2023-07-23 12:47:45.000000 microcat-0.2.6b0/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.222221 microcat-0.2.6b0/microcat/single_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/single_wf/config/
--rw-r--r--   0 root         (0) root         (0)     3587 2023-07-24 03:12:53.000000 microcat-0.2.6b0/microcat/single_wf/config/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/single_wf/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 01:32:51.000000 microcat-0.2.6b0/microcat/single_wf/envs/trimming.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/single_wf/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-21 01:32:43.000000 microcat-0.2.6b0/microcat/single_wf/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-07-21 01:32:43.000000 microcat-0.2.6b0/microcat/single_wf/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    41025 2023-07-24 05:41:37.000000 microcat-0.2.6b0/microcat/single_wf/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-07-21 01:32:43.000000 microcat-0.2.6b0/microcat/single_wf/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    39092 2023-07-24 05:43:54.000000 microcat-0.2.6b0/microcat/single_wf/rules/host.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.226221 microcat-0.2.6b0/microcat/single_wf/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.6b0/microcat/single_wf/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.6b0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py
--rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.6b0/microcat/single_wf/scripts/create_hdf5.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.6b0/microcat/single_wf/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3776 2023-07-18 02:36:09.000000 microcat-0.2.6b0/microcat/single_wf/scripts/extract_microbiome_output.R
--rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.6b0/microcat/single_wf/scripts/generate_PE_manifest_file.py
--rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.6b0/microcat/single_wf/scripts/get_ncbi_domains.py
--rwxrwxrwx   0 root         (0) root         (0)     1112 2023-07-17 14:48:20.000000 microcat-0.2.6b0/microcat/single_wf/scripts/krak2_output_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.6b0/microcat/single_wf/scripts/kraken2mpa.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.6b0/microcat/single_wf/scripts/kraken2sc.py
--rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.6b0/microcat/single_wf/scripts/microcat_bam_handle.Rmd
--rwxrwxrwx   0 root         (0) root         (0)     4624 2023-07-17 14:25:46.000000 microcat-0.2.6b0/microcat/single_wf/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15592 2023-07-17 14:25:42.000000 microcat-0.2.6b0/microcat/single_wf/scripts/sckmer_unpaired.R
--rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.6b0/microcat/single_wf/scripts/spilt_bam_by_tag.py
--rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.6b0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py
--rw-r--r--   0 root         (0) root         (0)    13281 2023-07-18 02:03:42.000000 microcat-0.2.6b0/microcat/single_wf/scripts/starsolo_tenX_auto.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.230221 microcat-0.2.6b0/microcat/single_wf/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-23 14:36:38.000000 microcat-0.2.6b0/microcat/single_wf/snakefiles/single_simulate.smk
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-23 14:44:14.000000 microcat-0.2.6b0/microcat/single_wf/snakefiles/single_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.222221 microcat-0.2.6b0/microcat/spatial_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.230221 microcat-0.2.6b0/microcat/spatial_wf/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.6b0/microcat/spatial_wf/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:48:11.222221 microcat-0.2.6b0/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-25 08:48:11.000000 microcat-0.2.6b0/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2279 2023-07-25 08:48:11.000000 microcat-0.2.6b0/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:48:11.000000 microcat-0.2.6b0/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-25 08:48:11.000000 microcat-0.2.6b0/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-25 08:48:11.000000 microcat-0.2.6b0/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-25 08:48:11.000000 microcat-0.2.6b0/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-23 14:40:32.000000 microcat-0.2.6b0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 08:48:11.230221 microcat-0.2.6b0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3134 2023-07-24 07:33:39.000000 microcat-0.2.6b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.6rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 03:24:51.000000 microcat-0.2.6rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.6rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       74 2023-07-25 12:48:48.000000 microcat-0.2.6rc0/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 12:02:38.000000 microcat-0.2.6rc0/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/bulk_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/bulk_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-07-23 14:44:49.000000 microcat-0.2.6rc0/microcat/bulk_wf/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/bulk_wf/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.6rc0/microcat/bulk_wf/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.6rc0/microcat/chemistry_defs.json
+-rw-r--r--   0 root         (0) root         (0)    43169 2023-07-25 12:48:27.000000 microcat-0.2.6rc0/microcat/cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9780 2023-07-25 03:11:48.000000 microcat-0.2.6rc0/microcat/configer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/multi_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/multi_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-07-25 08:58:34.000000 microcat-0.2.6rc0/microcat/multi_wf/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5099 2023-07-24 15:17:06.000000 microcat-0.2.6rc0/microcat/prepare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/profiles/generic/
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/cluster_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-25 12:46:50.000000 microcat-0.2.6rc0/microcat/profiles/generic/config.yaml
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/key_mapping.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      430 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      747 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/pbs_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      869 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/pbspro_status.py
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/queues.tsv.example
+-rwxr-xr-x   0 root         (0) root         (0)     4928 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/scheduler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1755 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/slurm_status.py
+-rwxr-xr-x   0 root         (0) root         (0)    12352 2023-07-23 12:47:45.000000 microcat-0.2.6rc0/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/single_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/single_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-07-24 03:12:53.000000 microcat-0.2.6rc0/microcat/single_wf/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/single_wf/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/trimming.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/single_wf/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-21 01:32:43.000000 microcat-0.2.6rc0/microcat/single_wf/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-07-21 01:32:43.000000 microcat-0.2.6rc0/microcat/single_wf/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    41025 2023-07-24 05:41:37.000000 microcat-0.2.6rc0/microcat/single_wf/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-07-21 01:32:43.000000 microcat-0.2.6rc0/microcat/single_wf/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    39092 2023-07-24 05:43:54.000000 microcat-0.2.6rc0/microcat/single_wf/rules/host.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.009124 microcat-0.2.6rc0/microcat/single_wf/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/create_hdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3776 2023-07-18 02:36:09.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1112 2023-07-17 14:48:20.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/krak2_output_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4624 2023-07-17 14:25:46.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15592 2023-07-17 14:25:42.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py
+-rw-r--r--   0 root         (0) root         (0)    13281 2023-07-18 02:03:42.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/starsolo_tenX_auto.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.009124 microcat-0.2.6rc0/microcat/single_wf/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-23 14:36:38.000000 microcat-0.2.6rc0/microcat/single_wf/snakefiles/single_simulate.smk
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-23 14:44:14.000000 microcat-0.2.6rc0/microcat/single_wf/snakefiles/single_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/spatial_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.009124 microcat-0.2.6rc0/microcat/spatial_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-07-25 08:58:46.000000 microcat-0.2.6rc0/microcat/spatial_wf/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/microcat/spatial_wf/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.6rc0/microcat/spatial_wf/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-23 14:40:32.000000 microcat-0.2.6rc0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-07-24 07:33:39.000000 microcat-0.2.6rc0/setup.py
```

### Comparing `microcat-0.2.6b0/LICENSE` & `microcat-0.2.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/PKG-INFO` & `microcat-0.2.6rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.6b0
+Version: 0.2.6rc0
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.6b0/microcat/__init__.py` & `microcat-0.2.6rc0/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/bulk_wf/config/config.yaml` & `microcat-0.2.6rc0/microcat/bulk_wf/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/chemistry_defs.json` & `microcat-0.2.6rc0/microcat/chemistry_defs.json`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/cli.py` & `microcat-0.2.6rc0/microcat/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,18 +696,17 @@
 @click.option(
     "--config",
     type=str,
     default=DEFAULT_CONFIG,
     help="Path of config.yaml",
     show_default=True
 )
-@click.argument("task",
-                default="all",
-                callback=validate_task,
-                metavar="[TASK]") 
+@click.option("--task",
+              default="all",
+              callback=validate_task)
 @click.pass_context
 def run_debug(
     ctx,
     config,
     task):
     """
     Execute the analysis workflow on debug mode.
@@ -820,37 +819,30 @@
 )
 @click.option(
     "--jobs",
     type=int,
     default=30,
     help="Job numbers",
 )
-@click.option(
-    "--unlock",
-    is_flag=True,
-    default=False,
-    help="Unlock the workflow before running",
-)
-@click.argument("task",
-                default="all",
-                callback=validate_task, metavar="[TASK]") 
+@click.option("--task",
+              default="all",
+              callback=validate_task) 
 @click.pass_context
 def run_local(
     ctx,
     config,
     cores,
     task,
     use_conda,
     list,
     conda_prefix,
     conda_create_envs_only,
     use_singularity,
     singularity_prefix,
     jobs,
-    unlock,
     wait):
     """
     Execute the analysis workflow on local computer mode
     """
     # Parse the YAML configuration file
     conf = parse_yaml(config)
     # Get the workflow type
@@ -882,16 +874,14 @@
         "--until",
         task
     ] + unknown
 
     # Add specific flags to the command based on the input arguments
     if "--touch" in unknown:
         pass
-    elif unlock:
-        pass
     elif conda_create_envs_only:
         cmd += ["--use-conda",
                 "--conda-create-envs-only",
                 "--cores 4"]
         if conda_prefix is not None:
             cmd += ["--conda-prefix", conda_prefix]
     else:
@@ -1047,35 +1037,32 @@
     help="List rule",
 )
 @click.option(
     "--singularity-prefix",
     default="",
     help="Singularity images prefix",
 )
-@click.option(
-    "--unlock",
-    is_flag=True,
-    default=False,
-    help="Unlock the workflow before running",
-)
-@click.argument("task",callback=validate_task, metavar="[TASK]") 
+# @click.argument("task",callback=validate_task, metavar="[TASK]") 
+@click.option("--task",
+              default="all",
+              callback=validate_task) 
 @click.pass_context
 def run_remote(
+    ctx,
     config,
     task,
     use_conda,
     conda_prefix,
     conda_create_envs_only,
     use_singularity,
     singularity_prefix,
     jobs,
     list,
     local_cores,
-    cluster_engine,
-    unlock
+    cluster_engine
     ):
     """
     Execute the analysis workflow on remote cluster mode
     """
 
     # Parse the YAML configuration file
     conf = parse_yaml(config)
@@ -1108,16 +1095,14 @@
         "--until",
         task
     ] + unknown
 
     # Add specific flags to the command based on the input arguments
     if "--touch" in unknown:
         pass
-    elif unlock:
-        pass
     elif conda_create_envs_only:
         cmd += ["--use-conda",
                 "--conda-create-envs-only",
                 "--cores", 
                 str(local_cores)]
         if conda_prefix is not None:
             cmd += ["--conda-prefix", conda_prefix]
@@ -1147,15 +1132,15 @@
             cluster_setting = submmit_conf['system']
             cluster_status_setting = profile_conf['cluster-status']
             if cluster_status_setting != cluster_setting + "_status.py":
                 click.secho(f"ERROR：Cluster system and Cluster system status script dont match！Please check profile.\n"
                             f"cluster: {cluster_setting}\n"
                             f"cluster-status: {cluster_status_setting}", fg="red")
             else:
-                click.echo(f"Cluster system is {cluster_setting}",fg="green")
+                click.secho(f"Cluster system is {cluster_setting}",fg="green")
                 queue_file = os.path.join(profile_path, "queue.tsv")   
                 if os.path.exists(queue_file):
                     click.secho("Snakemake will automatically selects the optimal queue for you.",fg="green")
                     df = pd.read_csv(queue_file, sep="\t")
                     click.echo(df.to_string(index=False))
                 else:
                     click.secho("Snakemake will selects the queue with config",fg="green")
```

### Comparing `microcat-0.2.6b0/microcat/configer.py` & `microcat-0.2.6rc0/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/prepare.py` & `microcat-0.2.6rc0/microcat/prepare.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/profiles/generic/key_mapping.yaml` & `microcat-0.2.6rc0/microcat/profiles/generic/key_mapping.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/profiles/generic/pbs_status.py` & `microcat-0.2.6rc0/microcat/profiles/generic/pbs_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/profiles/generic/pbspro_status.py` & `microcat-0.2.6rc0/microcat/profiles/generic/pbspro_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/profiles/generic/scheduler.py` & `microcat-0.2.6rc0/microcat/profiles/generic/scheduler.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/profiles/generic/slurm_status.py` & `microcat-0.2.6rc0/microcat/profiles/generic/slurm_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/sample.py` & `microcat-0.2.6rc0/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/config/config.yaml` & `microcat-0.2.6rc0/microcat/multi_wf/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/rules/ERCC.smk` & `microcat-0.2.6rc0/microcat/single_wf/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/rules/build.smk` & `microcat-0.2.6rc0/microcat/single_wf/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/rules/classfier.smk` & `microcat-0.2.6rc0/microcat/single_wf/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/rules/database.smk` & `microcat-0.2.6rc0/microcat/single_wf/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/rules/host.smk` & `microcat-0.2.6rc0/microcat/single_wf/rules/host.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/INVADEseq.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/create_hdf5.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/create_hdf5.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/extract_kraken_reads.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/extract_microbiome_output.R` & `microcat-0.2.6rc0/microcat/single_wf/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/generate_PE_manifest_file.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/generate_PE_manifest_file.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/get_ncbi_domains.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/krak2_output_denosing.R` & `microcat-0.2.6rc0/microcat/single_wf/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/kraken2mpa.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/kraken2sc.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/microcat_bam_handle.Rmd` & `microcat-0.2.6rc0/microcat/single_wf/scripts/microcat_bam_handle.Rmd`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/sample_denosing.R` & `microcat-0.2.6rc0/microcat/single_wf/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/sckmer_unpaired.R` & `microcat-0.2.6rc0/microcat/single_wf/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/spilt_bam_by_tag.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py` & `microcat-0.2.6rc0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/scripts/starsolo_tenX_auto.sh` & `microcat-0.2.6rc0/microcat/single_wf/scripts/starsolo_tenX_auto.sh`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat/single_wf/snakefiles/single_wf.smk` & `microcat-0.2.6rc0/microcat/single_wf/snakefiles/single_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6b0/microcat.egg-info/PKG-INFO` & `microcat-0.2.6rc0/microcat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.6b0
+Version: 0.2.6rc0
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.6b0/microcat.egg-info/SOURCES.txt` & `microcat-0.2.6rc0/microcat.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 microcat.egg-info/SOURCES.txt
 microcat.egg-info/dependency_links.txt
 microcat.egg-info/entry_points.txt
 microcat.egg-info/requires.txt
 microcat.egg-info/top_level.txt
 microcat/bulk_wf/config/config.yaml
 microcat/bulk_wf/snakefiles/bulk_wf.smk
+microcat/multi_wf/config/config.yaml
 microcat/profiles/generic/cluster_config.yaml
 microcat/profiles/generic/config.yaml
 microcat/profiles/generic/key_mapping.yaml
 microcat/profiles/generic/lsf_status.py
 microcat/profiles/generic/pbs_status.py
 microcat/profiles/generic/pbspro_status.py
 microcat/profiles/generic/queues.tsv.example
@@ -55,8 +56,9 @@
 microcat/single_wf/scripts/sample_denosing.R
 microcat/single_wf/scripts/sckmer_unpaired.R
 microcat/single_wf/scripts/spilt_bam_by_tag.py
 microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py
 microcat/single_wf/scripts/starsolo_tenX_auto.sh
 microcat/single_wf/snakefiles/single_simulate.smk
 microcat/single_wf/snakefiles/single_wf.smk
+microcat/spatial_wf/config/config.yaml
 microcat/spatial_wf/snakefiles/spatial_wf.smk
```

### Comparing `microcat-0.2.6b0/setup.py` & `microcat-0.2.6rc0/setup.py`

 * *Files identical despite different names*

