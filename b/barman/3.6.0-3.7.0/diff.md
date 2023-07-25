# Comparing `tmp/barman-3.6.0.tar.gz` & `tmp/barman-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/barman-3.6.0.tar", last modified: Thu Jun 15 12:24:44 2023, max compression
+gzip compressed data, was "dist/barman-3.7.0.tar", last modified: Tue Jul 25 17:21:44 2023, max compression
```

## Comparing `barman-3.6.0.tar` & `barman-3.7.0.tar`

### file list

```diff
@@ -1,306 +1,310 @@
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/build/
--rwxr-xr-x   0     1001      123     1417 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/build
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/build/templates/
--rw-r--r--   0     1001      123    81089 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/logo-horizontal-hires.png
--rw-r--r--   0     1001      123     6346 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/default.latex
--rw-r--r--   0     1001      123      161 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/default.yaml
--rw-r--r--   0     1001      123    16668 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/postgres.pdf
--rw-r--r--   0     1001      123     3895 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/edb-enterprisedb-logo.png
--rw-r--r--   0     1001      123   102895 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/logo-hires.png
--rw-r--r--   0     1001      123     9952 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/templates/Barman.tex
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/build/html-templates/
--rw-r--r--   0     1001      123     3838 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template-utils.html
--rw-r--r--   0     1001      123     1187 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/barman.css
--rw-r--r--   0     1001      123    21298 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/docs.css
--rw-r--r--   0     1001      123      238 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/SOURCES.md
--rw-r--r--   0     1001      123   147074 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/bootstrap.css
--rw-r--r--   0     1001      123     5572 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template.html
--rw-r--r--   0     1001      123      111 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template.css
--rw-r--r--   0     1001      123     3520 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/template-cli.html
--rw-r--r--   0     1001      123     1092 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/html-templates/override.css
--rw-r--r--   0     1001      123     1750 2023-06-15 12:24:22.000000 barman-3.6.0/doc/build/Makefile
--rw-r--r--   0     1001      123     2240 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-archive.1.md
--rw-r--r--   0     1001      123       47 2023-06-15 12:24:22.000000 barman-3.6.0/doc/.gitignore
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/barman.5.d/
--rw-r--r--   0     1001      123      537 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/30-configuration-file-directory.md
--rw-r--r--   0     1001      123      244 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_workers.md
--rw-r--r--   0     1001      123      405 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_format.md
--rw-r--r--   0     1001      123       80 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-log_level.md
--rw-r--r--   0     1001      123      505 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-active.md
--rw-r--r--   0     1001      123      472 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-last_backup_maximum_age.md
--rw-r--r--   0     1001      123     1055 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-primary_conninfo.md
--rw-r--r--   0     1001      123      220 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-parallel_jobs.md
--rw-r--r--   0     1001      123      210 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/20-configuration-file-locations.md
--rw-r--r--   0     1001      123      463 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-immediate_checkpoint.md
--rw-r--r--   0     1001      123      117 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-parallel_jobs_start_batch_size.md
--rw-r--r--   0     1001      123      222 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-azure_credential.md
--rw-r--r--   0     1001      123       52 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-log_file.md
--rw-r--r--   0     1001      123      144 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_archive_script.md
--rw-r--r--   0     1001      123      440 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_archive_retry_script.md
--rw-r--r--   0     1001      123      379 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_wal_delete_retry_script.md
--rw-r--r--   0     1001      123      162 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-custom_decompression_filter.md
--rw-r--r--   0     1001      123      487 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-reuse_backup.md
--rw-r--r--   0     1001      123      367 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-last_wal_maximum_age.md
--rw-r--r--   0     1001      123      179 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-check_timeout.md
--rw-r--r--   0     1001      123      139 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_wal_delete_script.md
--rw-r--r--   0     1001      123       79 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_recovery_script.md
--rw-r--r--   0     1001      123      110 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/00-header.md
--rw-r--r--   0     1001      123      272 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/15-description.md
--rw-r--r--   0     1001      123      757 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_method.md
--rw-r--r--   0     1001      123       97 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_wal_delete_script.md
--rw-r--r--   0     1001      123       79 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-retention_policy_mode.md
--rw-r--r--   0     1001      123      174 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/99-copying.md
--rw-r--r--   0     1001      123      263 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-gcp-zone.md
--rw-r--r--   0     1001      123      992 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_options.md
--rw-r--r--   0     1001      123      186 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-snapshot-instance.md
--rw-r--r--   0     1001      123      275 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_level.md
--rw-r--r--   0     1001      123       10 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/45-options.md
--rw-r--r--   0     1001      123      237 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_archiver_name.md
--rw-r--r--   0     1001      123       88 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-ssh_command.md
--rw-r--r--   0     1001      123       66 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-description.md
--rw-r--r--   0     1001      123      411 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-archiver_batch_size.md
--rw-r--r--   0     1001      123      413 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_delete_retry_script.md
--rw-r--r--   0     1001      123      172 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_backup_name.md
--rw-r--r--   0     1001      123       83 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-barman_lock_directory.md
--rw-r--r--   0     1001      123      464 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-archiver.md
--rw-r--r--   0     1001      123       63 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-wals_directory.md
--rw-r--r--   0     1001      123       86 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_directory.md
--rw-r--r--   0     1001      123      328 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-compression.md
--rw-r--r--   0     1001      123      109 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_archive_script.md
--rw-r--r--   0     1001      123      229 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/25-configuration-file-syntax.md
--rw-r--r--   0     1001      123       59 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/05-name.md
--rw-r--r--   0     1001      123      212 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-snapshot-provider.md
--rw-r--r--   0     1001      123      213 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-errors_directory.md
--rw-r--r--   0     1001      123      365 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-recovery_options.md
--rw-r--r--   0     1001      123      441 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_archiver_batch_size.md
--rw-r--r--   0     1001      123      388 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_archive_retry_script.md
--rw-r--r--   0     1001      123       91 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-minimum_redundancy.md
--rw-r--r--   0     1001      123      267 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-tablespace_bandwidth_limit.md
--rw-r--r--   0     1001      123      363 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_recovery_retry_script.md
--rw-r--r--   0     1001      123      294 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-azure_subscription_id.md
--rw-r--r--   0     1001      123      539 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression.md
--rw-r--r--   0     1001      123      300 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-azure_resource_group.md
--rw-r--r--   0     1001      123      129 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_delete_script.md
--rw-r--r--   0     1001      123      403 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_backup_retry_script.md
--rw-r--r--   0     1001      123      155 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/95-resources.md
--rw-r--r--   0     1001      123      129 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-incoming_wals_directory.md
--rw-r--r--   0     1001      123      405 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_recovery_retry_script.md
--rw-r--r--   0     1001      123      247 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-network_compression.md
--rw-r--r--   0     1001      123       79 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-basebackups_directory.md
--rw-r--r--   0     1001      123      130 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-wal_retention_policy.md
--rw-r--r--   0     1001      123      762 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/75-example.md
--rw-r--r--   0     1001      123      593 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/90-authors.md
--rw-r--r--   0     1001      123      250 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-create_slot.md
--rw-r--r--   0     1001      123      512 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-custom_compression_magic.md
--rw-r--r--   0     1001      123      652 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-recovery_staging_path.md
--rw-r--r--   0     1001      123      252 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-max_incoming_wals_queue.md
--rw-r--r--   0     1001      123      174 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_conninfo.md
--rw-r--r--   0     1001      123      362 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_backup_retry_script.md
--rw-r--r--   0     1001      123      239 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-backup_compression_location.md
--rw-r--r--   0     1001      123       26 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/80-see-also.md
--rw-r--r--   0     1001      123      138 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-parallel_jobs_start_batch_period.md
--rw-r--r--   0     1001      123      176 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-bandwidth_limit.md
--rw-r--r--   0     1001      123      119 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_recovery_script.md
--rw-r--r--   0     1001      123       80 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_backup_script.md
--rw-r--r--   0     1001      123      366 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-conninfo.md
--rw-r--r--   0     1001      123      233 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-path_prefix.md
--rw-r--r--   0     1001      123      653 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-retention_policy.md
--rw-r--r--   0     1001      123      359 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-primary_ssh_command.md
--rw-r--r--   0     1001      123      118 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_backup_script.md
--rw-r--r--   0     1001      123      651 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_archiver.md
--rw-r--r--   0     1001      123       91 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_delete_script.md
--rw-r--r--   0     1001      123      373 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-post_delete_retry_script.md
--rw-r--r--   0     1001      123      546 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-last_backup_minimum_size.md
--rw-r--r--   0     1001      123      368 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-forward-config-path.md
--rw-r--r--   0     1001      123      163 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-streaming_wals_directory.md
--rw-r--r--   0     1001      123      192 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-basebackup_retry_sleep.md
--rw-r--r--   0     1001      123      100 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-custom_compression_filter.md
--rw-r--r--   0     1001      123      425 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-pre_wal_delete_retry_script.md
--rw-r--r--   0     1001      123       56 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-barman_home.md
--rw-r--r--   0     1001      123      202 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-snapshot-disks.md
--rw-r--r--   0     1001      123     1545 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/70-hook-scripts.md
--rw-r--r--   0     1001      123      171 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-slot_name.md
--rw-r--r--   0     1001      123      183 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-basebackup_retry_times.md
--rw-r--r--   0     1001      123      275 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5.d/50-gcp-project.md
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/runbooks/
--rw-r--r--   0     1001      123     9399 2023-06-15 12:24:22.000000 barman-3.6.0/doc/runbooks/snapshot_recovery_azure.md
--rw-r--r--   0     1001      123    31574 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.5
--rw-r--r--   0     1001      123     5531 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-keep.1.md
--rw-r--r--   0     1001      123     6536 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-restore.1.md
--rw-r--r--   0     1001      123     6500 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-list.1
--rw-r--r--   0     1001      123    11659 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-archive.1
--rw-r--r--   0     1001      123     5329 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-check-wal-archive.1.md
--rw-r--r--   0     1001      123     9020 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-delete.1
--rw-r--r--   0     1001      123     5369 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-restore.1.md
--rw-r--r--   0     1001      123     5215 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-show.1.md
--rw-r--r--   0     1001      123    11338 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup.1.md
--rw-r--r--   0     1001      123     5106 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-list.1.md
--rw-r--r--   0     1001      123    26819 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1
--rw-r--r--   0     1001      123     8813 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-archive.1.md
--rw-r--r--   0     1001      123     8362 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-restore.1
--rw-r--r--   0     1001      123     6872 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-wal-restore.1
--rw-r--r--   0     1001      123      706 2023-06-15 12:24:22.000000 barman-3.6.0/doc/Dockerfile
--rw-r--r--   0     1001      123     3066 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-restore.1.md
--rw-r--r--   0     1001      123     6645 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-show.1
--rw-r--r--   0     1001      123     7164 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-delete.1.md
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/barman.d/
--rw-r--r--   0     1001      123      950 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.d/passive-server.conf-template
--rw-r--r--   0     1001      123     1546 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.d/ssh-server.conf-template
--rw-r--r--   0     1001      123     1500 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.d/streaming-server.conf-template
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/barman.1.d/
--rw-r--r--   0     1001      123      788 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-list-files.md
--rw-r--r--   0     1001      123      241 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-show-servers.md
--rw-r--r--   0     1001      123       41 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/10-synopsis.md
--rw-r--r--   0     1001      123      368 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-sync-backup.md
--rw-r--r--   0     1001      123       81 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-switch-xlog.md
--rw-r--r--   0     1001      123      347 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/85-bugs.md
--rw-r--r--   0     1001      123      110 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/00-header.md
--rw-r--r--   0     1001      123      272 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/15-description.md
--rw-r--r--   0     1001      123      174 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/99-copying.md
--rw-r--r--   0     1001      123       55 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/45-commands.md
--rw-r--r--   0     1001      123      295 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-rebuild-xlogdb.md
--rw-r--r--   0     1001      123      850 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-switch-wal.md
--rw-r--r--   0     1001      123     3139 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-backup.md
--rw-r--r--   0     1001      123       74 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-list-servers.md
--rw-r--r--   0     1001      123       98 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-generate-manifest.md
--rw-r--r--   0     1001      123     1048 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-get-wal.md
--rw-r--r--   0     1001      123       61 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-verify.md
--rw-r--r--   0     1001      123     5849 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-recover.md
--rw-r--r--   0     1001      123      393 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-check.md
--rw-r--r--   0     1001      123       51 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/75-exit-status.md
--rw-r--r--   0     1001      123       60 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/05-name.md
--rw-r--r--   0     1001      123      279 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-cron.md
--rw-r--r--   0     1001      123      798 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-status.md
--rw-r--r--   0     1001      123      668 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-receive-wal.md
--rw-r--r--   0     1001      123      155 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/95-resources.md
--rw-r--r--   0     1001      123      333 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-check-backup.md
--rw-r--r--   0     1001      123     1268 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-keep.md
--rw-r--r--   0     1001      123      270 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-diagnose.md
--rw-r--r--   0     1001      123      596 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/20-options.md
--rw-r--r--   0     1001      123      621 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/90-authors.md
--rw-r--r--   0     1001      123      701 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-put-wal.md
--rw-r--r--   0     1001      123      642 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-sync-info.md
--rw-r--r--   0     1001      123       26 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/80-see-also.md
--rw-r--r--   0     1001      123      291 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-list-backups.md
--rw-r--r--   0     1001      123      143 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-delete.md
--rw-r--r--   0     1001      123      578 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-replication-status.md
--rw-r--r--   0     1001      123      351 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-sync-wals.md
--rw-r--r--   0     1001      123      590 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-check-wal-archive.md
--rw-r--r--   0     1001      123      266 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-archive-wal.md
--rw-r--r--   0     1001      123      265 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-verify-backup.md
--rw-r--r--   0     1001      123     1420 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/50-show-backup.md
--rw-r--r--   0     1001      123      444 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.1.d/70-backup-id-shortcuts.md
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/images/
--rw-r--r--   0     1001      123   228769 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario2b.png
--rw-r--r--   0     1001      123   157428 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-georedundancy.png
--rw-r--r--   0     1001      123   179610 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario1.png
--rw-r--r--   0     1001      123   227695 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario1b.png
--rw-r--r--   0     1001      123   201845 2023-06-15 12:24:22.000000 barman-3.6.0/doc/images/barman-architecture-scenario2.png
--rw-r--r--   0     1001      123     3622 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-restore.1
--rw-r--r--   0     1001      123     7082 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup-keep.1
--rw-r--r--   0     1001      123    14779 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-backup.1
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/doc/manual/
--rw-r--r--   0     1001      123     5283 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/24-wal_archiving.en.md
--rw-r--r--   0     1001      123       43 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/.gitignore
--rw-r--r--   0     1001      123     2914 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/15-system_requirements.en.md
--rw-r--r--   0     1001      123     4309 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/99-references.en.md
--rw-r--r--   0     1001      123     1335 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/30-windows-support.en.md
--rw-r--r--   0     1001      123    49424 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/50-feature-details.en.md
--rw-r--r--   0     1001      123    13511 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/43-backup-commands.en.md
--rw-r--r--   0     1001      123     1083 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/25-streaming_backup.en.md
--rw-r--r--   0     1001      123     2629 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/41-global-commands.en.md
--rw-r--r--   0     1001      123     5034 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/23-wal_streaming.en.md
--rw-r--r--   0     1001      123     1017 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/26-rsync_backup.en.md
--rw-r--r--   0     1001      123     3665 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/66-about.en.md
--rw-r--r--   0     1001      123    11271 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/42-server-commands.en.md
--rw-r--r--   0     1001      123      784 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/00-head.en.md
--rw-r--r--   0     1001      123      823 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/20-server_setup.en.md
--rw-r--r--   0     1001      123     8659 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/16-installation.en.md
--rw-r--r--   0     1001      123    10341 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/55-barman-cli.en.md
--rw-r--r--   0     1001      123     6706 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/28-snapshots.en.md
--rw-r--r--   0     1001      123      667 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/Makefile
--rw-r--r--   0     1001      123      862 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/22-config_file.en.md
--rw-r--r--   0     1001      123     1001 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/02-before_you_start.en.md
--rw-r--r--   0     1001      123    11160 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/10-design.en.md
--rw-r--r--   0     1001      123     4014 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/01-intro.en.md
--rw-r--r--   0     1001      123     9313 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/21-preliminary_steps.en.md
--rw-r--r--   0     1001      123     1732 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/65-troubleshooting.en.md
--rw-r--r--   0     1001      123     3564 2023-06-15 12:24:22.000000 barman-3.6.0/doc/manual/17-configuration.en.md
--rw-r--r--   0     1001      123     6807 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-cloud-check-wal-archive.1
--rw-r--r--   0     1001      123     2331 2023-06-15 12:24:22.000000 barman-3.6.0/doc/Makefile
--rw-r--r--   0     1001      123     2630 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman-wal-archive.1
--rw-r--r--   0     1001      123     3501 2023-06-15 12:24:22.000000 barman-3.6.0/doc/barman.conf
--rw-r--r--   0     1001      123     2193 2023-06-15 12:24:22.000000 barman-3.6.0/README.rst
--rw-r--r--   0     1001      123    35147 2023-06-15 12:24:22.000000 barman-3.6.0/LICENSE
--rw-r--r--   0     1001      123      196 2023-06-15 12:24:22.000000 barman-3.6.0/MANIFEST.in
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/
--rw-r--r--   0     1001      123        1 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/dependency_links.txt
--rw-r--r--   0     1001      123      258 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/requires.txt
--rw-r--r--   0     1001      123        7 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/top_level.txt
--rw-r--r--   0     1001      123     9589 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/SOURCES.txt
--rw-r--r--   0     1001      123      729 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/entry_points.txt
--rw-r--r--   0     1001      123     1479 2023-06-15 12:24:44.000000 barman-3.6.0/barman.egg-info/PKG-INFO
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/
--rw-r--r--   0     1001      123      890 2023-06-15 12:24:22.000000 barman-3.6.0/barman/__init__.py
--rw-r--r--   0     1001      123   164482 2023-06-15 12:24:22.000000 barman-3.6.0/barman/server.py
--rw-r--r--   0     1001      123    42482 2023-06-15 12:24:22.000000 barman-3.6.0/barman/wal_archiver.py
--rw-r--r--   0     1001      123    11394 2023-06-15 12:24:22.000000 barman-3.6.0/barman/hooks.py
--rw-r--r--   0     1001      123     4343 2023-06-15 12:24:22.000000 barman-3.6.0/barman/diagnose.py
--rw-r--r--   0     1001      123    69167 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cli.py
--rw-r--r--   0     1001      123    77879 2023-06-15 12:24:22.000000 barman-3.6.0/barman/output.py
--rw-r--r--   0     1001      123    19890 2023-06-15 12:24:22.000000 barman-3.6.0/barman/fs.py
--rw-r--r--   0     1001      123    12760 2023-06-15 12:24:22.000000 barman-3.6.0/barman/annotations.py
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/clients/
--rw-r--r--   0     1001      123    14774 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_delete.py
--rw-r--r--   0     1001      123      724 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/__init__.py
--rwxr-xr-x   0     1001      123    11355 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_walarchive.py
--rw-r--r--   0     1001      123     6705 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_walrestore.py
--rw-r--r--   0     1001      123     4344 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_keep.py
--rw-r--r--   0     1001      123     3720 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_show.py
--rwxr-xr-x   0     1001      123    16333 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/walrestore.py
--rw-r--r--   0     1001      123    13672 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_restore.py
--rw-r--r--   0     1001      123     4438 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup_list.py
--rw-r--r--   0     1001      123     3147 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_check_wal_archive.py
--rwxr-xr-x   0     1001      123    11331 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/walarchive.py
--rw-r--r--   0     1001      123     6302 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_compression.py
--rw-r--r--   0     1001      123     6339 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_cli.py
--rwxr-xr-x   0     1001      123    14285 2023-06-15 12:24:22.000000 barman-3.6.0/barman/clients/cloud_backup.py
--rw-r--r--   0     1001      123    19109 2023-06-15 12:24:22.000000 barman-3.6.0/barman/retention_policies.py
--rw-r--r--   0     1001      123     4215 2023-06-15 12:24:22.000000 barman-3.6.0/barman/postgres_plumbing.py
--rw-r--r--   0     1001      123     5959 2023-06-15 12:24:22.000000 barman-3.6.0/barman/process.py
--rw-r--r--   0     1001      123    95393 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud.py
--rw-r--r--   0     1001      123    16411 2023-06-15 12:24:22.000000 barman-3.6.0/barman/xlog.py
--rw-r--r--   0     1001      123     2315 2023-06-15 12:24:22.000000 barman-3.6.0/barman/remote_status.py
--rw-r--r--   0     1001      123    45270 2023-06-15 12:24:22.000000 barman-3.6.0/barman/command_wrappers.py
--rw-r--r--   0     1001      123    49647 2023-06-15 12:24:22.000000 barman-3.6.0/barman/copy_controller.py
--rw-r--r--   0     1001      123     5491 2023-06-15 12:24:22.000000 barman-3.6.0/barman/backup_manifest.py
--rw-r--r--   0     1001      123    33055 2023-06-15 12:24:22.000000 barman-3.6.0/barman/compression.py
--rw-r--r--   0     1001      123     9554 2023-06-15 12:24:22.000000 barman-3.6.0/barman/exceptions.py
--rw-r--r--   0     1001      123    61344 2023-06-15 12:24:22.000000 barman-3.6.0/barman/backup.py
--rw-r--r--   0     1001      123    40522 2023-06-15 12:24:22.000000 barman-3.6.0/barman/config.py
--rw-r--r--   0     1001      123    89029 2023-06-15 12:24:22.000000 barman-3.6.0/barman/backup_executor.py
--rw-r--r--   0     1001      123    11374 2023-06-15 12:24:22.000000 barman-3.6.0/barman/lockfile.py
--rw-r--r--   0     1001      123    28226 2023-06-15 12:24:22.000000 barman-3.6.0/barman/infofile.py
--rw-r--r--   0     1001      123    25604 2023-06-15 12:24:22.000000 barman-3.6.0/barman/utils.py
--rw-r--r--   0     1001      123    63696 2023-06-15 12:24:22.000000 barman-3.6.0/barman/postgres.py
--rw-r--r--   0     1001      123    81412 2023-06-15 12:24:22.000000 barman-3.6.0/barman/recovery_executor.py
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/storage/
--rw-r--r--   0     1001      123      724 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/__init__.py
--rw-r--r--   0     1001      123     1799 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/file_manager.py
--rw-r--r--   0     1001      123     1679 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/file_stats.py
--rw-r--r--   0     1001      123     2397 2023-06-15 12:24:22.000000 barman-3.6.0/barman/storage/local_file_manager.py
--rw-r--r--   0     1001      123      805 2023-06-15 12:24:43.000000 barman-3.6.0/barman/version.py
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/barman/cloud_providers/
--rw-r--r--   0     1001      123    12220 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/__init__.py
--rw-r--r--   0     1001      123    14428 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/aws_s3.py
--rw-r--r--   0     1001      123    39481 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/azure_blob_storage.py
--rw-r--r--   0     1001      123    30678 2023-06-15 12:24:22.000000 barman-3.6.0/barman/cloud_providers/google_cloud_storage.py
--rw-r--r--   0     1001      123    55839 2023-06-15 12:24:22.000000 barman-3.6.0/NEWS
-drwxr-xr-x   0     1001      123        0 2023-06-15 12:24:44.000000 barman-3.6.0/scripts/
--rw-r--r--   0     1001      123       98 2023-06-15 12:24:22.000000 barman-3.6.0/scripts/barman.bash_completion
--rwxr-xr-x   0     1001      123     4933 2023-06-15 12:24:22.000000 barman-3.6.0/setup.py
--rw-r--r--   0     1001      123      280 2023-06-15 12:24:44.000000 barman-3.6.0/setup.cfg
--rw-r--r--   0     1001      123     1479 2023-06-15 12:24:44.000000 barman-3.6.0/PKG-INFO
--rw-r--r--   0     1001      123     1277 2023-06-15 12:24:22.000000 barman-3.6.0/AUTHORS
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/
+-rw-r--r--   0     1001      123      280 2023-07-25 17:21:44.000000 barman-3.7.0/setup.cfg
+-rw-r--r--   0     1001      123     2193 2023-07-25 17:21:16.000000 barman-3.7.0/README.rst
+-rw-r--r--   0     1001      123     1509 2023-07-25 17:21:44.000000 barman-3.7.0/PKG-INFO
+-rw-r--r--   0     1001      123      196 2023-07-25 17:21:16.000000 barman-3.7.0/MANIFEST.in
+-rw-r--r--   0     1001      123    35147 2023-07-25 17:21:16.000000 barman-3.7.0/LICENSE
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/
+-rw-r--r--   0     1001      123     9270 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-delete.1
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/barman.5.d/
+-rw-r--r--   0     1001      123      512 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-custom_compression_magic.md
+-rw-r--r--   0     1001      123       83 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-barman_lock_directory.md
+-rw-r--r--   0     1001      123      487 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-reuse_backup.md
+-rw-r--r--   0     1001      123      267 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-tablespace_bandwidth_limit.md
+-rw-r--r--   0     1001      123      174 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/99-copying.md
+-rw-r--r--   0     1001      123      413 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_delete_retry_script.md
+-rw-r--r--   0     1001      123      202 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-snapshot-disks.md
+-rw-r--r--   0     1001      123      411 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-archiver_batch_size.md
+-rw-r--r--   0     1001      123      379 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_wal_delete_retry_script.md
+-rw-r--r--   0     1001      123       80 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_backup_script.md
+-rw-r--r--   0     1001      123      162 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-custom_decompression_filter.md
+-rw-r--r--   0     1001      123       56 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-barman_home.md
+-rw-r--r--   0     1001      123      652 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-recovery_staging_path.md
+-rw-r--r--   0     1001      123       59 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/05-name.md
+-rw-r--r--   0     1001      123       52 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-log_file.md
+-rw-r--r--   0     1001      123      366 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-conninfo.md
+-rw-r--r--   0     1001      123      222 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-azure_credential.md
+-rw-r--r--   0     1001      123      130 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-wal_retention_policy.md
+-rw-r--r--   0     1001      123      119 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_recovery_script.md
+-rw-r--r--   0     1001      123      537 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/30-configuration-file-directory.md
+-rw-r--r--   0     1001      123      441 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-streaming_archiver_batch_size.md
+-rw-r--r--   0     1001      123      505 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-active.md
+-rw-r--r--   0     1001      123      520 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-autogenerate_manifest.md
+-rw-r--r--   0     1001      123      213 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-errors_directory.md
+-rw-r--r--   0     1001      123      138 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-parallel_jobs_start_batch_period.md
+-rw-r--r--   0     1001      123       26 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/80-see-also.md
+-rw-r--r--   0     1001      123      212 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-snapshot-provider.md
+-rw-r--r--   0     1001      123      300 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-azure_resource_group.md
+-rw-r--r--   0     1001      123      155 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/95-resources.md
+-rw-r--r--   0     1001      123      275 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-gcp-project.md
+-rw-r--r--   0     1001      123      171 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-slot_name.md
+-rw-r--r--   0     1001      123      172 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-streaming_backup_name.md
+-rw-r--r--   0     1001      123       79 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_recovery_script.md
+-rw-r--r--   0     1001      123      144 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_archive_script.md
+-rw-r--r--   0     1001      123      373 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_delete_retry_script.md
+-rw-r--r--   0     1001      123      100 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-custom_compression_filter.md
+-rw-r--r--   0     1001      123      129 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-incoming_wals_directory.md
+-rw-r--r--   0     1001      123      110 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/00-header.md
+-rw-r--r--   0     1001      123      651 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-streaming_archiver.md
+-rw-r--r--   0     1001      123       86 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_directory.md
+-rw-r--r--   0     1001      123      464 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-archiver.md
+-rw-r--r--   0     1001      123      183 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-basebackup_retry_times.md
+-rw-r--r--   0     1001      123      328 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-compression.md
+-rw-r--r--   0     1001      123      992 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_options.md
+-rw-r--r--   0     1001      123      233 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-path_prefix.md
+-rw-r--r--   0     1001      123      362 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_backup_retry_script.md
+-rw-r--r--   0     1001      123      109 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_archive_script.md
+-rw-r--r--   0     1001      123      247 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-network_compression.md
+-rw-r--r--   0     1001      123      229 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/25-configuration-file-syntax.md
+-rw-r--r--   0     1001      123      250 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-create_slot.md
+-rw-r--r--   0     1001      123      186 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-snapshot-instance.md
+-rw-r--r--   0     1001      123      129 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_delete_script.md
+-rw-r--r--   0     1001      123     1055 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-primary_conninfo.md
+-rw-r--r--   0     1001      123      192 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-basebackup_retry_sleep.md
+-rw-r--r--   0     1001      123      388 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_archive_retry_script.md
+-rw-r--r--   0     1001      123       79 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-retention_policy_mode.md
+-rw-r--r--   0     1001      123      405 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_compression_format.md
+-rw-r--r--   0     1001      123      294 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-azure_subscription_id.md
+-rw-r--r--   0     1001      123      440 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_archive_retry_script.md
+-rw-r--r--   0     1001      123       80 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-log_level.md
+-rw-r--r--   0     1001      123      156 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-aws_region.md
+-rw-r--r--   0     1001      123      762 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/75-example.md
+-rw-r--r--   0     1001      123       10 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/45-options.md
+-rw-r--r--   0     1001      123      472 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-last_backup_maximum_age.md
+-rw-r--r--   0     1001      123      463 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-immediate_checkpoint.md
+-rw-r--r--   0     1001      123       66 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-description.md
+-rw-r--r--   0     1001      123       91 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-minimum_redundancy.md
+-rw-r--r--   0     1001      123      237 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-streaming_archiver_name.md
+-rw-r--r--   0     1001      123       97 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_wal_delete_script.md
+-rw-r--r--   0     1001      123      174 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-streaming_conninfo.md
+-rw-r--r--   0     1001      123      368 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-forward-config-path.md
+-rw-r--r--   0     1001      123      653 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-retention_policy.md
+-rw-r--r--   0     1001      123      139 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_wal_delete_script.md
+-rw-r--r--   0     1001      123      220 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-parallel_jobs.md
+-rw-r--r--   0     1001      123      425 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_wal_delete_retry_script.md
+-rw-r--r--   0     1001      123      176 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-bandwidth_limit.md
+-rw-r--r--   0     1001      123      757 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_method.md
+-rw-r--r--   0     1001      123      117 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-parallel_jobs_start_batch_size.md
+-rw-r--r--   0     1001      123      142 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-aws_profile.md
+-rw-r--r--   0     1001      123       88 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-ssh_command.md
+-rw-r--r--   0     1001      123      359 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-primary_ssh_command.md
+-rw-r--r--   0     1001      123      163 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-streaming_wals_directory.md
+-rw-r--r--   0     1001      123      210 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/20-configuration-file-locations.md
+-rw-r--r--   0     1001      123      244 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_compression_workers.md
+-rw-r--r--   0     1001      123      275 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_compression_level.md
+-rw-r--r--   0     1001      123      365 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-recovery_options.md
+-rw-r--r--   0     1001      123      367 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-last_wal_maximum_age.md
+-rw-r--r--   0     1001      123      252 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-max_incoming_wals_queue.md
+-rw-r--r--   0     1001      123       91 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_delete_script.md
+-rw-r--r--   0     1001      123      593 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/90-authors.md
+-rw-r--r--   0     1001      123       79 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-basebackups_directory.md
+-rw-r--r--   0     1001      123      539 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_compression.md
+-rw-r--r--   0     1001      123       63 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-wals_directory.md
+-rw-r--r--   0     1001      123      405 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_recovery_retry_script.md
+-rw-r--r--   0     1001      123      363 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_recovery_retry_script.md
+-rw-r--r--   0     1001      123      179 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-check_timeout.md
+-rw-r--r--   0     1001      123     1545 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/70-hook-scripts.md
+-rw-r--r--   0     1001      123      118 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-post_backup_script.md
+-rw-r--r--   0     1001      123      239 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-backup_compression_location.md
+-rw-r--r--   0     1001      123      403 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-pre_backup_retry_script.md
+-rw-r--r--   0     1001      123      546 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-last_backup_minimum_size.md
+-rw-r--r--   0     1001      123      272 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/15-description.md
+-rw-r--r--   0     1001      123      263 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5.d/50-gcp-zone.md
+-rw-r--r--   0     1001      123     7339 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-delete.1.md
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/barman.d/
+-rw-r--r--   0     1001      123     1500 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.d/streaming-server.conf-template
+-rw-r--r--   0     1001      123     1546 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.d/ssh-server.conf-template
+-rw-r--r--   0     1001      123      950 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.d/passive-server.conf-template
+-rw-r--r--   0     1001      123     3622 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-wal-restore.1
+-rw-r--r--   0     1001      123    11905 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-wal-archive.1
+-rw-r--r--   0     1001      123    11792 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup.1.md
+-rw-r--r--   0     1001      123     6891 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-show.1
+-rw-r--r--   0     1001      123    15433 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup.1
+-rw-r--r--   0     1001      123     5388 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-show.1.md
+-rw-r--r--   0     1001      123     8986 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-wal-archive.1.md
+-rw-r--r--   0     1001      123     2240 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-wal-archive.1.md
+-rw-r--r--   0     1001      123     5542 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-wal-restore.1.md
+-rw-r--r--   0     1001      123       47 2023-07-25 17:21:16.000000 barman-3.7.0/doc/.gitignore
+-rw-r--r--   0     1001      123     6746 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-list.1
+-rw-r--r--   0     1001      123     6990 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-check-wal-archive.1
+-rw-r--r--   0     1001      123     3066 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-wal-restore.1.md
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/build/
+-rwxr-xr-x   0     1001      123     1417 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/build
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/build/html-templates/
+-rw-r--r--   0     1001      123     1187 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/barman.css
+-rw-r--r--   0     1001      123    21298 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/docs.css
+-rw-r--r--   0     1001      123   147074 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/bootstrap.css
+-rw-r--r--   0     1001      123     5572 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/template.html
+-rw-r--r--   0     1001      123      111 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/template.css
+-rw-r--r--   0     1001      123     3520 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/template-cli.html
+-rw-r--r--   0     1001      123     3838 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/template-utils.html
+-rw-r--r--   0     1001      123      238 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/SOURCES.md
+-rw-r--r--   0     1001      123     1092 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/html-templates/override.css
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/build/templates/
+-rw-r--r--   0     1001      123     9952 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/Barman.tex
+-rw-r--r--   0     1001      123    81089 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/logo-horizontal-hires.png
+-rw-r--r--   0     1001      123      161 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/default.yaml
+-rw-r--r--   0     1001      123    16668 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/postgres.pdf
+-rw-r--r--   0     1001      123   102895 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/logo-hires.png
+-rw-r--r--   0     1001      123     6346 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/default.latex
+-rw-r--r--   0     1001      123     3895 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/templates/edb-enterprisedb-logo.png
+-rw-r--r--   0     1001      123     1750 2023-07-25 17:21:16.000000 barman-3.7.0/doc/build/Makefile
+-rw-r--r--   0     1001      123      706 2023-07-25 17:21:16.000000 barman-3.7.0/doc/Dockerfile
+-rw-r--r--   0     1001      123     8858 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-restore.1
+-rw-r--r--   0     1001      123     2630 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-wal-archive.1
+-rw-r--r--   0     1001      123     5704 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-keep.1.md
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/barman.1.d/
+-rw-r--r--   0     1001      123      368 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-sync-backup.md
+-rw-r--r--   0     1001      123      347 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/85-bugs.md
+-rw-r--r--   0     1001      123      174 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/99-copying.md
+-rw-r--r--   0     1001      123      241 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-show-servers.md
+-rw-r--r--   0     1001      123       55 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/45-commands.md
+-rw-r--r--   0     1001      123       51 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/75-exit-status.md
+-rw-r--r--   0     1001      123      266 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-archive-wal.md
+-rw-r--r--   0     1001      123       60 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/05-name.md
+-rw-r--r--   0     1001      123       81 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-switch-xlog.md
+-rw-r--r--   0     1001      123       61 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-verify.md
+-rw-r--r--   0     1001      123     1268 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-keep.md
+-rw-r--r--   0     1001      123       41 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/10-synopsis.md
+-rw-r--r--   0     1001      123       26 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/80-see-also.md
+-rw-r--r--   0     1001      123      155 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/95-resources.md
+-rw-r--r--   0     1001      123     3681 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-backup.md
+-rw-r--r--   0     1001      123       98 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-generate-manifest.md
+-rw-r--r--   0     1001      123      351 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-sync-wals.md
+-rw-r--r--   0     1001      123      110 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/00-header.md
+-rw-r--r--   0     1001      123      333 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-check-backup.md
+-rw-r--r--   0     1001      123      590 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-check-wal-archive.md
+-rw-r--r--   0     1001      123      668 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-receive-wal.md
+-rw-r--r--   0     1001      123      798 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-status.md
+-rw-r--r--   0     1001      123     1048 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-get-wal.md
+-rw-r--r--   0     1001      123      279 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-cron.md
+-rw-r--r--   0     1001      123       74 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-list-servers.md
+-rw-r--r--   0     1001      123      596 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/20-options.md
+-rw-r--r--   0     1001      123      295 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-rebuild-xlogdb.md
+-rw-r--r--   0     1001      123     6330 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-recover.md
+-rw-r--r--   0     1001      123      265 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-verify-backup.md
+-rw-r--r--   0     1001      123      701 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-put-wal.md
+-rw-r--r--   0     1001      123      578 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-replication-status.md
+-rw-r--r--   0     1001      123      291 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-list-backups.md
+-rw-r--r--   0     1001      123     1420 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-show-backup.md
+-rw-r--r--   0     1001      123      393 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-check.md
+-rw-r--r--   0     1001      123      788 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-list-files.md
+-rw-r--r--   0     1001      123      850 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-switch-wal.md
+-rw-r--r--   0     1001      123      621 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/90-authors.md
+-rw-r--r--   0     1001      123      642 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-sync-info.md
+-rw-r--r--   0     1001      123      143 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-delete.md
+-rw-r--r--   0     1001      123      444 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/70-backup-id-shortcuts.md
+-rw-r--r--   0     1001      123      272 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/15-description.md
+-rw-r--r--   0     1001      123      270 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1.d/50-diagnose.md
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/runbooks/
+-rw-r--r--   0     1001      123     9399 2023-07-25 17:21:16.000000 barman-3.7.0/doc/runbooks/snapshot_recovery_azure.md
+-rw-r--r--   0     1001      123    10478 2023-07-25 17:21:16.000000 barman-3.7.0/doc/runbooks/snapshot_recovery_aws.md
+-rw-r--r--   0     1001      123     7118 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-wal-restore.1
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/manual/
+-rw-r--r--   0     1001      123    13511 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/43-backup-commands.en.md
+-rw-r--r--   0     1001      123     4309 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/99-references.en.md
+-rw-r--r--   0     1001      123     1001 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/02-before_you_start.en.md
+-rw-r--r--   0     1001      123     2914 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/15-system_requirements.en.md
+-rw-r--r--   0     1001      123      862 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/22-config_file.en.md
+-rw-r--r--   0     1001      123      823 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/20-server_setup.en.md
+-rw-r--r--   0     1001      123       43 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/.gitignore
+-rw-r--r--   0     1001      123     3564 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/17-configuration.en.md
+-rw-r--r--   0     1001      123     1732 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/65-troubleshooting.en.md
+-rw-r--r--   0     1001      123    50257 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/50-feature-details.en.md
+-rw-r--r--   0     1001      123     1017 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/26-rsync_backup.en.md
+-rw-r--r--   0     1001      123     8285 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/28-snapshots.en.md
+-rw-r--r--   0     1001      123    10741 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/55-barman-cli.en.md
+-rw-r--r--   0     1001      123    11160 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/10-design.en.md
+-rw-r--r--   0     1001      123      784 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/00-head.en.md
+-rw-r--r--   0     1001      123     9313 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/21-preliminary_steps.en.md
+-rw-r--r--   0     1001      123     1335 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/30-windows-support.en.md
+-rw-r--r--   0     1001      123     3665 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/66-about.en.md
+-rw-r--r--   0     1001      123     5034 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/23-wal_streaming.en.md
+-rw-r--r--   0     1001      123     2629 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/41-global-commands.en.md
+-rw-r--r--   0     1001      123     4014 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/01-intro.en.md
+-rw-r--r--   0     1001      123     1083 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/25-streaming_backup.en.md
+-rw-r--r--   0     1001      123      667 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/Makefile
+-rw-r--r--   0     1001      123    10192 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/16-installation.en.md
+-rw-r--r--   0     1001      123     5283 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/24-wal_archiving.en.md
+-rw-r--r--   0     1001      123    11271 2023-07-25 17:21:16.000000 barman-3.7.0/doc/manual/42-server-commands.en.md
+-rw-r--r--   0     1001      123     6891 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-restore.1.md
+-rw-r--r--   0     1001      123    27807 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.1
+-rw-r--r--   0     1001      123     3501 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.conf
+-rw-r--r--   0     1001      123     2331 2023-07-25 17:21:16.000000 barman-3.7.0/doc/Makefile
+-rw-r--r--   0     1001      123    32413 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman.5
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/doc/images/
+-rw-r--r--   0     1001      123   227695 2023-07-25 17:21:16.000000 barman-3.7.0/doc/images/barman-architecture-scenario1b.png
+-rw-r--r--   0     1001      123   228769 2023-07-25 17:21:16.000000 barman-3.7.0/doc/images/barman-architecture-scenario2b.png
+-rw-r--r--   0     1001      123   179610 2023-07-25 17:21:16.000000 barman-3.7.0/doc/images/barman-architecture-scenario1.png
+-rw-r--r--   0     1001      123   201845 2023-07-25 17:21:16.000000 barman-3.7.0/doc/images/barman-architecture-scenario2.png
+-rw-r--r--   0     1001      123   157428 2023-07-25 17:21:16.000000 barman-3.7.0/doc/images/barman-architecture-georedundancy.png
+-rw-r--r--   0     1001      123     7328 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-keep.1
+-rw-r--r--   0     1001      123     5279 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-backup-list.1.md
+-rw-r--r--   0     1001      123     5470 2023-07-25 17:21:16.000000 barman-3.7.0/doc/barman-cloud-check-wal-archive.1.md
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/
+-rw-r--r--   0     1001      123     1509 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/PKG-INFO
+-rw-r--r--   0     1001      123        7 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/top_level.txt
+-rw-r--r--   0     1001      123     9735 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      123      281 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/requires.txt
+-rw-r--r--   0     1001      123        1 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      123      729 2023-07-25 17:21:44.000000 barman-3.7.0/barman.egg-info/entry_points.txt
+-rw-r--r--   0     1001      123     1277 2023-07-25 17:21:16.000000 barman-3.7.0/AUTHORS
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/scripts/
+-rw-r--r--   0     1001      123       98 2023-07-25 17:21:16.000000 barman-3.7.0/scripts/barman.bash_completion
+-rwxr-xr-x   0     1001      123     4969 2023-07-25 17:21:16.000000 barman-3.7.0/setup.py
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/barman/
+-rw-r--r--   0     1001      123   164482 2023-07-25 17:21:16.000000 barman-3.7.0/barman/server.py
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/barman/clients/
+-rw-r--r--   0     1001      123     3147 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_check_wal_archive.py
+-rwxr-xr-x   0     1001      123    14508 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_backup.py
+-rw-r--r--   0     1001      123    18001 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_backup_delete.py
+-rwxr-xr-x   0     1001      123    11355 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_walarchive.py
+-rwxr-xr-x   0     1001      123    11331 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/walarchive.py
+-rw-r--r--   0     1001      123    13885 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_restore.py
+-rw-r--r--   0     1001      123     4344 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_backup_keep.py
+-rwxr-xr-x   0     1001      123    16333 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/walrestore.py
+-rw-r--r--   0     1001      123     3720 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_backup_show.py
+-rw-r--r--   0     1001      123     6705 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_walrestore.py
+-rw-r--r--   0     1001      123     4438 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_backup_list.py
+-rw-r--r--   0     1001      123      724 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/__init__.py
+-rw-r--r--   0     1001      123     6498 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_cli.py
+-rw-r--r--   0     1001      123     6302 2023-07-25 17:21:16.000000 barman-3.7.0/barman/clients/cloud_compression.py
+-rw-r--r--   0     1001      123      805 2023-07-25 17:21:42.000000 barman-3.7.0/barman/version.py
+-rw-r--r--   0     1001      123    89090 2023-07-25 17:21:16.000000 barman-3.7.0/barman/backup_executor.py
+-rw-r--r--   0     1001      123    63696 2023-07-25 17:21:16.000000 barman-3.7.0/barman/postgres.py
+-rw-r--r--   0     1001      123    45270 2023-07-25 17:21:16.000000 barman-3.7.0/barman/command_wrappers.py
+-rw-r--r--   0     1001      123    12760 2023-07-25 17:21:16.000000 barman-3.7.0/barman/annotations.py
+-rw-r--r--   0     1001      123    17247 2023-07-25 17:21:16.000000 barman-3.7.0/barman/xlog.py
+-rw-r--r--   0     1001      123    33055 2023-07-25 17:21:16.000000 barman-3.7.0/barman/compression.py
+-rw-r--r--   0     1001      123     4343 2023-07-25 17:21:16.000000 barman-3.7.0/barman/diagnose.py
+-rw-r--r--   0     1001      123    28226 2023-07-25 17:21:16.000000 barman-3.7.0/barman/infofile.py
+-rw-r--r--   0     1001      123    96662 2023-07-25 17:21:16.000000 barman-3.7.0/barman/cloud.py
+-rw-r--r--   0     1001      123    40768 2023-07-25 17:21:16.000000 barman-3.7.0/barman/config.py
+-rw-r--r--   0     1001      123    77879 2023-07-25 17:21:16.000000 barman-3.7.0/barman/output.py
+-rw-r--r--   0     1001      123    49647 2023-07-25 17:21:16.000000 barman-3.7.0/barman/copy_controller.py
+-rw-r--r--   0     1001      123     4215 2023-07-25 17:21:16.000000 barman-3.7.0/barman/postgres_plumbing.py
+-rw-r--r--   0     1001      123     5959 2023-07-25 17:21:16.000000 barman-3.7.0/barman/process.py
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/barman/storage/
+-rw-r--r--   0     1001      123     1679 2023-07-25 17:21:16.000000 barman-3.7.0/barman/storage/file_stats.py
+-rw-r--r--   0     1001      123     2397 2023-07-25 17:21:16.000000 barman-3.7.0/barman/storage/local_file_manager.py
+-rw-r--r--   0     1001      123      724 2023-07-25 17:21:16.000000 barman-3.7.0/barman/storage/__init__.py
+-rw-r--r--   0     1001      123     1799 2023-07-25 17:21:16.000000 barman-3.7.0/barman/storage/file_manager.py
+-rw-r--r--   0     1001      123    26369 2023-07-25 17:21:16.000000 barman-3.7.0/barman/utils.py
+-rw-r--r--   0     1001      123    62463 2023-07-25 17:21:16.000000 barman-3.7.0/barman/backup.py
+-rw-r--r--   0     1001      123    11374 2023-07-25 17:21:16.000000 barman-3.7.0/barman/lockfile.py
+-rw-r--r--   0     1001      123     2315 2023-07-25 17:21:16.000000 barman-3.7.0/barman/remote_status.py
+drwxr-xr-x   0     1001      123        0 2023-07-25 17:21:44.000000 barman-3.7.0/barman/cloud_providers/
+-rw-r--r--   0     1001      123    40361 2023-07-25 17:21:16.000000 barman-3.7.0/barman/cloud_providers/azure_blob_storage.py
+-rw-r--r--   0     1001      123    13574 2023-07-25 17:21:16.000000 barman-3.7.0/barman/cloud_providers/__init__.py
+-rw-r--r--   0     1001      123    31558 2023-07-25 17:21:16.000000 barman-3.7.0/barman/cloud_providers/google_cloud_storage.py
+-rw-r--r--   0     1001      123    42005 2023-07-25 17:21:16.000000 barman-3.7.0/barman/cloud_providers/aws_s3.py
+-rw-r--r--   0     1001      123      890 2023-07-25 17:21:16.000000 barman-3.7.0/barman/__init__.py
+-rw-r--r--   0     1001      123    81412 2023-07-25 17:21:16.000000 barman-3.7.0/barman/recovery_executor.py
+-rw-r--r--   0     1001      123    19109 2023-07-25 17:21:16.000000 barman-3.7.0/barman/retention_policies.py
+-rw-r--r--   0     1001      123    11394 2023-07-25 17:21:16.000000 barman-3.7.0/barman/hooks.py
+-rw-r--r--   0     1001      123     9808 2023-07-25 17:21:16.000000 barman-3.7.0/barman/exceptions.py
+-rw-r--r--   0     1001      123     5491 2023-07-25 17:21:16.000000 barman-3.7.0/barman/backup_manifest.py
+-rw-r--r--   0     1001      123    19890 2023-07-25 17:21:16.000000 barman-3.7.0/barman/fs.py
+-rw-r--r--   0     1001      123    42482 2023-07-25 17:21:16.000000 barman-3.7.0/barman/wal_archiver.py
+-rw-r--r--   0     1001      123    70013 2023-07-25 17:21:16.000000 barman-3.7.0/barman/cli.py
+-rw-r--r--   0     1001      123    56701 2023-07-25 17:21:16.000000 barman-3.7.0/NEWS
```

### Comparing `barman-3.6.0/doc/build/build` & `barman-3.7.0/doc/build/build`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/templates/logo-horizontal-hires.png` & `barman-3.7.0/doc/build/templates/logo-horizontal-hires.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/templates/default.latex` & `barman-3.7.0/doc/build/templates/default.latex`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/templates/postgres.pdf` & `barman-3.7.0/doc/build/templates/postgres.pdf`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/templates/edb-enterprisedb-logo.png` & `barman-3.7.0/doc/build/templates/edb-enterprisedb-logo.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/templates/logo-hires.png` & `barman-3.7.0/doc/build/templates/logo-hires.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/templates/Barman.tex` & `barman-3.7.0/doc/build/templates/Barman.tex`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/template-utils.html` & `barman-3.7.0/doc/build/html-templates/template-utils.html`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/barman.css` & `barman-3.7.0/doc/build/html-templates/barman.css`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/docs.css` & `barman-3.7.0/doc/build/html-templates/docs.css`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/bootstrap.css` & `barman-3.7.0/doc/build/html-templates/bootstrap.css`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/template.html` & `barman-3.7.0/doc/build/html-templates/template.html`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/template-cli.html` & `barman-3.7.0/doc/build/html-templates/template-cli.html`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/html-templates/override.css` & `barman-3.7.0/doc/build/html-templates/override.css`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/build/Makefile` & `barman-3.7.0/doc/build/Makefile`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman-wal-archive.1.md` & `barman-3.7.0/doc/barman-wal-archive.1.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-WAL-ARCHIVE(1) Barman User manuals | Version 3.6.0
+% BARMAN-WAL-ARCHIVE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-wal-archive - `archive_command` based on Barman's put-wal
 
 
 # SYNOPSIS
```

### Comparing `barman-3.6.0/doc/barman.5.d/30-configuration-file-directory.md` & `barman-3.7.0/doc/barman.5.d/30-configuration-file-directory.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-primary_conninfo.md` & `barman-3.7.0/doc/barman.5.d/50-primary_conninfo.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-backup_method.md` & `barman-3.7.0/doc/barman.5.d/50-backup_method.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-backup_options.md` & `barman-3.7.0/doc/barman.5.d/50-backup_options.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-backup_compression.md` & `barman-3.7.0/doc/barman.5.d/50-backup_compression.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/75-example.md` & `barman-3.7.0/doc/barman.5.d/75-example.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/90-authors.md` & `barman-3.7.0/doc/barman.5.d/90-authors.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-custom_compression_magic.md` & `barman-3.7.0/doc/barman.5.d/50-custom_compression_magic.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-recovery_staging_path.md` & `barman-3.7.0/doc/barman.5.d/50-recovery_staging_path.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-retention_policy.md` & `barman-3.7.0/doc/barman.5.d/50-retention_policy.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-streaming_archiver.md` & `barman-3.7.0/doc/barman.5.d/50-streaming_archiver.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/50-last_backup_minimum_size.md` & `barman-3.7.0/doc/barman.5.d/50-last_backup_minimum_size.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5.d/70-hook-scripts.md` & `barman-3.7.0/doc/barman.5.d/70-hook-scripts.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/runbooks/snapshot_recovery_azure.md` & `barman-3.7.0/doc/runbooks/snapshot_recovery_azure.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.5` & `barman-3.7.0/doc/barman.5`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN" "5" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN" "5" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman \- Backup and Recovery Manager for PostgreSQL
 .SH DESCRIPTION
 .PP
 Barman is an administration tool for disaster recovery of PostgreSQL
@@ -92,14 +92,41 @@
 would limit itself to maximum \f[C]archiver_batch_size\f[] WAL segments
 per single run.
 Integer.
 Global/Server.
 .RS
 .RE
 .TP
+.B autogenerate_manifest
+This option enables the auto\-generation of backup manifest files for
+rsync based backups and strategies.
+The manifest file is a JSON file containing the list of files contained
+in the backup.
+It is generated at the end of the backup process and stored in the
+backup directory.
+The manifest file generated follows the format described in the
+postgesql documentation, and is compatible with the
+\f[C]pg_verifybackup\f[] tool.
+The option is ignored if the backup method is not rsync.
+.RS
+.RE
+.TP
+.B aws_profile
+The name of the AWS profile to use when authenticating with AWS (e.g.
+INI section in AWS credentials file).
+Global/Server.
+aws_region
+.RS
+.RE
+The name of the AWS region containing the EC2 VM and storage volumes
+defined by \f[C]snapshot_instance\f[] and \f[C]snapshot_disks\f[].
+Global/Server.
+.RS
+.RE
+.TP
 .B azure_credential
 The credential type (either \f[C]azure\-cli\f[] or
 \f[C]managed\-identity\f[]) to use when authenticating with Azure.
 If this is omitted then the default Azure authentication flow will be
 used.
 Global/Server.
 .RS
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-keep.1.md` & `barman-3.7.0/doc/barman-cloud-backup-keep.1.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-backup-keep - Flag backups which should be kept forever
 
 
 # SYNOPSIS
@@ -22,15 +22,16 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-backup-keep [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                                [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                                [--endpoint-url ENDPOINT_URL]
+                                [-P AWS_PROFILE] [--profile AWS_PROFILE]
                                 [--read-timeout READ_TIMEOUT]
                                 [--azure-credential {azure-cli,managed-identity}]
                                 (-r | -s | --target {full,standalone})
                                 source_url server_name backup_id
 
 This script can be used to tag backups in cloud storage as archival backups
 such that they will not be deleted. Currently AWS S3, Azure Blob Storage and
@@ -56,17 +57,19 @@
   -s, --status          Print the keep status of the backup
   --target {full,standalone}
                         Specify the recovery target for this backup
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-restore.1.md` & `barman-3.7.0/doc/barman-cloud-restore.1.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-RESTORE(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-RESTORE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-restore - Restore a PostgreSQL backup from the Cloud
 
 
 # SYNOPSIS
@@ -26,21 +26,22 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-restore [-V] [--help] [-v | -q] [-t]
                             [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                            [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                            [--endpoint-url ENDPOINT_URL] [-P AWS_PROFILE]
+                            [--profile AWS_PROFILE]
                             [--read-timeout READ_TIMEOUT]
                             [--azure-credential {azure-cli,managed-identity}]
                             [--tablespace NAME:LOCATION]
                             [--snapshot-recovery-instance SNAPSHOT_RECOVERY_INSTANCE]
                             [--snapshot-recovery-zone GCP_ZONE]
-                            [--gcp-zone GCP_ZONE]
+                            [--aws-region AWS_REGION] [--gcp-zone GCP_ZONE]
                             [--azure-resource-group AZURE_RESOURCE_GROUP]
                             source_url server_name backup_id recovery_dir
 
 This script can be used to download a backup previously made with barman-
 cloud-backup command.Currently AWS S3, Azure Blob Storage and Google Cloud
 Storage are supported.
 
@@ -67,21 +68,26 @@
   --snapshot-recovery-zone GCP_ZONE
                         Zone containing the instance and disks for the
                         snapshot recovery (deprecated: replaced by --gcp-zone)
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
+  --aws-region AWS_REGION
+                        Name of the AWS region where the instance and disks
+                        for snapshot recovery are located
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
                         authenticating with Azure. If omitted then Azure Blob
                         Storage credentials will be obtained from the
                         environment and the default Azure authentication flow
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-list.1` & `barman-3.7.0/doc/barman-cloud-backup-list.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-LIST" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-LIST" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup\-list \- List backups stored in the Cloud
 .SH SYNOPSIS
 .PP
 barman\-cloud\-backup\-list [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
@@ -20,15 +20,16 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\-list\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ AWS_PROFILE]\ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-format\ FORMAT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name
 
 This\ script\ can\ be\ used\ to\ list\ backups\ made\ with\ barman\-cloud\-backup\ command.
 Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage\ are\ supported.
@@ -47,17 +48,19 @@
 \ \ \-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
 \ \ \-\-format\ FORMAT\ \ \ \ \ \ \ Output\ format\ (console\ or\ json).\ Default\ console.
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-wal-archive.1` & `barman-3.7.0/doc/barman-cloud-wal-archive.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-WAL\-ARCHIVE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-WAL\-ARCHIVE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-wal\-archive \- Archive PostgreSQL WAL files in the Cloud
 using \f[C]archive_command\f[]
 .SH SYNOPSIS
 .PP
@@ -27,15 +27,16 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-wal\-archive\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ AWS_PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-z\ |\ \-j\ |\ \-\-snappy]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tags\ [TAGS\ [TAGS\ ...]]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-history\-tags\ [HISTORY_TAGS\ [HISTORY_TAGS\ ...]]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-kms\-key\-name\ KMS_KEY_NAME]\ [\-e\ ENCRYPTION]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID]
@@ -76,17 +77,19 @@
 \ \ \-\-history\-tags\ [HISTORY_TAGS\ [HISTORY_TAGS\ ...]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Tags\ to\ be\ added\ to\ archived\ history\ files\ in\ cloud
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ storage
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 \ \ \-e\ ENCRYPTION,\ \-\-encryption\ ENCRYPTION
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ encryption\ algorithm\ used\ when\ storing\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ uploaded\ data\ in\ S3.\ Allowed\ values:
```

### Comparing `barman-3.6.0/doc/barman-cloud-check-wal-archive.1.md` & `barman-3.7.0/doc/barman-cloud-check-wal-archive.1.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-CHECK-WAL-ARCHIVE(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-CHECK-WAL-ARCHIVE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-check-wal-archive - Check a WAL archive destination for a new PostgreSQL cluster
 
 
 # SYNOPSIS
@@ -24,15 +24,15 @@
 
 
 # Usage
 ```
 usage: barman-cloud-check-wal-archive [-V] [--help] [-v | -q] [-t]
                                       [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
                                       [--endpoint-url ENDPOINT_URL]
-                                      [-P PROFILE]
+                                      [-P AWS_PROFILE] [--profile AWS_PROFILE]
                                       [--read-timeout READ_TIMEOUT]
                                       [--azure-credential {azure-cli,managed-identity}]
                                       [--timeline TIMELINE]
                                       destination_url server_name
 
 Checks that the WAL archive on the specified cloud storage can be safely used
 for a new PostgreSQL server.
@@ -52,17 +52,19 @@
                         The cloud provider to use as a storage backend
   --timeline TIMELINE   The earliest timeline whose WALs should cause the
                         check to fail
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-delete.1` & `barman-3.7.0/doc/barman-cloud-backup-delete.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup\-delete \- Delete backups stored in the Cloud
 .SH SYNOPSIS
 .PP
 barman\-cloud\-backup\-delete [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
@@ -45,15 +45,16 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\-delete\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ AWS_PROFILE]\ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ (\-b\ BACKUP_ID\ |\ \-r\ RETENTION_POLICY)
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-dry\-run]\ [\-\-batch\-size\ DELETE_BATCH_SIZE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name
 
 This\ script\ can\ be\ used\ to\ delete\ backups\ made\ with\ barman\-cloud\-backup
@@ -88,17 +89,19 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ maximum\ allowed\ batch\ size\ for\ the\ specified\ cloud
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ provider\ will\ be\ used\ (1000\ for\ aws\-s3,\ 256\ for\ azure\-
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ blob\-storage\ and\ 100\ for\ google\-cloud\-storage).
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-wal-restore.1.md` & `barman-3.7.0/doc/barman-cloud-wal-restore.1.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-WAL-RESTORE(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-WAL-RESTORE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-wal-restore - Restore PostgreSQL WAL files from the Cloud using `restore_command`
 
 
 # SYNOPSIS
@@ -22,15 +22,16 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-wal-restore [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                                [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                                [--endpoint-url ENDPOINT_URL] [-P AWS_PROFILE]
+                                [--profile AWS_PROFILE]
                                 [--read-timeout READ_TIMEOUT]
                                 [--azure-credential {azure-cli,managed-identity}]
                                 source_url server_name wal_name wal_dest
 
 This script can be used as a `restore_command` to download WAL files
 previously archived with barman-cloud-wal-archive command. Currently AWS S3,
 Azure Blob Storage and Google Cloud Storage are supported.
@@ -52,17 +53,19 @@
   -t, --test            Test cloud connectivity and exit
   --cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}
                         The cloud provider to use as a storage backend
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-show.1.md` & `barman-3.7.0/doc/barman-cloud-backup-show.1.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-SHOW(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-BACKUP-SHOW(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-backup-show - Show metadata for a backup stored in the Cloud
 
 
 # SYNOPSIS
@@ -22,15 +22,16 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-backup-show [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                                [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                                [--endpoint-url ENDPOINT_URL]
+                                [-P AWS_PROFILE] [--profile AWS_PROFILE]
                                 [--read-timeout READ_TIMEOUT]
                                 [--azure-credential {azure-cli,managed-identity}]
                                 [--format FORMAT]
                                 source_url server_name backup_id
 
 This script can be used to show metadata for backups made with barman-cloud-
 backup command. Currently AWS S3, Azure Blob Storage and Google Cloud Storage
@@ -51,17 +52,19 @@
   --cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}
                         The cloud provider to use as a storage backend
   --format FORMAT       Output format (console or json). Default console.
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup.1.md` & `barman-3.7.0/doc/barman-cloud-backup.1.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-BACKUP(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-backup - Backup a PostgreSQL instance and stores it in the Cloud
 
 
 # SYNOPSIS
@@ -38,27 +38,29 @@
 parameter.
 
 
 # Usage
 ```
 usage: barman-cloud-backup [-V] [--help] [-v | -q] [-t]
                            [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                           [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                           [--endpoint-url ENDPOINT_URL] [-P AWS_PROFILE]
+                           [--profile AWS_PROFILE]
                            [--read-timeout READ_TIMEOUT]
                            [--azure-credential {azure-cli,managed-identity}]
                            [-z | -j | --snappy] [-h HOST] [-p PORT] [-U USER]
                            [--immediate-checkpoint] [-J JOBS]
                            [-S MAX_ARCHIVE_SIZE] [-d DBNAME] [-n BACKUP_NAME]
                            [--snapshot-instance SNAPSHOT_INSTANCE]
                            [--snapshot-disk NAME] [--snapshot-zone GCP_ZONE]
                            [--snapshot-gcp-project GCP_PROJECT]
                            [--gcp-project GCP_PROJECT]
                            [--kms-key-name KMS_KEY_NAME] [--gcp-zone GCP_ZONE]
                            [--tags [TAGS [TAGS ...]]] [-e {AES256,aws:kms}]
                            [--sse-kms-key-id SSE_KMS_KEY_ID]
+                           [--aws-region AWS_REGION]
                            [--encryption-scope ENCRYPTION_SCOPE]
                            [--azure-subscription-id AZURE_SUBSCRIPTION_ID]
                            [--azure-resource-group AZURE_RESOURCE_GROUP]
                            destination_url server_name
 
 This script can be used to perform a backup of a local PostgreSQL instance and
 ship the resulting tarball(s) to the Cloud. Currently AWS S3, Azure Blob
@@ -111,30 +113,36 @@
   --tags [TAGS [TAGS ...]]
                         Tags to be added to all uploaded files in cloud
                         storage
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
   -e {AES256,aws:kms}, --encryption {AES256,aws:kms}
                         The encryption algorithm used when storing the
                         uploaded data in S3. Allowed values:
                         'AES256'|'aws:kms'.
   --sse-kms-key-id SSE_KMS_KEY_ID
                         The AWS KMS key ID that should be used for encrypting
                         the uploaded data in S3. Can be specified using the
                         key ID on its own or using the full ARN for the key.
                         Only allowed if `-e/--encryption` is set to `aws:kms`.
+  --aws-region AWS_REGION
+                        The name of the AWS region containing the EC2 VM and
+                        storage volumes defined by the --snapshot-instance and
+                        --snapshot-disk arguments.
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
                         Optionally specify the type of credential to use when
                         authenticating with Azure. If omitted then Azure Blob
                         Storage credentials will be obtained from the
                         environment and the default Azure authentication flow
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-list.1.md` & `barman-3.7.0/doc/barman-cloud-backup-list.1.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-LIST(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-BACKUP-LIST(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-backup-list - List backups stored in the Cloud
 
 
 # SYNOPSIS
@@ -22,15 +22,16 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-backup-list [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                                [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                                [--endpoint-url ENDPOINT_URL]
+                                [-P AWS_PROFILE] [--profile AWS_PROFILE]
                                 [--read-timeout READ_TIMEOUT]
                                 [--azure-credential {azure-cli,managed-identity}]
                                 [--format FORMAT]
                                 source_url server_name
 
 This script can be used to list backups made with barman-cloud-backup command.
 Currently AWS S3, Azure Blob Storage and Google Cloud Storage are supported.
@@ -49,17 +50,19 @@
   --cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}
                         The cloud provider to use as a storage backend
   --format FORMAT       Output format (console or json). Default console.
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
```

### Comparing `barman-3.6.0/doc/barman.1` & `barman-3.7.0/doc/barman.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman \- Backup and Recovery Manager for PostgreSQL
 .SH SYNOPSIS
 .PP
 barman [\f[I]OPTIONS\f[]] \f[I]COMMAND\f[]
@@ -174,14 +174,31 @@
 .RE
 .TP
 .B \-\-wait\-timeout
 the time, in seconds, spent waiting for the required WAL files to be
 archived before timing out
 .RS
 .RE
+.TP
+.B \-\-manifest
+forces the creation of a backup manifest file at the end of a backup.
+Overrides value of the parameter \f[C]autogenerate_manifest\f[], from
+the configuration file.
+Works with rsync backup method and strategies only
+.RS
+.RE
+.TP
+.B \-\-no\-manifest
+disables the automatic creation of a backup manifest file at the end of
+a backup.
+Overrides value of the parameter \f[C]autogenerate_manifest\f[], from
+the configuration file.
+Works with rsync backup method and strategies only
+.RS
+.RE
 .RE
 .TP
 .B check\-backup \f[I]SERVER_NAME\f[] \f[I]BACKUP_ID\f[]
 Make sure that all the required WAL files to check the consistency of a
 physical backup (that is, from the beginning to the end of the full
 backup) are correctly archived.
 This command is automatically invoked by the \f[C]cron\f[] command and
@@ -628,18 +645,34 @@
 attached.
 This option is required when recovering backups made with
 \f[C]backup_method\ =\ snapshot\f[].
 .RS
 .RE
 .TP
 .B \-\-gcp\-zone \f[I]ZONE_NAME\f[]
-Name of the availability zone where the instance and disks for snapshot
+Name of the GCP zone where the instance and disks for snapshot recovery
 are located.
-This option is required when recovering backups made with
-\f[C]backup_method\ =\ snapshot\f[].
+This option can be used to override the value of \f[C]gcp_zone\f[] in
+the Barman config.
+.RS
+.RE
+.TP
+.B \-\-azure\-resource\-group \f[I]RESOURCE_GROUP_NAME\f[]
+Name of the Azure resource group containing the instance and disks for
+snapshot recovery.
+This option can be used to override the value of
+\f[C]azure_resource_group\f[] in the Barman config.
+.RS
+.RE
+.TP
+.B \-\-aws\-region \f[I]REGION_NAME\f[]
+Name of the AWS region where the instance and disks for snapshot
+recovery are located.
+This option can be used to override the value of \f[C]aws_region\f[] in
+the Barman config.
 .RS
 .RE
 .RE
 .TP
 .B replication\-status \f[I][OPTIONS]\f[] \f[I]SERVER_NAME\f[]
 Shows live information and status of any streaming client attached to
 the given server (or servers).
```

### Comparing `barman-3.6.0/doc/barman-cloud-wal-archive.1.md` & `barman-3.7.0/doc/barman-cloud-wal-archive.1.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-WAL-ARCHIVE(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-WAL-ARCHIVE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-wal-archive - Archive PostgreSQL WAL files in the Cloud using `archive_command`
 
 
 # SYNOPSIS
@@ -27,15 +27,16 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-wal-archive [-V] [--help] [-v | -q] [-t]
                                 [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                                [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                                [--endpoint-url ENDPOINT_URL] [-P AWS_PROFILE]
+                                [--profile AWS_PROFILE]
                                 [--read-timeout READ_TIMEOUT]
                                 [--azure-credential {azure-cli,managed-identity}]
                                 [-z | -j | --snappy]
                                 [--tags [TAGS [TAGS ...]]]
                                 [--history-tags [HISTORY_TAGS [HISTORY_TAGS ...]]]
                                 [--kms-key-name KMS_KEY_NAME] [-e ENCRYPTION]
                                 [--sse-kms-key-id SSE_KMS_KEY_ID]
@@ -76,17 +77,19 @@
   --history-tags [HISTORY_TAGS [HISTORY_TAGS ...]]
                         Tags to be added to archived history files in cloud
                         storage
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
   -e ENCRYPTION, --encryption ENCRYPTION
                         The encryption algorithm used when storing the
                         uploaded data in S3. Allowed values:
```

### Comparing `barman-3.6.0/doc/barman-cloud-restore.1` & `barman-3.7.0/doc/barman-cloud-restore.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-RESTORE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-RESTORE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-restore \- Restore a PostgreSQL backup from the Cloud
 .SH SYNOPSIS
 .PP
 barman\-cloud\-restore [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
@@ -24,21 +24,22 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-restore\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ AWS_PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tablespace\ NAME:LOCATION]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-recovery\-instance\ SNAPSHOT_RECOVERY_INSTANCE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-recovery\-zone\ GCP_ZONE]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-gcp\-zone\ GCP_ZONE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-aws\-region\ AWS_REGION]\ [\-\-gcp\-zone\ GCP_ZONE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-resource\-group\ AZURE_RESOURCE_GROUP]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id\ recovery_dir
 
 This\ script\ can\ be\ used\ to\ download\ a\ backup\ previously\ made\ with\ barman\-
 cloud\-backup\ command.Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud
 Storage\ are\ supported.
 
@@ -65,21 +66,26 @@
 \ \ \-\-snapshot\-recovery\-zone\ GCP_ZONE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Zone\ containing\ the\ instance\ and\ disks\ for\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ snapshot\ recovery\ (deprecated:\ replaced\ by\ \-\-gcp\-zone)
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
+\ \ \-\-aws\-region\ AWS_REGION
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Name\ of\ the\ AWS\ region\ where\ the\ instance\ and\ disks
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ for\ snapshot\ recovery\ are\ located
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
```

### Comparing `barman-3.6.0/doc/barman-cloud-wal-restore.1` & `barman-3.7.0/doc/barman-cloud-wal-restore.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-WAL\-RESTORE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-WAL\-RESTORE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-wal\-restore \- Restore PostgreSQL WAL files from the
 Cloud using \f[C]restore_command\f[]
 .SH SYNOPSIS
 .PP
@@ -22,15 +22,16 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-wal\-restore\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ AWS_PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ wal_name\ wal_dest
 
 This\ script\ can\ be\ used\ as\ a\ `restore_command`\ to\ download\ WAL\ files
 previously\ archived\ with\ barman\-cloud\-wal\-archive\ command.\ Currently\ AWS\ S3,
 Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage\ are\ supported.
@@ -52,17 +53,19 @@
 \ \ \-t,\ \-\-test\ \ \ \ \ \ \ \ \ \ \ \ Test\ cloud\ connectivity\ and\ exit
 \ \ \-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
```

### Comparing `barman-3.6.0/doc/Dockerfile` & `barman-3.7.0/doc/Dockerfile`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman-wal-restore.1.md` & `barman-3.7.0/doc/barman-wal-restore.1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-WAL-RESTORE(1) Barman User manuals | Version 3.6.0
+% BARMAN-WAL-RESTORE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-wal-restore - 'restore_command' based on Barman's get-wal
 
 
 # SYNOPSIS
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-show.1` & `barman-3.7.0/doc/barman-cloud-backup-show.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-SHOW" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-SHOW" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup\-show \- Show metadata for a backup stored in the
 Cloud
 .SH SYNOPSIS
 .PP
@@ -21,15 +21,16 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\-show\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ AWS_PROFILE]\ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-format\ FORMAT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id
 
 This\ script\ can\ be\ used\ to\ show\ metadata\ for\ backups\ made\ with\ barman\-cloud\-
 backup\ command.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and\ Google\ Cloud\ Storage
@@ -50,17 +51,19 @@
 \ \ \-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
 \ \ \-\-format\ FORMAT\ \ \ \ \ \ \ Output\ format\ (console\ or\ json).\ Default\ console.
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-delete.1.md` & `barman-3.7.0/doc/barman-cloud-backup-delete.1.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.6.0
+% BARMAN-CLOUD-BACKUP-DELETE(1) Barman User manuals | Version 3.7.0
 % EnterpriseDB <https://www.enterprisedb.com>
-% June 15, 2023
+% July 25, 2023
 
 # NAME
 
 barman-cloud-backup-delete - Delete backups stored in the Cloud
 
 
 # SYNOPSIS
@@ -42,15 +42,16 @@
 of PostgreSQL servers written in Python and maintained by EnterpriseDB.
 
 
 # Usage
 ```
 usage: barman-cloud-backup-delete [-V] [--help] [-v | -q] [-t]
                                   [--cloud-provider {aws-s3,azure-blob-storage,google-cloud-storage}]
-                                  [--endpoint-url ENDPOINT_URL] [-P PROFILE]
+                                  [--endpoint-url ENDPOINT_URL]
+                                  [-P AWS_PROFILE] [--profile AWS_PROFILE]
                                   [--read-timeout READ_TIMEOUT]
                                   [--azure-credential {azure-cli,managed-identity}]
                                   (-b BACKUP_ID | -r RETENTION_POLICY)
                                   [--dry-run] [--batch-size DELETE_BATCH_SIZE]
                                   source_url server_name
 
 This script can be used to delete backups made with barman-cloud-backup
@@ -85,17 +86,19 @@
                         the maximum allowed batch size for the specified cloud
                         provider will be used (1000 for aws-s3, 256 for azure-
                         blob-storage and 100 for google-cloud-storage).
 
 Extra options for the aws-s3 cloud provider:
   --endpoint-url ENDPOINT_URL
                         Override default S3 endpoint URL with the given one
-  -P PROFILE, --profile PROFILE
+  -P AWS_PROFILE, --aws-profile AWS_PROFILE
                         profile name (e.g. INI section in AWS credentials
                         file)
+  --profile AWS_PROFILE
+                        profile name (deprecated: replaced by --aws-profile)
   --read-timeout READ_TIMEOUT
                         the time in seconds until a timeout is raised when
                         waiting to read from a connection (defaults to 60
                         seconds)
 
 Extra options for the azure-blob-storage cloud provider:
   --azure-credential {azure-cli,managed-identity}, --credential {azure-cli,managed-identity}
```

### Comparing `barman-3.6.0/doc/barman.d/passive-server.conf-template` & `barman-3.7.0/doc/barman.d/passive-server.conf-template`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.d/ssh-server.conf-template` & `barman-3.7.0/doc/barman.d/ssh-server.conf-template`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.d/streaming-server.conf-template` & `barman-3.7.0/doc/barman.d/streaming-server.conf-template`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-list-files.md` & `barman-3.7.0/doc/barman.1.d/50-list-files.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-switch-wal.md` & `barman-3.7.0/doc/barman.1.d/50-switch-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-backup.md` & `barman-3.7.0/doc/barman.1.d/50-backup.md`

 * *Files 13% similar despite different names*

```diff
@@ -70,7 +70,20 @@
 
     --wait, -w
     :   wait for all required WAL files by the base backup to be archived
 
     --wait-timeout
     :   the time, in seconds, spent waiting for the required WAL
         files to be archived before timing out
+
+    --manifest
+    :   forces the creation of a backup manifest file at the end of a backup. 
+        Overrides value of the parameter `autogenerate_manifest`, 
+        from the configuration file. 
+        Works with rsync backup method and strategies only
+
+    --no-manifest
+    :   disables the automatic creation of a backup manifest file 
+        at the end of a backup. 
+        Overrides value of the parameter `autogenerate_manifest`, 
+        from the configuration file. 
+        Works with rsync backup method and strategies only
```

### Comparing `barman-3.6.0/doc/barman.1.d/50-get-wal.md` & `barman-3.7.0/doc/barman.1.d/50-get-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-recover.md` & `barman-3.7.0/doc/barman.1.d/50-recover.md`

 * *Files 8% similar despite different names*

```diff
@@ -119,10 +119,20 @@
 
     --snapshot-recovery-instance *INSTANCE_NAME*
     :   Name of the instance where the disks recovered from the snapshots are
         attached. This option is required when recovering backups made with
         `backup_method = snapshot`.
 
     --gcp-zone *ZONE_NAME*
-    :   Name of the availability zone where the instance and disks for snapshot
-        are located. This option is required when recovering backups made with
-        `backup_method = snapshot`.
+    :   Name of the GCP zone where the instance and disks for snapshot recovery
+        are located. This option can be used to override the value of `gcp_zone`
+        in the Barman config.
+
+    --azure-resource-group *RESOURCE_GROUP_NAME*
+    :   Name of the Azure resource group containing the instance and disks for
+        snapshot recovery. This option can be used to override the value of
+        `azure_resource_group` in the Barman config.
+
+    --aws-region *REGION_NAME*
+    :   Name of the AWS region where the instance and disks for snapshot
+        recovery are located. This option can be used to override the value of
+        `aws_region` in the Barman config.
```

### Comparing `barman-3.6.0/doc/barman.1.d/50-status.md` & `barman-3.7.0/doc/barman.1.d/50-status.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-receive-wal.md` & `barman-3.7.0/doc/barman.1.d/50-receive-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-keep.md` & `barman-3.7.0/doc/barman.1.d/50-keep.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/20-options.md` & `barman-3.7.0/doc/barman.1.d/20-options.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/90-authors.md` & `barman-3.7.0/doc/barman.1.d/90-authors.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-put-wal.md` & `barman-3.7.0/doc/barman.1.d/50-put-wal.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-sync-info.md` & `barman-3.7.0/doc/barman.1.d/50-sync-info.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-replication-status.md` & `barman-3.7.0/doc/barman.1.d/50-replication-status.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-check-wal-archive.md` & `barman-3.7.0/doc/barman.1.d/50-check-wal-archive.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman.1.d/50-show-backup.md` & `barman-3.7.0/doc/barman.1.d/50-show-backup.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/images/barman-architecture-scenario2b.png` & `barman-3.7.0/doc/images/barman-architecture-scenario2b.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/images/barman-architecture-georedundancy.png` & `barman-3.7.0/doc/images/barman-architecture-georedundancy.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/images/barman-architecture-scenario1.png` & `barman-3.7.0/doc/images/barman-architecture-scenario1.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/images/barman-architecture-scenario1b.png` & `barman-3.7.0/doc/images/barman-architecture-scenario1b.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/images/barman-architecture-scenario2.png` & `barman-3.7.0/doc/images/barman-architecture-scenario2.png`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman-wal-restore.1` & `barman-3.7.0/doc/barman-wal-restore.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-WAL\-RESTORE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-WAL\-RESTORE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-wal\-restore \- \[aq]restore_command\[aq] based on Barman\[aq]s
 get\-wal
 .SH SYNOPSIS
 .PP
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup-keep.1` & `barman-3.7.0/doc/barman-cloud-backup-keep.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-BACKUP\-DELETE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup\-keep \- Flag backups which should be kept forever
 .SH SYNOPSIS
 .PP
 barman\-cloud\-backup\-keep [\f[I]OPTIONS\f[]] \f[I]SOURCE_URL\f[]
@@ -20,15 +20,16 @@
 PostgreSQL servers written in Python and maintained by EnterpriseDB.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\-keep\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ AWS_PROFILE]\ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ (\-r\ |\ \-s\ |\ \-\-target\ {full,standalone})
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ source_url\ server_name\ backup_id
 
 This\ script\ can\ be\ used\ to\ tag\ backups\ in\ cloud\ storage\ as\ archival\ backups
 such\ that\ they\ will\ not\ be\ deleted.\ Currently\ AWS\ S3,\ Azure\ Blob\ Storage\ and
@@ -54,17 +55,19 @@
 \ \ \-s,\ \-\-status\ \ \ \ \ \ \ \ \ \ Print\ the\ keep\ status\ of\ the\ backup
 \ \ \-\-target\ {full,standalone}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Specify\ the\ recovery\ target\ for\ this\ backup
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
```

### Comparing `barman-3.6.0/doc/barman-cloud-backup.1` & `barman-3.7.0/doc/barman-cloud-backup.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-BACKUP" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-CLOUD\-BACKUP" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-backup \- Backup a PostgreSQL instance and stores it in
 the Cloud
 .SH SYNOPSIS
 .PP
@@ -41,27 +41,29 @@
 parameter.
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-backup\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]\ [\-P\ AWS_PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-z\ |\ \-j\ |\ \-\-snappy]\ [\-h\ HOST]\ [\-p\ PORT]\ [\-U\ USER]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-immediate\-checkpoint]\ [\-J\ JOBS]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-S\ MAX_ARCHIVE_SIZE]\ [\-d\ DBNAME]\ [\-n\ BACKUP_NAME]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-instance\ SNAPSHOT_INSTANCE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-disk\ NAME]\ [\-\-snapshot\-zone\ GCP_ZONE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-snapshot\-gcp\-project\ GCP_PROJECT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-gcp\-project\ GCP_PROJECT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-kms\-key\-name\ KMS_KEY_NAME]\ [\-\-gcp\-zone\ GCP_ZONE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-tags\ [TAGS\ [TAGS\ ...]]]\ [\-e\ {AES256,aws:kms}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-aws\-region\ AWS_REGION]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-encryption\-scope\ ENCRYPTION_SCOPE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-subscription\-id\ AZURE_SUBSCRIPTION_ID]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-resource\-group\ AZURE_RESOURCE_GROUP]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ destination_url\ server_name
 
 This\ script\ can\ be\ used\ to\ perform\ a\ backup\ of\ a\ local\ PostgreSQL\ instance\ and
 ship\ the\ resulting\ tarball(s)\ to\ the\ Cloud.\ Currently\ AWS\ S3,\ Azure\ Blob
@@ -114,30 +116,36 @@
 \ \ \-\-tags\ [TAGS\ [TAGS\ ...]]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Tags\ to\ be\ added\ to\ all\ uploaded\ files\ in\ cloud
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ storage
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 \ \ \-e\ {AES256,aws:kms},\ \-\-encryption\ {AES256,aws:kms}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ encryption\ algorithm\ used\ when\ storing\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ uploaded\ data\ in\ S3.\ Allowed\ values:
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \[aq]AES256\[aq]|\[aq]aws:kms\[aq].
 \ \ \-\-sse\-kms\-key\-id\ SSE_KMS_KEY_ID
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ AWS\ KMS\ key\ ID\ that\ should\ be\ used\ for\ encrypting
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ uploaded\ data\ in\ S3.\ Can\ be\ specified\ using\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ key\ ID\ on\ its\ own\ or\ using\ the\ full\ ARN\ for\ the\ key.
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Only\ allowed\ if\ `\-e/\-\-encryption`\ is\ set\ to\ `aws:kms`.
+\ \ \-\-aws\-region\ AWS_REGION
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ name\ of\ the\ AWS\ region\ containing\ the\ EC2\ VM\ and
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ storage\ volumes\ defined\ by\ the\ \-\-snapshot\-instance\ and
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \-\-snapshot\-disk\ arguments.
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Optionally\ specify\ the\ type\ of\ credential\ to\ use\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ authenticating\ with\ Azure.\ If\ omitted\ then\ Azure\ Blob
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Storage\ credentials\ will\ be\ obtained\ from\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ environment\ and\ the\ default\ Azure\ authentication\ flow
```

### Comparing `barman-3.6.0/doc/manual/24-wal_archiving.en.md` & `barman-3.7.0/doc/manual/24-wal_archiving.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/15-system_requirements.en.md` & `barman-3.7.0/doc/manual/15-system_requirements.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/99-references.en.md` & `barman-3.7.0/doc/manual/99-references.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/30-windows-support.en.md` & `barman-3.7.0/doc/manual/30-windows-support.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/50-feature-details.en.md` & `barman-3.7.0/doc/manual/50-feature-details.en.md`

 * *Files 0% similar despite different names*

```diff
@@ -1100,14 +1100,18 @@
 
 - `--gcp-zone`: The name of the availability zone in which the recovery instance is located. If not provided then Barman will use the value of `gcp_zone` set in the server config.
 
 The following additional `barman recover` arguments are available with the `azure` provider:
 
 - `--azure-resource-group`: The resource group to which the recovery instance belongs. If not provided then Barman will use the value of `azure_resource_group` set in the server config.
 
+The following additional `barman recover` arguments are available with the `aws` provider:
+
+- `--aws-region`: The AWS region in which the recovery instance is located. If not provided then Barman will use the value of `aws_region` set in the server config.
+
 Note the following `barman recover` arguments / config variables are unavailable when recovering snapshot backups:
 
 | **Command argument**      | **Config variable** .   |
 |:-------------------------:|:-----------------------:|
 | `--bwlimit`               | `bandwidth_limit`       |
 | `--jobs`                  | `parallel_jobs`         |
 | `--recovery-staging-path` | `recovery_staging_path` |
@@ -1207,7 +1211,20 @@
 - `resource_group`: The Azure resource group to which the resources involved in the backup belong.
 
 The following fields are available in `snapshots_info/snapshots/*/provider`:
 
 - `location`: The Azure location of the disk from which the snapshot was taken.
 - `lun`: The LUN identifying the disk from which the snapshot was taken at the time of the backup.
 - `snapshot_name`: The name of the snapshot.
+
+#### AWS provider-specific metadata
+
+The following fields are available in `snapshots_info/provider_info`:
+
+- `account_id`: The ID of the AWS account which owns the resources used to make the backup.
+- `region`: The AWS region in which the resources involved in backup are located.
+
+The following fields are available in `snapshots_info/snapshots/*/provider`:
+
+- `device_name`: The device to which the source disk was mapped on the backup VM at the time of the backup.
+- `snapshot_id`: The ID of the snapshot as assigned by AWS.
+- `snapshot_name`: The name of the snapshot.
```

### Comparing `barman-3.6.0/doc/manual/43-backup-commands.en.md` & `barman-3.7.0/doc/manual/43-backup-commands.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/25-streaming_backup.en.md` & `barman-3.7.0/doc/manual/25-streaming_backup.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/41-global-commands.en.md` & `barman-3.7.0/doc/manual/41-global-commands.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/23-wal_streaming.en.md` & `barman-3.7.0/doc/manual/23-wal_streaming.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/26-rsync_backup.en.md` & `barman-3.7.0/doc/manual/26-rsync_backup.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/66-about.en.md` & `barman-3.7.0/doc/manual/66-about.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/42-server-commands.en.md` & `barman-3.7.0/doc/manual/42-server-commands.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/00-head.en.md` & `barman-3.7.0/doc/manual/00-head.en.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 % Barman Manual
 % EnterpriseDB UK Limited
-% June 15, 2023 (3.6.0)
+% July 25, 2023 (3.7.0)
 
 **Barman** (Backup and Recovery Manager) is an open-source administration tool for disaster recovery of PostgreSQL servers written in Python. It allows your organisation to perform remote backups of multiple servers in business critical environments to reduce risk and help DBAs during the recovery phase.
 
 [Barman][11] is distributed under GNU GPL 3 and maintained by [EnterpriseDB][13], a platinum sponsor of the [PostgreSQL project][31].
 
 > **IMPORTANT:** \newline
 > This manual assumes that you are familiar with theoretical disaster
```

### Comparing `barman-3.6.0/doc/manual/20-server_setup.en.md` & `barman-3.7.0/doc/manual/20-server_setup.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/16-installation.en.md` & `barman-3.7.0/doc/manual/16-installation.en.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,26 +20,33 @@
 
 Then, as `root` simply type:
 
 ``` bash
 yum install barman
 ```
 
-> **NOTE:**
-> We suggest that you exclude any Barman related packages from getting updated
-> via the PGDG repository. This can be done by adding the following line
-> to any PGDG repository definition that is included in the Barman server inside
-> any `/etc/yum.repos.d/pgdg-*.repo` file:
-
-   ```ini
-   exclude=barman* python*-barman
-   ```
+In addition to the Barman packages available in the EDB and PGDG repositories, Barman RPMs published by the Fedora project can be found in EPEL.
+These RPMs are not maintained by the Barman developers and use a different configuration layout to the packages available in the PGDG and EDB repositories:
+
+- EDB and PGDG packages use `/etc/barman.conf` as the main configuration file and `/etc/barman.d` for additional configuration files.
+- The Fedora packages use `/etc/barman/barman.conf` as the main configuration file and `/etc/barman/conf.d` for additional configuration files.
+
+The difference in configuration file layout means that upgrades between the EPEL and non-EPEL Barman packages can break existing Barman installations until configuration files are manually updated.
+We therefore recommend that you use a single source repository for Barman packages.
+This can be achieved by adding the following line to the definition of the repositories from which you do not want to obtain Barman packages:
+
+```ini
+exclude=barman* python*-barman
+```
+
+Specifically:
 
-> By doing this, you solely rely on
-> EnterpriseDB's 2ndQuadrant repositories for package management of Barman software.
+- To use only Barman packages from the EDB repositories, add the exclude directive from above to repository definitions in `/etc/yum.repos.d/epel.repo` and `/etc/yum.repos.d/pgdg-*.repo`.
+- To use only Barman packages from the PGDG repositories, add the exclude directive from above to repository definitions in `/etc/yum.repos.d/epel.repo` and `/etc/yum.repos.d/enterprisedb*.repo`.
+- To use only Barman packages from the EPEL repositories, add the exclude directive from above to repository definitions in `/etc/yum.repos.d/pgdg-*.repo` and `/etc/yum.repos.d/enterprisedb*.repo`.
 
 ## Installation on Debian/Ubuntu using packages
 
 Barman can be installed on Debian and Ubuntu Linux systems using
 packages.
 
 It is directly available in the official repository for Debian and Ubuntu, however, these repositories might not contain the latest available version.
@@ -133,14 +140,22 @@
    server and points to the `bin` directory for the appropriate
    `PG_MAJOR_VERSION`.
 
 The [psql][psql] program is recommended in addition to the above binaries.
 While Barman does not use it directly the documentation provides examples of how it can be used to verify PostgreSQL connections are working as intended.
 The `psql` binary can be found in the PostgreSQL client packages.
 
+### Third party PostgreSQL variants
+
+If you are using Barman for the backup and recovery of third-party
+PostgreSQL variants then you will need to check whether the PGDG
+client/server binaries described above are compatible with your variant.
+If they are incompatible then you will need to install compatible
+alternatives from appropriate packages.
+
 # Upgrading Barman
 
 Barman follows the trunk-based development paradigm, and as such
 there is only one stable version, the latest. After every commit,
 Barman goes through thousands of automated tests for each
 supported PostgreSQL version and on each supported Linux distribution.
```

### Comparing `barman-3.6.0/doc/manual/55-barman-cli.en.md` & `barman-3.7.0/doc/manual/55-barman-cli.en.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,22 @@
 apt-get install barman-cli-cloud
 ```
 
 ## barman-cloud hook scripts
 
 Install the `barman-cli-cloud` package on the Barman server as described above.
 
-Configure `barman-cloud-backup` as a post backup script by adding the following
-to the Barman configuration for a PostgreSQL server:
+It is possible to use `barman-cloud-backup` as a post backup script for the
+following Barman backup flavours:
+
+- Backups taken with `backup_method = rsync`.
+- Backups taken with `backup_method = postgres` where `backup_compression` is
+  not used.
+
+To do so, add the following to a server configuration in Barman:
 
 ```
 post_backup_retry_script = 'barman-cloud-backup [*OPTIONS*] *DESTINATION_URL* ${BARMAN_SERVER}
 ```
 
 > **WARNING:** When running as a hook script barman-cloud-backup requires that
 > the status of the backup is DONE and it will fail if the backup has any other
@@ -214,14 +220,19 @@
 - `--gcp-zone`
 
 If the `--cloud-provider` is `azure-blob-storage` then the following arguments are also required:
 
 - `--azure-subscription-id`
 - `--azure-resource-group`
 
+If the `--cloud-provider` is `aws-s3` then the following optional arguments can be used:
+
+- `--aws-profile`
+- `--aws-region`
+
 The following options cannot be used with `barman-cloud-backup` when cloud snapshots are requested:
 
 - `--bzip2`, `--gzip` or `--snappy`
 - `--jobs`
 
 Once a backup has been taken it can be managed using the standard barman-cloud commands such as `barman-cloud-backup-delete` and `barman-cloud-backup-keep`.
 
@@ -243,8 +254,12 @@
 
 - `--gcp-zone`
 
 The following additional arguments are required with the `azure` provider:
 
 - `--azure-resource-group`
 
+The following additional argument is available with the `aws-s3` provider:
+
+- `--aws-region`
+
 The `--tablespace` option cannot be used with `barman-cloud-restore` when restoring a cloud snapshot backup:
```

### Comparing `barman-3.6.0/doc/manual/28-snapshots.en.md` & `barman-3.7.0/doc/manual/28-snapshots.en.md`

 * *Files 14% similar despite different names*

```diff
@@ -69,24 +69,49 @@
 
 - `Microsoft.Compute/disks/read`
 - `Microsoft.Compute/virtualMachines/read`
 - `Microsoft.Compute/snapshots/read`
 - `Microsoft.Compute/snapshots/write`
 - `Microsoft.Compute/snapshots/delete`
 
+#### AWS snapshot prerequisites
+
+The boto3 library must be available to the Python distribution used by Barman.
+
+This library is an optional dependency and not installed as standard by any of the Barman packages.
+It can be installed as follows using `pip`:
+
+```bash
+pip3 install boto3
+```
+
+The following additional prerequisites apply to snapshot backups on AWS:
+
+- All disks included in the snapshot backup must be non-root EBS volumes and must be attached to the same VM instance.
+- NVMe volumes are not currently supported.
+
+The following permissions are required:
+
+- `ec2:CreateSnapshot`
+- `ec2:CreateTags`
+- `ec2:DeleteSnapshot`
+- `ec2:DescribeSnapshots`
+- `ec2:DescribeInstances`
+- `ec2:DescribeVolumes`
+
 ### Configuration for snapshot backups
 
 To configure Barman for backup via cloud snapshots, set the `backup_method` parameter to `snapshot` and set `snapshot_provider` to a supported cloud provider:
 
 ``` ini
 backup_method = snapshot
 snapshot_provider = gcp
 ```
 
-Currently Google Cloud Platform (`gcp`) and Microsoft Azure (`azure`) are supported.
+Currently Google Cloud Platform (`gcp`), Microsoft Azure (`azure`) and AWS (`aws`) are supported.
 
 The following parameters must be set regardless of cloud provider:
 
 ``` ini
 snapshot_instance = INSTANCE_NAME
 snapshot_disks = DISK_NAME,DISK2_NAME,...
 ```
@@ -117,14 +142,33 @@
 azure_subscription_id = AZURE_SUBSCRIPTION_ID
 azure_resource_group = AZURE_RESOURCE_GROUP
 ```
 
 `azure_subscription_id` should be set to the ID of the Azure subscription ID which owns the instance and storage volumes defined by `snapshot_instance` and `snapshot_disks`.
 `azure_resource_group` should be set to the resource group to which the instance and disks belong.
 
+#### Configuration for AWS snapshots
+
+When specifying `snapshot_instance` or `snapshot_disks`, Barman will accept either the instance/volume ID which was assigned to the resource by AWS *or* a name.
+If a name is used then Barman will query AWS to find resources with a matching `Name` tag.
+If zero or multiple matching resources are found then Barman will exit with an error.
+
+The following optional parameters can be set when using AWS:
+
+``` ini
+aws_region = AWS_REGION
+aws_profile = AWS_PROFILE_NAME
+```
+
+If `aws_profile` is used it should be set to the name of a section in the AWS credentials file.
+If `aws_profile` is not used then the default profile will be used.
+If no credentials file exists then credentials will be sourced from the environment.
+
+If `aws_region` is specified it will override any region that may be defined in the AWS profile.
+
 ### Taking a snapshot backup
 
 Once the configuration options are set and appropriate credentials are available to Barman, backups can be taken using the [barman backup](#backup) command.
 
 Barman will validate the configuration parameters for snapshot backups during the `barman check` command and also when starting a backup.
 
 Note that the following arguments / config variables are unavailable when using `backup_method = snapshot`:
```

### Comparing `barman-3.6.0/doc/manual/Makefile` & `barman-3.7.0/doc/manual/Makefile`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/22-config_file.en.md` & `barman-3.7.0/doc/manual/22-config_file.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/02-before_you_start.en.md` & `barman-3.7.0/doc/manual/02-before_you_start.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/10-design.en.md` & `barman-3.7.0/doc/manual/10-design.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/01-intro.en.md` & `barman-3.7.0/doc/manual/01-intro.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/21-preliminary_steps.en.md` & `barman-3.7.0/doc/manual/21-preliminary_steps.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/65-troubleshooting.en.md` & `barman-3.7.0/doc/manual/65-troubleshooting.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/manual/17-configuration.en.md` & `barman-3.7.0/doc/manual/17-configuration.en.md`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman-cloud-check-wal-archive.1` & `barman-3.7.0/doc/barman-cloud-check-wal-archive.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-CLOUD\-CHECK\-WAL\-ARCHIVE" "1" "June 15, 2023" "Barman User manuals" "Version
-3.6.0"
+.TH "BARMAN\-CLOUD\-CHECK\-WAL\-ARCHIVE" "1" "July 25, 2023" "Barman User manuals" "Version
+3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-cloud\-check\-wal\-archive \- Check a WAL archive destination
 for a new PostgreSQL cluster
 .SH SYNOPSIS
 .PP
@@ -24,15 +24,15 @@
 .SH Usage
 .IP
 .nf
 \f[C]
 usage:\ barman\-cloud\-check\-wal\-archive\ [\-V]\ [\-\-help]\ [\-v\ |\ \-q]\ [\-t]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-cloud\-provider\ {aws\-s3,azure\-blob\-storage,google\-cloud\-storage}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-endpoint\-url\ ENDPOINT_URL]
-\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ PROFILE]
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-P\ AWS_PROFILE]\ [\-\-profile\ AWS_PROFILE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-read\-timeout\ READ_TIMEOUT]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-azure\-credential\ {azure\-cli,managed\-identity}]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ [\-\-timeline\ TIMELINE]
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ destination_url\ server_name
 
 Checks\ that\ the\ WAL\ archive\ on\ the\ specified\ cloud\ storage\ can\ be\ safely\ used
 for\ a\ new\ PostgreSQL\ server.
@@ -52,17 +52,19 @@
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ The\ cloud\ provider\ to\ use\ as\ a\ storage\ backend
 \ \ \-\-timeline\ TIMELINE\ \ \ The\ earliest\ timeline\ whose\ WALs\ should\ cause\ the
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ check\ to\ fail
 
 Extra\ options\ for\ the\ aws\-s3\ cloud\ provider:
 \ \ \-\-endpoint\-url\ ENDPOINT_URL
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ Override\ default\ S3\ endpoint\ URL\ with\ the\ given\ one
-\ \ \-P\ PROFILE,\ \-\-profile\ PROFILE
+\ \ \-P\ AWS_PROFILE,\ \-\-aws\-profile\ AWS_PROFILE
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (e.g.\ INI\ section\ in\ AWS\ credentials
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ file)
+\ \ \-\-profile\ AWS_PROFILE
+\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ profile\ name\ (deprecated:\ replaced\ by\ \-\-aws\-profile)
 \ \ \-\-read\-timeout\ READ_TIMEOUT
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ the\ time\ in\ seconds\ until\ a\ timeout\ is\ raised\ when
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ waiting\ to\ read\ from\ a\ connection\ (defaults\ to\ 60
 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ seconds)
 
 Extra\ options\ for\ the\ azure\-blob\-storage\ cloud\ provider:
 \ \ \-\-azure\-credential\ {azure\-cli,managed\-identity},\ \-\-credential\ {azure\-cli,managed\-identity}
```

### Comparing `barman-3.6.0/doc/Makefile` & `barman-3.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/doc/barman-wal-archive.1` & `barman-3.7.0/doc/barman-wal-archive.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.2.1
 .\"
-.TH "BARMAN\-WAL\-ARCHIVE" "1" "June 15, 2023" "Barman User manuals" "Version 3.6.0"
+.TH "BARMAN\-WAL\-ARCHIVE" "1" "July 25, 2023" "Barman User manuals" "Version 3.7.0"
 .hy
 .SH NAME
 .PP
 barman\-wal\-archive \- \f[C]archive_command\f[] based on Barman\[aq]s
 put\-wal
 .SH SYNOPSIS
 .PP
```

### Comparing `barman-3.6.0/doc/barman.conf` & `barman-3.7.0/doc/barman.conf`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/README.rst` & `barman-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/LICENSE` & `barman-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman.egg-info/SOURCES.txt` & `barman-3.7.0/barman.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,17 @@
 doc/barman.5.d/20-configuration-file-locations.md
 doc/barman.5.d/25-configuration-file-syntax.md
 doc/barman.5.d/30-configuration-file-directory.md
 doc/barman.5.d/45-options.md
 doc/barman.5.d/50-active.md
 doc/barman.5.d/50-archiver.md
 doc/barman.5.d/50-archiver_batch_size.md
+doc/barman.5.d/50-autogenerate_manifest.md
+doc/barman.5.d/50-aws_profile.md
+doc/barman.5.d/50-aws_region.md
 doc/barman.5.d/50-azure_credential.md
 doc/barman.5.d/50-azure_resource_group.md
 doc/barman.5.d/50-azure_subscription_id.md
 doc/barman.5.d/50-backup_compression.md
 doc/barman.5.d/50-backup_compression_format.md
 doc/barman.5.d/50-backup_compression_level.md
 doc/barman.5.d/50-backup_compression_location.md
@@ -280,9 +283,10 @@
 doc/manual/43-backup-commands.en.md
 doc/manual/50-feature-details.en.md
 doc/manual/55-barman-cli.en.md
 doc/manual/65-troubleshooting.en.md
 doc/manual/66-about.en.md
 doc/manual/99-references.en.md
 doc/manual/Makefile
+doc/runbooks/snapshot_recovery_aws.md
 doc/runbooks/snapshot_recovery_azure.md
 scripts/barman.bash_completion
```

### Comparing `barman-3.6.0/barman.egg-info/entry_points.txt` & `barman-3.7.0/barman.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman.egg-info/PKG-INFO` & `barman-3.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barman
-Version: 3.6.0
+Version: 3.7.0
 Summary: Backup and Recovery Manager for PostgreSQL
 Home-page: https://www.pgbarman.org/
 Author: EnterpriseDB
 Author-email: barman@enterprisedb.com
 License: GPL-3.0
 Platform: Linux
 Platform: Mac OS X
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cloud
+Provides-Extra: aws-snapshots
 Provides-Extra: azure
 Provides-Extra: azure-snapshots
 Provides-Extra: snappy
 Provides-Extra: google
 Provides-Extra: google-snapshots
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `barman-3.6.0/barman/__init__.py` & `barman-3.7.0/barman/__init__.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/server.py` & `barman-3.7.0/barman/server.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/wal_archiver.py` & `barman-3.7.0/barman/wal_archiver.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/hooks.py` & `barman-3.7.0/barman/hooks.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/diagnose.py` & `barman-3.7.0/barman/diagnose.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/cli.py` & `barman-3.7.0/barman/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     check_non_negative,
     check_positive,
     check_tli,
     configure_logging,
     drop_privileges,
     force_str,
     get_log_levels,
-    is_backup_id,
+    get_backup_id_using_shortcut,
     parse_log_level,
     RESERVED_BACKUP_IDS,
     SHA256,
 )
 from barman.xlog import check_archive_usable
 from barman.backup_manifest import BackupManifest
 from barman.storage.local_file_manager import LocalFileManager
@@ -440,14 +440,30 @@
             "--name",
             help="a name which can be used to reference this backup in barman "
             "commands such as recover and delete",
             dest="backup_name",
             default=None,
             type=check_backup_name,
         ),
+        argument(
+            "--manifest",
+            help="forces the creation of the backup manifest file for the "
+            "rsync backup method",
+            dest="automatic_manifest",
+            action="store_true",
+            default=SUPPRESS,
+        ),
+        argument(
+            "--no-manifest",
+            help="disables the creation of the backup manifest file for the "
+            "rsync backup method",
+            dest="automatic_manifest",
+            action="store_false",
+            default=SUPPRESS,
+        ),
     ]
 )
 def backup(args):
     """
     Perform a full backup for the given server (supports 'all')
     """
     servers = get_server_list(args, skip_inactive=True, skip_passive=True)
@@ -466,14 +482,19 @@
             server.config.basebackup_retry_times = args.retry_times
         if hasattr(args, "immediate_checkpoint"):
             # As well as overriding the immediate_checkpoint value in the config
             # we must also update the immediate_checkpoint attribute on the
             # postgres connection because it has already been set from the config
             server.config.immediate_checkpoint = args.immediate_checkpoint
             server.postgres.immediate_checkpoint = args.immediate_checkpoint
+        if hasattr(args, "automatic_manifest"):
+            # Override the set value for the autogenerate_manifest config option.
+            # The backup executor class will automatically ignore --manifest requests
+            # for backup methods different from rsync.
+            server.config.autogenerate_manifest = args.automatic_manifest
         if args.jobs is not None:
             server.config.parallel_jobs = args.jobs
         if args.jobs_start_batch_size is not None:
             server.config.parallel_jobs_start_batch_size = args.jobs_start_batch_size
         if args.jobs_start_batch_period is not None:
             server.config.parallel_jobs_start_batch_period = (
                 args.jobs_start_batch_period
@@ -792,14 +813,19 @@
             help="Zone containing the instance and disks for the snapshot recovery",
         ),
         argument(
             "--azure-resource-group",
             help="Azure resource group containing the instance and disks for recovery "
             "of a snapshot backup",
         ),
+        argument(
+            "--aws-region",
+            help="The name of the AWS region containing the EC2 VM and storage "
+            "volumes for recovery of a snapshot backup",
+        ),
     ]
 )
 def recover(args):
     """
     Recover a server at a given time, name, LSN or xid
     """
     server = get_server(args)
@@ -962,14 +988,15 @@
             "recovery_instance": args.snapshot_recovery_instance,
         }
         # Special handling for deprecated snapshot_recovery_zone arg
         if args.gcp_zone is None and args.snapshot_recovery_zone is not None:
             args.gcp_zone = args.snapshot_recovery_zone
         # Override provider-specific options in the config
         for arg in (
+            "aws_region",
             "azure_resource_group",
             "gcp_zone",
         ):
             value = getattr(args, arg)
             if value is not None:
                 setattr(server.config, arg, value)
     else:
@@ -2059,23 +2086,16 @@
 
     Exit with error if the backup id doesn't exist.
 
     :param Server server: server object to search for the required backup
     :param args: command line arguments namespace
     :rtype: barman.infofile.LocalBackupInfo
     """
-    if args.backup_id in ("latest", "last"):
-        backup_id = server.get_last_backup_id()
-    elif args.backup_id in ("oldest", "first"):
-        backup_id = server.get_first_backup_id()
-    elif args.backup_id in ("last-failed"):
-        backup_id = server.get_last_backup_id([BackupInfo.FAILED])
-    elif is_backup_id(args.backup_id):
-        backup_id = args.backup_id
-    else:
+    backup_id = get_backup_id_using_shortcut(server, args.backup_id, BackupInfo)
+    if backup_id is None:
         try:
             backup_id = server.get_backup_id_from_name(args.backup_id)
         except ValueError as exc:
             output.error(str(exc))
             output.close_and_exit()
     backup_info = server.get_backup(backup_id)
     if backup_info is None:
```

### Comparing `barman-3.6.0/barman/output.py` & `barman-3.7.0/barman/output.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/fs.py` & `barman-3.7.0/barman/fs.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/annotations.py` & `barman-3.7.0/barman/annotations.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_backup_delete.py` & `barman-3.7.0/barman/clients/cloud_backup_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     OperationErrorExit,
 )
 from barman.cloud import CloudBackupCatalog, configure_logging
 from barman.cloud_providers import (
     get_cloud_interface,
     get_snapshot_interface_from_backup_info,
 )
-from barman.exceptions import InvalidRetentionPolicy
+from barman.exceptions import BadXlogPrefix, InvalidRetentionPolicy
 from barman.retention_policies import RetentionPolicyFactory
 from barman.utils import force_str
 from barman import xlog
 
 
 def _get_files_for_backup(catalog, backup_info):
     backup_files = []
@@ -101,24 +101,87 @@
         # use BackupManager to get a set of all other timelines with backups so that
         # we can preserve all WALs on other timelines.
         timelines_to_protect = BackupManager.get_timelines_to_protect(
             remove_until=remove_until,
             deleted_backup=deleted_backup,
             available_backups=catalog.get_backup_list(),
         )
+        # Identify any prefixes under which all WALs are no longer needed.
+        # This is a shortcut which allows us to delete all WALs under a prefix without
+        # checking each individual WAL.
+        try:
+            wal_prefixes = catalog.get_wal_prefixes()
+        except NotImplementedError:
+            # If fetching WAL prefixes isn't supported by the cloud provider then
+            # the old method of checking each WAL must be used for all WALs.
+            wal_prefixes = []
+        deletable_prefixes = []
+        for wal_prefix in wal_prefixes:
+            try:
+                tli_and_log = wal_prefix.split("/")[-2]
+                tli, log = xlog.decode_hash_dir(tli_and_log)
+            except (BadXlogPrefix, IndexError):
+                # If the prefix does not appear to be a tli and log we output a warning
+                # and move on to the next prefix rather than error out.
+                logging.warning(
+                    "Ignoring malformed WAL object prefix: {}".format(wal_prefix)
+                )
+                continue
+            # If this prefix contains a timeline which should be protected then we
+            # cannot delete the WALS under it so advance to the next prefix.
+            if tli in timelines_to_protect:
+                continue
+
+            # If the tli and log fall are inclusively between the tli and log for the
+            # begin and end WAL of any protected WAL range then this prefix cannot be
+            # deleted outright.
+            for begin_wal, end_wal in wal_ranges_to_protect:
+                begin_tli, begin_log, _ = xlog.decode_segment_name(begin_wal)
+                end_tli, end_log, _ = xlog.decode_segment_name(end_wal)
+                if (
+                    tli >= begin_tli
+                    and log >= begin_log
+                    and tli <= end_tli
+                    and log <= end_log
+                ):
+                    break
+            else:
+                # The prefix tli and log do not match any protected timelines or
+                # protected WAL ranges so all WALs are eligible for deletion if the tli
+                # is the same timeline and the log is below the begin_wal log of the
+                # backup being deleted.
+                until_begin_tli, until_begin_log, _ = xlog.decode_segment_name(
+                    remove_until.begin_wal
+                )
+                if tli == until_begin_tli and log < until_begin_log:
+                    # All WALs under this prefix pre-date the backup being deleted so they
+                    # can be deleted in one request.
+                    deletable_prefixes.append(wal_prefix)
+        for wal_prefix in deletable_prefixes:
+            if not dry_run:
+                cloud_interface.delete_under_prefix(wal_prefix)
+            else:
+                print(
+                    "Skipping deletion of all objects under prefix %s "
+                    "due to --dry-run option" % wal_prefix
+                )
         try:
             wal_paths = catalog.get_wal_paths()
         except Exception as exc:
             logging.error(
                 "Cannot clean up WALs for backup %s because an error occurred listing WALs: %s",
                 deleted_backup.backup_id,
                 force_str(exc),
             )
             return
         for wal_name, wal in wal_paths.items():
+            # If the wal starts with a prefix we deleted then ignore it so that the
+            # dry-run output is accurate
+            if any(wal.startswith(prefix) for prefix in deletable_prefixes):
+                continue
             if xlog.is_history_file(wal_name):
                 continue
             if timelines_to_protect:
                 tli, _, _ = xlog.decode_segment_name(wal_name)
                 if tli in timelines_to_protect:
                     continue
```

### Comparing `barman-3.6.0/barman/clients/__init__.py` & `barman-3.7.0/barman/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_walarchive.py` & `barman-3.7.0/barman/clients/cloud_walarchive.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_walrestore.py` & `barman-3.7.0/barman/clients/cloud_walrestore.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_backup_keep.py` & `barman-3.7.0/barman/clients/cloud_backup_keep.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_backup_show.py` & `barman-3.7.0/barman/clients/cloud_backup_show.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/walrestore.py` & `barman-3.7.0/barman/clients/walrestore.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_restore.py` & `barman-3.7.0/barman/clients/cloud_restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 def parse_arguments(args=None):
     """
     Parse command line arguments
 
     :return: The options parsed
     """
 
-    parser, _, azure_arguments = create_argument_parser(
+    parser, s3_arguments, azure_arguments = create_argument_parser(
         description="This script can be used to download a backup "
         "previously made with barman-cloud-backup command."
         "Currently AWS S3, Azure Blob Storage and Google Cloud Storage are supported.",
     )
     parser.add_argument("backup_id", help="the backup ID")
     parser.add_argument("recovery_dir", help="the path to a directory for recovery.")
     parser.add_argument(
@@ -153,14 +153,21 @@
         "--snapshot-recovery-zone",
         help=(
             "Zone containing the instance and disks for the snapshot recovery "
             "(deprecated: replaced by --gcp-zone)"
         ),
         dest="gcp_zone",
     )
+    s3_arguments.add_argument(
+        "--aws-region",
+        help=(
+            "Name of the AWS region where the instance and disks for snapshot "
+            "recovery are located"
+        ),
+    )
     gcs_arguments = parser.add_argument_group(
         "Extra options for google-cloud-storage cloud provider"
     )
     gcs_arguments.add_argument(
         "--gcp-zone",
         help="Zone containing the instance and disks for the snapshot recovery",
     )
```

### Comparing `barman-3.6.0/barman/clients/cloud_backup_list.py` & `barman-3.7.0/barman/clients/cloud_backup_list.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_check_wal_archive.py` & `barman-3.7.0/barman/clients/cloud_check_wal_archive.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/walarchive.py` & `barman-3.7.0/barman/clients/walarchive.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_compression.py` & `barman-3.7.0/barman/clients/cloud_compression.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/clients/cloud_cli.py` & `barman-3.7.0/barman/clients/cloud_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,18 +176,23 @@
     )
     s3_arguments.add_argument(
         "--endpoint-url",
         help="Override default S3 endpoint URL with the given one",
     )
     s3_arguments.add_argument(
         "-P",
-        "--profile",
+        "--aws-profile",
         help="profile name (e.g. INI section in AWS credentials file)",
     )
     s3_arguments.add_argument(
+        "--profile",
+        help="profile name (deprecated: replaced by --aws-profile)",
+        dest="aws_profile",
+    )
+    s3_arguments.add_argument(
         "--read-timeout",
         type=int,
         help="the time in seconds until a timeout is raised when waiting to "
         "read from a connection (defaults to 60 seconds)",
     )
     azure_arguments = parser.add_argument_group(
         "Extra options for the azure-blob-storage cloud provider"
```

### Comparing `barman-3.6.0/barman/clients/cloud_backup.py` & `barman-3.7.0/barman/clients/cloud_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,14 +386,19 @@
     )
     s3_arguments.add_argument(
         "--sse-kms-key-id",
         help="The AWS KMS key ID that should be used for encrypting the uploaded data "
         "in S3. Can be specified using the key ID on its own or using the full ARN for "
         "the key. Only allowed if `-e/--encryption` is set to `aws:kms`.",
     )
+    s3_arguments.add_argument(
+        "--aws-region",
+        help="The name of the AWS region containing the EC2 VM and storage volumes "
+        "defined by the --snapshot-instance and --snapshot-disk arguments.",
+    )
     azure_arguments.add_argument(
         "--encryption-scope",
         help="The name of an encryption scope defined in the Azure Blob Storage "
         "service which is to be used to encrypt the data in Azure",
     )
     azure_arguments.add_argument(
         "--azure-subscription-id",
```

### Comparing `barman-3.6.0/barman/retention_policies.py` & `barman-3.7.0/barman/retention_policies.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/postgres_plumbing.py` & `barman-3.7.0/barman/postgres_plumbing.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/process.py` & `barman-3.7.0/barman/process.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/cloud.py` & `barman-3.7.0/barman/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1198,14 +1198,34 @@
 
         if errors:
             raise CloudProviderError(
                 "Error from cloud provider while deleting objects - "
                 "please check the command output."
             )
 
+    @abstractmethod
+    def get_prefixes(self, prefix):
+        """
+        Return only the common prefixes under the supplied prefix.
+
+        :param str prefix: The object key prefix under which the common prefixes
+            will be found.
+        :rtype: Iterator[str]
+        :return: A list of unique prefixes immediately under the supplied prefix.
+        """
+
+    @abstractmethod
+    def delete_under_prefix(self, prefix):
+        """
+        Delete all objects under the specified prefix.
+
+        :param str prefix: The object key prefix under which all objects should be
+            deleted.
+        """
+
 
 class CloudBackup(with_metaclass(ABCMeta)):
     """
     Abstract base class for taking cloud backups of PostgreSQL servers.
 
     This class handles the coordination of the physical backup copy with the PostgreSQL
     server via the PostgreSQL low-level backup API. This is handled by the
@@ -2046,14 +2066,20 @@
         Remove backup with backup_id from the cached list. This is intended for
         cases where we want to update the state without firing lots of requests
         at the bucket.
         """
         if self._backup_list:
             self._backup_list.pop(backup_id)
 
+    def get_wal_prefixes(self):
+        """
+        Return only the common prefixes under the wals prefix.
+        """
+        return self.cloud_interface.get_prefixes(self.wal_prefix)
+
     def get_wal_paths(self):
         """
         Retrieve a dict of WAL paths keyed by the WAL name from cloud storage
         """
         if self._wal_paths is None:
             wal_paths = {}
             for wal in self.cloud_interface.list_bucket(
@@ -2273,34 +2299,41 @@
         """
         Delete all snapshots for the supplied backup.
 
         :param barman.infofile.LocalBackupInfo backup_info: Backup information.
         """
 
     @abstractmethod
-    def get_attached_volumes(self, instance_name, disks=None):
+    def get_attached_volumes(self, instance_name, disks=None, fail_on_missing=True):
         """
         Returns metadata for the volumes attached to this instance.
 
         Queries the cloud provider for metadata relating to the volumes attached to
         the named instance and returns a dict of `VolumeMetadata` objects, keyed by
         disk name.
 
         If the optional disks parameter is supplied then this method must return
         metadata for the disks in the supplied list only. A SnapshotBackupException
         must be raised if any of the supplied disks are not found to be attached to
         the instance.
 
+        If the optional disks parameter is supplied then this method returns metadata
+        for the disks in the supplied list only. If fail_on_missing is set to True then
+        a SnapshotBackupException is raised if any of the supplied disks are not found
+        to be attached to the instance.
+
         If the disks parameter is not supplied then this method must return a
         VolumeMetadata for all disks attached to this instance.
 
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
         :param list[str]|None disks: A list containing the names of disks to be
             backed up.
+        :param bool fail_on_missing: Fail with a SnapshotBackupException if any
+            specified disks are not attached to the instance.
         :rtype: dict[str, VolumeMetadata]
         :return: A dict of VolumeMetadata objects representing each volume
             attached to the instance, keyed by volume identifier.
         """
 
     @abstractmethod
     def instance_exists(self, instance_name):
```

### Comparing `barman-3.6.0/barman/xlog.py` & `barman-3.7.0/barman/xlog.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import os
 import re
 from functools import partial
 from tempfile import NamedTemporaryFile
 
 from barman.exceptions import (
     BadHistoryFileContents,
+    BadXlogPrefix,
     BadXlogSegmentName,
     CommandException,
     WalArchiveContentError,
 )
 
 # xlog file segment name parser (regular expression)
 _xlog_re = re.compile(
@@ -50,14 +51,17 @@
         \.history                      # or only .history, if a history file
     )
     $
     """,
     re.VERBOSE,
 )
 
+# xlog prefix parser (regular expression)
+_xlog_prefix_re = re.compile(r"^([\dA-Fa-f]{8})([\dA-Fa-f]{8})$")
+
 # xlog location parser for concurrent backup (regular expression)
 _location_re = re.compile(r"^([\dA-F]+)/([\dA-F]+)$")
 
 # Taken from xlog_internal.h from PostgreSQL sources
 
 #: XLOG_SEG_SIZE is the size of a single WAL file.  This must be a power of 2
 #: and larger than XLOG_BLCKSZ (preferably, a great deal larger than
@@ -311,14 +315,32 @@
     # tli is always not None
     if log is not None:
         return "%08X%08X" % (tli, log)
     else:
         return ""
 
 
+def decode_hash_dir(hash_dir):
+    """
+    Get the timeline and log from a hash dir prefix.
+
+    :param str hash_dir: A string representing the prefix used when determining
+        the folder or object key prefix under which Barman will store a given
+        WAL segment. This prefix is composed of the timeline and the higher 32-bit
+        number of the WAL segment.
+    :rtype: List[int]
+    :return: A list of two elements where the first item is the timeline and the
+        second is the higher 32-bit number of the WAL segment.
+    """
+    match = _xlog_prefix_re.match(hash_dir)
+    if not match:
+        raise BadXlogPrefix(hash_dir)
+    return [int(x, 16) if x else None for x in match.groups()]
+
+
 def parse_lsn(lsn_string):
     """
     Transform a string XLOG location, formatted as %X/%X, in the corresponding
     numeric representation
 
     :param str lsn_string: the string XLOG location, i.e. '2/82000168'
     :rtype: int
```

### Comparing `barman-3.6.0/barman/remote_status.py` & `barman-3.7.0/barman/remote_status.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/command_wrappers.py` & `barman-3.7.0/barman/command_wrappers.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/copy_controller.py` & `barman-3.7.0/barman/copy_controller.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/backup_manifest.py` & `barman-3.7.0/barman/backup_manifest.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/compression.py` & `barman-3.7.0/barman/compression.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/exceptions.py` & `barman-3.7.0/barman/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,20 @@
 
 class SnapshotBackupException(BackupException):
     """
     Exception for snapshot backups
     """
 
 
+class SnapshotInstanceNotFoundException(SnapshotBackupException):
+    """
+    Raised when the VM instance related to a snapshot backup cannot be found
+    """
+
+
 class SyncError(SyncException):
     """
     Synchronisation error
     """
 
 
 class SyncNothingToDo(SyncException):
@@ -331,14 +337,20 @@
 
 class BadXlogSegmentName(WALFileException):
     """
     Exception for a bad xlog name
     """
 
 
+class BadXlogPrefix(WALFileException):
+    """
+    Exception for a bad xlog prefix
+    """
+
+
 class BadHistoryFileContents(WALFileException):
     """
     Exception for a corrupted history file
     """
 
 
 class AbortedRetryHookScript(HookScriptException):
```

### Comparing `barman-3.6.0/barman/backup.py` & `barman-3.7.0/barman/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,19 @@
 from barman.utils import (
     force_str,
     fsync_dir,
     fsync_file,
     get_backup_info_from_name,
     human_readable_timedelta,
     pretty_size,
+    SHA256,
 )
 from barman.command_wrappers import PgVerifyBackup
+from barman.storage.local_file_manager import LocalFileManager
+from barman.backup_manifest import BackupManifest
 
 _logger = logging.getLogger(__name__)
 
 
 class BackupManager(RemoteStatusMixin, KeepManagerMixin):
     """Manager of the backup archive for a server"""
 
@@ -714,14 +717,35 @@
                     )
 
                 # Run the post-backup-script if present.
                 script = HookScriptRunner(self, "backup_script", "post")
                 script.env_from_backup_info(backup_info)
                 script.run()
 
+                # if the autogenerate_manifest functionality is active and the
+                # backup files copy is successfully completed using the rsync method,
+                # generate the backup manifest
+                if (
+                    isinstance(self.executor, RsyncBackupExecutor)
+                    and self.config.autogenerate_manifest
+                    and backup_info.status != BackupInfo.FAILED
+                ):
+                    local_file_manager = LocalFileManager()
+                    backup_manifest = BackupManifest(
+                        backup_info.get_data_directory(), local_file_manager, SHA256()
+                    )
+                    backup_manifest.create_backup_manifest()
+
+                    output.info(
+                        "Backup manifest for backup '%s' successfully "
+                        "generated for server %s",
+                        backup_info.backup_id,
+                        self.config.name,
+                    )
+
         output.result("backup", backup_info)
         return backup_info
 
     def recover(
         self, backup_info, dest, tablespaces=None, remote_command=None, **kwargs
     ):
         """
```

### Comparing `barman-3.6.0/barman/config.py` & `barman-3.7.0/barman/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,17 @@
     This class represents the configuration for a specific Server instance.
     """
 
     KEYS = [
         "active",
         "archiver",
         "archiver_batch_size",
+        "autogenerate_manifest",
+        "aws_profile",
+        "aws_region",
         "azure_credential",
         "azure_resource_group",
         "azure_subscription_id",
         "backup_compression",
         "backup_compression_format",
         "backup_compression_level",
         "backup_compression_location",
@@ -513,14 +516,17 @@
         "wal_retention_policy",
         "wals_directory",
     ]
 
     BARMAN_KEYS = [
         "archiver",
         "archiver_batch_size",
+        "autogenerate_manifest",
+        "aws_profile",
+        "aws_region",
         "azure_credential",
         "azure_resource_group",
         "azure_subscription_id",
         "backup_compression",
         "backup_compression_format",
         "backup_compression_level",
         "backup_compression_location",
@@ -587,14 +593,15 @@
         "wal_retention_policy",
     ]
 
     DEFAULTS = {
         "active": "true",
         "archiver": "off",
         "archiver_batch_size": "0",
+        "autogenerate_manifest": "false",
         "backup_directory": "%(barman_home)s/%(name)s",
         "backup_method": "rsync",
         "backup_options": "",
         "basebackup_retry_sleep": "30",
         "basebackup_retry_times": "0",
         "basebackups_directory": "%(backup_directory)s/base",
         "check_timeout": "30",
@@ -625,14 +632,15 @@
         "disabled",
     ]
 
     PARSERS = {
         "active": parse_boolean,
         "archiver": parse_boolean,
         "archiver_batch_size": int,
+        "autogenerate_manifest": parse_boolean,
         "backup_compression": parse_backup_compression,
         "backup_compression_format": parse_backup_compression_format,
         "backup_compression_level": int,
         "backup_compression_location": parse_backup_compression_location,
         "backup_compression_workers": int,
         "backup_method": parse_backup_method,
         "backup_options": BackupOptions,
```

### Comparing `barman-3.6.0/barman/backup_executor.py` & `barman-3.7.0/barman/backup_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1570,15 +1570,17 @@
         :param list[str] snapshot_disks: A list containing the names of the disks for
             which snapshots should be taken at backup time.
         :rtype tuple[list[str],list[str]]
         :return: A tuple where the first element is a list of all disks which are not
             attached to the VM instance and the second element is a list of all disks
             which are attached but not mounted.
         """
-        attached_volumes = snapshot_interface.get_attached_volumes(snapshot_instance)
+        attached_volumes = snapshot_interface.get_attached_volumes(
+            snapshot_instance, snapshot_disks, fail_on_missing=False
+        )
         missing_disks = []
         for disk in snapshot_disks:
             if disk not in attached_volumes.keys():
                 missing_disks.append(disk)
 
         unmounted_disks = []
         for disk in snapshot_disks:
```

### Comparing `barman-3.6.0/barman/lockfile.py` & `barman-3.7.0/barman/lockfile.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/infofile.py` & `barman-3.7.0/barman/infofile.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/utils.py` & `barman-3.7.0/barman/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -839,7 +839,30 @@
             "Multiple backups found matching name '%s' "
             "(try using backup ID instead): %s"
         ) % (backup_name, matching_backup_ids)
 
         raise ValueError(msg)
     elif len(matching_backups) == 1:
         return matching_backups[0]
+
+
+def get_backup_id_using_shortcut(server, shortcut, BackupInfo):
+    """
+    Get backup ID from one of Barman shortcuts.
+
+    :param str server: The obj where to look from.
+    :param str shortcut: pattern to search.
+    :param BackupInfo BackupInfo: Place where we keep some Barman constants.
+    :return str backup_id|None: The backup ID for the provided shortcut.
+    """
+    backup_id = None
+
+    if shortcut in ("latest", "last"):
+        backup_id = server.get_last_backup_id()
+    elif shortcut in ("oldest", "first"):
+        backup_id = server.get_first_backup_id()
+    elif shortcut in ("last-failed"):
+        backup_id = server.get_last_backup_id([BackupInfo.FAILED])
+    elif is_backup_id(shortcut):
+        backup_id = shortcut
+
+    return backup_id
```

### Comparing `barman-3.6.0/barman/postgres.py` & `barman-3.7.0/barman/postgres.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/recovery_executor.py` & `barman-3.7.0/barman/recovery_executor.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/storage/__init__.py` & `barman-3.7.0/barman/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/storage/file_manager.py` & `barman-3.7.0/barman/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/storage/file_stats.py` & `barman-3.7.0/barman/storage/file_stats.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/storage/local_file_manager.py` & `barman-3.7.0/barman/storage/local_file_manager.py`

 * *Files identical despite different names*

### Comparing `barman-3.6.0/barman/version.py` & `barman-3.7.0/barman/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # You should have received a copy of the GNU General Public License
 # along with Barman.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 This module contains the current Barman version.
 """
 
-__version__ = '3.6.0'
+__version__ = '3.7.0'
```

### Comparing `barman-3.6.0/barman/cloud_providers/__init__.py` & `barman-3.7.0/barman/cloud_providers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 def _make_s3_cloud_interface(config, cloud_interface_kwargs):
     from barman.cloud_providers.aws_s3 import S3CloudInterface
 
     cloud_interface_kwargs.update(
         {
-            "profile_name": config.profile,
+            "profile_name": config.aws_profile,
             "endpoint_url": config.endpoint_url,
             "read_timeout": config.read_timeout,
         }
     )
     if "encryption" in config:
         cloud_interface_kwargs["encryption"] = config.encryption
     if "sse_kms_key_id" in config:
@@ -190,14 +190,18 @@
                 "backups when cloud provider is azure-blob-storage"
             )
         return AzureCloudSnapshotInterface(
             config.azure_subscription_id,
             resource_group=config.azure_resource_group,
             credential=_get_azure_credential(config.azure_credential),
         )
+    elif config.cloud_provider == "aws-s3":
+        from barman.cloud_providers.aws_s3 import AwsCloudSnapshotInterface
+
+        return AwsCloudSnapshotInterface(config.aws_profile, config.aws_region)
     else:
         raise CloudProviderUnsupported(
             "No snapshot provider for cloud provider: %s" % config.cloud_provider
         )
 
 
 def get_snapshot_interface_from_server_config(server_config):
@@ -233,14 +237,20 @@
                 "is azure"
             )
         return AzureCloudSnapshotInterface(
             server_config.azure_subscription_id,
             resource_group=server_config.azure_resource_group,
             credential=_get_azure_credential(server_config.azure_credential),
         )
+    elif server_config.snapshot_provider == "aws":
+        from barman.cloud_providers.aws_s3 import AwsCloudSnapshotInterface
+
+        return AwsCloudSnapshotInterface(
+            server_config.aws_profile, server_config.aws_region
+        )
     else:
         raise CloudProviderUnsupported(
             "Unsupported snapshot provider: %s" % server_config.snapshot_provider
         )
 
 
 def get_snapshot_interface_from_backup_info(backup_info, config=None):
@@ -290,14 +300,28 @@
         else:
             resource_group = None
         return AzureCloudSnapshotInterface(
             backup_info.snapshots_info.subscription_id,
             resource_group=resource_group,
             credential=_get_azure_credential(config.azure_credential),
         )
+    elif backup_info.snapshots_info.provider == "aws":
+        from barman.cloud_providers.aws_s3 import AwsCloudSnapshotInterface
+
+        # When creating a snapshot interface for existing backups we use the region
+        # from the backup_info, unless a region is set in the config in which case the
+        # config region takes precedence.
+        region = None
+        profile = None
+        if config is not None and hasattr(config, "aws_region"):
+            region = config.aws_region
+            profile = config.aws_profile
+        if region is None:
+            region = backup_info.snapshots_info.region
+        return AwsCloudSnapshotInterface(profile, region)
     else:
         raise CloudProviderUnsupported(
             "Unsupported snapshot provider in backup info: %s"
             % backup_info.snapshots_info.provider
         )
 
 
@@ -317,12 +341,18 @@
         return GcpSnapshotsInfo.from_dict(snapshots_info)
     elif "provider" in snapshots_info and snapshots_info["provider"] == "azure":
         from barman.cloud_providers.azure_blob_storage import (
             AzureSnapshotsInfo,
         )
 
         return AzureSnapshotsInfo.from_dict(snapshots_info)
+    elif "provider" in snapshots_info and snapshots_info["provider"] == "aws":
+        from barman.cloud_providers.aws_s3 import (
+            AwsSnapshotsInfo,
+        )
+
+        return AwsSnapshotsInfo.from_dict(snapshots_info)
     else:
         raise CloudProviderUnsupported(
             "Unsupported snapshot provider in backup info: %s"
             % snapshots_info["provider"]
         )
```

### Comparing `barman-3.6.0/barman/cloud_providers/azure_blob_storage.py` & `barman-3.7.0/barman/cloud_providers/azure_blob_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,14 +502,34 @@
                     'Deletion of object %s failed with error code: "%s"'
                     % (resp.request.url, resp.status_code)
                 )
 
         if errors:
             raise CloudProviderError()
 
+    def get_prefixes(self, prefix):
+        """
+        Return only the common prefixes under the supplied prefix.
+
+        :param str prefix: The object key prefix under which the common prefixes
+            will be found.
+        :rtype: Iterator[str]
+        :return: A list of unique prefixes immediately under the supplied prefix.
+        """
+        raise NotImplementedError()
+
+    def delete_under_prefix(self, prefix):
+        """
+        Delete all objects under the specified prefix.
+
+        :param str prefix: The object key prefix under which all objects should be
+            deleted.
+        """
+        raise NotImplementedError()
+
 
 def import_azure_mgmt_compute():
     """
     Import and return the azure.mgmt.compute module.
 
     This particular import happens in a function so that it can be deferred until
     needed while still allowing tests to easily mock the library.
@@ -746,32 +766,35 @@
                 snapshot.identifier,
                 backup_info.backup_id,
             )
             self._delete_snapshot(
                 snapshot.identifier, backup_info.snapshots_info.resource_group
             )
 
-    def get_attached_volumes(self, instance_name, disks=None):
+    def get_attached_volumes(self, instance_name, disks=None, fail_on_missing=True):
         """
         Returns metadata for the volumes attached to this instance.
 
         Queries Azure for metadata relating to the volumes attached to the named
         instance and returns a dict of `VolumeMetadata` objects, keyed by disk name.
 
         If the optional disks parameter is supplied then this method returns metadata
-        for the disks in the supplied list only. A SnapshotBackupException is raised if
-        any of the supplied disks are not found to be attached to the instance.
+        for the disks in the supplied list only. If fail_on_missing is set to True then
+        a SnapshotBackupException is raised if any of the supplied disks are not found
+        to be attached to the instance.
 
         If the disks parameter is not supplied then this method returns a
         VolumeMetadata object for every disk attached to this instance.
 
         :param str instance_name: The name of the VM instance to which the disks
             are attached.
         :param list[str]|None disks: A list containing the names of disks to be
             backed up.
+        :param bool fail_on_missing: Fail with a SnapshotBackupException if any
+            specified disks are not attached to the instance.
         :rtype: dict[str, VolumeMetadata]
         :return: A dict of VolumeMetadata objects representing each volume
             attached to the instance, keyed by volume identifier.
         """
         instance_metadata = self._get_instance_metadata(instance_name)
         attached_volumes = {}
         for attachment_metadata in instance_metadata.storage_profile.data_disks:
@@ -780,15 +803,15 @@
                 continue
             assert disk_name not in attached_volumes
             disk_metadata = self._get_disk_metadata(disk_name)
             attached_volumes[disk_name] = AzureVolumeMetadata(
                 attachment_metadata, disk_metadata
             )
         # Check all requested disks were found and complain if necessary
-        if disks is not None:
+        if disks is not None and fail_on_missing:
             unattached_disks = []
             for disk_name in disks:
                 if disk_name not in attached_volumes:
                     # Verify the disk definitely exists by fetching the metadata
                     self._get_disk_metadata(disk_name)
                     # Append to list of unattached disks
                     unattached_disks.append(disk_name)
```

### Comparing `barman-3.6.0/barman/cloud_providers/google_cloud_storage.py` & `barman-3.7.0/barman/cloud_providers/google_cloud_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -346,14 +346,34 @@
                 except GoogleAPIError as e:
                     failures[path] = [str(e.__class__), e.__str__()]
 
         if failures:
             logging.error(failures)
             raise CloudProviderError()
 
+    def get_prefixes(self, prefix):
+        """
+        Return only the common prefixes under the supplied prefix.
+
+        :param str prefix: The object key prefix under which the common prefixes
+            will be found.
+        :rtype: Iterator[str]
+        :return: A list of unique prefixes immediately under the supplied prefix.
+        """
+        raise NotImplementedError()
+
+    def delete_under_prefix(self, prefix):
+        """
+        Delete all objects under the specified prefix.
+
+        :param str prefix: The object key prefix under which all objects should be
+            deleted.
+        """
+        raise NotImplementedError()
+
 
 def import_google_cloud_compute():
     """
     Import and return the google.cloud.compute module.
 
     This particular import happens in a function so that it can be deferred until
     needed while still allowing tests to easily mock the library.
@@ -579,32 +599,35 @@
             _logger.info(
                 "Deleting snapshot '%s' for backup %s",
                 snapshot.identifier,
                 backup_info.backup_id,
             )
             self._delete_snapshot(snapshot.identifier)
 
-    def get_attached_volumes(self, instance_name, disks=None):
+    def get_attached_volumes(self, instance_name, disks=None, fail_on_missing=True):
         """
         Returns metadata for the volumes attached to this instance.
 
         Queries GCP for metadata relating to the volumes attached to the named instance
         and returns a dict of `VolumeMetadata` objects, keyed by disk name.
 
         If the optional disks parameter is supplied then this method returns metadata
-        for the disks in the supplied list only. A SnapshotBackupException is raised if
-        any of the supplied disks are not found to be attached to the instance.
+        for the disks in the supplied list only. If fail_on_missing is set to True then
+        a SnapshotBackupException is raised if any of the supplied disks are not found
+        to be attached to the instance.
 
         If the disks parameter is not supplied then this method returns a
         VolumeMetadata for all disks attached to this instance.
 
         :param str instance_name: The name of the VM instance to which the disks
             to be backed up are attached.
         :param list[str]|None disks: A list containing the names of disks to be
             backed up.
+        :param bool fail_on_missing: Fail with a SnapshotBackupException if any
+            specified disks are not attached to the instance.
         :rtype: dict[str, VolumeMetadata]
         :return: A dict of VolumeMetadata objects representing each volume
             attached to the instance, keyed by volume identifier.
         """
         instance_metadata = self._get_instance_metadata(instance_name)
         attached_volumes = {}
         for attachment_metadata in instance_metadata.disks:
@@ -619,15 +642,15 @@
             assert disk_name not in attached_volumes
             disk_metadata = self._get_disk_metadata(disk_name)
             attached_volumes[disk_name] = GcpVolumeMetadata(
                 attachment_metadata,
                 disk_metadata,
             )
         # Check all requested disks were found and complain if necessary
-        if disks is not None:
+        if disks is not None and fail_on_missing:
             unattached_disks = []
             for disk_name in disks:
                 if disk_name not in attached_volumes:
                     # Verify the disk definitely exists by fetching the metadata
                     self._get_disk_metadata(disk_name)
                     # Append to list of unattached disks
                     unattached_disks.append(disk_name)
```

### Comparing `barman-3.6.0/NEWS` & `barman-3.7.0/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 Barman News - History of user-visible changes
 
+Version 3.7.0 - 25 July 2023
+
+- Support is added for snapshot backups on AWS using EBS volumes.
+
+- The `--profile` option in the `barman-cloud-*` scripts is renamed
+  `--aws-profile`. The old name is deprecated and will be removed in
+  a future release.
+
+- Backup manifests can now be generated automatically on completion
+  of a backup made with `backup_method = rsync`. This is enabled by
+  setting the `autogenerate_manifest` configuration variable and can
+  be overridden using the `--manifest` and `--no-manifest` CLI options.
+
+- Bug fixes:
+
+    - The `barman-cloud-*` scripts now correctly use continuation
+      tokens to page through objects in AWS S3-compatible object
+      stores. This fixes a bug where `barman-cloud-backup-delete`
+      would only delete the oldest 1000 eligible WALs after backup
+      deletion.
+
+    - Minor documentation fixes.
+
 Version 3.6.0 - 15 June 2023
 
 - PostgreSQL version 10 is no longer supported.
 
 - Support is added for snapshot backups on Microsoft Azure using
   Managed Disks.
```

### Comparing `barman-3.6.0/setup.py` & `barman-3.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     },
     license="GPL-3.0",
     description=__doc__.split("\n")[0],
     long_description="\n".join(__doc__.split("\n")[2:]),
     install_requires=install_requires,
     extras_require={
         "cloud": ["boto3"],
+        "aws-snapshots": ["boto3"],
         "azure": ["azure-identity", "azure-storage-blob"],
         "azure-snapshots": ["azure-identity", "azure-mgmt-compute"],
         "snappy": ["python-snappy"],
         "google": [
             "google-cloud-storage",
         ],
         "google-snapshots": [
```

### Comparing `barman-3.6.0/PKG-INFO` & `barman-3.7.0/barman.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barman
-Version: 3.6.0
+Version: 3.7.0
 Summary: Backup and Recovery Manager for PostgreSQL
 Home-page: https://www.pgbarman.org/
 Author: EnterpriseDB
 Author-email: barman@enterprisedb.com
 License: GPL-3.0
 Platform: Linux
 Platform: Mac OS X
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cloud
+Provides-Extra: aws-snapshots
 Provides-Extra: azure
 Provides-Extra: azure-snapshots
 Provides-Extra: snappy
 Provides-Extra: google
 Provides-Extra: google-snapshots
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `barman-3.6.0/AUTHORS` & `barman-3.7.0/AUTHORS`

 * *Files identical despite different names*

