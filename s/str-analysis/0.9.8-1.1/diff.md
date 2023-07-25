# Comparing `tmp/str_analysis-0.9.8.tar.gz` & `tmp/str_analysis-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/str_analysis-0.9.8.tar", last modified: Tue Oct 18 03:27:04 2022, max compression
+gzip compressed data, was "str_analysis-1.1.tar", last modified: Tue Jul 25 15:24:51 2023, max compression
```

## Comparing `str_analysis-0.9.8.tar` & `str_analysis-1.1.tar`

### file list

```diff
@@ -1,52 +1,69 @@
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/
--rw-r--r--   0 weisburd   (502) staff       (20)    20624 2022-10-18 03:27:04.000000 str_analysis-0.9.8/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)    17525 2022-01-21 17:46:01.000000 str_analysis-0.9.8/README.md
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2022-10-18 03:27:04.000000 str_analysis-0.9.8/setup.cfg
--rw-r--r--   0 weisburd   (502) staff       (20)     2871 2022-10-18 03:25:56.000000 str_analysis-0.9.8/setup.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis/
--rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-08-15 22:19:51.000000 str_analysis-0.9.8/str_analysis/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)    56915 2022-01-21 14:15:11.000000 str_analysis-0.9.8/str_analysis/call_non_ref_pathogenic_motifs.py
--rw-r--r--   0 weisburd   (502) staff       (20)    18286 2022-06-21 13:30:13.000000 str_analysis-0.9.8/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py
--rwxr-xr-x   0 weisburd   (502) staff       (20)    19732 2022-06-21 13:30:13.000000 str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1627 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations_tests.py
--rwxr-xr-x   0 weisburd   (502) staff       (20)     9144 2022-10-10 22:03:14.000000 str_analysis-0.9.8/str_analysis/combine_json_to_tsv.py
--rwxr-xr-x   0 weisburd   (502) staff       (20)    22723 2022-10-09 22:08:17.000000 str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv.py
--rw-r--r--   0 weisburd   (502) staff       (20)    12146 2022-06-21 13:31:54.000000 str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2855 2022-01-04 00:49:53.000000 str_analysis-0.9.8/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py
--rw-r--r--   0 weisburd   (502) staff       (20)     3623 2022-02-08 18:43:09.000000 str_analysis-0.9.8/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py
--rw-r--r--   0 weisburd   (502) staff       (20)     9148 2022-06-20 04:10:53.000000 str_analysis-0.9.8/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py
--rw-r--r--   0 weisburd   (502) staff       (20)     6195 2022-01-11 03:40:51.000000 str_analysis-0.9.8/str_analysis/convert_strling_calls_to_expansion_hunter_json.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis/data/
--rw-r--r--   0 weisburd   (502) staff       (20)     2203 2022-01-04 00:49:06.000000 str_analysis-0.9.8/str_analysis/data/non_ref_motif.locus_info.json
--rw-r--r--   0 weisburd   (502) staff       (20)    31832 2021-08-20 15:25:44.000000 str_analysis-0.9.8/str_analysis/data/non_ref_motif.offtarget_regions.json.gz
--rw-r--r--   0 weisburd   (502) staff       (20)    24794 2022-06-21 16:43:40.000000 str_analysis-0.9.8/str_analysis/filter_vcf_to_STR_variants.py
--rw-r--r--   0 weisburd   (502) staff       (20)    16239 2022-06-21 14:11:35.000000 str_analysis-0.9.8/str_analysis/filter_vcf_to_STR_variants_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)    61985 2022-07-11 14:21:21.000000 str_analysis-0.9.8/str_analysis/generate_gnomad_json.py
--rw-r--r--   0 weisburd   (502) staff       (20)      915 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/generate_gnomad_json_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)    21388 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/simulate_str_expansions.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1492 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/simulate_str_expansions_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)     3614 2022-01-11 03:43:11.000000 str_analysis-0.9.8/str_analysis/trim_repeat_loci.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis/utils/
--rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-08-15 19:10:09.000000 str_analysis-0.9.8/str_analysis/utils/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)     7133 2021-10-21 15:05:22.000000 str_analysis-0.9.8/str_analysis/utils/bam_utils.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2147 2022-05-15 19:58:41.000000 str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1757 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)     4223 2019-07-28 15:41:24.000000 str_analysis-0.9.8/str_analysis/utils/dat_utils.py
--rw-r--r--   0 weisburd   (502) staff       (20)     4925 2021-12-09 03:44:25.000000 str_analysis-0.9.8/str_analysis/utils/ehdn_info_for_locus.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1157 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/export_json.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1221 2021-08-25 16:27:04.000000 str_analysis-0.9.8/str_analysis/utils/fasta_utils.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2669 2022-06-13 01:13:43.000000 str_analysis-0.9.8/str_analysis/utils/find_repeat_unit.py
--rw-r--r--   0 weisburd   (502) staff       (20)      952 2022-06-12 05:38:06.000000 str_analysis-0.9.8/str_analysis/utils/find_repeat_unit_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)     4796 2022-01-20 19:56:03.000000 str_analysis-0.9.8/str_analysis/utils/known_pathogenic_strs_tsv.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2267 2022-06-12 13:37:10.000000 str_analysis-0.9.8/str_analysis/utils/misc_utils.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1866 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1239 2021-11-19 17:05:07.000000 str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit_tests.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1628 2022-01-09 18:02:32.000000 str_analysis-0.9.8/str_analysis/utils/strling_info_for_locus.py
--rw-r--r--   0 weisburd   (502) staff       (20)     4036 2022-06-08 20:53:36.000000 str_analysis-0.9.8/str_analysis/utils/trf_runner.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/
--rw-r--r--   0 weisburd   (502) staff       (20)    20624 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)     1919 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 weisburd   (502) staff       (20)        1 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 weisburd   (502) staff       (20)      297 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/entry_points.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       77 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/requires.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       13 2022-10-18 03:27:04.000000 str_analysis-0.9.8/str_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-07-25 15:24:51.508026 str_analysis-1.1/
+-rw-r--r--   0 weisburd   (502) staff       (20)     1072 2021-06-22 19:41:51.000000 str_analysis-1.1/LICENSE
+-rw-r--r--   0 weisburd   (502) staff       (20)     4461 2023-07-25 15:24:51.507407 str_analysis-1.1/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)     3672 2023-07-07 18:06:16.000000 str_analysis-1.1/README.md
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-07-25 15:24:51.508307 str_analysis-1.1/setup.cfg
+-rw-r--r--   0 weisburd   (502) staff       (20)     3394 2023-07-25 15:24:31.000000 str_analysis-1.1/setup.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-07-25 15:24:51.461836 str_analysis-1.1/str_analysis/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-08-15 22:19:51.000000 str_analysis-1.1/str_analysis/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    21130 2023-07-24 03:37:29.000000 str_analysis-1.1/str_analysis/add_adjacent_loci_to_expansion_hunter_catalog.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    10169 2023-07-09 17:47:46.000000 str_analysis-1.1/str_analysis/add_adjacent_loci_to_expansion_hunter_catalog__manual_unittest.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    17984 2023-07-18 00:59:53.000000 str_analysis-1.1/str_analysis/annotate_EHdn_locus_outliers.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    16846 2023-07-17 18:10:55.000000 str_analysis-1.1/str_analysis/annotate_and_filter_variant_catalog.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    61327 2023-07-10 00:25:36.000000 str_analysis-1.1/str_analysis/call_non_ref_motifs.py
+-rw-r--r--   0 weisburd   (502) staff       (20)       15 2023-01-09 15:44:47.000000 str_analysis-1.1/str_analysis/check_combined_non_ref_pathogenic_motifs.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    17725 2023-07-07 19:33:53.000000 str_analysis-1.1/str_analysis/check_combined_results_tsv_for_genome_wide_repeats.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    25414 2023-04-27 17:48:29.000000 str_analysis-1.1/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py
+-rwxr-xr-x   0 weisburd   (502) staff       (20)    19719 2023-07-07 17:37:29.000000 str_analysis-1.1/str_analysis/check_trios_for_mendelian_violations.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1627 2021-10-21 15:05:22.000000 str_analysis-1.1/str_analysis/check_trios_for_mendelian_violations_tests.py
+-rwxr-xr-x   0 weisburd   (502) staff       (20)     9144 2022-10-10 22:03:14.000000 str_analysis-1.1/str_analysis/combine_json_to_tsv.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1237 2023-07-17 19:12:46.000000 str_analysis-1.1/str_analysis/combine_str_catalogs.py
+-rwxr-xr-x   0 weisburd   (502) staff       (20)    26515 2023-04-09 21:15:46.000000 str_analysis-1.1/str_analysis/combine_str_json_to_tsv.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    12378 2023-03-16 14:43:42.000000 str_analysis-1.1/str_analysis/combine_str_json_to_tsv_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    21166 2023-07-14 23:22:02.000000 str_analysis-1.1/str_analysis/convert_annotated_EHdn_locus_outliers_to_expansion_hunter_catalog.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4538 2023-05-07 21:36:57.000000 str_analysis-1.1/str_analysis/convert_bed_to_expansion_hunter_variant_catalog.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1050 2022-12-25 02:57:26.000000 str_analysis-1.1/str_analysis/convert_expansion_hunter_denovo_locus_tsv_to_bed.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2855 2022-01-04 00:49:53.000000 str_analysis-1.1/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     3623 2022-02-08 18:43:09.000000 str_analysis-1.1/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     9222 2022-12-25 03:05:35.000000 str_analysis-1.1/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     6379 2023-03-08 18:29:37.000000 str_analysis-1.1/str_analysis/convert_hipstr_vcf_to_expansion_hunter_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     6195 2022-01-11 03:40:51.000000 str_analysis-1.1/str_analysis/convert_strling_calls_to_expansion_hunter_json.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-07-25 15:24:51.472736 str_analysis-1.1/str_analysis/data/
+-rw-r--r--   0 weisburd   (502) staff       (20)     2455 2023-07-10 00:26:22.000000 str_analysis-1.1/str_analysis/data/non_ref_motif.locus_info.json
+-rw-r--r--   0 weisburd   (502) staff       (20)    31832 2021-08-20 15:25:44.000000 str_analysis-1.1/str_analysis/data/non_ref_motif.offtarget_regions.json.gz
+-rw-r--r--   0 weisburd   (502) staff       (20)    53050 2023-07-07 17:33:30.000000 str_analysis-1.1/str_analysis/filter_vcf_to_STR_variants.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    37632 2023-04-19 21:35:04.000000 str_analysis-1.1/str_analysis/filter_vcf_to_STR_variants_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    65851 2023-07-18 02:20:30.000000 str_analysis-1.1/str_analysis/generate_gnomad_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      915 2021-11-19 17:05:07.000000 str_analysis-1.1/str_analysis/generate_gnomad_json_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    15266 2023-07-05 15:33:53.000000 str_analysis-1.1/str_analysis/gnomad_sample_qc.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    21412 2023-07-07 17:37:29.000000 str_analysis-1.1/str_analysis/simulate_str_expansions.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1492 2021-10-21 15:05:22.000000 str_analysis-1.1/str_analysis/simulate_str_expansions_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     3614 2022-01-11 03:43:11.000000 str_analysis-1.1/str_analysis/trim_repeat_loci.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-07-25 15:24:51.505696 str_analysis-1.1/str_analysis/utils/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-08-15 19:10:09.000000 str_analysis-1.1/str_analysis/utils/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     7133 2021-10-21 15:05:22.000000 str_analysis-1.1/str_analysis/utils/bam_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2173 2023-05-17 14:09:04.000000 str_analysis-1.1/str_analysis/utils/canonical_repeat_unit.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1757 2021-11-19 17:05:07.000000 str_analysis-1.1/str_analysis/utils/canonical_repeat_unit_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4223 2019-07-28 15:41:24.000000 str_analysis-1.1/str_analysis/utils/dat_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4925 2021-12-09 03:44:25.000000 str_analysis-1.1/str_analysis/utils/ehdn_info_for_locus.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1157 2021-11-19 17:05:07.000000 str_analysis-1.1/str_analysis/utils/export_json.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1221 2021-08-25 16:27:04.000000 str_analysis-1.1/str_analysis/utils/fasta_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1743 2023-07-09 22:21:06.000000 str_analysis-1.1/str_analysis/utils/file_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    17553 2023-04-19 13:16:28.000000 str_analysis-1.1/str_analysis/utils/find_repeat_unit.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    19748 2023-07-11 21:33:01.000000 str_analysis-1.1/str_analysis/utils/find_repeat_unit_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     7734 2023-07-23 18:56:36.000000 str_analysis-1.1/str_analysis/utils/get_adjacent_repeats.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     9005 2023-07-09 21:22:39.000000 str_analysis-1.1/str_analysis/utils/gtf_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4237 2023-07-11 21:33:01.000000 str_analysis-1.1/str_analysis/utils/gtf_utils__manual_unittest.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4796 2022-01-20 19:56:03.000000 str_analysis-1.1/str_analysis/utils/known_pathogenic_strs_tsv.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2267 2022-06-12 13:37:10.000000 str_analysis-1.1/str_analysis/utils/misc_utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1866 2021-11-19 17:05:07.000000 str_analysis-1.1/str_analysis/utils/most_frequent_repeat_unit.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1239 2021-11-19 17:05:07.000000 str_analysis-1.1/str_analysis/utils/most_frequent_repeat_unit_tests.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1628 2022-01-09 18:02:32.000000 str_analysis-1.1/str_analysis/utils/strling_info_for_locus.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     4049 2022-11-03 20:11:33.000000 str_analysis-1.1/str_analysis/utils/trf_runner.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-07-25 15:24:51.469759 str_analysis-1.1/str_analysis.egg-info/
+-rw-r--r--   0 weisburd   (502) staff       (20)     4461 2023-07-25 15:24:51.000000 str_analysis-1.1/str_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)     2776 2023-07-25 15:24:51.000000 str_analysis-1.1/str_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)        1 2023-07-25 15:24:51.000000 str_analysis-1.1/str_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      784 2023-07-25 15:24:51.000000 str_analysis-1.1/str_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      154 2023-07-25 15:24:51.000000 str_analysis-1.1/str_analysis.egg-info/requires.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       13 2023-07-25 15:24:51.000000 str_analysis-1.1/str_analysis.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `str_analysis-0.9.8/setup.py` & `str_analysis-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,60 +3,62 @@
 
 from setuptools import find_packages, setup
 from setuptools.command.build_py import build_py
 
 with open("README.md", "rt") as fh:
     long_description = fh.read()
 
+with open("requirements.txt", "rt") as f:
+    requirements = [r.strip() for r in f.readlines()]
+
+
 class CoverageCommand(build_py):
     """Run all unittests and generate a coverage report."""
-
     def run(self):
-        """Run the coverage command"""
         os.system("python3 -m coverage run --omit='*/site-packages/*,*tests.py,setup.py,*__init__.py' ./setup.py test "
                   "&& python3 -m coverage html --include=*.py "
                   "&& open htmlcov/index.html")
 
 
 class PublishCommand(build_py):
     """Publish package to PyPI"""
     def run(self):
-        """Publish"""
         os.system("rm -rf dist")
         os.system("python3 setup.py sdist"
                   "&& python3 setup.py bdist_wheel"
-                  "&& twine upload dist/*whl dist/*gz")
-
-
-with open("requirements.txt", "rt") as f:
-    requirements = [r.strip() for r in f.readlines()]
+                  "&& python3 -m twine upload dist/*whl dist/*gz")
 
 
 def test_suite():
     """Discover unittests"""
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover('str_analysis', pattern='*tests.py')
     return test_suite
 
 
 setup(
     name='str_analysis',
-    version="0.9.8",
-    description="Utilities  short tandem repeats (STRs)",
+    version="1.1",
+    description="Utilities for analyzing short tandem repeats (STRs)",
     install_requires=requirements,
     cmdclass={
         'coverage': CoverageCommand,
         'publish': PublishCommand,
     },
     entry_points = {
         'console_scripts': [
-            'call_non_ref_pathogenic_motifs = str_analysis.call_non_ref_pathogenic_motifs:main',
-            'combine_json_to_tsv = str_analysis.combine_json_to_tsv:main',
-            'combine_str_json_to_tsv = str_analysis.combine_str_json_to_tsv:main',
+            'call_non_ref_motifs = str_analysis.call_non_ref_motifs:main',
+            'filter_vcf_to_STR_variants = str_analysis.filter_vcf_to_STR_variants:main',
+            'add_adjacent_loci_to_expansion_hunter_catalog = str_analysis.add_adjacent_loci_to_expansion_hunter_catalog:main',
+            'check_trios_for_mendelian_violations = str_analysis.check_trios_for_mendelian_violations:main',
             'simulate_str_expansions = str_analysis.simulate_str_expansions:main',
+            'annotate_EHdn_locus_outliers = str_analysis.annotate_EHdn_locus_outliers:main',
+            'convert_annotated_EHdn_locus_outliers_to_expansion_hunter_catalog = str_analysis.convert_annotated_EHdn_locus_outliers_to_expansion_hunter_catalog:main',
+            'combine_str_json_to_tsv = str_analysis.combine_str_json_to_tsv:main',
+            'combine_json_to_tsv = str_analysis.combine_json_to_tsv:main',
         ],
     },
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=["str_analysis", "str_analysis.utils"],
     data_files=[
         ('data', ['str_analysis/data/non_ref_motif.offtarget_regions.json.gz']),
```

### Comparing `str_analysis-0.9.8/str_analysis/call_non_ref_pathogenic_motifs.py` & `str_analysis-1.1/str_analysis/call_non_ref_motifs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from str_analysis.utils.strling_info_for_locus import parse_strling_info_for_locus
+from str_analysis.utils.file_utils import open_file
 
 DESCRIPTION = """This script takes a bam or cram file and determines which motifs are present at known pathogenic STR 
 loci (such as RFC1, BEAN1, DAB1, etc.) where several motifs are known to segregate in the population. It then 
 optionally runs ExpansionHunterDenovo, ExpansionHunter, and/or STRling and gathers relevant fields from their outputs
 for comparison and further evidence. It can also then run REViewer to generate read visualization images based on the
 ExpansionHunter outputs. Finally it generates a json file per locus that contains all collected information as 
 well as a "call" field indicating whether pathogenic motifs were detected.
@@ -18,20 +18,19 @@
 import pkgutil
 import re
 import pandas as pd
 from pprint import pformat, pprint
 
 import pysam
 
-from str_analysis.utils.canonical_repeat_unit import \
-    compute_canonical_motif
+from str_analysis.utils.canonical_repeat_unit import compute_canonical_motif
 from str_analysis.utils.ehdn_info_for_locus import parse_ehdn_info_for_locus
 from str_analysis.utils.misc_utils import parse_interval
-from str_analysis.utils.most_frequent_repeat_unit import \
-    compute_most_frequent_repeat_unit
+from str_analysis.utils.most_frequent_repeat_unit import compute_most_frequent_repeat_unit
+from str_analysis.utils.strling_info_for_locus import parse_strling_info_for_locus
 
 LOCUS_INFO = json.loads(pkgutil.get_data(__name__, "data/non_ref_motif.locus_info.json"))
 """
 Dictionary with info about each STR locus - including the reference coordinates, known benign and pathogenic motifs,
 as well as whether to use off-target regions by default when running ExpansionHunter.
 """
 
@@ -77,25 +76,26 @@
     "GRCh38": "38", "hg38": "38", "38": "38",
 }
 
 
 PATHOGENIC_MOTIF_CALL = "PATHOGENIC MOTIF"
 BENIGN_MOTIF_CALL = "BENIGN MOTIF"
 UNCERTAIN_SIG_CALL = "MOTIF OF UNCERTAIN SIGNIFICANCE"
-
+REF_MOTIF_CALL = "REFERENCE MOTIF"
 NO_CALL = "NO CALL (no motif has sufficient read support)"
 
 PATHOGENIC_PATHOGENIC_CALL = f"{PATHOGENIC_MOTIF_CALL} / {PATHOGENIC_MOTIF_CALL}"
 BENIGN_BENIGN_CALL = f"{BENIGN_MOTIF_CALL} / {BENIGN_MOTIF_CALL}"
 UNCERTAIN_SIG_UNCERTAIN_SIG_CALL = f"{UNCERTAIN_SIG_CALL} / {UNCERTAIN_SIG_CALL}"
+REF_REF_CALL = f"{REF_MOTIF_CALL} / {REF_MOTIF_CALL}"
 
 BENIGN_PATHOGENIC_CALL = f"{BENIGN_MOTIF_CALL} / {PATHOGENIC_MOTIF_CALL}"
 PATHOGENIC_UNCERTAIN_SIG_CALL = f"{PATHOGENIC_MOTIF_CALL} / {UNCERTAIN_SIG_CALL}"
 BENIGN_UNCERTAIN_SIG_CALL = f"{BENIGN_MOTIF_CALL} / {UNCERTAIN_SIG_CALL}"
-
+REF_UNCERTAIN_SIG_CALL = f"{REF_MOTIF_CALL} / {UNCERTAIN_SIG_CALL}"
 
 def parse_args():
     """Parse command-line args, perform basic validation, and then return the args object."""
 
     p = argparse.ArgumentParser(description=DESCRIPTION)
     p.add_argument("-g", "--genome-version", help="Reference genome version",
                    choices=GENOME_VERSION_ALIASES.keys(), required=True)
@@ -135,18 +135,21 @@
     grp.add_argument("--run-reviewer", action="store_true", help="Run the REViewer tool to visualize "
         "ExpansionHunter output. --run-expansion-hunter must also be specified.")
     grp.add_argument("--run-reviewer-for-pathogenic-calls", action="store_true", help="Run the REViewer tool to "
         f"visualize ExpansionHunter output only when this script calls a sample as having {PATHOGENIC_PATHOGENIC_CALL}."
         " --run-expansion-hunter must also be specified.")
 
     grp = p.add_mutually_exclusive_group(required=True)
-    grp.add_argument("--all-loci", action="store_true", help="Generate calls for all these loci: " + ", ".join(LOCUS_INFO.keys()))
-    grp.add_argument("-l", "--locus", action="append", help="Generate calls for this specific locus. "
-        "This argument can be specified more than once to call multiple loci.",
-        choices=LOCUS_INFO.keys())
+    grp.add_argument("--loci-from-variant-catalog", help="Path of ExpansionHunter variant catalog file. This script "
+        "will check for non-reference motifs at all of these loci. This can be a local path or a gs:// path.")
+    grp.add_argument("--known-loci", action="store_true", help="Generate calls for loci known to have non-reference "
+                                                               "motifs: " + ", ".join(LOCUS_INFO.keys()))
+
+    p.add_argument("-l", "--locus", action="append", help="Generate calls for this specific locus id. "
+        "This argument can be specified more than once to call multiple loci.")
 
     p.add_argument("-v", "--verbose", action="store_true", help="Print detailed log messages.")
     p.add_argument("bam_or_cram_path", help="bam or cram path.")
 
     args = p.parse_args()
     args.genome_version = GENOME_VERSION_ALIASES[args.genome_version]
 
@@ -800,46 +803,51 @@
             relevant_bases = read_sequence[start_offset:end_offset]
             if len(relevant_bases) >= motif_size:
                 overlapping_sequences.append(relevant_bases)
 
     return overlapping_sequences, left_flank_n_well_aligned_bases, right_flank_n_well_aligned_bases
 
 
-def compute_final_call(n_total_well_supported_motifs, n_pathogenic_motifs, n_benign_motifs):
+def compute_final_call(n_ref_alleles, n_total_well_supported_alleles, n_pathogenic_alleles, n_benign_alleles):
     """Decide which combination of motifs is supported by the data.
 
     NOTE: there's no attempt to determine the size of the expansion and whether it's in the pathogenic range.
 
     Return:
         str: a string such as "BENIGN MOTIF / PATHOGENIC MOTIF" indicating which motifs were detected
     """
 
-    if n_total_well_supported_motifs == 0:
+    if n_total_well_supported_alleles == 0:
         final_call = NO_CALL
-    elif n_pathogenic_motifs == n_total_well_supported_motifs:
+    elif n_pathogenic_alleles == n_total_well_supported_alleles:
         # Reads support only known pathogenic motif(s)
         final_call = PATHOGENIC_PATHOGENIC_CALL
-    elif n_benign_motifs == n_total_well_supported_motifs:
+    elif n_benign_alleles == n_total_well_supported_alleles:
         # Reads support only known benign motif(s)
         final_call = BENIGN_BENIGN_CALL
-    elif n_benign_motifs == 0 and n_pathogenic_motifs == 0:
+    elif n_benign_alleles == 0 and n_pathogenic_alleles == 0:
         # Reads support one or more non-reference motifs of unknown significance
-        final_call = UNCERTAIN_SIG_UNCERTAIN_SIG_CALL
-    elif n_benign_motifs > 0 and n_pathogenic_motifs > 0:
+        if n_total_well_supported_alleles == n_ref_alleles:
+            final_call = REF_REF_CALL
+        elif n_ref_alleles > 0:
+            final_call = REF_UNCERTAIN_SIG_CALL
+        else:
+            final_call = UNCERTAIN_SIG_UNCERTAIN_SIG_CALL
+    elif n_benign_alleles > 0 and n_pathogenic_alleles > 0:
         # Reads support one known benign motif and one pathogenic motif
         final_call = BENIGN_PATHOGENIC_CALL
-    elif n_pathogenic_motifs > 0:
+    elif n_pathogenic_alleles > 0:
         # Reads support one pathogenic motif and at least one other motif of unknown significance
         final_call = PATHOGENIC_UNCERTAIN_SIG_CALL
-    elif n_benign_motifs > 0:
+    elif n_benign_alleles > 0:
         # Reads support one known benign motif and at least one other motif of unknown significance
         final_call = BENIGN_UNCERTAIN_SIG_CALL
     else:
-        raise Exception(f"Unexpected state when n_total_well_supported_motifs={n_total_well_supported_motifs}, "
-                        f"n_pathogenic_motifs={n_pathogenic_motifs}, n_benign_motifs={n_benign_motifs}")
+        raise Exception(f"Unexpected state when n_total_well_supported_alleles={n_total_well_supported_alleles}, "
+                        f"n_pathogenic_alleles={n_pathogenic_alleles}, n_benign_alleles={n_benign_alleles}")
 
     return final_call
 
 
 def process_offtarget_regions(
     motif,
     motif_number,
@@ -887,42 +895,45 @@
             read_count_with_offtargets * normalize_to_coverage / flank_coverage_mean if flank_coverage_mean > 0 else 0,
     })
 
 
 def process_locus(
         locus_id,
         args,
+        locus_info=LOCUS_INFO,
         strling_genotype_df=None,
         expansion_hunter_denovo_json=None,
         normalize_to_coverage=NORMALIZE_TO_COVERAGE,
         min_read_support=MIN_READ_SUPPORT):
     """Compute results for a single locus and write them to a json file.
 
     Args:
         locus_id (str): Locus id
         args (object): Command-line args from argparse.
+        locus_info (dict): nested dictionary with info about each locus. See data/non_ref_motif.locus_info.json for the schema.
         strling_genotype_df (pd.DataFrame): optional parsed STRling genotypes table
         expansion_hunter_denovo_json (dict): optional parsed ExpansionHunterDenovo profile json
         normalize_to_coverage (int): Normalize to this mean coverage. For example = 40 means normalize to 40x coverage.
         min_read_support (int): Ignore motifs supported by fewer than this many reads.
     """
-    locus_coords_1based = LOCUS_INFO[locus_id]["LocusCoords_1based"][args.genome_version]
+    locus_coords_1based = locus_info[locus_id]["LocusCoords_1based"][args.genome_version]
     locus_chrom, start_1based, end_1based = parse_interval(locus_coords_1based)
     locus_start_0based = start_1based - 1
     locus_end = end_1based
-    use_offtarget_regions = args.use_offtarget_regions or LOCUS_INFO[locus_id]["UseOfftargetRegions"]
+    use_offtarget_regions = args.use_offtarget_regions or locus_info[locus_id]["UseOfftargetRegions"]
 
-    known_pathogenic_motifs = list(map(compute_canonical_motif, LOCUS_INFO[locus_id]["Motifs"]["PATHOGENIC"]))
-    known_benign_motifs = list(map(compute_canonical_motif, LOCUS_INFO[locus_id]["Motifs"]["BENIGN"]))
+    canonical_reference_motif = compute_canonical_motif(locus_info[locus_id]["Motifs"]["REFERENCE"])
+    reference_motif_size = len(canonical_reference_motif)
 
-    pathogenic_motif_size = len(known_pathogenic_motifs[0])
+    known_pathogenic_motifs = list(map(compute_canonical_motif, locus_info[locus_id]["Motifs"].get("PATHOGENIC", [])))
+    known_benign_motifs = list(map(compute_canonical_motif, locus_info[locus_id]["Motifs"].get("BENIGN", [])))
 
     # Process bam/cram
     overlapping_sequences, left_flank_n_well_aligned_bases, right_flank_n_well_aligned_bases = process_reads_in_locus(
-        args.bam_or_cram_path, args.reference_fasta, locus_chrom, locus_start_0based, locus_end, pathogenic_motif_size)
+        args.bam_or_cram_path, args.reference_fasta, locus_chrom, locus_start_0based, locus_end, reference_motif_size)
 
     locus_results_json = {}
     left_flank_coverage = left_flank_n_well_aligned_bases / FLANK_SIZE
     right_flank_coverage = right_flank_n_well_aligned_bases / FLANK_SIZE
     locus_results_json.update({
         "sample_id": args.sample_id,
         "locus_id": locus_id,
@@ -935,18 +946,19 @@
     # Compute the motif(s) found in the reads and how many times each one occurs
     motif_to_read_count = collections.defaultdict(int)
     motif_to_n_occurrences = collections.defaultdict(int)
     canonical_motif_to_read_count = collections.defaultdict(int)
     canonical_motif_to_n_occurrences = collections.defaultdict(int)
     if locus_id == "RFC1":
         # In gnomAD, EHdn sometimes finds 6bp repeat units (eg. AAAGGG), so check for those as well
-        motif_sizes_to_check = [pathogenic_motif_size, pathogenic_motif_size + 1]
+        motif_sizes_to_check = [reference_motif_size, reference_motif_size + 1]
     else:
         motif_sizes_to_check = {len(m) for m in known_pathogenic_motifs + known_benign_motifs}
-
+        motif_sizes_to_check.add(reference_motif_size)
+        
     for overlapping_sequence in overlapping_sequences:
         for motif_size in motif_sizes_to_check:
             if len(overlapping_sequence) < motif_size:
                 continue
 
             motif, count = compute_most_frequent_repeat_unit(
                 overlapping_sequence,
@@ -955,15 +967,15 @@
                 min_fraction_bases_covered=MIN_FRACTION_OF_BASES_COVERED)
 
             if args.verbose:
                 if motif:
                     print(f"Found {motif} occurs {count}x in read bases that "
                           f"overlap the {locus_id} locus: {overlapping_sequence}")
                 else:
-                    if motif_size == pathogenic_motif_size:
+                    if motif_size == reference_motif_size:
                         print(f"Didn't find a consistent {motif_size}bp repeat unit in read bases "
                               f"that overlap the {locus_id} locus: {overlapping_sequence}")
 
             if motif is not None:
                 canonical_motif = compute_canonical_motif(motif)
                 motif_to_read_count[motif] += 1
                 motif_to_n_occurrences[motif] += count
@@ -997,58 +1009,65 @@
         well_supported_canonical_motifs.add(canonical_motif)
         well_supported_motifs.append(motif)
 
     # Select the repeat unit(s) with the most read support
     well_supported_motifs.sort(key=lambda motif: motif_to_n_occurrences[motif], reverse=True)
     selected_motifs = well_supported_motifs[:2]
 
-    # Sort then into BENIGN .. PATHOGENIC .. UNCERTAIN SIGNIFICANCE to match the order in the "call" output field
+    # Sort them into BENIGN .. PATHOGENIC .. UNCERTAIN SIGNIFICANCE to match the order in the "call" output field
     selected_motifs = sorted(selected_motifs, key=lambda motif:
         1 if compute_canonical_motif(motif) in known_benign_motifs else
         2 if compute_canonical_motif(motif) in known_pathogenic_motifs else
         3)
 
     flank_coverage_mean = (left_flank_coverage + right_flank_coverage) / 2.0
-    n_pathogenic_motifs = 0
-    n_benign_motifs = 0
-    n_total_well_supported_motifs = 0
+    n_pathogenic_alleles = 0
+    n_benign_alleles = 0
+    n_total_well_supported_alleles = 0
+    
+    n_ref_alleles = 0  # for known motifs/loci, a motif can be counted as both reference and benign
     for i in 0, 1:
         motif_number = i + 1
         if len(selected_motifs) <= i:
             continue
 
-        n_total_well_supported_motifs += 1
+        n_total_well_supported_alleles += 1
         motif = selected_motifs[i]
         canonical_motif = compute_canonical_motif(motif)
         if canonical_motif in known_pathogenic_motifs:
-            n_pathogenic_motifs += 1
+            n_pathogenic_alleles += 1
         elif canonical_motif in known_benign_motifs:
-            n_benign_motifs += 1
+            n_benign_alleles += 1
 
+        if canonical_motif == canonical_reference_motif:
+            n_ref_alleles += 1
+            
         read_count = canonical_motif_to_read_count.get(canonical_motif)
         n_occurrences = canonical_motif_to_n_occurrences.get(canonical_motif)
 
         locus_results_json.update({
             f"motif{motif_number}_repeat_unit": motif,
             f"motif{motif_number}_canonical_repeat_unit": canonical_motif,
             f"motif{motif_number}_read_count": read_count,
             f"motif{motif_number}_normalized_read_count":
                 read_count * normalize_to_coverage / flank_coverage_mean if flank_coverage_mean > 0 else 0,
             f"motif{motif_number}_n_occurrences": n_occurrences,
+            f"motif{motif_number}_is_reference_motif": canonical_motif == canonical_reference_motif,
         })
 
         if use_offtarget_regions:
             process_offtarget_regions(motif, motif_number, read_count, flank_coverage_mean, args, locus_results_json)
 
-    final_call = compute_final_call(n_total_well_supported_motifs, n_pathogenic_motifs, n_benign_motifs)
+    final_call = compute_final_call(n_ref_alleles, n_total_well_supported_alleles, n_pathogenic_alleles, n_benign_alleles)
 
     locus_results_json.update({
-        "n_total_well_supported_motifs": n_total_well_supported_motifs,
-        "n_benign_motifs": n_benign_motifs,
-        "n_pathogenic_motifs": n_pathogenic_motifs,
+        "n_reference_alleles": n_ref_alleles,
+        "n_total_well_supported_alleles": n_total_well_supported_alleles,
+        "n_benign_alleles": n_benign_alleles,
+        "n_pathogenic_alleles": n_pathogenic_alleles,
         "call": final_call,
     })
 
     print(f"Final call: {final_call}")
 
     # Process STRling results
     if strling_genotype_df is not None:
@@ -1177,25 +1196,75 @@
     expansion_hunter_denovo_json = None
     if args.expansion_hunter_denovo_profile:
         print(f"Parsing {args.expansion_hunter_denovo_profile}")
         open_func = gzip.open if args.expansion_hunter_denovo_profile.endswith("gz") else open
         with open_func(args.expansion_hunter_denovo_profile, "rt") as f:
             expansion_hunter_denovo_json = json.load(f)
 
-    if args.locus:
-        loci = args.locus
-    elif args.all_loci:
-        loci = LOCUS_INFO.keys()
-    else:
-        raise ValueError("Must specify --locus or --all-loci")
+    if args.known_loci:
+        locus_info = LOCUS_INFO
+    elif args.loci_from_variant_catalog:
+        # convert variant catalog to locus_info format
+        with open_file(args.loci_from_variant_catalog) as f:
+            loci_from_variant_catalog = json.load(f)
+
+        locus_info = {}
+        for i, locus in enumerate(loci_from_variant_catalog):
+            reference_motifs = []
+            locus_structure = locus["LocusStructure"]
+            for locus_structure_part in locus_structure.split(")"):
+                reference_motif = locus_structure_part.strip("()*+")
+                reference_motifs.append(reference_motif)
+
+            if len(reference_motifs) > 1:
+                if "MainReferenceRegion" not in locus:
+                    print(f"WARNING: Skipping locus #{i+1} with LocusStructure {locus_structure}. This script only "
+                          f"allows loci with a ReferenceRegion list if a 'MainReferenceRegion' key is also provided.")
+                    continue
+
+                main_reference_region = locus["MainReferenceRegion"]
+                variant_ids = locus.get("VariantId", [])
+                reference_regions = locus.get("ReferenceRegion", [])
+                if len(reference_motifs) != len(reference_regions):
+                    raise ValueError(f"LocusStructure {locus_structure} doesn't match the # of ReferenceRegions at "
+                                     f"locus {locus.get('LocusId')} in {args.loci_from_variant_catalog} record #{i+1}")
+
+                if len(variant_ids) != len(reference_regions):
+                    raise ValueError(f"The number of VariantIds doesn't match the number of ReferenceRegions for "
+                                     f"locus {locus.get('LocusId')} in {args.loci_from_variant_catalog} record #{i+1}")
+
+                for reference_motif, variant_id, ref_region in zip(reference_motifs, variant_ids, reference_regions):
+                    if reference_region == locus["MainReferenceRegion"]:
+                        locus_id = variant_id
+                        reference_region = ref_region
+                        break
+                else:
+                    raise ValueError(f"MainReferenceRegion {main_reference_region} doesn't match any of the entries in "
+                                     f"the ReferenceRegion list {reference_regions} for locus {locus.get('LocusId')} "
+                                     f"in {args.loci_from_variant_catalog} record #{i+1}")
+
+            else:
+                locus_id = locus["LocusId"]
+                reference_region = locus["ReferenceRegion"]
+
+            if locus_id in locus_info:
+                raise ValueError(f"Non-unique locus id {locus_id} in {args.loci_from_variant_catalog} record #{i+1}")
+
+            chrom, start_0based, end_1based = parse_interval(reference_region)
+            locus_info[locus_id] = {
+                "LocusCoords_1based": {args.genome_version: f"{chrom}:{start_0based + 1}-{end_1based}"},
+                "Motifs": {"REFERENCE": reference_motif},
+                "UseOfftargetRegions": False,
+            }
 
-    for locus_id in loci:
+    for locus_id in args.locus or locus_info.keys():
         print(f"Processing {locus_id} in {args.bam_or_cram_path}")
         process_locus(
             locus_id,
             args,
+            locus_info=locus_info,
             strling_genotype_df=strling_genotype_df,
             expansion_hunter_denovo_json=expansion_hunter_denovo_json)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `str_analysis-0.9.8/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py` & `str_analysis-1.1/str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-"""This script makes it easier to manually look through genotypes of many samples at known pathogenic loci and
-check for samples that may be expanded into the pathogenic range.
-
-The script's main input file is a .tsv file generated by the combine_str_json_to_tsv.py script which
-combines multiple ExpansionHunter .json output files into a single .tsv table. It's assumed that this input .tsv will
-have at least the columns listed below. One way to add these Sample_* and VariantCatalog_* columns is to run
-combine_str_json_to_tsv.py with the --sample-metadata and the --variant-catalog args.
+"""
+The script takes a .tsv file generated by the combine_str_json_to_tsv.py script for ExpansionHunter calls at
+known disease-associated loci.
+It then prints out the subset of rows that might represent pathogenic expansions and should be reviewed in more detail.
 
 The input .tsv must have at least these input columns:
 
     "LocusId", "SampleId", "Sample_affected", "Sample_sex",
     "Num Repeats: Allele 1", "Num Repeats: Allele 2", "CI end: Allele 1", "CI end: Allele 2",
 
+One way to add the  Sample_* and VariantCatalog_* columns is to run combine_str_json_to_tsv.py with the
+--sample-metadata and  the --variant-catalog args. Variant catalogs can be taken from the variant_catalogs directory in
+this github repo.
+
+This script then prints out a table for each locus with sample genotypes sorted by most expanded to least expanded.
+It can print all sample genotypes, or set a cut-off based on the known pathogenic threshold, or alternatively, by
+print all affected individuals that are more expanded than some user-defined number of unaffected individuals.
+It also takes into account locus inheritance - for example, printing 2 separate tables (males, females) for X-linked
+recessive loci.
 """
 
 import argparse
 import os
 import subprocess
 from ast import literal_eval
 
@@ -37,360 +43,532 @@
     "RepeatUnit",
     "VariantId",
 
     "Sample_analysis_status",
     "Sample_coded_phenotype",
     "Sample_phenotypes",
     "Sample_genome_version",
-    "Sample_sample_type",
 
     "VariantCatalog_Inheritance",
     "VariantCatalog_Diseases",
 
     "Genotype",
     "GenotypeConfidenceInterval",
 ]
 
 GNOMAD_STR_TABLE_PATH = "https://gnomad-public-us-east-1.s3.amazonaws.com/release/3.1.3/tsv/gnomAD_STR_genotypes__2022_01_20.tsv.gz"
 
+SEPARATOR_STRING = "---"
 
 def run(command):
     print(command)
     subprocess.check_call(command, shell=True)
 
 
-def main():
+def parse_args():
     p = argparse.ArgumentParser()
-    grp = p.add_mutually_exclusive_group(required=True)
+    grp = p.add_argument_group()
     grp.add_argument("--use-affected", action="store_true", help="Use affected status to determine which samples to "
-        "include in the output for each locus. Only include those affected samples that have longer expansions than "
-        "the top 10 unaffected samples (adjustsable by --max-n-unaffected).")
+        "include in the output for each locus. Only include those affected samples that have larger expansions than "
+        "the top N unaffected samples (adjustsable by --max-n-unaffected).")
     grp.add_argument("--use-thresholds", action="store_true", help="Use known pathogenic thresholds to determine which "
         "samples to include in the output for each locus. All samples with expansions above the pathogenic threshold "
         "will be included.")
     p.add_argument("-n", "--max-rows", type=int, default=10000000, help="Limit the max number of samples to include in "
         "the output for each locus.")
     p.add_argument("--max-n-unaffected", type=int, default=10, help="After this many unaffected samples are "
         "encountered with genotypes above a particular expansion size at locus, all samples (affected or unaffected) "
         "that have smaller expansions at that locus will be ignored")
     p.add_argument("--use-gnomad", action="store_true", help="Include samples from the gnomAD v3.1 STR release"
         "@ https://gnomad.broadinstitute.org/downloads#v3-short-tandem-repeats")
+
     p.add_argument("-l", "--locus", action="append", help="If specified, only these locus ids will be processed")
     p.add_argument("--highlight-samples", nargs="*", help="If specified, this can be the path of a text file that "
-        "contains sample ids (one per line) or just 1 or more sample ids listed on the commandline - one per line")
+        "contains sample ids (one per line) or just 1 or more sample ids listed on the commandline")
+    p.add_argument("--truth-samples", help="If specified, this can be the path of a table that contains two columns: "
+        "sample id and locus id. The script will then mark each sample at that locus to indicate that it's a truth "
+        "sample")
+    p.add_argument("--previously-seen-samples", help="If specified, this can be the path of a table that contains "
+        "two columns: sample id and locus id. The script will then mark each sample at that locus to "
+        "indicate that it's already been evaluated")
+    p.add_argument("--previously-diagnosed-loci", nargs="*", help="If specified, this can be the path of a "
+        "text file that contains locus ids (one per line) or just 1 or more locus ids listed on the commandline. These "
+        "loci will be marked as having been previously diagnosed using short-read sequencing data.")
     p.add_argument("combined_tsv_path", nargs="+", help="Path of combined ExpansionHunter .tsv table generated by the "
         "combine_str_json_to_tsv.py script. It's assumed that combine_str_json_to_tsv.py "
         "was run with --sample-metadata and --variant-catalog args to add sample-level and locus-level metadata columns")
 
+    p.add_argument("--results-path", help="Export a .tsv table of rows that pass thresholds to this path",
+        default="pathogenic_and_intermediate_results.tsv")
+
     # Parse and validate command-line args + read in the combined table(s) from the given command_tsv_path(s)
     args = p.parse_args()
 
-    if args.use_gnomad:
-        print("Loading gnomAD STR table...")
-        gnomad_df = pd.read_table(GNOMAD_STR_TABLE_PATH, usecols=[
-                "Id",
-                "LocusId",
-                "ReferenceRegion",
-                "Motif",
-                "IsAdjacentRepeat",
-                "Sex",
-                "Allele1",
-                "Allele2",
-                "Genotype",
-                "GenotypeConfidenceInterval",
-            ],
-            dtype={
-                "Id": str,
-                "Sex": str,
-                "Allele1": str,
-                "Allele2": str,
-                "GenotypeConfidenceInterval": str,
-                "IsAdjacentRepeat": bool,
-            },
-        )
-        gnomad_df = gnomad_df[~gnomad_df["IsAdjacentRepeat"]]
-        print(f"Processing {len(gnomad_df)} gnomAD table rows...")
-        for column_name, value in [
-            ("Sample_genome_version", "38"),
-            ("Sample_sample_type", "WGS"),
-            ("Sample_affected", "Not Affected"),
-        ]:
-            gnomad_df.loc[:, column_name] = value
-
-        gnomad_df.loc[:, "Id"] = "gnomAD:" + gnomad_df["Id"]
-        gnomad_df.loc[:, "VariantId"] = gnomad_df["LocusId"]
-
-        gnomad_df.loc[:, ("CI1", "CI2")] = gnomad_df["GenotypeConfidenceInterval"].str.split("/", expand=True)
-        gnomad_df.loc[:, "CI1"] = gnomad_df["CI1"].fillna("")
-        gnomad_df.loc[:, "CI2"] = gnomad_df["CI2"].fillna("")
-        gnomad_df.loc[:, ("CI start: Allele 1", "CI end: Allele 1")] = gnomad_df["CI1"].str.split("-", expand=True)
-        gnomad_df.loc[:, ("CI start: Allele 2", "CI end: Allele 2")] = gnomad_df["CI2"].str.split("-", expand=True)
-        gnomad_df.drop(columns=["CI1", "CI2", "CI start: Allele 1", "CI start: Allele 2"], inplace=True)
-        gnomad_df.rename({
-            "Id": "SampleId",
-            "Sex": "Sample_sex",
-            "Allele1": "Num Repeats: Allele 1",
-            "Allele2": "Num Repeats: Allele 2",
-            "Motif": "RepeatUnit",
-        }, axis="columns", inplace=True)
+    for combined_tsv_path in args.combined_tsv_path:
+        if not os.path.isfile(combined_tsv_path):
+            p.error(f"{combined_tsv_path} not found")
 
+    if not args.use_affected and not args.use_thresolds:
+        p.error("Must specify --use-thresholds or --use-affected")
 
-    highlight_sample_ids = []
-    if args.highlight_samples:
-        for h in args.highlight_samples:
-            if os.path.isfile(h):
-                with open(h, "rt") as f:
-                    sample_ids_list = [s.strip() for s in f.readlines()]
-                print(f"Read {len(sample_ids_list)} sample ids to highlight from: {h}")
-                highlight_sample_ids.extend(sample_ids_list)
-            else:
-                highlight_sample_ids.append(h)
+    return args
 
-        print(f"Will highlight {len(highlight_sample_ids)} sample ids: {highlight_sample_ids}")
-        
+
+def load_gnomad_df():
+    print("Loading gnomAD STR table...")
+    gnomad_df = pd.read_table(GNOMAD_STR_TABLE_PATH, usecols=[
+        "Id",
+        "LocusId",
+        "ReferenceRegion",
+        "Motif",
+        "IsAdjacentRepeat",
+        "Sex",
+        "Allele1",
+        "Allele2",
+        "Genotype",
+        "GenotypeConfidenceInterval",
+    ],
+        dtype={
+          "Id": str,
+          "Sex": str,
+          "Allele1": str,
+          "Allele2": str,
+          "GenotypeConfidenceInterval": str,
+          "IsAdjacentRepeat": bool,
+        },
+    )
+    gnomad_df = gnomad_df[~gnomad_df["IsAdjacentRepeat"]]
+    print(f"Processing {len(gnomad_df)} gnomAD table rows...")
+    for column_name, value in [
+        ("Sample_genome_version", "38"),
+        ("Sample_affected", "Not Affected"),
+    ]:
+        gnomad_df.loc[:, column_name] = value
+
+    gnomad_df.loc[:, "Id"] = "gnomAD:" + gnomad_df["Id"]
+    gnomad_df.loc[:, "VariantId"] = gnomad_df["LocusId"]
+
+    gnomad_df.loc[:, ("CI1", "CI2")] = gnomad_df["GenotypeConfidenceInterval"].str.split("/", expand=True)
+    gnomad_df.loc[:, "CI1"] = gnomad_df["CI1"].fillna("")
+    gnomad_df.loc[:, "CI2"] = gnomad_df["CI2"].fillna("")
+    gnomad_df.loc[:, ("CI start: Allele 1", "CI end: Allele 1")] = gnomad_df["CI1"].str.split("-", expand=True)
+    gnomad_df.loc[:, ("CI start: Allele 2", "CI end: Allele 2")] = gnomad_df["CI2"].str.split("-", expand=True)
+    gnomad_df.drop(columns=["CI1", "CI2", "CI start: Allele 1", "CI start: Allele 2"], inplace=True)
+    gnomad_df.rename({
+        "Id": "SampleId",
+        "Sex": "Sample_sex",
+        "Allele1": "Num Repeats: Allele 1",
+        "Allele2": "Num Repeats: Allele 2",
+        "Motif": "RepeatUnit",
+    }, axis="columns", inplace=True)
+
+    return gnomad_df
+
+
+def load_results_tables(args):
     all_dfs = []
-    all_locus_ids = set()
     for combined_tsv_path in args.combined_tsv_path:
-        if not os.path.isfile(combined_tsv_path):
-            p.error(f"{combined_tsv_path} not found")
 
+        # read in table
         df = pd.read_table(combined_tsv_path, low_memory=False)
+        df.loc[:, "Num Repeats: Allele 1"] = df["Num Repeats: Allele 1"].fillna(0).astype(int)
+        df.loc[:, "Num Repeats: Allele 2"] = df["Num Repeats: Allele 2"].fillna(0).astype(int)
+
+        df.loc[:, "Num Repeats: Min Allele 1, 2"] = df.apply(lambda row: (
+            min(row["Num Repeats: Allele 1"], row["Num Repeats: Allele 2"])
+            if
+            row["Num Repeats: Allele 1"] > 0 and row["Num Repeats: Allele 2"] > 0
+            else
+            max(row["Num Repeats: Allele 1"], row["Num Repeats: Allele 2"])
+        ), axis=1)
+
+        df.loc[:, "Num Repeats: Max Allele 1, 2"] = df[["Num Repeats: Allele 1", "Num Repeats: Allele 2"]].max(axis=1)
 
         # check that all required columns are present
         missing_required_columns = set(REQUIRED_COLUMNS) - set(df.columns)
         if missing_required_columns:
-            p.error(f"{combined_tsv_path} is missing these required columns: {missing_required_columns}")
+            raise ValueError(f"{combined_tsv_path} is missing these required columns: {missing_required_columns}")
 
         # fill in values for missing optional columns
         missing_optional_columns = set(OPTIONAL_COLUMNS) - set(df.columns)
         if missing_optional_columns:
             print(f"WARNING: {combined_tsv_path} is missing these columns: {missing_optional_columns}. "
                   f"Filling them with None...")
             for c in missing_optional_columns:
                 df.loc[:, c] = None
 
+        for integer_column in ("CI end: Allele 1", "CI end: Allele 2"):
+            df.loc[:, integer_column] = pd.to_numeric(df[integer_column], errors="coerce")
+
+        all_dfs.append((df, combined_tsv_path))
+
+    return all_dfs
+
+
+def print_results_for_locus(args, locus_id, locus_df, highlight_locus=False):
+    """Prints the sorted table of results for a single locus"""
+
+    for column_name in (
+            "Sample_affected", "Sample_sex", "Sample_analysis_status", "Sample_coded_phenotype",
+            "Sample_genome_version",
+    ):
+        # split values like a; b; b; and collapse to a; b
+        locus_df.loc[:, column_name] = locus_df[column_name].apply(
+            lambda s: "; ".join(set(s.split("; "))) if not pd.isna(s) else s)
+        # truncate long text so it fits on screen
+        locus_df.loc[:, column_name] = locus_df[column_name].str[0:50]
+
+    unexpected_affected_status_values = set(locus_df[
+        ~locus_df["Sample_affected"].isin({"Affected", "Not Affected", "Unknown"})
+    ].Sample_affected)
+    if unexpected_affected_status_values:
+        print(f"WARNING: Some rows have unexpected affected value(s): {unexpected_affected_status_values}")
+
+    # Sort
+    locus_df = locus_df.sort_values(
+        by=["Num Repeats: Allele 2", "Num Repeats: Allele 1", "Sample_affected"],
+        ascending=False)
+
+    # Get the 1st row and use it to look up metadata values which are the same across all rows for the locus
+    # (ie. Inheritance Mode)
+    first_row = locus_df.iloc[0].to_dict()
+
+    disease_info = first_row.get("VariantCatalog_Diseases")
+    intermediate_threshold_min = None
+    pathogenic_threshold_min = None
+    if disease_info and not pd.isna(disease_info):
+        try:
+            disease_info = literal_eval(disease_info)
+        except Exception as e:
+            raise ValueError(f"Unable to parse {disease_info} as json: {e}")
+
+        try:
+            intermediate_threshold_min = min(int(float(d["NormalMax"]) + 1) for d in disease_info if d.get("NormalMax"))
+        except ValueError as e:
+            print(f"WARNING: {locus_id} couldn't parse NormalMax fields from disease_info {disease_info}: {e}")
+
+        try:
+            pathogenic_threshold_min = min(int(float(d["PathogenicMin"])) for d in disease_info if d.get("PathogenicMin"))
+        except ValueError as e:
+            print(f"WARNING: {locus_id} couldn't parse PathogenicMin fields from disease_info {disease_info}: {e}")
+
+    reference_region = first_row["ReferenceRegion"]
+    genome_version = f"GRCh{first_row['Sample_genome_version']}" if first_row.get('Sample_genome_version') else ""
+    motif = first_row.get("RepeatUnit")
+    locus_description = f"{locus_id} ({reference_region}: {genome_version})  https://stripy.org/database/{locus_id}"
+    inheritance_mode = first_row.get("VariantCatalog_Inheritance")
+    if not inheritance_mode or pd.isna(inheritance_mode):
+        inheritance_mode = "XR" if "X" in reference_region else "AD"
+
+    if highlight_locus:
+        locus_description += " " * 100 + "  <== previously diagnosed using short reads"
+    print("**Locus**: ", locus_description)
+    print("**Disease**: ", str(disease_info))
+    print("**Inheritance**: ", inheritance_mode)
+    print("**Pathogenic Threshold**: >=", pathogenic_threshold_min, "x", motif)
+    print("**Intermediate Threshold**: >=", intermediate_threshold_min, "x", motif)
+
+    # replace NA with "Unknown" strings
+    locus_df.loc[:, "Sample_affected"] = locus_df["Sample_affected"].fillna("Unknown")
+    locus_df.loc[:, "Sample_sex"] = locus_df["Sample_sex"].fillna("Unknown")
+
+    # create a list of dfs that are subsets of locus_df and where rows pass thresholds
+    dfs_to_process = []
+    if locus_id == "COMP":
+        # COMP is a special case where contractions below 5 repeats are also pathogenic
+        df_comp = locus_df[
+            (locus_df["CI end: Allele 1"] < 5) |
+            (locus_df["CI end: Allele 2"] < 5)
+        ]
+        dfs_to_process.append(df_comp)
+
+    # add 2 rows to each table representing the pathogenic thresholds
+    threshold_records = []
+    threshold_records_for_male_samples = []
+    for label, threshold in [
+        ("Intermediate Threshold", intermediate_threshold_min),
+        ("Pathogenic Threshold",   pathogenic_threshold_min),
+    ]:
+        if not threshold: continue
+
+        threshold_record = {c: SEPARATOR_STRING for c in locus_df.columns}
+        threshold_record.update({
+            "SampleId": f"**{label}**", "LocusId": locus_id, "VariantId": locus_id,
+            "Genotype": f">= {threshold}",
+            "Num Repeats: Min Allele 1, 2": threshold,
+            "Num Repeats: Max Allele 1, 2": threshold,
+            "Num Repeats: Allele 1": threshold,
+            "Num Repeats: Allele 2": 0,
+        })
+
+        threshold_records_for_male_samples.append(dict(threshold_record))
+
+        threshold_record.update({
+            "Num Repeats: Allele 2": threshold,
+        })
+        threshold_records.append(dict(threshold_record))
+
+    threshold_records = pd.DataFrame(threshold_records)
+    threshold_records_for_male_samples = pd.DataFrame(threshold_records_for_male_samples)
+    args.max_rows += 2  # add 2 to allow for these threshold rows
+
+    # create a list of dfs to print, filtered by the pathogenic thresholds and/or affected status
+    threshold = min(list(filter(None, [intermediate_threshold_min, pathogenic_threshold_min])) or [0]) if args.use_thresholds else 0
+
+    if inheritance_mode == "XR":
+
+        # split results by male/female
+        male_df = locus_df[~locus_df["Genotype"].str.contains("/")]
+        if args.use_thresholds:
+            male_df = male_df[
+                (male_df["CI end: Allele 1"] >= threshold)
+            ].iloc[0:args.max_rows]
+        male_df = pd.concat([threshold_records_for_male_samples, male_df], ignore_index=True)
+        dfs_to_process.append(male_df)
+
+        female_df = locus_df[locus_df["Genotype"].str.contains("/")]
+        if args.use_thresholds:
+            female_df = female_df[
+                (female_df["CI end: Allele 1"] >= threshold) &
+                (female_df["CI end: Allele 2"] >= threshold)
+            ].iloc[0:args.max_rows]
+
+        female_df = pd.concat([threshold_records, female_df], ignore_index=True)
+        dfs_to_process.append(female_df)
+
+    else:
+        if args.use_thresholds:
+            if inheritance_mode == "AR":
+                locus_df = locus_df[
+                    (locus_df["CI end: Allele 1"] >= threshold) &
+                    (locus_df["CI end: Allele 2"] >= threshold)
+                ].iloc[0:args.max_rows]
+            else:
+                # for x-linked dominant, it's enough for one of the alleles to be above the threshold
+                # (ie. male vs. female genotyes)
+                locus_df = locus_df[
+                    (locus_df["CI end: Allele 1"] >= threshold) |
+                    (locus_df["CI end: Allele 2"] >= threshold)
+                ].iloc[0:args.max_rows]
+
+        locus_df = pd.concat([threshold_records, locus_df], ignore_index=True)
+        dfs_to_process.append(locus_df)
+
+    if args.use_affected:
+        # filter by affected status
+        filtered_dfs_list = []
+        for df_to_process in dfs_to_process:
+            unaffected_counter = 0
+            idx = 0
+            for affected_status in df_to_process["Sample_affected"]:
+                idx += 1
+                if affected_status and ("Not Affected" in affected_status or "Unknown" in affected_status):
+                    unaffected_counter += 1
+
+                if unaffected_counter >= args.max_n_unaffected:
+                    break
+
+            df_to_process = df_to_process.iloc[:idx]
+
+            filtered_dfs_list.append(df_to_process)
+        dfs_to_process = filtered_dfs_list
+
+    for i, df_to_process in enumerate(dfs_to_process):
+        print(f"Found {len(df_to_process)} samples passed filters in table {i+1} out of "
+              f"{len(dfs_to_process)} for locus {locus_id}")
+
+        if len(df_to_process) == 0:
+            continue
+
+        if inheritance_mode in {"AR", "XR"}:
+            df_to_process = df_to_process.sort_values(
+                by=["Num Repeats: Min Allele 1, 2", "Sample_affected"],
+                ascending=False)
+        elif inheritance_mode in {"AD", "XD", "Unknown"}:
+            df_to_process = df_to_process.sort_values(
+                by=["Num Repeats: Max Allele 1, 2", "Sample_affected"],
+                ascending=False)
+        else:
+            raise ValueError(f"Unexpected inheritance mode: {inheritance_mode}")
+
+        # Print the filtered results for this locus
+        df_to_process = df_to_process[[
+            "SampleId",
+            "LocusId",
+
+            "Sample_affected",
+            "Sample_sex",
+            "Sample_genome_version",
+
+            "Genotype",
+            "GenotypeConfidenceInterval",
+
+            "VariantCatalog_Inheritance",
+            "RepeatUnit",
+
+            "Sample_analysis_status",
+            "Sample_coded_phenotype",
+            "Sample_phenotypes",
+        ]]
+
+        # Shorten some column names so more can fit on screen
+        df_to_process.rename(columns={
+            "Sample_affected": "affected",
+            "Sample_sex": "sex",
+            "Sample_analysis_status": "analysis_status",
+            "Sample_coded_phenotype": "coded_phenotype",
+            "Sample_phenotypes": "hpo",
+            "Sample_genome_version": "genome",
+            "GenotypeConfidenceInterval": "GenotypeCI",
+            "VariantCatalog_Inheritance": "Mode",
+            "RepeatUnit": "Motif",
+        }, inplace=True)
+
+        # Print the candidate pathogenic rows for this locus
+        print(tabulate(df_to_process, headers="keys", tablefmt="psql", showindex=False))
+
+    return pd.concat(dfs_to_process)
+
+
+def main():
+    args = parse_args()
+
+    all_dfs = load_results_tables(args)
+
+    all_sample_ids = set()
+    all_locus_ids = set()
+    for df, _ in all_dfs:
         all_locus_ids |= set(df.LocusId)
+        all_sample_ids |= set(df.SampleId)
 
-        if args.use_gnomad:
+    all_variant_ids = set()
+    for df, _ in all_dfs:
+        all_variant_ids |= set(df.VariantId)
+
+    variant_ids_that_are_not_locus_ids = all_variant_ids - all_locus_ids
+    if variant_ids_that_are_not_locus_ids:
+        print("WARNING: discarding records with VariantIds:", ", ".join(variant_ids_that_are_not_locus_ids))
+        for i, (df, df_source_path) in enumerate(all_dfs):
+            df = df[~df.VariantId.isin(variant_ids_that_are_not_locus_ids)]
+            all_dfs[i] = (df, df_source_path)
+
+    if args.use_gnomad:
+        gnomad_df = load_gnomad_df()
+
+        for i, df in enumerate(all_dfs):
             print("gnomad_df columns: ", gnomad_df.columns)
             print("df columns: ", df.columns)
-            df = pd.concat([df, gnomad_df])
-            df.fillna("", inplace=True)
+            df_with_gnomad = pd.concat([df, gnomad_df])
+            df_with_gnomad.fillna("", inplace=True)
+            all_dfs[i] = df_with_gnomad
+
+    previously_diagnosed_loci = set()
+    if args.previously_diagnosed_loci:
+        for l in args.previously_diagnosed_loci:
+            if not os.path.isfile(l):
+                previously_diagnosed_loci.add(l)
+            else:
+                with open(l, "rt") as f:
+                    for i, s in enumerate(f.readlines()):
+                        previously_diagnosed_loci.add(s.strip())
 
-        for integer_column in ("CI end: Allele 1", "CI end: Allele 2"):
-            df.loc[:, integer_column] = pd.to_numeric(df[integer_column], errors="coerce")
+                print(f"Read {i + 1} sample ids to highlight from: {l}")
 
-        all_dfs.append((df, combined_tsv_path))
+        if previously_diagnosed_loci - all_locus_ids:
+            print(f"WARNING: cannot highlight {len(previously_diagnosed_loci - all_locus_ids)} loci as they aren't in the "
+                  f"main table(s): {previously_diagnosed_loci - all_locus_ids}")
+
+        previously_diagnosed_loci = previously_diagnosed_loci & all_locus_ids
+        print(f"Will highlight {len(previously_diagnosed_loci)} locus ids: {previously_diagnosed_loci}")
+
+    highlight_sample_ids = set()
+    if args.highlight_samples:
+        for h in args.highlight_samples:
+            if not os.path.isfile(h):
+                highlight_sample_ids.add(h)
+            else:
+                with open(h, "rt") as f:
+                    for i, s in enumerate(f.readlines()):
+                        highlight_sample_ids.add(s.strip())
+
+                print(f"Read {i + 1} sample ids to highlight from: {h}")
+
+        if highlight_sample_ids - all_sample_ids:
+            print(f"WARNING: cannot highlight {len(highlight_sample_ids - all_sample_ids)} ids as they aren't in the "
+                  f"main table(s): {highlight_sample_ids - all_sample_ids}")
+
+        highlight_sample_ids = highlight_sample_ids & all_sample_ids
+        print(f"Will highlight {len(highlight_sample_ids)} sample ids: {highlight_sample_ids}")
+
+    if args.truth_samples:
+        truth_df = pd.read_table(args.truth_samples, names=["sample_id", "locus_id"] + [f"c{i}" for i in range(3, 10)])
+
+        if set(truth_df.sample_id) - all_sample_ids:
+            print(f"WARNING: cannot mark {len(set(truth_df.sample_id) - all_sample_ids)} samples ids from the truth "
+                  f"samples table since they aren't in the main table(s): {set(truth_df.sample_id) - all_sample_ids}")
+        if set(truth_df.locus_id) - all_locus_ids:
+            print(f"WARNING: cannot mark {len(set(truth_df.locus_id) - all_locus_ids)} loci from the truth samples "
+                  f"table since they aren't in the main table(s): {set(truth_df.locus_id) - all_locus_ids}")
+
+    if args.previously_seen_samples:
+        previously_seen_samples_df = pd.read_table(args.previously_seen_samples,
+                                                   names=["sample_id", "locus_id"] + [f"c{i}" for i in range(3, 10)])
+
+        if set(previously_seen_samples_df.sample_id) - all_sample_ids:
+            print(f"WARNING: cannot mark {len(set(previously_seen_samples_df.sample_id) - all_sample_ids)} samples ids "
+                  f"from the previously seen samples table since they aren't in the main table(s): "
+                  f"{set(previously_seen_samples_df.sample_id) - all_sample_ids}")
+        if set(previously_seen_samples_df.locus_id) - all_locus_ids:
+            print(f"WARNING: cannot mark {len(set(previously_seen_samples_df.locus_id) - all_locus_ids)} loci from the "
+                  f"previously seen sample table since they aren't in the main table(s): "
+                  f"{set(previously_seen_samples_df.locus_id) - all_locus_ids}")
 
     # Process each locus
+    results_dfs = []
     for locus_id in sorted(all_locus_ids):
         if args.locus and locus_id not in args.locus:
             continue
 
-        print(">"*100)  # print a divider
+        # Filter to rows for the current locus
         for i, (full_df, df_source_path) in enumerate(all_dfs):
-
             print("="*100)  # print a divider
             print(f"** {locus_id} from {df_source_path} **")
+            locus_df = full_df[full_df.LocusId == locus_id]
+            if len(locus_df) == 0:
+                return
 
-            locus_specific_df = full_df[full_df.LocusId == locus_id]
-            if len(locus_specific_df) == 0:
-                continue
-
-            locus_specific_df = locus_specific_df.sort_values(by=["Num Repeats: Allele 2", "Num Repeats: Allele 1"], ascending=False)
-
-            # get the 1st row and use it to look up metadata values which are the same across all rows for the locus (eg. Inheritance Mode)
-            first_row = locus_specific_df.iloc[0].to_dict()
-            inheritance_mode = first_row.get("VariantCatalog_Inheritance") or "Unknown"
-
-            disease_info = first_row.get("VariantCatalog_Diseases")
-            intermediate_threshold_min = None
-            pathogenic_threshold_min = None
-            if disease_info and not pd.isna(disease_info):
-                try:
-                    disease_info = literal_eval(disease_info)
-                except Exception as e:
-                    raise ValueError(f"Unable to parse {disease_info} as json: {e}")
-
-                try:
-                    intermediate_threshold_min = min(int(float(d["NormalMax"]) + 1) for d in disease_info if d.get("NormalMax"))
-                except ValueError as e:
-                    print(f"WARNING: {locus_id} couldn't parse NormalMax fields from disease_info {disease_info}: {e}")
-
-                try:
-                    pathogenic_threshold_min = min(int(float(d["PathogenicMin"])) for d in disease_info if d.get("PathogenicMin"))
-                except ValueError as e:
-                    print(f"WARNING: {locus_id} couldn't parse PathogenicMin fields from disease_info {disease_info}: {e}")
-
-            reference_region = first_row["ReferenceRegion"]
-            genome_version = f"GRCh{first_row['Sample_genome_version']}" if first_row.get('Sample_genome_version') else ""
-            motif = first_row.get("RepeatUnit")
-            locus_description = f"{locus_id} ({reference_region}: {genome_version})  https://stripy.org/database/{locus_id}"
-            print("**Locus**: ", locus_description)
-            print("**Disease**: ", str(disease_info))
-            print("**Inheritance**: ", inheritance_mode)
-            print("**Pathogenic Threshold**: >=", pathogenic_threshold_min, "x", motif)
-            print("**Intermediate Threshold**: >=", intermediate_threshold_min, "x", motif)
-
-            locus_specific_df.loc[:, "Sample_sample_type"] = locus_specific_df["Sample_sample_type"].fillna("Unknown")
-            locus_specific_df.loc[:, "Sample_sex"] = locus_specific_df["Sample_sex"].fillna("Unknown")
-            locus_specific_df.loc[:, "Sample_affected"] = locus_specific_df["Sample_affected"].fillna("Unknown")
-
-            locus_specific_df = locus_specific_df[locus_specific_df["Sample_affected"] != "Unknown"]
-
-            filtered_df_list = []
-            if locus_id == "COMP":
-                # COMP is a special case where contractions below 5 repeats are also pathogenic
-                df_comp = locus_specific_df[
-                    (locus_specific_df["CI end: Allele 1"] < 5) |
-                    (locus_specific_df["CI end: Allele 2"] < 5)
-                ]
-                filtered_df_list.append(df_comp)
-
-            if args.use_thresholds:
-                threshold = intermediate_threshold_min or pathogenic_threshold_min
-            else:
-                threshold = 0
-
-            if threshold:
-                if inheritance_mode == "XR":
-                    df_female = locus_specific_df[
-                        (locus_specific_df["Sample_sex"].str.upper().str.startswith("F") | locus_specific_df["Sample_sex"].str.upper().str.startswith("U")) &
-                        (locus_specific_df["CI end: Allele 1"]) &
-                        (locus_specific_df["CI end: Allele 1"] >= threshold) &
-                        (locus_specific_df["CI end: Allele 2"] >= threshold)
-                    ].iloc[0:args.max_rows]
-                    df_male = locus_specific_df[
-                        (locus_specific_df["Sample_sex"].str.upper().str.startswith("M")) &
-                        (locus_specific_df["CI end: Allele 1"] >= threshold)
-                    ].iloc[0:args.max_rows]
-                    filtered_dfs_for_locus_and_sample_type = [df_male, df_female]
-                elif inheritance_mode == "AR":
-                    filtered_dfs_for_locus_and_sample_type = [
-                        locus_specific_df[
-                            (locus_specific_df["CI end: Allele 1"] >= threshold) &
-                            (locus_specific_df["CI end: Allele 2"] >= threshold)
-                        ] .iloc[0:args.max_rows]
-                    ]
-                else:
-                    filtered_dfs_for_locus_and_sample_type = [
-                        locus_specific_df[
-                            (locus_specific_df["CI end: Allele 1"] >= threshold) |
-                            (locus_specific_df["CI end: Allele 2"] >= threshold)
-                        ].iloc[0:args.max_rows]
-                    ]
-                filtered_df_list += filtered_dfs_for_locus_and_sample_type
-
-            if args.use_affected:
-                if inheritance_mode == "XR":
-                    dfs_to_process = [
-                        locus_specific_df[
-                            locus_specific_df["Sample_sex"].str.upper().str.startswith("F")
-                        ],
-                        locus_specific_df[
-                            locus_specific_df["Sample_sex"].str.upper().str.startswith("M")
-                        ],
-                    ]
-                else:
-                    dfs_to_process = [locus_specific_df]
-
-                for locus_and_sample_type_and_sex_specific_df in dfs_to_process:
-
-                    unaffected_counter = 0
-                    idx = 0
-                    for affected_status in locus_and_sample_type_and_sex_specific_df["Sample_affected"]:
-                        idx += 1
-                        if affected_status and ("Not Affected" in affected_status or "Unknown" in affected_status):
-                            unaffected_counter += 1
-
-                        if unaffected_counter >= args.max_n_unaffected:
-                            break
-                    
-                    filtered_df_for_locus_and_sample_type_and_sex = locus_and_sample_type_and_sex_specific_df.iloc[:idx]
-
-                    filtered_df_list.append(filtered_df_for_locus_and_sample_type_and_sex)
-
-        for i, filtered_df_for_locus in enumerate(filtered_df_list):
-            print(f"Found {len(filtered_df_for_locus)} samples passed filters in table {i+1} out of {len(filtered_df_list)} for locus {locus_id}")
-
-            if len(filtered_df_for_locus) == 0:
-                continue
-
-            inheritance_mode = first_row.get("VariantCatalog_Inheritance") or "Unknown"
-
-            for label, threshold in [
-                ("Intermediate Threshold", intermediate_threshold_min),
-                ("Pathogenic Threshold", pathogenic_threshold_min),
-            ]:
-                if not threshold:
-                    continue
-                threshold_record = {
-                    "SampleId": f"**{label}**",
-                    "LocusId": locus_id,
-                    "VariantId": locus_id,
-                    "Genotype": f">= {threshold}",
-                }
-
-                for column in filtered_df_for_locus.columns:
-                    if column.lower().startswith("sample_") or column in ("GenotypeConfidenceInterval",):
-                        threshold_record[column] = "---"
-                if inheritance_mode == "XR":
-                    filtered_df_for_locus = filtered_df_for_locus.append({
-                        **threshold_record,
-                        "Num Repeats: Allele 1": threshold,
-                        "Sample_sex": "male",
-                    }, ignore_index=True)
-                    filtered_df_for_locus = filtered_df_for_locus.append({
-                        **threshold_record,
-                        "Num Repeats: Allele 2": threshold,
-                        "Sample_sex": "female",
-                    }, ignore_index=True)
-                else:
-                    filtered_df_for_locus = filtered_df_for_locus.append({
-                        **threshold_record,
-                        "Num Repeats: Allele 2": threshold,
-                    }, ignore_index=True)
-
-            filtered_df_for_locus = filtered_df_for_locus.sort_values(by=["Num Repeats: Allele 2", "Num Repeats: Allele 1"], ascending=False)
-
-            # Print the filtered results for this locus
-            filtered_df_for_locus = filtered_df_for_locus[[
-                "SampleId",
-                "LocusId",
-                "VariantId",
-
-                "Genotype",
-                "GenotypeConfidenceInterval",
-
-                "Sample_sex",
-                "Sample_affected",
-                "Sample_sample_type",
-
-                "Sample_analysis_status",
-                "Sample_coded_phenotype",
-                "Sample_genome_version",
-
-                "RepeatUnit",
-                "VariantCatalog_Inheritance",
-            ]]
             if highlight_sample_ids:
-                highlight_sample_ids = set(highlight_sample_ids)
-                filtered_df_for_locus.loc[:, "SampleId"] = filtered_df_for_locus["SampleId"].apply(lambda s: (s if s not in highlight_sample_ids else f"==> {s}"))
-
-            # Shorten some column names so more can fit on screen
-            filtered_df_for_locus.rename(columns={
-                "Sample_affected": "affected",
-                "Sample_sex": "sex",
-                "Sample_sample_type": "type",
-                "GenotypeConfidenceInterval": "GenotypeCI",
-            }, inplace=True)
-
-            for column_name in "affected", "sex", "type":
-                filtered_df_for_locus.loc[:, column_name] = filtered_df_for_locus[column_name].apply(
-                    lambda s: "; ".join(set(s.split("; "))))
+                locus_df.loc[:, "SampleId"] = locus_df["SampleId"].apply(
+                    lambda s: (s if s not in highlight_sample_ids else f"==> {s}"))
 
-            # Print the candidate pathogenic rows for this locus
-            print(tabulate(filtered_df_for_locus, headers="keys", tablefmt="psql", showindex=False))
+            truth_samples_for_this_locus = set()
+            if args.truth_samples and locus_id in set(truth_df.locus_id):
+                truth_samples_for_this_locus = set(
+                    truth_df[truth_df.locus_id == locus_id].sample_id)
+
+            previously_seen_samples_for_this_locus = set()
+            if args.previously_seen_samples and locus_id in set(previously_seen_samples_df.locus_id):
+                previously_seen_samples_for_this_locus = set(
+                    previously_seen_samples_df[previously_seen_samples_df.locus_id == locus_id].sample_id)
+
+            locus_df.loc[:, "SampleId"] = locus_df["SampleId"].apply(
+                lambda s: (
+                    f"*T* {s}" if s in truth_samples_for_this_locus else (
+                    f"*P* {s}" if s in previously_seen_samples_for_this_locus else s)
+                )
+            )
+
+            results_df = print_results_for_locus(
+                args, locus_id, locus_df, highlight_locus=locus_id in previously_diagnosed_loci)
+
+            results_dfs.append(results_df)
+
+    final_results_df = pd.concat(results_dfs)
+    final_results_df = final_results_df[final_results_df["Sample_affected"] != SEPARATOR_STRING]
+    final_results_df.to_csv(args.results_path, index=False, header=True, sep="\t")
+    print(f"Wrote {len(final_results_df)} rows to {args.results_path}")
+    for locus_id, count in sorted(dict(final_results_df.groupby("LocusId").count().SampleId).items()):
+        print(f"{count:10,d}  {locus_id} rows")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations.py` & `str_analysis-1.1/str_analysis/check_trios_for_mendelian_violations.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from str_analysis.utils.misc_utils import parse_interval
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s %(levelname)s: %(message)s")
 
 # The basic set of columns that need to be present in the input table
 BASIC_INPUT_COLUMNS = [
-    "SampleId", "LocusId", "VariantId", "Filename", "Genotype", "GenotypeConfidenceInterval", "ReferenceRegion",
+    "SampleId", "LocusId", "VariantId", "Genotype", "GenotypeConfidenceInterval", "ReferenceRegion",
     "RepeatUnit", "Sex", "Num Repeats: Allele 2", "Coverage",
 ]
 
 # Optional extra columns that will be added to the output if they're present in the input table
 EXTRA_INPUT_COLUMNS = [
     "NumSpanningReads", "NumFlankingReads", "NumInrepeatReads",
     "NumAllelesSupportedBySpanningReads", "NumAllelesSupportedByFlankingReads", "NumAllelesSupportedByInrepeatReads",
@@ -43,15 +43,15 @@
         help=".fam file that describes parent-child relationships of individual IDs in "
         "the combined_str_calls_tsv",
         type=pathlib.Path,
         required=True,
     )
     p.add_argument(
         "combined_str_calls_tsv",
-        help=".tsv table that conatains str calls for all individuals, created by the "
+        help=".tsv table that contains str calls for all individuals, created by the "
         "combine_expansion_hunter_json_results_to_tsv script",
         type=pathlib.Path,
     )
     args = p.parse_args(args=args_list)
 
     for path in [args.combined_str_calls_tsv, args.fam_file]:
         if not path.is_file():
@@ -85,23 +85,23 @@
     """Parse a tsv table generated by combine_str_json_to_tsv.py, check for duplicates that have the same
     ("SampleId", "LocusId", "VariantId") and then return the table as a pandas DataFrame.
 
     Raises:
         ValueError: if it finds duplicates by ("SampleId", "LocusId", "VariantId")
     """
 
-    combined_str_calls_df = pd.read_table(combined_str_calls_tsv_path)
+    combined_str_calls_df = pd.read_table(combined_str_calls_tsv_path, dtype=str)
     combined_str_calls_df_columns = set(combined_str_calls_df.columns)
     expected_columns = list(BASIC_INPUT_COLUMNS)
     if all(k in combined_str_calls_df_columns for k in EXTRA_INPUT_COLUMNS):
         expected_columns += list(EXTRA_INPUT_COLUMNS)
 
     combined_str_calls_df = combined_str_calls_df[expected_columns]
     #combined_str_calls_df = combined_str_calls_df.drop_duplicates()
-    combined_str_calls_df.set_index(["Filename", "SampleId", "LocusId", "VariantId"], inplace=True)
+    combined_str_calls_df.set_index(["SampleId", "LocusId", "VariantId"], inplace=True)
     check_for_duplicate_keys(combined_str_calls_df, combined_str_calls_tsv_path)
     return combined_str_calls_df.reset_index()
 
 
 def parse_fam_file(fam_file_path):
     """Reads the .fam file and returns a pandas DataFrame.
 
@@ -134,15 +134,15 @@
     2nd list of rows for samples that aren't part of a full trio.
     """
     print("Caching paternal & maternal genotypes")
     all_rows = {}
     for _, row in tqdm.tqdm(combined_str_calls_df.iterrows(), unit=" table rows", total=len(combined_str_calls_df)):
         if row.Genotype is not None:
             all_rows[(row.SampleId, row.LocusId, row.VariantId)] = row
-            all_rows[(row.Filename, row.LocusId, row.VariantId)] = row
+            #all_rows[(row.Filename, row.LocusId, row.VariantId)] = row
 
     calls_counter = 0
     trio_ids = set()
     trio_rows = []
     other_rows = []
     print(f"{len(combined_str_calls_df)} total rows")
     combined_str_calls_df = combined_str_calls_df[~combined_str_calls_df.father_id.isna() & ~combined_str_calls_df.mother_id.isna()]
```

### Comparing `str_analysis-0.9.8/str_analysis/check_trios_for_mendelian_violations_tests.py` & `str_analysis-1.1/str_analysis/check_trios_for_mendelian_violations_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/combine_json_to_tsv.py` & `str_analysis-1.1/str_analysis/combine_json_to_tsv.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv.py` & `str_analysis-1.1/str_analysis/combine_str_json_to_tsv.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pathlib
 import re
 
 import numpy as np
 import pandas as pd
 
 from str_analysis.combine_json_to_tsv import get_sample_id_column_index
+from str_analysis.utils.misc_utils import parse_interval
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s %(levelname)s: %(message)s")
 ALREADY_WARNED_ABOUT = set()  # used for logging
 
 
 def parse_args(args_list=None):
     """Parse command line args and return the argparse args object"""
@@ -47,14 +48,20 @@
     )
     p.add_argument(
         "--include-extra-gangstr-fields",
         action="store_true",
         help="If specified, additional fields from GangSTR will be added. The input json files are expected to be the "
              "result of running convert_gangstr_vcf_to_expansion_hunter_json."
     )
+    p.add_argument(
+        "--include-extra-hipstr-fields",
+        action="store_true",
+        help="If specified, additional fields from HipSTR will be added. The input json files are expected to be the "
+             "result of running convert_hipstr_vcf_to_expansion_hunter_json."
+    )
 
     p.add_argument(
         "-o",
         "--output-prefix",
         help="Combined table output filename prefix",
     )
     p.add_argument(
@@ -80,14 +87,20 @@
     if not args.json_paths:
         args.json_paths = [p for p in pathlib.Path(".").glob("**/*.json")]
         logging.info(f"Found {len(args.json_paths)} json files in .")
 
     return args
 
 
+def compute_bed_file_record(variant_record):
+    chrom, start_0based, end_1based = parse_interval(variant_record["ReferenceRegion"])
+
+    return [chrom, start_0based, end_1based, variant_record["SummaryString"], "."]
+
+
 def main():
     """Main"""
 
     args = parse_args()
 
     output_prefix = args.output_prefix or f"combined_expansion_hunter"
     output_prefix += f".{len(args.json_paths)}_json_files"
@@ -116,14 +129,15 @@
 
     variant_table_columns = []
     allele_table_columns = []
     wrote_variant_table_header = wrote_allele_table_header = False
     variant_records_counter = allele_records_counter = 0
     variant_output_file = open(f"{output_prefix}.variants.tsv", "wt")
     allele_output_file = open(f"{output_prefix}.alleles.tsv", "wt")
+    bed_file_records = []
     sample_metadata_lookup_counters = {}
 
     for just_get_header in True, False:
         if just_get_header:
             json_paths = args.json_paths[:20]
         else:
             json_paths = args.json_paths
@@ -135,62 +149,75 @@
                 logging.info(f"Skipping {json_path}... Unable to parse json: {e}")
                 continue
 
             if not isinstance(json_contents, dict) or "SampleParameters" not in json_contents:
                 logging.info(f"Skipping {json_path}... Expected key 'SampleParameters' not found.")
                 continue
 
-            for record in convert_expansion_hunter_json_to_tsv_columns(
+            for variant_record in convert_expansion_hunter_json_to_tsv_columns(
                 json_contents,
                 variant_catalog_contents=combined_variant_catalog_contents,
                 sample_metadata_lookup=sample_metadata_lookup,
                 sample_metadata_lookup_counters=sample_metadata_lookup_counters,
                 json_file_path=json_path,
-                return_allele_records=False,
+                yield_allele_records=False,
                 include_extra_expansion_hunter_fields=args.include_extra_expansion_hunter_fields,
                 include_extra_gangstr_fields=args.include_extra_gangstr_fields,
+                include_extra_hipstr_fields=args.include_extra_hipstr_fields,
             ):
                 if just_get_header:
-                    variant_table_columns.extend([k for k in record.keys() if k not in variant_table_columns])
+                    variant_table_columns.extend([k for k in variant_record.keys() if k not in variant_table_columns])
                 else:
                     if not wrote_variant_table_header:
                         variant_output_file.write("\t".join(variant_table_columns) + "\n")
                         wrote_variant_table_header = True
                     variant_records_counter += 1
-                    variant_output_file.write("\t".join([str(record[c] if c in record else "") for c in variant_table_columns]) + "\n")
+                    variant_output_file.write(
+                        "\t".join([str(variant_record.get(c, "")) for c in variant_table_columns]) + "\n")
 
-            for record in convert_expansion_hunter_json_to_tsv_columns(
+                    bed_file_records.append(compute_bed_file_record(variant_record))
+
+            for allele_record in convert_expansion_hunter_json_to_tsv_columns(
                 json_contents,
                 variant_catalog_contents=combined_variant_catalog_contents,
                 sample_metadata_lookup=sample_metadata_lookup,
                 json_file_path=json_path,
-                return_allele_records=True,
+                yield_allele_records=True,
                 include_extra_expansion_hunter_fields=args.include_extra_expansion_hunter_fields,
                 include_extra_gangstr_fields=args.include_extra_gangstr_fields,
+                include_extra_hipstr_fields=args.include_extra_hipstr_fields,
             ):
                 if just_get_header:
-                    allele_table_columns.extend([k for k in record.keys() if k not in allele_table_columns])
+                    allele_table_columns.extend([k for k in allele_record.keys() if k not in allele_table_columns])
                 else:
                     if not wrote_allele_table_header:
                         allele_output_file.write("\t".join(allele_table_columns) + "\n")
                         wrote_allele_table_header = True
                     allele_records_counter += 1
-                    allele_output_file.write("\t".join([str(record[c] if c in record else "") for c in allele_table_columns]) + "\n")
+                    allele_output_file.write(
+                        "\t".join([str(allele_record.get(c, "")) for c in allele_table_columns]) + "\n")
 
     if sample_metadata_lookup_counters:
         logging.info(f"Found matches for {sample_metadata_lookup_counters['sample_ids_found']} out of "
               f"{sample_metadata_lookup_counters['total_sample_ids']} "
               f"({100*sample_metadata_lookup_counters['sample_ids_found']/sample_metadata_lookup_counters['total_sample_ids']:0.1f}%) "
               f"ExpansionHunter json sample ids in {args.sample_metadata}")
 
         if len(sample_metadata_lookup) != len(sample_metadata_df):
             logging.info(f"{len(sample_metadata_df) - len(sample_metadata_lookup)} duplicate sample ids in {args.sample_metadata}")
+
     logging.info(f"Wrote {variant_records_counter} records to {output_prefix}.variants.tsv")
     logging.info(f"Wrote {allele_records_counter} records to {output_prefix}.alleles.tsv")
 
+    with open(f"{output_prefix}.bed", "wt") as f:
+        for bed_record in sorted(bed_file_records, key=lambda r: tuple(r[0:2])):
+            f.write("\t".join(map(str, bed_record)) + "\n")
+
+    logging.info(f"Wrote {len(bed_file_records)} records to {output_prefix}.bed")
+
 
 class ParseError(Exception):
     """Represents an error that occurs while parsing"""
     pass
 
 
 def parse_json_file(json_path):
@@ -225,43 +252,87 @@
     """
     average = np.average(values, weights=weights)
     # Fast and numerically precise:
     variance = np.average((values-average)**2, weights=weights)
     return average, np.sqrt(variance)
 
 
+def compute_variant_summary_string(variant_record):
+    """Returns a short easy-to-read string summarizing the tool's STR genotype.
+
+    Args:
+        variant_record (dict): list of 1 or more allele spec dictionaries
+    Return:
+        str: short summary of the variant
+    """
+
+    repeat_unit = variant_record["RepeatUnit"]
+    chrom, start_0based, end_1based = parse_interval(variant_record["ReferenceRegion"])
+    reference_locus_size = end_1based - start_0based
+    num_repeats_ref = int(reference_locus_size/len(repeat_unit))
+
+    if f"Repeat Size (bp): Allele 2" not in variant_record:
+        het_or_hom = "HEMI"
+        allele_numbers = [1]
+    elif variant_record[f"Repeat Size (bp): Allele 1"] == variant_record[f"Repeat Size (bp): Allele 2"]:
+        het_or_hom = "HOM"
+        allele_numbers = [1]
+    else:
+        het_or_hom = "HET"
+        allele_numbers = [1, 2]
+
+    ins_or_del_or_ref = []
+    for i in allele_numbers:
+        allele_size = int(variant_record[f"Repeat Size (bp): Allele {i}"])
+        if allele_size == reference_locus_size:
+            ins_or_del_or_ref.append("REF")
+        elif allele_size > reference_locus_size:
+            ins_or_del_or_ref.append("INS")
+        elif allele_size < reference_locus_size:
+            ins_or_del_or_ref.append("DEL")
+
+    summary_string = str(num_repeats_ref) + "=>" + variant_record["Genotype"]
+    summary_string += "[" + variant_record["GenotypeConfidenceInterval"] + "]"
+    summary_string += ":" + f"{repeat_unit}[{len(repeat_unit)}bp]"
+    summary_string += ":" + het_or_hom
+    summary_string += ":" + ",".join(ins_or_del_or_ref)
+
+    return summary_string
+
+
 def convert_expansion_hunter_json_to_tsv_columns(
     json_contents,
     variant_catalog_contents=None,
     sample_metadata_lookup=None,
     sample_metadata_lookup_counters=None,
     variant_info=None,
     json_file_path="",
-    return_allele_records=True,
+    yield_allele_records=True,
     include_extra_expansion_hunter_fields=False,
     include_extra_gangstr_fields=False,
+    include_extra_hipstr_fields=False,
 ):
     """Converts a dictionary that represents the contents of an ExpansionHunter v3 or v4 json output file to
     a dictionary of tsv column values.
 
     Args:
         json_contents (dict): a dict with the contents of an ExpansionHunter v3 or v4 json output file
         variant_catalog_contents (dict): optional dict with the contents of the variant catalog used when running
             expansion hunter. If provided, the fields will be added to the output table.
         sample_metadata_lookup (dict): maps sample id to row of sample metadata
         sample_metadata_lookup_counters (dict): dictionary for accumulating counters and stats about the
             ability to find samples in sample_metadata_lookup
         variant_info (dict): if provided, results will be added to this dict. Otherwise, a new dict will be created.
         json_file_path (str): if provided, it will be added as a field to the output table, and also used for logging
-        return_allele_records (bool): if True, the returned list will have one record per allele rather than per variant
+        yield_allele_records (bool): if True, the returned list will have one record per allele rather than per variant
         include_extra_expansion_hunter_fields (bool): if True, include additional fields provided by ExpansionHunter.
         include_extra_gangstr_fields (bool): if True, include additional fields provided by GangSTR.
-
-    Returns:
-        list: a list of tsv rows
+        include_extra_hipstr_fields (bool): if True, include additional fields provided by HipSTR.
+    Yields:
+        dict: dictionary representing the output tsv row
     """
 
     if variant_info is None:
         variant_info = collections.OrderedDict()
 
     if variant_catalog_contents:
         variant_catalog_contents = {c['LocusId']: c for c in variant_catalog_contents}
@@ -307,15 +378,14 @@
                         output_value = ""
 
                     if key not in variant_info:
                         variant_info[key] = output_value
                     else:
                         variant_info[key] += f"; {output_value}"
 
-    records_to_return = []
     for locus_json in locus_results_list:
         locus_record = collections.OrderedDict(variant_info)
         for key in "LocusId", "ReadLength", "Coverage", "AlleleCount":
             locus_record[key] = locus_json[key]
 
         # if variant catalog specified, transfer info from it
         locus_id = locus_record["LocusId"]
@@ -371,73 +441,89 @@
                 variant_record["NumSpanningReads"] = int(enclosing)
                 variant_record["NumFlankingReads"] = int(flanking)  # + int(spanning)
                 variant_record["NumInrepeatReads"] = int(FRR)
                 variant_record["NumReadsTotal"] = sum([variant_record[k] for k in (
                     "NumSpanningReads", "NumFlankingReads", "NumInrepeatReads")])
                 variant_record["Q"] = float(variant_json["Q"])
 
+            if include_extra_hipstr_fields:
+                variant_record["Q"] = float(variant_json["Q"])
+                variant_record["DP"] = float(variant_json["DP"])
+                variant_record["AB"] = float(variant_json["AB"])
+                variant_record["FS"] = float(variant_json["FS"])
+                variant_record["DFLANKINDEL"] = float(variant_json["DFLANKINDEL"])
+                variant_record["DSTUTTER"] = float(variant_json["DSTUTTER"])
+
             variant_record["Genotype"] = variant_json["Genotype"]
             variant_record["GenotypeConfidenceInterval"] = variant_json["GenotypeConfidenceInterval"]
             genotype_tuples = list(zip(
                 variant_json["Genotype"].split("/"),
                 variant_json["GenotypeConfidenceInterval"].split("/"),
             ))
 
             for i, (genotype, genotypeCI) in enumerate(genotype_tuples):
-                if return_allele_records:
+                if yield_allele_records:
                     suffix = ""
-                    allele_record = collections.OrderedDict(variant_record)
+                    output_record = collections.OrderedDict(variant_record)
                 else:
                     suffix = f": Allele {i+1}"
-                    allele_record = variant_record
+                    output_record = variant_record
 
                 confidence_interval_start, confidence_interval_end = genotypeCI.split("-")
-                allele_record[f"Allele Number{suffix}"] = i + 1
-                allele_record[f"Num Repeats{suffix}"] = int(genotype)
-                allele_record[f"Repeat Size (bp){suffix}"] = int(genotype) * len(variant_json.get("RepeatUnit", ""))
-                allele_record[f"CI start{suffix}"] = int(confidence_interval_start)
-                allele_record[f"CI end{suffix}"] = int(confidence_interval_end)
-                allele_record[f"CI size{suffix}"] = int(confidence_interval_end) - int(confidence_interval_start)
-                allele_record[f"CI ratio{suffix}"] = allele_record[f"CI size{suffix}"]/(allele_record[f"Num Repeats{suffix}"] or 1)
+                output_record[f"Allele Number{suffix}"] = i + 1
+                output_record[f"Num Repeats{suffix}"] = int(genotype)
+                output_record[f"Repeat Size (bp){suffix}"] = int(genotype) * len(variant_json.get("RepeatUnit", ""))
+                output_record[f"CI start{suffix}"] = int(confidence_interval_start)
+                output_record[f"CI end{suffix}"] = int(confidence_interval_end)
+                output_record[f"CI size{suffix}"] = int(confidence_interval_end) - int(confidence_interval_start)
+                output_record[f"CI ratio{suffix}"] = output_record[f"CI size{suffix}"]/(output_record[f"Num Repeats{suffix}"] or 1)
 
                 if include_extra_expansion_hunter_fields:
                     is_homozygous = len(genotype_tuples) > 1 and genotype_tuples[0][0] == genotype_tuples[1][0]
                     divisor = 2 if is_homozygous else 1
-                    allele_record[f"NumSpanningReadsThatSupportGenotype{suffix}"] = sum(t[1] for t in spanning_read_tuples if t[0] == int(genotype)) / divisor
-                    allele_record[f"NumFlankingReadsThatSupportGenotype{suffix}"] = sum(t[1] for t in flanking_read_tuples if t[0] == int(genotype)) / divisor
-                    allele_record[f"NumInrepeatReadsThatSupportGenotype{suffix}"] = sum(t[1] for t in inrepeat_read_tuples if t[0] == int(genotype)) / divisor
-                    allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] = (
-                        allele_record[f"NumSpanningReadsThatSupportGenotype{suffix}"] +
-                        allele_record[f"NumFlankingReadsThatSupportGenotype{suffix}"] +
-                        allele_record[f"NumInrepeatReadsThatSupportGenotype{suffix}"]
+                    read_length = locus_record.get("ReadLength", 150)
+                    ru_length = variant_record["RepeatUnitLength"]
+                    for label, read_tuples in [("Spanning", spanning_read_tuples), ("Flanking", flanking_read_tuples), ("Inrepeat", inrepeat_read_tuples)]:
+                        output_record[f"Num{label}ReadsThatSupportGenotype{suffix}"] = sum(
+                            t[1] for t in read_tuples
+                            if (t[0] == int(genotype)) or (int(genotype) > t[0] and t[0]*ru_length > 0.8*read_length)
+                        ) / divisor
+
+                    output_record[f"NumReadsTotalThatSupportGenotype{suffix}"] = (
+                        output_record[f"NumSpanningReadsThatSupportGenotype{suffix}"] +
+                        output_record[f"NumFlankingReadsThatSupportGenotype{suffix}"] +
+                        output_record[f"NumInrepeatReadsThatSupportGenotype{suffix}"]
                     )
-                    allele_record[f"FractionOfReadsThatSupportsGenotype{suffix}"] = (
-                        allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] / float(allele_record["NumReadsTotal"]) if int(allele_record["NumReadsTotal"]) > 0 else 0
+                    output_record[f"FractionOfReadsThatSupportsGenotype{suffix}"] = (
+                        output_record[f"NumReadsTotalThatSupportGenotype{suffix}"] / float(output_record["NumReadsTotal"]) if int(output_record["NumReadsTotal"]) > 0 else 0
                     )
+
+                    # ExpansionHunter Q score based on EnsemblTR https://github.com/gymrek-lab/EnsembleTR/blob/main/ensembletr/utils.py#L53-L59
+                    output_record[f"Q{suffix}"] = 1/np.exp(4*output_record[f"CI ratio{suffix}"])
+
                 if include_extra_gangstr_fields:
                     # ex. "2,10|3,7|4,14"
                     for source_field, dest_field in [("ENCLREADS", f"NumSpanningReadsThatSupportGenotype{suffix}"),
                                                      ("FLNKREADS", f"NumFlankingReadsThatSupportGenotype{suffix}")]:
                         if variant_json[source_field] != "NULL":
                             read_support = dict([key_value.split(",") for key_value in variant_json[source_field].split("|")])
-                            allele_record[dest_field] = int(read_support.get(genotype, 0))
+                            output_record[dest_field] = int(read_support.get(genotype, 0))
                         else:
-                            allele_record[dest_field] = 0
+                            output_record[dest_field] = 0
 
-                    allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] = (
-                            allele_record.get(f"NumSpanningReadsThatSupportGenotype{suffix}", 0) +
-                            allele_record.get(f"NumFlankingReadsThatSupportGenotype{suffix}", 0)
+                    output_record[f"NumReadsTotalThatSupportGenotype{suffix}"] = (
+                            output_record.get(f"NumSpanningReadsThatSupportGenotype{suffix}", 0) +
+                            output_record.get(f"NumFlankingReadsThatSupportGenotype{suffix}", 0)
                     )
-                    allele_record[f"FractionOfReadsThatSupportsGenotype{suffix}"] = (
-                        allele_record[f"NumReadsTotalThatSupportGenotype{suffix}"] / float(allele_record["NumReadsTotal"]) if int(allele_record["NumReadsTotal"]) > 0 else 0
+                    output_record[f"FractionOfReadsThatSupportsGenotype{suffix}"] = (
+                        output_record[f"NumReadsTotalThatSupportGenotype{suffix}"] / float(output_record["NumReadsTotal"]) if int(output_record["NumReadsTotal"]) > 0 else 0
                     )
-                if return_allele_records:
-                    records_to_return.append(allele_record)
-
-            if not return_allele_records:
-                records_to_return.append(allele_record)
+                if yield_allele_records:
+                    yield output_record
 
-    return records_to_return
+            if not yield_allele_records:
+                output_record["SummaryString"] = compute_variant_summary_string(output_record)
+                yield output_record
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `str_analysis-0.9.8/str_analysis/combine_str_json_to_tsv_tests.py` & `str_analysis-1.1/str_analysis/combine_str_json_to_tsv_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,68 +164,77 @@
     ] + ([
         'Allele Number: Allele 1',
         'Num Repeats: Allele 1',
         'Repeat Size (bp): Allele 1',
         'CI start: Allele 1',
         'CI end: Allele 1',
         'CI size: Allele 1',
+        'CI ratio: Allele 1',
         'NumSpanningReadsThatSupportGenotype: Allele 1',
         'NumFlankingReadsThatSupportGenotype: Allele 1',
         'NumInrepeatReadsThatSupportGenotype: Allele 1',
         'NumReadsTotalThatSupportGenotype: Allele 1',
         'FractionOfReadsThatSupportsGenotype: Allele 1',
-    ] + ([] if row['AlleleCount'] == 1 else [
+        'Q: Allele 1',
+    ] + ([
+        'SummaryString',
+    ] if row['AlleleCount'] == 1 else [
         'Allele Number: Allele 2',
         'Num Repeats: Allele 2',
         'Repeat Size (bp): Allele 2',
         'CI start: Allele 2',
         'CI end: Allele 2',
         'CI size: Allele 2',
+        'CI ratio: Allele 2',
         'NumSpanningReadsThatSupportGenotype: Allele 2',
         'NumFlankingReadsThatSupportGenotype: Allele 2',
         'NumInrepeatReadsThatSupportGenotype: Allele 2',
         'NumReadsTotalThatSupportGenotype: Allele 2',
         'FractionOfReadsThatSupportsGenotype: Allele 2',
+        'Q: Allele 2',
+        'SummaryString',
     ]) if not with_allele_records else [
         'Allele Number',
         'Num Repeats',
         'Repeat Size (bp)',
         'CI start',
         'CI end',
         'CI size',
+        "CI ratio",
         'NumSpanningReadsThatSupportGenotype',
         'NumFlankingReadsThatSupportGenotype',
         'NumInrepeatReadsThatSupportGenotype',
         'NumReadsTotalThatSupportGenotype',
         'FractionOfReadsThatSupportsGenotype',
+        'Q',
     ])
 
 
 class Tests(unittest.TestCase):
 
     def test_parse_read_count_tuples(self):
         result = parse_read_count_tuples("(11, 4), (16, 2), (17, 13)")
         self.assertListEqual(result, [(11, 4), (16, 2), (17, 13)])
 
         result = parse_read_count_tuples("()")
         self.assertListEqual(result, [])
 
     def test_convert_expansion_hunter_json_to_tsv_columns_for_variants(self):
-        variant_rows = convert_expansion_hunter_json_to_tsv_columns(
+        variant_rows = list(convert_expansion_hunter_json_to_tsv_columns(
             EHv4_JSON,
             variant_catalog_contents=VARIANT_CATALOG_CONTENTS,
             json_file_path="",
-            return_allele_records=False,
+            yield_allele_records=False,
             include_extra_expansion_hunter_fields=True,
-        )
+        ))
         self.assertEqual(len(variant_rows), 4)
         for row in variant_rows:
             self.assertIn('InVariantCatalog', row)
             self.assertIn('AlleleCount', row)
-            self.assertListEqual(list(row.keys()), get_expected_columns(row, with_allele_records=False, with_json_file_path=False))
+            self.assertSetEqual(set(list(row.keys())), set(get_expected_columns(row, with_allele_records=False, with_json_file_path=False)))
 
             self.assertIn(row["LocusId"], {"1-146228800-146228820-NOTCH2NLC", "ATXN7", "X-25013650-25013697-ARX"})
             self.assertIn(row["VariantId"], {"1-146228800-146228820-NOTCH2NLC", "ATXN7", "ATXN7_GCC_ADJACENT", "X-25013650-25013697-ARX"})
 
             self.assertEqual(row["Sex"], "Male")
             self.assertEqual(row["SampleId"], "TestSample")
 
@@ -246,21 +255,21 @@
             self.assertAlmostEqual(variant_rows[0][f"NumSpanningReadsThatSupportGenotype: Allele {allele_num}"], 30.0)
             self.assertAlmostEqual(variant_rows[0][f"NumFlankingReadsThatSupportGenotype: Allele {allele_num}"], 0.5)
             self.assertEqual(variant_rows[0][f"NumInrepeatReadsThatSupportGenotype: Allele {allele_num}"], 0)
             self.assertAlmostEqual(variant_rows[0][f"NumReadsTotalThatSupportGenotype: Allele {allele_num}"], 30.5)
             self.assertAlmostEqual(variant_rows[0][f"FractionOfReadsThatSupportsGenotype: Allele {allele_num}"], 30.5/76)
 
     def test_convert_expansion_hunter_json_to_tsv_columns_for_alleles(self):
-        allele_rows = convert_expansion_hunter_json_to_tsv_columns(
+        allele_rows = list(convert_expansion_hunter_json_to_tsv_columns(
             EHv4_JSON,
             variant_catalog_contents=VARIANT_CATALOG_CONTENTS,
             json_file_path="/temp/file.json",
-            return_allele_records=True,
-            include_all_fields=True,
-        )
+            yield_allele_records=True,
+            include_extra_expansion_hunter_fields=True,
+        ))
         self.assertEqual(len(allele_rows), 7)
         for row in allele_rows:
             self.assertIn('InVariantCatalog', row)
             self.assertIn('AlleleCount', row)
             self.assertListEqual(list(row.keys()), get_expected_columns(row, with_allele_records=True, with_json_file_path=True))
 
             self.assertIn(row["LocusId"], {"1-146228800-146228820-NOTCH2NLC", "ATXN7", "X-25013650-25013697-ARX"})
```

### Comparing `str_analysis-0.9.8/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py` & `str_analysis-1.1/str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py` & `str_analysis-1.1/str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py` & `str_analysis-1.1/str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """This script converts a GangSTR output VCF to the .json format ExpansionHunter uses to output results.
 This makes it easier to pass GangSTR results to downstream scripts.
 """
-from pprint import pprint
 
 """
 GangSTR output vcf format:
 
 chr14   
 39042968        
 .       
@@ -48,16 +47,18 @@
         "SampleId": "NA19239",
         "Sex": "Female"
   }
 """
 
 
 import argparse
+import gzip
 import json
 import os
+from pprint import pprint
 import re
 
 
 def main():
     p = argparse.ArgumentParser()
     p.add_argument("--variant-catalog", help="ExpansionHunter variant catalog. If specified, fields from this"
                                              " variant catalog will be added to the output .json.")
@@ -94,31 +95,31 @@
             variant_ids = [variant_ids]
         for variant_id, variant_type, reference_region in zip(variant_ids, variant_types, reference_regions):
             variant_catalog_lookup[reference_region] = dict(record)
             variant_catalog_lookup[reference_region]["ReferenceRegion"] = reference_region
             variant_catalog_lookup[reference_region]["VariantType"] = variant_type
             variant_catalog_lookup[reference_region]["VariantId"] = variant_id
 
-    #pprint(variant_catalog_lookup)
     return variant_catalog_lookup
 
 
 def process_gangstr_vcf(vcf_path, variant_catalog=None):
-    sample_id = os.path.basename(vcf_path).replace("gangstr.", "").strip(".")
+    sample_id = os.path.basename(vcf_path).replace(".vcf", "").replace(".gz", "").replace("gangstr", "").strip(".")
     locus_results = {
         "LocusResults": {},
         "SampleParameters": {
             "SampleId": sample_id,
             "Sex": None,
         },
     }
 
     variant_catalog_lookup = create_variant_catalog_lookup(variant_catalog or [])
 
-    with open(vcf_path, "rt") as vcf:
+    fopen = gzip.open if vcf_path.endswith("gz") else open
+    with fopen(vcf_path, "rt") as vcf:
         line_counter = 0
         for line in vcf:
             if line.startswith("#"):
                 if line.startswith("##command="):
                     # Parse the "--bam-samps RGP_1126_1 --samp-sex F" args from the command
                     sample_id_match = re.search("bam-samps ([^-]+)", line)
                     if sample_id_match:
```

### Comparing `str_analysis-0.9.8/str_analysis/convert_strling_calls_to_expansion_hunter_json.py` & `str_analysis-1.1/str_analysis/convert_strling_calls_to_expansion_hunter_json.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/data/non_ref_motif.locus_info.json` & `str_analysis-1.1/str_analysis/data/non_ref_motif.locus_info.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'BEAN1'": "{'Motifs': {'REFERENCE': 'TAAAA'}}",*

 * * "'DAB1'": "{'Motifs': {'REFERENCE': 'AAAAT'}}",*

 * * "'MARCHF6'": "{'Motifs': {'REFERENCE': 'ATTTT'}}",*

 * * "'RAPGEF2'": "{'Motifs': {'REFERENCE': 'TTTTA'}}",*

 * * "'RFC1'": "{'Motifs': {'REFERENCE': 'AAAAG'}}",*

 * * "'SAMD12'": "{'Motifs': {'REFERENCE': 'TAAAA'}}",*

 * * "'STARD7'": "{'Motifs': {'REFERENCE': 'AAAAT'}}",*

 * * "'TNRC6A'": "{'Motifs': {'REFERENCE': 'TTTTA'}}",*

 * * "'YEATS2'": "{'Motifs': {'REFERENCE': 'TTTTA'}}"}*

```diff
@@ -7,60 +7,64 @@
         "Motifs": {
             "BENIGN": [
                 "TAAAA"
             ],
             "PATHOGENIC": [
                 "TGGAA",
                 "TAGAA"
-            ]
+            ],
+            "REFERENCE": "TAAAA"
         },
         "UseOfftargetRegions": false
     },
     "DAB1": {
         "LocusCoords_1based": {
             "37": "1:57832716-57832790",
             "38": "chr1:57367044-57367118"
         },
         "Motifs": {
             "BENIGN": [
                 "AAAAT"
             ],
             "PATHOGENIC": [
                 "GAAAT"
-            ]
+            ],
+            "REFERENCE": "AAAAT"
         },
         "UseOfftargetRegions": false
     },
     "MARCHF6": {
         "LocusCoords_1based": {
             "37": "5:10356459-10356523",
             "38": "chr5:10356347-10356411"
         },
         "Motifs": {
             "BENIGN": [
                 "ATTTT"
             ],
             "PATHOGENIC": [
                 "ATTTC"
-            ]
+            ],
+            "REFERENCE": "ATTTT"
         },
         "UseOfftargetRegions": false
     },
     "RAPGEF2": {
         "LocusCoords_1based": {
             "37": "4:160263679-160263768",
             "38": "chr4:159342527-159342616"
         },
         "Motifs": {
             "BENIGN": [
                 "TTTTA"
             ],
             "PATHOGENIC": [
                 "TTTCA"
-            ]
+            ],
+            "REFERENCE": "TTTTA"
         },
         "UseOfftargetRegions": false
     },
     "RFC1": {
         "LocusCoords_1based": {
             "37": "4:39350045-39350099",
             "38": "chr4:39348425-39348479"
@@ -69,15 +73,16 @@
             "BENIGN": [
                 "AAAAG",
                 "AAAGG"
             ],
             "PATHOGENIC": [
                 "AAGGG",
                 "ACAGG"
-            ]
+            ],
+            "REFERENCE": "AAAAG"
         },
         "UseOfftargetRegions": false
     },
     "SAMD12": {
         "LocusCoords_1based": {
             "37": "8:119379055-119379119",
             "38": "chr8:118366816-118366880"
@@ -85,57 +90,61 @@
         "Motifs": {
             "BENIGN": [
                 "TAAAA"
             ],
             "PATHOGENIC": [
                 "TGAAA",
                 "TCAAA"
-            ]
+            ],
+            "REFERENCE": "TAAAA"
         },
         "UseOfftargetRegions": false
     },
     "STARD7": {
         "LocusCoords_1based": {
             "37": "2:96862805-96862859",
             "38": "chr2:96197067-96197121"
         },
         "Motifs": {
             "BENIGN": [
                 "AAAAT"
             ],
             "PATHOGENIC": [
                 "GAAAT"
-            ]
+            ],
+            "REFERENCE": "AAAAT"
         },
         "UseOfftargetRegions": false
     },
     "TNRC6A": {
         "LocusCoords_1based": {
             "37": "16:24624761-24624850",
             "38": "chr16:24613440-24613529"
         },
         "Motifs": {
             "BENIGN": [
                 "TTTTA"
             ],
             "PATHOGENIC": [
                 "TTTCA"
-            ]
+            ],
+            "REFERENCE": "TTTTA"
         },
         "UseOfftargetRegions": false
     },
     "YEATS2": {
         "LocusCoords_1based": {
             "37": "3:183429976-183430010",
             "38": "chr3:183712188-183712222"
         },
         "Motifs": {
             "BENIGN": [
                 "TTTTA"
             ],
             "PATHOGENIC": [
                 "TTTCA"
-            ]
+            ],
+            "REFERENCE": "TTTTA"
         },
         "UseOfftargetRegions": false
     }
 }
```

### Comparing `str_analysis-0.9.8/str_analysis/data/non_ref_motif.offtarget_regions.json.gz` & `str_analysis-1.1/str_analysis/data/non_ref_motif.offtarget_regions.json.gz`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/generate_gnomad_json.py` & `str_analysis-1.1/str_analysis/generate_gnomad_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 """
 This script takes ExpansionHunter calls and metadata files and reprocesses them into tables and .json files
 that can be loaded into the gnomAD browser, and also shared publicly through the gnomAD downloads page.
 
 The script is intended to be run twice:
 1. The 1st time, it is run without the --existing-readviz-filename-list arg so it can generate the
 readviz_rename_list__...tsv file which maps regular readviz image filenames like NA12878.ATXN1.svg to encrypted ones
@@ -224,57 +226,61 @@
 
 # Fraction of samples that can be pcr-free/pcr-plus information before generating an error
 MISSING_PCR_PROTOCOL_THRESHOLD = 0.25
 
 # Expected number of known pathogenic repeats
 EXPECTED_N_KNOWN_PATHOGENIC_REPEATS = 60
 
+# gnomAD projects for which it's ok to release individual-level genotype data
+PUBLIC_PROJECT_NAMES = {"1000 Genomes Project", "Human Genome Diversity Project"}
+
 # Add this "salt" value to the sha512 hash to prevent dictionary attacks on the encrypted sample ids
 salt = pwd.getpwuid(os.getuid()).pw_name
 
 
 def parse_args():
     """Parse command-line args, perform basic validation, and then return the args object."""
 
     p = argparse.ArgumentParser()
     p.add_argument(
         "--expansion-hunter-tsv",
-        default="~/code/str-analysis/local_files/gnomad_str_data/data/without_offtargets/combined_expansion_hunter.19243_json_files.variants.tsv",
         help="Table generated by running python3 -m str_analysis.combine_expansionhunter_json_to_tsv on all samples "
              "called by ExpansionHunter."
     )
     p.add_argument(
         "--non-ref-motif-tsv",
-        default="~/code/str-analysis/local_files/gnomad_str_data/data/without_offtargets/combined.173160_json_files.tsv",
         help="Table generated by running python3 -m str_analysis.combine_json_to_tsv on all loci called by "
-             "str_analysis.call_non_ref_pathogenic_motifs.",
+             "str_analysis.call_non_ref_motifs.",
     )
     p.add_argument(
         "--expansion-hunter-tsv-using-offtargets",
-        default="~/code/str-analysis/local_files/gnomad_str_data/data/with_offtargets/combined_expansion_hunter.19243_json_files.variants.tsv",
         help="Table generated by running python3 -m str_analysis.combine_expansionhunter_json_to_tsv on all samples "
              "called by ExpansionHunter while using a variant catalog that includes off-target regions."
     )
     p.add_argument(
         "--non-ref-motif-tsv-using-offtargets",
-        default="~/code/str-analysis/local_files/gnomad_str_data/data/with_offtargets/combined.173187_json_files.tsv",
         help="Table generated by running python3 -m str_analysis.combine_json_to_tsv on all loci called by "
-             "str_analysis.call_non_ref_pathogenic_motifs with options set to use a variant catalog that "
+             "str_analysis.call_non_ref_motifs with options set to use a variant catalog that "
              "includes off-target regions.",
     )
     p.add_argument(
         "--gnomad-metadata-tsv",
         default="~/code/sample_metadata/metadata/gnomad_v3.1_metadata_v3.1_with_read_lengths.tsv.gz",
         help="gnomAD metadata table path.",
     )
     p.add_argument(
         "--known-pathogenic-strs-tsv",
         default="./data/known_pathogenic_str_loci_metadata_hg38_hg19.tsv",
         help="Table of known pathogenic STRs.",
     )
+    p.add_argument(
+        "--inferred-pcr-status-table",
+        default="~/code/str-analysis/local_files/gnomAD-SV_v3.master_sample_metadata.pre_00c_qc.gatksv_sample_id.inferred_pcr_status",
+        help="Table of inferred PCR+/PCR- labels for all samples")
+
     grp = p.add_mutually_exclusive_group()
     grp.add_argument(
         "--existing-readviz-filename-list",
         help="A text file that lists all readviz .svg filenames that exist (one per line). These are the encrypted "
              "public filenames that don't contain sample ids - for example: ffa0880117e0791d51b0ef85b56f3a54216.svg",
     )
     grp.add_argument(
@@ -294,23 +300,27 @@
         help="Where to write output files. Supports local and Google storage (gs://) paths.",
     )
     p.add_argument(
         "--output-filename-suffix",
         default="",
         help="An optional label to append to all output filenames",
     )
+    p.add_argument(
+        "--local-output-dir",
+        help="Optionally specify local directory to write output files to",
+    )
     args = p.parse_args()
 
     print("Args:")
     for key, value in sorted(args.__dict__.items()):
         print(f"     {key} = {value}")
 
     for path in args.expansion_hunter_tsv, args.non_ref_motif_tsv, args.gnomad_metadata_tsv, \
                 args.known_pathogenic_strs_tsv:
-        if not os.path.isfile(os.path.expanduser(path)):
+        if path and not os.path.isfile(os.path.expanduser(path)):
             p.error(f"{path} file not found")
 
     return args
 
 def process_sample_id(sample_id):
     """Utility method for normalizing a gnomAD sample id
 
@@ -349,37 +359,38 @@
     df = pd.read_table(expansion_hunter_tsv, low_memory=False)
     df.loc[:, "SampleId"] = df.SampleId.apply(process_sample_id)
     df.loc[:, "Motif: Allele 1"] = df["RepeatUnit"]
     df.loc[:, "Motif: Allele 2"] = df["RepeatUnit"]
     df.loc[:, "ReadvizFilename"] = None if no_readviz_images else df["SampleId"] + "." + df["LocusId"] + ".svg"
     df = df[combined_table_columns]
 
-    # Parse the args.non_ref_motif_tsv generated by call_non_ref_pathogenic_motifs
-    print(f"Loading {non_ref_motif_tsv}")
-    non_ref_motifs_df = pd.read_table(non_ref_motif_tsv, low_memory=False)
-    non_ref_motifs_df = non_ref_motifs_df[~non_ref_motifs_df["expansion_hunter_call_genotype"].isna()]
-
-    non_ref_motifs_df["Motif: Allele 1"], non_ref_motifs_df["Motif: Allele 2"] = zip(
-        *non_ref_motifs_df["expansion_hunter_call_repeat_unit"].apply(split_by_forward_slash))
-
-    non_ref_motifs_df.loc[:, "Num Repeats: Allele 1"], non_ref_motifs_df.loc[:, "Num Repeats: Allele 2"] = zip(
-        *non_ref_motifs_df["expansion_hunter_call_genotype"].apply(split_by_forward_slash))
-
-    non_ref_motifs_df.loc[:, "SampleId"] = non_ref_motifs_df.sample_id.apply(process_sample_id)
-    non_ref_motifs_df.loc[:, "LocusId"] = non_ref_motifs_df["locus_id"]
-    non_ref_motifs_df.loc[:, "VariantId"] = non_ref_motifs_df["locus_id"]
-    non_ref_motifs_df.loc[:, "ReferenceRegion"] = non_ref_motifs_df["locus_coords"]
-    non_ref_motifs_df.loc[:, "Genotype"] = non_ref_motifs_df["expansion_hunter_call_genotype"]
-    non_ref_motifs_df.loc[:, "GenotypeConfidenceInterval"] = non_ref_motifs_df["expansion_hunter_call_CI"]
-    non_ref_motifs_df.loc[:, "RepeatUnit"] = None   # will be set later
-    non_ref_motifs_df.loc[:, "ReadvizFilename"] = None if no_readviz_images else non_ref_motifs_df["expansion_hunter_call_reviewer_svg"]
-    non_ref_motifs_df = non_ref_motifs_df[combined_table_columns]
+    # Parse the args.non_ref_motif_tsv generated by call_non_ref_motifs
+    if non_ref_motif_tsv:
+        print(f"Loading {non_ref_motif_tsv}")
+        non_ref_motifs_df = pd.read_table(non_ref_motif_tsv, low_memory=False)
+        non_ref_motifs_df = non_ref_motifs_df[~non_ref_motifs_df["expansion_hunter_call_genotype"].isna()]
+
+        non_ref_motifs_df["Motif: Allele 1"], non_ref_motifs_df["Motif: Allele 2"] = zip(
+            *non_ref_motifs_df["expansion_hunter_call_repeat_unit"].apply(split_by_forward_slash))
+
+        non_ref_motifs_df.loc[:, "Num Repeats: Allele 1"], non_ref_motifs_df.loc[:, "Num Repeats: Allele 2"] = zip(
+            *non_ref_motifs_df["expansion_hunter_call_genotype"].apply(split_by_forward_slash))
+
+        non_ref_motifs_df.loc[:, "SampleId"] = non_ref_motifs_df.sample_id.apply(process_sample_id)
+        non_ref_motifs_df.loc[:, "LocusId"] = non_ref_motifs_df["locus_id"]
+        non_ref_motifs_df.loc[:, "VariantId"] = non_ref_motifs_df["locus_id"]
+        non_ref_motifs_df.loc[:, "ReferenceRegion"] = non_ref_motifs_df["locus_coords"]
+        non_ref_motifs_df.loc[:, "Genotype"] = non_ref_motifs_df["expansion_hunter_call_genotype"]
+        non_ref_motifs_df.loc[:, "GenotypeConfidenceInterval"] = non_ref_motifs_df["expansion_hunter_call_CI"]
+        non_ref_motifs_df.loc[:, "RepeatUnit"] = None   # will be set later
+        non_ref_motifs_df.loc[:, "ReadvizFilename"] = None if no_readviz_images else non_ref_motifs_df["expansion_hunter_call_reviewer_svg"]
+        non_ref_motifs_df = non_ref_motifs_df[combined_table_columns]
 
-    df = df[~df["LocusId"].isin(set(non_ref_motifs_df["LocusId"]))]
-    df = pd.concat([df, non_ref_motifs_df])
+        df = df[~df["LocusId"].isin(set(non_ref_motifs_df["LocusId"]))]
+        df = pd.concat([df, non_ref_motifs_df])
 
     return df
 
 
 def load_data_df(args):
     """Load the tables specified by args.expansion_hunter_tsv, args.non_ref_motif_tsv, and args.gnomad_metadata_tsv.
     Rename and select relevant columns, combine the tables, then return a single combined table.
@@ -424,32 +435,72 @@
     gnomad_df.loc[:, "pcr_free"] = gnomad_df["project_meta.product"].apply(
         lambda s: pd.NA if not s or pd.isna(s) else (True if "pcr-free" in s.lower() else False), convert_dtype="boolean")
     gnomad_df["pcr_free"].fillna(gnomad_df["project_meta.v2_pcr_free"].astype("boolean"), inplace=True)
     gnomad_df["pcr_free"].fillna(PCR_INFO_NOT_AVAILABLE, inplace=True)
     gnomad_df.loc[:, "pcr_protocol"] = gnomad_df["pcr_free"].replace({True: "pcr_free", False: "pcr_plus"})
 
     gnomad_df = gnomad_df[[
-        "s", "population_inference.pop", "sex_imputation.sex_karyotype",
+        "s", "project_meta.sample_id", "population_inference.pop", "sex_imputation.sex_karyotype",
         "age", "pcr_protocol", "read_length",
+        "project_meta.title", "project_meta.neuro_case",
     ]]
-    gnomad_df.loc[:, "s"] = gnomad_df.s.apply(process_sample_id)
+    gnomad_df.loc[:, "s"] = gnomad_df["project_meta.sample_id"].apply(process_sample_id)
+
+    is_public_project = gnomad_df["project_meta.title"].isin(PUBLIC_PROJECT_NAMES)
+    gnomad_df.loc[~is_public_project, "project_meta.title"] = None
+    gnomad_df.loc[is_public_project, "public_sample_id"] = gnomad_df[is_public_project].s
+    gnomad_df.rename(columns={"project_meta.title": "public_project_id", "project_meta.neuro_case": "is_neuro_case"},
+                     inplace=True)
 
     unknown_sample_ids = set(df.SampleId) - set(gnomad_df.s)
     if len(unknown_sample_ids) > 0:
         print(f"WARNING: Dropping {len(unknown_sample_ids)} sample ids in {args.expansion_hunter_tsv} that "
               f"were not found in the gnomAD metadata table, or were found but are not 'release': ", unknown_sample_ids)
+        assert len(unknown_sample_ids) < 5, unknown_sample_ids
+
+        df = df[~df.SampleId.isin(unknown_sample_ids)]
 
     # Merge the data frames
     print(f"Combining STR data tables with gnomAD metadata")
     df = pd.merge(left=df, right=gnomad_df, how="inner", left_on="SampleId", right_on="s").drop(columns="s")
 
     print(f"Found {len(set(df.SampleId))} gnomAD 'release' samples")
     df = df[df.read_length >= MIN_READ_LENGTH]
     print(f"Kept {len(set(df.SampleId))} gnomAD samples after filtering to ReadLength >= {MIN_READ_LENGTH}")
 
+
+    # Add imputed PCR labels
+    inferred_pcr_status_df = pd.read_table(args.inferred_pcr_status_table)
+    inferred_pcr_status_df = inferred_pcr_status_df[["external_sample_id", "inferred_pcr_status"]]
+    inferred_pcr_status_df["external_sample_id"] = inferred_pcr_status_df["external_sample_id"].apply(process_sample_id)
+    inferred_pcr_status_df["inferred_pcr_status"] = inferred_pcr_status_df["inferred_pcr_status"].replace({
+        "PCRMINUS": "pcr_free",
+        "PCRPLUS": "pcr_plus",
+    })
+
+    df = df.set_index("SampleId").join(
+        inferred_pcr_status_df.set_index("external_sample_id"),
+        how="left").reset_index().rename(columns={"index": "SampleId"})
+
+    # mark HGDP samples as pcr_free, since they are known to have been sequenced with a PCR-free protocol
+    df.loc[df.SampleId.str.startswith("HGDP"), "pcr_protocol"] = "pcr_free"
+
+    # fill in missing PCR status with inferred PCR status
+    df.loc[df["pcr_protocol"] == PCR_INFO_NOT_AVAILABLE, "pcr_protocol"] = float('nan')
+    df["pcr_protocol"] = df["pcr_protocol"].fillna(df["inferred_pcr_status"])
+    df.drop(columns="inferred_pcr_status", inplace=True)
+
+    # discard any remaining samples with unknown PCR status
+    n_samples_before_filter = len(set(df.SampleId))
+    df = df[~df.pcr_protocol.isna()]
+    n_samples_after_filter = len(set(df.SampleId))
+    if n_samples_after_filter < n_samples_before_filter:
+        print(f"Dropping {n_samples_before_filter - n_samples_after_filter} samples with unknown PCR status")
+    assert n_samples_before_filter - n_samples_after_filter < 5
+
     locus_id_with_max_samples = None
     max_num_samples = 0
     for locus_id in sorted(set(df.LocusId)):
         num_samples = len(set(df[df.LocusId == locus_id].SampleId))
         if num_samples > max_num_samples:
             locus_id_with_max_samples = locus_id
             max_num_samples = num_samples
@@ -524,14 +575,17 @@
 def add_gene_ids(gnomad_json):
     """Add the GeneId field to gnomad_json.
 
     Args:
         gnomad_json (dict): The main .json structure being generated by this script.
     """
     for locus_id in gnomad_json:
+        if not gnomad_json[locus_id].get("GeneName"):
+            continue
+
         gene_name = gnomad_json[locus_id]["GeneName"]
         if gene_name in GENE_NAME_TO_GENE_ID:
             gnomad_json[locus_id]["GeneId"] = GENE_NAME_TO_GENE_ID[gene_name]
             continue
 
         # Get gene id via the Ensembl API.
         response = None
@@ -560,29 +614,30 @@
 
     known_pathogenic_strs_info = parse_known_pathogenic_strs_tsv(args.known_pathogenic_strs_tsv)
     if len(known_pathogenic_strs_info) != EXPECTED_N_KNOWN_PATHOGENIC_REPEATS:
         raise ValueError(f"{args.known_pathogenic_strs_tsv} contains {len(known_pathogenic_strs_info)} pathogenic loci."
                          f" Expected {EXPECTED_N_KNOWN_PATHOGENIC_REPEATS} loci.")
     locus_ids_without_annotations = set(gnomad_json.keys()) - set(known_pathogenic_strs_info)
     if locus_ids_without_annotations:
-        raise ValueError(f"LocusIds not found in known pathogenic STRs spreadsheet: {locus_ids_without_annotations}")
+        print(f"WARNING: These LocusIds were not found in known pathogenic STRs spreadsheet: {locus_ids_without_annotations}")
 
     # Compute STRipy urls
     for locus_id in gnomad_json:
         stripy_name = locus_id
         stripy_url = f"https://stripy.org/database/{stripy_name}"
         r = requests.get(stripy_url)
         if r.ok and "invalid locus" not in r.content.decode("UTF-8").lower():
             known_pathogenic_strs_info[locus_id]["STRipyName"] = stripy_name
         else:
             print(f"WARNING: STRipy page not found for {locus_id}")
 
     # Add the metadata to gnomad_json
     for locus_id in gnomad_json:
-        gnomad_json[locus_id].update(known_pathogenic_strs_info[locus_id])
+        if locus_id in known_pathogenic_strs_info:
+            gnomad_json[locus_id].update(known_pathogenic_strs_info[locus_id])
 
 
 def compute_most_common_motif_lookup_dict(df):
     """Create a lookup dictionary that maps (LocusId, canonical motif) pairs to the most common non-canonical motif
     among observed motifs that share this same canonical motif. This allows converting motif rearrangements such as
     AAAAG, AAAGA, AAGAA, etc. at the RFC1 locus into "AAAAG" which is the rearrangement that is seen most frequently
     in the general population. Similarly, for the HTT locus, "AGC", "CAG", and "GCA" would get converted to "CAG" since
@@ -631,14 +686,17 @@
         gnomad_json (dict): The main .json structure being generated by this script.
         most_common_motif_lookup (dict): The dictionary generated by compute_most_common_motif_lookup_dict(..)
     """
 
     non_ref_pathogenic_motif_info = json.loads(pkgutil.get_data("str_analysis", "data/non_ref_motif.locus_info.json"))
 
     for locus_id in gnomad_json:
+        if not gnomad_json[locus_id].get("GeneName"):
+            continue
+
         gene_name = gnomad_json[locus_id]["GeneName"]
         if gene_name not in non_ref_pathogenic_motif_info:
             continue
 
         gnomad_json[locus_id]["RepeatUnitClassification"] = {}
         for classification, motifs in non_ref_pathogenic_motif_info[gene_name]["Motifs"].items():
             for motif in motifs:
@@ -684,14 +742,15 @@
     """
 
     readviz_paths_to_rename = set()
     readviz_json = collections.defaultdict(list)
     user_friendly_genotypes_json = []
     user_friendly_genotypes_json_binned = collections.defaultdict(list)
     age_counter = collections.defaultdict(int)
+    public_sample_id_counter = collections.defaultdict(set)
 
     total_readviz_counter = collections.defaultdict(int)
     missing_readviz_counter = collections.defaultdict(int)
 
     existing_readviz_filenames_set = None
     if existing_readviz_filename_list:
         existing_readviz_filenames_df = pd.read_table(existing_readviz_filename_list, names=["filenames"], low_memory=False)
@@ -714,14 +773,17 @@
         motif2 = most_common_motif_lookup[locus_id, canonical_motif2]
 
         # Get gnomAD fields
         sex_karyotype = row["sex_imputation.sex_karyotype"]
         population = row["population_inference.pop"]
         pcr_protocol = row["pcr_protocol"]
         read_length = int(row["read_length"])
+        public_project_id = row["public_project_id"] if not pd.isna(row["public_project_id"]) else None
+        public_sample_id = row["public_sample_id"] if not pd.isna(row["public_sample_id"]) else None
+        is_neuro_case = row["is_neuro_case"]
 
         # Compute age_range
         if row["age"] == AGE_NOT_AVAILABLE:
             age_range = AGE_NOT_AVAILABLE
         else:
             age = int(row["age"])
             age_lower_bound = AGE_RANGE_SIZE * math.floor(age/AGE_RANGE_SIZE)
@@ -821,16 +883,22 @@
             "IsAdjacentRepeat": is_adjacent_repeat,
             "Population": population,
             "Sex": sex_karyotype,
             "Age": age_range_for_user_friendly_genotypes_file,
             "PcrProtocol": pcr_protocol,
             "ReadLength": read_length,
             "ReadvizFilename": encrypted_svg_filename,
+            "PublicProjectId": public_project_id,
+            "PublicSampleId": public_sample_id,
+            "IsNeuroCase": is_neuro_case,
         }
 
+        if public_sample_id:
+            public_sample_id_counter[public_project_id].add(public_sample_id)
+
         # transfer additional columns from the table row. The values are: (to_column, to_column_type, warn_if_missing)
         extra_columns = {
             "ReferenceRegion": ("ReferenceRegion", str, True),
             "Genotype": ("Genotype", str, True),
             "GenotypeConfidenceInterval": ("GenotypeConfidenceInterval", str, True),
             "Num Repeats: Allele 1": ("Allele1", int, True),
             "Num Repeats: Allele 2": ("Allele2", int, False),  # expected to be missing in hemizygous genotypes
@@ -868,26 +936,33 @@
                 "Age": age_range_to_show_in_readviz_section,
                 "Population": population,
                 "PcrProtocol": pcr_protocol,
                 "Genotype": row["Genotype"],
                 "GenotypeConfidenceInterval": row["GenotypeConfidenceInterval"],
                 "ReadLength": read_length,
                 "ReadvizFilename": encrypted_svg_filename,
+                "PublicProjectId": public_project_id,
+                "PublicSampleId": public_sample_id,
+                "IsNeuroCase": is_neuro_case,
             })
 
+    for project_id, sample_id_set in sorted(public_sample_id_counter.items(), key=lambda x: -len(x[1])):
+        print(f"{len(sample_id_set):,d} public sample ids in gnomAD project '{project_id}'")
+
     # check whether an unexpected number of readviz images are missing
-    for locus_id, missing_count in missing_readviz_counter.items():
-        total = total_readviz_counter[locus_id]
-        message = (f"{locus_id:20s}:  {missing_count} out of {total} ({100*missing_count/total:0.2f}%) readviz images removed "
-                   f"because they are missing from {existing_readviz_filename_list}")
+    if not no_readviz_images:
+        for locus_id, missing_count in missing_readviz_counter.items():
+            total = total_readviz_counter[locus_id]
+            message = (f"{locus_id:20s}:  {missing_count} out of {total} ({100*missing_count/total:0.2f}%) readviz images removed "
+                       f"because they are missing from {existing_readviz_filename_list}")
 
-        if missing_count/total > MISSING_READVIZ_ERROR_THRESHOLD:
-            raise ValueError(message)
+            if missing_count/total > MISSING_READVIZ_ERROR_THRESHOLD:
+                raise ValueError(message)
 
-        print(message)
+            print(message)
 
     # Check for samples that fall into a unique metadata bin - where they are the only samples with a particular
     # combination of values for population, sex, age-bin, and pcr-protocol. Having only 1 individual in a bin like this
     # could allow someone to get all STR genotypes for that single individual by looking up its metadata signature
     # at each STR locus.
     # For added caution, and in-keeping with the principle of only sharing per-variant information, this loop discards
     # the Age and PCR-protocol values from the user_friendly_genotypes_json data structure. This should move these
@@ -1037,57 +1112,61 @@
                 metadata for each sample.
         no_readviz_images (bool): If True, this method will skip validation of the "ReadvizFilename" field. This is used
             for datasets where REViewer images were not generated.
     """
 
     total_samples = len(set(df["SampleId"]))
     if len(gnomad_json) != EXPECTED_N_KNOWN_PATHOGENIC_REPEATS:
-        raise ValueError(f"gnomad_json contains {len(gnomad_json)} pathogenic loci. "
+        print(f"WARNING: gnomad_json contains {len(gnomad_json)} pathogenic loci. "
             f"Expected {EXPECTED_N_KNOWN_PATHOGENIC_REPEATS} loci.")
 
     gnomad_json_str_loci = set(gnomad_json)
     readviz_json_str_loci = set(readviz_json)
     if gnomad_json_str_loci != readviz_json_str_loci:
         raise ValueError(f"gnomad_json locus ids are different from readviz_json locus ids:\n"
                          f"{gnomad_json_str_loci} \n{readviz_json_str_loci}")
 
     fraction_male_samples = sum(df["sex_imputation.sex_karyotype"] == "XY")/len(df)
     for locus_id, data in gnomad_json.items():
         # Check that expected keys are present and have non-null values.
         for key in "ReferenceRepeatUnit", "LocusId", "GeneName", "GeneId", "ReferenceRegion", \
                    "AlleleCountHistogram", "AlleleCountScatterPlot", "AgeDistribution", "Diseases":
-            if data[key] is None:
-                raise ValueError(f"{locus_id} {key} is None")
+            if data.get(key) is None:
+                print(f"WARNING: {locus_id} {key} is None")
 
         # Check that expected keys are present in the data["Diseases"] dictionary and have non-null values.
         for key in "Symbol", "Name", "Inheritance", "PathogenicMin", "OMIM":
-            for i, disease_data in enumerate(data["Diseases"]):
-                if disease_data[key] is None:
-                    raise ValueError(f"{locus_id} disease #{i} {key} is None")
+            diseases = data.get("Diseases", [])
+            if not diseases:
+                print(f"WARNING: {locus_id} has no Diseases data")
+                break
+            for i, disease_data in enumerate(diseases):
+                if disease_data.get(key) is None:
+                    print(f"WARNING: {locus_id} disease #{i} {key} is None")
 
         # Check that total counts in the histogram and scatter plot roughly match expectation, taking into account
         # hemizygous genotypes (which only contribute 1 count) and missing genotypes due to low coverage in some samples
         if "X" in data["ReferenceRegion"]:
             expected_counts_in_histogram = total_samples * (2 - fraction_male_samples)
         else:
             expected_counts_in_histogram = total_samples * 2
 
         for key, expected_counts in [
             ("AlleleCountHistogram", expected_counts_in_histogram),
             ("AlleleCountScatterPlot", total_samples)
         ]:
             total_counts_in_plot = sum([sum(d.values()) for d in data[key].values()])
             if not ((1 - MISSING_GENOTYPES_ERROR_THRESHOLD) * expected_counts < total_counts_in_plot <= expected_counts):
-                raise ValueError(f"ERROR: {locus_id} total counts in {key} = {total_counts_in_plot} while expected counts = {expected_counts}")
+                print(f"WARNING: {locus_id} total counts in {key} = {total_counts_in_plot} while expected counts = {expected_counts}")
 
         total_readviz_samples = len(readviz_json[locus_id])
         if total_readviz_samples < (1 - MISSING_GENOTYPES_ERROR_THRESHOLD) * total_samples:
-            raise ValueError(f"{locus_id}: only {total_readviz_samples} readviz records. Expected {total_samples}")
+            print(f"WARNING: {locus_id}: only {total_readviz_samples} readviz records. Expected {total_samples}")
         if total_readviz_samples > total_samples:
-            raise ValueError(f"{locus_id}: found {total_readviz_samples} readviz records which is more than the total "
+            print(f"WARNING: {locus_id}: found {total_readviz_samples} readviz records which is more than the total "
                              f"number of samples ({total_samples})")
 
         if not no_readviz_images:
             total_readviz_samples_with_image = sum(1 for r in readviz_json[locus_id] if r["ReadvizFilename"] is not None)
             if total_readviz_samples_with_image < (1 - MISSING_READVIZ_ERROR_THRESHOLD) * total_readviz_samples:
                 raise ValueError(f"{locus_id}: found {total_readviz_samples_with_image} readviz images. Expected at "
                                  f"least {total_readviz_samples}.")
@@ -1149,15 +1228,19 @@
     sort_keys(gnomad_json)
 
     # Perform validity checks
     validate_json(df, gnomad_json, readviz_json, user_friendly_genotypes_json, no_readviz_images=args.no_readviz)
 
     # Write out the data structures
     date_stamp = datetime.now().strftime("%Y_%m_%d")
-    local_output_dir = os.path.expanduser(os.path.dirname(args.expansion_hunter_tsv))
+    local_output_dir = args.local_output_dir
+    if local_output_dir is None:
+        local_output_dir = os.path.expanduser(os.path.dirname(args.expansion_hunter_tsv))
+    print(f"Output dir: {local_output_dir}")
+
     output_filename_label = f"__{args.output_filename_suffix}" if args.output_filename_suffix else ""
 
     # write out the full df for debugging and internal analyses that need sample ids
     export_to_tsv(df, f"{local_output_dir}/gnomAD_STR_calls_with_gnomAD_metadata_and_sample_ids{output_filename_label}__{date_stamp}.tsv")
 
     # write out readviz_records to a .tsv mostly for debugging
     readviz_metadata_df = pd.DataFrame([
@@ -1180,15 +1263,15 @@
             record["Id"],
             -1*int(record["Allele2"]) if record["Allele2"] else 0,
             -1*int(record["Allele1"]) if record["Allele1"] else 0,
         )
 
     user_friendly_genotypes_json.sort(key=user_friendly_genotypes_sort_key)
     user_friendly_genotypes_df = pd.DataFrame(user_friendly_genotypes_json)
-    user_friendly_genotypes_df = user_friendly_genotypes_df[[
+    user_friendly_genotypes_df = user_friendly_genotypes_df.filter(items=[
         "Id", "LocusId",
         "ReferenceRegion",
         "Chrom", "Start_0based", "End",
         "Motif",
         "IsAdjacentRepeat",
         "Population", "Sex", "Age", "PcrProtocol",
         "Genotype",
@@ -1197,15 +1280,18 @@
         "GenotypeConfidenceInterval",
         "GenotypeUsingOfftargetRegions",
         "Allele1UsingOfftargetRegions",
         "Allele2UsingOfftargetRegions",
         "GenotypeConfidenceIntervalUsingOfftargetRegions",
         "ReadvizFilename",
         "ReadLength",
-    ]]
+        "IsNeuroCase",
+        "PublicProjectId",
+        "PublicSampleId",
+    ])
     output_path = f"{local_output_dir}/gnomAD_STR_genotypes{output_filename_label}__"
     if args.include_all_age_and_pcr_info:
         output_path += "including_all_age_and_pcr_info__"
     output_path += f"{date_stamp}.tsv"
     export_to_tsv(
         user_friendly_genotypes_df,
         output_path,
```

### Comparing `str_analysis-0.9.8/str_analysis/generate_gnomad_json_tests.py` & `str_analysis-1.1/str_analysis/generate_gnomad_json_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/simulate_str_expansions.py` & `str_analysis-1.1/str_analysis/simulate_str_expansions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import argparse
 import logging
 import math
 import os
 
 import pyfaidx
```

### Comparing `str_analysis-0.9.8/str_analysis/simulate_str_expansions_tests.py` & `str_analysis-1.1/str_analysis/simulate_str_expansions_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/trim_repeat_loci.py` & `str_analysis-1.1/str_analysis/trim_repeat_loci.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/bam_utils.py` & `str_analysis-1.1/str_analysis/utils/bam_utils.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit.py` & `str_analysis-1.1/str_analysis/utils/canonical_repeat_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     Args:
         motif (str): A repeat motif like "CAG".
         include_reverse_complement (bool): if False, will not consider the reverse-complement of the given motif.  
     Return:
         str: The alphabetically first repeat motif.
     """
+    motif = motif.upper()
     minimal_motif = _alphabetically_first_motif_under_shift(motif)
 
     if include_reverse_complement:
         motif_rc = reverse_complement(motif)
         minimal_motif_rc = _alphabetically_first_motif_under_shift(motif_rc)
     
         if minimal_motif_rc < minimal_motif:
```

### Comparing `str_analysis-0.9.8/str_analysis/utils/canonical_repeat_unit_tests.py` & `str_analysis-1.1/str_analysis/utils/canonical_repeat_unit_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/dat_utils.py` & `str_analysis-1.1/str_analysis/utils/dat_utils.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/ehdn_info_for_locus.py` & `str_analysis-1.1/str_analysis/utils/ehdn_info_for_locus.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/export_json.py` & `str_analysis-1.1/str_analysis/utils/export_json.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/fasta_utils.py` & `str_analysis-1.1/str_analysis/utils/fasta_utils.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/known_pathogenic_strs_tsv.py` & `str_analysis-1.1/str_analysis/utils/known_pathogenic_strs_tsv.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/misc_utils.py` & `str_analysis-1.1/str_analysis/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit.py` & `str_analysis-1.1/str_analysis/utils/most_frequent_repeat_unit.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/most_frequent_repeat_unit_tests.py` & `str_analysis-1.1/str_analysis/utils/most_frequent_repeat_unit_tests.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/strling_info_for_locus.py` & `str_analysis-1.1/str_analysis/utils/strling_info_for_locus.py`

 * *Files identical despite different names*

### Comparing `str_analysis-0.9.8/str_analysis/utils/trf_runner.py` & `str_analysis-1.1/str_analysis/utils/trf_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import os
 import subprocess
 import tempfile
 import unittest
 
-from utils.dat_utils import parse_dat_file
+from str_analysis.utils.dat_utils import parse_dat_file
 
 
 class TRFRunner:
     """Class for piping nucleotide sequences to a background TandemRepeatFinder process."""
 
     def __init__(self,
                  trf_command_path,
```

### Comparing `str_analysis-0.9.8/str_analysis.egg-info/SOURCES.txt` & `str_analysis-1.1/str_analysis.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,38 @@
+LICENSE
 README.md
 setup.py
 str_analysis/__init__.py
-str_analysis/call_non_ref_pathogenic_motifs.py
+str_analysis/add_adjacent_loci_to_expansion_hunter_catalog.py
+str_analysis/add_adjacent_loci_to_expansion_hunter_catalog__manual_unittest.py
+str_analysis/annotate_EHdn_locus_outliers.py
+str_analysis/annotate_and_filter_variant_catalog.py
+str_analysis/call_non_ref_motifs.py
+str_analysis/check_combined_non_ref_pathogenic_motifs.py
+str_analysis/check_combined_results_tsv_for_genome_wide_repeats.py
 str_analysis/check_combined_results_tsv_for_pathogenic_repeats.py
 str_analysis/check_trios_for_mendelian_violations.py
 str_analysis/check_trios_for_mendelian_violations_tests.py
 str_analysis/combine_json_to_tsv.py
+str_analysis/combine_str_catalogs.py
 str_analysis/combine_str_json_to_tsv.py
 str_analysis/combine_str_json_to_tsv_tests.py
+str_analysis/convert_annotated_EHdn_locus_outliers_to_expansion_hunter_catalog.py
+str_analysis/convert_bed_to_expansion_hunter_variant_catalog.py
+str_analysis/convert_expansion_hunter_denovo_locus_tsv_to_bed.py
 str_analysis/convert_expansion_hunter_variant_catalog_to_gangstr_spec.py
 str_analysis/convert_gangstr_spec_to_expansion_hunter_variant_catalog.py
 str_analysis/convert_gangstr_vcf_to_expansion_hunter_json.py
+str_analysis/convert_hipstr_vcf_to_expansion_hunter_json.py
 str_analysis/convert_strling_calls_to_expansion_hunter_json.py
 str_analysis/filter_vcf_to_STR_variants.py
 str_analysis/filter_vcf_to_STR_variants_tests.py
 str_analysis/generate_gnomad_json.py
 str_analysis/generate_gnomad_json_tests.py
+str_analysis/gnomad_sample_qc.py
 str_analysis/simulate_str_expansions.py
 str_analysis/simulate_str_expansions_tests.py
 str_analysis/trim_repeat_loci.py
 str_analysis.egg-info/PKG-INFO
 str_analysis.egg-info/SOURCES.txt
 str_analysis.egg-info/dependency_links.txt
 str_analysis.egg-info/entry_points.txt
@@ -31,15 +44,19 @@
 str_analysis/utils/bam_utils.py
 str_analysis/utils/canonical_repeat_unit.py
 str_analysis/utils/canonical_repeat_unit_tests.py
 str_analysis/utils/dat_utils.py
 str_analysis/utils/ehdn_info_for_locus.py
 str_analysis/utils/export_json.py
 str_analysis/utils/fasta_utils.py
+str_analysis/utils/file_utils.py
 str_analysis/utils/find_repeat_unit.py
 str_analysis/utils/find_repeat_unit_tests.py
+str_analysis/utils/get_adjacent_repeats.py
+str_analysis/utils/gtf_utils.py
+str_analysis/utils/gtf_utils__manual_unittest.py
 str_analysis/utils/known_pathogenic_strs_tsv.py
 str_analysis/utils/misc_utils.py
 str_analysis/utils/most_frequent_repeat_unit.py
 str_analysis/utils/most_frequent_repeat_unit_tests.py
 str_analysis/utils/strling_info_for_locus.py
 str_analysis/utils/trf_runner.py
```

